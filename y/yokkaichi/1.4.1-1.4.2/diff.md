# Comparing `tmp/yokkaichi-1.4.1.tar.gz` & `tmp/yokkaichi-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yokkaichi-1.4.1.tar", last modified: Fri May 12 19:45:41 2023, max compression
+gzip compressed data, was "yokkaichi-1.4.2.tar", last modified: Sun May 14 19:42:33 2023, max compression
```

## Comparing `yokkaichi-1.4.1.tar` & `yokkaichi-1.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-12 19:45:41.444591 yokkaichi-1.4.1/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.4.1/LICENSE.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-12 19:45:41.444591 yokkaichi-1.4.1/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2252 2023-05-12 19:27:27.000000 yokkaichi-1.4.1/README.md
--rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-05-12 19:45:41.444591 yokkaichi-1.4.1/setup.cfg
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1529 2023-05-12 19:42:32.000000 yokkaichi-1.4.1/setup.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-12 19:45:41.444591 yokkaichi-1.4.1/yokkaichi/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2921 2023-05-12 18:51:44.000000 yokkaichi-1.4.1/yokkaichi/MasscanScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     6071 2023-05-12 18:51:44.000000 yokkaichi-1.4.1/yokkaichi/ServerScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-05-12 19:42:32.000000 yokkaichi-1.4.1/yokkaichi/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     8205 2023-05-12 19:42:32.000000 yokkaichi-1.4.1/yokkaichi/__main__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1261 2023-05-12 18:51:44.000000 yokkaichi-1.4.1/yokkaichi/args_to_cfg.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3874 2023-05-12 18:51:44.000000 yokkaichi-1.4.1/yokkaichi/config_loader.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1160 2023-05-12 18:51:44.000000 yokkaichi-1.4.1/yokkaichi/port_parser.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-12 19:45:41.444591 yokkaichi-1.4.1/yokkaichi.egg-info/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-12 19:45:41.000000 yokkaichi-1.4.1/yokkaichi.egg-info/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)      364 2023-05-12 19:45:41.000000 yokkaichi-1.4.1/yokkaichi.egg-info/SOURCES.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-05-12 19:45:41.000000 yokkaichi-1.4.1/yokkaichi.egg-info/dependency_links.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       91 2023-05-12 19:45:41.000000 yokkaichi-1.4.1/yokkaichi.egg-info/requires.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-05-12 19:45:41.000000 yokkaichi-1.4.1/yokkaichi.egg-info/top_level.txt
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-14 19:42:33.005383 yokkaichi-1.4.2/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.4.2/LICENSE.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-14 19:42:33.005383 yokkaichi-1.4.2/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2252 2023-05-12 19:27:27.000000 yokkaichi-1.4.2/README.md
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-05-14 19:42:33.005383 yokkaichi-1.4.2/setup.cfg
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1503 2023-05-14 19:38:14.000000 yokkaichi-1.4.2/setup.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-14 19:42:33.005383 yokkaichi-1.4.2/yokkaichi/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2921 2023-05-12 18:51:44.000000 yokkaichi-1.4.2/yokkaichi/MasscanScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     6039 2023-05-14 19:38:14.000000 yokkaichi-1.4.2/yokkaichi/ServerScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-05-14 19:38:14.000000 yokkaichi-1.4.2/yokkaichi/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     8322 2023-05-14 19:38:14.000000 yokkaichi-1.4.2/yokkaichi/__main__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1261 2023-05-12 18:51:44.000000 yokkaichi-1.4.2/yokkaichi/args_to_cfg.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2068 2023-05-14 19:38:14.000000 yokkaichi-1.4.2/yokkaichi/config_loader.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1160 2023-05-12 18:51:44.000000 yokkaichi-1.4.2/yokkaichi/port_parser.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-14 19:42:33.005383 yokkaichi-1.4.2/yokkaichi.egg-info/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-14 19:42:32.000000 yokkaichi-1.4.2/yokkaichi.egg-info/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      364 2023-05-14 19:42:32.000000 yokkaichi-1.4.2/yokkaichi.egg-info/SOURCES.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-05-14 19:42:32.000000 yokkaichi-1.4.2/yokkaichi.egg-info/dependency_links.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       63 2023-05-14 19:42:32.000000 yokkaichi-1.4.2/yokkaichi.egg-info/requires.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-05-14 19:42:32.000000 yokkaichi-1.4.2/yokkaichi.egg-info/top_level.txt
```

### Comparing `yokkaichi-1.4.1/LICENSE.txt` & `yokkaichi-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.1/PKG-INFO` & `yokkaichi-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.4.1
+Version: 1.4.2
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `yokkaichi-1.4.1/README.md` & `yokkaichi-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.1/setup.py` & `yokkaichi-1.4.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     url="https://github.com/Oreeeee/yokkaichi",
     install_requires=[
         "rich",
         "mcstatus",
         "ip2location",
         "python-masscan",
         "requests",
-        'tomli >= 1.1.0 ; python_version < "3.11"',
+        "tomli >= 1.1.0",
     ],
     classifiers=[
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
```

