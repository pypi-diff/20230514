# Comparing `tmp/backup_github-1.0.0.tar.gz` & `tmp/backup_github-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backup_github-1.0.0.tar", max compression
+gzip compressed data, was "backup_github-1.1.0.tar", max compression
```

## Comparing `backup_github-1.0.0.tar` & `backup_github-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     3087 2023-02-18 21:23:32.779249 backup_github-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-02-18 21:23:32.779249 backup_github-1.0.0/backup_github/__init__.py
--rw-r--r--   0        0        0    10635 2023-02-18 21:23:32.779249 backup_github-1.0.0/backup_github/backup.py
--rw-r--r--   0        0        0     6284 2023-02-18 21:23:32.779249 backup_github-1.0.0/backup_github/github.py
--rw-r--r--   0        0        0      761 2023-02-18 21:23:32.779249 backup_github-1.0.0/backup_github/main.py
--rw-r--r--   0        0        0     1013 2023-02-18 21:23:32.779249 backup_github-1.0.0/backup_github/parse_args.py
--rw-r--r--   0        0        0      594 2023-02-18 21:23:32.779249 backup_github-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3954 1970-01-01 00:00:00.000000 backup_github-1.0.0/setup.py
--rw-r--r--   0        0        0     3536 1970-01-01 00:00:00.000000 backup_github-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3351 2023-05-14 20:38:44.668626 backup_github-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-14 20:38:44.668626 backup_github-1.1.0/backup_github/__init__.py
+-rw-r--r--   0        0        0     8303 2023-05-14 20:38:44.668626 backup_github-1.1.0/backup_github/backup.py
+-rw-r--r--   0        0        0     6182 2023-05-14 20:38:44.668626 backup_github-1.1.0/backup_github/github.py
+-rw-r--r--   0        0        0     1801 2023-05-14 20:38:44.668626 backup_github-1.1.0/backup_github/main.py
+-rw-r--r--   0        0        0      495 2023-05-14 20:38:44.668626 backup_github-1.1.0/backup_github/metrics.py
+-rw-r--r--   0        0        0     1611 2023-05-14 20:38:44.668626 backup_github-1.1.0/backup_github/parse_args.py
+-rw-r--r--   0        0        0      910 2023-05-14 20:38:44.668626 backup_github-1.1.0/backup_github/utils.py
+-rw-r--r--   0        0        0      594 2023-05-14 20:38:44.672626 backup_github-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4217 1970-01-01 00:00:00.000000 backup_github-1.1.0/setup.py
+-rw-r--r--   0        0        0     3800 1970-01-01 00:00:00.000000 backup_github-1.1.0/PKG-INFO
```

### Comparing `backup_github-1.0.0/backup_github/github.py` & `backup_github-1.1.0/backup_github/github.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,33 +26,34 @@
     class ServerError(Exception):
         def __init__(self, message=None):
             self.message = message
             super().__init__(self.message)
 
     def raise_by_status(self, response):
         if response.status_code == 403:
-            logging.info("Status is 403 - Rate limit exceeded exception")
+            logging.warning("Status is 403 - Rate limit exceeded exception")
             raise self.RateLimitExceededException(
                 json.loads(response.content)["message"]
             )
         elif response.status_code == 404:
-            logging.info(f"Status is {response.status_code} - Client error: Not found")
+            logging.warning(
+                f"Status is {response.status_code} - Client error: Not found"
+            )
             raise self.ClientError(json.loads(response.content)["message"])
         elif 400 <= response.status_code < 500:
-            logging.info(f"Status is {response.status_code} - Client error")
+            logging.warning(f"Status is {response.status_code} - Client error")
             raise self.ClientError(json.loads(response.content)["message"])
         elif 500 <= response.status_code < 600:
-            logging.info(f"Status is {response.status_code} - Server error")
+            logging.warning(f"Status is {response.status_code} - Server error")
             raise self.ServerError(json.loads(response.content)["message"])
 
     def retry(func):
         def ret(self, *args, **kwargs):
             for _ in range(self.retry_count + 1):
                 try:
