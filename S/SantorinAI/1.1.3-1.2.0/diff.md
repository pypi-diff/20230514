# Comparing `tmp/SantorinAI-1.1.3.tar.gz` & `tmp/SantorinAI-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SantorinAI-1.1.3.tar", last modified: Sun May 14 14:54:14 2023, max compression
+gzip compressed data, was "SantorinAI-1.2.0.tar", last modified: Sun May 14 15:58:43 2023, max compression
```

## Comparing `SantorinAI-1.1.3.tar` & `SantorinAI-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/SantorinAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-14 14:54:14.000000 SantorinAI-1.1.3/SantorinAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 14:54:14.000000 SantorinAI-1.1.3/SantorinAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:54:14.000000 SantorinAI-1.1.3/SantorinAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 14:54:14.000000 SantorinAI-1.1.3/SantorinAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 14:54:14.000000 SantorinAI-1.1.3/SantorinAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/santorinai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17372 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/santorinai/board_displayer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/board_displayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/board_displayer/board_displayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/pawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/santorinai/player_examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/player_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/player_examples/first_choice_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/player_examples/random_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/santorinai/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:14.900063 SantorinAI-1.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/test/test_board.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-14 14:54:04.000000 SantorinAI-1.1.3/test/test_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:43.909122 SantorinAI-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-14 15:58:43.909122 SantorinAI-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:43.905122 SantorinAI-1.2.0/SantorinAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-14 15:58:43.000000 SantorinAI-1.2.0/SantorinAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 15:58:43.000000 SantorinAI-1.2.0/SantorinAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:58:43.000000 SantorinAI-1.2.0/SantorinAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 15:58:43.000000 SantorinAI-1.2.0/SantorinAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 15:58:43.000000 SantorinAI-1.2.0/SantorinAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:43.905122 SantorinAI-1.2.0/santorinai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:43.909122 SantorinAI-1.2.0/santorinai/board_displayer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/board_displayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/board_displayer/board_displayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/pawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:43.909122 SantorinAI-1.2.0/santorinai/player_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/player_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/player_examples/first_choice_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/player_examples/random_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/santorinai/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:58:43.909122 SantorinAI-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:43.909122 SantorinAI-1.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/test/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-14 15:58:33.000000 SantorinAI-1.2.0/test/test_tester.py
```

### Comparing `SantorinAI-1.1.3/LICENSE` & `SantorinAI-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.3/PKG-INFO` & `SantorinAI-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.1.3
+Version: 1.2.0
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -56,28 +56,37 @@
         # Do some magic here to choose a position
         my_choice = (2, 3) # A position on the 5x5 board
 
         return my_choice
 
     # Movement and building
     def play_move(self, board, pawn):
-        my_initial_position = pawn.pos
+        my_pawn_pos = pawn.pos
 
         board_array = board.board # A 5x5 array of integers representing the board
         # 0: empty
         # 1: tower level 1
         # 2: tower level 2
         # 3: tower level 3
         # 4: terminated tower
 
+        pawns = board.pawns # The other pawns on the board
+
         # Do some magic here to choose a position
-        my_move_vector = (1, 1) # Moving top right
-        my_build_vector = (1, 0) # Building right (relative to the new position)
+        my_move_position = ( # Moving top right
+            my_pawn_pos[0] + 1, 
+            my_pawn_pos[1] + 1
+        ) 
+
+        my_build_position = ( # Building right (relative to the new position)
+            my_move_position[0] + 1, 
+            my_move_position[1] + 0
+        ) 
 
-        return my_move_vector, my_build_vector
+        return my_move_position, my_build_position
 ```
 
 Check our random players example in [our player examples folder](./santorinai/player_examples/)  to help you create your own.
 
 ### 3. Test your player
 
 ```python
@@ -136,25 +145,30 @@
 
 # Movements
 available_move_positions = board.get_possible_movement_positions(pawn)
 available_build_positions = board.get_possible_building_positions(pawn)
 
 # Board control
 board.place_pawn(pos) # Place the current playing pawn on the board
-board.play_move(move_vector, build_vector) # Play a move (move and build) with the current playing pawn
+board.play_move(move_position, build_position) # Play a move (move and build) with the current playing pawn
 
 # Other
