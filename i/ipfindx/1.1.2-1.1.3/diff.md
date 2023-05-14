# Comparing `tmp/ipfindx-1.1.2.tar.gz` & `tmp/ipfindx-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfindx-1.1.2.tar", last modified: Sun May 14 16:22:39 2023, max compression
+gzip compressed data, was "ipfindx-1.1.3.tar", last modified: Sun May 14 16:28:12 2023, max compression
```

## Comparing `ipfindx-1.1.2.tar` & `ipfindx-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-14 16:22:39.455624 ipfindx-1.1.2/
--rw-r--r--   0 alex      (1000) alex      (1000)     1067 2023-05-14 15:45:39.000000 ipfindx-1.1.2/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)     2143 2023-05-14 16:22:39.451624 ipfindx-1.1.2/PKG-INFO
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-14 16:22:39.451624 ipfindx-1.1.2/ipfindx/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-14 15:46:33.000000 ipfindx-1.1.2/ipfindx/__init__.py
--rwxr-xr-x   0 alex      (1000) alex      (1000)     1623 2023-05-14 16:21:03.000000 ipfindx-1.1.2/ipfindx/ipfindx.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-14 16:22:39.451624 ipfindx-1.1.2/ipfindx.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     2143 2023-05-14 16:22:39.000000 ipfindx-1.1.2/ipfindx.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      243 2023-05-14 16:22:39.000000 ipfindx-1.1.2/ipfindx.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-14 16:22:39.000000 ipfindx-1.1.2/ipfindx.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       48 2023-05-14 16:22:39.000000 ipfindx-1.1.2/ipfindx.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        9 2023-05-14 16:22:39.000000 ipfindx-1.1.2/ipfindx.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        8 2023-05-14 16:22:39.000000 ipfindx-1.1.2/ipfindx.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-14 16:22:39.455624 ipfindx-1.1.2/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)     2353 2023-05-14 16:22:20.000000 ipfindx-1.1.2/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-14 16:28:12.626426 ipfindx-1.1.3/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1067 2023-05-14 15:45:39.000000 ipfindx-1.1.3/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)     2143 2023-05-14 16:28:12.622426 ipfindx-1.1.3/PKG-INFO
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-14 16:28:12.622426 ipfindx-1.1.3/ipfindx/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-05-14 15:46:33.000000 ipfindx-1.1.3/ipfindx/__init__.py
+-rwxr-xr-x   0 alex      (1000) alex      (1000)     1647 2023-05-14 16:27:48.000000 ipfindx-1.1.3/ipfindx/ipfindx.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-14 16:28:12.622426 ipfindx-1.1.3/ipfindx.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     2143 2023-05-14 16:28:12.000000 ipfindx-1.1.3/ipfindx.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      243 2023-05-14 16:28:12.000000 ipfindx-1.1.3/ipfindx.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-14 16:28:12.000000 ipfindx-1.1.3/ipfindx.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       48 2023-05-14 16:28:12.000000 ipfindx-1.1.3/ipfindx.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        9 2023-05-14 16:28:12.000000 ipfindx-1.1.3/ipfindx.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        8 2023-05-14 16:28:12.000000 ipfindx-1.1.3/ipfindx.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-14 16:28:12.626426 ipfindx-1.1.3/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)     2353 2023-05-14 16:27:54.000000 ipfindx-1.1.3/setup.py
```

### Comparing `ipfindx-1.1.2/LICENSE` & `ipfindx-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfindx-1.1.2/PKG-INFO` & `ipfindx-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfindx
-Version: 1.1.2
+Version: 1.1.3
 Summary: Get IP address information
 Home-page: https://github.com/MrHacker-X/IPFindX
 Author: Alex Butler 🚩
 Author-email: mrhackerxofficial@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfindx-1.1.2/ipfindx/ipfindx.py` & `ipfindx-1.1.3/ipfindx/ipfindx.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 print('\033[;92m')
 # Parse command line arguments
 parser = argparse.ArgumentParser(description='Get IP address information.')
 parser.add_argument('-i', '--ip', type=str, required=True, help='IP address')
 parser.add_argument('-o', '--output', type=str, help='Output file name')
 args = parser.parse_args()
 
+def run():
+    print()
+
 # Make API request
 url = f"http://ip-api.com/json/{args.ip}?fields=status,message,continent,continentCode,country,countryCode,region,regionName,city,district,zip,lat,lon,timezone,offset,currency,isp,org,as,asname,reverse,mobile,proxy,hosting,query"
 res = requests.get(url)
 data = json.loads(res.text)
 
 # Print banner
 print("""\033[;92m
 ╭━━┳━━━┳━━━╮╱╱╱╱╱╭┳━╮╭━╮
 ╰┫┣┫╭━╮┃╭━━╯╱╱╱╱╱┃┣╮╰╯╭╯
 ╱┃┃┃╰━╯┃╰━━┳┳━╮╭━╯┃╰╮╭╯
 ╱┃┃┃╭━━┫╭━━╋┫╭╮┫╭╮┃╭╯╰╮
 ╭┫┣┫┃╱╱┃┃╱╱┃┃┃┃┃╰╯┣╯╭╮╰╮
-╰━━┻╯╱╱╰╯╱╱╰┻╯╰┻━━┻━╯╰━╯V:1.1.2
+╰━━┻╯╱╱╰╯╱╱╰┻╯╰┻━━┻━╯╰━╯V:1.1.3
 ////////\033[;93mMrHacker-X\033[;92m///////
 """)
 
 # Print the key-value pairs to the console
 for key, value in data.items():
     print(f"\033[1;92m[+]\033[1;93m {key}:\033[1;92m {value}")
```

### Comparing `ipfindx-1.1.2/ipfindx.egg-info/PKG-INFO` & `ipfindx-1.1.3/ipfindx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfindx
-Version: 1.1.2
+Version: 1.1.3
 Summary: Get IP address information
 Home-page: https://github.com/MrHacker-X/IPFindX
 Author: Alex Butler 🚩
 Author-email: mrhackerxofficial@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfindx-1.1.2/setup.py` & `ipfindx-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ipfindx',
-    version='1.1.2',
+    version='1.1.3',
     author='Alex Butler 🚩',
     author_email='mrhackerxofficial@gmail.com',
     description='Get IP address information',
     long_description='''[+] ipfindx is a command-line tool that allows you to quickly retrieve information about an IP address from the ip-api.com API. With ipfindx, you can quickly and easily obtain information such as the IP address's location, country, region, city, and ISP. To use ipfindx, simply provide an IP address as a command-line argument, and ipfindx will make a request to the ip-api.com API and display the results. You can also specify an output file name with the `-o` or `--output` option to save the results to a file. ipfindx is a useful tool for network administrators, developers, and anyone who needs to quickly obtain information about an IP address. With its simple and intuitive command-line interface, ipfindx makes it easy to look up IP addresses and obtain the information you need to diagnose network issues, troubleshoot problems, and perform other tasks.
 
 [+] Features:
```