-                    time.sleep(1)
                     return func(self, *args, **kwargs)
                 except self.RateLimitExceededException:
                     logging.warning("Rate limit exceeded")
                     limit = self.get_rate_limit()
                     reset = limit["reset"]
                     seconds = max(
                         self.retry_seconds, reset - time.time() + self.retry_seconds
@@ -77,108 +78,89 @@
         return ret
 
     def __init__(
         self, token, organization, output_dir, retry_count=10, retry_seconds=1
     ):
         self.headers = {
             "Accept": "application/vnd.github+json",
-            "Authorization": "Bearer " + token,
+            "Authorization": f"Bearer {token}",
         }
         self.token = token
         self.organization = organization
         self.output_dir = output_dir
         self.retry_count = retry_count
         self.retry_seconds = retry_seconds
 
     @retry
-    def make_request(self, url, params=None):
-        resp = requests.get(url, headers=self.headers, params=params)
-        logging.info(f"Make request to {url}")
-        self.raise_by_status(resp)
-        logging.info("OK")
-        return resp.json()
+    def make_request(self, url, params={}):
+        res = []
+        params["page"] = 1
+        params["per_page"] = 100
+        while True:
+            resp = requests.get(url, headers=self.headers, params=params)
+            logging.debug(f"Make request to {url}")
+            self.raise_by_status(resp)
+            logging.debug("OK")
+            if isinstance(resp.json(), list):
+                res += resp.json()
+            else:
+                return resp.json()
+            if len(resp.json()) == 0:
+                break
+            params["page"] = params["page"] + 1
+        return res
 
     def get_organization(self):
-        return self.make_request("https://api.github.com/orgs/" + self.organization)
+        return self.make_request(f"https://api.github.com/orgs/{self.organization}")
 
     def get_members(self):
         return self.make_request(
-            "https://api.github.com/orgs/" + self.organization + "/members"
+            f"https://api.github.com/orgs/{self.organization}/members"
         )
 
     def get_member_status(self, member_login):
         return self.make_request(
-            "https://api.github.com/orgs/"
-            + self.organization
-            + "/memberships/"
-            + member_login
+            f"https://api.github.com/orgs/{self.organization}/memberships/{member_login}"
         )
 
     def get_repo(self, repo_name):
         return self.make_request(
-            "https://api.github.com/repos/" + self.organization + "/" + repo_name
+            f"https://api.github.com/repos/{self.organization}/{repo_name}"
         )
 
     def get_issues(self, repo_name):
         return self.make_request(
-            "https://api.github.com/repos/"
-            + self.organization
-            + "/"
-            + repo_name
-            + "/issues",
+            f"https://api.github.com/repos/{self.organization}/{repo_name}/issues",
             {"state": "all"},
         )
 
     def get_pulls(self, repo_name):
         return self.make_request(
-            "https://api.github.com/repos/"
-            + self.organization
-            + "/"
-            + repo_name
-            + "/pulls",
+            f"https://api.github.com/repos/{self.organization}/{repo_name}/pulls",
             {"state": "all"},
         )
 
     def get_comments_for_issue(self, repo_name, issue_number):
         return self.make_request(
-            "https://api.github.com/repos/"
-            + self.organization
-            + "/"
-            + repo_name
-            + "/issues/"
-            + str(issue_number)
-            + "/comments"
+            f"https://api.github.com/repos/{self.organization}/{repo_name}/issues/{str(issue_number)}/comments"
         )
 
     def get_reviews(self, repo_name, pull_number):
         return self.make_request(
-            "https://api.github.com/repos/"
-            + self.organization
-            + "/"
-            + repo_name
-            + "/pulls/"
-            + str(pull_number)
-            + "/reviews"
+            f"https://api.github.com/repos/{self.organization}/{repo_name}/pulls/{str(pull_number)}/reviews"
         )
 
     def get_comments_for_review(self, repo_name, pull_number, review_id):
         return self.make_request(
-            "https://api.github.com/repos/"
-            + self.organization
-            + "/"
-            + repo_name
-            + "/pulls/"
-            + str(pull_number)
-            + "/reviews/"
-            + str(review_id)
-            + "/comments"
+            f"https://api.github.com/repos/{self.organization}/{repo_name}/pulls/"
+            f"{str(pull_number)}/reviews/{str(review_id)}/comments"
         )
 
     def get_repositories(self):
         return self.make_request(
-            "https://api.github.com/orgs/" + self.organization + "/repos"
+            f"https://api.github.com/orgs/{self.organization}/repos"
         )
 
     def get_rate_limit(self):
         return self.make_request("https://api.github.com/rate_limit")["resources"][
             "core"
         ]
```

### Comparing `backup_github-1.0.0/backup_github/parse_args.py` & `backup_github-1.1.0/backup_github/parse_args.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,9 +32,36 @@
         "-r",
         "--repository",
         nargs="+",
         default=None,
         dest="repository",
         help="name of repositories to limit backup",
     )