-board.is_vector_valid(vector)
+board.is_position_valid(position)
 board.is_move_possible(start_pos, end_pos)
 board.is_position_within_board(pos)
 board.is_position_adjacent(pos1, pos2)
 board.is_pawn_on_position(pos)
 board.is_build_possible(builder_pos, build_pos)
 board.copy() # Create a copy of the board, useful to test moves
 print(board) # Print the board
+
+# Display
+from santorinai.board_displayer.board_displayer import init_window, update_board
+window = init_window([player1.name(), player2.name()])
+update_board(window, board)
 ```
 
 ## Credits
 
 Creator of Santorini: [Roxley Games](https://roxley.com/)
 
 Board 2D Gui library: [PySimpleGUI](https://www.pysimplegui.org/en/latest/)
```

### Comparing `SantorinAI-1.1.3/README.md` & `SantorinAI-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -41,28 +41,37 @@
         # Do some magic here to choose a position
         my_choice = (2, 3) # A position on the 5x5 board
 
         return my_choice
 
     # Movement and building
     def play_move(self, board, pawn):
-        my_initial_position = pawn.pos
+        my_pawn_pos = pawn.pos
 
         board_array = board.board # A 5x5 array of integers representing the board
         # 0: empty
         # 1: tower level 1
         # 2: tower level 2
         # 3: tower level 3
         # 4: terminated tower
 
+        pawns = board.pawns # The other pawns on the board
+
         # Do some magic here to choose a position
-        my_move_vector = (1, 1) # Moving top right
-        my_build_vector = (1, 0) # Building right (relative to the new position)
+        my_move_position = ( # Moving top right
+            my_pawn_pos[0] + 1, 
+            my_pawn_pos[1] + 1
+        ) 
+
+        my_build_position = ( # Building right (relative to the new position)
+            my_move_position[0] + 1, 
+            my_move_position[1] + 0
+        ) 
 
-        return my_move_vector, my_build_vector
+        return my_move_position, my_build_position
 ```
 
 Check our random players example in [our player examples folder](./santorinai/player_examples/)  to help you create your own.
 
 ### 3. Test your player
 
 ```python
@@ -121,25 +130,30 @@
 
 # Movements
 available_move_positions = board.get_possible_movement_positions(pawn)
 available_build_positions = board.get_possible_building_positions(pawn)
 
 # Board control
 board.place_pawn(pos) # Place the current playing pawn on the board
-board.play_move(move_vector, build_vector) # Play a move (move and build) with the current playing pawn
+board.play_move(move_position, build_position) # Play a move (move and build) with the current playing pawn
 
 # Other
-board.is_vector_valid(vector)
+board.is_position_valid(position)
 board.is_move_possible(start_pos, end_pos)
 board.is_position_within_board(pos)
 board.is_position_adjacent(pos1, pos2)
 board.is_pawn_on_position(pos)
 board.is_build_possible(builder_pos, build_pos)
 board.copy() # Create a copy of the board, useful to test moves
 print(board) # Print the board
+
+# Display
+from santorinai.board_displayer.board_displayer import init_window, update_board
+window = init_window([player1.name(), player2.name()])
+update_board(window, board)
 ```
 
 ## Credits
 
 Creator of Santorini: [Roxley Games](https://roxley.com/)
 
 Board 2D Gui library: [PySimpleGUI](https://www.pysimplegui.org/en/latest/)
```

### Comparing `SantorinAI-1.1.3/SantorinAI.egg-info/PKG-INFO` & `SantorinAI-1.2.0/SantorinAI.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.1.3
+Version: 1.2.0
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -56,28 +56,37 @@
         # Do some magic here to choose a position
         my_choice = (2, 3) # A position on the 5x5 board
 
         return my_choice
 
     # Movement and building
     def play_move(self, board, pawn):
-        my_initial_position = pawn.pos
+        my_pawn_pos = pawn.pos
 
         board_array = board.board # A 5x5 array of integers representing the board
         # 0: empty
         # 1: tower level 1
         # 2: tower level 2
         # 3: tower level 3
         # 4: terminated tower
 
+        pawns = board.pawns # The other pawns on the board
+
         # Do some magic here to choose a position
