# Comparing `tmp/SantorinAI-1.2.0.tar.gz` & `tmp/SantorinAI-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SantorinAI-1.2.0.tar", last modified: Sun May 14 15:58:43 2023, max compression
+gzip compressed data, was "SantorinAI-1.2.1.tar", last modified: Sun May 14 16:15:08 2023, max compression
```

## Comparing `SantorinAI-1.2.0.tar` & `SantorinAI-1.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:43.909122 SantorinAI-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-14 15:58:43.909122 SantorinAI-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:43.905122 SantorinAI-1.2.0/SantorinAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-14 15:58:43.000000 SantorinAI-1.2.0/SantorinAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 15:58:43.000000 SantorinAI-1.2.0/SantorinAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:58:43.000000 SantorinAI-1.2.0/SantorinAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 15:58:43.000000 SantorinAI-1.2.0/SantorinAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 15:58:43.000000 SantorinAI-1.2.0/SantorinAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:43.905122 SantorinAI-1.2.0/santorinai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:43.909122 SantorinAI-1.2.0/santorinai/board_displayer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/board_displayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/board_displayer/board_displayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/pawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:43.909122 SantorinAI-1.2.0/santorinai/player_examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/player_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/player_examples/first_choice_player.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/player_examples/random_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:58:43.909122 SantorinAI-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:43.909122 SantorinAI-1.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/test/test_board.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/test/test_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:15:08.352902 SantorinAI-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-14 16:15:08.352902 SantorinAI-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:15:08.352902 SantorinAI-1.2.1/SantorinAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-14 16:15:08.000000 SantorinAI-1.2.1/SantorinAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 16:15:08.000000 SantorinAI-1.2.1/SantorinAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:15:08.000000 SantorinAI-1.2.1/SantorinAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 16:15:08.000000 SantorinAI-1.2.1/SantorinAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 16:15:08.000000 SantorinAI-1.2.1/SantorinAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:15:08.352902 SantorinAI-1.2.1/santorinai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/santorinai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/santorinai/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:15:08.352902 SantorinAI-1.2.1/santorinai/board_displayer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/santorinai/board_displayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/santorinai/board_displayer/board_displayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/santorinai/pawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/santorinai/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:15:08.352902 SantorinAI-1.2.1/santorinai/player_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/santorinai/player_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/santorinai/player_examples/first_choice_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/santorinai/player_examples/random_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/santorinai/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:15:08.352902 SantorinAI-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:15:08.352902 SantorinAI-1.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19186 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/test/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-14 16:14:55.000000 SantorinAI-1.2.1/test/test_tester.py
```

### Comparing `SantorinAI-1.2.0/LICENSE` & `SantorinAI-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.0/PKG-INFO` & `SantorinAI-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.2.0/README.md` & `SantorinAI-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.0/SantorinAI.egg-info/PKG-INFO` & `SantorinAI-1.2.1/SantorinAI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.2.0/SantorinAI.egg-info/SOURCES.txt` & `SantorinAI-1.2.1/SantorinAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.0/santorinai/board.py` & `SantorinAI-1.2.1/santorinai/board.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,18 +317,14 @@
             return False, "The pawn has already been placed."
 
         # Check input
         ok, msg = self.is_position_valid(position)
         if not ok:
             return False, msg
 
-        # Check if the position is valid
-        if not self.is_position_within_board(position):
-            return False, "The position is not within the board bounds."
-
         # Check if the position is not occupied by another pawn
         if self.is_pawn_on_position(position):
             return False, "The position is already occupied by another pawn."
 
         # Get the pawn of the current player
         pawn = self.get_playing_pawn()
 
@@ -374,21 +370,21 @@
         # === MOVE ===
         # Check the input
         position_valid, reason = self.is_position_valid(move_position)
         if not position_valid:
             return False, reason
 
         # Check if the move is possible
-        initial_pos = pawn.pos
         move_possible, reason = self.is_move_possible(pawn.pos, move_position)
 
         if not move_possible:
             return False, reason
 
         # Apply the move
+        initial_pos = pawn.pos
         pawn.move(move_position)
 
         # Check if the tower is terminated
         if self.board[pawn.pos[0]][pawn.pos[1]] == 3:
             self.winner_player_number = pawn.player_number
             return True, "The move was played and the game is over."