+    parser.add_argument(
+        "-i",
+        "--issues",
+        action="store_true",
+        dest="issues",
+        help="run backup of issues",
+    )
+    parser.add_argument(
+        "-p",
+        "--pulls",
+        action="store_true",
+        dest="pulls",
+        help="run backup of pulls",
+    )
+    parser.add_argument(
+        "-m",
+        "--members",
+        action="store_true",
+        dest="members",
+        help="run backup of members",
+    )
+    parser.add_argument(
+        "--all",
+        action="store_true",
+        dest="all",
+        help="run backup of all data",
+    )
     parsed = parser.parse_args(args)
     return parsed
```

### Comparing `backup_github-1.0.0/pyproject.toml` & `backup_github-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "backup-github"
-version = "1.0.0"
+version = "1.1.0"
 description = ""
 authors = ["Karina5005 <karinaanisimova23062001@gmail.com>"]
 readme = "README.md"
 packages = [{include = "backup_github"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `backup_github-1.0.0/setup.py` & `backup_github-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['prometheus_client>=0.16.0,<0.17.0', 'requests>=2.28.2,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['backup-github = backup_github.main:main']}
 
 setup_kwargs = {
     'name': 'backup-github',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': '',
-    'long_description': '# GitHub-Backup\n\n## Project description\n\nApplication for backing up information about a GitHub organization\n\n## Installation\n\nYou can clone this repository and set up the environment directly from the command line using the following command:\n\n```bash\ngit clone git@github.com:cloud-labs-infra/github-backup.git\ncd github-backup\nmake env\nexport PYTHONPATH=$PYTHONPATH:$PWD/github_backup\n```\n\n## Testing\n\nYou can run the tests using the following command:\n\n```bash\nmake test\n```\n\nThis command runs all unit tests and calculates coverage\n\n## Usage\n\nCLI Usage is as follows:\n\n    ./venv/bin/python github_backup/main.py [-h] [-t TOKEN] [-o OUTPUT_DIR]\n               [-r REPOSITORY [REPOSITORY ...]]\n               ORGANIZATION_NAME\n\n    Backup a GitHub organization\n    \n    positional arguments:\n      ORGANIZATION_NAME                     github organization name\n    \n    options:\n      -h, --help                            show this help message and exit\n      -t TOKEN, --token TOKEN\n                                            personal token\n      -o OUTPUT_DIR, --output-directory OUTPUT_DIR\n                                            directory for backup\n      -r REPOSITORY [REPOSITORY ...], --repository REPOSITORY [REPOSITORY ...]\n                                            name of repositories to limit backup\n\n\n## Backup structure\n\n    .\n    └── organization\n        ├── members\n        │ └── login1\n        │     ├── member.json\n        │     └── membership.json\n        └── repos\n            └── repo1\n                ├── content\n                │ └── repo1.git\n                ├── issues\n                │ └── 1\n                │     ├── assignee.json\n                │     ├── comments\n                │     ├── issue.json\n                │     └── user.json\n                ├── pulls\n                │ └── 2\n                │     ├── assignee.json\n                │     ├── base.json\n                │     ├── comments\n                │     │ └── 1\n                │     │     ├── comment.json\n                │     │     └── user.json\n                │     ├── head.json\n                │     ├── pull.json\n                │     ├── reviews\n                │     │ ├── 1\n                │     │ │   ├── review.json\n                │     │ │   └── user.json\n                │     │ └── 2\n                │     │     ├── comments\n                │     │     │ └── 1\n                │     │     │     ├── comment.json\n                │     │     │     └── user.json\n                │     │     ├── review.json\n                │     │     └── user.json\n                │     └── user.json\n                └── repo.json\n\n## License\n\n[MIT](https://choosealicense.com/licenses/mit/)\n\n## Project status\n\nThe project is currently in a development state',
+    'long_description': '# GitHub-Backup\n\n## Project description\n\nApplication for backing up information about a GitHub organization\n\n## Installation\n\nYou can clone this repository and set up the environment directly from the command line using the following command:\n\n```bash\ngit clone git@github.com:cloud-labs-infra/github-backup.git\ncd github-backup\npoetry install\n```\n\n## Testing\n\nYou can run the tests using the following command:\n\n```bash\npoetry run pytest --cov=./ --cov-report=xml\n```\n\nThis command runs all unit tests and calculates coverage\n\n## Usage\n\nCLI Usage is as follows:\n\n    poetry run backup-github [-h] [-t TOKEN] [-o OUTPUT_DIR] [-r REPOSITORY [REPOSITORY ...]] [-i] [-p] [-m]\n                                               [--all]\n                                               ORGANIZATION_NAME\n\n    Backup a GitHub organization\n    \n    positional arguments:\n      ORGANIZATION_NAME                     github organization name\n    \n    options:\n      -h, --help                            show this help message and exit\n      -t TOKEN, --token TOKEN\n                                            personal token\n      -o OUTPUT_DIR, --output-directory OUTPUT_DIR\n                                            directory for backup\n      -r REPOSITORY [REPOSITORY ...], --repository REPOSITORY [REPOSITORY ...]\n                                            name of repositories to limit backup\n      -i, --issues                          run backup of issues\n      -p, --pulls                           run backup of pulls\n      -m, --members                         run backup of members\n      --all                                 run backup of all data\n\n\n## Backup structure\n\n    .\n    └── organization\n        ├── members\n        │ └── login1\n        │     ├── member.json\n        │     └── membership.json\n        └── repos\n            └── repo1\n                ├── content\n                │ └── repo1.git\n                ├── issues\n                │ └── 1\n                │     ├── assignee.json\n                │     ├── comments\n                │     ├── issue.json\n                │     └── user.json\n                ├── pulls\n                │ └── 2\n                │     ├── assignee.json\n                │     ├── base.json\n                │     ├── comments\n                │     │ └── 1\n                │     │     ├── comment.json\n                │     │     └── user.json\n                │     ├── head.json\n                │     ├── pull.json\n                │     ├── reviews\n                │     │ ├── 1\n                │     │ │   ├── review.json\n                │     │ │   └── user.json\n                │     │ └── 2\n                │     │     ├── comments\n                │     │     │ └── 1\n                │     │     │     ├── comment.json\n                │     │     │     └── user.json\n                │     │     ├── review.json\n                │     │     └── user.json\n                │     └── user.json\n                └── repo.json\n\n## Project status\n\nThe project is currently in a development state',
     'author': 'Karina5005',
     'author_email': 'karinaanisimova23062001@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `backup_github-1.0.0/PKG-INFO` & `backup_github-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,58 @@
-Metadata-Version: 2.1
-Name: backup-github
-Version: 1.0.0
-Summary: 
-Author: Karina5005
-Author-email: karinaanisimova23062001@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: prometheus_client (>=0.16.0,<0.17.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Description-Content-Type: text/markdown
-
 # GitHub-Backup
 
 ## Project description
 
 Application for backing up information about a GitHub organization
 
 ## Installation
 
 You can clone this repository and set up the environment directly from the command line using the following command:
 
 ```bash
 git clone git@github.com:cloud-labs-infra/github-backup.git
 cd github-backup
-make env
-export PYTHONPATH=$PYTHONPATH:$PWD/github_backup
+poetry install
 ```
 
 ## Testing
 
 You can run the tests using the following command:
 
 ```bash
-make test
+poetry run pytest --cov=./ --cov-report=xml
 ```
 
 This command runs all unit tests and calculates coverage
 
 ## Usage
 
 CLI Usage is as follows:
 
-    ./venv/bin/python github_backup/main.py [-h] [-t TOKEN] [-o OUTPUT_DIR]
-               [-r REPOSITORY [REPOSITORY ...]]
-               ORGANIZATION_NAME
+    poetry run backup-github [-h] [-t TOKEN] [-o OUTPUT_DIR] [-r REPOSITORY [REPOSITORY ...]] [-i] [-p] [-m]
+                                               [--all]
+                                               ORGANIZATION_NAME
 
     Backup a GitHub organization
     
     positional arguments:
       ORGANIZATION_NAME                     github organization name
     
     options:
       -h, --help                            show this help message and exit
       -t TOKEN, --token TOKEN
                                             personal token
       -o OUTPUT_DIR, --output-directory OUTPUT_DIR
                                             directory for backup
       -r REPOSITORY [REPOSITORY ...], --repository REPOSITORY [REPOSITORY ...]
                                             name of repositories to limit backup
+      -i, --issues                          run backup of issues
+      -p, --pulls                           run backup of pulls
+      -m, --members                         run backup of members
+      --all                                 run backup of all data
 
 
 ## Backup structure
 
     .
     └── organization
         ├── members
@@ -100,14 +89,10 @@
                 │     │     │     ├── comment.json
                 │     │     │     └── user.json
                 │     │     ├── review.json
                 │     │     └── user.json
                 │     └── user.json
                 └── repo.json
 
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
-
 ## Project status
 
-The project is currently in a development state
+The project is currently in a development state
```