-        my_move_vector = (1, 1) # Moving top right
-        my_build_vector = (1, 0) # Building right (relative to the new position)
+        my_move_position = ( # Moving top right
+            my_pawn_pos[0] + 1, 
+            my_pawn_pos[1] + 1
+        ) 
+
+        my_build_position = ( # Building right (relative to the new position)
+            my_move_position[0] + 1, 
+            my_move_position[1] + 0
+        ) 
 
-        return my_move_vector, my_build_vector
+        return my_move_position, my_build_position
 ```
 
 Check our random players example in [our player examples folder](./santorinai/player_examples/)  to help you create your own.
 
 ### 3. Test your player
 
 ```python
@@ -136,25 +145,30 @@
 
 # Movements
 available_move_positions = board.get_possible_movement_positions(pawn)
 available_build_positions = board.get_possible_building_positions(pawn)
 
 # Board control
 board.place_pawn(pos) # Place the current playing pawn on the board
-board.play_move(move_vector, build_vector) # Play a move (move and build) with the current playing pawn
+board.play_move(move_position, build_position) # Play a move (move and build) with the current playing pawn
 
 # Other
-board.is_vector_valid(vector)
+board.is_position_valid(position)
 board.is_move_possible(start_pos, end_pos)
 board.is_position_within_board(pos)
 board.is_position_adjacent(pos1, pos2)
 board.is_pawn_on_position(pos)
 board.is_build_possible(builder_pos, build_pos)
 board.copy() # Create a copy of the board, useful to test moves
 print(board) # Print the board
+
+# Display
+from santorinai.board_displayer.board_displayer import init_window, update_board
+window = init_window([player1.name(), player2.name()])
+update_board(window, board)
 ```
 
 ## Credits
 
 Creator of Santorini: [Roxley Games](https://roxley.com/)
 
 Board 2D Gui library: [PySimpleGUI](https://www.pysimplegui.org/en/latest/)
```

### Comparing `SantorinAI-1.1.3/SantorinAI.egg-info/SOURCES.txt` & `SantorinAI-1.2.0/SantorinAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.3/santorinai/board.py` & `SantorinAI-1.2.0/santorinai/board.py`

 * *Files 9% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 
         # Check if the build position is not occupied by another pawn
         if self.is_pawn_on_position(build_position):
             return False, "It is not possible to build on another pawn."
 
         return True, "The build is possible."
 
-    def get_playing_pawn(self):
+    def get_playing_pawn(self) -> Pawn:
         """
         Gets the pawn of the current player.
 
         Returns:
             Pawn: The pawn of the current player.
         """
         return self.pawns[self.pawn_turn - 1]
@@ -267,14 +267,40 @@
                     pawn.pos, (pawn.pos[0] + x, pawn.pos[1] + y)
                 )
                 if build_possible:
                     possible_builds.append((pawn.pos[0] + x, pawn.pos[1] + y))
 
         return possible_builds
 
+    def get_possible_movement_and_building_positions(self, pawn: Pawn):
+        """
+        Gets all the possible moves and builds for a given pawn.
+        :param pawn: The pawn for which to get the possible moves and builds.
+        :return: A list of all the possible moves and builds for the given pawn.
+        [(move_position, build_position), ...]
+        """
+
+        if pawn.pos == (None, None):
+            # Pawn not placed yet
+            possible_spawn_positions = self.get_possible_movement_positions(pawn)
+            return [(position, None) for position in possible_spawn_positions]
+
+        possible_moves = self.get_possible_movement_positions(pawn)
+
+        possible_moves_and_builds = []
+        original_position = pawn.pos
+        for move in possible_moves:
+            pawn.move(move)
+            possible_builds = self.get_possible_building_positions(pawn)
+            for build in possible_builds:
+                possible_moves_and_builds.append((move, build))
+
+        pawn.move(original_position)
+        return possible_moves_and_builds
+
     def place_pawn(self, position: Tuple[int, int]) -> Tuple[bool, str]:
         """
         Places a pawn on the board.
 
         Args:
             position (tuple): The position [x, y] to place the pawn.
 
@@ -286,14 +312,19 @@
         if self.is_game_over():
             return False, "The game is over."
 
         # Check if the pawn has already been placed
         if self.get_playing_pawn().pos != (None, None):
             return False, "The pawn has already been placed."
 
+        # Check input
+        ok, msg = self.is_position_valid(position)
+        if not ok:
+            return False, msg
+
         # Check if the position is valid
         if not self.is_position_within_board(position):
             return False, "The position is not within the board bounds."
 
         # Check if the position is not occupied by another pawn
         if self.is_pawn_on_position(position):
             return False, "The position is already occupied by another pawn."
@@ -306,22 +337,22 @@
 
         # Next player's turn
         self.next_turn()
 
         return True, "The pawn was placed."
 
     def play_move(
-        self, move_vector: Tuple[int, int], build_vector: Tuple[int, int]
+        self, move_position: Tuple[int, int], build_position: Tuple[int, int]
     ) -> Tuple[bool, str]:
         """
         Plays a move on the board with the current playing pawn.
 
         Args:
