# Comparing `tmp/stb_mnt-4.5.3.tar.gz` & `tmp/stb_mnt-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stb_mnt-4.5.3.tar", max compression
+gzip compressed data, was "stb_mnt-4.6.0.tar", max compression
```

## Comparing `stb_mnt-4.5.3.tar` & `stb_mnt-4.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2023-01-09 22:18:45.026759 stb_mnt-4.5.3/LICENSE
--rw-r--r--   0        0        0     4275 2023-05-12 12:46:48.810016 stb_mnt-4.5.3/README.md
--rw-r--r--   0        0        0     1329 2023-05-12 13:25:40.840047 stb_mnt-4.5.3/pyproject.toml
--rw-r--r--   0        0        0       69 2023-01-09 19:47:55.893082 stb_mnt-4.5.3/stb/__init__.py
--rw-r--r--   0        0        0     2702 2023-02-17 18:43:44.943340 stb_mnt-4.5.3/stb/__main__.py
--rw-r--r--   0        0        0       79 2023-01-09 22:02:40.485385 stb_mnt-4.5.3/stb/__version__.py
--rw-r--r--   0        0        0     7339 2023-03-12 18:54:33.634270 stb_mnt-4.5.3/stb/config.py
--rw-r--r--   0        0        0     5389 2023-01-24 13:50:32.276659 stb_mnt-4.5.3/stb/db.py
--rw-r--r--   0        0        0     3966 2023-02-21 18:34:18.607097 stb_mnt-4.5.3/stb/graph.py
--rw-r--r--   0        0        0        0 2022-09-25 11:30:34.799917 stb_mnt-4.5.3/stb/py.typed
--rw-r--r--   0        0        0      813 2023-02-23 20:17:01.377182 stb_mnt-4.5.3/stb/run.py
--rw-r--r--   0        0        0     6005 2023-05-12 13:12:28.356703 stb_mnt-4.5.3/stb/setup.py
--rwxr-xr-x   0        0        0     6365 2023-01-26 09:29:16.979999 stb_mnt-4.5.3/stb/update.py
--rw-r--r--   0        0        0     3251 2023-05-12 13:11:06.760035 stb_mnt-4.5.3/stb/use.py
--rw-r--r--   0        0        0        0 2023-01-24 13:47:27.999993 stb_mnt-4.5.3/stb/utils/__init__.py
--rw-r--r--   0        0        0     4852 2023-01-24 20:56:14.909999 stb_mnt-4.5.3/stb/utils/common.py
--rw-r--r--   0        0        0     2725 2023-01-24 20:22:14.616666 stb_mnt-4.5.3/stb/utils/dependency_parser.py
--rw-r--r--   0        0        0     5485 1970-01-01 00:00:00.000000 stb_mnt-4.5.3/setup.py
--rw-r--r--   0        0        0     5327 1970-01-01 00:00:00.000000 stb_mnt-4.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-01-09 22:18:45.026759 stb_mnt-4.6.0/LICENSE
+-rw-r--r--   0        0        0     4275 2023-05-12 12:46:48.810016 stb_mnt-4.6.0/README.md
+-rw-r--r--   0        0        0     1329 2023-05-14 14:09:27.894369 stb_mnt-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-01-09 19:47:55.893082 stb_mnt-4.6.0/stb/__init__.py
+-rw-r--r--   0        0        0     2702 2023-02-17 18:43:44.943340 stb_mnt-4.6.0/stb/__main__.py
+-rw-r--r--   0        0        0       79 2023-01-09 22:02:40.485385 stb_mnt-4.6.0/stb/__version__.py
+-rw-r--r--   0        0        0     7339 2023-03-12 18:54:33.634270 stb_mnt-4.6.0/stb/config.py
+-rw-r--r--   0        0        0     5465 2023-05-14 14:09:17.597759 stb_mnt-4.6.0/stb/db.py
+-rw-r--r--   0        0        0     3966 2023-02-21 18:34:18.607097 stb_mnt-4.6.0/stb/graph.py
+-rw-r--r--   0        0        0        0 2022-09-25 11:30:34.799917 stb_mnt-4.6.0/stb/py.typed
+-rw-r--r--   0        0        0      813 2023-02-23 20:17:01.377182 stb_mnt-4.6.0/stb/run.py
+-rw-r--r--   0        0        0     6005 2023-05-12 13:12:28.356703 stb_mnt-4.6.0/stb/setup.py
+-rwxr-xr-x   0        0        0     6365 2023-01-26 09:29:16.979999 stb_mnt-4.6.0/stb/update.py
+-rw-r--r--   0        0        0     3251 2023-05-12 13:11:06.760035 stb_mnt-4.6.0/stb/use.py
+-rw-r--r--   0        0        0        0 2023-01-24 13:47:27.999993 stb_mnt-4.6.0/stb/utils/__init__.py
+-rw-r--r--   0        0        0     4852 2023-01-24 20:56:14.909999 stb_mnt-4.6.0/stb/utils/common.py
+-rw-r--r--   0        0        0     2725 2023-01-24 20:22:14.616666 stb_mnt-4.6.0/stb/utils/dependency_parser.py
+-rw-r--r--   0        0        0     5485 1970-01-01 00:00:00.000000 stb_mnt-4.6.0/setup.py
+-rw-r--r--   0        0        0     5327 1970-01-01 00:00:00.000000 stb_mnt-4.6.0/PKG-INFO
```

### Comparing `stb_mnt-4.5.3/LICENSE` & `stb_mnt-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.3/README.md` & `stb_mnt-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.3/pyproject.toml` & `stb_mnt-4.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "stb-mnt"
 packages = [{ include = "stb" }]
