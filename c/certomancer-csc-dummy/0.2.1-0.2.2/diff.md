# Comparing `tmp/certomancer-csc-dummy-0.2.1.tar.gz` & `tmp/certomancer-csc-dummy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certomancer-csc-dummy-0.2.1.tar", last modified: Sat Aug 20 09:46:16 2022, max compression
+gzip compressed data, was "certomancer-csc-dummy-0.2.2.tar", last modified: Sun May 14 10:18:19 2023, max compression
```

## Comparing `certomancer-csc-dummy-0.2.1.tar` & `certomancer-csc-dummy-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-08-20 09:46:16.078955 certomancer-csc-dummy-0.2.1/
--rw-r--r--   0 matthias   (501) staff       (20)     1080 2022-07-15 15:39:15.000000 certomancer-csc-dummy-0.2.1/LICENSE
--rw-r--r--   0 matthias   (501) staff       (20)     4546 2022-08-20 09:46:16.078835 certomancer-csc-dummy-0.2.1/PKG-INFO
--rw-r--r--   0 matthias   (501) staff       (20)     3662 2022-07-15 15:39:15.000000 certomancer-csc-dummy-0.2.1/README.md
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-08-20 09:46:16.077856 certomancer-csc-dummy-0.2.1/certomancer_csc_dummy.egg-info/
--rw-r--r--   0 matthias   (501) staff       (20)     4546 2022-08-20 09:46:16.000000 certomancer-csc-dummy-0.2.1/certomancer_csc_dummy.egg-info/PKG-INFO
--rw-r--r--   0 matthias   (501) staff       (20)      413 2022-08-20 09:46:16.000000 certomancer-csc-dummy-0.2.1/certomancer_csc_dummy.egg-info/SOURCES.txt
--rw-r--r--   0 matthias   (501) staff       (20)        1 2022-08-20 09:46:16.000000 certomancer-csc-dummy-0.2.1/certomancer_csc_dummy.egg-info/dependency_links.txt
--rw-r--r--   0 matthias   (501) staff       (20)       62 2022-08-20 09:46:16.000000 certomancer-csc-dummy-0.2.1/certomancer_csc_dummy.egg-info/entry_points.txt
--rw-r--r--   0 matthias   (501) staff       (20)       98 2022-08-20 09:46:16.000000 certomancer-csc-dummy-0.2.1/certomancer_csc_dummy.egg-info/requires.txt
--rw-r--r--   0 matthias   (501) staff       (20)       10 2022-08-20 09:46:16.000000 certomancer-csc-dummy-0.2.1/certomancer_csc_dummy.egg-info/top_level.txt
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-08-20 09:46:16.078666 certomancer-csc-dummy-0.2.1/csc_dummy/
--rw-r--r--   0 matthias   (501) staff       (20)        0 2022-07-15 15:39:15.000000 certomancer-csc-dummy-0.2.1/csc_dummy/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)      583 2022-07-15 15:39:15.000000 certomancer-csc-dummy-0.2.1/csc_dummy/__main__.py
--rw-r--r--   0 matthias   (501) staff       (20)    22304 2022-07-15 15:39:15.000000 certomancer-csc-dummy-0.2.1/csc_dummy/csc_dummy_server.py
--rw-r--r--   0 matthias   (501) staff       (20)      504 2022-07-15 15:39:15.000000 certomancer-csc-dummy-0.2.1/csc_dummy/runner.py
--rw-r--r--   0 matthias   (501) staff       (20)       51 2022-08-20 09:43:25.000000 certomancer-csc-dummy-0.2.1/csc_dummy/version.py
--rw-r--r--   0 matthias   (501) staff       (20)       38 2022-08-20 09:46:16.078991 certomancer-csc-dummy-0.2.1/setup.cfg
--rw-r--r--   0 matthias   (501) staff       (20)     1982 2022-08-20 09:44:14.000000 certomancer-csc-dummy-0.2.1/setup.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-05-14 10:18:19.078766 certomancer-csc-dummy-0.2.2/
+-rw-r--r--   0 matthias   (501) staff       (20)     1080 2022-07-15 15:39:15.000000 certomancer-csc-dummy-0.2.2/LICENSE
+-rw-r--r--   0 matthias   (501) staff       (20)     4593 2023-05-14 10:18:19.078630 certomancer-csc-dummy-0.2.2/PKG-INFO
+-rw-r--r--   0 matthias   (501) staff       (20)     3662 2022-07-15 15:39:15.000000 certomancer-csc-dummy-0.2.2/README.md
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-05-14 10:18:19.077404 certomancer-csc-dummy-0.2.2/certomancer_csc_dummy.egg-info/
+-rw-r--r--   0 matthias   (501) staff       (20)     4593 2023-05-14 10:18:19.000000 certomancer-csc-dummy-0.2.2/certomancer_csc_dummy.egg-info/PKG-INFO
+-rw-r--r--   0 matthias   (501) staff       (20)      413 2023-05-14 10:18:19.000000 certomancer-csc-dummy-0.2.2/certomancer_csc_dummy.egg-info/SOURCES.txt
+-rw-r--r--   0 matthias   (501) staff       (20)        1 2023-05-14 10:18:19.000000 certomancer-csc-dummy-0.2.2/certomancer_csc_dummy.egg-info/dependency_links.txt
+-rw-r--r--   0 matthias   (501) staff       (20)       62 2023-05-14 10:18:19.000000 certomancer-csc-dummy-0.2.2/certomancer_csc_dummy.egg-info/entry_points.txt
+-rw-r--r--   0 matthias   (501) staff       (20)       99 2023-05-14 10:18:19.000000 certomancer-csc-dummy-0.2.2/certomancer_csc_dummy.egg-info/requires.txt
+-rw-r--r--   0 matthias   (501) staff       (20)       10 2023-05-14 10:18:19.000000 certomancer-csc-dummy-0.2.2/certomancer_csc_dummy.egg-info/top_level.txt
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2023-05-14 10:18:19.078429 certomancer-csc-dummy-0.2.2/csc_dummy/
+-rw-r--r--   0 matthias   (501) staff       (20)        0 2022-07-15 15:39:15.000000 certomancer-csc-dummy-0.2.2/csc_dummy/__init__.py
+-rw-r--r--   0 matthias   (501) staff       (20)      583 2022-07-15 15:39:15.000000 certomancer-csc-dummy-0.2.2/csc_dummy/__main__.py
+-rw-r--r--   0 matthias   (501) staff       (20)    22304 2022-07-15 15:39:15.000000 certomancer-csc-dummy-0.2.2/csc_dummy/csc_dummy_server.py
+-rw-r--r--   0 matthias   (501) staff       (20)      504 2022-07-15 15:39:15.000000 certomancer-csc-dummy-0.2.2/csc_dummy/runner.py
+-rw-r--r--   0 matthias   (501) staff       (20)       51 2023-05-14 10:15:51.000000 certomancer-csc-dummy-0.2.2/csc_dummy/version.py
+-rw-r--r--   0 matthias   (501) staff       (20)       38 2023-05-14 10:18:19.078813 certomancer-csc-dummy-0.2.2/setup.cfg
+-rw-r--r--   0 matthias   (501) staff       (20)     2029 2023-05-14 10:17:50.000000 certomancer-csc-dummy-0.2.2/setup.py
```

### Comparing `certomancer-csc-dummy-0.2.1/LICENSE` & `certomancer-csc-dummy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `certomancer-csc-dummy-0.2.1/PKG-INFO` & `certomancer-csc-dummy-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: certomancer-csc-dummy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Certomancer-based demo CSC server for integration tests
 Home-page: https://github.com/MatthiasValvekens/certomancer-csc-dummy
 Author: Matthias Valvekens
 Author-email: dev@mvalvekens.be
 License: MIT
 Keywords: pki testing csc signature
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Certomancer-based dummy CSC server implementation
```