-            move_vector (tuple): The displacement vector [x, y] to apply to the pawn, (-1, 1) for example.
-            build_vector (tuple): The build vector [x, y] to apply to the pawn, (-1, 1) for example.
+            move_position (tuple): The position (x, y) to move the pawn to.
+            build_position (tuple): The position (x, y) to build a tower on.
 
         Returns:
             bool: True if the move was played, False otherwise.
             str: A string describing why the move was not played.
         """
         # Check if the game is over
         if self.is_game_over():
@@ -330,116 +361,103 @@
         # Get the pawn of the current player
         pawn = self.get_playing_pawn()
 
         # Check if the pawn has been placed
         if pawn.pos == (None, None):
             return False, "The pawn has not been placed yet."
 
-        # Check if their is any possible move
+        # Check if there is any possible move
         possible_moves = self.get_possible_movement_positions(pawn)
         if len(possible_moves) == 0:
             self.next_turn()
             return True, "There is no possible move to play, the pawn is stuck."
 
         # === MOVE ===
-        # Check if the vector is valid
-        disp_vector_valid, reason = self.is_vector_valid(move_vector)
-        if not disp_vector_valid:
+        # Check the input
+        position_valid, reason = self.is_position_valid(move_position)
+        if not position_valid:
             return False, reason
 
         # Check if the move is possible
         initial_pos = pawn.pos
-        new_pos = (
-            pawn.pos[0] + move_vector[0],
-            pawn.pos[1] + move_vector[1],
-        )
-        move_possible, reason = self.is_move_possible(pawn.pos, new_pos)
+        move_possible, reason = self.is_move_possible(pawn.pos, move_position)
 
         if not move_possible:
             return False, reason
 
         # Apply the move
-        pawn.move(new_pos)
+        pawn.move(move_position)
 
         # Check if the tower is terminated
         if self.board[pawn.pos[0]][pawn.pos[1]] == 3:
             self.winner_player_number = pawn.player_number
             return True, "The move was played and the game is over."
 
         # === BUILD ===
-        # Check if the vector is valid
-        const_vector_valid, reason = self.is_vector_valid(build_vector)
-        if not const_vector_valid:
+        # Check the input
+        position_valid, reason = self.is_position_valid(build_position)
+        if not position_valid:
             # Reverse the move
             pawn.move(initial_pos)
             return False, reason
 
-        # Check if their is any possible build
-        # No need to check, it is always possible to build after a move
+        # Check if there is any possible build
+        # > No need to check, it is always possible to build after a move (we can always build on the initial position)
 
         # Check if the build is possible
-        build_pos = (
-            pawn.pos[0] + build_vector[0],
-            pawn.pos[1] + build_vector[1],
-        )
-
-        build_possible, reason = self.is_build_possible(pawn.pos, build_pos)
+        build_possible, reason = self.is_build_possible(pawn.pos, build_position)
 
         if not build_possible:
             # The move was played but the build is not possible
             # Reverse the move
             pawn.move(initial_pos)
             return False, reason
 
         # Build the tower
-        self.board[build_pos[0]][build_pos[1]] += 1
+        self.board[build_position[0]][build_position[1]] += 1
 
         if self.is_everyone_stuck():
             self.winner_player_number = pawn.player_number
             return True, "No one can play, the game is over."
 
         # Change the turn
         self.next_turn()
 
         return True, "The move was played."
 
-    def is_vector_valid(self, vector: Tuple[int, int]):
+    def is_position_valid(self, pos: Tuple[int, int]):
         """
-        Checks if a vector is valid.
+        Checks if a pos is valid.
 
         Args:
