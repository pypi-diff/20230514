# Comparing `tmp/SantorinAI-1.2.3.tar.gz` & `tmp/SantorinAI-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SantorinAI-1.2.3.tar", last modified: Sun May 14 16:50:18 2023, max compression
+gzip compressed data, was "SantorinAI-1.2.4.tar", last modified: Sun May 14 17:18:17 2023, max compression
```

## Comparing `SantorinAI-1.2.3.tar` & `SantorinAI-1.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:18.732221 SantorinAI-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-14 16:50:18.732221 SantorinAI-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:18.728222 SantorinAI-1.2.3/SantorinAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-14 16:50:18.000000 SantorinAI-1.2.3/SantorinAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 16:50:18.000000 SantorinAI-1.2.3/SantorinAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:50:18.000000 SantorinAI-1.2.3/SantorinAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 16:50:18.000000 SantorinAI-1.2.3/SantorinAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 16:50:18.000000 SantorinAI-1.2.3/SantorinAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:18.728222 SantorinAI-1.2.3/santorinai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:18.728222 SantorinAI-1.2.3/santorinai/board_displayer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/board_displayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/board_displayer/board_displayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/pawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:18.728222 SantorinAI-1.2.3/santorinai/player_examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/player_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/player_examples/first_choice_player.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/player_examples/random_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/santorinai/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:50:18.732221 SantorinAI-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:18.732221 SantorinAI-1.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/test/test_board.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-14 16:50:05.000000 SantorinAI-1.2.3/test/test_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:18:17.906987 SantorinAI-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-14 17:18:17.906987 SantorinAI-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:18:17.898986 SantorinAI-1.2.4/SantorinAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-14 17:18:17.000000 SantorinAI-1.2.4/SantorinAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 17:18:17.000000 SantorinAI-1.2.4/SantorinAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:18:17.000000 SantorinAI-1.2.4/SantorinAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 17:18:17.000000 SantorinAI-1.2.4/SantorinAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 17:18:17.000000 SantorinAI-1.2.4/SantorinAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:18:17.902987 SantorinAI-1.2.4/santorinai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/santorinai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/santorinai/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:18:17.902987 SantorinAI-1.2.4/santorinai/board_displayer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/santorinai/board_displayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/santorinai/board_displayer/board_displayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/santorinai/pawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/santorinai/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:18:17.902987 SantorinAI-1.2.4/santorinai/player_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/santorinai/player_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/santorinai/player_examples/first_choice_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/santorinai/player_examples/random_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/santorinai/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:18:17.906987 SantorinAI-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:18:17.906987 SantorinAI-1.2.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/test/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-14 17:18:06.000000 SantorinAI-1.2.4/test/test_tester.py
```

### Comparing `SantorinAI-1.2.3/LICENSE` & `SantorinAI-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.3/PKG-INFO` & `SantorinAI-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.2.3/README.md` & `SantorinAI-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.3/SantorinAI.egg-info/PKG-INFO` & `SantorinAI-1.2.4/SantorinAI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.2.3/SantorinAI.egg-info/SOURCES.txt` & `SantorinAI-1.2.4/SantorinAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.3/santorinai/board.py` & `SantorinAI-1.2.4/santorinai/board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.3/santorinai/board_displayer/board_displayer.py` & `SantorinAI-1.2.4/santorinai/board_displayer/board_displayer.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.3/santorinai/pawn.py` & `SantorinAI-1.2.4/santorinai/pawn.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.3/santorinai/player.py` & `SantorinAI-1.2.4/santorinai/player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.3/santorinai/player_examples/first_choice_player.py` & `SantorinAI-1.2.4/santorinai/player_examples/first_choice_player.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,22 @@
         return my_choice
 
     def play_move(self, board, pawn):
         my_initial_position = pawn.pos
 
         # Get movement positions
         available_positions = board.get_possible_movement_positions(pawn)
+        if len(available_positions) == 0:
+            # The pawn cannot move
+            return None, None
+
         my_move_choice = available_positions[0]
 
         # Simulate the move (this will not impact the actual board)
         pawn.move(my_move_choice)
 
         # Get construction positions
         available_positions = board.get_possible_building_positions(pawn)
+        # Their is always at least one position available
         my_build_choice = available_positions[0]
 
         return my_move_choice, my_build_choice
```

### Comparing `SantorinAI-1.2.3/santorinai/player_examples/random_player.py` & `SantorinAI-1.2.4/santorinai/player_examples/random_player.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,18 @@
         return my_choice
 
     def play_move(self, board, pawn):
         my_initial_position = pawn.pos
 
         # Get movement positions
         available_positions = board.get_possible_movement_positions(pawn)
+        if len(available_positions) == 0:
+            # The pawn cannot move
+            return None, None
+
         my_move_choice = choice(available_positions)
 
         # Simulate the move
         pawn.move(my_move_choice)
 
         # Get construction positions for the new position
         available_positions = board.get_possible_building_positions(pawn)
```

### Comparing `SantorinAI-1.2.3/santorinai/tester.py` & `SantorinAI-1.2.4/santorinai/tester.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.3/setup.py` & `SantorinAI-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="SantorinAI",
-    version="1.2.3",
+    version="1.2.4",
     author="Tom Mansion",
     author_email="tomansion@yahoo.fr",
     description="A Python library for the Santorini board game",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tomansion/santorinai",
     packages=find_packages(),
```

### Comparing `SantorinAI-1.2.3/test/test_board.py` & `SantorinAI-1.2.4/test/test_board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.3/test/test_tester.py` & `SantorinAI-1.2.4/test/test_tester.py`

 * *Files identical despite different names*

