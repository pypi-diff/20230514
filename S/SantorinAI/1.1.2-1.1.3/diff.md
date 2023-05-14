# Comparing `tmp/SantorinAI-1.1.2.tar.gz` & `tmp/SantorinAI-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SantorinAI-1.1.2.tar", last modified: Sun May 14 13:43:37 2023, max compression
+gzip compressed data, was "SantorinAI-1.1.3.tar", last modified: Sun May 14 14:54:14 2023, max compression
```

## Comparing `SantorinAI-1.1.2.tar` & `SantorinAI-1.1.3.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/SantorinAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-14 13:43:37.000000 SantorinAI-1.1.2/SantorinAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-14 13:43:37.000000 SantorinAI-1.1.2/SantorinAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 13:43:37.000000 SantorinAI-1.1.2/SantorinAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 13:43:37.000000 SantorinAI-1.1.2/SantorinAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 13:43:37.000000 SantorinAI-1.1.2/SantorinAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/santorinai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17372 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/santorinai/board_displayer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/board_displayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/board_displayer/board_displayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/pawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/test/test_board.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/test/test_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/SantorinAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-14 14:54:14.000000 SantorinAI-1.1.3/SantorinAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 14:54:14.000000 SantorinAI-1.1.3/SantorinAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:54:14.000000 SantorinAI-1.1.3/SantorinAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 14:54:14.000000 SantorinAI-1.1.3/SantorinAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 14:54:14.000000 SantorinAI-1.1.3/SantorinAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/santorinai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17372 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/santorinai/board_displayer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/board_displayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/board_displayer/board_displayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/pawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/santorinai/player_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/player_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/player_examples/first_choice_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/player_examples/random_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/test/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/test/test_tester.py
```

### Comparing `SantorinAI-1.1.2/LICENSE` & `SantorinAI-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.2/PKG-INFO` & `SantorinAI-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -19,15 +19,15 @@
 AI Player tester for the Santorini game
 
 ## How to use
 ### 1. Install
 
 With pip:
 ```bash
-pip install santorinai --upgrade
+pip install --upgrade santorinai
 ```
 
 You can also clone the repository and install it manually:
 ```bash
 git clone https://github.com/Tomansion/SantorinAI.git
 cd SantorinAI
 pip install -r requirements.txt
@@ -72,21 +72,21 @@
         # Do some magic here to choose a position
         my_move_vector = (1, 1) # Moving top right
         my_build_vector = (1, 0) # Building right (relative to the new position)
 
         return my_move_vector, my_build_vector
 ```
 
-Check our random players example in [our player examples folder](./player_examples/)  to help you create your own.
+Check our random players example in [our player examples folder](./santorinai/player_examples/)  to help you create your own.
 
 ### 3. Test your player
 
 ```python
 from santorinai.tester import Tester
-from player_examples.random_player import RandomPlayer
+from santorinai.player_examples.random_player import RandomPlayer
 from my_player import MyPlayer
 
 # Init the tester
 tester = Tester()
 tester.verbose_level = 2 # 0: no output, 1: Each game results, 2: Each move summary
 tester.delay_between_moves = 0.1 # Delay between each move in seconds
 tester.display_board = True # Display a graphical view of the board in a window
```

### Comparing `SantorinAI-1.1.2/README.md` & `SantorinAI-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 AI Player tester for the Santorini game
 
 ## How to use
 ### 1. Install
 
 With pip:
 ```bash
-pip install santorinai --upgrade
+pip install --upgrade santorinai
 ```
 
 You can also clone the repository and install it manually:
 ```bash
 git clone https://github.com/Tomansion/SantorinAI.git
 cd SantorinAI
 pip install -r requirements.txt
@@ -57,21 +57,21 @@
         # Do some magic here to choose a position
         my_move_vector = (1, 1) # Moving top right
         my_build_vector = (1, 0) # Building right (relative to the new position)
 
         return my_move_vector, my_build_vector
 ```
 
-Check our random players example in [our player examples folder](./player_examples/)  to help you create your own.
+Check our random players example in [our player examples folder](./santorinai/player_examples/)  to help you create your own.
 
 ### 3. Test your player
 
 ```python
 from santorinai.tester import Tester
-from player_examples.random_player import RandomPlayer
+from santorinai.player_examples.random_player import RandomPlayer
 from my_player import MyPlayer
 
 # Init the tester
 tester = Tester()
 tester.verbose_level = 2 # 0: no output, 1: Each game results, 2: Each move summary
 tester.delay_between_moves = 0.1 # Delay between each move in seconds
 tester.display_board = True # Display a graphical view of the board in a window
```

### Comparing `SantorinAI-1.1.2/SantorinAI.egg-info/PKG-INFO` & `SantorinAI-1.1.3/SantorinAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -19,15 +19,15 @@
 AI Player tester for the Santorini game
 
 ## How to use
 ### 1. Install
 
 With pip:
 ```bash
-pip install santorinai --upgrade
+pip install --upgrade santorinai
 ```
 
 You can also clone the repository and install it manually:
 ```bash
 git clone https://github.com/Tomansion/SantorinAI.git
 cd SantorinAI
 pip install -r requirements.txt
@@ -72,21 +72,21 @@
         # Do some magic here to choose a position
         my_move_vector = (1, 1) # Moving top right
         my_build_vector = (1, 0) # Building right (relative to the new position)
 
         return my_move_vector, my_build_vector
 ```
 
-Check our random players example in [our player examples folder](./player_examples/)  to help you create your own.
+Check our random players example in [our player examples folder](./santorinai/player_examples/)  to help you create your own.
 
 ### 3. Test your player
 
 ```python
 from santorinai.tester import Tester
-from player_examples.random_player import RandomPlayer
+from santorinai.player_examples.random_player import RandomPlayer
 from my_player import MyPlayer
 
 # Init the tester
 tester = Tester()
 tester.verbose_level = 2 # 0: no output, 1: Each game results, 2: Each move summary
 tester.delay_between_moves = 0.1 # Delay between each move in seconds
 tester.display_board = True # Display a graphical view of the board in a window
```

### Comparing `SantorinAI-1.1.2/santorinai/board.py` & `SantorinAI-1.1.3/santorinai/board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.2/santorinai/board_displayer/board_displayer.py` & `SantorinAI-1.1.3/santorinai/board_displayer/board_displayer.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.2/santorinai/pawn.py` & `SantorinAI-1.1.3/santorinai/pawn.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.2/santorinai/player.py` & `SantorinAI-1.1.3/santorinai/player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.2/santorinai/tester.py` & `SantorinAI-1.1.3/santorinai/tester.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.2/setup.py` & `SantorinAI-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="SantorinAI",
-    version="1.1.2",
+    version="1.1.3",
     author="Tom Mansion",
     author_email="tomansion@yahoo.fr",
     description="A Python library for the Santorini board game",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tomansion/santorinai",
     packages=find_packages(),
```

### Comparing `SantorinAI-1.1.2/test/test_board.py` & `SantorinAI-1.1.3/test/test_board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.2/test/test_tester.py` & `SantorinAI-1.1.3/test/test_tester.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Test file for tester.py
 
 import unittest
 
 from santorinai.tester import Tester
-from player_examples.random_player import RandomPlayer
-from player_examples.first_choice_player import FirstChoicePlayer
+from santorinai.player_examples.random_player import RandomPlayer
+from santorinai.player_examples.first_choice_player import FirstChoicePlayer
 
 
 class TestTester(unittest.TestCase):
     def test_play_1v1_bad_players(self):
         tester = Tester()
         player1 = "Test"
         player2 = "Test"
```