-            vector (tuple): The vector to check.
+            pos (tuple): The position to check.
 
         Returns:
-            bool: True if the vector is valid, False otherwise.
-            str: A string describing why the vector is not valid.
+            bool: True if the position is valid, False otherwise.
+            str: A string describing why the pos is not valid.
         """
 
-        # Check if the vector is a tuple
-        if not isinstance(vector, tuple):
-            return False, "The vector is not a tuple, but a {}.".format(type(vector))
-
-        # Check if the vector is a 2D vector
-        if len(vector) != 2:
-            return False, "The vector is not a 2D vector, but a {}D vector.".format(
-                len(vector)
+        # Check if the pos is a tuple
+        if not isinstance(pos, tuple):
+            return False, "The position is not a tuple, but a {}.".format(type(pos))
+
+        # Check if the pos is a 2D pos
+        if len(pos) != 2:
+            return False, "The position is not a coordinate, it but has {} dim.".format(
+                len(pos)
             )
 
-        # Check if the vector is a valid displacement vector
-        if not vector[0] in [-1, 0, 1] or not vector[1] in [-1, 0, 1]:
-            return (
-                False,
-                "The vector is not a valid displacement vector (" + str(vector) + ").",
-            )
+        if not isinstance(pos[0], int) or not isinstance(pos[1], int):
+            return False, "Not all the coordinates are integers: {}.".format(pos)
 
-        # The vector can't be a null vector
-        if vector == (0, 0):
-            return False, "The vector needs to go somewhere (0, 0)."
+        # Check if the pos is in the board bounds
+        if not self.is_position_within_board(pos):
+            return False, "The position is not within the board bounds."
 
-        return True, "The vector is valid."
+        return True, "The position is valid."
 
     def is_game_over(self):
         """
         Checks if the game is over.
 
         Returns:
             bool: True if the game is over, False otherwise.
@@ -505,15 +523,15 @@
         Returns:
             str: A string representation of the board.
         """
         output = "\n"
 
         for y in range(self.board_size - 1, -1, -1):
             for x in range(self.board_size):
-                # Check if their is a pawn at this position
+                # Check if there is a pawn at this position
                 pawn = None
                 for p in self.pawns:
                     if p.pos == (x, y):
                         pawn = p
                         break
                 pawn_number = str(pawn.number) if pawn is not None else "_"
                 output += pawn_number + str(self.board[x][y]) + " "
```

### Comparing `SantorinAI-1.1.3/santorinai/board_displayer/board_displayer.py` & `SantorinAI-1.2.0/santorinai/board_displayer/board_displayer.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.3/santorinai/pawn.py` & `SantorinAI-1.2.0/santorinai/pawn.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.3/santorinai/player.py` & `SantorinAI-1.2.0/santorinai/player.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     def play_move(
         self, board: Board, pawn: Pawn
     ) -> Tuple[Tuple[int, int], Tuple[int, int]]:
         """
         Play a move given a board
         :param board: the board
         :param pawn: the pawn that needs to be moved and that needs to build
-        :return: two vectors of the form (x1, y1), (x2, y2)
+        :return: two positions of the form (x1, y1), (x2, y2)
 
-        The first vector is the move of the pawn and the second vector is the
-        construction of a building relative to the new position of the pawn
+        The first coordinate corresponds to the new position of the pawn
+        The second coordinate corresponds to the position of the construction of the tower
 
