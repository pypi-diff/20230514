# Comparing `tmp/SantorinAI-1.2.2.tar.gz` & `tmp/SantorinAI-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SantorinAI-1.2.2.tar", last modified: Sun May 14 16:41:42 2023, max compression
+gzip compressed data, was "SantorinAI-1.2.3.tar", last modified: Sun May 14 16:50:18 2023, max compression
```

## Comparing `SantorinAI-1.2.2.tar` & `SantorinAI-1.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:41:42.950183 SantorinAI-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-14 16:41:42.950183 SantorinAI-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:41:42.950183 SantorinAI-1.2.2/SantorinAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-14 16:41:42.000000 SantorinAI-1.2.2/SantorinAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 16:41:42.000000 SantorinAI-1.2.2/SantorinAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:41:42.000000 SantorinAI-1.2.2/SantorinAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 16:41:42.000000 SantorinAI-1.2.2/SantorinAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 16:41:42.000000 SantorinAI-1.2.2/SantorinAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:41:42.950183 SantorinAI-1.2.2/santorinai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/santorinai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/santorinai/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:41:42.950183 SantorinAI-1.2.2/santorinai/board_displayer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/santorinai/board_displayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/santorinai/board_displayer/board_displayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/santorinai/pawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/santorinai/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:41:42.950183 SantorinAI-1.2.2/santorinai/player_examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/santorinai/player_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/santorinai/player_examples/first_choice_player.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/santorinai/player_examples/random_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/santorinai/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:41:42.950183 SantorinAI-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:41:42.950183 SantorinAI-1.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/test/test_board.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-14 16:41:32.000000 SantorinAI-1.2.2/test/test_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:18.732221 SantorinAI-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-14 16:50:18.732221 SantorinAI-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:18.728222 SantorinAI-1.2.3/SantorinAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-14 16:50:18.000000 SantorinAI-1.2.3/SantorinAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 16:50:18.000000 SantorinAI-1.2.3/SantorinAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:50:18.000000 SantorinAI-1.2.3/SantorinAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 16:50:18.000000 SantorinAI-1.2.3/SantorinAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 16:50:18.000000 SantorinAI-1.2.3/SantorinAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:18.728222 SantorinAI-1.2.3/santorinai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:18.728222 SantorinAI-1.2.3/santorinai/board_displayer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/board_displayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/board_displayer/board_displayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/pawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:18.728222 SantorinAI-1.2.3/santorinai/player_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/player_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/player_examples/first_choice_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/player_examples/random_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:50:18.732221 SantorinAI-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:18.732221 SantorinAI-1.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/test/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/test/test_tester.py
```

### Comparing `SantorinAI-1.2.2/LICENSE` & `SantorinAI-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.2/PKG-INFO` & `SantorinAI-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.2.2/README.md` & `SantorinAI-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.2/SantorinAI.egg-info/PKG-INFO` & `SantorinAI-1.2.3/SantorinAI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.2.2/SantorinAI.egg-info/SOURCES.txt` & `SantorinAI-1.2.3/SantorinAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.2/santorinai/board.py` & `SantorinAI-1.2.3/santorinai/board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.2/santorinai/board_displayer/board_displayer.py` & `SantorinAI-1.2.3/santorinai/board_displayer/board_displayer.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.2/santorinai/pawn.py` & `SantorinAI-1.2.3/santorinai/pawn.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.2/santorinai/player.py` & `SantorinAI-1.2.3/santorinai/player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.2/santorinai/player_examples/first_choice_player.py` & `SantorinAI-1.2.3/santorinai/player_examples/first_choice_player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.2/santorinai/player_examples/random_player.py` & `SantorinAI-1.2.3/santorinai/player_examples/random_player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.2/santorinai/tester.py` & `SantorinAI-1.2.3/santorinai/tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
             while not board.is_game_over():
                 current_pawn = board.get_playing_pawn()
                 self.display_message(f"   Current pawn: {current_pawn}", 2)
 
                 # Check if the player can move
                 if len(board.get_possible_movement_positions(current_pawn)) == 0:
                     self.display_message(f"   The pawn cannot move", 2)
+                    board.next_turn()
                     # We don't ask the player to move, we just skip his turn
                     continue
 
                 board_copy = board.copy()
                 current_pawn_copy = board_copy.get_playing_pawn()
 
                 # Ask the player where to move the pawn
```

### Comparing `SantorinAI-1.2.2/setup.py` & `SantorinAI-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="SantorinAI",
-    version="1.2.2",
+    version="1.2.3",
     author="Tom Mansion",
     author_email="tomansion@yahoo.fr",
     description="A Python library for the Santorini board game",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tomansion/santorinai",
     packages=find_packages(),
```

### Comparing `SantorinAI-1.2.2/test/test_board.py` & `SantorinAI-1.2.3/test/test_board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.2/test/test_tester.py` & `SantorinAI-1.2.3/test/test_tester.py`

 * *Files identical despite different names*

