# Comparing `tmp/ipfindx-1.0.1.tar.gz` & `tmp/ipfindx-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfindx-1.0.1.tar", last modified: Sun May 14 15:51:29 2023, max compression
+gzip compressed data, was "ipfindx-1.0.2.tar", last modified: Sun May 14 16:13:37 2023, max compression
```

## Comparing `ipfindx-1.0.1.tar` & `ipfindx-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-14 15:51:29.038096 ipfindx-1.0.1/
--rw-r--r--   0 alex      (1000) alex      (1000)     1067 2023-05-14 15:45:39.000000 ipfindx-1.0.1/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)     2143 2023-05-14 15:51:29.034096 ipfindx-1.0.1/PKG-INFO
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-14 15:51:29.034096 ipfindx-1.0.1/ipfindx/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-14 15:46:33.000000 ipfindx-1.0.1/ipfindx/__init__.py
--rwxr-xr-x   0 alex      (1000) alex      (1000)     1623 2023-05-14 15:38:53.000000 ipfindx-1.0.1/ipfindx/ipfindx.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-14 15:51:29.034096 ipfindx-1.0.1/ipfindx.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     2143 2023-05-14 15:51:28.000000 ipfindx-1.0.1/ipfindx.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      243 2023-05-14 15:51:28.000000 ipfindx-1.0.1/ipfindx.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-14 15:51:28.000000 ipfindx-1.0.1/ipfindx.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       49 2023-05-14 15:51:28.000000 ipfindx-1.0.1/ipfindx.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        9 2023-05-14 15:51:28.000000 ipfindx-1.0.1/ipfindx.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        8 2023-05-14 15:51:28.000000 ipfindx-1.0.1/ipfindx.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-14 15:51:29.038096 ipfindx-1.0.1/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)     2364 2023-05-14 14:59:26.000000 ipfindx-1.0.1/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-14 16:13:37.263619 ipfindx-1.0.2/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1067 2023-05-14 15:45:39.000000 ipfindx-1.0.2/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)     2143 2023-05-14 16:13:37.263619 ipfindx-1.0.2/PKG-INFO
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-14 16:13:37.259619 ipfindx-1.0.2/ipfindx/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-14 15:46:33.000000 ipfindx-1.0.2/ipfindx/__init__.py
+-rwxr-xr-x   0 alex      (1000) alex      (1000)     1623 2023-05-14 16:11:58.000000 ipfindx-1.0.2/ipfindx/ipfindx.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-14 16:13:37.263619 ipfindx-1.0.2/ipfindx.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     2143 2023-05-14 16:13:36.000000 ipfindx-1.0.2/ipfindx.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      243 2023-05-14 16:13:37.000000 ipfindx-1.0.2/ipfindx.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-14 16:13:36.000000 ipfindx-1.0.2/ipfindx.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       44 2023-05-14 16:13:36.000000 ipfindx-1.0.2/ipfindx.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        9 2023-05-14 16:13:36.000000 ipfindx-1.0.2/ipfindx.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        8 2023-05-14 16:13:36.000000 ipfindx-1.0.2/ipfindx.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-14 16:13:37.263619 ipfindx-1.0.2/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)     2359 2023-05-14 16:12:01.000000 ipfindx-1.0.2/setup.py
```

### Comparing `ipfindx-1.0.1/LICENSE` & `ipfindx-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfindx-1.0.1/PKG-INFO` & `ipfindx-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfindx
-Version: 1.0.1
+Version: 1.0.2
 Summary: Get IP address information
 Home-page: https://github.com/MrHacker-X/IPFindX
 Author: Alex Butler 🚩
 Author-email: mrhackerxofficial@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfindx-1.0.1/ipfindx/ipfindx.py` & `ipfindx-1.0.2/ipfindx/ipfindx.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # Print banner
 print("""\033[;92m
 ╭━━┳━━━┳━━━╮╱╱╱╱╱╭┳━╮╭━╮
 ╰┫┣┫╭━╮┃╭━━╯╱╱╱╱╱┃┣╮╰╯╭╯
 ╱┃┃┃╰━╯┃╰━━┳┳━╮╭━╯┃╰╮╭╯
 ╱┃┃┃╭━━┫╭━━╋┫╭╮┫╭╮┃╭╯╰╮
 ╭┫┣┫┃╱╱┃┃╱╱┃┃┃┃┃╰╯┣╯╭╮╰╮
-╰━━┻╯╱╱╰╯╱╱╰┻╯╰┻━━┻━╯╰━╯V:1.0.1
+╰━━┻╯╱╱╰╯╱╱╰┻╯╰┻━━┻━╯╰━╯V:1.0.2
 ////////\033[;93mMrHacker-X\033[;92m///////
 """)
 
 # Print the key-value pairs to the console
 for key, value in data.items():
     print(f"\033[1;92m[+]\033[1;93m {key}:\033[1;92m {value}")
```

### Comparing `ipfindx-1.0.1/ipfindx.egg-info/PKG-INFO` & `ipfindx-1.0.2/ipfindx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfindx
-Version: 1.0.1
+Version: 1.0.2
 Summary: Get IP address information
 Home-page: https://github.com/MrHacker-X/IPFindX
 Author: Alex Butler 🚩
 Author-email: mrhackerxofficial@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfindx-1.0.1/setup.py` & `ipfindx-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ipfindx',
-    version='1.0.1',
+    version='1.0.2',
     author='Alex Butler 🚩',
     author_email='mrhackerxofficial@gmail.com',
     description='Get IP address information',
     long_description='''[+] ipfindx is a command-line tool that allows you to quickly retrieve information about an IP address from the ip-api.com API. With ipfindx, you can quickly and easily obtain information such as the IP address's location, country, region, city, and ISP. To use ipfindx, simply provide an IP address as a command-line argument, and ipfindx will make a request to the ip-api.com API and display the results. You can also specify an output file name with the `-o` or `--output` option to save the results to a file. ipfindx is a useful tool for network administrators, developers, and anyone who needs to quickly obtain information about an IP address. With its simple and intuitive command-line interface, ipfindx makes it easy to look up IP addresses and obtain the information you need to diagnose network issues, troubleshoot problems, and perform other tasks.
 
 [+] Features:
 
@@ -20,13 +20,13 @@
     url='https://github.com/MrHacker-X/IPFindX',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     entry_points={
         'console_scripts': [
-            'ipfindx=ipfindx.ipfindx:main',
+            'ipfindx=ipfindx.ipfindx',
         ],
     },
     classifiers=[    'Development Status :: 4 - Beta',    'Intended Audience :: Developers',    'License :: OSI Approved :: MIT License',    'Programming Language :: Python :: 3',    'Programming Language :: Python :: 3.10',    'Topic :: Internet :: Name Service (DNS)',    'Topic :: Internet :: Proxy Servers',    'Topic :: Internet :: WWW/HTTP',    'Topic :: System :: Networking',    'Intended Audience :: System Administrators',    'Intended Audience :: Financial and Insurance Industry',    'Intended Audience :: Science/Research',],
 
 )
```