-        Return example: (1, 0), (-1, 1) means that the player wants to move the pawn right one tile
-         and construct a building at the top left of his new position
+        Return example: (2, 2), (2, 3) means that the player wants to move the pawn at
+        at center of the board and build a tower at the top of his position
         """
         pass
```

### Comparing `SantorinAI-1.1.3/santorinai/player_examples/first_choice_player.py` & `SantorinAI-1.2.0/santorinai/player_examples/first_choice_player.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,25 +17,15 @@
     def play_move(self, board, pawn):
         my_initial_position = pawn.pos
 
         # Get movement positions
         available_positions = board.get_possible_movement_positions(pawn)
         my_move_choice = available_positions[0]
 
-        # Simulate the move
+        # Simulate the move (this will not impact the actual board)
         pawn.move(my_move_choice)
 
         # Get construction positions
         available_positions = board.get_possible_building_positions(pawn)
         my_build_choice = available_positions[0]
 
-        my_move_vector = (
-            my_move_choice[0] - my_initial_position[0],
-            my_move_choice[1] - my_initial_position[1],
-        )
-
-        my_build_vector = (
-            my_build_choice[0] - my_move_choice[0],
-            my_build_choice[1] - my_move_choice[1],
-        )
-
-        return my_move_vector, my_build_vector
+        return my_move_choice, my_build_choice
```

### Comparing `SantorinAI-1.1.3/santorinai/player_examples/random_player.py` & `SantorinAI-1.2.0/santorinai/player_examples/random_player.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,22 +22,12 @@
         # Get movement positions
         available_positions = board.get_possible_movement_positions(pawn)
         my_move_choice = choice(available_positions)
 
         # Simulate the move
         pawn.move(my_move_choice)
 
-        # Get construction positions
+        # Get construction positions for the new position
         available_positions = board.get_possible_building_positions(pawn)
         my_build_choice = choice(available_positions)
 
-        my_move_vector = (
-            my_move_choice[0] - my_initial_position[0],
-            my_move_choice[1] - my_initial_position[1],
-        )
-
-        my_build_vector = (
-            my_build_choice[0] - my_move_choice[0],
-            my_build_choice[1] - my_move_choice[1],
-        )
-
-        return my_move_vector, my_build_vector
+        return my_move_choice, my_build_choice
```

### Comparing `SantorinAI-1.1.3/santorinai/tester.py` & `SantorinAI-1.2.0/santorinai/tester.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.3/setup.py` & `SantorinAI-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="SantorinAI",
-    version="1.1.3",
+    version="1.2.0",
     author="Tom Mansion",
     author_email="tomansion@yahoo.fr",
     description="A Python library for the Santorini board game",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tomansion/santorinai",
     packages=find_packages(),
```

### Comparing `SantorinAI-1.1.3/test/test_board.py` & `SantorinAI-1.2.0/test/test_board.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,43 +260,45 @@
         move_ok, _ = board.play_move((None, None), (None, None))
         self.assertTrue(move_ok)
         self.assertEqual(board.pawn_turn, 2)
         self.assertEqual(board.get_playing_pawn().number, 2)
         self.assertEqual(board.get_playing_pawn().player_number, 2)
 
         # Pawn 2 moves top and builds down
-        move_ok, _ = board.play_move((0, 1), (0, -1))
+        move_ok, _ = board.play_move((0, 2), (0, 1))
         self.assertTrue(move_ok)
         self.assertEqual(board.pawn_turn, 3)
         self.assertEqual(board.pawns[1].pos, (0, 2))
         self.assertEqual(board.board[0][1], 1)
 
         # Current board:   Current pawns:
         # 0 0 0 0 0        _ _ _ _ _
         # 0 0 0 0 0        _ _ _ _ _
         # 0 0 0 0 0        2 _ _ _ _
         # 1 0 0 0 0        _ 4 _ _ _
         # 0 0 0 0 0        1 3 _ _ _
 
         # Pawn 3 moves top left and builds down right
-        move_ok, _ = board.play_move((-1, 1), (1, -1))
+        move_ok, _ = board.play_move((0, 1), (1, 0))
         self.assertTrue(move_ok)
         self.assertEqual(board.pawn_turn, 4)
         self.assertEqual(board.pawns[2].pos, (0, 1))
         self.assertEqual(board.board[1][0], 1)
 
         # Current board:   Current pawns:
         # 0 0 0 0 0        _ _ _ _ _
         # 0 0 0 0 0        _ _ _ _ _
         # 0 0 0 0 0        2 _ _ _ _
         # 1 0 0 0 0        3 4 _ _ _
         # 0 1 0 0 0        1 _ _ _ _
 
-        # Pawn 4 moves try to move multiple times and fails
-        move_ok, _ = board.play_move((-1, 0), (1, -1))
+        # Pawn 4 moves tries to move top left but fails
+        move_ok, _ = board.play_move((0, 2), (0, 3))
+        self.assertFalse(move_ok)
+        move_ok, _ = board.play_move((0, 2), None)
         self.assertFalse(move_ok)
         self.assertEqual(board.pawn_turn, 4)
 
         self.assertFalse(board.play_move(("a", "b"), (1, -1))[0])
         self.assertFalse(board.play_move((1, -1), ("a", "b"))[0])
         self.assertFalse(board.play_move("test", (None, None))[0])
         self.assertFalse(board.play_move((1, -1), "test")[0])
@@ -304,24 +306,24 @@
         self.assertFalse(board.play_move((None, None), (None, None))[0])
         self.assertFalse(board.play_move((0, 0), (0, 0))[0])
         self.assertFalse(board.play_move((1, 1), (0, 0))[0])
         self.assertFalse(board.play_move((1, 1), (1, 0, 0))[0])
         self.assertEqual(board.pawn_turn, 4)
 
         # Pawn 4 moves down and try to build left but fails
-        move_ok, _ = board.play_move((0, -1), (-1, 0))
+        move_ok, _ = board.play_move((1, 0), (0, 0))
         self.assertFalse(move_ok)
         self.assertEqual(board.pawn_turn, 4)
         # The pawn is not moved:
         self.assertEqual(board.pawns[3].pos, (1, 1))
         # Pawn 4 try to play again but fails
-        self.assertFalse(board.place_pawn((1, 1))[0])
+        self.assertFalse(board.place_pawn((2, 2))[0])
 
         # Pawn 4 moves down and builds right
-        move_ok, _ = board.play_move((0, -1), (1, 0))
+        move_ok, _ = board.play_move((1, 0), (2, 0))
         self.assertTrue(move_ok)
         self.assertEqual(board.pawn_turn, 1)
 
         # Board so far:
         # _0 _0 _0 _0 _0
         # _0 _0 _0 _0 _0
         # 20 _0 _0 _0 _0
@@ -369,32 +371,32 @@
 
         # ==== Constructions ====
         board.board[0][4] = 1
         board.board[0][3] = 2
         board.board[0][2] = 2
 
         # ==== First move====
-        self.assertTrue(board.play_move((0, -1), (0, -1))[0])
-        self.assertTrue(board.play_move((0, -1), (0, -1))[0])
-        self.assertTrue(board.play_move((0, -1), (0, -1))[0])
-        self.assertTrue(board.play_move((0, -1), (0, -1))[0])
+        self.assertTrue(board.play_move((0, 3), (0, 2))[0])
+        self.assertTrue(board.play_move((1, 3), (1, 4))[0])
+        self.assertTrue(board.play_move((2, 3), (2, 4))[0])
+        self.assertTrue(board.play_move((3, 3), (3, 4))[0])
 
         self.assertFalse(board.is_game_over())
         self.assertFalse(board.is_everyone_stuck())
         self.assertEqual(board.winner_player_number, None)
 
         # ==== Second and finish move ====
-        self.assertTrue(board.play_move((0, -1), (None, "Test"))[0])
+        self.assertTrue(board.play_move((0, 2), (None, "Test"))[0])
         self.assertTrue(board.is_game_over())
         self.assertEqual(board.winner_player_number, 1)
 
         self.assertFalse(board.is_everyone_stuck())
 
         # We can't play anymore
-        self.assertFalse(board.play_move((0, -1), (0, -1))[0])
+        self.assertFalse(board.play_move((2, 2), (2, 1))[0])
         self.assertFalse(board.place_pawn((2, 2))[0])
 
         # Congratulation to the winner!
         print(board)
 
     def test_every_one_is_stuck_again(self):
         board = Board(self.NB_PLAYERS)
@@ -426,15 +428,15 @@
         board.board[4][3] = 2
 
         # First and last move
         self.assertFalse(board.is_game_over())
         self.assertFalse(board.is_everyone_stuck())
         self.assertEqual(board.winner_player_number, None)
 
-        self.assertTrue(board.play_move((0, 1), (0, -1))[0])
+        self.assertTrue(board.play_move((0, 4), (0, 3))[0])
 
         self.assertTrue(board.is_game_over())
         self.assertTrue(board.is_everyone_stuck())
         self.assertEqual(board.winner_player_number, 1)  # The last player who played
 
         # What a waste of time
         print(board)
```

### Comparing `SantorinAI-1.1.3/test/test_tester.py` & `SantorinAI-1.2.0/test/test_tester.py`

 * *Files identical despite different names*

