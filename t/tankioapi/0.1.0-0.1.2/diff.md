# Comparing `tmp/tankioapi-0.1.0.tar.gz` & `tmp/tankioapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tankioapi-0.1.0.tar", last modified: Sun May 14 11:20:49 2023, max compression
+gzip compressed data, was "tankioapi-0.1.2.tar", last modified: Sun May 14 11:48:17 2023, max compression
```

## Comparing `tankioapi-0.1.0.tar` & `tankioapi-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 11:20:49.525527 tankioapi-0.1.0/
--rw-rw-rw-   0        0        0     1072 2023-05-13 16:20:18.000000 tankioapi-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4489 2023-05-14 11:20:49.523526 tankioapi-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3096 2023-05-14 11:18:16.000000 tankioapi-0.1.0/README.md
--rw-rw-rw-   0        0        0     1971 2023-05-14 10:45:06.000000 tankioapi-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 11:20:49.525527 tankioapi-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3784 2023-05-13 16:58:45.000000 tankioapi-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:20:49.290527 tankioapi-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 11:20:49.472530 tankioapi-0.1.0/src/tankioapi.egg-info/
--rw-rw-rw-   0        0        0     4489 2023-05-14 11:20:48.000000 tankioapi-0.1.0/src/tankioapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      509 2023-05-14 11:20:49.000000 tankioapi-0.1.0/src/tankioapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 11:20:48.000000 tankioapi-0.1.0/src/tankioapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-14 11:20:48.000000 tankioapi-0.1.0/src/tankioapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-14 11:20:48.000000 tankioapi-0.1.0/src/tankioapi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 11:20:49.479528 tankioapi-0.1.0/src/toapi/
--rw-rw-rw-   0        0        0     1309 2023-05-13 18:31:19.000000 tankioapi-0.1.0/src/toapi/__init__.py
--rw-rw-rw-   0        0        0     5367 2023-05-14 11:02:57.000000 tankioapi-0.1.0/src/toapi/client.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:20:49.521528 tankioapi-0.1.0/src/toapi/dataclasses/
--rw-rw-rw-   0        0        0     1216 2023-05-13 20:00:35.000000 tankioapi-0.1.0/src/toapi/dataclasses/__init__.py
--rw-rw-rw-   0        0        0     4114 2023-05-14 10:07:07.000000 tankioapi-0.1.0/src/toapi/dataclasses/game_object.py
--rw-rw-rw-   0        0        0     2291 2023-05-13 20:14:00.000000 tankioapi-0.1.0/src/toapi/dataclasses/mode.py
--rw-rw-rw-   0        0        0     2010 2023-05-13 17:50:36.000000 tankioapi-0.1.0/src/toapi/dataclasses/rank.py
--rw-rw-rw-   0        0        0     2887 2023-05-14 09:45:15.000000 tankioapi-0.1.0/src/toapi/dataclasses/rating.py
--rw-rw-rw-   0        0        0     1487 2023-05-13 18:08:39.000000 tankioapi-0.1.0/src/toapi/dataclasses/top.py
--rw-rw-rw-   0        0        0     5855 2023-05-14 10:25:17.000000 tankioapi-0.1.0/src/toapi/dataclasses/user.py
--rw-rw-rw-   0        0        0     1609 2023-05-13 18:17:03.000000 tankioapi-0.1.0/src/toapi/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:48:17.247064 tankioapi-0.1.2/
+-rw-rw-rw-   0        0        0     1072 2023-05-13 16:20:18.000000 tankioapi-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       89 2023-05-14 11:37:12.000000 tankioapi-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4497 2023-05-14 11:48:17.244067 tankioapi-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3116 2023-05-14 11:25:34.000000 tankioapi-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1959 2023-05-14 11:44:13.000000 tankioapi-0.1.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-14 11:48:17.182065 tankioapi-0.1.2/requirements/
+-rw-rw-rw-   0        0        0       29 2023-05-14 11:20:40.000000 tankioapi-0.1.2/requirements/dev.txt
+-rw-rw-rw-   0        0        0       24 2023-05-13 16:18:41.000000 tankioapi-0.1.2/requirements/speedup.txt
+-rw-rw-rw-   0        0        0        7 2023-05-13 16:15:33.000000 tankioapi-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 11:48:17.248069 tankioapi-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     3784 2023-05-14 11:35:55.000000 tankioapi-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:48:17.152068 tankioapi-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 11:48:17.200064 tankioapi-0.1.2/src/tankioapi.egg-info/
+-rw-rw-rw-   0        0        0     4497 2023-05-14 11:48:16.000000 tankioapi-0.1.2/src/tankioapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-05-14 11:48:17.000000 tankioapi-0.1.2/src/tankioapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 11:48:16.000000 tankioapi-0.1.2/src/tankioapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-14 11:48:16.000000 tankioapi-0.1.2/src/tankioapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-14 11:48:16.000000 tankioapi-0.1.2/src/tankioapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 11:48:17.212068 tankioapi-0.1.2/src/toapi/
+-rw-rw-rw-   0        0        0     1309 2023-05-14 11:47:09.000000 tankioapi-0.1.2/src/toapi/__init__.py
+-rw-rw-rw-   0        0        0     5367 2023-05-14 11:02:57.000000 tankioapi-0.1.2/src/toapi/client.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:48:17.241065 tankioapi-0.1.2/src/toapi/dataclasses/
+-rw-rw-rw-   0        0        0     1216 2023-05-13 20:00:35.000000 tankioapi-0.1.2/src/toapi/dataclasses/__init__.py
+-rw-rw-rw-   0        0        0     4114 2023-05-14 10:07:07.000000 tankioapi-0.1.2/src/toapi/dataclasses/game_object.py
+-rw-rw-rw-   0        0        0     2291 2023-05-13 20:14:00.000000 tankioapi-0.1.2/src/toapi/dataclasses/mode.py
+-rw-rw-rw-   0        0        0     2010 2023-05-13 17:50:36.000000 tankioapi-0.1.2/src/toapi/dataclasses/rank.py
+-rw-rw-rw-   0        0        0     2887 2023-05-14 09:45:15.000000 tankioapi-0.1.2/src/toapi/dataclasses/rating.py
+-rw-rw-rw-   0        0        0     1487 2023-05-13 18:08:39.000000 tankioapi-0.1.2/src/toapi/dataclasses/top.py
+-rw-rw-rw-   0        0        0     5855 2023-05-14 10:25:17.000000 tankioapi-0.1.2/src/toapi/dataclasses/user.py
+-rw-rw-rw-   0        0        0     1609 2023-05-13 18:17:03.000000 tankioapi-0.1.2/src/toapi/errors.py
```

### Comparing `tankioapi-0.1.0/LICENSE` & `tankioapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tankioapi-0.1.0/PKG-INFO` & `tankioapi-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: tankioapi
-Version: 0.1.0
+Version: 0.1.2
 Summary: A Python written wrapper for the Tanki Online game API
 Home-page: https://github.com/stngularity/tankioapi.py
 Author: stngularity
 Author-email: stngularity <stngularity@gmail.com>
 License: MIT License