-version = "4.5.3"
+version = "4.6.0"
 description = "A universal tool for local microservice management."
 readme = "README.md"
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
 ]
```

### Comparing `stb_mnt-4.5.3/stb/__main__.py` & `stb_mnt-4.6.0/stb/__main__.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.3/stb/config.py` & `stb_mnt-4.6.0/stb/config.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.3/stb/db.py` & `stb_mnt-4.6.0/stb/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         )
 
 
 app = typer.Typer(
     name="migrator",
     help="creates/upgrades/drops dbs for microservices",
 )
-REQUIRED_DOTENV_KEYS = "POSTGRES_PASSWORD", "POSTGRES_PORT", "POSTGRES_USER"
+REQUIRED_DOTENV_KEYS = "POSTGRES_PASSWORD", "POSTGRES_USER"
 OLD_PARALLEL_MIGRATIONS_ARG = typer.Option(
     False,
     "-p",
     "--parallel",
     help="Deprecated. This behavior is now the default. If you want to disable it, use --no-parallel.",
     callback=old_parallel_flag_deprecation_callback,
 )
@@ -110,18 +110,20 @@
     command: Choices,
     parallel_migrations: bool = False,
     force_drop: bool = False,
 ) -> None:
     service = get_service(service_path)
 
     for field in REQUIRED_DOTENV_KEYS:
-        if not service.dotenv.get(field):
+        if field not in service.dotenv:
             err = f"{field} field is required for the correct functioning of stb db but it was not filled out in {service.dotenv_path}"
             typer.echo(err, err=True)
             raise LookupError(err)
+    if not "POSTGRES_PORT" in service.dotenv:
+        service.dotenv["POSTGRES_PORT"] = "5432"
 
     aerich_apps = find_aerich_apps(service)
     postgres_dbs = {v for k, v in service.dotenv.items() if k.startswith("POSTGRES_DB")}
     postgres_user = service.dotenv["POSTGRES_USER"]
     postgres_password = cast(str, service.dotenv["POSTGRES_PASSWORD"])
     postgres_port = service.dotenv["POSTGRES_PORT"]
