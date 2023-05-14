# Comparing `tmp/snakifyer-1.0.2.tar.gz` & `tmp/snakifyer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakifyer-1.0.2.tar", last modified: Sun Jan 15 20:19:51 2023, max compression
+gzip compressed data, was "snakifyer-2.0.0.tar", last modified: Sun May 14 09:07:40 2023, max compression
```

## Comparing `snakifyer-1.0.2.tar` & `snakifyer-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 20:19:51.972037 snakifyer-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-15 20:19:36.000000 snakifyer-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-01-15 20:19:51.972037 snakifyer-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-01-15 20:19:36.000000 snakifyer-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-15 20:19:51.972037 snakifyer-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-01-15 20:19:36.000000 snakifyer-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 20:19:51.968037 snakifyer-1.0.2/snakifyer/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-15 20:19:36.000000 snakifyer-1.0.2/snakifyer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-01-15 20:19:36.000000 snakifyer-1.0.2/snakifyer/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-15 20:19:36.000000 snakifyer-1.0.2/snakifyer/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-01-15 20:19:36.000000 snakifyer-1.0.2/snakifyer/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 20:19:51.972037 snakifyer-1.0.2/snakifyer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-01-15 20:19:51.000000 snakifyer-1.0.2/snakifyer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-01-15 20:19:51.000000 snakifyer-1.0.2/snakifyer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-15 20:19:51.000000 snakifyer-1.0.2/snakifyer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-15 20:19:51.000000 snakifyer-1.0.2/snakifyer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-15 20:19:51.000000 snakifyer-1.0.2/snakifyer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-15 20:19:51.000000 snakifyer-1.0.2/snakifyer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:07:40.700109 snakifyer-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-14 09:07:22.000000 snakifyer-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-14 09:07:40.700109 snakifyer-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-14 09:07:22.000000 snakifyer-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 09:07:40.700109 snakifyer-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-14 09:07:22.000000 snakifyer-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:07:40.700109 snakifyer-2.0.0/snakifyer/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-14 09:07:22.000000 snakifyer-2.0.0/snakifyer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-05-14 09:07:22.000000 snakifyer-2.0.0/snakifyer/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-14 09:07:22.000000 snakifyer-2.0.0/snakifyer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-05-14 09:07:22.000000 snakifyer-2.0.0/snakifyer/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:07:40.700109 snakifyer-2.0.0/snakifyer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-14 09:07:40.000000 snakifyer-2.0.0/snakifyer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-14 09:07:40.000000 snakifyer-2.0.0/snakifyer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:07:40.000000 snakifyer-2.0.0/snakifyer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-14 09:07:40.000000 snakifyer-2.0.0/snakifyer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 09:07:40.000000 snakifyer-2.0.0/snakifyer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 09:07:40.000000 snakifyer-2.0.0/snakifyer.egg-info/top_level.txt
```

### Comparing `snakifyer-1.0.2/LICENSE` & `snakifyer-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snakifyer-1.0.2/PKG-INFO` & `snakifyer-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakifyer
-Version: 1.0.2
+Version: 2.0.0
 Summary: A simple to bot to automate problem submissions on snakify.org 
 Home-page: https://github.com/akashrchandran/snakifyer
 Author: Akash R Chandran
 Author-email: chandranrakash@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,11 +36,19 @@
 ```
 # Usage
 > just run `snakifyer` on your terminal.
 ```
 snakifyer
 ```
 > for first time users it may ask for username and password. You have to share it once and it will get saved locally.
-<hr style="border:2px solid gray">
 
+## Using commandline arguments
+```
+snakifyer -u username -p password
+```
+# Reset config to add new account
+```
+snakifyer -r
+```
+<hr style="border:2px solid gray">
 
 ![image](https://user-images.githubusercontent.com/78685510/212165621-97247489-bf02-4ba8-ac2c-8d4eeaa4b472.png)
```

### Comparing `snakifyer-1.0.2/setup.py` & `snakifyer-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "beautifulsoup4",
     "requests",
     "rich",
 ]
 
 setup(
     name=pkg_name,
-    version="1.0.2",
+    version="2.0.0",
     author="Akash R Chandran",
     author_email="chandranrakash@gmail.com",
     description="A simple to bot to automate problem submissions on snakify.org ",
     long_description=read_file("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/akashrchandran/snakifyer",
     install_requires=requirements,
```

### Comparing `snakifyer-1.0.2/snakifyer/api.py` & `snakifyer-2.0.0/snakifyer/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -80,8 +80,33 @@
         return [
             {
                 'name': link.text,
                 'link': link['href'],
                 'slug': link['href'].split('/')[-2],
             }
             for link in links
+        ]
+    
+    def get_all_sections(self):
+        url = "https://snakify.org/en/"
+        req = self.session.get(url)
+        soup = BeautifulSoup(req.text, 'html.parser')
+        links = soup.find(class_ = "nav nav-sidebar").find_all('li')
+        return {
+            link.get_text(strip=True): link.find('a')['href'].split('/')[-2]
+            for link in links
+        }
+    
+    def get_all_problems_in_section(self, section):
+        url = f"https://snakify.org/en/lessons/{section}/"
+        req = self.session.get(url)
+        print(req)
+        soup = BeautifulSoup(req.text, 'html.parser')
+        links = soup.find_all(class_ = "problem-available")
+        return [
+            {
+                'name': link.get_text(strip=True),
+                'link': link.find('a')['href'],
+                'slug': link.find('a')['href'].split('/')[-2],
+            }
+            for link in links
         ]
```

### Comparing `snakifyer-1.0.2/snakifyer/cli.py` & `snakifyer-2.0.0/snakifyer/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 CONFIG_PATH = os.path.join(OS_CONFIG, "snakifyer")
 CONFIG_FILE = os.path.join(CONFIG_PATH, "config.json")
 
 parser = argparse.ArgumentParser()
 
 parser.add_argument("-u",
                     "--username",
-                    metavar="USERNAME",
-                    help='username of snakify account.'
+                    metavar="Email",
+                    help='email of snakify account.'
                     )
 
 parser.add_argument("-p",
                     "--password",
                     metavar="PASSWORD",
-                    help='skip check for if it already downloaded and is available in directory. '
+                    help='password of snakify account.'
                     )
 
 parser.add_argument("-r",
                     "--reset",
                     nargs='?',
                     const=True,
                     help="reset config to add new account.",
                     choices=[True, False],
                     )
 
 def parse_cmd(config):
     args = parser.parse_args()
     if args.username:
-        config['username'] = args.username
+        config['email'] = args.username
     if args.password:
         config['password'] = args.password
     if args.reset:
         reset_config()
```

### Comparing `snakifyer-1.0.2/snakifyer.egg-info/PKG-INFO` & `snakifyer-2.0.0/snakifyer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakifyer
-Version: 1.0.2
+Version: 2.0.0
 Summary: A simple to bot to automate problem submissions on snakify.org 
 Home-page: https://github.com/akashrchandran/snakifyer
 Author: Akash R Chandran
 Author-email: chandranrakash@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,11 +36,19 @@
 ```
 # Usage
 > just run `snakifyer` on your terminal.
 ```
 snakifyer
 ```
 > for first time users it may ask for username and password. You have to share it once and it will get saved locally.
-<hr style="border:2px solid gray">
 
+## Using commandline arguments
+```
+snakifyer -u username -p password
+```
+# Reset config to add new account
+```
+snakifyer -r
+```
+<hr style="border:2px solid gray">
 
 ![image](https://user-images.githubusercontent.com/78685510/212165621-97247489-bf02-4ba8-ac2c-8d4eeaa4b472.png)
```

