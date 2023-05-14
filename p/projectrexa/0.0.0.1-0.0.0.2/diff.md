# Comparing `tmp/projectrexa-0.0.0.1.tar.gz` & `tmp/projectrexa-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projectrexa-0.0.0.1.tar", last modified: Sun May 14 14:30:17 2023, max compression
+gzip compressed data, was "projectrexa-0.0.0.2.tar", last modified: Sun May 14 15:51:40 2023, max compression
```

## Comparing `projectrexa-0.0.0.1.tar` & `projectrexa-0.0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 14:30:17.538341 projectrexa-0.0.0.1/
--rw-rw-rw-   0        0        0      934 2023-05-14 14:30:17.539339 projectrexa-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      497 2023-05-14 13:48:30.000000 projectrexa-0.0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 14:30:17.536336 projectrexa-0.0.0.1/projectrexa.egg-info/
--rw-rw-rw-   0        0        0      934 2023-05-14 14:30:17.000000 projectrexa-0.0.0.1/projectrexa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-14 14:30:17.000000 projectrexa-0.0.0.1/projectrexa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 14:30:17.000000 projectrexa-0.0.0.1/projectrexa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-05-14 14:30:17.000000 projectrexa-0.0.0.1/projectrexa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 14:30:17.000000 projectrexa-0.0.0.1/projectrexa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-05-14 13:43:02.000000 projectrexa-0.0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-05-14 14:30:17.542345 projectrexa-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1436 2023-05-14 14:29:01.000000 projectrexa-0.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 15:51:40.861869 projectrexa-0.0.0.2/
+-rw-rw-rw-   0        0        0      934 2023-05-14 15:51:40.861869 projectrexa-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2023-05-14 13:48:30.000000 projectrexa-0.0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 15:51:40.859871 projectrexa-0.0.0.2/projectrexa.egg-info/
+-rw-rw-rw-   0        0        0      934 2023-05-14 15:51:36.000000 projectrexa-0.0.0.2/projectrexa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-14 15:51:36.000000 projectrexa-0.0.0.2/projectrexa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 15:51:36.000000 projectrexa-0.0.0.2/projectrexa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-14 15:51:36.000000 projectrexa-0.0.0.2/projectrexa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 15:51:36.000000 projectrexa-0.0.0.2/projectrexa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-05-14 13:43:02.000000 projectrexa-0.0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-05-14 15:51:40.923711 projectrexa-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1429 2023-05-14 15:50:56.000000 projectrexa-0.0.0.2/setup.py
```

### Comparing `projectrexa-0.0.0.1/PKG-INFO` & `projectrexa-0.0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: projectrexa
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: A library to make it easier to use ProjectRexa SSO.
 Home-page: https://projectrexa.ml
-Download-URL: https://github.com/Om-Mishra7/ProjectRexa-PyPI/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/Om-Mishra7/ProjectRexa-PyPI/archive/refs/tags/v_02.tar.gz
 Author: ProjectRexa
 Author-email: admin@projectrexa.ml
 License: MIT
 Keywords: ProjectRexa
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
```

### Comparing `projectrexa-0.0.0.1/projectrexa.egg-info/PKG-INFO` & `projectrexa-0.0.0.2/projectrexa.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: projectrexa
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: A library to make it easier to use ProjectRexa SSO.
 Home-page: https://projectrexa.ml
-Download-URL: https://github.com/Om-Mishra7/ProjectRexa-PyPI/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/Om-Mishra7/ProjectRexa-PyPI/archive/refs/tags/v_02.tar.gz
 Author: ProjectRexa
 Author-email: admin@projectrexa.ml
 License: MIT
 Keywords: ProjectRexa
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
```

### Comparing `projectrexa-0.0.0.1/setup.py` & `projectrexa-0.0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Project name: 
 name='projectrexa',
 
 # Packages to include in the distribution: 
 packages=find_packages(','),
 
 # Project version number:
-version='0.0.0.1',
+version='0.0.0.2',
 
 # List a license for the project, eg. MIT License
 license='MIT',
 
 # Short description of your library: 
 description='A library to make it easier to use ProjectRexa SSO.',
 
@@ -37,18 +37,18 @@
 # Your email address:
 author_email='admin@projectrexa.ml',
 
 # Link to your github repository or website: 
 url='https://projectrexa.ml',
 
 # Download Link from where the project can be downloaded from:
-download_url='https://github.com/Om-Mishra7/ProjectRexa-PyPI/archive/refs/tags/v_01.tar.gz',
+download_url='https://github.com/Om-Mishra7/ProjectRexa-PyPI/archive/refs/tags/v_02.tar.gz',
 
 # List of keywords: 
 keywords=['ProjectRexa'],
 
 # List project dependencies: 
-install_requires=['flask','cryptography','base64','json','requests'],
+install_requires=['flask','cryptography','base64','requests'],
 
 # https://pypi.org/classifiers/ 
 classifiers=['Development Status :: 2 - Pre-Alpha']
 )
```