-Project-URL: homepage, https://github.com/stngularity/tankioapi.py
-Project-URL: Source Code, https://github.com/stngularity/tankioapi.py
-Project-URL: changelog, https://github.com/stngularity/tankioapi.py/blob/main/CHANGELOG.md
-Project-URL: Bug Tracker, https://github.com/stngularity/tankioapi.py/issues
+Project-URL: homepage, https://github.com/stngularity/tankioapi
+Project-URL: Source Code, https://github.com/stngularity/tankioapi
+Project-URL: changelog, https://github.com/stngularity/tankioapi/blob/main/CHANGELOG.md
+Project-URL: Bug Tracker, https://github.com/stngularity/tankioapi/issues
 Keywords: game,api,to,tanki online
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -40,15 +40,15 @@
     <img src="https://img.shields.io/github/license/stngularity/tankioapi?color=%2346df11&label=License">
 </p>
 
 ## Notification
 This project was created just to exist. Of course, I will update it when the API itself changes, but not immediately. Well, if You want to support this project, You can give it a star.
 
 ## Information
-As mentioned earlier, this project is created just to exist. And so, the module itself is needed to get the top of players and get information about the player separately. If You know more functionality of the API of the game `Tanki Online`, then please report this functionality in the [`Issues`](/issues).
+As mentioned earlier, this project is created just to exist. And so, the module itself is needed to get the top of players and get information about the player separately. If You know more functionality of the API of the game `Tanki Online`, then please report this functionality in the [`Issues`](https://github.com/stngularity/tankioapi/issues).
 
 ###### Features
 - `async`/`await` support
 - Getting top of players
 - Getting information of any player by him name
 
 ## Installing
@@ -76,15 +76,15 @@
 > ```sh
 > $ git clone https://github.com/stngularity/tankioapi
 > $ cd tankioapi
 > $ python3 -m pip install -U .[speedup]
 > ```
 
 ## Examples
-Here are examples of some of the features of the library. More examples in [`examples/`](/blob/main/examples)
+Here are examples of some of the features of the library. More examples in [`examples/`](/examples)
 
 ###### Getting all tops of players
 ```py
 import asyncio
 from toapi import TankiOnline
 
 tops = asyncio.run(TankiOnline.get_tops())
@@ -112,8 +112,8 @@
 print(f"KD: {user.kills}/{user.deaths} ({round(user.kills/user.deaths, 2)})")
 print(f"Caught golds: {user.caught_golds}")
 print(f"Crystals: {user.crystals}")
 print(f"GS: {user.gear_score}")
 ```
 
 ## License
-This project is distributed under the `MIT` license. You can learn more from the [**LICENSE**](/blob/main/LICENSE) file.
+This project is distributed under the `MIT` license. You can learn more from the [**LICENSE**](/LICENSE) file.
```

### Comparing `tankioapi-0.1.0/README.md` & `tankioapi-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <img src="https://img.shields.io/github/license/stngularity/tankioapi?color=%2346df11&label=License">
 </p>
 
 ## Notification
 This project was created just to exist. Of course, I will update it when the API itself changes, but not immediately. Well, if You want to support this project, You can give it a star.
 
 ## Information
-As mentioned earlier, this project is created just to exist. And so, the module itself is needed to get the top of players and get information about the player separately. If You know more functionality of the API of the game `Tanki Online`, then please report this functionality in the [`Issues`](/issues).
+As mentioned earlier, this project is created just to exist. And so, the module itself is needed to get the top of players and get information about the player separately. If You know more functionality of the API of the game `Tanki Online`, then please report this functionality in the [`Issues`](https://github.com/stngularity/tankioapi/issues).
 
 ###### Features
 - `async`/`await` support
 - Getting top of players
 - Getting information of any player by him name
 
 ## Installing
@@ -44,15 +44,15 @@
 > ```sh
 > $ git clone https://github.com/stngularity/tankioapi
 > $ cd tankioapi
 > $ python3 -m pip install -U .[speedup]
 > ```
 
 ## Examples
-Here are examples of some of the features of the library. More examples in [`examples/`](/blob/main/examples)
+Here are examples of some of the features of the library. More examples in [`examples/`](/examples)
 
 ###### Getting all tops of players
 ```py
 import asyncio
 from toapi import TankiOnline
 
 tops = asyncio.run(TankiOnline.get_tops())
@@ -80,8 +80,8 @@
 print(f"KD: {user.kills}/{user.deaths} ({round(user.kills/user.deaths, 2)})")
 print(f"Caught golds: {user.caught_golds}")
 print(f"Crystals: {user.crystals}")
 print(f"GS: {user.gear_score}")
 ```
 
 ## License
-This project is distributed under the `MIT` license. You can learn more from the [**LICENSE**](/blob/main/LICENSE) file.
+This project is distributed under the `MIT` license. You can learn more from the [**LICENSE**](/LICENSE) file.
```

### Comparing `tankioapi-0.1.0/pyproject.toml` & `tankioapi-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Utilities",
     "Typing :: Typed"
 ]
 
 [project.urls]
-homepage = "https://github.com/stngularity/tankioapi.py"
-"Source Code" = "https://github.com/stngularity/tankioapi.py"
-changelog = "https://github.com/stngularity/tankioapi.py/blob/main/CHANGELOG.md"
-"Bug Tracker" = "https://github.com/stngularity/tankioapi.py/issues"
+homepage = "https://github.com/stngularity/tankioapi"
+"Source Code" = "https://github.com/stngularity/tankioapi"
+changelog = "https://github.com/stngularity/tankioapi/blob/main/CHANGELOG.md"
+"Bug Tracker" = "https://github.com/stngularity/tankioapi/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["toapi*"]
 namespaces = false
 
 # The configuration for "iSort" tool
```

### Comparing `tankioapi-0.1.0/setup.py` & `tankioapi-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `tankioapi-0.1.0/src/tankioapi.egg-info/PKG-INFO` & `tankioapi-0.1.2/src/tankioapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: tankioapi
-Version: 0.1.0
+Version: 0.1.2
 Summary: A Python written wrapper for the Tanki Online game API
 Home-page: https://github.com/stngularity/tankioapi.py
 Author: stngularity
 Author-email: stngularity <stngularity@gmail.com>
 License: MIT License
-Project-URL: homepage, https://github.com/stngularity/tankioapi.py
-Project-URL: Source Code, https://github.com/stngularity/tankioapi.py
-Project-URL: changelog, https://github.com/stngularity/tankioapi.py/blob/main/CHANGELOG.md
-Project-URL: Bug Tracker, https://github.com/stngularity/tankioapi.py/issues
+Project-URL: homepage, https://github.com/stngularity/tankioapi
+Project-URL: Source Code, https://github.com/stngularity/tankioapi
+Project-URL: changelog, https://github.com/stngularity/tankioapi/blob/main/CHANGELOG.md
+Project-URL: Bug Tracker, https://github.com/stngularity/tankioapi/issues
 Keywords: game,api,to,tanki online
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -40,15 +40,15 @@
     <img src="https://img.shields.io/github/license/stngularity/tankioapi?color=%2346df11&label=License">
 </p>
 
 ## Notification
 This project was created just to exist. Of course, I will update it when the API itself changes, but not immediately. Well, if You want to support this project, You can give it a star.
 
 ## Information
-As mentioned earlier, this project is created just to exist. And so, the module itself is needed to get the top of players and get information about the player separately. If You know more functionality of the API of the game `Tanki Online`, then please report this functionality in the [`Issues`](/issues).
+As mentioned earlier, this project is created just to exist. And so, the module itself is needed to get the top of players and get information about the player separately. If You know more functionality of the API of the game `Tanki Online`, then please report this functionality in the [`Issues`](https://github.com/stngularity/tankioapi/issues).
 
 ###### Features
 - `async`/`await` support
 - Getting top of players
 - Getting information of any player by him name
 
 ## Installing
@@ -76,15 +76,15 @@
 > ```sh
 > $ git clone https://github.com/stngularity/tankioapi
 > $ cd tankioapi
 > $ python3 -m pip install -U .[speedup]
 > ```
 
 ## Examples
-Here are examples of some of the features of the library. More examples in [`examples/`](/blob/main/examples)
+Here are examples of some of the features of the library. More examples in [`examples/`](/examples)
 
 ###### Getting all tops of players
 ```py
 import asyncio
 from toapi import TankiOnline
 
 tops = asyncio.run(TankiOnline.get_tops())
@@ -112,8 +112,8 @@
 print(f"KD: {user.kills}/{user.deaths} ({round(user.kills/user.deaths, 2)})")
 print(f"Caught golds: {user.caught_golds}")
 print(f"Crystals: {user.crystals}")
 print(f"GS: {user.gear_score}")
 ```
 
 ## License
-This project is distributed under the `MIT` license. You can learn more from the [**LICENSE**](/blob/main/LICENSE) file.
+This project is distributed under the `MIT` license. You can learn more from the [**LICENSE**](/LICENSE) file.
```

### Comparing `tankioapi-0.1.0/src/toapi/__init__.py` & `tankioapi-0.1.2/src/toapi/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from .client import *
 from .errors import *
 
 __name__ = "tankio_api"
 __author__ = "stngularity"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023-present stngularity"
-__version__ = "0.1.0"
+__version__ = "0.1.2"
```

### Comparing `tankioapi-0.1.0/src/toapi/client.py` & `tankioapi-0.1.2/src/toapi/client.py`

 * *Files identical despite different names*

### Comparing `tankioapi-0.1.0/src/toapi/dataclasses/__init__.py` & `tankioapi-0.1.2/src/toapi/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `tankioapi-0.1.0/src/toapi/dataclasses/game_object.py` & `tankioapi-0.1.2/src/toapi/dataclasses/game_object.py`

 * *Files identical despite different names*

### Comparing `tankioapi-0.1.0/src/toapi/dataclasses/mode.py` & `tankioapi-0.1.2/src/toapi/dataclasses/mode.py`

 * *Files identical despite different names*

### Comparing `tankioapi-0.1.0/src/toapi/dataclasses/rank.py` & `tankioapi-0.1.2/src/toapi/dataclasses/rank.py`

 * *Files identical despite different names*

### Comparing `tankioapi-0.1.0/src/toapi/dataclasses/rating.py` & `tankioapi-0.1.2/src/toapi/dataclasses/rating.py`

 * *Files identical despite different names*

### Comparing `tankioapi-0.1.0/src/toapi/dataclasses/top.py` & `tankioapi-0.1.2/src/toapi/dataclasses/top.py`

 * *Files identical despite different names*

### Comparing `tankioapi-0.1.0/src/toapi/dataclasses/user.py` & `tankioapi-0.1.2/src/toapi/dataclasses/user.py`

 * *Files identical despite different names*

### Comparing `tankioapi-0.1.0/src/toapi/errors.py` & `tankioapi-0.1.2/src/toapi/errors.py`

 * *Files identical despite different names*