```

### Comparing `SantorinAI-1.2.0/santorinai/board_displayer/board_displayer.py` & `SantorinAI-1.2.1/santorinai/board_displayer/board_displayer.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.0/santorinai/pawn.py` & `SantorinAI-1.2.1/santorinai/pawn.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.0/santorinai/player.py` & `SantorinAI-1.2.1/santorinai/player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.0/santorinai/player_examples/first_choice_player.py` & `SantorinAI-1.2.1/santorinai/player_examples/first_choice_player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.0/santorinai/player_examples/random_player.py` & `SantorinAI-1.2.1/santorinai/player_examples/random_player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.0/santorinai/tester.py` & `SantorinAI-1.2.1/santorinai/tester.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.0/setup.py` & `SantorinAI-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="SantorinAI",
-    version="1.2.0",
+    version="1.2.1",
     author="Tom Mansion",
     author_email="tomansion@yahoo.fr",
     description="A Python library for the Santorini board game",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tomansion/santorinai",
     packages=find_packages(),
```

### Comparing `SantorinAI-1.2.0/test/test_board.py` & `SantorinAI-1.2.1/test/test_board.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,19 +330,41 @@
         # 31 _0 _0 _0 _0
         # 10 41 _1 _0 _0
 
         # Pawn 1 has only one possible move
         possible_moves = board.get_possible_movement_positions(board.get_playing_pawn())
         self.assertEqual(len(possible_moves), 1)
         self.assertEqual(possible_moves[0], (1, 1))
-        # Pawn 1 has only one possible build
+        # Pawn 1 has only one possible build from this position
         possible_moves = board.get_possible_building_positions(board.get_playing_pawn())
         self.assertEqual(len(possible_moves), 1)
         self.assertEqual(possible_moves[0], (1, 1))
-        print(board)
+
+        # Tests that a valid move with an invalid build is not allowed
+        # and that the pawn is not moved
+        move_ok, _ = board.play_move((1, 1), (0, 1))
+        self.assertFalse(move_ok)
+        self.assertEqual(board.pawn_turn, 1)
+        self.assertEqual(board.pawns[0].pos, (0, 0))
+        move_ok, _ = board.play_move((1, 1), (1, 1))
+        self.assertFalse(move_ok)
+        self.assertEqual(board.pawn_turn, 1)
+        self.assertEqual(board.pawns[0].pos, (0, 0))
+        move_ok, _ = board.play_move((1, 1), ("haha", "hoho"))
+        self.assertFalse(move_ok)
+        self.assertEqual(board.pawn_turn, 1)
+        self.assertEqual(board.pawns[0].pos, (0, 0))
+        move_ok, _ = board.play_move((1, 1), "test")
+        self.assertFalse(move_ok)
+        self.assertEqual(board.pawn_turn, 1)
+        self.assertEqual(board.pawns[0].pos, (0, 0))
+        move_ok, _ = board.play_move((1, 1), (2, 2, 2))
+        self.assertFalse(move_ok)
+        self.assertEqual(board.pawn_turn, 1)
+        self.assertEqual(board.pawns[0].pos, (0, 0))
 
         # Make every one stuck
         self.assertFalse(board.is_everyone_stuck())
         self.assertFalse(board.is_game_over())
         board.board[0][3] = 4
         board.board[1][3] = 4
         board.board[1][2] = 4
@@ -437,7 +459,35 @@
         self.assertTrue(board.is_game_over())
         self.assertTrue(board.is_everyone_stuck())
         self.assertEqual(board.winner_player_number, 1)  # The last player who played
 
         # What a waste of time
         print(board)
         print(board.pawns[0])
+
+    def test_get_possible_movement_and_building_positions(self):
+        board = Board(self.NB_PLAYERS)
+
+        # At first, all positions are free
+        all_possible_moves = board.get_possible_movement_and_building_positions(
+            board.get_playing_pawn()
+        )
+        self.assertEqual(len(all_possible_moves), 25)
+        board.place_pawn((2, 2))
+
+        # Pawn 1 has many possible moves
+        all_possible_moves = board.get_possible_movement_and_building_positions(
+            board.pawns[0]
+        )
+
+        print(all_possible_moves)
+        print(len(all_possible_moves))
+
+        self.assertGreater(len(all_possible_moves), 50)
+
+        # Pawn 2 has one less placement
+        all_possible_moves = board.get_possible_movement_and_building_positions(
+            board.get_playing_pawn()
+        )
+        self.assertEqual(len(all_possible_moves), 24)
+        board.place_pawn((3, 2))
+
```

### Comparing `SantorinAI-1.2.0/test/test_tester.py` & `SantorinAI-1.2.1/test/test_tester.py`

 * *Files identical despite different names*