### Comparing `certomancer-csc-dummy-0.2.1/README.md` & `certomancer-csc-dummy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `certomancer-csc-dummy-0.2.1/certomancer_csc_dummy.egg-info/PKG-INFO` & `certomancer-csc-dummy-0.2.2/certomancer_csc_dummy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: certomancer-csc-dummy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Certomancer-based demo CSC server for integration tests
 Home-page: https://github.com/MatthiasValvekens/certomancer-csc-dummy
 Author: Matthias Valvekens
 Author-email: dev@mvalvekens.be
 License: MIT
 Keywords: pki testing csc signature
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Certomancer-based dummy CSC server implementation
```

### Comparing `certomancer-csc-dummy-0.2.1/csc_dummy/__main__.py` & `certomancer-csc-dummy-0.2.2/csc_dummy/__main__.py`

 * *Files identical despite different names*

### Comparing `certomancer-csc-dummy-0.2.1/csc_dummy/csc_dummy_server.py` & `certomancer-csc-dummy-0.2.2/csc_dummy/csc_dummy_server.py`

 * *Files identical despite different names*

### Comparing `certomancer-csc-dummy-0.2.1/setup.py` & `certomancer-csc-dummy-0.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,37 +26,38 @@
     license='MIT',
     author='Matthias Valvekens',
     author_email='dev@mvalvekens.be',
     description='A Certomancer-based demo CSC server for integration tests',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 3 - Alpha',
 
         'Intended Audience :: Developers',
 
         'License :: OSI Approved :: MIT License',
 
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 
         'Topic :: Security :: Cryptography',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     entry_points={
         "console_scripts": [
             "certomancer-csc = csc_dummy.__main__:launch"
         ]
     },
     install_requires=[
         'asn1crypto>=1.5.0',
         'cryptography>=3.3.1',
-        'certomancer >=0.8.3, <0.10.0',
+        'certomancer >=0.11.0, <0.12.0',
         'aiohttp~=3.8.0',
         'python-pae==0.1.0',
     ],
     setup_requires=['wheel',],
     keywords="pki testing csc signature"
 )
```