```

### Comparing `stb_mnt-4.5.3/stb/graph.py` & `stb_mnt-4.6.0/stb/graph.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.3/stb/run.py` & `stb_mnt-4.6.0/stb/run.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.3/stb/setup.py` & `stb_mnt-4.6.0/stb/setup.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.3/stb/update.py` & `stb_mnt-4.6.0/stb/update.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.3/stb/use.py` & `stb_mnt-4.6.0/stb/use.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.3/stb/utils/common.py` & `stb_mnt-4.6.0/stb/utils/common.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.3/stb/utils/dependency_parser.py` & `stb_mnt-4.6.0/stb/utils/dependency_parser.py`

 * *Files identical despite different names*

### Comparing `stb_mnt-4.5.3/setup.py` & `stb_mnt-4.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'typing-extensions>=4.3.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['stb = stb:app']}
 
 setup_kwargs = {
     'name': 'stb-mnt',
-    'version': '4.5.3',
+    'version': '4.6.0',
     'description': 'A universal tool for local microservice management.',
     'long_description': '# stb\n\nA universal tool for local microservice management\n\n## Requirements\n\n* [Poetry](https://python-poetry.org/) - Required for setup functionality \n* [Pyenv](https://github.com/pyenv/pyenv) - Optional\n\n## Installation\n\n```bash\npipx install stb-mnt\n```\n\n## Usage\n\n### Setup\n\n* To download and setup my_company/backend/service1 microservice as a subdirectory to the current working directory, use:\n\n```bash\nstb setup my_company/backend/service1\n```\n\n* To download and setup my_company/backend/service1 and my_company/backend/service2 as subdirectories to current working directory, use:\n\n```bash\nstb setup my_company/backend/service1 my_company/backend/service2\n```\n\n* To setup all backend services, use:\n\n```bash\nstb setup my_company/backend\n```\n\nNote that if you want to clone repositories, you must first set a `git_url` using `stb config set git_url` command\n\n### Update\n\n* To update .env file in accordance with .env.example in a microservice:\n\n```bash\nstb update env\n```\n\n* To synchronize service ports between all installed microservices (you can specify which ones will run locally with the `--local` option):\n\n```bash\nstb update ports\n```\n\n* To update poetry.lock file, install dependencies, stash current changes, checkout to master, pull from remote, and recreate databases:\n\n```bash\nstb update package -piucd\n```\n\nor  \n\n```bash\nstb update package --pull --update --checkout --reset-databases\n```\n\n### DB\n\n* To upgrade migrations in a microservice:\n\n```bash\nstb db upgrade\n```\n\n* To create databases and upgrade its migrations in a microservice:\n\n```bash\nstb db create\n```\n\n* To drop databases in a microservice:\n\n```bash\nstb db drop\n```\n\n* To drop and recreate databases, and upgrade migrations in a microservice:\n\n```bash\nstb db reset\n```\n\n* To upgrade migrations in parallel for faster upgrades (useful for large monoliths with multiple databases), you can use the -p (--parallel) option:\n\n```bash\nstb db create -p\n```\n  \n```bash\nstb db reset -p\n```\n  \n* To force dropping of databases in case another program is using them at the same time, you can use the -f (--force) option:\n\n```bash\nstb db drop -f\n```\n  \n```bash\nstb db reset -f\n```\n  \n### Use\n\n`stb use` allows you to take a company private package and install either a cloud version or a local version of it. STB will preserve all extras, automatically set package source, and will gracefully handle any issues that might happen while updating.\n\n* To install a local version of `my_package` that is located at `../my_package`:\n\n```bash\nstb use ../my_package\n```\n\n* To install a local version of `my_package` that is located at `../my_package` in editable mode:\n\n```bash\nstb use ../my_package --editable\n```\n\n* To install a cloud version of `my_package` with tag `8.3.1`:\n\n```bash\nstb use "my_package==8.3.1"\n```\n\n* To install a cloud version of my_package with tag `8.3.1`, my_other_package with any tag higher than `1.2.3`, and my_third_package with any tag more than or equal to `4.5.6` and less than `5.0.0`:\n\n```bash\nstb use "my_package==8.3.1" "my_other_package>1.2.3" "my_third_package^4.5.6"\n```\n\n### Run\n\n* To update and run the select services concurrently:\n\n```bash\nstb run service1 service2\n```\n\n### Config\n\n* To set a git url for cloning:\n\n```bash\nstb config set git_url git@gitlab.my_company.com\n```\n\n### Graph\n\n* To get a dependency graph of your microservices:\n\n```bash\nstb graph json my_company/backend/ my_company/infrastructure/\n```\n\n* To get a dependency graph of your microservices as an svg image (requires graphviz):\n\n```bash\nstb graph graphviz my_company/backend/ my_company/infrastructure/\n```\n\n### How directories are selected for update/db\n\nFor every update, you can specify:\n\n1) A microservice directory, which will cause stb to update only that microservice\n2) Several microservice directories, which will cause stb to update these microservices and integrate them together (for example, `update ports` assigns ports to local microservices and updates their links in other microservices to match the assigned ports)\n3) A directory with multiple microservice subdirectories inside it, which is equivalent to (2) with the list of subdirectories as arguments\n4) Nothing, which will choose the current working directory as the first argument and will be equivalent to (1) or (3)\n',
     'author': 'Stanislav Zmiev',
     'author_email': 'szmiev2000@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `stb_mnt-4.5.3/PKG-INFO` & `stb_mnt-4.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stb-mnt
-Version: 4.5.3
+Version: 4.6.0
 Summary: A universal tool for local microservice management.
 Author: Stanislav Zmiev
 Author-email: szmiev2000@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