### Comparing `yokkaichi-1.4.1/yokkaichi/MasscanScan.py` & `yokkaichi-1.4.2/yokkaichi/MasscanScan.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.1/yokkaichi/ServerScan.py` & `yokkaichi-1.4.2/yokkaichi/ServerScan.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class ServerScan:
     def __init__(self, cfg, masscan_list, ip_list):
         self.cfg = cfg
         self.masscan_list = masscan_list
         self.ip_list = ip_list
 
-        self.results = {"server_list": []}
+        self.results = []
         self.lock = threading.Lock()
 
     def start_scan(self):
         if self.cfg.use_ip2location:
             console.print("Loading IP2Location database", style="cyan")
             if self.cfg.ip2location_cache:
                 self.ip2location_db = IP2Location.IP2Location(
@@ -158,10 +158,10 @@
         ip2location_data_str = str(self.ip2location_db.get_all(ip))
         # Convert the data to dict
         ip2location_data_dict = ast.literal_eval(ip2location_data_str)
 
         return ip2location_data_dict
 
     def add_to_file(self, server_info):
-        self.results["server_list"].append(server_info)
+        self.results.append(server_info)
         with open(self.cfg.output_file, "w", encoding="utf-8") as f:
             json.dump(self.results, f, indent=4, ensure_ascii=False)
```

### Comparing `yokkaichi-1.4.1/yokkaichi/__main__.py` & `yokkaichi-1.4.2/yokkaichi/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,20 @@
 from .constants.rich_console import console
 from .port_parser import parse_port_range
 from .args_to_cfg import args_to_cfg
 from .MasscanScan import MasscanScan
 from .ServerScan import ServerScan
 from yokkaichi import __version__
 from . import config_loader
+import IP2Location
 import platform
 import argparse
 import requests
 import pathlib
-
-try:
-    import tomllib
-except ModuleNotFoundError:
-    # Use tomli instead (Python versions before 3.11)
-    import tomli as tomllib
+import tomli
 
 
 def display_version():
     console.print(
         f"yokkaichi [bold cyan]{__version__}[/bold cyan] on [bold cyan]{platform.python_implementation()} {platform.python_version()}[/bold cyan]",
         style="green",
     )
@@ -43,14 +39,27 @@
         # Add IPs to IP list
         for ip in cidr_list.text.splitlines():
             country_ip_list.append(ip)
 
     return country_ip_list
 
 
+def verify_ip2location(db):
+    if not pathlib.Path(db).is_file():
+        console.print("IP2Location database doesn't exist", style="bold red")
+        exit(1)
+
+    try:
+        IP2Location.IP2Location(db)
+    except ValueError:
+        # IP2Location's default exception messages are okay
+        console.print("The IP2Location database is corrupted", style="bold red")
+        exit(1)
+
+
 def load_ip_list(ip_list_location):
     ips = []
     # Load file
     try:
         with open(ip_list_location, "r") as f:
             ip_list = f.readlines()
             for ip in ip_list:
@@ -68,15 +77,15 @@
         display_version()
 
     # Load the config file
     if args.config_file != None:
         try:
             cfg = config_loader.parse_cfg(args.config_file)
             # TODO: Make use of it
-        except tomllib.TOMLDecodeError:
+        except tomli.TOMLDecodeError:
             console.print(
                 "Config file is invalid! (Failed parsing TOML)", style="bold red"
             )
         except FileNotFoundError:
             console.print(
                 f"[bold white]{args.config_file}[/bold white] doesn't exist. Create a sample config in this location? (y/n) ",
                 style="yellow",
@@ -99,18 +108,15 @@
         )
         if input().lower() == "n":
             exit(0)
     else:
         # Touch the file
         pathlib.Path(cfg.output).touch()
 
-    # Check does IP2Location db exist
-    if cfg.use_ip2location and not pathlib.Path(cfg.ip2location_db).is_file():
-        console.print("This IP2Location DB doesn't exist", style="bold red")
-        exit(1)
+    verify_ip2location(cfg.ip2location_db)
 
     if cfg.ip_list_scan:
         console.print("Loading IPs", style="cyan")
         ip_list = load_ip_list(cfg.ip_list)
         console.print(f"Loaded {len(ip_list)} IPs", style="green")
     else:
         ip_list = None
```

### Comparing `yokkaichi-1.4.1/yokkaichi/args_to_cfg.py` & `yokkaichi-1.4.2/yokkaichi/args_to_cfg.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.1/yokkaichi/port_parser.py` & `yokkaichi-1.4.2/yokkaichi/port_parser.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.1/yokkaichi.egg-info/PKG-INFO` & `yokkaichi-1.4.2/yokkaichi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.4.1
+Version: 1.4.2
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

