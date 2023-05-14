# Comparing `tmp/bdsim-1.0.0.tar.gz` & `tmp/bdsim-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/corkep/Dropbox/code/bdsim/dist/.tmp-jk5v8wgo/bdsim-1.0.0.tar", last modified: Sun Jan 22 22:18:24 2023, max compression
+gzip compressed data, was "bdsim-1.1.0.tar", last modified: Sun May 14 00:13:45 2023, max compression
```

## Comparing `bdsim-1.0.0.tar` & `bdsim-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,74 @@
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-01-22 22:18:24.022480 bdsim-1.0.0/
--rw-rw----   0 corkep     (503) staff       (20)     1068 2022-11-21 06:57:48.000000 bdsim-1.0.0/LICENSE
--rw-rw----   0 corkep     (503) staff       (20)    18743 2023-01-22 22:18:24.022212 bdsim-1.0.0/PKG-INFO
--rw-rw----   0 corkep     (503) staff       (20)    16807 2023-01-22 21:37:07.000000 bdsim-1.0.0/README.md
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-01-22 22:18:24.013335 bdsim-1.0.0/bdsim/
--rw-rw----   0 corkep     (503) staff       (20)      354 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/__init__.py
--rwxrwx---   0 corkep     (503) staff       (20)     7947 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/bdeditor.py
--rwxrwx---   0 corkep     (503) staff       (20)     7478 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/bdrun.py
--rw-rw----   0 corkep     (503) staff       (20)    41306 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/blockdiagram.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-01-22 22:18:24.021547 bdsim-1.0.0/bdsim/blocks/
--rw-rw----   0 corkep     (503) staff       (20)      273 2022-11-21 06:57:48.000000 bdsim-1.0.0/bdsim/blocks/__init__.py
--rw-rw----   0 corkep     (503) staff       (20)    15918 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/blocks/connections.py
--rw-rw----   0 corkep     (503) staff       (20)    12773 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/blocks/discrete.py
--rw-rw----   0 corkep     (503) staff       (20)    15730 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/blocks/displays.py
--rw-rw----   0 corkep     (503) staff       (20)    21272 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/blocks/functions.py
--rw-rw----   0 corkep     (503) staff       (20)      983 2022-11-21 06:57:48.000000 bdsim-1.0.0/bdsim/blocks/io.py
--rw-rw----   0 corkep     (503) staff       (20)    14305 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/blocks/linalg.py
--rw-rw----   0 corkep     (503) staff       (20)     7439 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/blocks/sinks.py
--rw-rw----   0 corkep     (503) staff       (20)    12712 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/blocks/sources.py
--rw-rw----   0 corkep     (503) staff       (20)     5421 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/blocks/spatial.py
--rwxrwx---   0 corkep     (503) staff       (20)     3867 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/blocks/tex2icon.py
--rw-rw----   0 corkep     (503) staff       (20)    10804 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/blocks/transfers.py
--rw-rw----   0 corkep     (503) staff       (20)      442 2022-11-21 06:57:49.000000 bdsim-1.0.0/bdsim/blocks/vision.py
--rw-rw----   0 corkep     (503) staff       (20)    64568 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/components.py
--rw-rw----   0 corkep     (503) staff       (20)     9846 2023-01-22 08:47:02.000000 bdsim-1.0.0/bdsim/graphics.py
--rw-r--r--   0 corkep     (503) staff       (20)      855 2023-01-22 06:20:05.000000 bdsim-1.0.0/bdsim/newplots.py
--rw-rw----   0 corkep     (503) staff       (20)    12582 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/run_realtime.py
--rw-rw----   0 corkep     (503) staff       (20)    48615 2023-01-22 08:44:29.000000 bdsim-1.0.0/bdsim/run_sim.py
--rw-r--r--   0 corkep     (503) staff       (20)      121 2023-01-22 06:20:05.000000 bdsim-1.0.0/bdsim/test-stubs.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-01-22 22:18:24.015522 bdsim-1.0.0/bdsim.egg-info/
--rw-rw----   0 corkep     (503) staff       (20)    18743 2023-01-22 22:18:23.000000 bdsim-1.0.0/bdsim.egg-info/PKG-INFO
--rw-rw----   0 corkep     (503) staff       (20)      711 2023-01-22 22:18:24.000000 bdsim-1.0.0/bdsim.egg-info/SOURCES.txt
--rw-rw----   0 corkep     (503) staff       (20)        1 2023-01-22 22:18:23.000000 bdsim-1.0.0/bdsim.egg-info/dependency_links.txt
--rw-rw----   0 corkep     (503) staff       (20)       65 2023-01-22 22:18:23.000000 bdsim-1.0.0/bdsim.egg-info/entry_points.txt
--rw-rw----   0 corkep     (503) staff       (20)      228 2023-01-22 22:18:23.000000 bdsim-1.0.0/bdsim.egg-info/requires.txt
--rw-rw----   0 corkep     (503) staff       (20)        6 2023-01-22 22:18:23.000000 bdsim-1.0.0/bdsim.egg-info/top_level.txt
--rw-rw----   0 corkep     (503) staff       (20)     1490 2023-01-22 21:37:10.000000 bdsim-1.0.0/pyproject.toml
--rw-rw----   0 corkep     (503) staff       (20)       38 2023-01-22 22:18:24.022601 bdsim-1.0.0/setup.cfg
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-14 00:13:45.693340 bdsim-1.1.0/
+-rw-rw----   0 corkep     (503) staff       (20)     1068 2022-11-21 06:57:48.000000 bdsim-1.1.0/LICENSE
+-rw-rw----   0 corkep     (503) staff       (20)    22336 2023-05-14 00:13:45.692638 bdsim-1.1.0/PKG-INFO
+-rw-r--r--   0 corkep     (503) staff       (20)    20379 2023-05-14 00:02:13.000000 bdsim-1.1.0/README.md
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-14 00:13:45.626771 bdsim-1.1.0/bdsim/
+-rw-rw----   0 corkep     (503) staff       (20)      462 2023-03-12 00:27:33.000000 bdsim-1.1.0/bdsim/__init__.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-14 00:13:45.658078 bdsim-1.1.0/bdsim/bdedit/
+-rw-rw----   0 corkep     (503) staff       (20)   214076 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/Icons.py
+-rw-rw----   0 corkep     (503) staff       (20)      550 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/__init__.py
+-rwxrwx---   0 corkep     (503) staff       (20)     6767 2023-01-22 22:15:43.000000 bdsim-1.1.0/bdsim/bdedit/bdedit.py
+-rw-rw----   0 corkep     (503) staff       (20)    46296 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block.py
+-rw-rw----   0 corkep     (503) staff       (20)     3493 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_connector_block.py
+-rw-rw----   0 corkep     (503) staff       (20)    27281 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_graphics_block.py
+-rw-rw----   0 corkep     (503) staff       (20)    16144 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_graphics_socket.py
+-rw-rw----   0 corkep     (503) staff       (20)    65171 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_graphics_wire.py
+-rw-rw----   0 corkep     (503) staff       (20)    26025 2023-01-22 22:16:45.000000 bdsim-1.1.0/bdsim/bdedit/block_importer.py
+-rw-rw----   0 corkep     (503) staff       (20)     1681 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_main_block.py
+-rw-rw----   0 corkep     (503) staff       (20)    56804 2023-03-12 00:27:34.000000 bdsim-1.1.0/bdsim/bdedit/block_param_window.py
+-rw-rw----   0 corkep     (503) staff       (20)    10984 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_socket.py
+-rw-rw----   0 corkep     (503) staff       (20)    22093 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/block_wire.py
+-rw-rw----   0 corkep     (503) staff       (20)     8773 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/floating_label.py
+-rw-rw----   0 corkep     (503) staff       (20)     6662 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/floating_label_graphics.py
+-rw-rw----   0 corkep     (503) staff       (20)     3482 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/grouping_box.py
+-rw-rw----   0 corkep     (503) staff       (20)    13971 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/grouping_box_graphics.py
+-rw-rw----   0 corkep     (503) staff       (20)    35012 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface.py
+-rw-rw----   0 corkep     (503) staff       (20)    20471 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface_graphics_scene.py
+-rw-rw----   0 corkep     (503) staff       (20)    36974 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface_graphics_view.py
+-rw-rw----   0 corkep     (503) staff       (20)    41772 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface_manager.py
+-rw-rw----   0 corkep     (503) staff       (20)    21061 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface_scene.py
+-rw-rw----   0 corkep     (503) staff       (20)     7608 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface_scene_history.py
+-rw-rw----   0 corkep     (503) staff       (20)     1645 2023-01-22 08:44:29.000000 bdsim-1.1.0/bdsim/bdedit/interface_serialize.py
+-rwxrwx---   0 corkep     (503) staff       (20)     8230 2023-05-12 03:20:38.000000 bdsim-1.1.0/bdsim/bdrun.py
+-rw-r--r--   0 corkep     (503) staff       (20)    47042 2023-05-11 10:20:38.000000 bdsim-1.1.0/bdsim/blockdiagram.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-14 00:13:45.672358 bdsim-1.1.0/bdsim/blocks/
+-rw-rw----   0 corkep     (503) staff       (20)      291 2023-04-03 00:16:30.000000 bdsim-1.1.0/bdsim/blocks/__init__.py
+-rw-r--r--   0 corkep     (503) staff       (20)    15328 2023-04-19 22:21:12.000000 bdsim-1.1.0/bdsim/blocks/connections.py
+-rw-r--r--   0 corkep     (503) staff       (20)    12585 2023-05-01 04:27:59.000000 bdsim-1.1.0/bdsim/blocks/discrete.py
+-rw-r--r--   0 corkep     (503) staff       (20)    17776 2023-05-13 23:27:14.000000 bdsim-1.1.0/bdsim/blocks/displays.py
+-rw-r--r--   0 corkep     (503) staff       (20)    23971 2023-04-28 05:08:21.000000 bdsim-1.1.0/bdsim/blocks/functions.py
+-rw-rw----   0 corkep     (503) staff       (20)     2444 2023-04-30 21:23:08.000000 bdsim-1.1.0/bdsim/blocks/io.py
+-rw-r--r--   0 corkep     (503) staff       (20)    14257 2023-04-19 21:49:23.000000 bdsim-1.1.0/bdsim/blocks/linalg.py
+-rw-r--r--   0 corkep     (503) staff       (20)     7432 2023-04-19 20:51:16.000000 bdsim-1.1.0/bdsim/blocks/sinks.py
+-rw-r--r--   0 corkep     (503) staff       (20)    13423 2023-04-28 02:23:28.000000 bdsim-1.1.0/bdsim/blocks/sources.py
+-rw-r--r--   0 corkep     (503) staff       (20)     5439 2023-04-19 22:41:09.000000 bdsim-1.1.0/bdsim/blocks/spatial.py
+-rw-r--r--   0 corkep     (503) staff       (20)    17072 2023-04-30 04:30:47.000000 bdsim-1.1.0/bdsim/blocks/transfers.py
+-rw-rw----   0 corkep     (503) staff       (20)      442 2022-11-21 06:57:49.000000 bdsim-1.1.0/bdsim/blocks/vision.py
+-rw-r--r--   0 corkep     (503) staff       (20)    67747 2023-05-01 04:23:25.000000 bdsim-1.1.0/bdsim/components.py
+-rw-r--r--   0 corkep     (503) staff       (20)    10214 2023-04-30 00:39:07.000000 bdsim-1.1.0/bdsim/graphics.py
+-rw-r--r--   0 corkep     (503) staff       (20)      855 2023-01-22 06:20:05.000000 bdsim-1.1.0/bdsim/newplots.py
+-rw-r--r--   0 corkep     (503) staff       (20)    12653 2023-04-12 03:39:20.000000 bdsim-1.1.0/bdsim/run_realtime.py
+-rw-r--r--   0 corkep     (503) staff       (20)    58796 2023-05-11 09:44:42.000000 bdsim-1.1.0/bdsim/run_sim.py
+-rw-r--r--   0 corkep     (503) staff       (20)      190 2023-03-14 04:44:13.000000 bdsim-1.1.0/bdsim/test-stubs.py
+-rwxrwx---   0 corkep     (503) staff       (20)     5104 2023-04-18 08:13:58.000000 bdsim-1.1.0/bdsim/tex2icon.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-14 00:13:45.630706 bdsim-1.1.0/bdsim.egg-info/
+-rw-rw----   0 corkep     (503) staff       (20)    22336 2023-05-14 00:13:45.000000 bdsim-1.1.0/bdsim.egg-info/PKG-INFO
+-rw-rw----   0 corkep     (503) staff       (20)     1723 2023-05-14 00:13:45.000000 bdsim-1.1.0/bdsim.egg-info/SOURCES.txt
+-rw-rw----   0 corkep     (503) staff       (20)        1 2023-05-14 00:13:45.000000 bdsim-1.1.0/bdsim.egg-info/dependency_links.txt
+-rw-rw----   0 corkep     (503) staff       (20)      113 2023-05-14 00:13:45.000000 bdsim-1.1.0/bdsim.egg-info/entry_points.txt
+-rw-rw----   0 corkep     (503) staff       (20)      287 2023-05-14 00:13:45.000000 bdsim-1.1.0/bdsim.egg-info/requires.txt
+-rw-rw----   0 corkep     (503) staff       (20)        6 2023-05-14 00:13:45.000000 bdsim-1.1.0/bdsim.egg-info/top_level.txt
+-rw-rw----   0 corkep     (503) staff       (20)     1805 2023-04-25 06:02:55.000000 bdsim-1.1.0/pyproject.toml
+-rw-rw----   0 corkep     (503) staff       (20)       38 2023-05-14 00:13:45.693542 bdsim-1.1.0/setup.cfg
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-14 00:13:45.689737 bdsim-1.1.0/tests/
+-rw-rw----   0 corkep     (503) staff       (20)     3818 2023-04-10 12:13:42.000000 bdsim-1.1.0/tests/test_bdsim.py
+-rw-rw----   0 corkep     (503) staff       (20)    19421 2023-04-18 09:41:18.000000 bdsim-1.1.0/tests/test_blockdiagram.py
+-rw-r--r--   0 corkep     (503) staff       (20)     8576 2023-04-15 00:55:21.000000 bdsim-1.1.0/tests/test_components.py
+-rwxrwx---   0 corkep     (503) staff       (20)     1085 2022-11-21 06:57:49.000000 bdsim-1.1.0/tests/test_connections.py
+-rw-rw----   0 corkep     (503) staff       (20)     2796 2023-05-01 04:28:27.000000 bdsim-1.1.0/tests/test_discrete.py
+-rwxrwx---   0 corkep     (503) staff       (20)     7673 2023-01-22 08:44:29.000000 bdsim-1.1.0/tests/test_functions.py
+-rw-rw----   0 corkep     (503) staff       (20)     4312 2022-11-21 06:57:49.000000 bdsim-1.1.0/tests/test_linalg.py
+-rw-r--r--   0 corkep     (503) staff       (20)     3850 2023-04-14 22:15:25.000000 bdsim-1.1.0/tests/test_sinks.py
+-rw-r--r--   0 corkep     (503) staff       (20)     8519 2023-04-14 21:42:24.000000 bdsim-1.1.0/tests/test_sources.py
+-rw-rw----   0 corkep     (503) staff       (20)     1145 2022-11-21 06:57:49.000000 bdsim-1.1.0/tests/test_spatial.py
+-rw-rw----   0 corkep     (503) staff       (20)     3659 2023-01-22 08:44:29.000000 bdsim-1.1.0/tests/test_transfers.py
```

### Comparing `bdsim-1.0.0/LICENSE` & `bdsim-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bdsim-1.0.0/PKG-INFO` & `bdsim-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,7 @@
-Metadata-Version: 2.1
-Name: bdsim
-Version: 1.0.0
-Summary: Simulate dynamic systems expressed in block diagram form using Python
-Author-email: Peter Corke <rvc@petercorke.com>
-License: MIT License
-        
-        Copyright (c) 2020 Peter Corke
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: homepage, https://github.com/petercorke/bdsim
-Project-URL: documentation, https://petercorke.github.io/bdsim/
-Project-URL: repository, https://github.com/petercorke/bdsim
-Keywords: python,block diagram,dynamic simulation
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 [![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-python)
 [![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
 
 [![PyPI version](https://badge.fury.io/py/bdsim.svg)](https://badge.fury.io/py/bdsim)
 ![Python Version](https://img.shields.io/pypi/pyversions/bdsim.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
@@ -133,22 +93,20 @@
     13	
     14	# connect the blocks
     15	bd.connect(demand, sum[0], scope[1])
     17	bd.connect(sum, gain)
     18	bd.connect(gain, plant)
     19	bd.connect(plant, sum[1], scope[0])
     20	
-    21	bd.compile()   # check the diagram
-    22	bd.report()    # list all blocks and wires
-    23
+    21	bd.compile()          # check the diagram
+    22
+    23	sim.report(bd)   # list the system
     24  out = sim.run(bd, 5)   # simulate for 5s
-    25  sim.savefig(scope, 'scope0')
-    26  sim.done(bd, block=True)
 ```
-which is just 16 lines of executable code.
+which is just 15 lines of executable code.
 
 The red block annotations on the hand-drawn diagram are used as the names of the variables holding references to the block instance. The blocks can also have user-assigned names, see lines 8 and 11, which are used in diagnostics and as labels in plots.
 
 After the blocks are created their input and output ports need to be connected. In `bdsim` all wires are point to point, a *one-to-many* connection is implemented by *many* wires,
 for example
 ```
 bd.connect(source, dest1, dest2, ...)
@@ -162,16 +120,103 @@
 bd.connect(source[2:5], dest[3:6)
 ```
 will connect `source[2]` -> `dest[3]`, `source[3]` -> `dest[4]`, `source[4]` -> `dest[5]`.
 The number of wires in each slice must be consistent.  You could even do a cross over by connecting `source[2:5]` to `dest[6:3:-1]`.
 
 Line 21 assembles all the blocks and wires, instantiates subsystems, checks connectivity to create a flat wire list, and then builds the dataflow execution plan.
 
-Line 22 generates a report, in tabular form, showing a summary of the block diagram:
+Line 23 generates a report, in tabular form, showing a summary of the block diagram:
+
+```
+┌────────┬──────────┬────────┬────────┬─────────────┐
+│ block  │   type   │ inport │ source │ source type │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│demand@ │ step     │        │        │             │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│gain.0  │ gain     │ 0      │ sum.0  │ float64     │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│plant   │ lti_siso │ 0      │ gain.0 │ float64     │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│scope.0 │ scope    │ 0      │ plant  │ float64     │
+│        │          │ 1      │ demand │ int         │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│sum.0   │ sum      │ 0      │ demand │ int         │
+│        │          │ 1      │ plant  │ float64     │
+└────────┴──────────┴────────┴────────┴─────────────┘
+```
+
+Line 24 runs the simulation for 5 seconds 
+using the default variable-step RK45 solver and saves output values at least every 0.05s.  It
+causes the following output
+
+```
+>>> Start simulation: T = 5.00, dt = 0.050
+  Continuous state variables: 1
+     x0 =  [0.]
+  Discrete state variables:   0
+
+no graphics backend specified: Qt5Agg found, using instead of MacOSX
+
+bdsim ◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉ 100.0% - 0s
+
+<<< Simulation complete
+  block diagram evaluations: 784
+  block diagram exec time:   0.075 ms
+  time steps:                123
+  integration intervals:     2
+```
+
+This provides a summary of the number of states for the complete system: the number of continuous states, the number
+of discrete states, and the initial value of the state vectors.
+
+During execution a progress bar is updated and scope blocks pops up a graphical window
+
+![bdsim output](https://github.com/petercorke/bdsim/raw/master/figs/Figure_1.png)
+
+The simulation results are in a container object (`BDStruct`)
+```
+>>> out
+t      = ndarray:float64 (123,)
+x      = ndarray:float64 (123, 1)
+xnames = ['plantx0'] (list)
+ynames = [] (list)            
+```
+which contains an array of time values, an array of state values, and a list of the
+names of the state variables.
+
+By default the `.run()` method at line 24 blocks blocks the script until all figure
+windows are closed (by pressing the operating system close button or typing "q"), or the
+script is killed with SIGINT. If you want to continue the script with the figures still
+active then the `hold=False` option should be set.
 
+If we wished to also record additional outputs, we can add them as _watched_ signals
+```
+out = sim.run(bd, watch=[demand, sum])  # simulate for 5s
+```
+and now the output is
+```
+>>> out
+t      = ndarray:float64 (123,)
+x      = ndarray:float64 (123, 1)
+xnames = ['plantx0'] (list)
+y0     = ndarray:float64 (123,)
+y1     = ndarray:int64 (123,)
+ynames = ['plant[0]', 'demand[0]'] (list)
+```
+where
+
+- `t` the time vector: ndarray, shape=(M,)
+- `x` is the state vector: ndarray, shape=(M,N), one row per timestep
+- `xnames` is a list of the names of the states corresponding to columns of `x`, eg. "plant.x0"
+
+The `watch` argument is a list of outputs to log, in this case `plant` defaults
+to output port 0.  This information is saved in additional variables `y0`, `y1`
+etc.  `ynames` is a list of the names of the watched variables.
+
+An alternative system report, created by `sim.report(bd, type="lists")` is more detailed
 ```
 Blocks::
 
 ┌───┬─────────┬─────┬──────┬────────┬─────────┬───────┐
 │id │    name │ nin │ nout │ nstate │ ndstate │ type  │
 ├───┼─────────┼─────┼──────┼────────┼─────────┼───────┤
 │ 0 │  demand │   0 │    1 │      0 │       0 │ step  │
@@ -189,88 +234,70 @@
 │ 0 │ 0[0] │ 1[0] │ demand[0] --> sum.0[0]   │ int     │
 │ 1 │ 0[0] │ 4[1] │ demand[0] --> scope.0[1] │ int     │
 │ 2 │ 3[0] │ 1[1] │ plant[0] --> sum.0[1]    │ float64 │
 │ 3 │ 1[0] │ 2[0] │ sum.0[0] --> gain.0[0]   │ float64 │
 │ 4 │ 2[0] │ 3[0] │ gain.0[0] --> plant[0]   │ float64 │
 │ 5 │ 3[0] │ 4[0] │ plant[0] --> scope.0[0]  │ float64 │
 └───┴──────┴──────┴──────────────────────────┴─────────┘
-
-Continuous state variables:   1
-Discrete state variables:     0
-initial state  x0 =  [0.]
 ```
 In the first table we can see key information about each block, its `id` (used internally), name, the number of input and output ports, the number of
 continuous- and discrete-time states, and the type which is the block class.  Note that the name is auto-generated based on the type, except if it has
 been set explicitly as for the blocks `demand` and `plant`.
 
 The second table shows all wires in point-to-point form, showing the start and end block and port (the block is represented here by its `id`) and the type of the object sent along the wire.
 
-Finally, there is a summary of the number of states for the complete system: the number of continuous states, the number
-of discrete states, and the initial value of the continuous state vector.
-
-Line 24 runs the simulation for 5 seconds 
-using the default variable-step RK45 solver and saves output values at least every 0.1s.  The scope block pops up a graph
-
-![bdsim output](https://github.com/petercorke/bdsim/raw/master/figs/Figure_1.png)
-
-The simulation results are in a container object
+To save figures we need to make two modifications, changing line 4 to
 ```
->>> out
-results:
-t           | ndarray (67,)
-x           | ndarray (67, 1)
-xnames      | list              
+     4  sim = bdsim.BDSim(hold=False)  # create simulator
 ```
-which contains an array of time values, an array of state values, and a list of the names of the state variables.
-
-Line 25 saves the content of the scope to be saved in the file called `scope0.pdf`.
-
-Line 26 blocks the script until all figure windows are closed, or the script is killed with SIGINT.
-
-The result `out` is effectively a structure with elements
-
+which prevents `.run()` from blocking and then deleting all the figures.
+Then, after the `.run()` we add 
 ```
->>> out
-results:
-t           | ndarray (67,)
-x           | ndarray (67, 1)
-xnames      | list        
-y0          | ndarray (67,)
-y1          | ndarray (67,)
-ynames      | list   
+     25 scope.savefig()  # save scope figure
 ```
-where
+If the filename is not given it defaults to the block name, in this case `scope.0.pdf`.
 
-- `t` the time vector: ndarray, shape=(M,)
-- `x` is the state vector: ndarray, shape=(M,N), one row per timestep
-- `xnames` is a list of the names of the states corresponding to columns of `x`, eg. "plant.x0"
 
-The `watch` argument is a list of outputs to log, in this case `plant` defaults
-to output port 0.  This information is saved in additional variables `y0`, `y1`
-etc.  `ynames` is a list of the names of the watched variables.
+The output can be pickled and written to a file
 
-Line 29 saves the scope graphics as a PDF file.
+```[shell]
+examples/eg1.py -o
+python -mpickle bd.out
+t      = ndarray:float64 (123,)
+x      = ndarray:float64 (123, 1)
+xnames = ['plantx0'] (list)
+y0     = ndarray:float64 (123,)
+y1     = ndarray:int64 (123,)
+ynames = ['plant[0]', 'demand[0]'] (list)
+```
 
-Line 30 blocks until the last figure is dismissed.
+by default the results are written to `bd.out`, use the option `--out FILE` to set it
+to a specific value.
 
-More details on this Wiki about:
+The block parameters can also be overridden from the command line without having to 
+edit the code.  To increase the loop gain we could write:
+```[shell]
+examples/eg1.py --set gain.0:K=20
+```
 
-- [Adding blocks](Adding-blocks)
-- [Connecting blocks](Connecting-blocks)
-- [Running the simulation](Running)
+More details on this Wiki about:
 
+- [Adding blocks](https://github.com/petercorke/bdsim/wiki/Adding-blocks)
+- [Connecting blocks](https://github.com/petercorke/bdsim/wiki/Connecting-blocks)
+- [Running the simulation](https://github.com/petercorke/bdsim/wiki/Running)
+- [Command line options](https://github.com/petercorke/bdsim/wiki/Runtime-options)
 
 ## Other examples
 
 In the folder `bdsim/examples` you can find a few other runnable examples:
 
 - [`eg1.py`](https://github.com/petercorke/bdsim/blob/master/examples/eg1.py) the example given above
 - [`waveform.py`](https://github.com/petercorke/bdsim/blob/master/examples/waveform.py) two signal generators connected to two scopes
 
-Examples from Chapter four of _Robotics, Vision & Control (2017)_:
+Examples from Chapter four of _Robotics, Vision & Control 2e (2017)_:
 
 - [`rvc4_2.py`](https://github.com/petercorke/bdsim/blob/master/examples/rvc4_2.py) Fig 4.2 - a car-like vehicle with bicycle kinematics driven by a rectangular pulse steering signal
 - [`rvc4_4.py`](https://github.com/petercorke/bdsim/blob/master/examples/rvc4_4.py) Fig 4.4 - a car-like vehicle driving to a point
 
 ![RVC Figure 4.4](https://github.com/petercorke/bdsim/raw/master/figs/rvc4_4.gif)
 
 - [`rvc4_6.py`](https://github.com/petercorke/bdsim/blob/master/examples/rvc4_6.py) Fig 4.6 - a car-like vehicle driving to/along a line
@@ -308,15 +335,14 @@
     14  scope[0] = plant
     15  scope[1] = demand
     16  plant[0] = 10 * (demand - plant)
     17
     18  bd.compile()   # check the diagram
     19  bd.report()    # list all blocks and wires
     20
-    21  sim.set_options(animation=True)
     22  out = sim.run(bd, 5, watch=[plant,])  # simulate for 5s
 ```
 This requires fewer lines of code and the code is more readable. Importantly, it results in in *exactly the same* block diagram in terms of blocks and wires
 ```
 Wires::
 
 ┌───┬──────┬──────┬──────────────────────────────┬─────────┐
@@ -346,14 +372,14 @@
 
 * parse the JSON file
 * instantiate all blocks and wires
 * compile and run the diagram
 
 # Article
 
-I published [this article on LinkedIn](https://www.linkedin.com/in/petercorke/recent-activity/shares/), which describes the thouhgt process behind bdsim.
+I published [this article on LinkedIn](https://www.linkedin.com/pulse/journey-toward-open-source-block-diagram-simulation-peter-corke/?trackingId=wrJYinHUgAHDq63Nv65PnA%3D%3D), which describes the thought process behind bdsim.
 
 # Limitations
 
 There are lots!  The biggest is that `bdsim` is based on a very standard variable-step integrator from the scipy library.  For discontinuous inputs (step, square wave, triangle wave, piecewise constant) the transitions get missed.  This also makes it inaccurate to simulate hybrid discrete-continuous time systems.  We really need a better integrator, perhaps [`odedc`](https://help.scilab.org/docs/6.1.0/en_US/odedc.html) from SciLab could be integrated.
```

#### html2text {}

```diff
@@ -1,35 +1,12 @@
-Metadata-Version: 2.1 Name: bdsim Version: 1.0.0 Summary: Simulate dynamic
-systems expressed in block diagram form using Python Author-email: Peter Corke
-petercorke.com> License: MIT License Copyright (c) 2020 Peter Corke Permission
-is hereby granted, free of charge, to any person obtaining a copy of this
-software and associated documentation files (the "Software"), to deal in the
-Software without restriction, including without limitation the rights to use,
-copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
-Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions: The above copyright notice and this
-permission notice shall be included in all copies or substantial portions of
-the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
-EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
-OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Project-URL: homepage, https://github.com/petercorke/
-bdsim Project-URL: documentation, https://petercorke.github.io/bdsim/ Project-
-URL: repository, https://github.com/petercorke/bdsim Keywords: python,block
-diagram,dynamic simulation Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev Provides-Extra: docs License-File: LICENSE [![A
-Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-
-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/
-petercorke/robotics-toolbox-python) [![QUT Centre for Robotics Open Source]
-(https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://
-qcr.github.io) [![PyPI version](https://badge.fury.io/py/bdsim.svg)](https://
+[![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/
+robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://
+github.com/petercorke/robotics-toolbox-python) [![QUT Centre for Robotics Open
+Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https:
+//qcr.github.io) [![PyPI version](https://badge.fury.io/py/bdsim.svg)](https://
 badge.fury.io/py/bdsim) ![Python Version](https://img.shields.io/pypi/
 pyversions/bdsim.svg) [![License: MIT](https://img.shields.io/badge/License-
 MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Build Status](https://
 github.com/petercorke/bdsim/workflows/build/badge.svg?branch=master)](https://
 github.com/petercorke/bdsim/actions?query=workflow%3Abuild) [![Coverage](https:
 //codecov.io/gh/petercorke/bdsim/branch/master/graph/badge.svg)](https://
 codecov.io/gh/petercorke/bdsim) [![PyPI - Downloads](https://img.shields.io/
@@ -92,38 +69,84 @@
 examples/eg1.py)) ```python 1 #!/usr/bin/env python3 2 import bdsim 4 sim =
 bdsim.BDSim() # create simulator 5 bd = sim.blockdiagram() # create an empty
 block diagram 6 7 # define the blocks 8 demand = bd.STEP(T=1, name='demand') 9
 sum = bd.SUM('+-') 10 gain = bd.GAIN(10) 11 plant = bd.LTI_SISO(0.5, [2, 1],
 name='plant') 12 scope = bd.SCOPE(styles=['k', 'r--']) 13 14 # connect the
 blocks 15 bd.connect(demand, sum[0], scope[1]) 17 bd.connect(sum, gain) 18
 bd.connect(gain, plant) 19 bd.connect(plant, sum[1], scope[0]) 20 21 bd.compile
-() # check the diagram 22 bd.report() # list all blocks and wires 23 24 out =
-sim.run(bd, 5) # simulate for 5s 25 sim.savefig(scope, 'scope0') 26 sim.done
-(bd, block=True) ``` which is just 16 lines of executable code. The red block
-annotations on the hand-drawn diagram are used as the names of the variables
-holding references to the block instance. The blocks can also have user-
-assigned names, see lines 8 and 11, which are used in diagnostics and as labels
-in plots. After the blocks are created their input and output ports need to be
-connected. In `bdsim` all wires are point to point, a *one-to-many* connection
-is implemented by *many* wires, for example ``` bd.connect(source, dest1,
-dest2, ...) ``` creates individual wires from `source` -> `dest1`, `source` -
-> `dest2` and so on. Ports are designated using Python indexing notation, for
-example `block[2]` is port 2 (the third port) of `block`. Whether it is an
-input or output port depends on context. In the example above an index on the
-first argument refers to an output port, while on the second (or subsequent)
-arguments it refers to an input port. If a block has only a single input or
-output port then no index is required, 0 is assumed. A group of ports can be
-denoted using slice notation, for example ``` bd.connect(source[2:5], dest[3:6)
-``` will connect `source[2]` -> `dest[3]`, `source[3]` -> `dest[4]`, `source
-[4]` -> `dest[5]`. The number of wires in each slice must be consistent. You
-could even do a cross over by connecting `source[2:5]` to `dest[6:3:-1]`. Line
-21 assembles all the blocks and wires, instantiates subsystems, checks
+() # check the diagram 22 23 sim.report(bd) # list the system 24 out = sim.run
+(bd, 5) # simulate for 5s ``` which is just 15 lines of executable code. The
+red block annotations on the hand-drawn diagram are used as the names of the
+variables holding references to the block instance. The blocks can also have
+user-assigned names, see lines 8 and 11, which are used in diagnostics and as
+labels in plots. After the blocks are created their input and output ports need
+to be connected. In `bdsim` all wires are point to point, a *one-to-many*
+connection is implemented by *many* wires, for example ``` bd.connect(source,
+dest1, dest2, ...) ``` creates individual wires from `source` -> `dest1`,
+`source` -> `dest2` and so on. Ports are designated using Python indexing
+notation, for example `block[2]` is port 2 (the third port) of `block`. Whether
+it is an input or output port depends on context. In the example above an index
+on the first argument refers to an output port, while on the second (or
+subsequent) arguments it refers to an input port. If a block has only a single
+input or output port then no index is required, 0 is assumed. A group of ports
+can be denoted using slice notation, for example ``` bd.connect(source[2:5],
+dest[3:6) ``` will connect `source[2]` -> `dest[3]`, `source[3]` -> `dest[4]`,
+`source[4]` -> `dest[5]`. The number of wires in each slice must be consistent.
+You could even do a cross over by connecting `source[2:5]` to `dest[6:3:-1]`.
+Line 21 assembles all the blocks and wires, instantiates subsystems, checks
 connectivity to create a flat wire list, and then builds the dataflow execution
-plan. Line 22 generates a report, in tabular form, showing a summary of the
-block diagram: ``` Blocks::
+plan. Line 23 generates a report, in tabular form, showing a summary of the
+block diagram: ```
+ââââââââââ¬âââââââââââ¬âââââââââ¬âââââââââ¬ââââââââââââââ
+â block â type â inport â source â source type â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âdemand@ â step â â â â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âgain.0 â gain â 0 â sum.0 â float64 â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âplant â lti_siso â 0 â gain.0 â float64 â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âscope.0 â scope â 0 â plant â float64 â â â â 1 â demand
+â int â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âsum.0 â sum â 0 â demand â int â â â â 1 â plant â
+float64 â
+ââââââââââ´âââââââââââ´âââââââââ´âââââââââ´ââââââââââââââ
+``` Line 24 runs the simulation for 5 seconds using the default variable-step
+RK45 solver and saves output values at least every 0.05s. It causes the
+following output ``` >>> Start simulation: T = 5.00, dt = 0.050 Continuous
+state variables: 1 x0 = [0.] Discrete state variables: 0 no graphics backend
+specified: Qt5Agg found, using instead of MacOSX bdsim
+ââââââââââââââââââââââââââââââââ
+100.0% - 0s <<< Simulation complete block diagram evaluations: 784 block
+diagram exec time: 0.075 ms time steps: 123 integration intervals: 2 ``` This
+provides a summary of the number of states for the complete system: the number
+of continuous states, the number of discrete states, and the initial value of
+the state vectors. During execution a progress bar is updated and scope blocks
+pops up a graphical window ![bdsim output](https://github.com/petercorke/bdsim/
+raw/master/figs/Figure_1.png) The simulation results are in a container object
+(`BDStruct`) ``` >>> out t = ndarray:float64 (123,) x = ndarray:float64 (123,
+1) xnames = ['plantx0'] (list) ynames = [] (list) ``` which contains an array
+of time values, an array of state values, and a list of the names of the state
+variables. By default the `.run()` method at line 24 blocks blocks the script
+until all figure windows are closed (by pressing the operating system close
+button or typing "q"), or the script is killed with SIGINT. If you want to
+continue the script with the figures still active then the `hold=False` option
+should be set. If we wished to also record additional outputs, we can add them
+as _watched_ signals ``` out = sim.run(bd, watch=[demand, sum]) # simulate for
+5s ``` and now the output is ``` >>> out t = ndarray:float64 (123,) x =
+ndarray:float64 (123, 1) xnames = ['plantx0'] (list) y0 = ndarray:float64
+(123,) y1 = ndarray:int64 (123,) ynames = ['plant[0]', 'demand[0]'] (list) ```
+where - `t` the time vector: ndarray, shape=(M,) - `x` is the state vector:
+ndarray, shape=(M,N), one row per timestep - `xnames` is a list of the names of
+the states corresponding to columns of `x`, eg. "plant.x0" The `watch` argument
+is a list of outputs to log, in this case `plant` defaults to output port 0.
+This information is saved in additional variables `y0`, `y1` etc. `ynames` is a
+list of the names of the watched variables. An alternative system report,
+created by `sim.report(bd, type="lists")` is more detailed ``` Blocks::
 âââââ¬ââââââââââ¬ââââââ¬âââââââ¬âââââââââ¬ââââââââââ¬ââââââââ
 âid â name â nin â nout â nstate â ndstate â type â
 âââââ¼ââââââââââ¼ââââââ¼âââââââ¼âââââââââ¼ââââââââââ¼ââââââââ¤
 â 0 â demand â 0 â 1 â 0 â 0 â step â â 1 â sum.0 â 2 â
 1 â 0 â 0 â sum â â 2 â gain.0 â 1 â 1 â 0 â 0 â gain â
 â 3 â plant â 1 â 1 â 1 â 0 â LTI â â 4 â scope.0 â 2 â
 0 â 0 â 0 â scope â
@@ -135,79 +158,71 @@
 â 0 â 0[0] â 1[0] â demand[0] --> sum.0[0] â int â â 1 â 0[0]
 â 4[1] â demand[0] --> scope.0[1] â int â â 2 â 3[0] â 1[1] â
 plant[0] --> sum.0[1] â float64 â â 3 â 1[0] â 2[0] â sum.0[0] --
 > gain.0[0] â float64 â â 4 â 2[0] â 3[0] â gain.0[0] --> plant[0]
 â float64 â â 5 â 3[0] â 4[0] â plant[0] --> scope.0[0] â float64
 â
 âââââ´âââââââ´âââââââ´âââââââââââââââââââââââââââ´ââââââââââ
-Continuous state variables: 1 Discrete state variables: 0 initial state x0 =
-[0.] ``` In the first table we can see key information about each block, its
-`id` (used internally), name, the number of input and output ports, the number
-of continuous- and discrete-time states, and the type which is the block class.
+``` In the first table we can see key information about each block, its `id`
+(used internally), name, the number of input and output ports, the number of
+continuous- and discrete-time states, and the type which is the block class.
 Note that the name is auto-generated based on the type, except if it has been
 set explicitly as for the blocks `demand` and `plant`. The second table shows
 all wires in point-to-point form, showing the start and end block and port (the
 block is represented here by its `id`) and the type of the object sent along
-the wire. Finally, there is a summary of the number of states for the complete
-system: the number of continuous states, the number of discrete states, and the
-initial value of the continuous state vector. Line 24 runs the simulation for 5
-seconds using the default variable-step RK45 solver and saves output values at
-least every 0.1s. The scope block pops up a graph ![bdsim output](https://
-github.com/petercorke/bdsim/raw/master/figs/Figure_1.png) The simulation
-results are in a container object ``` >>> out results: t | ndarray (67,) x |
-ndarray (67, 1) xnames | list ``` which contains an array of time values, an
-array of state values, and a list of the names of the state variables. Line 25
-saves the content of the scope to be saved in the file called `scope0.pdf`.
-Line 26 blocks the script until all figure windows are closed, or the script is
-killed with SIGINT. The result `out` is effectively a structure with elements
-``` >>> out results: t | ndarray (67,) x | ndarray (67, 1) xnames | list y0 |
-ndarray (67,) y1 | ndarray (67,) ynames | list ``` where - `t` the time vector:
-ndarray, shape=(M,) - `x` is the state vector: ndarray, shape=(M,N), one row
-per timestep - `xnames` is a list of the names of the states corresponding to
-columns of `x`, eg. "plant.x0" The `watch` argument is a list of outputs to
-log, in this case `plant` defaults to output port 0. This information is saved
-in additional variables `y0`, `y1` etc. `ynames` is a list of the names of the
-watched variables. Line 29 saves the scope graphics as a PDF file. Line 30
-blocks until the last figure is dismissed. More details on this Wiki about: -
-[Adding blocks](Adding-blocks) - [Connecting blocks](Connecting-blocks) -
-[Running the simulation](Running) ## Other examples In the folder `bdsim/
-examples` you can find a few other runnable examples: - [`eg1.py`](https://
-github.com/petercorke/bdsim/blob/master/examples/eg1.py) the example given
-above - [`waveform.py`](https://github.com/petercorke/bdsim/blob/master/
-examples/waveform.py) two signal generators connected to two scopes Examples
-from Chapter four of _Robotics, Vision & Control (2017)_: - [`rvc4_2.py`]
-(https://github.com/petercorke/bdsim/blob/master/examples/rvc4_2.py) Fig 4.2 -
-a car-like vehicle with bicycle kinematics driven by a rectangular pulse
-steering signal - [`rvc4_4.py`](https://github.com/petercorke/bdsim/blob/
-master/examples/rvc4_4.py) Fig 4.4 - a car-like vehicle driving to a point !
-[RVC Figure 4.4](https://github.com/petercorke/bdsim/raw/master/figs/
-rvc4_4.gif) - [`rvc4_6.py`](https://github.com/petercorke/bdsim/blob/master/
-examples/rvc4_6.py) Fig 4.6 - a car-like vehicle driving to/along a line ![RVC
-Figure 4.6](https://github.com/petercorke/bdsim/raw/master/figs/rvc4_6.gif) -
-[`rvc4_8.py`](https://github.com/petercorke/bdsim/blob/master/examples/
-rvc4_8.py) Fig 4.8 - a car-like vehicle using pure-pursuit trajectory following
-![RVC Figure 4.6](https://github.com/petercorke/bdsim/raw/master/figs/
-rvc4_8.gif) - [`rvc4_11.py`](https://github.com/petercorke/bdsim/blob/master/
-examples/rvc4_11.py) Fig 4.11 a car-like vehicle driving to a pose ![RVC Figure
-4.11](https://github.com/petercorke/bdsim/raw/master/figs/rvc4_11.gif) Figs 4.8
-(pure pursuit) and Fig 4.21 (quadrotor control) are yet to be done. # A more
-concise way Wiring, and some simple arithmetic blocks like `GAIN`, `SUM` and
-`PROD` can be implicitly generated by overloaded Python operators. This strikes
-a nice balance between block diagram coding and Pythonic programming. ``` 1 #!/
-usr/bin/env python3 2 3 import bdsim 4 5 sim = bdsim.BDSim() # create simulator
-6 bd = sim.blockdiagram() # create an empty block diagram 7 8 # define the
-blocks 9 demand = bd.STEP(T=1, name='demand') 10 plant = bd.LTI_SISO(0.5, [2,
-1], name='plant') 11 scope = bd.SCOPE(styles=['k', 'r--'], movie='eg1.mp4') 12
-13 # connect the blocks using Python syntax 14 scope[0] = plant 15 scope[1] =
-demand 16 plant[0] = 10 * (demand - plant) 17 18 bd.compile() # check the
-diagram 19 bd.report() # list all blocks and wires 20 21 sim.set_options
-(animation=True) 22 out = sim.run(bd, 5, watch=[plant,]) # simulate for 5s ```
-This requires fewer lines of code and the code is more readable. Importantly,
-it results in in *exactly the same* block diagram in terms of blocks and wires
-``` Wires::
+the wire. To save figures we need to make two modifications, changing line 4 to
+``` 4 sim = bdsim.BDSim(hold=False) # create simulator ``` which prevents `.run
+()` from blocking and then deleting all the figures. Then, after the `.run()`
+we add ``` 25 scope.savefig() # save scope figure ``` If the filename is not
+given it defaults to the block name, in this case `scope.0.pdf`. The output can
+be pickled and written to a file ```[shell] examples/eg1.py -o python -mpickle
+bd.out t = ndarray:float64 (123,) x = ndarray:float64 (123, 1) xnames =
+['plantx0'] (list) y0 = ndarray:float64 (123,) y1 = ndarray:int64 (123,) ynames
+= ['plant[0]', 'demand[0]'] (list) ``` by default the results are written to
+`bd.out`, use the option `--out FILE` to set it to a specific value. The block
+parameters can also be overridden from the command line without having to edit
+the code. To increase the loop gain we could write: ```[shell] examples/eg1.py
+--set gain.0:K=20 ``` More details on this Wiki about: - [Adding blocks](https:
+//github.com/petercorke/bdsim/wiki/Adding-blocks) - [Connecting blocks](https:/
+/github.com/petercorke/bdsim/wiki/Connecting-blocks) - [Running the simulation]
+(https://github.com/petercorke/bdsim/wiki/Running) - [Command line options]
+(https://github.com/petercorke/bdsim/wiki/Runtime-options) ## Other examples In
+the folder `bdsim/examples` you can find a few other runnable examples: -
+[`eg1.py`](https://github.com/petercorke/bdsim/blob/master/examples/eg1.py) the
+example given above - [`waveform.py`](https://github.com/petercorke/bdsim/blob/
+master/examples/waveform.py) two signal generators connected to two scopes
+Examples from Chapter four of _Robotics, Vision & Control 2e (2017)_: -
+[`rvc4_2.py`](https://github.com/petercorke/bdsim/blob/master/examples/
+rvc4_2.py) Fig 4.2 - a car-like vehicle with bicycle kinematics driven by a
+rectangular pulse steering signal - [`rvc4_4.py`](https://github.com/
+petercorke/bdsim/blob/master/examples/rvc4_4.py) Fig 4.4 - a car-like vehicle
+driving to a point ![RVC Figure 4.4](https://github.com/petercorke/bdsim/raw/
+master/figs/rvc4_4.gif) - [`rvc4_6.py`](https://github.com/petercorke/bdsim/
+blob/master/examples/rvc4_6.py) Fig 4.6 - a car-like vehicle driving to/along a
+line ![RVC Figure 4.6](https://github.com/petercorke/bdsim/raw/master/figs/
+rvc4_6.gif) - [`rvc4_8.py`](https://github.com/petercorke/bdsim/blob/master/
+examples/rvc4_8.py) Fig 4.8 - a car-like vehicle using pure-pursuit trajectory
+following ![RVC Figure 4.6](https://github.com/petercorke/bdsim/raw/master/
+figs/rvc4_8.gif) - [`rvc4_11.py`](https://github.com/petercorke/bdsim/blob/
+master/examples/rvc4_11.py) Fig 4.11 a car-like vehicle driving to a pose ![RVC
+Figure 4.11](https://github.com/petercorke/bdsim/raw/master/figs/rvc4_11.gif)
+Figs 4.8 (pure pursuit) and Fig 4.21 (quadrotor control) are yet to be done. #
+A more concise way Wiring, and some simple arithmetic blocks like `GAIN`, `SUM`
+and `PROD` can be implicitly generated by overloaded Python operators. This
+strikes a nice balance between block diagram coding and Pythonic programming.
+``` 1 #!/usr/bin/env python3 2 3 import bdsim 4 5 sim = bdsim.BDSim() # create
+simulator 6 bd = sim.blockdiagram() # create an empty block diagram 7 8 #
+define the blocks 9 demand = bd.STEP(T=1, name='demand') 10 plant = bd.LTI_SISO
+(0.5, [2, 1], name='plant') 11 scope = bd.SCOPE(styles=['k', 'r--'],
+movie='eg1.mp4') 12 13 # connect the blocks using Python syntax 14 scope[0] =
+plant 15 scope[1] = demand 16 plant[0] = 10 * (demand - plant) 17 18 bd.compile
+() # check the diagram 19 bd.report() # list all blocks and wires 20 22 out =
+sim.run(bd, 5, watch=[plant,]) # simulate for 5s ``` This requires fewer lines
+of code and the code is more readable. Importantly, it results in in *exactly
+the same* block diagram in terms of blocks and wires ``` Wires::
 âââââ¬âââââââ¬âââââââ¬âââââââââââââââââââââââââââââââ¬ââââââââââ
 âid â from â to â description â type â
 âââââ¼âââââââ¼âââââââ¼âââââââââââââââââââââââââââââââ¼ââââââââââ¤
 â 0 â 1[0] â 2[0] â plant[0] --> scope.0[0] â float64 â â 1 â 0
 [0] â 2[1] â demand[0] --> scope.0[1] â int â â 2 â 0[0] â 3[0]
 â demand[0] --> _sum.0[0] â int â â 3 â 1[0] â 3[1] â plant[0] --
 > _sum.0[1] â float64 â â 4 â 3[0] â 4[0] â _sum.0[0] --> _gain.0
@@ -218,16 +233,17 @@
 bdedit: the graphical editing tool ![block diagram](https://github.com/
 petercorke/bdsim/raw/master/figs/eg1-bdedit.png) `bdedit` is a multi-platform
 PyQt5-based graphical tool to create, edit, render and execute block diagram
 models. From the examples folder ``` % bdedit eg1.bd ``` will create a display
 like that shown above. Pushing the run button, top left (triangle in circle)
 will spawn `bdrun` as a subprocess which will: * parse the JSON file *
 instantiate all blocks and wires * compile and run the diagram # Article I
-published [this article on LinkedIn](https://www.linkedin.com/in/petercorke/
-recent-activity/shares/), which describes the thouhgt process behind bdsim. #
-Limitations There are lots! The biggest is that `bdsim` is based on a very
-standard variable-step integrator from the scipy library. For discontinuous
-inputs (step, square wave, triangle wave, piecewise constant) the transitions
-get missed. This also makes it inaccurate to simulate hybrid discrete-
-continuous time systems. We really need a better integrator, perhaps [`odedc`]
-(https://help.scilab.org/docs/6.1.0/en_US/odedc.html) from SciLab could be
-integrated.
+published [this article on LinkedIn](https://www.linkedin.com/pulse/journey-
+toward-open-source-block-diagram-simulation-peter-corke/
+?trackingId=wrJYinHUgAHDq63Nv65PnA%3D%3D), which describes the thought process
+behind bdsim. # Limitations There are lots! The biggest is that `bdsim` is
+based on a very standard variable-step integrator from the scipy library. For
+discontinuous inputs (step, square wave, triangle wave, piecewise constant) the
+transitions get missed. This also makes it inaccurate to simulate hybrid
+discrete-continuous time systems. We really need a better integrator, perhaps
+[`odedc`](https://help.scilab.org/docs/6.1.0/en_US/odedc.html) from SciLab
+could be integrated.
```

### Comparing `bdsim-1.0.0/README.md` & `bdsim-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,48 @@
+Metadata-Version: 2.1
+Name: bdsim
+Version: 1.1.0
+Summary: Simulate dynamic systems expressed in block diagram form using Python
+Author-email: Peter Corke <rvc@petercorke.com>
+License: MIT License
+        
+        Copyright (c) 2020 Peter Corke
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/petercorke/bdsim
+Project-URL: documentation, https://petercorke.github.io/bdsim/
+Project-URL: repository, https://github.com/petercorke/bdsim
+Keywords: python,block diagram,dynamic simulation
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: edit
+License-File: LICENSE
+
 [![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-python)
 [![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
 
 [![PyPI version](https://badge.fury.io/py/bdsim.svg)](https://badge.fury.io/py/bdsim)
 ![Python Version](https://img.shields.io/pypi/pyversions/bdsim.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
@@ -93,22 +134,20 @@
     13	
     14	# connect the blocks
     15	bd.connect(demand, sum[0], scope[1])
     17	bd.connect(sum, gain)
     18	bd.connect(gain, plant)
     19	bd.connect(plant, sum[1], scope[0])
     20	
-    21	bd.compile()   # check the diagram
-    22	bd.report()    # list all blocks and wires
-    23
+    21	bd.compile()          # check the diagram
+    22
+    23	sim.report(bd)   # list the system
     24  out = sim.run(bd, 5)   # simulate for 5s
-    25  sim.savefig(scope, 'scope0')
-    26  sim.done(bd, block=True)
 ```
-which is just 16 lines of executable code.
+which is just 15 lines of executable code.
 
 The red block annotations on the hand-drawn diagram are used as the names of the variables holding references to the block instance. The blocks can also have user-assigned names, see lines 8 and 11, which are used in diagnostics and as labels in plots.
 
 After the blocks are created their input and output ports need to be connected. In `bdsim` all wires are point to point, a *one-to-many* connection is implemented by *many* wires,
 for example
 ```
 bd.connect(source, dest1, dest2, ...)
@@ -122,16 +161,103 @@
 bd.connect(source[2:5], dest[3:6)
 ```
 will connect `source[2]` -> `dest[3]`, `source[3]` -> `dest[4]`, `source[4]` -> `dest[5]`.
 The number of wires in each slice must be consistent.  You could even do a cross over by connecting `source[2:5]` to `dest[6:3:-1]`.
 
 Line 21 assembles all the blocks and wires, instantiates subsystems, checks connectivity to create a flat wire list, and then builds the dataflow execution plan.
 
-Line 22 generates a report, in tabular form, showing a summary of the block diagram:
+Line 23 generates a report, in tabular form, showing a summary of the block diagram:
+
+```
+┌────────┬──────────┬────────┬────────┬─────────────┐
+│ block  │   type   │ inport │ source │ source type │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│demand@ │ step     │        │        │             │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│gain.0  │ gain     │ 0      │ sum.0  │ float64     │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│plant   │ lti_siso │ 0      │ gain.0 │ float64     │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│scope.0 │ scope    │ 0      │ plant  │ float64     │
+│        │          │ 1      │ demand │ int         │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│sum.0   │ sum      │ 0      │ demand │ int         │
+│        │          │ 1      │ plant  │ float64     │
+└────────┴──────────┴────────┴────────┴─────────────┘
+```
+
+Line 24 runs the simulation for 5 seconds 
+using the default variable-step RK45 solver and saves output values at least every 0.05s.  It
+causes the following output
+
+```
+>>> Start simulation: T = 5.00, dt = 0.050
+  Continuous state variables: 1
+     x0 =  [0.]
+  Discrete state variables:   0
+
+no graphics backend specified: Qt5Agg found, using instead of MacOSX
+
+bdsim ◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉ 100.0% - 0s
+
+<<< Simulation complete
+  block diagram evaluations: 784
+  block diagram exec time:   0.075 ms
+  time steps:                123
+  integration intervals:     2
+```
+
+This provides a summary of the number of states for the complete system: the number of continuous states, the number
+of discrete states, and the initial value of the state vectors.
+
+During execution a progress bar is updated and scope blocks pops up a graphical window
+
+![bdsim output](https://github.com/petercorke/bdsim/raw/master/figs/Figure_1.png)
+
+The simulation results are in a container object (`BDStruct`)
+```
+>>> out
+t      = ndarray:float64 (123,)
+x      = ndarray:float64 (123, 1)
+xnames = ['plantx0'] (list)
+ynames = [] (list)            
+```
+which contains an array of time values, an array of state values, and a list of the
+names of the state variables.
+
+By default the `.run()` method at line 24 blocks blocks the script until all figure
+windows are closed (by pressing the operating system close button or typing "q"), or the
+script is killed with SIGINT. If you want to continue the script with the figures still
+active then the `hold=False` option should be set.
 
+If we wished to also record additional outputs, we can add them as _watched_ signals
+```
+out = sim.run(bd, watch=[demand, sum])  # simulate for 5s
+```
+and now the output is
+```
+>>> out
+t      = ndarray:float64 (123,)
+x      = ndarray:float64 (123, 1)
+xnames = ['plantx0'] (list)
+y0     = ndarray:float64 (123,)
+y1     = ndarray:int64 (123,)
+ynames = ['plant[0]', 'demand[0]'] (list)
+```
+where
+
+- `t` the time vector: ndarray, shape=(M,)
+- `x` is the state vector: ndarray, shape=(M,N), one row per timestep
+- `xnames` is a list of the names of the states corresponding to columns of `x`, eg. "plant.x0"
+
+The `watch` argument is a list of outputs to log, in this case `plant` defaults
+to output port 0.  This information is saved in additional variables `y0`, `y1`
+etc.  `ynames` is a list of the names of the watched variables.
+
+An alternative system report, created by `sim.report(bd, type="lists")` is more detailed
 ```
 Blocks::
 
 ┌───┬─────────┬─────┬──────┬────────┬─────────┬───────┐
 │id │    name │ nin │ nout │ nstate │ ndstate │ type  │
 ├───┼─────────┼─────┼──────┼────────┼─────────┼───────┤
 │ 0 │  demand │   0 │    1 │      0 │       0 │ step  │
@@ -149,88 +275,70 @@
 │ 0 │ 0[0] │ 1[0] │ demand[0] --> sum.0[0]   │ int     │
 │ 1 │ 0[0] │ 4[1] │ demand[0] --> scope.0[1] │ int     │
 │ 2 │ 3[0] │ 1[1] │ plant[0] --> sum.0[1]    │ float64 │
 │ 3 │ 1[0] │ 2[0] │ sum.0[0] --> gain.0[0]   │ float64 │
 │ 4 │ 2[0] │ 3[0] │ gain.0[0] --> plant[0]   │ float64 │
 │ 5 │ 3[0] │ 4[0] │ plant[0] --> scope.0[0]  │ float64 │
 └───┴──────┴──────┴──────────────────────────┴─────────┘
-
-Continuous state variables:   1
-Discrete state variables:     0
-initial state  x0 =  [0.]
 ```
 In the first table we can see key information about each block, its `id` (used internally), name, the number of input and output ports, the number of
 continuous- and discrete-time states, and the type which is the block class.  Note that the name is auto-generated based on the type, except if it has
 been set explicitly as for the blocks `demand` and `plant`.
 
 The second table shows all wires in point-to-point form, showing the start and end block and port (the block is represented here by its `id`) and the type of the object sent along the wire.
 
-Finally, there is a summary of the number of states for the complete system: the number of continuous states, the number
-of discrete states, and the initial value of the continuous state vector.
-
-Line 24 runs the simulation for 5 seconds 
-using the default variable-step RK45 solver and saves output values at least every 0.1s.  The scope block pops up a graph
-
-![bdsim output](https://github.com/petercorke/bdsim/raw/master/figs/Figure_1.png)
-
-The simulation results are in a container object
+To save figures we need to make two modifications, changing line 4 to
 ```
->>> out
-results:
-t           | ndarray (67,)
-x           | ndarray (67, 1)
-xnames      | list              
+     4  sim = bdsim.BDSim(hold=False)  # create simulator
 ```
-which contains an array of time values, an array of state values, and a list of the names of the state variables.
-
-Line 25 saves the content of the scope to be saved in the file called `scope0.pdf`.
-
-Line 26 blocks the script until all figure windows are closed, or the script is killed with SIGINT.
-
-The result `out` is effectively a structure with elements
-
+which prevents `.run()` from blocking and then deleting all the figures.
+Then, after the `.run()` we add 
 ```
->>> out
-results:
-t           | ndarray (67,)
-x           | ndarray (67, 1)
-xnames      | list        
-y0          | ndarray (67,)
-y1          | ndarray (67,)
-ynames      | list   
+     25 scope.savefig()  # save scope figure
 ```
-where
+If the filename is not given it defaults to the block name, in this case `scope.0.pdf`.
 
-- `t` the time vector: ndarray, shape=(M,)
-- `x` is the state vector: ndarray, shape=(M,N), one row per timestep
-- `xnames` is a list of the names of the states corresponding to columns of `x`, eg. "plant.x0"
 
-The `watch` argument is a list of outputs to log, in this case `plant` defaults
-to output port 0.  This information is saved in additional variables `y0`, `y1`
-etc.  `ynames` is a list of the names of the watched variables.
+The output can be pickled and written to a file
 
-Line 29 saves the scope graphics as a PDF file.
+```[shell]
+examples/eg1.py -o
+python -mpickle bd.out
+t      = ndarray:float64 (123,)
+x      = ndarray:float64 (123, 1)
+xnames = ['plantx0'] (list)
+y0     = ndarray:float64 (123,)
+y1     = ndarray:int64 (123,)
+ynames = ['plant[0]', 'demand[0]'] (list)
+```
 
-Line 30 blocks until the last figure is dismissed.
+by default the results are written to `bd.out`, use the option `--out FILE` to set it
+to a specific value.
 
-More details on this Wiki about:
+The block parameters can also be overridden from the command line without having to 
+edit the code.  To increase the loop gain we could write:
+```[shell]
+examples/eg1.py --set gain.0:K=20
+```
 
-- [Adding blocks](Adding-blocks)
-- [Connecting blocks](Connecting-blocks)
-- [Running the simulation](Running)
+More details on this Wiki about:
 
+- [Adding blocks](https://github.com/petercorke/bdsim/wiki/Adding-blocks)
+- [Connecting blocks](https://github.com/petercorke/bdsim/wiki/Connecting-blocks)
+- [Running the simulation](https://github.com/petercorke/bdsim/wiki/Running)
+- [Command line options](https://github.com/petercorke/bdsim/wiki/Runtime-options)
 
 ## Other examples
 
 In the folder `bdsim/examples` you can find a few other runnable examples:
 
 - [`eg1.py`](https://github.com/petercorke/bdsim/blob/master/examples/eg1.py) the example given above
 - [`waveform.py`](https://github.com/petercorke/bdsim/blob/master/examples/waveform.py) two signal generators connected to two scopes
 
-Examples from Chapter four of _Robotics, Vision & Control (2017)_:
+Examples from Chapter four of _Robotics, Vision & Control 2e (2017)_:
 
 - [`rvc4_2.py`](https://github.com/petercorke/bdsim/blob/master/examples/rvc4_2.py) Fig 4.2 - a car-like vehicle with bicycle kinematics driven by a rectangular pulse steering signal
 - [`rvc4_4.py`](https://github.com/petercorke/bdsim/blob/master/examples/rvc4_4.py) Fig 4.4 - a car-like vehicle driving to a point
 
 ![RVC Figure 4.4](https://github.com/petercorke/bdsim/raw/master/figs/rvc4_4.gif)
 
 - [`rvc4_6.py`](https://github.com/petercorke/bdsim/blob/master/examples/rvc4_6.py) Fig 4.6 - a car-like vehicle driving to/along a line
@@ -268,15 +376,14 @@
     14  scope[0] = plant
     15  scope[1] = demand
     16  plant[0] = 10 * (demand - plant)
     17
     18  bd.compile()   # check the diagram
     19  bd.report()    # list all blocks and wires
     20
-    21  sim.set_options(animation=True)
     22  out = sim.run(bd, 5, watch=[plant,])  # simulate for 5s
 ```
 This requires fewer lines of code and the code is more readable. Importantly, it results in in *exactly the same* block diagram in terms of blocks and wires
 ```
 Wires::
 
 ┌───┬──────┬──────┬──────────────────────────────┬─────────┐
@@ -306,14 +413,14 @@
 
 * parse the JSON file
 * instantiate all blocks and wires
 * compile and run the diagram
 
 # Article
 
-I published [this article on LinkedIn](https://www.linkedin.com/in/petercorke/recent-activity/shares/), which describes the thouhgt process behind bdsim.
+I published [this article on LinkedIn](https://www.linkedin.com/pulse/journey-toward-open-source-block-diagram-simulation-peter-corke/?trackingId=wrJYinHUgAHDq63Nv65PnA%3D%3D), which describes the thought process behind bdsim.
 
 # Limitations
 
 There are lots!  The biggest is that `bdsim` is based on a very standard variable-step integrator from the scipy library.  For discontinuous inputs (step, square wave, triangle wave, piecewise constant) the transitions get missed.  This also makes it inaccurate to simulate hybrid discrete-continuous time systems.  We really need a better integrator, perhaps [`odedc`](https://help.scilab.org/docs/6.1.0/en_US/odedc.html) from SciLab could be integrated.
```

#### html2text {}

```diff
@@ -1,22 +1,46 @@
-[![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/
-robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://
-github.com/petercorke/robotics-toolbox-python) [![QUT Centre for Robotics Open
-Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https:
-//qcr.github.io) [![PyPI version](https://badge.fury.io/py/bdsim.svg)](https://
-badge.fury.io/py/bdsim) ![Python Version](https://img.shields.io/pypi/
-pyversions/bdsim.svg) [![License: MIT](https://img.shields.io/badge/License-
-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Build Status](https://
-github.com/petercorke/bdsim/workflows/build/badge.svg?branch=master)](https://
-github.com/petercorke/bdsim/actions?query=workflow%3Abuild) [![Coverage](https:
-//codecov.io/gh/petercorke/bdsim/branch/master/graph/badge.svg)](https://
-codecov.io/gh/petercorke/bdsim) [![PyPI - Downloads](https://img.shields.io/
-pypi/dm/bdsim)](https://pypistats.org/packages/bdsim) [![GitHub stars](https://
-img.shields.io/github/stars/petercorke/bdsim.svg?style=social&label=Star)]
-(https://GitHub.com/petercorke/bdsim/stargazers/)
+Metadata-Version: 2.1 Name: bdsim Version: 1.1.0 Summary: Simulate dynamic
+systems expressed in block diagram form using Python Author-email: Peter Corke
+petercorke.com> License: MIT License Copyright (c) 2020 Peter Corke Permission
+is hereby granted, free of charge, to any person obtaining a copy of this
+software and associated documentation files (the "Software"), to deal in the
+Software without restriction, including without limitation the rights to use,
+copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
+Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions: The above copyright notice and this
+permission notice shall be included in all copies or substantial portions of
+the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
+EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
+OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE. Project-URL: homepage, https://github.com/petercorke/
+bdsim Project-URL: documentation, https://petercorke.github.io/bdsim/ Project-
+URL: repository, https://github.com/petercorke/bdsim Keywords: python,block
+diagram,dynamic simulation Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
+System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
+markdown Provides-Extra: dev Provides-Extra: docs Provides-Extra: edit License-
+File: LICENSE [![A Python Robotics Package](https://raw.githubusercontent.com/
+petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)]
+(https://github.com/petercorke/robotics-toolbox-python) [![QUT Centre for
+Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/
+badge.svg)](https://qcr.github.io) [![PyPI version](https://badge.fury.io/py/
+bdsim.svg)](https://badge.fury.io/py/bdsim) ![Python Version](https://
+img.shields.io/pypi/pyversions/bdsim.svg) [![License: MIT](https://
+img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/
+MIT) [![Build Status](https://github.com/petercorke/bdsim/workflows/build/
+badge.svg?branch=master)](https://github.com/petercorke/bdsim/
+actions?query=workflow%3Abuild) [![Coverage](https://codecov.io/gh/petercorke/
+bdsim/branch/master/graph/badge.svg)](https://codecov.io/gh/petercorke/bdsim)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/bdsim)](https://
+pypistats.org/packages/bdsim) [![GitHub stars](https://img.shields.io/github/
+stars/petercorke/bdsim.svg?style=social&label=Star)](https://GitHub.com/
+petercorke/bdsim/stargazers/)
                                       A Python block diagram simulation package
                                           * GitHub_repository
 [https://github.com/petercorke/bdsim/     * Documentation
 raw/master/figs/                          * Wiki_(examples_and_details)
 BDSimLogo_NoBackgnd@2x.png]               * Installation
                                           * Dependencies: numpy, scipy,
                                             matplotlib, ansitable, ffmpeg (if
@@ -69,38 +93,84 @@
 examples/eg1.py)) ```python 1 #!/usr/bin/env python3 2 import bdsim 4 sim =
 bdsim.BDSim() # create simulator 5 bd = sim.blockdiagram() # create an empty
 block diagram 6 7 # define the blocks 8 demand = bd.STEP(T=1, name='demand') 9
 sum = bd.SUM('+-') 10 gain = bd.GAIN(10) 11 plant = bd.LTI_SISO(0.5, [2, 1],
 name='plant') 12 scope = bd.SCOPE(styles=['k', 'r--']) 13 14 # connect the
 blocks 15 bd.connect(demand, sum[0], scope[1]) 17 bd.connect(sum, gain) 18
 bd.connect(gain, plant) 19 bd.connect(plant, sum[1], scope[0]) 20 21 bd.compile
-() # check the diagram 22 bd.report() # list all blocks and wires 23 24 out =
-sim.run(bd, 5) # simulate for 5s 25 sim.savefig(scope, 'scope0') 26 sim.done
-(bd, block=True) ``` which is just 16 lines of executable code. The red block
-annotations on the hand-drawn diagram are used as the names of the variables
-holding references to the block instance. The blocks can also have user-
-assigned names, see lines 8 and 11, which are used in diagnostics and as labels
-in plots. After the blocks are created their input and output ports need to be
-connected. In `bdsim` all wires are point to point, a *one-to-many* connection
-is implemented by *many* wires, for example ``` bd.connect(source, dest1,
-dest2, ...) ``` creates individual wires from `source` -> `dest1`, `source` -
-> `dest2` and so on. Ports are designated using Python indexing notation, for
-example `block[2]` is port 2 (the third port) of `block`. Whether it is an
-input or output port depends on context. In the example above an index on the
-first argument refers to an output port, while on the second (or subsequent)
-arguments it refers to an input port. If a block has only a single input or
-output port then no index is required, 0 is assumed. A group of ports can be
-denoted using slice notation, for example ``` bd.connect(source[2:5], dest[3:6)
-``` will connect `source[2]` -> `dest[3]`, `source[3]` -> `dest[4]`, `source
-[4]` -> `dest[5]`. The number of wires in each slice must be consistent. You
-could even do a cross over by connecting `source[2:5]` to `dest[6:3:-1]`. Line
-21 assembles all the blocks and wires, instantiates subsystems, checks
+() # check the diagram 22 23 sim.report(bd) # list the system 24 out = sim.run
+(bd, 5) # simulate for 5s ``` which is just 15 lines of executable code. The
+red block annotations on the hand-drawn diagram are used as the names of the
+variables holding references to the block instance. The blocks can also have
+user-assigned names, see lines 8 and 11, which are used in diagnostics and as
+labels in plots. After the blocks are created their input and output ports need
+to be connected. In `bdsim` all wires are point to point, a *one-to-many*
+connection is implemented by *many* wires, for example ``` bd.connect(source,
+dest1, dest2, ...) ``` creates individual wires from `source` -> `dest1`,
+`source` -> `dest2` and so on. Ports are designated using Python indexing
+notation, for example `block[2]` is port 2 (the third port) of `block`. Whether
+it is an input or output port depends on context. In the example above an index
+on the first argument refers to an output port, while on the second (or
+subsequent) arguments it refers to an input port. If a block has only a single
+input or output port then no index is required, 0 is assumed. A group of ports
+can be denoted using slice notation, for example ``` bd.connect(source[2:5],
+dest[3:6) ``` will connect `source[2]` -> `dest[3]`, `source[3]` -> `dest[4]`,
+`source[4]` -> `dest[5]`. The number of wires in each slice must be consistent.
+You could even do a cross over by connecting `source[2:5]` to `dest[6:3:-1]`.
+Line 21 assembles all the blocks and wires, instantiates subsystems, checks
 connectivity to create a flat wire list, and then builds the dataflow execution
-plan. Line 22 generates a report, in tabular form, showing a summary of the
-block diagram: ``` Blocks::
+plan. Line 23 generates a report, in tabular form, showing a summary of the
+block diagram: ```
+ââââââââââ¬âââââââââââ¬âââââââââ¬âââââââââ¬ââââââââââââââ
+â block â type â inport â source â source type â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âdemand@ â step â â â â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âgain.0 â gain â 0 â sum.0 â float64 â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âplant â lti_siso â 0 â gain.0 â float64 â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âscope.0 â scope â 0 â plant â float64 â â â â 1 â demand
+â int â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âsum.0 â sum â 0 â demand â int â â â â 1 â plant â
+float64 â
+ââââââââââ´âââââââââââ´âââââââââ´âââââââââ´ââââââââââââââ
+``` Line 24 runs the simulation for 5 seconds using the default variable-step
+RK45 solver and saves output values at least every 0.05s. It causes the
+following output ``` >>> Start simulation: T = 5.00, dt = 0.050 Continuous
+state variables: 1 x0 = [0.] Discrete state variables: 0 no graphics backend
+specified: Qt5Agg found, using instead of MacOSX bdsim
+ââââââââââââââââââââââââââââââââ
+100.0% - 0s <<< Simulation complete block diagram evaluations: 784 block
+diagram exec time: 0.075 ms time steps: 123 integration intervals: 2 ``` This
+provides a summary of the number of states for the complete system: the number
+of continuous states, the number of discrete states, and the initial value of
+the state vectors. During execution a progress bar is updated and scope blocks
+pops up a graphical window ![bdsim output](https://github.com/petercorke/bdsim/
+raw/master/figs/Figure_1.png) The simulation results are in a container object
+(`BDStruct`) ``` >>> out t = ndarray:float64 (123,) x = ndarray:float64 (123,
+1) xnames = ['plantx0'] (list) ynames = [] (list) ``` which contains an array
+of time values, an array of state values, and a list of the names of the state
+variables. By default the `.run()` method at line 24 blocks blocks the script
+until all figure windows are closed (by pressing the operating system close
+button or typing "q"), or the script is killed with SIGINT. If you want to
+continue the script with the figures still active then the `hold=False` option
+should be set. If we wished to also record additional outputs, we can add them
+as _watched_ signals ``` out = sim.run(bd, watch=[demand, sum]) # simulate for
+5s ``` and now the output is ``` >>> out t = ndarray:float64 (123,) x =
+ndarray:float64 (123, 1) xnames = ['plantx0'] (list) y0 = ndarray:float64
+(123,) y1 = ndarray:int64 (123,) ynames = ['plant[0]', 'demand[0]'] (list) ```
+where - `t` the time vector: ndarray, shape=(M,) - `x` is the state vector:
+ndarray, shape=(M,N), one row per timestep - `xnames` is a list of the names of
+the states corresponding to columns of `x`, eg. "plant.x0" The `watch` argument
+is a list of outputs to log, in this case `plant` defaults to output port 0.
+This information is saved in additional variables `y0`, `y1` etc. `ynames` is a
+list of the names of the watched variables. An alternative system report,
+created by `sim.report(bd, type="lists")` is more detailed ``` Blocks::
 âââââ¬ââââââââââ¬ââââââ¬âââââââ¬âââââââââ¬ââââââââââ¬ââââââââ
 âid â name â nin â nout â nstate â ndstate â type â
 âââââ¼ââââââââââ¼ââââââ¼âââââââ¼âââââââââ¼ââââââââââ¼ââââââââ¤
 â 0 â demand â 0 â 1 â 0 â 0 â step â â 1 â sum.0 â 2 â
 1 â 0 â 0 â sum â â 2 â gain.0 â 1 â 1 â 0 â 0 â gain â
 â 3 â plant â 1 â 1 â 1 â 0 â LTI â â 4 â scope.0 â 2 â
 0 â 0 â 0 â scope â
@@ -112,79 +182,71 @@
 â 0 â 0[0] â 1[0] â demand[0] --> sum.0[0] â int â â 1 â 0[0]
 â 4[1] â demand[0] --> scope.0[1] â int â â 2 â 3[0] â 1[1] â
 plant[0] --> sum.0[1] â float64 â â 3 â 1[0] â 2[0] â sum.0[0] --
 > gain.0[0] â float64 â â 4 â 2[0] â 3[0] â gain.0[0] --> plant[0]
 â float64 â â 5 â 3[0] â 4[0] â plant[0] --> scope.0[0] â float64
 â
 âââââ´âââââââ´âââââââ´âââââââââââââââââââââââââââ´ââââââââââ
-Continuous state variables: 1 Discrete state variables: 0 initial state x0 =
-[0.] ``` In the first table we can see key information about each block, its
-`id` (used internally), name, the number of input and output ports, the number
-of continuous- and discrete-time states, and the type which is the block class.
+``` In the first table we can see key information about each block, its `id`
+(used internally), name, the number of input and output ports, the number of
+continuous- and discrete-time states, and the type which is the block class.
 Note that the name is auto-generated based on the type, except if it has been
 set explicitly as for the blocks `demand` and `plant`. The second table shows
 all wires in point-to-point form, showing the start and end block and port (the
 block is represented here by its `id`) and the type of the object sent along
-the wire. Finally, there is a summary of the number of states for the complete
-system: the number of continuous states, the number of discrete states, and the
-initial value of the continuous state vector. Line 24 runs the simulation for 5
-seconds using the default variable-step RK45 solver and saves output values at
-least every 0.1s. The scope block pops up a graph ![bdsim output](https://
-github.com/petercorke/bdsim/raw/master/figs/Figure_1.png) The simulation
-results are in a container object ``` >>> out results: t | ndarray (67,) x |
-ndarray (67, 1) xnames | list ``` which contains an array of time values, an
-array of state values, and a list of the names of the state variables. Line 25
-saves the content of the scope to be saved in the file called `scope0.pdf`.
-Line 26 blocks the script until all figure windows are closed, or the script is
-killed with SIGINT. The result `out` is effectively a structure with elements
-``` >>> out results: t | ndarray (67,) x | ndarray (67, 1) xnames | list y0 |
-ndarray (67,) y1 | ndarray (67,) ynames | list ``` where - `t` the time vector:
-ndarray, shape=(M,) - `x` is the state vector: ndarray, shape=(M,N), one row
-per timestep - `xnames` is a list of the names of the states corresponding to
-columns of `x`, eg. "plant.x0" The `watch` argument is a list of outputs to
-log, in this case `plant` defaults to output port 0. This information is saved
-in additional variables `y0`, `y1` etc. `ynames` is a list of the names of the
-watched variables. Line 29 saves the scope graphics as a PDF file. Line 30
-blocks until the last figure is dismissed. More details on this Wiki about: -
-[Adding blocks](Adding-blocks) - [Connecting blocks](Connecting-blocks) -
-[Running the simulation](Running) ## Other examples In the folder `bdsim/
-examples` you can find a few other runnable examples: - [`eg1.py`](https://
-github.com/petercorke/bdsim/blob/master/examples/eg1.py) the example given
-above - [`waveform.py`](https://github.com/petercorke/bdsim/blob/master/
-examples/waveform.py) two signal generators connected to two scopes Examples
-from Chapter four of _Robotics, Vision & Control (2017)_: - [`rvc4_2.py`]
-(https://github.com/petercorke/bdsim/blob/master/examples/rvc4_2.py) Fig 4.2 -
-a car-like vehicle with bicycle kinematics driven by a rectangular pulse
-steering signal - [`rvc4_4.py`](https://github.com/petercorke/bdsim/blob/
-master/examples/rvc4_4.py) Fig 4.4 - a car-like vehicle driving to a point !
-[RVC Figure 4.4](https://github.com/petercorke/bdsim/raw/master/figs/
-rvc4_4.gif) - [`rvc4_6.py`](https://github.com/petercorke/bdsim/blob/master/
-examples/rvc4_6.py) Fig 4.6 - a car-like vehicle driving to/along a line ![RVC
-Figure 4.6](https://github.com/petercorke/bdsim/raw/master/figs/rvc4_6.gif) -
-[`rvc4_8.py`](https://github.com/petercorke/bdsim/blob/master/examples/
-rvc4_8.py) Fig 4.8 - a car-like vehicle using pure-pursuit trajectory following
-![RVC Figure 4.6](https://github.com/petercorke/bdsim/raw/master/figs/
-rvc4_8.gif) - [`rvc4_11.py`](https://github.com/petercorke/bdsim/blob/master/
-examples/rvc4_11.py) Fig 4.11 a car-like vehicle driving to a pose ![RVC Figure
-4.11](https://github.com/petercorke/bdsim/raw/master/figs/rvc4_11.gif) Figs 4.8
-(pure pursuit) and Fig 4.21 (quadrotor control) are yet to be done. # A more
-concise way Wiring, and some simple arithmetic blocks like `GAIN`, `SUM` and
-`PROD` can be implicitly generated by overloaded Python operators. This strikes
-a nice balance between block diagram coding and Pythonic programming. ``` 1 #!/
-usr/bin/env python3 2 3 import bdsim 4 5 sim = bdsim.BDSim() # create simulator
-6 bd = sim.blockdiagram() # create an empty block diagram 7 8 # define the
-blocks 9 demand = bd.STEP(T=1, name='demand') 10 plant = bd.LTI_SISO(0.5, [2,
-1], name='plant') 11 scope = bd.SCOPE(styles=['k', 'r--'], movie='eg1.mp4') 12
-13 # connect the blocks using Python syntax 14 scope[0] = plant 15 scope[1] =
-demand 16 plant[0] = 10 * (demand - plant) 17 18 bd.compile() # check the
-diagram 19 bd.report() # list all blocks and wires 20 21 sim.set_options
-(animation=True) 22 out = sim.run(bd, 5, watch=[plant,]) # simulate for 5s ```
-This requires fewer lines of code and the code is more readable. Importantly,
-it results in in *exactly the same* block diagram in terms of blocks and wires
-``` Wires::
+the wire. To save figures we need to make two modifications, changing line 4 to
+``` 4 sim = bdsim.BDSim(hold=False) # create simulator ``` which prevents `.run
+()` from blocking and then deleting all the figures. Then, after the `.run()`
+we add ``` 25 scope.savefig() # save scope figure ``` If the filename is not
+given it defaults to the block name, in this case `scope.0.pdf`. The output can
+be pickled and written to a file ```[shell] examples/eg1.py -o python -mpickle
+bd.out t = ndarray:float64 (123,) x = ndarray:float64 (123, 1) xnames =
+['plantx0'] (list) y0 = ndarray:float64 (123,) y1 = ndarray:int64 (123,) ynames
+= ['plant[0]', 'demand[0]'] (list) ``` by default the results are written to
+`bd.out`, use the option `--out FILE` to set it to a specific value. The block
+parameters can also be overridden from the command line without having to edit
+the code. To increase the loop gain we could write: ```[shell] examples/eg1.py
+--set gain.0:K=20 ``` More details on this Wiki about: - [Adding blocks](https:
+//github.com/petercorke/bdsim/wiki/Adding-blocks) - [Connecting blocks](https:/
+/github.com/petercorke/bdsim/wiki/Connecting-blocks) - [Running the simulation]
+(https://github.com/petercorke/bdsim/wiki/Running) - [Command line options]
+(https://github.com/petercorke/bdsim/wiki/Runtime-options) ## Other examples In
+the folder `bdsim/examples` you can find a few other runnable examples: -
+[`eg1.py`](https://github.com/petercorke/bdsim/blob/master/examples/eg1.py) the
+example given above - [`waveform.py`](https://github.com/petercorke/bdsim/blob/
+master/examples/waveform.py) two signal generators connected to two scopes
+Examples from Chapter four of _Robotics, Vision & Control 2e (2017)_: -
+[`rvc4_2.py`](https://github.com/petercorke/bdsim/blob/master/examples/
+rvc4_2.py) Fig 4.2 - a car-like vehicle with bicycle kinematics driven by a
+rectangular pulse steering signal - [`rvc4_4.py`](https://github.com/
+petercorke/bdsim/blob/master/examples/rvc4_4.py) Fig 4.4 - a car-like vehicle
+driving to a point ![RVC Figure 4.4](https://github.com/petercorke/bdsim/raw/
+master/figs/rvc4_4.gif) - [`rvc4_6.py`](https://github.com/petercorke/bdsim/
+blob/master/examples/rvc4_6.py) Fig 4.6 - a car-like vehicle driving to/along a
+line ![RVC Figure 4.6](https://github.com/petercorke/bdsim/raw/master/figs/
+rvc4_6.gif) - [`rvc4_8.py`](https://github.com/petercorke/bdsim/blob/master/
+examples/rvc4_8.py) Fig 4.8 - a car-like vehicle using pure-pursuit trajectory
+following ![RVC Figure 4.6](https://github.com/petercorke/bdsim/raw/master/
+figs/rvc4_8.gif) - [`rvc4_11.py`](https://github.com/petercorke/bdsim/blob/
+master/examples/rvc4_11.py) Fig 4.11 a car-like vehicle driving to a pose ![RVC
+Figure 4.11](https://github.com/petercorke/bdsim/raw/master/figs/rvc4_11.gif)
+Figs 4.8 (pure pursuit) and Fig 4.21 (quadrotor control) are yet to be done. #
+A more concise way Wiring, and some simple arithmetic blocks like `GAIN`, `SUM`
+and `PROD` can be implicitly generated by overloaded Python operators. This
+strikes a nice balance between block diagram coding and Pythonic programming.
+``` 1 #!/usr/bin/env python3 2 3 import bdsim 4 5 sim = bdsim.BDSim() # create
+simulator 6 bd = sim.blockdiagram() # create an empty block diagram 7 8 #
+define the blocks 9 demand = bd.STEP(T=1, name='demand') 10 plant = bd.LTI_SISO
+(0.5, [2, 1], name='plant') 11 scope = bd.SCOPE(styles=['k', 'r--'],
+movie='eg1.mp4') 12 13 # connect the blocks using Python syntax 14 scope[0] =
+plant 15 scope[1] = demand 16 plant[0] = 10 * (demand - plant) 17 18 bd.compile
+() # check the diagram 19 bd.report() # list all blocks and wires 20 22 out =
+sim.run(bd, 5, watch=[plant,]) # simulate for 5s ``` This requires fewer lines
+of code and the code is more readable. Importantly, it results in in *exactly
+the same* block diagram in terms of blocks and wires ``` Wires::
 âââââ¬âââââââ¬âââââââ¬âââââââââââââââââââââââââââââââ¬ââââââââââ
 âid â from â to â description â type â
 âââââ¼âââââââ¼âââââââ¼âââââââââââââââââââââââââââââââ¼ââââââââââ¤
 â 0 â 1[0] â 2[0] â plant[0] --> scope.0[0] â float64 â â 1 â 0
 [0] â 2[1] â demand[0] --> scope.0[1] â int â â 2 â 0[0] â 3[0]
 â demand[0] --> _sum.0[0] â int â â 3 â 1[0] â 3[1] â plant[0] --
 > _sum.0[1] â float64 â â 4 â 3[0] â 4[0] â _sum.0[0] --> _gain.0
@@ -195,16 +257,17 @@
 bdedit: the graphical editing tool ![block diagram](https://github.com/
 petercorke/bdsim/raw/master/figs/eg1-bdedit.png) `bdedit` is a multi-platform
 PyQt5-based graphical tool to create, edit, render and execute block diagram
 models. From the examples folder ``` % bdedit eg1.bd ``` will create a display
 like that shown above. Pushing the run button, top left (triangle in circle)
 will spawn `bdrun` as a subprocess which will: * parse the JSON file *
 instantiate all blocks and wires * compile and run the diagram # Article I
-published [this article on LinkedIn](https://www.linkedin.com/in/petercorke/
-recent-activity/shares/), which describes the thouhgt process behind bdsim. #
-Limitations There are lots! The biggest is that `bdsim` is based on a very
-standard variable-step integrator from the scipy library. For discontinuous
-inputs (step, square wave, triangle wave, piecewise constant) the transitions
-get missed. This also makes it inaccurate to simulate hybrid discrete-
-continuous time systems. We really need a better integrator, perhaps [`odedc`]
-(https://help.scilab.org/docs/6.1.0/en_US/odedc.html) from SciLab could be
-integrated.
+published [this article on LinkedIn](https://www.linkedin.com/pulse/journey-
+toward-open-source-block-diagram-simulation-peter-corke/
+?trackingId=wrJYinHUgAHDq63Nv65PnA%3D%3D), which describes the thought process
+behind bdsim. # Limitations There are lots! The biggest is that `bdsim` is
+based on a very standard variable-step integrator from the scipy library. For
+discontinuous inputs (step, square wave, triangle wave, piecewise constant) the
+transitions get missed. This also makes it inaccurate to simulate hybrid
+discrete-continuous time systems. We really need a better integrator, perhaps
+[`odedc`](https://help.scilab.org/docs/6.1.0/en_US/odedc.html) from SciLab
+could be integrated.
```

### Comparing `bdsim-1.0.0/bdsim/bdrun.py` & `bdsim-1.1.0/bdsim/bdrun.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import sys
+import traceback
 
 from bdsim import BDSim
 from colored import fg, attr
 
 # available for use in bdedit expressions
 import numpy as np
 import math
@@ -75,78 +76,102 @@
             connector_dict[end] = start
 
         elif block["block_type"] == "MAIN":
             continue  # nothing to be done
 
         else:
             # regular bdsim Block
-            block_init = bd.__dict__[block["block_type"]]  # block class
+            try:
+                block_init = bd.__dict__[block["block_type"]]  # block class
+            except KeyError:
+                print(fg("red"))
+                print(f"block [{block['block_type']}] not loaded, check BDSIMPATH")
+                print(attr(0))
+
             params = dict(block["parameters"])  # block params as a dict
 
             if verbose:
                 print(f"[{block['title']}]:")
             # process the parameters
+            default_params = []
             for key, value in params.items():
                 if verbose:
                     print(f"    {key}: ", end="")
 
                 newvalue = None
                 if isinstance(value, str):
                     # either an "any" type or an assignment
                     if value[0] == "=":
                         # assignment
                         try:
                             newvalue = eval(value[1:], namespace)
                         except (ValueError, TypeError, NameError, SyntaxError):
                             print(fg("red"))
                             print(
-                                f"bdload: error resolving parameter {key}: {value} for block [{block['title']}]"
+                                f"bdload: error resolving parameter {key}: {value} for"
+                                f" block [{block['title']}]"
                             )
                             traceback.print_exc(limit=-1, file=sys.stderr)
                             print(attr(0))
                             raise RuntimeError(
-                                f"cannot instantiate block {block['title']} - bad parameters?"
+                                f"cannot instantiate block [{block['title']}] - bad"
+                                " parameters?"
                             )
                     else:
                         # assume it's an "any" type, attempt to evaluate it
                         try:
                             newvalue = eval(value, namespace)
                         except (NameError, SyntaxError):
                             pass
+                else:
+                    newvalue = value
 
-                if newvalue is not None:
-                    params[key] = newvalue
+                if newvalue is None:
+                    # default_params.append(key)
                     if verbose:
-                        print(f" {value} -> {newvalue}")
+                        print(f" {value} default")
                 else:
+                    params[key] = newvalue
                     if verbose:
-                        print(f" {value}")
+                        print(f" {value} -> {newvalue}")
+
+            # for key in default_params:
+            #     del params[key]
 
             # instantiate the block
             try:
                 if "blockargs" in params:
                     blockargs = params["blockargs"]
                     del params["blockargs"]
                 else:
                     blockargs = {}
 
-                # blockargs = blockargs or {}
+                blockargs = blockargs or {}
 
                 newblock = block_init(
                     name=block["title"], **params, **blockargs
                 )  # instantiate the block
 
-            except (ValueError, TypeError, NameError, SyntaxError):
+            except (
+                ValueError,
+                TypeError,
+                NameError,
+                SyntaxError,
+                AssertionError,
+                AttributeError,
+            ):
                 print(fg("red"))
                 print(f"bdload: error instantiating block [{block['title']}]")
-                args = ", ".join([f"{arg[0]}={arg[1]}" for arg in block["parameters"]])
+                args = ", ".join(
+                    [f"{arg[0]} = {arg[1]}" for arg in block["parameters"]]
+                )
                 print(f"  {block['block_type']}({args})")
                 print(attr(0))
                 raise RuntimeError(
-                    f"cannot instantiate block {block['title']} - bad parameters?"
+                    f"cannot instantiate block [{block['title']}] - bad parameters?"
                 )
 
             block_dict[block["id"]] = newblock  # add to mapping
             for output in block["outputs"]:
                 # each output id is mapped to the output Plug
                 output_dict[output["id"]] = newblock[output["index"]]
 
@@ -191,26 +216,27 @@
                 print(start, " --> ", end)
             bd.connect(start, end)
 
     return bd
 
 
 def bdrun(filename=None, globals={}, **kwargs):
-
     if filename is None:
-        filename = sys.argv[1]
+        if len(sys.argv) > 1:
+            filename = sys.argv[1]
+        else:
+            print("Usage:\n  bdrun file.bd <bdsim args>")
+            return
 
     sim = BDSim(**kwargs)  # create simulator
     bd = sim.blockdiagram()  # create diagram
 
     bd = bdload(bd, filename=filename, globalvars=globals, **kwargs)
     bd.compile()
     bd.report()
 
-    T = 10.0
-    qout = sim.run(bd, 5, dt=0.02)  # simulate for 5s
-    # sim.done(bd, block=True)
+    out = sim.run(bd)  # simulate
     print("bdrun exiting")
 
 
 if __name__ == "__main__":
     bdrun()
```

### Comparing `bdsim-1.0.0/bdsim/blockdiagram.py` & `bdsim-1.1.0/bdsim/blockdiagram.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,29 @@
 import importlib
 import inspect
 import traceback
 from collections import Counter, namedtuple
 from copy import deepcopy
 import numpy as np
 from colored import fg, attr
+import warnings
 
 
 from ansitable import ANSITable, Column
 
 from bdsim.components import *
 
+# from stubs import BlockDiagramMixin
 
 # ------------------------------------------------------------------------- #
 
 
+# class BlockDiagram(BlockDiagramMixin):
 class BlockDiagram:
-    """
+    r"""
     Block diagram class.  This object is the parent of all blocks and wires in
     the system.
 
     :ivar wirelist: all wires in the diagram
     :vartype wirelist: list of Wire instances
     :ivar blocklist: all blocks in the diagram
     :vartype blocklist: list of Block subclass instances
@@ -40,18 +43,24 @@
     :vartype compiled: bool
     :ivar blockcounter: unique counter for each block type
     :vartype blockcounter: collections.Counter
     :ivar blockdict: index of all blocks by category
     :vartype blockdict: dict of lists
     :ivar name: name of this diagram
     :vartype name: str
+
+    This object:
+
+    * holds all the blocks and wires that comprise the system
+    * manages continuous- and discrete-time state vector for the whole system, splitting
+      it across blocks as required
+    * evaluates the entire diagram as a function to compute :meth:`\dot{x} = f(x, t)`
     """
 
     def __init__(self, name="main", **kwargs):
-
         self.wirelist = []  # list of all wires
         self.blocklist = []  # list of all blocks
         self.clocklist = []  # list of all clock sources
         self.compiled = False  # network has been compiled
         self.blockcounter = Counter()
         self.name = name
         self.nstates = 0
@@ -59,17 +68,25 @@
         self._issubsystem = False
         self.blocknames = {}
         self.options = None
         self.n_auto_sum = 0
         self.n_auto_prod = 0
         self.n_auto_const = 0
         self.n_auto_gain = 0
+        self.n_auto_pow = 0
 
-    def __getitem__(self, b):
-        return self.blocknames[b]
+    def __getitem__(self, id):
+        print(id)
+        if isinstance(id, str):
+            return self.blocknames[id]
+        else:
+            for b in self.blocklist:
+                if b.id == id:
+                    return b
+            raise ValueError(f"block {id} not found")
 
     def __len__(self):
         return len(self.blocklist)
 
     def __deepcopy__(self, memo):
         # deep copy a block diagram
         # retain references (don't copy) to blocks and the runtime
@@ -134,33 +151,32 @@
         # return s.lstrip("\n")
 
     def ls(self):
         for k, v in self.blockdict.items():
             print("{:12s}: ".format(k), ", ".join(v))
 
     def connect(self, start, *ends, name=None):
-
         """
         TODO:
             s.connect(out[3], in1[2], in2[3])  # one to many
             block[1] = SigGen()  # use setitem
             block[1] = SumJunction(block2[3], block3[4]) * Gain(value=2)
         """
 
         # start.type = 'start'
 
         for end in ends:
-
             if isinstance(start, Block):
                 if isinstance(end, Block):
                     # connect(X, Y)
                     # wires from all outport to all inports
-                    assert (
-                        start.nout == end.nin
-                    ), "can only connect blocks where number of input and output ports match"
+                    assert start.nout == end.nin, (
+                        "can only connect blocks where number of input and output ports"
+                        " match"
+                    )
                     for i in range(start.nout):
                         wire = Wire(StartPlug(start, i), EndPlug(end, i), name)
                         self.add_wire(wire)
 
                 elif isinstance(end, Plug) and not end.isslice:
                     # connect(X, Y[i])
                     assert (
@@ -168,27 +184,27 @@
                     ), "can only connect single output block to a port"
                     end.type = "end"
                     wire = Wire(StartPlug(start, 0), end, name)
                     self.add_wire(wire)
 
                 elif isinstance(end, Plug) and end.isslice:
                     # connect(X, Y[m:n])
-                    assert (
-                        start.nout == end.width
-                    ), "can only connect single output block to an input port slice of width 1"
+                    assert start.nout == end.width, (
+                        "can only connect single output block to an input port slice of"
+                        " width 1"
+                    )
                     end.type = "end"
                     for i in range(start.nout):
                         wire = Wire(StartPlug(start, i), end[i], name)
                         self.add_wire(wire)
 
                 else:
                     raise ValueError("bad end type")
 
             elif isinstance(start, Plug) and not start.isslice:
-
                 if isinstance(end, Block):
                     # connect(X[i], Y)
                     # wires from all outport to all inports
                     assert (
                         end.nin == 1
                     ), "can only connect a port to a block with single input port"
                     wire = Wire(start, EndPlug(end, 0), name)
@@ -209,20 +225,20 @@
                     wire = Wire(start, end[0], name)
                     self.add_wire(wire)
 
                 else:
                     raise ValueError("bad end type")
 
             elif isinstance(start, Plug) and start.isslice:
-
                 if isinstance(end, Block):
                     # connect(X[i:j], Y)
-                    assert (
-                        start.width == end.nin
-                    ), "can only connect output slice to a block with matching number of input ports"
+                    assert start.width == end.nin, (
+                        "can only connect output slice to a block with matching number"
+                        " of input ports"
+                    )
                     for i in range(end.nin):
                         wire = Wire(start[i], EndPlug(end, i), name)
                         self.add_wire(wire)
 
                 elif isinstance(end, Plug) and not end.isslice:
                     # connect(X[i:j], Y[m])
                     assert (
@@ -292,15 +308,17 @@
 
         # process all subsystem imports
         # ssblocks = [b for b in self.blocklist if b.type == 'subsystem']
         # for b in ssblocks:
         #     print('  importing subsystem', b.name)
         #     if b.ssvar is not None:
         #         print('-- Wiring in subsystem', b, 'from module local variable ', b.ssvar)
-        self.blocklist, self.wirelist = self._subsystem_import(self, None)
+        self.blocklist, self.wirelist = self._subsystem_import(
+            self, None, verbose=verbose
+        )
 
         # check that wires all point to valid blocks
         for w in self.wirelist:
             if w.start.block not in self.blocklist:
                 raise RuntimeError(
                     f"wire {w} starts at unreferenced block {w.start.block}"
                 )
@@ -311,16 +329,15 @@
         for b in self.blocklist:
             try:
                 b.check()
             except:
                 raise RuntimeError("block failed check " + str(b))
 
         # build a dictionary of all block names
-        for b in self.blocklist:
-            self.blocknames[b.name] = b
+        self.blocknames = {b.name: b for b in self.blocklist}
 
         # visit all stateful blocks
         for b in self.blocklist:
             if b.blockclass == "transfer":
                 self.nstates += b.nstates
                 if b._state_names is not None:
                     assert (
@@ -427,30 +444,30 @@
                     error = True
 
         if error:
             if not subsystem:
                 raise RuntimeError("could not compile system")
 
         # create the execution plan/schedule
-        self.execution_plan()
+        self.schedule_generate()
 
         ## evaluate the network once to check out wire types
         x = self.getstate0()
 
         for clock in self.clocklist:
             clock._x = clock.getstate0()
 
         if report:
             self.report()
-            self.plan_print()
+            self.schedule_report()
 
         if not subsystem and evaluate:
             # run all the blocks for one step
             try:
-                self.evaluate_plan(x, 0.0, sinks=False)
+                self.schedule_evaluate(x, 0.0, sinks=False)
             except RuntimeError as err:
                 print("\nFrom compile: unrecoverable error in value propagation:", err)
                 traceback.print_exc(file=sys.stderr)
                 error = True
 
         if error:
             # show report if there was an error
@@ -459,28 +476,29 @@
             if not subsystem:
                 raise RuntimeError("could not compile system")
         else:
             self.compiled = True
 
         return self.compiled
 
-    def _subsystem_import(self, bd, sspath):
-
+    def _subsystem_import(self, bd, sspath, verbose=False):
         blocks = []
         wires = bd.wirelist
 
         for b in bd.blocklist:
             # rename the block to include subsystem path
             if sspath is not None:
                 b.name = sspath + "/" + b.name
 
             if b.type == "subsystem":
                 # deal with a subsystem
                 #  - recurse to import it
                 #  - add its blocks and wires to the set
+                if verbose:
+                    print("instantiating subsystem ", b.name)
                 ssb, ssw = self._subsystem_import(b.subsystem, b.name)
                 blocks.extend(ssb)
                 wires.extend(ssw)
 
                 # INPORT/OUTPORT blocks now become simple pass throughs
                 # same number of inputs and outputs
                 b.inport.nin = b.inport.nout
@@ -507,40 +525,43 @@
             b.id = i
         for i, w in enumerate(wires):
             w.id = i
         return blocks, wires
 
     # ---------------------------------------------------------------------- #
 
-    def evaluate_plan(self, x, t, checkfinite=True, debuglist=[], sinks=True):
+    def schedule_evaluate(self, x, t, checkfinite=True, sinks=True, simstate=None):
         """
         Evaluate all blocks in the network
 
-        :param x: state :type x: numpy.ndarray :param t: current time :type t:
-        float :param checkfinite: check for Inf or Nan values in block outputs
-        :type checkfinite: bool :return: state derivative :rtype: numpy.ndarray
+        :param x: state
+        :type x: ndarray
+        :param t: current time
+        :type t: float
+        :param checkfinite: check for Inf or Nan values in block outputs
+        :type checkfinite: bool
+        :param sinks: evaluate sink blocks, defaults to Trye
+        :type sinks: bool, optional
+        :param simstate: simulation state
+        :return: state derivative
+        :rtype: numpy.ndarray
 
         Performs the following steps:
 
         1. Partition the state vector ``x`` to all stateful blocks
         2. Execute the blocks in the order given by the ``plan``. The block
            outputs are "sent" to their connected inputs.
 
         Sink blocks are not executed here, but after completion their inputs
         will all be valid.
         """
 
         # TODO: don't copy outputs to inputs of next block, have inputs
         # pull the value from connected inputs
 
-        try:
-            self.state.t = t
-        except:
-            pass
-
         self.runtime.DEBUG("state", ">>>>>>>>> t={}, x={} >>>>>>>>>>>>>>>>", t, x)
 
         # reset all the blocks ready for the evalation
         self.reset()
 
         # split the state vector to stateful blocks
         for b in self.blocklist:
@@ -550,32 +571,35 @@
         # split the discrete state vector to clocked blocks
         for clock in self.clocklist:
             clock.setstate()
 
         self.runtime.DEBUG("propagate", "t={:.3f}", t)
 
         for sequence, group in enumerate(self.plan):
-
             # self.runtime.DEBUG('propagate', '---- sequence = ', sequence)
 
             for b in group:
                 # ask the block for output, check for errors
                 try:
-                    out = b.output(t)
+                    if sequence == 0:
+                        # blocks called at step 0 have no inputs
+                        out = b.output(t, None, b._x)
+                    else:
+                        out = b.output(t, b.inputs, b._x)
                 except Exception as err:
                     # output method failed, report it
                     print(fg("red"))
                     print(
                         "--Error at t={:f} when computing output of [{:s}::{:s}]".format(
                             t, b.type, str(b)
                         )
                     )
                     print()
                     # print('  {}'.format(err))
-                    traceback.print_exc(limit=-1, file=sys.stderr)
+                    traceback.print_exc(file=sys.stderr)
 
                     print()
                     for i, input in enumerate(b.inputs):
                         print(f"Input[{i}] = {input}")
 
                     if b.nstates > 0:
                         print(f"Block state x = {b._x}")
@@ -587,15 +611,16 @@
                 # check that output is a list of correct length
                 if not isinstance(out, (tuple, list)):
                     raise AssertionError(
                         f"block {b} output {b} must be a list: {type(out)}"
                     )
                 if len(out) != b.nout:
                     raise AssertionError(
-                        f"block {b} output {b} has incorrect length: {len(out)} instead of {b.nout}"
+                        f"block {b} output {b} has incorrect length: {len(out)} instead"
+                        f" of {b.nout}"
                     )
 
                 # TODO check output validity once at the startq
 
                 # check it has no nan or inf values
                 if (
                     checkfinite
@@ -614,21 +639,26 @@
                 #         # send value to wire
                 #         w.send(value)
 
                 #         # TODO send return status no longer needed
                 #         # TODO use common error handler in all cases above
                 b.output_values = out
 
+        if sinks:
+            for b in self.blocklist:
+                if isinstance(b, SinkBlock):
+                    b.step(t, b.inputs)
+
         # gather the derivative
-        YD = self.deriv()
+        YD = self.deriv(t)
 
         self.runtime.DEBUG("deriv", YD)
         return YD
 
-    def execution_plan(self):
+    def schedule_generate(self):
         """
         Create execution plan
 
         The plan is saved in the attribute ``plan`` and is a list
         ``[L0, L1, ... LN]`` where each ``Li`` is a list of blocks.  The blocks
         in the lists are executed sequentially, ie. all the blocks in ``L0``
         then all the blocks in ``L1`` etc.
@@ -640,15 +670,15 @@
             - The plan is essentially a dataflow graph.
             - The blocks in list ``Li`` could potentially be executed in
               parallel.
             - Constant blocks and stateful blocks are all executed in ``L0``
             - The block attribute ``_sequence`` is ``i`` and indicates its
               execution order
 
-        :seealso: :func:`plan_print`, :func:`plan_dotfile`
+        :seealso: :func:`schedule_report`, :func:`schedule_dotfile`
         """
 
         plan = []
         group = []
         for b in self.blocklist:
             b._sequence = None
             if b.blockclass in ("source", "transfer", "clocked"):
@@ -678,45 +708,28 @@
             if len(group) == 0:
                 break
             plan.append(group)
             sequence += 1
 
         self.plan = plan
 
-    def plan_print(self):
-        """
-        Display execution plan in tabular form
-
-        :seealso: :func:`execution_plan`, :func:`plan_dotfile`
-        """
-        table = ANSITable(
-            Column("Sequence"),
-            Column("Blocks", colalign="<", headalign="^"),
-            border="thin",
-        )
-
-        for sequence, group in enumerate(self.plan):
-            table.row(sequence, ", ".join([str(b) for b in group]))
-
-        table.print()
-
-    def plan_dotfile(self, filename):
+    def schedule_dotfile(self, filename):
         """
         Write a GraphViz dot file representing the execution schedule
 
         :param file: Name of file to write to
         :type file: str
 
         The file can be processed using neato or dot::
 
             % dot -Tpng -o out.png dotfile.dot
 
         Display execution plan as a dataflow graph.
 
-        :seealso: :func:`execution_plan`, :func:`plan_print`
+        :seealso: :func:`schedule_plan`, :func:`schedule_print`
         """
 
         if isinstance(filename, str):
             file = open(filename, "w")
         else:
             file = filename
 
@@ -744,119 +757,182 @@
                 for p in b._parents:
                     file.write('\t"{:s}" -> "{:s}"\n'.format(p.name, b.name))
 
         file.write("}\n")
 
     # ---------------------------------------------------------------------- #
 
-    def _debugger(self, state=None, integrator=None):
-
-        if state.t_stop is not None and state.t < state.t_stop:
+    def _debugger(self, simstate=None, integrator=None):
+        if simstate.t_stop is not None and simstate.t < simstate.t_stop:
             return
-
-        state.t_stop = None
+        
+        def print_output(b, t, inports, x):
+            out = b.output(t, inports, x)
+            if len(out) == 1:
+                print(f"{b.name} = {out[0]}")
+            else:
+                print(f"{b.name}:")
+                for i, o in enumerate(out):
+                    print(f"  [{i}] = {o}")
+
+        np.set_printoptions(precision=6, linewidth=120)
+        simstate.t_stop = None
+        if not hasattr(self, "debug_watch"):
+            self.debug_watch = None
         print("\n")
-        while True:
-            cmd = input(f"(bdsim, t={state.t:.4f}) ")
+        if self.debug_watch is not None:
+            t = simstate.t
+            for b in self.debug_watch:
+                print_output(b, t, b.inputs, b._x)
 
-            if len(cmd) == 0:
-                continue
+        while True:
+            try:
+                t = simstate.t
+                cmd = input(f"(bdsim, t={t:.6f}) ")
 
-            if cmd[0] == "p":
-                # print variables
-                if len(cmd) > 1:
-                    id = int(cmd[1:])
-                    b = self.blocklist[id]
-                    print(b.name, b.output(t=state.t))
-                else:
-                    for b in self.blocklist:
-                        if b.nout > 0:
-                            print(b.name, b.output(t=state.t))
-            elif cmd[0] == "i":
-                print(integrator.status, integrator.step_size, integrator.nfev)
-            elif cmd[0] == "s":
-                # step
-                break
-            elif cmd[0] == "c":
-                # continue
-                self.debug_stop = False
-                self.t_stop = None
-                break
-            elif cmd[0] == "t":
-                self.t_stop = float(cmd[1:])
-                break
-            elif cmd[0] == "q":
-                sys.exit(1)
-            elif cmd[0] in "h?":
-                print("p    print all outputs")
-                print("pI   print block id I output")
-                print("i    print integrator status")
-                print("s    single step")
-                print("c    continue")
-                print("tT   stop at or after time T")
-                print("q    quit")
+                if len(cmd) == 0:
+                    continue
 
+                if cmd[0] == "p":
+                    # print variables
+                    if len(cmd) > 1:
+                        id = int(cmd[1:])
+                        b = self.blocklist[id]
+                        print_output(b, t, b.inputs, b._x)
+                    else:
+                        for b in self.blocklist:
+                            if b.nout > 0:
+                                print_output(b, t, b.inputs, b._x)
+                elif cmd[0] == "i":
+                    print(f"status={integrator.status}, dt={integrator.step_size:.4g}, nfev={integrator.nfev}")
+                elif cmd[0] == "s":
+                    # step
+                    break
+                elif cmd[0] == "c":
+                    # continue
+                    self.debug_stop = False
+                    self.t_stop = None
+                    break
+                elif cmd[0] == "t":
+                    self.t_stop = float(cmd[1:])
+                    break
+                elif cmd[0] == "q":
+                    sys.exit(1)
+                elif cmd[0] == "r":
+                    self.report()
+                elif cmd[0] == "w":
+                    if len(cmd) == 1:
+                        # clear the watch list
+                        print(self.debug_watch)
+                        self.debug_watch = None
+                    else:
+                        self.debug_watch = [self.blocklist[int(s.strip())] for s in cmd[2:].split(" ")]
+                elif cmd == "pdb":
+                    import pdb
+
+                    pdb.runeval('print("type exit to leave Pdb")')
+                elif cmd[0] in "h?":
+                    print("p    print all outputs")
+                    print("pI   print block id I output")
+                    print("i    print integrator status")
+                    print("s    single step")
+                    print("c    continue")
+                    print("tT   stop at or after time T")
+                    print("r    print block and wires")
+                    print("pdb  enter PDB debugger")
+                    print("w id watch list, display at every step")
+                    print("q    quit")
+
+            except (IndexError, ValueError, TypeError):
+                print("??")
+                pass
     # ---------------------------------------------------------------------- #
 
-    def report_summary(self):
+    def report_summary(self, sortby="name", **kwargs):
         """
         Print a summary of block diagram.
 
+        :param sortby: sort rows by specified block attribute: "name" [default] or "type"
+        :type sortby: str, optional
+        :param style: table style, one of: ansi (default), markdown, latex
+        :type style: str
+
         Print a table with 4 columns:
 
         1. Block name, sorted in alphabetical order
         2. The input port (if not a source block)
         3. The block driving this port (if not a source block)
         4. The type of value driving this port (if not a source block)
 
         If the block is an event source, add a ``@`` suffix.
         """
+
         table = ANSITable(
             Column("block", headalign="^", colalign="<"),
+            Column("type", headalign="^", colalign="<"),
             Column("inport", headalign="^", colalign="<"),
             Column("source", headalign="^", colalign="<"),
             Column("source type", headalign="^", colalign="<"),
             border="thin",
         )
 
+        if sortby == "name":
+            sortfunc = lambda x: x.name
+        elif sortby == "type":
+            sortfunc = lambda x: x.type
+
         first = True
         legend = None
-        for b in sorted(self.blocklist, key=lambda x: x.name):
+        for b in sorted(self.blocklist, key=sortfunc):
             name = str(b)
             if isinstance(b, EventSource):
                 name += "@"
                 legend = "Note: @ = event source"
             # add a divider before each subsequent row
             if not first:
                 table.rule()
             else:
                 first = False
 
             # print the details
             if len(b.sources) > 0:
                 # non source block, list all its inputs, one per row
-                for (port, source) in enumerate(b.sources):  # every port
-
-                    value = b.input(port)
+                inputs = b.inputs
+                for port, source in enumerate(b.sources):  # every port
+                    value = inputs[port]
                     typ = type(value).__name__
                     if isinstance(value, np.ndarray):
                         typ += "{:s}.{:s}".format(str(value.shape), str(value.dtype))
-
-                    table.row(name if port == 0 else "", port, source.block.name, typ)
+                    src_name = source.block.name
+                    if source.block.nout > 1:
+                        src_name += f"[{source.port}]"
+                    if port == 0:
+                        # first row for this block
+                        table.row(name, b.type, port, src_name, typ)
+                    else:
+                        # subsequent rows
+                        table.row("", "", port, src_name, typ)
             else:
                 # source block, just list the name
-                table.row(name, "", "", "")
-        table.print()
+                table.row(name, b.type, "", "", "")
+        table.print(**kwargs)
+
         if legend:
             print(legend + "\n")
 
-    def report(self):
+    def report(self, **kwargs):
+        warnings.warn("use reports_lists() method instead", DeprecationWarning)
+        self.report_lists(**kwargs)
+
+    def report_lists(self, **kwargs):
         """
         Print a tabular report about the block diagram.
 
+        :param kwargs: options passed to :meth:`ansitable.ANSITable.print`
+
         Print the important lists in pretty format.
 
         * block list, all blocks
         * wire list, all wires
         * clock list, all discrete time clocks
 
         """
@@ -870,15 +946,15 @@
             Column("nstate"),
             Column("ndstate"),
             Column("type", headalign="^", colalign="<"),
             border="thin",
         )
         for b in self.blocklist:
             table.row(b.id, str(b), b.nin, b.nout, b.nstates, b.ndstates, b.type)
-        table.print()
+        table.print(**kwargs)
 
         # print all the wires
         print("\nWires::\n")
         table = ANSITable(
             Column("id"),
             Column("from", headalign="^"),
             Column("to", headalign="^"),
@@ -894,15 +970,15 @@
                 value = w.end.block.inputs[w.end.port]
                 typ = type(value).__name__
                 if isinstance(value, np.ndarray):
                     typ += "{:s}.{:s}".format(str(value.shape), str(value.dtype))
             except:
                 typ = "??"
             table.row(w.id, start, end, w.fullname, typ)
-        table.print()
+        table.print(**kwargs)
 
         if len(self.clocklist) > 0:
             # print all the clocked blocks
             print("\nClocked blocks::\n")
             table = ANSITable(
                 Column("id"),
                 Column("block"),
@@ -911,47 +987,62 @@
                 Column("offset"),
                 border="thin",
             )
             for b in self.blocklist:
                 if b.blockclass == "clocked":
                     c = b.clock
                     table.row(b.id, str(b), c.name, c.T, c.offset)
-            table.print()
-
-        print("\nContinuous state variables: {:d}".format(self.nstates))
-        print("Discrete state variables:   {:d}".format(self.ndstates))
+            table.print(**kwargs)
 
         if not self.compiled:
             print("** System has not been compiled, or had a compile time error")
 
+    def report_schedule(self, **kwargs):
+        """
+        Display execution schedule in tabular form
+
+        :param kwargs: options passed to :meth:`ansitable.ANSITable.print`
+
+        :seealso: :func:`schedule_plan`, :func:`schedule_dotfile`
+        """
+        table = ANSITable(
+            Column("Step"),
+            Column("Blocks", colalign="<", headalign="^"),
+            border="thin",
+        )
+
+        for sequence, group in enumerate(self.plan):
+            table.row(sequence, ", ".join([str(b) for b in group]))
+
+        table.print(**kwargs)
+
     # ---------------------------------------------------------------------- #
 
     def _error_handler(self, where, block):
         # called from except clause
 
         import traceback
         import types
 
         t, v, tb = sys.exc_info()  # get the exception
 
         print(fg("red"))  # red text
 
         # print the traceback
-        print(
-            f"[{where}]: exception {t.__name__} occurred in {block.type} block {block.name}  "
-        )
+        print(f"[{block.type} block: {block.name}.{where}]: exception {t.__name__}")
         print(f"  {v}\n")
         traceback.print_tb(tb)
 
         # print all block inputs
         print()
         for i in range(block.nin):
             input = block.inputs[i]
             print(
-                f"input {i} from {block.sources[i].block.name} [{input.__class__.__name__}]"
+                f"input {i} from"
+                f" {block.sources[i].block.name} [{input.__class__.__name__}]"
             )
             print("  ", input)
 
         print(attr(0))  # default text
 
         # traceback = err[2]
         # back_frame = traceback.tb_frame.f_back
@@ -985,102 +1076,103 @@
         """
         for b in self.blocklist:
             try:
                 b.reset()
             except:
                 self._error_handler("reset", b)
 
-    def step(self, state=None):
+    def step(self, t):
         """
         Step all blocks
 
-        :param state: simulation state, defaults to None
-        :type state: SimState, optional
-        :param graphics: graphics enabled, defaults to False
-        :type graphics: bool, optional
+        :param t: simulation time, defaults to None
+        :type t: float
+        :param inports: block input port values
+        :type inports: list
 
         Tell all blocks to take action on new inputs by invoking their
         ``step`` method and passing the ``state`` object.  Used to save
         results to a figure or file.
 
         Called at the end of every integration interval.
 
         .. note::
             - if ``graphics`` is False, Graphics blocks are not called
         """
 
         # TODO could be done by output method, even if no outputs
 
         for b in self.blocklist:
-            if b.isgraphics and not state.options.graphics:
-                continue  # skip graphics blocks
             try:
-                b.step(state=state)
+                if isinstance(b, SinkBlock):
+                    b.step(t, b.inputs)
             except:
                 self._error_handler("step", b)
 
-    def deriv(self):
+    def deriv(self, t):
         """
-        Harvest derivatives from all blocks .
+        Harvest derivatives from all blocks.
+
+        :param t: simulation time, defaults to None
+        :type t: float
+        :param simstate: simulation state, defaults to None
+        :type simstate: SimState, optional
         """
         YD = np.array([])
         for b in self.blocklist:
             if b.blockclass == "transfer":
                 try:
-                    yd = b.deriv().flatten()
+                    yd = b.deriv(t, b.inputs, b._x)
                     if not isinstance(yd, np.ndarray):
                         raise AssertionError(f"deriv: block {b} did not return ndarray")
                     if yd.ndim != 1 or yd.shape[0] != b.nstates:
                         raise AssertionError(
-                            f"deriv: block {b} returns wrong shape {yd.shape}, should be ({b.nstates},)"
+                            f"deriv: block {b} returns wrong shape {yd.shape}, should"
+                            f" be ({b.nstates},)"
                         )
                     YD = np.r_[YD, yd]
                 except:
                     self._error_handler("deriv", b)
         return YD
 
-    def start(self, graphics=False, state=None, **kwargs):
+    def start(self, simstate=None):
         """
         Start all blocks
 
-        :param state: simulation state, defaults to None
-        :type state: SimState, optional
-        :param graphics: graphics enabled, defaults to False
-        :type graphics: bool, optional
+        :param simstate: simulation state, defaults to None
+        :type simstate: SimState, optional
 
         Inform all blocks that BlockDiagram execution is about to start by
         invoking their ``start`` method and passing the ``state`` object.  Used
         to open files, create figures etc.
 
         .. note:: if ``graphics`` is False, Graphics blocks are not called
 
         """
 
         for c in self.clocklist:
             try:
-                c.start(state=state, **kwargs)
+                c.start(simstate)
             except:
-                self._error_handler("start clock", c)
+                self._error_handler("start_clocked", c)
 
         # safe wrapper for block starting, does error handling
         for b in self.blocklist:
-            if b.isgraphics and not graphics:
-                continue
             # print('starting block', b)
             try:
-                b.start(state=state, **kwargs)
+                b.start(simstate)
             except:
-                self._error_handler("block.start", b)
+                self._error_handler("start", b)
 
     def initialstate(self):
         for b in self.blocklist:
             if b.blockclass in ("transfer", "clocked"):
                 b._x = b._x0
 
-    def done(self, block=False, graphics=False):
+    def done(self, block=False):
         """
         Finishup all blocks
 
         :param state: simulation state, defaults to None
         :type state: SimState, optional
         :param graphics: graphics enabled, defaults to False
         :type graphics: bool, optional
@@ -1088,96 +1180,140 @@
         Inform all blocks that BlockDiagram execution is complete by invoking their
         ``done`` method and passing options.  Used
         to close files, display figures etc.
 
         .. note:: if ``graphics`` is False, Graphics blocks are not called
         """
         for b in self.blocklist:
-            if b.isgraphics and not graphics:
-                continue
             try:
                 b.done(block=block)
             except:
-                self._error_handler("block.done", b)
+                self._error_handler("done", b)
 
-    def dotfile(self, filename):
+    def dotfile(self, filename, shapes=None):
         """
         Write a GraphViz dot file representing the network.
 
-        :param file: Name of file to write to
-        :type file: str
+        :param file: Name of file to write to, or file handle
+        :type file: str, file handle
+        :param shapes: block shapes
+        :type shapes: dict
+
+        Create a GraphViz format file for procesing by ``dot``.  The graph is:
+
+        * directed graph, drawn left to right
+        * source blocks are in the first column
+        * sink and graphics blocks are in the last column
+        * ``SUM`` and ``PROD`` blocks have the sign or operation of their input wires
+          labeled.
 
-        The file can be processed using neato or dot::
+        The file can be processed using ``dot``::
 
             % dot -Tpng -o out.png dotfile.dot
 
+        .. image:: ../../figs/eg1.png
+            :width: 600
+            :alt: Block diagram represented as a mathematical graph
+
+        .. note:: By default all blocks have the default shape, with source blocks shown
+            as a rectangle ("record"), and sink/graphics blocks as a rounded rectangle
+            ("Mrecord").  This can be overriden by provide a dictionary ``shapes`` that
+            maps block class (sink, source, graphics, function, transfer) to the names
+            of GraphViz shapes.
+
+        :seealso: :meth:`showgraph`
         """
+        if shapes is None:
+            shapes = dict(source="record", sink="Mrecord", graphics="Mrecord")
 
         if isinstance(filename, str):
             file = open(filename, "w")
         else:
             file = filename
 
         header = r"""digraph G {
+    rankdir = "LR"
 
-    graph [splines=ortho, rankdir=LR]
-    node [shape=box]
-    
-    """
+"""
         file.write(header)
         # add the blocks
         for b in self.blocklist:
             options = []
+            if b.blockclass in shapes:
+                options.append("shape={:s}".format(shapes[b.blockclass]))
             if b.blockclass == "source":
-                options.append("shape=box3d")
-            elif b.blockclass == "sink":
-                options.append("shape=folder")
-            elif b.blockclass == "function":
-                if b.type == "gain":
-                    options.append("shape=triangle")
-                    options.append("orientation=-90")
-                    options.append('label="{:g}"'.format(b.gain))
-                elif b.type == "sum":
-                    options.append("shape=point")
-            elif b.blockclass == "transfer":
-                options.append("shape=component")
+                options.append('rank="source"')
+            if b.blockclass in ("sink", "graphics"):
+                options.append('rank="sink"')
             if b.pos is not None:
                 options.append('pos="{:g},{:g}!"'.format(b.pos[0], b.pos[1]))
-            options.append(
-                'xlabel=<<BR/><FONT POINT-SIZE="8" COLOR="blue">{:s}</FONT>>'.format(
-                    b.type
-                )
-            )
-            file.write('\t"{:s}" [{:s}]\n'.format(b.name, ", ".join(options)))
+            # options.append(
+            #     'xlabel=<<BR/><FONT POINT-SIZE="8" COLOR="blue">{:s}</FONT>>'.format(
+            #         b.type
+            #     )
+            # )
+            if len(options) > 0:
+                file.write('\t"{:s}" [{:s}]\n'.format(b.name, ", ".join(options)))
+        file.write("\n")
 
         # add the wires
         for w in self.wirelist:
             options = []
             # options.append('xlabel="{:s}"'.format(w.name))
             if w.end.block.type == "sum":
                 options.append(
                     'headlabel="{:s} "'.format(w.end.block.signs[w.end.port])
                 )
+                options.append("labeldistance=1.5")
+            if w.end.block.type == "prod":
+                options.append('headlabel="{:s} "'.format(w.end.block.ops[w.end.port]))
+                options.append("labeldistance=1.5")
             file.write(
                 '\t"{:s}" -> "{:s}" [{:s}]\n'.format(
                     w.start.block.name, w.end.block.name, ", ".join(options)
                 )
             )
 
         file.write("}\n")
 
-    def blockvalues(self):
+    def showgraph(self):
+        """
+        Display diagram as a graph in browser tab
+
+        :seealso: :meth:`dotfile`
+        """
+
+        # Lazy import
+        try:
+            import tempfile
+            import subprocess
+            import webbrowser
+        except ModuleNotFoundError:
+            return
+
+        # create the temporary dotfile
+        dotfile = tempfile.TemporaryFile(mode="w")
+        self.dotfile(dotfile)
+
+        # rewind the dot file, create PDF file in the filesystem, run dot
+        dotfile.seek(0)
+        pdffile = tempfile.NamedTemporaryFile(suffix=".pdf", delete=False)
+        subprocess.run("dot -Tpdf", shell=True, stdin=dotfile, stdout=pdffile)
+
+        # open the PDF file in browser (hopefully portable), then cleanup
+        webbrowser.open(f"file://{pdffile.name}")
+
+    def blockvalues(self, t=None, simstate=None):
         for b in self.blocklist:
             print("Block {:s}:".format(b.name))
             print("  inputs:  ", b.inputs)
-            print("  outputs: ", b.output(t=0))
+            print("  outputs: ", b.output(t, b.inputs, b._x))
 
 
 if __name__ == "__main__":  # pragma: no cover
-
     import bdsim
 
     bd = bdsim.BlockDiagram()
 
     # define the blocks
     demand = bd.STEP(T=1, pos=(0, 0), name="demand")
     sum = bd.SUM("+-", pos=(1, 0))
```

### Comparing `bdsim-1.0.0/bdsim/blocks/connections.py` & `bdsim-1.1.0/bdsim/blocks/connections.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,343 +23,383 @@
 
 # ------------------------------------------------------------------------ #
 class Item(FunctionBlock):
 
     """
     :blockname:`ITEM`
 
-    .. table::
-       :align: left
+    Select item from a dictionary signal.
 
-    +------------+---------+---------+
-    | inputs     | outputs |  states |
-    +------------+---------+---------+
-    | 1          | 1       | 0       |
-    +------------+---------+---------+
-    | dict       | any     |         |
-    +------------+---------+---------+
+    :inputs: 1
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - 0
+            - dict
+            - ``D``
+        *   - Output
+            - 0
+            - any
+            - ``D[i]``
+
+    For a dictionary type input signal, select one item as the output signal.
+    For example::
+
+        item = bd.ITEM("xd")
+
+    selects the ``xd`` item from the dictionary signal input to the block.
+
+    This is somewhat like a demultiplexer :class:`DeMux` but allows for
+    named heterogeneous data.
+    A dictionary signal can serve a similar purpose to a "bus" in Simulink(R).
+
+    :seealso: :class:`Dict`
     """
 
     nin = 1
     nout = 1
 
     def __init__(self, item, **blockargs):
         """
-        Selector item from a dictionary signal.
-
         :param item: name of dictionary item
         :type item: str
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: An ITEM block
-        :rtype: Item instance
-
-        For a dictionary type input signal, select one item as the output signal.
-        For example::
-
-            ITEM('xd')
-
-        selects the ``xd`` item from the dictionary signal input to the block.
-
-        A dictionary signal can serve a similar purpose to a "bus" in Simulink(R).
-
-        This is somewhat like a demultiplexer :class:`DeMux` but allows for
-        named heterogeneous data.
-
-        :seealso: :class:`Dict`
         """
 
         super().__init__(**blockargs)
         self.item = item
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
+        input = inports[0]
         # TODO, handle inputs that are vectors themselves
-        assert isinstance(self.inputs[0], dict), "Input signal must be a dict"
-        assert self.item in self.inputs[0], "Item is not in input dict"
-        return [self.inputs[0][self.item]]
+        assert isinstance(input, dict), "Input signal must be a dict"
+        assert self.item in input, "Item is not in input dict"
+        return [input[self.item]]
 
 
 class Dict(FunctionBlock):
 
     """
     :blockname:`DICT`
 
-    .. table::
-       :align: left
+    Create a dictionary signal.
+
+    :inputs: N
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - i
+            - any
+            - :math:`x_i`
+        *   - Output
+            - 0
+            - dict
+            - ``{key: x[i] for i, key in enumerate(keys)}``
+
+    Inputs are assigned to a dictionary signal, using the corresponding
+    names from ``keys``.
+    For example::
+
+        dd = bd.DICT(["x", "xd", "xdd"])
 
-    +------------+---------+---------+
-    | inputs     | outputs |  states |
-    +------------+---------+---------+
-    | N          | 1       | 0       |
-    +------------+---------+---------+
-    | any        | dict    |         |
-    +------------+---------+---------+
+    expects three inputs and assigns them to dictionary items ``x``, ``xd``, ``xdd`` of
+    the output dictionary respectively.
+
+    This is somewhat like a multiplexer :class:`Mux` but allows for named heterogeneous
+    data.  A dictionary signal can serve a similar purpose to a "bus" in Simulink(R).
+
+
+    :seealso: :class:`Item` :class:`Mux`
     """
 
     nin = 1
     nout = 1
 
-    def __init__(self, item, **blockargs):
+    def __init__(self, keys, **blockargs):
         """
-        Create a dictionary signal.
-
         :param keys: list of dictionary keys
         :type keys: list
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: A DICT block
-        :rtype: Dict instance
-
-        Inputs are assigned to a dictionary signal, using the corresponding
-        names from ``keys``.
-        For example::
-
-            DICT(['x', 'xd', 'xdd'])
-
-        expects three inputs and assigns them to dictionary items ``x``, ``xd``, ``xdd`` of
-        the output dictionary respectively.
-
-        A dictionary signal can serve a similar purpose to a "bus" in Simulink(R).
-
-        This is somewhat like a multiplexer :class:`Mux` but allows for
-        named heterogeneous data.
-
-        :seealso: :class:`Item` :class:`Mux`
         """
 
         super().__init__(**blockargs)
-        self.item = item
+        self.keys = keys
 
-    def output(self, t=None):
-        # TODO, handle inputs that are vectors themselves
-        assert isinstance(self.inputs[0], dict), "Input signal must be a dict"
-        assert self.item in self.inputs[0], "Item is not in signal dict"
-        return [self.inputs[0][self.item]]
+    def output(self, t, inports, x):
+        return {key: inports[i] for i, key in enumerate(self.keys)}
 
 
 # ------------------------------------------------------------------------ #
 class Mux(FunctionBlock):
     """
     :blockname:`MUX`
 
-    .. table::
-       :align: left
+    Multiplex signals.
+
+    :inputs: N
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - i
+            - float, ndarray
+            - :math:`x_i`
+        *   - Output
+            - 0
+            - ndarray
+            - :math:`[x_0 \ldots x_{N-1}]`
+
+    This block takes a number of scalar or 1D-array signals and concatenates
+    them into a single 1-D array signal.  For example::
+
+        mux = bd.MUX(2)
 
-    +------------+---------+---------+
-    | inputs     | outputs |  states |
-    +------------+---------+---------+
-    | nin        | 1       | 0       |
-    +------------+---------+---------+
-    | float,     | A(M,)   |         |
-    | A(N,)      | A(M,)   |         |
-    +------------+---------+---------+
+    :seealso: :class:`Demux` :class:`Dict`
     """
 
+    # TODO could be generalized to creating a list of non numeric data
+
     nin = -1
     nout = 1
 
     def __init__(self, nin=1, **blockargs):
         """
-        Multiplex signals.
-
         :param nin: Number of input ports, defaults to 1
         :type nin: int, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: A MUX block
-        :rtype: Mux instance
-
-        This block takes a number of scalar or 1D-array signals and concatenates
-        them into a single 1-D array signal.  For example::
-
-            MUX(2, inputs=(func1[2], sum3))
-
-        multiplexes the outputs of blocks ``func1`` (port 2) and ``sum3`` into a
-        single output vector as a 1D-array.
-
-        :seealso: :class:`Dict`
         """
         super().__init__(nin=nin, **blockargs)
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
         # TODO, handle inputs that are vectors themselves
         out = []
-        for input in self.inputs:
+        for input in inports:
             if isinstance(input, (int, float, bool)):
                 out.append(input)
             elif isinstance(input, np.ndarray):
                 out.extend(input.flatten().tolist())
         return [np.array(out)]
 
 
 # ------------------------------------------------------------------------ #
 class DeMux(FunctionBlock):
     """
     :blockname:`DEMUX`
 
-    .. table::
-       :align: left
+    Demultiplex signals.
 
-    +------------+---------+---------+
-    | inputs     | outputs |  states |
-    +------------+---------+---------+
-    | 1          | nout    | 0       |
-    +------------+---------+---------+
-    | float,     | float   |         |
-    | A(nout,)   |         |         |
-    +------------+---------+---------+
+    :inputs: 1
+    :outputs: N
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - 0
+            - iterable
+            - :math:`x`
+        *   - Output
+            - i
+            - any
+            - :math:`x_i`
+
+    This block has a single input port and ``nout`` output ports.  The input signal is
+    an iterable whose ``nout`` elements are routed element-wise to individual scalar
+    output ports.  If the input is a 1D Numpy array, then each output port is an
+    element of that array.
+
+    :seealso: :class:`Mux`
     """
 
     nin = 1
     nout = -1
 
     def __init__(self, nout=1, **blockargs):
         """
-        Demultiplex signals.
-
         :param nout: number of outputs, defaults to 1
         :type nout: int, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: A DEMUX block
-        :rtype: DeMux instance
-
-        This block has a single input port and ``nout`` output ports.  A 1D-array
-        input signal (with ``nout`` elements) is routed element-wise to individual
-        scalar output ports.
-
         """
         super().__init__(nout=nout, **blockargs)
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
+        input = inports[0]
         # TODO, handle inputs that are vectors themselves
         assert (
-            len(self.inputs[0]) == self.nout
+            len(input) == self.nout
         ), "Input width not equal to number of output ports"
-        return list(self.inputs[0])
+        return list(input)
 
 
 # ------------------------------------------------------------------------ #
 
 
 class Index(FunctionBlock):
     """
     :blockname:`INDEX`
 
-    .. table::
-       :align: left
+    :inputs: 1
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - i
+            - iterable
+            - :math:`x`
+        *   - Output
+            - j
+            - iterable
+            - :math:`x_i`
+
+    The specified element(s) of the input iterable (list, string, etc.)
+    are output.  The index can be an integer, sequence of integers, a Python slice
+    object, or a string with Python slice notation, eg. ``"::-1"``.
 
-    +------------+---------+---------+
-    | inputs     | outputs |  states |
-    +------------+---------+---------+
-    | 1          | 1       | 0       |
-    +------------+---------+---------+
-    | ndarray    | ndarray |         |
-    +------------+---------+---------+
+    :seealso: :class:`Slice1` :class:`Slice2`
     """
 
     nin = 1
     nout = 1
 
     def __init__(self, index=[], **blockargs):
         """
         Index an iterable signal.
 
         :param index: elements of input array, defaults to []
         :type index: list, slice or str, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: An INDEX block
-        :rtype: Index instance
-
-        The specified element(s) of the input iterable (list, string, etc.)
-        are output.  The index can be an integer, sequence of integers, a Python slice
-        object, or a string with Python slice notation, eg. ``"::-1"``.
-
-        :seealso: :class:`Slice1` :class:`Slice2`
         """
         super().__init__(**blockargs)
 
         if isinstance(index, str):
             args = [None if a == "" else int(a) for a in index.split(":")]
             self.index = slice(*args)
         self.index = index
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
+        input = inports[0]
         if len(self.index) == 1:
-            return [self.inputs[0][self.index[0]]]
+            return [input[self.index[0]]]
+        elif isinstance(input, np.ndarray):
+            return [np.array([input[i] for i in self.index])]
         else:
-            return [np.r_[[self.inputs[0][i] for i in self.index]]]
+            return [[input[i] for i in self.index]]
 
 
 # ------------------------------------------------------------------------ #
 
 
 class SubSystem(SubsystemBlock):
     """
     :blockname:`SUBSYSTEM`
 
-    .. table::
-       :align: left
+    Instantiate a subsystem.
+
+    :inputs: N
+    :outputs: M
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - i
+            - any
+            - :math:`x_i`
+        *   - Output
+            - j
+            - any
+            - :math:`y_j`
+
+    This block represents a subsystem in a block diagram.  The definition
+    of the subsystem can be:
+
+    - the name of a module which is imported and must contain only
+      only ``BlockDiagram`` instance, or
+    - a ``BlockDiagram`` instance
+
+    The referenced block diagram must contain one or both of:
+
+    - one ``InPort`` block, which has outputs but no inputs. These
+      outputs are connected to the inputs to the enclosing ``SubSystem`` block.
+    - one ``OutPort`` block, which has inputs but no outputs. These
+      inputs are connected to the outputs to the enclosing ``SubSystem`` block.
 
-    +------------+------------+---------+
-    | inputs     | outputs    |  states |
-    +------------+------------+---------+
-    | ss.in.nout | ss.out.nin | 0       |
-    +------------+------------+---------+
-    | any        | any        |         |
-    +------------+------------+---------+
+    .. note::
+
+        - The referenced block diagram is treated like a macro and copied into
+          the parent block diagram at compile time. The ``SubSystem``, ``InPort`` and
+          ``OutPort`` blocks are eliminated, that is, all hierarchical structure is
+          lost.
+        - The same subsystem can be used multiple times, its blocks and wires
+          will be cloned.  Subsystems can also include subsystems.
+        - The number of input and output ports is not specified, they are computed
+          from the number of ports on the ``InPort`` and ``OutPort`` blocks within the
+          subsystem.
     """
 
     nin = -1
     nout = -1
 
     def __init__(self, subsys, nin=1, nout=1, **blockargs):
         """
-        Instantiate a subsystem.
-
         :param subsys: Subsystem as either a filename or a ``BlockDiagram`` instance
         :type subsys: str or BlockDiagram
-
         :param nin: Number of input ports, defaults to 1
         :type nin: int, optional
         :param nout: Number of output ports, defaults to 1
         :type nout: int, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
         :raises ImportError: DESCRIPTION
         :raises ValueError: DESCRIPTION
-        :return: A SUBSYSTEM block
-        :rtype: SubSystem instance
-
-        This block represents a subsystem in a block diagram.  The definition
-        of the subsystem can be:
-
-            - the name of a module which is imported and must contain only
-              only ``BlockDiagram`` instance, or
-            - a ``BlockDiagram`` instance
-
-        The referenced block diagram must contain one or both of:
-
-            - one ``InPort`` block, which has outputs but no inputs. These
-              outputs are connected to the inputs to the enclosing ``SubSystem`` block.
-            - one ``OutPort`` block, which has inputs but no outputs. These
-              inputs are connected to the outputs to the enclosing ``SubSystem`` block.
-
-        .. note::
-
-        - The referenced block diagram is treated like a macro and copied into
-          the parent block diagram at compile time. The ``SubSystem``, ``InPort`` and
-          ``OutPort`` blocks are eliminated, that is, all hierarchical structure is
-          lost.
-        - The same subsystem can be used multiple times, its blocks and wires
-           will be cloned.  Subsystems can also include subsystems.
-        - The number of input and output ports is not specified, they are computed
-          from the number of ports on the ``InPort`` and ``OutPort`` blocks within the
-          subsystem.
         """
         super().__init__(**blockargs)
 
         if isinstance(subsys, str):
             # attempt to import the file
             try:
                 module = importlib.import_module(subsys, package=".")
@@ -425,101 +465,107 @@
 # ------------------------------------------------------------------------ #
 
 
 class InPort(SubsystemBlock):
     """
     :blockname:`INPORT`
 
-    .. table::
-       :align: left
+    Input ports for a subsystem.
 
-    +------------+---------+---------+
-    | inputs     | outputs |  states |
-    +------------+---------+---------+
-    | 0          | nout    | 0       |
-    +------------+---------+---------+
-    |            | any     |         |
-    +------------+---------+---------+
+    :inputs: 0
+    :outputs: N
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Output
+            - j
+            - any
+            - :math:`y_j`
+
+    This block connects a subsystem to a parent block diagram.  Inputs to the
+    parent-level ``SubSystem`` block appear as the outputs of this block.
+
+    .. note:: Only one ``INPORT`` block can appear in a block diagram but it
+        can have multiple ports.  This is different to Simulink(R) which
+        would require multiple single-port input blocks.
     """
 
     nin = 0
     nout = -1
 
     def __init__(self, nout=1, **blockargs):
         """
-        Input ports for a subsystem.
-
         :param nout: Number of output ports, defaults to 1
         :type nout: int, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: An INPORT block
-        :rtype: InPort instance
-
-        This block connects a subsystem to a parent block diagram.  Inputs to the
-        parent-level ``SubSystem`` block appear as the outputs of this block.
-
-        .. note:: Only one ``INPORT`` block can appear in a block diagram but it
-            can have multiple ports.  This is different to Simulink(R) which
-            would require multiple single-port input blocks.
         """
         super().__init__(nout=nout, **blockargs)
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
         # signal feed through
 
-        return self.inputs
+        return inports
 
 
 # ------------------------------------------------------------------------ #
 
 
 class OutPort(SubsystemBlock):
     """
     :blockname:`OUTPORT`
 
-    .. table::
-       :align: left
+    Output ports for a subsystem.
 
-    +------------+---------+---------+
-    | inputs     | outputs |  states |
-    +------------+---------+---------+
-    | nin        | 0       | 0       |
-    +------------+---------+---------+
-    | any        |         |         |
-    +------------+---------+---------+
+    :inputs: N
+    :outputs: 0
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - i
+            - any
+            - :math:`x_i`
+
+    This block connects a subsystem to a parent block diagram.  The
+    inputs of this block become the outputs of the parent-level ``SubSystem``
+    block.
+
+    .. note:: Only one ``OUTPORT`` block can appear in a block diagram but it
+        can have multiple ports.  This is different to Simulink(R) which
+        would require multiple single-port output blocks.
     """
 
     nin = -1
     nout = 0
 
     def __init__(self, nin=1, **blockargs):
         """
-        Output ports for a subsystem.
-
         :param nin: Number of input ports, defaults to 1
         :type nin: int, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: A OUTPORT block
-        :rtype: OutPort instance
-
-        This block connects a subsystem to a parent block diagram.  The the
-        inputs of this block become the outputs of the parent-level ``SubSystem``
-        block.
-
-        .. note:: Only one ``OUTPORT`` block can appear in a block diagram but it
-            can have multiple ports.  This is different to Simulink(R) which
-            would require multiple single-port output blocks.
         """
         super().__init__(nin=nin, **blockargs)
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
         # signal feed through
-        return self.inputs
+        return inports
 
 
 if __name__ == "__main__":  # pragma: no cover
 
     from pathlib import Path
 
     exec(
```

### Comparing `bdsim-1.0.0/bdsim/blocks/discrete.py` & `bdsim-1.1.0/bdsim/blocks/discrete.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,205 +10,224 @@
 
 import numpy as np
 import math
 from math import sin, cos, atan2, sqrt, pi
 
 import matplotlib.pyplot as plt
 import inspect
-from spatialmath import base, Twist3, SE3
+from spatialmath import Twist3, SE3
+import spatialmath.base as smb
 
 from bdsim.components import ClockedBlock
 
 # ------------------------------------------------------------------------
 
 
 class ZOH(ClockedBlock):
     """
     :blockname:`ZOH`
 
-    .. table::
-       :align: left
+    Zero-order hold.
 
-    +------------+---------+---------+
-    | inputs     | outputs |  states |
-    +------------+---------+---------+
-    | 1          | 1       | N       |
-    +------------+---------+---------+
-    | float,     | float,  |         |
-    | A(N,)      | A(N,)   |         |
-    +------------+---------+---------+
+    :inputs: 1
+    :outputs: 1
+    :states: N
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - 0
+            - float, ndarray
+            - :math:`x`
+        *   - Output
+            - 0
+            - float, ndarray
+            - :math:`y`
+
+    Output is the input at the previous clock time $y_{k} = x_{k-1}.  The state can be a
+    scalar or a vector, this is given by the type of ``x0``.
+
+    .. note:: If input is not a scalar, ``x0`` must have the shape of the
+        input signal.
     """
 
     nin = 1
     nout = 1
 
     def __init__(self, clock, x0=0, **blockargs):
         """
-        Zero-order hold.
-
         :param clock: clock source
         :type clock: Clock
         :param x0: Initial value of the hold, defaults to 0
         :type x0: array_like, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: a ZOH block
-        :rtype: Integrator instance
-
-        Output is the input at the previous clock time.  The state can be a scalar or a
-        vector, this is given by the type of ``x0``.
-
-        .. note:: If input is not a scalar, ``x0`` must have the shape of the
-            input signal.
         """
         self.type = "sampler"
         super().__init__(nin=1, nout=1, clock=clock, **blockargs)
 
-        x0 = base.getvector(x0)
+        x0 = smb.getvector(x0)
         self._x0 = x0
         self.ndstates = len(x0)
         # print('nstates', self.nstates)
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
         # print('* output, x is ', self._x)
-        return [self._x]
+        return [x]
 
-    def next(self):
-        xnext = np.array(self.inputs)
-        return xnext
+    def next(self, t, inports, x):
+        u = smb.getvector(inports[0])
+        return u  # must be an ndarray
 
 
 # ------------------------------------------------------------------------
 
 
 class DIntegrator(ClockedBlock):
     """
     :blockname:`DINTEGRATOR`
 
-    .. table::
-       :align: left
+    Discrete-time integrator.
 
-    +------------+---------+---------+
-    | inputs     | outputs |  states |
-    +------------+---------+---------+
-    | 1          | 1       | N       |
-    +------------+---------+---------+
-    | float,     | float,  |         |
-    | A(N,)      | A(N,)   |         |
-    +------------+---------+---------+
+    :inputs: 1
+    :outputs: 1
+    :states: N
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - 0
+            - float, ndarray
+            - :math:`x`
+        *   - Output
+            - 0
+            - float, ndarray
+            - :math:`y`
+
+    Create a discrete-time integrator block.
+
+    Output is the time integral of the input.  The state can be a scalar or a
+    vector, this is given by the type of ``x0``.
+
+    The minimum and maximum values can be:
+
+        - a scalar, in which case the same value applies to every element of
+          the state vector, or
+        - a vector, of the same shape as ``x0`` that applies elementwise to
+          the state.
     """
 
     nin = 1
     nout = 1
 
     def __init__(self, clock, x0=0, gain=1.0, min=None, max=None, **blockargs):
         """
-        Discrete-time integrator.
-
         :param clock: clock source
         :type clock: Clock
         :param x0: Initial state, defaults to 0
         :type x0: array_like, optional
         :param gain: gain or scaling factor, defaults to 1
         :type gain: float
         :param min: Minimum value of state, defaults to None
         :type min: float or array_like, optional
         :param max: Maximum value of state, defaults to None
         :type max: float or array_like, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: an INTEGRATOR block
-        :rtype: Integrator instance
-
-        Create a discrete-time integrator block.
-
-        Output is the time integral of the input.  The state can be a scalar or a
-        vector, this is given by the type of ``x0``.
-
-        The minimum and maximum values can be:
-
-            - a scalar, in which case the same value applies to every element of
-              the state vector, or
-            - a vector, of the same shape as ``x0`` that applies elementwise to
-              the state.
         """
         super().__init__(clock=clock, **blockargs)
 
         if isinstance(x0, (int, float)):
             x0 = np.r_[x0]
 
         elif isinstance(x0, np.ndarray):
             if x0.ndim > 1:
                 raise ValueError("state must be a 1D vector")
         else:
-            x0 = base.getvector(x0)
+            x0 = smb.getvector(x0)
 
         self.ndstates = x0.shape[0]
 
         if min is not None:
-            min = base.getvector(min, self.ndstates)
+            min = smb.getvector(min, self.ndstates)
         if max is not None:
-            max = base.getvector(max, self.ndstates)
+            max = smb.getvector(max, self.ndstates)
 
         self._x0 = x0
         self.min = min
         self.max = max
         self.gain = gain
 
-    def output(self, t=None):
-        return [self._x]
+    def output(self, t, u, x):
+        return [x]
 
-    def next(self):
-        xnext = self._x + self.gain * self.clock.T * np.array(self.inputs[0])
+    def next(self, t, u, x):
+        xnext = x + self.gain * self.clock.T * np.array(u[0])
         if self.min is not None or self.max is not None:
             xnext = np.clip(xnext, self.min, self.max)
         return xnext
 
 
 class DPoseIntegrator(ClockedBlock):
     """
     :blockname:`DPOSEINTEGRATOR`
 
-    .. table::
-       :align: left
+    Discrete-time spatial velocity integrator.
+
+    :inputs: 1
+    :outputs: 1
+    :states: 6
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - 0
+            - ndarray(6,)
+            - :math:`x`
+        *   - Output
+            - 0
+            - SE3
+            - :math:`y`
+
+    This block integrates spatial velocity over time.
+    The block input is a spatial velocity as a 6-vector
+    :math:`(v_x, v_y, v_z, \omega_x, \omega_y, \omega_z)` and the output
+    is pose as an ``SE3`` instance.
 
-       +------------+---------+---------+
-       | inputs     | outputs |  states |
-       +------------+---------+---------+
-       | 1          | 1       | N       |
-       +------------+---------+---------+
-       | A(6,)      | SE3     |         |
-       +------------+---------+---------+
+    .. note:: State is a velocity twist.
     """
 
     nin = 1
     nout = 1
     inlabels = ("ν",)
     outlabels = ("ξ",)
 
     def __init__(self, clock, x0=None, **blockargs):
         r"""
-        Discrete-time spatial velocity integrator.
-
         :param clock: clock source
         :type clock: Clock
         :param x0: Initial pose, defaults to null
         :type x0: SE3, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: an DPOSEINTEGRATOR block
-        :rtype: Integrator instance
-
-        This block integrates spatial velocity over time.
-        The block input is a spatial velocity as a 6-vector
-        :math:`(v_x, v_y, v_z, \omega_x, \omega_y, \omega_z)` and the output
-        is pose as an ``SE3`` instance.
-
-        .. note:: State is a velocity twist.
-
         """
         super().__init__(clock=clock, **blockargs)
 
         if x0 is None:
             x0 = Twist3()
         elif isinstance(x0, SE3):
             x0 = Twist3(x0).A
@@ -219,20 +238,20 @@
 
         self.ndstates = 6
 
         self._x0 = x0
 
         print("nstates", self.nstates, x0)
 
-    def output(self, t=None):
-        return [Twist3(self._x).SE3()]
+    def output(self, t, u, x):
+        return [Twist3(x).SE3()]
 
-    def next(self):
-        T_delta = SE3.Delta(self.inputs[0] * self.clock.T)
-        pose = Twist3(self._x).SE3() * T_delta
+    def next(self, t, u, x):
+        T_delta = SE3.Delta(u[0] * self.clock.T)
+        pose = Twist3(x).SE3() * T_delta
         return Twist3(pose).A
 
 
 # ------------------------------------------------------------------------ #
 
 
 # @block
```

### Comparing `bdsim-1.0.0/bdsim/blocks/displays.py` & `bdsim-1.1.0/bdsim/blocks/displays.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,260 +25,315 @@
 # ------------------------------------------------------------------------ #
 
 
 class Scope(GraphicsBlock):
     """
     :blockname:`SCOPE`
 
-    .. table::
-       :align: left
+    Plot input signals against time.
 
-       +--------+---------+---------+
-       | inputs | outputs |  states |
-       +--------+---------+---------+
-       | 1      | 0       | 0       |
-       +--------+---------+---------+
-       | float, |         |         |
-       | A(N,)  |         |         |
-       +--------+---------+---------+
+    :inputs: N
+    :outputs: 0
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - i
+            - float
+            - :math:`x_i` is the i'th line
+
+    Create a scope block that plots multiple signals against time.
+
+    For each line plotted we can specify the:
+    
+    * line style as a heterogeneous list of:
+
+      * Matplotlib `fmt` string comprising a color and line style, eg. ``"k"`` or ``"r:"``
+
+      * a dict of Matplotlib line style options for `Line2D <https://matplotlib.org/3.2.2/api/_as_gen/matplotlib.lines.Line2D.html#matplotlib.lines.Line2D>`_
+        , eg. ``{"color": "k", "linewidth": 3, "alpha": 0.5)``
+
+    * line label, used in the legend and vertical axis. This can include math mode
+      notation or unicode characters.
+
+    The vertical scale factor defaults to auto-scaling but can be fixed by
+    providing a 2-tuple ``[ymin, ymax]``. All lines are plotted against the
+    same vertical scale.
+
+    .. figure:: ../../figs/Figure_1.png
+        :width: 500px
+        :alt: example of generated graphic
+
+        Example of scope display.
+
+    **Scalar input ports against time**
+
+    The number of lines to plot will be inferred from:
+
+    * the length of the ``labels`` list if specified
+    * the length of the ``styles`` list if specified
+    * ``nin`` if specified, it defaults to 1
+
+    These numbers must be consistent.
+
+    Examples::
+
+        bd.SCOPE()       # a scope with 1 input port
+        bd.SCOPE(nin=3)  # a scope with 3 input ports
+        bd.SCOPE(styles=["k", "r--"])        # a scope with 2 input ports
+        bd.SCOPE(labels=["x", r"$\gamma$"])  # a scope with 2 input ports
+        bd.SCOPE(styles=[{'color': 'blue'}, {'color': 'red', 'linestyle': '--'}])
+
+    **Single input port with NumPy array**
+     
+    The port is fed with a 1D-array, and ``vector`` is an:
+
+    * int, this is the expected width of the array, all its elements will be plotted
+    * a list of ints, interpretted as indices of the elements to plot.
+
+    Examples::
+
+        bd.SCOPE(vector=[0,1,2]) # display elements 0, 1, 2 of array on port 0
+        bd.SCOPE(vector=[0,1], styles=[{'color': 'blue'}, {'color': 'red', 'linestyle': '--'}])
+
+    .. note:: 
+        * If the vector is of width 3, by default the inputs are plotted as red, green 
+          and blue lines. 
+        * If the vector is of width 6, by default the first three inputs are plotted as
+          solid red, green and blue lines and the last three inputs are plotted as 
+          dashed red, green and blue lines.
     """
 
     nin = -1
     nout = 0
 
     def __init__(
         self,
-        nin=None,
+        nin=1,
         vector=None,
         styles=None,
         stairs=False,
         scale="auto",
         labels=None,
         grid=True,
         watch=False,
+        title=None,
+        loc="best",
         **blockargs,
     ):
         """
-        Plots input signals against time.
-
         :param nin: number of inputs, defaults to 1 or if given, the length of
                     style vector
         :type nin: int, optional
         :param vector: vector signal on single input port, defaults to None
         :type vector: int or list, optional
         :param styles: styles for each line to be plotted
         :type styles: str or dict, list of strings or dicts; one per line, optional
-        :param stairs: force staircase style plot, defaults to False
+        :param stairs: force staircase style plot for all lines, defaults to False
         :type stairs: bool, optional
         :param scale: fixed y-axis scale or defaults to 'auto'
         :type scale: str or array_like(2)
         :param labels: vertical axis labels
         :type labels: sequence of strings
         :param grid: draw a grid, defaults to True. Can be boolean or a tuple of
                      options for grid()
         :type grid: bool or sequence
         :param watch: add these signals to the watchlist, defaults to False
         :type watch: bool, optional
+        :param title: title of plot
+        :type title: str
+        :param loc: location of legend, see :meth:`matplotlib.pyplot.legend`, defaults to "best"
+        :type loc: str
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: A SCOPE block
-        :rtype: Scope instance
-
-        Create a block that plots:
-
-        * scalar input ports against time, ``vector=None``
-        * selected elements of a NumPy array on a single input port. If ``vector`` is an
-          int this is the expected width of the array. If ``vector`` is a list of ints these
-          are the indices of the array to display.
-
-        Each line can have its own color or style which is specified by:
-
-            - a dict of options for `Line2D <https://matplotlib.org/3.2.2/api/_as_gen/matplotlib.lines.Line2D.html#matplotlib.lines.Line2D>`_ or
-            - a  MATLAB-style linestyle like 'k--'
-
-        The number of lines to plot will be inferred from:
-        * the length of the ``labels`` list if specified
-        * the length of the ``styles`` list if specified
-        * ``nin`` if specified
-        * ``vector`` if specified
-
-        If multiple lines are plotted then a heterogeneous list of styles, dicts or strings,
-        one per line must be given.
-
-        The vertical scale factor defaults to auto-scaling but can be fixed by
-        providing a 2-tuple [ymin, ymax]. All lines are plotted against the
-        same vertical scale.
-
-        Examples::
-
-            SCOPE()
-            SCOPE(nin=2)
-            SCOPE(nin=2, scale=[-1,2])
-            SCOPE(styles='k--')
-            SCOPE(styles=[{'color': 'blue'}, {'color': 'red', 'linestyle': '--'}])
-            SCOPE(styles=['k', 'r--'])
-            SCOPE(vector=[0,1,2]) # display elements 0, 1, 2 of array on port 0
-
-
-        .. figure:: ../../figs/Figure_1.png
-           :width: 500px
-           :alt: example of generated graphic
-
-           Example of scope display.
         """
 
         def listify(s):
+            # guarantee that result is a list
             if isinstance(s, str):
                 return [s]
             elif isinstance(s, (list, tuple)):
                 return s
             else:
                 raise ValueError("unknown argument to listify")
 
         # number of lines plotted (nplots) is inferred from the number of labels
         # or linestyles
-        nplots = None
-
-        if nin is not None:
-            nplots = nin
-
-        if styles is not None:
-            self.styles = listify(styles)
-            if nplots is not None:
-                assert nplots == len(styles), "need one style per input"
-            else:
-                nplots = len(styles)
-
-        if labels is not None:
-            self.labels = listify(labels)
-            if nplots is not None:
-                assert nplots == len(labels), "need one label per input"
-            else:
-                nplots = len(labels)
-        else:
-            self.labels = None
 
+        nplots = None
         if vector is not None:
             # vector argument is given
             #  block has single input which is an array
             #  vector is int, width of vector
             #  vector is a list of ints, select those inputs from the input vector
 
-            if nin is not None and nin != 1:
+            if nin != 1:
                 raise ValueError("if vector is given, nin must be 1")
 
             if isinstance(vector, int):
-                nvec = vector
+                nplots = vector
             elif isinstance(vector, list):
-                nvec = len(vector)
+                nplots = len(vector)
             else:
                 raise ValueError("vector must be an int or list of indices")
 
+        if styles is not None:
+            self.styles = listify(styles)
             if nplots is None:
-                nplots = nvec
+                nplots = len(self.styles)
             else:
-                if nvec != nplots:
-                    raise ValueError("vector argument doesnt match nplots")
-
-        if nplots is None:
-            # still indeterminate, set default
-            nin = 1
-            nplots = 1
+                assert nplots == len(self.styles), "need one style per plot"
+        else:
+            self.styles = None
 
-        if vector is not None:
-            nin = 1
-            nplots = nvec
+        if labels is not None:
+            self.labels = listify(labels)
+            if nplots is None:
+                nplots = len(self.labels)
+            else:
+                assert nplots == len(self.labels), "need one label per plot"
         else:
+            self.labels = None
+
+        if nplots is None:
+            # nplots has not been determined from styles or labels, so use nin
+            nplots = nin
+        elif nin == 1 and vector is None:
+            # nplots is different to the default nin value, override it
             nin = nplots
 
         self.nplots = nplots
         self.vector = vector
 
         super().__init__(nin=nin, **blockargs)
 
-        if styles is None:
-            self.styles = [None] * nplots
-
         self.xlabel = "Time (s)"
 
         self.grid = grid
         self.stairs = stairs
 
         self.line = [None] * nplots
         self.scale = scale
 
         self.watch = watch
+        self.title = title
+        self.loc = loc
 
         # TODO, wire width
         # inherit names from wires, block needs to be able to introspect
 
-    def start(self, state=None):
+    def start(self, simstate):
+        super().start(simstate)
+
+        if not self._enabled:
+            return
+
         # init the arrays that hold the data
         self.tdata = np.array([])
         self.ydata = [
             np.array([]),
         ] * self.nplots
 
+
         # create the figures
-        self.fig = self.create_figure(state)
+        self.fig = self.create_figure(simstate)
         self.ax = self.fig.add_subplot(111)
 
-        if self.stairs:
-            kwargs = {**dict(drawstyle="steps"), **kwargs}
+        # get labels if not provided
+        if self.labels is None:
+            if self.vector is None:
+                self.labels = [self.sourcename(i) for i in range(self.nin)]
+            else:
+                self.labels = [str(i) for i in range(self.vector)]
+                if self.styles is None:
+                    if self.vector == 3:
+                        self.styles = ["r", "g", "b"]
+                    elif self.vector == 6:
+                        self.styles = ["r", "g", "b", "r--", "g--", "b--"]
+
+        if self.styles is None:
+            self.styles = [None] * self.nplots
 
         # create empty lines with defined styles
         for i in range(0, self.nplots):
             args = []
             kwargs = {}
             style = self.styles[i]
             if isinstance(style, dict):
                 kwargs = style
             elif isinstance(style, str):
                 args = [style]
+            if self.stairs:
+                kwargs["drawstyle"] = "steps"  # force steppy plot
+
             (self.line[i],) = self.ax.plot(
-                self.tdata, self.ydata[i], *args, label=self.styles[i], linewidth=2
+                self.tdata,
+                self.ydata[i],
+                *args,
+                label=self.styles[i],
+                linewidth=2,
+                **kwargs,
             )
 
         # label the axes
         if self.labels is not None:
             self.ax.set_ylabel(",".join(self.labels))
         self.ax.set_xlabel(self.xlabel)
-        self.ax.set_title(self.name_tex)
+
+        if self.title is not None:
+            name = self.title
+        else:
+            name = self.name_tex
+        self.ax.set_title(name)
 
         # grid control
         if self.grid is True:
             self.ax.grid(self.grid)
         elif isinstance(self.grid, (list, tuple)):
             self.ax.grid(True, *self.grid)
 
         # set limits
-        self.ax.set_xlim(0, state.T)
+        self.ax.set_xlim(0, simstate.T)
 
         if self.scale != "auto":
             self.ax.set_ylim(*self.scale)
         if self.labels is not None:
-            self.ax.legend(self.labels)
+            def fix_underscore(s):
+                if s[0] == "_":
+                    return "-" + s[1:]
+                else:
+                    return s
+            self.ax.legend([fix_underscore(label) for label in self.labels], loc=self.loc)
 
         if self.watch:
             for wire in self.input_wires:
                 plug = wire.start  # start plug for input wire
 
                 # append to the watchlist, bdsim.run() will do the rest
-                state.watchlist.append(plug)
-                state.watchnamelist.append(str(plug))
+                simstate.watchlist.append(plug)
+                simstate.watchnamelist.append(str(plug))
+        plt.draw()
+        plt.show(block=False)
 
-        super().start()
+    def step(self, t, inports):
+        if not self._enabled:
+            return
 
-    def step(self, state=None):
         # inputs are set
-        self.tdata = np.append(self.tdata, state.t)
+        self.tdata = np.append(self.tdata, t)
 
         if self.vector is None:
             # take data from multiple inputs as a list
-            data = self.inputs
+            data = inports
             if len(data) != self.nplots:
                 raise RuntimeError(
                     "number of signals to plot doesnt match init parameters"
                 )
 
         else:
             # single input with vector data
@@ -293,34 +348,62 @@
         # plot the data
         for i in range(0, self.nplots):
             self.line[i].set_data(self.tdata, self.ydata[i])
 
         if self.scale == "auto":
             self.ax.relim()
             self.ax.autoscale_view(scalex=False, scaley=True)
-        super().step(state=state)
+
+        super().step(t, inports)
 
 
 # ------------------------------------------------------------------------ #
 
 
 class ScopeXY(GraphicsBlock):
     """
     :blockname:`SCOPEXY`
 
-    .. table::
-       :align: left
+    Plot X against Y.
+
+    :inputs: 2
+    :outputs: 0
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - 0
+            - float
+            - :math:`x`
+        *   - Input
+            - 1
+            - float
+            - :math:`y`
+
+    Create an XY scope where input :math:`y` (vertical axis) is plotted against :math:`x`
+    (horizontal axis).
+
+    Line style is one of:
+
+      * Matplotlib `fmt` string comprising a color and line style, eg. ``"k"`` or ``"r:"``
+
+      * a dict of Matplotlib line style options for `Line2D <https://matplotlib.org/3.2.2/api/_as_gen/matplotlib.lines.Line2D.html#matplotlib.lines.Line2D>`_
+        , eg. ``dict(color="k", linewidth=3, alpha=0.5)``
+
+    The scale factor defaults to auto-scaling but can be fixed by
+    providing either:
 
-    +--------+---------+---------+
-    | inputs | outputs |  states |
-    +--------+---------+---------+
-    | 2      | 0       | 0       |
-    +--------+---------+---------+
-    | float  |         |         |
-    +--------+---------+---------+
+        - a 2-tuple ``[min, max]`` which is used for the x- and y-axes
+        - a 4-tuple ``[xmin, xmax, ymin, ymax]``
     """
 
     nin = 2
     nout = 0
 
     def __init__(
         self,
@@ -339,35 +422,14 @@
         :type scale: str or array_like(2) or array_like(4)
         :param labels: axis labels (xlabel, ylabel), defaults to ["X","Y"]
         :type labels: 2-element tuple or list
         :param init: function to initialize the graphics, defaults to None
         :type init: callable
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: A SCOPEXY block
-        :rtype: ScopeXY instance
-
-        Create an XY scope.
-
-        This block has two inputs which are plotted against each other. Port 0
-        is the horizontal axis, and port 1 is the vertical axis.
-
-        The line style is given by either:
-
-            - a dict of options for ``plot``, or
-            - as a simple MATLAB-style linestyle like ``'k--'``.
-
-        The scale factor defaults to auto-scaling but can be fixed by
-        providing either:
-
-            - a 2-tuple [min, max] which is used for the x- and y-axes
-            - a 4-tuple [xmin, xmax, ymin, ymax]
-
-        :input x: signal plotted on horizontal axis
-        :input y: signal plotted on vertical axis
         """
         super().__init__(**blockargs)
         self.xdata = []
         self.ydata = []
         if init is not None:
             assert callable(init), "graphics init function must be callable"
         self.init = init
@@ -376,29 +438,34 @@
         if scale != "auto":
             scale = sm.expand_dims(scale, 2)
         self.scale = scale
         self.aspect = aspect
         self.labels = labels
         self.inport_names(("x", "y"))
 
-    def start(self, state, **kwargs):
+    def start(self, simstate):
+        super().start(simstate)
+
+        if not self._enabled:
+            return
+
         # create the plot
         super().reset()
 
-        self.fig = self.create_figure(state)
+        self.fig = self.create_figure(simstate)
         self.ax = self.fig.gca()
 
         args = []
         blockargs = {}
         style = self.styles
         if isinstance(style, dict):
             blockargs = style
         elif isinstance(style, str):
             args = [style]
-        (self.line,) = self.ax.plot(self.xdata, self.ydata, *args, **kwargs)
+        (self.line,) = self.ax.plot(self.xdata, self.ydata, *args)
 
         self.ax.grid(True)
         self.ax.set_xlabel(self.labels[0])
         self.ax.set_ylabel(self.labels[1])
         self.ax.set_title(self.name)
         if not (isinstance(self.scale, str) and self.scale == "auto"):
             self.ax.set_xlim(*self.scale[0:2])
@@ -406,55 +473,78 @@
         self.ax.set_aspect(self.aspect)
         if self.init is not None:
             self.init(self.ax)
 
         plt.draw()
         plt.show(block=False)
 
-        super().start()
-
-    def step(self, state=None):
-        self._step(self.inputs[0], self.inputs[1], state)
+    def step(self, t, inports):
+        if not self._enabled:
+            return
+        self._step(inports[0], inports[1], t)
 
-    def _step(self, x, y, state):
+    def _step(self, x, y, t):
         self.xdata.append(x)
         self.ydata.append(y)
 
-        # if self.bd.runtime.options.graphics:
         plt.figure(self.fig.number)
         self.line.set_data(self.xdata, self.ydata)
 
         if self.bd.runtime.options.animation:
             self.fig.canvas.flush_events()
 
         if isinstance(self.scale, str) and self.scale == "auto":
             self.ax.relim()
             self.ax.autoscale_view()
-        super().step(state=state)
+        super().step(t, None)
 
     # def done(self, block=False, **blockargs):
     #     if self.bd.runtime.options.graphics:
     #         plt.show(block=block)
     #         super().done()
 
 
 class ScopeXY1(ScopeXY):
     """
     :blockname:`SCOPEXY1`
 
-    .. table::
-       :align: left
+    Plot X[0] against X[1].
+
+    :inputs: 1
+    :outputs: 0
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - 0
+            - ndarray
+            - :math:`x`
 
-    +-------------+---------+---------+
-    | inputs      | outputs |  states |
-    +-------------+---------+---------+
-    | 1           | 0       | 0       |
-    +-------------+---------+---------+
-    | ndarray(2)  |         |         |
-    +-------------+---------+---------+
+    Create an XY scope where input :math:`x_j` (vertical axis) is plotted against
+    :math:`x_i` (horizontal axis). This block has one vector input and the elements to
+    be plotted are given by a 2-element iterable :math:`(i, j)`.
+
+    Line style is one of:
+
+      * Matplotlib `fmt` string comprising a color and line style, eg. ``"k"`` or ``"r:"``
+
+      * a dict of Matplotlib line style options for `Line2D <https://matplotlib.org/3.2.2/api/_as_gen/matplotlib.lines.Line2D.html#matplotlib.lines.Line2D>`_
+        , eg. ``dict(color="k", linewidth=3, alpha=0.5)``
+
+    The scale factor defaults to auto-scaling but can be fixed by
+    providing either:
+
+        - a 2-tuple ``[min, max]`` which is used for the x- and y-axes
+        - a 4-tuple ``[xmin, xmax, ymin, ymax]``
     """
 
     nin = 1
     nout = 0
 
     def __init__(self, indices=[0, 1], **blockargs):
         """
@@ -466,45 +556,30 @@
         :type scale: str or array_like(2) or array_like(4)
         :param labels: axis labels (xlabel, ylabel)
         :type labels: 2-element tuple or list
         :param init: function to initialize the graphics, defaults to None
         :type init: callable
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: A SCOPEXY block
-        :rtype: ScopeXY instance
-
-        Create an XY scope with vector input
-
-        This block has one vector input and two elemetns are plotted against each other. The first
-        selected element is the horizontal axis, and second is the vertical axis.
-
-        The line style is given by either:
-
-            - a dict of options for ``plot``, or
-            - as a simple MATLAB-style linestyle like ``'k--'``.
-
-        The scale factor defaults to auto-scaling but can be fixed by
-        providing either:
-
-            - a 2-tuple [min, max] which is used for the x- and y-axes
-            - a 4-tuple [xmin, xmax, ymin, ymax]
         """
         super().__init__(**blockargs)
         self.inport_names(("xy",))
         if len(indices) != 2:
             raise ValueError("indices must have 2 elements")
         self.indices = [int(x) for x in indices]
 
-    def step(self, state=None):
+    def step(self, t, inports):
+        if not self._enabled:
+            return
+
         # inputs are set
-        x = self.inputs[0][self.indices[0]]
-        y = self.inputs[0][self.indices[1]]
+        x = inports[0][self.indices[0]]
+        y = inports[0][self.indices[1]]
 
-        super()._step(x, y, state)
+        super()._step(x, y, t)
 
 
 # ------------------------------------------------------------------------ #
 
 
 if __name__ == "__main__":  # pragma: no cover
```

### Comparing `bdsim-1.0.0/bdsim/blocks/functions.py` & `bdsim-1.1.0/bdsim/blocks/functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,97 +6,115 @@
 - are a subclass of ``FunctionBlock`` |rarr| ``Block``
 
 """
 
 # The constructor of each class ``MyClass`` with a ``@block`` decorator becomes a method ``MYCLASS()`` of the BlockDiagram instance.
 
 import numpy as np
+from scipy import linalg
 import scipy.interpolate
 import math
 import inspect
 import spatialmath.base as smb
 from typing import Any, Union, Callable
 
 ArrayLike = Union[np.ndarray, int, float, list, tuple]
 
 from bdsim.components import FunctionBlock
 
-
-# PID
-# product
+# TODO:
 # transform 3D points
 
 
 class Sum(FunctionBlock):
-    """Summing junction.
+    """
     :blockname:`SUM`
 
-    :inputs: N [float, ndarray(N), ndarray(N,M)]
-
-    :outputs: 1 [float, ndarray(N), ndarray(N,M)]
+    Summing junction.
 
+    :inputs: N
+    :outputs: 1
     :states: 0
 
-    :param signs: signs associated with input ports, accepted characters: + or -, defaults to '++'
-    :type signs: str, optional
-    :param mode: controls angle wrapping per element, accepted characters r or c or C or L, defaults to None
-    :type mode: str, optional
-    :param inputs: Optional incoming connections
-    :type inputs: Block or Plug
-    :param blockargs: |BlockOptions|
-    :type blockargs: dict
-    :return: A SUM block
-    :rtype: Sum instance
+    .. list-table::
+        :header-rows: 1
 
-    Add or subtract input signals according to the `signs` string.  The
+        * - Port type
+          - Port number
+          - Types
+          - Description
+        * - Input
+          - i
+          - int, float, ndarray
+          - :math:`x_i`
+        * - Output
+          - 0
+          - int, float, ndarray
+          - :math:`\sum_i \pm x_i`
+
+    Add or subtract input signals according to the ``signs`` string.  The
     number of input ports is the length of this string.
 
     For example::
 
         sum = bd.SUM('+-+')
 
-    is a 3-input summing junction which computes port0 - port1 + port2.
-
-    If some elements of the inputs are angles then ``mode`` controls, per element, how
-    they are wrapped.  The elements of the string can be
+    is a 3-input summing junction which computes ``in[0] - in[1] + in[2]``.
 
-    | character  | purpose                           |
-    | :--------- | :-------------------------------- |
-    | r          | real number, don't wrap (default) |
-    | c          | angle on circle, wrap to [-π, π)  |
-    | C          | angle on circle, wrap to [0, 2π)  |
-    | L          | latitude angle, wrap to [0, π]    |
-
-    For example if ``mode="rc"`` then a 2-element array would have its
-    second element wrapped to the range [-π, π).
-
-    :note: The signals must be compatible, all scalars, or all arrays
-        of the same shape.
+    :note: The signals must be compatible for addition, and if some are
+        arrays they must be broadcastable.
     """
 
     nin = -1
     nout = 1
 
     _modefuncs = {
         "r": lambda x: x,
         "c": smb.wrap_mpi_pi,
         "C": smb.wrap_0_2pi,
         "L": smb.wrap_0_pi,
         "l": smb.wrap_0_pi,
     }
 
     def __init__(self, signs: str = "++", mode: str = None, **blockargs):
+        """
+        :param signs: signs associated with input ports, accepted characters: + or -, defaults to "++"
+        :type signs: str, optional
+        :param mode: controls addition mode, per element, string comprises ``r`` or ``c`` or ``C`` or ``L``, defaults to None
+        :type mode: str, optional
+        :param blockargs: |BlockOptions|
+        :type blockargs: dict
+
+        ``mode`` controls how elements of the input vectors are added/subtracted.
+        Elements which are angles must be treated specially, and this is indicated by
+        the corresponding characters in ``mode``.  The string's length must equal the
+        width of the input vectors. The characters of the string can be:
+
+        ==============  ============================================
+        mode character  purpose
+        ==============  ============================================
+        r               real number, don't wrap (default)
+        c               angle on circle, wrap to [-π, π)
+        C               angle on circle, wrap to [0, 2π)
+        L               colatitude angle, wrap to [0, π]
+        ==============  ============================================
+
+        For example if ``mode="rc"`` then a 2-element array would have its
+        second element wrapped to the range [-π, π).
+
+        """
         super().__init__(nin=len(signs), **blockargs)
+
         assert isinstance(signs, str), "first argument must be signs string"
         assert all([x in "+-" for x in signs]), "invalid sign"
         self.signs = signs
         self.mode = mode
 
-    def output(self, t=None):
-        for i, input in enumerate(self.inputs):
+    def output(self, t, inports, x):
+        for i, input in enumerate(inports):
             # code makes no assumption about types of inputs
             # NOTE: use sum = sum =/- input rather than sum +/-= input since
             #       these are references
             if self.signs[i] == "-":
                 if i == 0:
                     sum = -input
                 else:
@@ -135,66 +153,79 @@
                 sum = self._modefuncs[self.mode[0]](sum)
 
         return [sum]
 
 
 # ------------------------------------------------------------------------ #
 class Prod(FunctionBlock):
-    """Product junction.
-
+    r"""
     :blockname:`PROD`
 
-    :inputs: N [float, ndarray(N), ndarray(N,M)]
-
-    :outputs: 1 [float, ndarray(N), ndarray(N,M)]
+    Product junction.
 
+    :inputs: N
+    :outputs: 1
     :states: 0
 
-    :param ops: operations associated with input ports, accepted characters: * or /, defaults to '**'
-    :type ops: str, optional
-    :param inputs: Optional incoming connections
-    :type inputs: Block or Plug
-    :param matrix: Arguments are matrices, defaults to False
-    :type matrix: bool, optional
-    :param blockargs: |BlockOptions|
-    :type blockargs: dict
-    :return: A PROD block
-    :rtype: Prod instance
+    .. list-table::
+        :header-rows: 1
 
-    Multiply or divide input signals according to the `ops` string.  The
+        * - Port type
+          - Port number
+          - Types
+          - Description
+        * - Input
+          - i
+          - int, float, ndarray
+          - :math:`x_i`
+        * - Output
+          - 0
+          - int, float, ndarray
+          - :math:`\prod_i \{x_i | \frac{1}{x_i}\}`
+
+    Multiply or divide input signals according to the ``ops`` string.  The
     number of input ports is the length of this string.
 
     For example::
 
         prod = PROD('*/*')
 
-    is a 3-input product junction which computes port0 / port 1 * port2.
-
-    :note: The inputs can be scalars or NumPy arrays.
+    is a 3-input product junction which computes ``in[0] / in[1] * in[2]``.
 
     :note: By default the ``*`` and ``/`` operators are used which perform element-wise
         operations.
 
     :note: The option ``matrix`` will instead use ``@`` and ``@ np.linalg.inv()``. The
         shapes of matrices must conform.  A matrix on a ``/`` input must be square and
-        non-singular.
+        non-singular.  Matrices are multiplied in ascending port order.
     """
 
     nin = -1
     nout = 1
 
     def __init__(self, ops: str = "**", matrix: bool = False, **blockargs):
+        """
+        :param ops: operations associated with input ports, accepted characters: * or /, defaults to '**'
+        :type ops: str, optional
+        :param inputs: Optional incoming connections
+        :type inputs: Block or Plug
+        :param matrix: Arguments are matrices, defaults to False
+        :type matrix: bool, optional
+        :param blockargs: |BlockOptions|
+        :type blockargs: dict
+
+        """
         super().__init__(nin=len(ops), **blockargs)
         assert isinstance(ops, str), "first argument must be signs string"
         assert all([x in "*/" for x in ops]), "invalid op"
         self.ops = ops
         self.matrix = matrix
 
-    def output(self, t=None):
-        for i, input in enumerate(self.inputs):
+    def output(self, t, inports, x):
+        for i, input in enumerate(inports):
             if i == 0:
                 if self.ops[i] == "*":
                     prod = input
                 else:
                     if self.matrix:
                         prod = np.linalg.inv(input)
                     prod = 1.0 / input
@@ -216,166 +247,311 @@
 # ------------------------------------------------------------------------ #
 
 
 class Gain(FunctionBlock):
     """
     :blockname:`GAIN`
 
-    .. table::
-       :align: left
+    Gain block.
+
+    :inputs: 1
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        * - Port type
+          - Port number
+          - Types
+          - Description
+        * - Input
+          - 0
+          - int, float, ndarray
+          - :math:`x`
+        * - Output
+          - 0
+          - int, float, ndarray
+          - :math:`K x`
+
+    Either or both the input and gain can be Numpy arrays and Numpy will
+    compute the appropriate product :math:`u K`.
+
+    If :math:`u` and ``K`` are both NumPy arrays the ``@`` operator is used
+    and :math:`u` is postmultiplied by the gain. To premultiply by the gain,
+    to compute :math:`K u` use the ``premul`` option.
 
-    +------------+---------+---------+
-    | inputs     | outputs |  states |
-    +------------+---------+---------+
-    | 1          | 1       | 0       |
-    +------------+---------+---------+
-    | float,     | float,  |         |
-    | A(N,),     | A(N,),  |         |
-    | A(N,M)     | A(N,M)  |         |
-    +------------+---------+---------+
+    For example::
+
+        gain = bd.GAIN(2.5)
     """
 
     nin = 1
     nout = 1
 
     def __init__(
         self, K: Union[int, float, np.ndarray] = 1, premul: bool = False, **blockargs
     ):
         """
-        Gain block.
-
         :param K: The gain value, defaults to 1
-        :type K: array_like
+        :type K: scalar, array_like
         :param premul: premultiply by constant, default is postmultiply, defaults to False
         :type premul: bool, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: A GAIN block
-        :rtype: Gain instance
-
-        Scale the input signal. If the input is :math:`u` the output is :math:`u K`.
-
-        Either or both the input and gain can be Numpy arrays and Numpy will
-        compute the appropriate product :math:`u K`.
 
-        If :math:`u` and ``K`` are both NumPy arrays the ``@`` operator is used
-        and :math:`u` is postmultiplied by the gain. To premultiply by the gain,
-        to compute :math:`K u` use the ``premul`` option.
-
-        For example::
-
-            gain = bd.GAIN(constant)
         """
         super().__init__(**blockargs)
         self.K = K
         self.premul = premul
 
         self.add_param("K")
 
-    def output(self, t=None):
-        input = self.inputs[0]
+    def output(self, t, inports, x):
+        input = inports[0]
 
         if isinstance(input, np.ndarray) and isinstance(self.K, np.ndarray):
             # array x array case
             if self.premul:
                 # premultiply by gain
                 return [self.K @ input]
             else:
                 # postmultiply by gain
                 return [input @ self.K]
         else:
-            return [self.inputs[0] * self.K]
+            return [input * self.K]
 
 
 # ------------------------------------------------------------------------ #
 
 
-class Clip(FunctionBlock):
+class Pow(FunctionBlock):
     """
+    :blockname:`POW`
+
+    Power block.
+
+    :inputs: 1
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        * - Port type
+          - Port number
+          - Types
+          - Description
+        * - Input
+          - 0
+          - int, float, ndarray
+          - :math:`x`
+        * - Output
+          - 0
+          - int, float, ndarray
+          - :math:`x^p`
+
+    If the input is a Numpy array the result depends on ``matrix``.
+    If ``matrix`` is False the block performs an elementwise exponentiation and
+    the result is a Numpy array of the same size.
+
+    If ``matrix`` is True and the input is a square matrix and ``p`` is an integer
+    then matrixwise exponentiation is performedand using repeated matrix
+    multiplication and matrix inversion.  If ``p`` is not an integer it uses SciPy
+    to compute the power using an eigenvalue decomposition.
+
+    For example::
+
+        pow = bd.POW(2)
+
+    :seealso: :func:`numpy.linalg.matrix_power` :func:`scipy.linalg.fractional_matrix_power`
+    """
+
+    nin = 1
+    nout = 1
+
+    def __init__(self, p: Union[int, float] = 1, matrix: bool = False, **blockargs):
+        """
+        :param p: The exponent value, defaults to 1
+        :type p: scalar
+        :param matrix: premultiply by constant, default is postmultiply, defaults to False
+        :type matrix: bool, optional
+        :param blockargs: |BlockOptions|
+        :type blockargs: dict
+
+        """
+        super().__init__(**blockargs)
+
+        self.p = p
+        self.matrix = matrix
+        self.add_param("p")
+
+    def output(self, t, inports, x):
+        input = inports[0]
+
+        if isinstance(input, np.ndarray):
+            # input is an array
+            if self.matrix:
+                # matrixwise exponentiation
+                if isinstance(self.p, int):
+                    # integer case
+                    return [np.linalg.matrix_power(input, self.p)]
+                else:
+                    # general fractional case
+                    return [linalg.fractional_matrix_power(input, self.p)]
+            else:
+                # elementwise exponentiation
+                return [input**self.p]
+        else:
+            return [input**self.p]
+
+
+# ------------------------------------------------------------------------ #
+
+
+class Clip(FunctionBlock):
+    r"""
     :blockname:`CLIP`
 
-    .. table::
-       :align: left
+    Signal clipping.
+
+    :inputs: 1
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
 
-    +------------+---------+---------+
-    | inputs     | outputs |  states |
-    +------------+---------+---------+
-    | 1          | 1       | 0       |
-    +------------+---------+---------+
-    | float,     | float,  |         |
-    | A(N,)      | A(N,)   |         |
-    +------------+---------+---------+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - 0
+            - int, float, ndarray
+            - :math:`x`
+        *   - Output
+            - 0
+            - int, float, ndarray
+            - :math:`\min(\max(x,a), b)`
+
+    The input signal is clipped to the range from ``minimum`` to ``maximum`` inclusive.
+
+    The signal can be a 1D-array in which case each element is clipped.  The
+    minimum and maximum values can be:
+
+        - a scalar, in which case the same value applies to every element of
+          the input vector , or
+        - a 1D-array, of the same shape as the input vector that applies elementwise to
+          the input vector.
 
+    For example::
+
+        clip = bd.CLIP(-1, 1)
     """
 
     nin = 1
     nout = 1
 
     def __init__(
         self, min: ArrayLike = -math.inf, max: ArrayLike = math.inf, **blockargs
     ):
         """
-        Signal clipping.
-
         :param min: Minimum value, defaults to -math.inf
-        :type min: float or array_like, optional
+        :type min: scalar or array_like, optional
         :param max: Maximum value, defaults to math.inf
         :type max: float or array_like, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: A CLIP block
-        :rtype: Clip instance
-
-        The input signal is clipped to the range from ``minimum`` to ``maximum`` inclusive.
-
-        The signal can be a 1D-array in which case each element is clipped.  The
-        minimum and maximum values can be:
-
-            - a scalar, in which case the same value applies to every element of
-              the input vector , or
-            - a 1D-array, of the same shape as the input vector that applies elementwise to
-              the input vector.
-
-        For example::
-
-            clip = bd.CLIP()
-
         """
         super().__init__(**blockargs)
         self.min = min
         self.max = max
 
-    def output(self, t=None):
-        input = self.inputs[0]
+    def output(self, t, inports, x):
+        input = inports[0]
 
         if isinstance(input, np.ndarray):
             out = np.clip(input, self.min, self.max)
         else:
             out = min(self.max, max(input, self.min))
         return [out]
 
 
 # ------------------------------------------------------------------------ #
 
 # TODO can have multiple outputs: pass in a tuple of functions, return a tuple
 class Function(FunctionBlock):
-    """
+    r"""
     :blockname:`FUNCTION`
 
-    .. table::
-       :align: left
+    Python function.
+
+    :inputs: N
+    :outputs: M
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - i
+            - any
+            - :math:`x_i`
+        *   - Output
+            - j
+            - any
+            - :math:`f_j(x_0, \ldots, x_{N-1})`
+
+    Inputs to the block are passed as separate arguments to the function.
+    Programmatic ositional or keyword arguments can also be passed to the function.
+
+    A block with one output port that sums its two input ports is::
+
+        func = bd.FUNCTION(lambda u1, u2: u1+u2, nin=2)
+
+    A block with a function that takes two inputs and has two additional arguments::
 
-    +------------+---------+---------+
-    | inputs     | outputs |  states |
-    +------------+---------+---------+
-    | nin        | nout    | 0       |
-    +------------+---------+---------+
-    | any        | any     |         |
-    +------------+---------+---------+
+        def myfun(u1, u2, param1, param2):
+            pass
 
+        FUNCTION(myfun, nin=2, args=(p1,p2))
+
+    If we need access to persistent (static) data, to keep some state::
+
+        def myfun(u1, u2, param1, param2, state):
+            pass
+
+        func = bd.FUNCTION(myfun, nin=2, args=(p1,p2), persistent=True)
+
+    where a dictionary is passed in as the last argument and which is kept from call to call.
+
+    A block with a function that takes two inputs and additional keyword arguments::
+
+        def myfun(u1, u2, param1=1, param2=2, param3=3, param4=4):
+            pass
+
+        func = bd.FUNCTION(myfun, nin=2, kwargs=dict(param2=7, param3=8))
+
+    A block with two inputs and two outputs, the outputs are defined by two lambda
+    functions with the same inputs::
+
+        FUNCTION( [ lambda x, y: x_t, lambda x, y: x* y])
+
+    A block with two inputs and two outputs, the outputs are defined by a
+    single function which returns a list::
+
+        def myfun(u1, u2):
+            return [ u1+u2, u1*u2 ]
+
+        func = bd.FUNCTION( myfun, nin=2, nout=2)
     """
 
     nin = -1
     nout = -1
 
     def __init__(
         self,
@@ -385,90 +561,28 @@
         persistent: bool = False,
         fargs: list = None,
         fkwargs: dict = None,
         **blockargs,
     ):
 
         """
-        Python function.
-
-        :param func: A function or lambda, or list thereof, defaults to None
+        :param func: function or lambda, or list thereof, defaults to None
         :type func: callable or sequence of callables, optional
         :param nin: number of inputs, defaults to 1
         :type nin: int, optional
         :param nout: number of outputs, defaults to 1
         :type nout: int, optional
         :param persistent: pass in a reference to a dictionary instance to hold persistent state, defaults to False
         :type persistent: bool, optional
         :param fargs: extra positional arguments passed to the function, defaults to []
         :type fargs: list, optional
         :param fkwargs: extra keyword arguments passed to the function, defaults to {}
         :type fkwargs: dict, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict, optional
-        :return: A FUNCTION block
-        :rtype: A Function instance
-
-        Inputs to the block are passed as separate arguments to the function.
-        Programmatic ositional or keyword arguments can also be passed to the function.
-
-        A block with one output port that sums its two input ports is::
-
-            FUNCTION(lambda u1, u2: u1+u2, nin=2)
-
-        A block with a function that takes two inputs and has two additional arguments::
-
-            def myfun(u1, u2, param1, param2):
-                pass
-
-            FUNCTION(myfun, nin=2, args=(p1,p2))
-
-        If we need access to persistent (static) data, to keep some state::
-
-            def myfun(u1, u2, param1, param2, state):
-                pass
-
-            FUNCTION(myfun, nin=2, args=(p1,p2), persistent=True)
-
-        where a dictionary is passed in as the last argument and which is kept from call to call.
-
-        A block with a function that takes two inputs and additional keyword arguments::
-
-            def myfun(u1, u2, param1=1, param2=2, param3=3, param4=4):
-                pass
-
-            FUNCTION(myfun, nin=2, kwargs=dict(param2=7, param3=8))
-
-        A block with two inputs and two outputs, the outputs are defined by two lambda
-        functions with the same inputs::
-
-            FUNCTION( [ lambda x, y: x_t, lambda x, y: x* y])
-
-        A block with two inputs and two outputs, the outputs are defined by a
-        single function which returns a list::
-
-            def myfun(u1, u2):
-                return [ u1+u2, u1*u2 ]
-
-            FUNCTION( myfun, nin=2, nout=2)
-
-        For example::
-
-            func = bd.FUNCTION(myfun, args)
-
-        If inputs are specified then connections are automatically made and
-        are assigned to sequential input ports::
-
-            func = bd.FUNCTION(myfun, block1, block2, args)
-
-        is equivalent to::
-
-            func = bd.FUNCTION(myfun, args)
-            bd.connect(block1, func[0])
-            bd.connect(block2, func[1])
         """
         if func is None:
             raise ValueError("function is not defined")
 
         super().__init__(nin=nin, nout=nout, **blockargs)
 
         if fargs is None:
@@ -486,48 +600,51 @@
                 if fkwargs is None:
                     # we can check the number of arguments
                     n = len(inspect.signature(func).parameters)
                     if persistent:
                         n -= 1  # discount dict if used
                     if nin + len(fargs) != n:
                         raise ValueError(
-                            f"argument count mismatch: function has {n} args, dict={dict}, nin={nin}"
+                            f"argument count mismatch: function has {n} args,"
+                            f" dict={dict}, nin={nin}"
                         )
         elif callable(func):
             if len(fkwargs) == 0:
                 # we can check the number of arguments
                 n = len(inspect.signature(func).parameters)
                 if persistent:
                     n -= 1  # discount dict if used
                 if nin + len(fargs) != n:
                     raise ValueError(
-                        f"argument count mismatch: function has {n} args, dict={dict}, nin={nin}"
+                        f"argument count mismatch: function has {n} args, dict={dict},"
+                        f" nin={nin}"
                     )
             # self.nout = nout
 
         self.func = func
         if persistent:
             self.userdata = dict()
             fargs += (self.userdata,)
         else:
             self.userdata = None
         self.args = fargs
         self.kwargs = fkwargs
 
-    def start(self, state=None):
-        super().start()
+    def start(self, simstate):
+        super().start(simstate)
         if self.userdata is not None:
             self.userdata.clear()
             print("clearing user data")
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
+
         if callable(self.func):
             # single function
             try:
-                val = self.func(*self.inputs, *self.args, **self.kwargs)
+                val = self.func(*inports, *self.args, **self.kwargs)
             except TypeError:
                 raise RuntimeError(
                     "Function invocation failed, check number of arguments"
                 ) from None
             if isinstance(val, (list, tuple)):
                 if len(val) != self.nout:
                     raise RuntimeError(
@@ -541,15 +658,15 @@
                     )
                 return [val]
         else:
             # list of functions
             out = []
             for f in self.func:
                 try:
-                    val = f(*self.inputs, *self.args, **self.kwargs)
+                    val = f(*inports, *self.args, **self.kwargs)
                 except TypeError:
                     raise RuntimeError(
                         "Function invocation failed, check number of arguments"
                     ) from None
                 out.append(val)
             return out
 
@@ -557,24 +674,65 @@
 # ------------------------------------------------------------------------ #
 
 
 class Interpolate(FunctionBlock):
     """
     :blockname:`INTERPOLATE`
 
-    .. table::
-       :align: left
+    Interpolate signal.
+
+    :inputs: 1
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
 
-    +------------+---------+---------+
-    | inputs     | outputs |  states |
-    +------------+---------+---------+
-    | 0 or 1     | 1       | 0       |
-    +------------+---------+---------+
-    | float      | any     |         |
-    +------------+---------+---------+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - 0
+            - int, float
+            - :math:`x`
+        *   - Output
+            - 0
+            - float
+            - :math:`f(x)`
+
+    Interpolate a scalar function of a scalar.
+
+    A simple triangle function with domain [0,10] and range [0,1] can be
+    defined by::
+
+        interp = bd.INTERPOLATE(x=(0,5,10), y=(0,1,0))
+
+    We might also express this as a list of 2D-coordinates::
+
+        interp = bd.INTERPOLATE(xy=[(0,0), (5,1), (10,0)])
+
+    .. plot::
+
+        import matplotlib.pyplot as plt
+        plt.plot([0, 5, 10], 
+                 [0, 1, 0], lw=2)
+        plt.grid(True)
+        plt.xlabel("in[0]")
+        plt.ylabel("out[0]")
+
+    The data can also be expressed as Numpy arrays.  If that is the case,
+    the interpolation function can be vector valued. ``x`` has a shape of
+    (N,1) and ``y`` has a shape of (N,M).  Alternatively ``xy`` has a shape
+    of (N,M+1) and the first column is the x-data.
+
+    :note: if ``time=True``.  In this case the block has no
+        input ports and is a ``Source`` not a ``Function`` block.
+
+    :seealso: :func:`scipy.interpolate.interp1d`
     """
 
     nin = -1
     nout = 1
 
     def __init__(
         self,
@@ -582,52 +740,26 @@
         y: Union[list, tuple, np.ndarray] = None,
         xy: np.ndarray = None,
         time: bool = False,
         kind: str = "linear",
         **blockargs,
     ):
         """
-        Interpolate signal.
-
         :param x: x-values of function, defaults to None
         :type x: array_like, shape (N,) optional
         :param y: y-values of function, defaults to None
         :type y: array_like, optional
         :param xy: combined x- and y-values of function, defaults to None
         :type xy: array_like, optional
         :param time: x new is simulation time, defaults to False
         :type time: bool, optional
         :param kind: interpolation method, defaults to 'linear'
         :type kind: str, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: An INTERPOLATE block
-        :rtype: An Interpolate instance
-
-        Interpolate the input signal using to a piecewise function.
-
-        A simple triangle function with domain [0,10] and range [0,1] can be
-        defined by::
-
-            INTERPOLATE(x=(0,5,10), y=(0,1,0))
-
-        We might also express this as a list of 2D-coordinats::
-
-            INTERPOLATE(xy=[(0,0), (5,1), (10,0)])
-
-        The data can also be expressed as Numpy arrays.  If that is the case,
-        the interpolation function can be vector valued. ``x`` has a shape of
-        (N,1) and ``y`` has a shape of (N,M).  Alternatively ``xy`` has a shape
-        of (N,M+1) and the first column is the x-data.
-
-        The input to the interpolator comes from:
-
-        - Input port 0
-        - Simulation time, if ``time=True``.  In this case the block has no
-          input ports and is a ``Source`` not a ``Function``.
         """
         self.time = time
         if time:
             nin = 0
             self.blockclass = "source"
         else:
             nin = 1
@@ -648,26 +780,29 @@
                 print(x, y)
             elif isinstance(xy, np.ndarray):
                 x = xy[:, 0]
                 y = xy[:, 1:]
         self.f = scipy.interpolate.interp1d(x=x, y=y, kind=kind, axis=0)
         self.x = x
 
-    def start(self, state, **blockargs):
-        if self.time:
-            assert self.x[0] >= 0, "interpolation not defined for t<0"
-            if self.x[-1] is np.inf:
-                self.x[-1] = state.T
-            assert self.x[-1] >= state.T, "interpolation not defined for t>T"
+    def start(self, simstate, **blockargs):
+        super().start(simstate)
+
+        if simstate is not None:
+            if self.time:
+                assert self.x[0] >= 0, "interpolation not defined for t<0"
+                if self.x[-1] is np.inf:
+                    self.x[-1] = simstate.T
+                assert self.x[-1] >= simstate.T, "interpolation not defined for t>T"
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
         if self.time:
             xnew = t
         else:
-            xnew = self.inputs[0]
+            xnew = inports[0]
         return [self.f(xnew)]
 
 
 if __name__ == "__main__":  # pragma: no cover
 
     from pathlib import Path
```

### Comparing `bdsim-1.0.0/bdsim/blocks/sinks.py` & `bdsim-1.1.0/bdsim/blocks/sinks.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,82 +20,82 @@
 # ------------------------------------------------------------------------ #
 
 
 class Print(SinkBlock):
     """
     :blockname:`PRINT`
 
-    .. table::
-       :align: left
+    Print signal.
 
-    +--------+---------+---------+
-    | inputs | outputs |  states |
-    +--------+---------+---------+
-    | 1      | 0       | 0       |
-    +--------+---------+---------+
-    | any    |         |         |
-    +--------+---------+---------+
+    :inputs: 1
+    :outputs: 0
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - 0
+            - any
+            - :math:`x`
+
+    Creates a console print block which displays the value of the input signal
+    at each simulation time step. The display format is like::
+
+        PRINT(print.0 @ t=0.100) [-1.0 0.2]
+
+    and includes the block name, time, and the formatted value.
+
+    The numerical formatting of the signal is controlled by ``fmt``:
+
+    - if not provided, ``str()`` is used to format the signal
+    - if provided:
+
+        - a scalar is formatted by the ``fmt.format()``
+        - a NumPy array is formatted by ``fmt.format()`` applied to every
+          element
+
+    Examples::
+
+        bd.PRINT(name="X")  # block name appears in the printed text
+        bd.PRINT(fmt="{:.1f}") # print with explicit format
+
+    .. note::
+        - By default writes to stdout
+        - The output is cleaner if progress bar printing is disabled using the
+          ``-p`` command line option.
     """
 
     nin = 1
     nout = 0
 
     def __init__(self, fmt=None, file=None, **blockargs):
         """
-        Print signal.
-
         :param fmt: Format string, defaults to None
         :type fmt: str, optional
         :param file: file to write data to, defaults to None
         :type file: file object, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
         :return: A PRINT block
         :rtype: Print instance
-
-        Creates a console print block which displays the value of a signal
-        at each simulation time step. The display format is like::
-
-            PRINT(print.0 @ t=0.100) [-1.0 0.2]
-
-        and includes the block name, time, and the formatted value.
-
-        The numerical formatting of the signal is controlled by ``fmt``:
-
-        - if not provided, ``str()`` is used to format the signal
-        - if provided:
-            - a scalar is formatted by the ``fmt.format()``
-            - a NumPy array is formatted by ``fmt.format()`` applied to every
-              element
-
-        Examples::
-
-            pr = bd.PRINT()     # create PRINT block
-            bd.connect(x, inputs=pr)   # its input comes from x
-
-            bd.PRINT(x)         # create PRINT block with input from x
-
-            bd.PRINT(x, name='X')  # block name appears in the printed text
-
-            bd.PRINT(x, fmt="{:.1f}") # print with explicit format
-
-        .. note::
-            - By default writes to stdout
-            - The output is cleaner if progress bar printing is disabled.
-
         """
         super().__init__(**blockargs)
         self.format = fmt
         self.file = file
 
         # TODO format can be a string or function
 
-    def step(self, state=None):
-        prefix = "{:12s}".format("PRINT({:s} (t={:.3f})".format(self.name, state.t))
-        value = self.inputs[0]
+    def step(self, t, inports):
+        prefix = "{:12s}".format("PRINT({:s} (t={:.3f})".format(self.name, t))
+        value = inports[0]
         if self.format is None:
             # no format string
             if hasattr(value, "strline"):
                 print(prefix, value.strline(), file=self.file)
             else:
                 print(prefix, str(value), file=self.file)
         else:
@@ -115,160 +115,184 @@
 # ------------------------------------------------------------------------ #
 
 
 class Stop(SinkBlock):
     """
     :blockname:`STOP`
 
-    .. table::
-       :align: left
+    Conditionally stop simulation.
+
+    :inputs: 1
+    :outputs: 0
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - 0
+            - any
+            - :math:`x`
 
-    +--------+---------+---------+
-    | inputs | outputs |  states |
-    +--------+---------+---------+
-    | 1      | 0       | 0       |
-    +--------+---------+---------+
-    | any    |         |         |
-    +--------+---------+---------+
+    Conditionally stop the simulation if the input :math:`x` is:
+
+    - bool type and True
+    - numeric type and > 0
+
+    If ``func`` is provided, then it is applied to the block input
+    and if it returns True the simulation is stopped.
     """
 
     nin = 1
     nout = 0
 
     def __init__(self, func=None, **blockargs):
         """
-        Conditional simulation stop.
-
         :param func: evaluate stop condition, defaults to None
         :type func: callable, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: A STOP block
-        :rtype: Stop instance
-
-        Conditionally stop the simulation if the input is:
-
-        - bool type and True
-        - numeric type and > 0
-
-        If ``func`` is provided, then it is applied to the block input
-        and if it returns True the simulation is stopped.
         """
         super().__init__(**blockargs)
 
         if func is not None and not callable(func):
             raise TypeError("argument must be a callable")
         self.stopfunc = func
 
-    def step(self, state=None):
-        value = self.inputs[0]
+    def start(self, simstate):
+        self._simstate = simstate
+
+    def step(self, t, inports):
+        value = inports[0]
+
         if self.stopfunc is not None:
             value = self.stopfunc(value)
 
         stop = False
         if isinstance(value, bool):
             stop = value
         else:
             try:
                 stop = value > 0
             except:
                 raise RuntimeError("bad input type to stop block")
 
-        # we signal stop condition by setting state.stop to the block calling
+        # we signal stop condition by setting simstate.stop to the block calling
         # the stop
         if stop:
-            state.stop = self
+            self._simstate.stop = self
 
 
 # ------------------------------------------------------------------------ #
 
 
 class Null(SinkBlock):
     """
     :blockname:`NULL`
 
-    .. table::
-       :align: left
+    Discard signal.
 
-    +--------+---------+---------+
-    | inputs | outputs |  states |
-    +--------+---------+---------+
-    | N      | 0       | 0       |
-    +--------+---------+---------+
-    | any    |         |         |
-    +--------+---------+---------+
+    :inputs: N
+    :outputs: 0
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - i
+            - any
+            - :math:`x_i`
+
+    Create a sink block with arbitrary number of input ports that discards
+    all data, like ``/dev/null``. Useful for testing.
+
+    .. note:: ``bdsim`` issues a warning for unconnected outputs but execution can continue.
     """
 
     nin = -1
     nout = 0
 
     def __init__(self, nin=1, **blockargs):
         """
-        Discard signal.
-
         :param nin: number of input ports, defaults to 1
         :type nin: int, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: A NULL block
-        :rtype: Null instance
-
-        Create a sink block with arbitrary number of input ports that discards
-        all data.  Useful for testing.
-
         """
         super().__init__(nin=nin, **blockargs)
 
 
 # ------------------------------------------------------------------------ #
 
 
 class Watch(SinkBlock):
     """
     :blockname:`WATCH`
 
-    .. table::
-       :align: left
+    Watch a signal.
+
+    :inputs: N
+    :outputs: 0
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Input
+            - i
+            - any
+            - :math:`x_i`
+
+    Causes the output ports connected to this block's input ports :math:`x_i` to be
+    logged during the simulation run. Equivalent to adding it as the ``watch=`` argument
+    to ``bdsim.run``.
+
+    For example::
+
+        step = bd.STEP(5)
+        ramp = bd.RAMP()
+        watch = bd.WATCH(2) # watch 2 ports
+        watch[0] = step
+        watch[1] = ramp
 
-    +--------+---------+---------+
-    | inputs | outputs |  states |
-    +--------+---------+---------+
-    | N      | 0       | 0       |
-    +--------+---------+---------+
-    | 1      |         |         |
-    +--------+---------+---------+
+    :seealso: :method:`BDSim.run`
     """
 
     nin = 1
     nout = 0
 
     def __init__(self, **blockargs):
         """
-        Watch a signal.
-
+        :param nin: number of input ports, defaults to 1
+        :type nin: int, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: A NULL block
-        :rtype: Null instance
-
-        Causes the input signal to be logged during the
-        simulation run.  Equivalent to adding it as the ``watch=`` argument
-        to ``bdsim.run``.
-
-        :seealso: :method:`BDSim.run`
         """
         super().__init__(**blockargs)
 
-    def start(self, state=None):
+    def start(self, simstate):
         # called at start of simulation, add this block to the watchlist
         plug = self.sources[0]  # start plug for input wire
 
         # append to the watchlist, bdsim.run() will do the rest
-        state.watchlist.append(plug)
-        state.watchnamelist.append(str(plug))
+        simstate.watchlist.append(plug)
+        simstate.watchnamelist.append(str(plug))
 
 
 if __name__ == "__main__":  # pragma: no cover
 
     from pathlib import Path
 
     exec(open(Path(__file__).parent.parent.parent / "tests" / "test_sinks.py").read())
```

### Comparing `bdsim-1.0.0/bdsim/blocks/sources.py` & `bdsim-1.1.0/bdsim/blocks/sources.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,113 +12,156 @@
 from bdsim.components import SourceBlock, EventSource
 
 # ------------------------------------------------------------------------ #
 class Constant(SourceBlock):
     """
     :blockname:`CONSTANT`
 
-    .. table::
-       :align: left
+    Constant value.
 
-    +--------+---------+---------+
-    | inputs | outputs |  states |
-    +--------+---------+---------+
-    | 0      | 1       | 0       |
-    +--------+---------+---------+
-    |        | float,  |         |
-    |        | A(N,)   |         |
-    +--------+---------+---------+
+    :inputs: 0
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Output
+            - 0
+            - any
+            - constant ``value``
+
+    The output value is a constant and can be any
+    Python type, for example float, list or Numpy ndarray.
     """
 
     nin = 0
     nout = 1
 
     def __init__(self, value=0, **blockargs):
         """
-        Constant value.
-
         :param value: the constant, defaults to 0
         :type value: any, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: a CONSTANT block
-        :rtype: Constant instance
-
-        This block has only one output port, but the value can be any
-        Python type, for example float, list or Numpy ndarray.
         """
         super().__init__(**blockargs)
 
         if isinstance(value, (tuple, list)):
             value = np.array(value)
         self.value = value
 
         self.add_param("value")
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
         return [self.value]
 
 
 # ------------------------------------------------------------------------ #
 
 
 class Time(SourceBlock):
     """
     :blockname:`TIME`
 
-    .. table::
-       :align: left
+    Simulation time.
+
+    :inputs: 0
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
 
-    +--------+---------+---------+
-    | inputs | outputs |  states |
-    +--------+---------+---------+
-    | 0      | 1       | 0       |
-    +--------+---------+---------+
-    |        | float   |         |
-    +--------+---------+---------+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Output
+            - 0
+            - float
+            - :math:`t`
+
+    Outputs the current simulation time.
+
+    For example::
+
+        time = bd.TIME()
     """
 
     nin = 0
     nout = 1
 
     def __init__(self, value=None, **blockargs):
         """
-        Simulation time.
-
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: a TIME block
-        :rtype: Time instance
-
-        The block has only one output port which is the current simulation time.
-
         """
         super().__init__(**blockargs)
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
         return [t]
 
 
 # ------------------------------------------------------------------------ #
 
 
 class WaveForm(SourceBlock, EventSource):
     """
     :blockname:`WAVEFORM`
 
-    .. table::
-       :align: left
+    Waveform generator.
+
+    :inputs: 0
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Output
+            - 0
+            - float
+            - :math:`y(t)`
+
+    A general waveform generator.  For example::
+
+        wave = bd.WAVEFORM(wave='sine', freq=2)   # 2Hz sine wave varying from -1 to 1
+        wave = bd.WAVEFORM(wave='square', freq=2, unit='rad/s') # 2rad/s square wave varying from -1 to 1
+
+    The minimum and maximum values of the waveform are given by default in
+    terms of amplitude and offset. The signals are symmetric about the offset
+    value. For example::
+
+        wave = bd.WAVEFORM(wave='sine') # varies between -1 and +1
+        wave = bd.WAVEFORM(wave='sine', amplitude=2) # varies between -2 and +2
+        wave = bd.WAVEFORM(wave='sine', offset=1) # varies between 0 and +2
+        wave = bd.WAVEFORM(wave='sine', amplitude=2, offset=1) # varies between -1 and +3
+
+    Alternatively we can specify the minimum and maximum values which override
+    amplitude and offset::
 
-    +--------+---------+---------+
-    | inputs | outputs |  states |
-    +--------+---------+---------+
-    | 0      | 1       | 0       |
-    +--------+---------+---------+
-    |        | float   |         |
-    +--------+---------+---------+
+        wave = bd.WAVEFORM(wave='triangle', min=0, max=5) # varies between 0 and +5
+
+    At time 0 the sine and triangle wave are zero and increasing, and the
+    square wave has its first rise.  We can specify a phase shift with
+    a number in the range [0,1] where 1 corresponds to one cycle.
+
+    .. note:: For discontinuous signals (square, triangle) the block declares
+        events for every discontinuity.
+
+    :seealso: :meth:`declare_events`
     """
 
     nin = 0
     nout = 1
 
     def __init__(
         self,
@@ -130,16 +173,14 @@
         offset=0,
         min=None,
         max=None,
         duty=0.5,
         **blockargs,
     ):
         """
-        Waveform as function of time.
-
         :param wave: type of waveform to generate, one of: 'sine', 'square' [default], 'triangle'
         :type wave: str, optional
         :param freq: frequency, defaults to 1
         :type freq: float, optional
         :param unit: frequency unit, one of: 'rad/s', 'Hz' [default]
         :type unit: str, optional
         :param amplitude: amplitude, defaults to 1
@@ -152,46 +193,15 @@
         :type min: float, optional
         :param max: maximum value, defaults to None
         :type max: float, optional
         :param duty: duty cycle for square wave in range [0,1], defaults to 0.5
         :type duty: float, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: a WAVEFORM block
-        :rtype: WaveForm instance
-
-        Create a waveform generator block.
-
-        Examples::
-
-            WAVEFORM(wave='sine', freq=2)   # 2Hz sine wave varying from -1 to 1
-            WAVEFORM(wave='square', freq=2, unit='rad/s') # 2rad/s square wave varying from -1 to 1
-
-        The minimum and maximum values of the waveform are given by default in
-        terms of amplitude and offset. The signals are symmetric about the offset
-        value. For example::
-
-            WAVEFORM(wave='sine') varies between -1 and +1
-            WAVEFORM(wave='sine', amplitude=2) varies between -2 and +2
-            WAVEFORM(wave='sine', offset=1) varies between 0 and +2
-            WAVEFORM(wave='sine', amplitude=2, offset=1) varies between -1 and +3
-
-        Alternatively we can specify the minimum and maximum values which override
-        amplitude and offset::
 
-            WAVEFORM(wave='triangle', min=0, max=5) varies between 0 and +5
-
-        At time 0 the sine and triangle wave are zero and increasing, and the
-        square wave has its first rise.  We can specify a phase shift with
-        a number in the range [0,1] where 1 corresponds to one cycle.
-
-        .. note:: For discontinuous signals (square, triangle) the block declares
-            events for every discontinuity.
-
-        :seealso :meth:`declare_events`
         """
         super().__init__(**blockargs)
 
         assert 0 < duty < 1, "duty must be in range [0,1]"
 
         if wave in ("square", "triangle", "sine"):
             self.wave = wave
@@ -215,33 +225,36 @@
         if 0 <= duty <= 1:
             self.duty = duty
         else:
             raise ValueError("duty out of range")
         self.amplitude = amplitude
         self.offset = offset
 
-    def start(self, state=None):
+    def start(self, simstate):
+        super().start(simstate)
+
         if self.wave == "square":
             t1 = self.phase / self.freq
             t2 = (self.duty + self.phase) / self.freq
         elif self.wave == "triangle":
             t1 = (0.25 + self.phase) / self.freq
             t2 = (0.75 + self.phase) / self.freq
         else:
             return
 
         # t1 < t2
         T = 1.0 / self.freq
-        while t1 < self.bd.simstate.T:
-            self.bd.simstate.declare_event(self, t1)
-            self.bd.simstate.declare_event(self, t2)
-            t1 += T
-            t2 += T
+        if simstate is not None:
+            while t1 < simstate.T:
+                simstate.declare_event(self, t1)
+                simstate.declare_event(self, t2)
+                t1 += T
+                t2 += T
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
         T = 1.0 / self.freq
         phase = (t * self.freq - self.phase) % 1.0
 
         # define all signals in the range -1 to 1
         if self.wave == "square":
             if phase < self.duty:
                 out = 1
@@ -268,124 +281,165 @@
 # ------------------------------------------------------------------------ #
 
 
 class Piecewise(SourceBlock, EventSource):
     """
     :blockname:`PIECEWISE`
 
-    .. table::
-       :align: left
+    Piecewise constant signal.
+
+    :inputs: 0
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Output
+            - 0
+            - float
+            - :math:`y(t)`
+
+    Generate a signal that is a piecewise constant function of time.  This is described
+    as a series of 2-tuples (time, value).  The output value is taken from the active
+    tuple, that is, the latest one in the list whose time is no greater than simulation
+    time.
+
+    The tuples can be provided in two different ways.  Firstly, a form convenient for
+    Python programming::
 
-    +--------+---------+---------+
-    | inputs | outputs |  states |
-    +--------+---------+---------+
-    | 0      | 1       | 0       |
-    +--------+---------+---------+
-    |        | float   |         |
-    +--------+---------+---------+
+        steering = bd.PIECEWISE((0,0), (2, 0.5), (3,0), (4,-0.5), (5,0))
+
+    Secondly, in a form that can be used from ``bdsim`` where we explicitly pass
+    in a list in a way that can be represented in a JSON file::
+
+        steering = bd.PIECEWISE(seq=[(0,0), (3, 0.5), (4,0), (5,-0.5), (6,0)])
+
+    .. plot::
+
+        import matplotlib.pyplot as plt
+        plt.plot([0, 2, 2,   3,   3, 4,   4,   5,   5, 5.2], 
+                 [0, 0, 0.5, 0.5, 0, 0, -0.5, -0.5, 0, 0], lw=2)
+        plt.grid(True)
+
+    .. note::
+        - The tuples must be ordered by monotonically increasing time.
+        - There is no default initial value, the list should contain
+          a tuple with time zero otherwise the output will be undefined.
+        - The 2-tuples can
+
+    .. note:: The block declares an event for the start of each segment.
+
+    :seealso: :meth:`declare_events`
     """
 
     nin = 0
     nout = 1
 
-    def __init__(self, *seq, **blockargs):
+    def __init__(self, *args, seq=None, **blockargs):
         """
-        Piecewise constant signal.
-
         :param seq: sequence of time, value pairs
-        :type seq: list of 2-tuples
+        :type seq: list of 2-element iterables
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: a PIECEWISE block
-        :rtype: Piecewise instance
-
-        Outputs a piecewise constant function of time.  This is described as
-        a series of 2-tuples (time, value).  The output value is taken from the
-        active tuple, that is, the latest one in the list whose time is no greater
-        than simulation time.
-
-        .. note::
-            - The tuples must be order by monotonically increasing time.
-            - There is no default initial value, the list should contain
-              a tuple with time zero otherwise the output will be undefined.
-
-        .. note:: The block declares an event for the start of each segment.
 
-        :seealso: :meth:`declare_events`
         """
         super().__init__(**blockargs)
 
+        if len(args) > 0:
+            seq = args
+
         self.t = [x[0] for x in seq]
         self.y = [x[1] for x in seq]
 
-    def start(self, state=None):
-        for t in self.t:
-            state.declare_event(self, t)
+    def start(self, simstate):
+        super().start(simstate)
+
+        if simstate is not None:
+            for t in self.t:
+                simstate.declare_event(self, t)
 
-    def output(self, t):
+    def output(self, t, inports, x):
         i = sum([1 if t >= _t else 0 for _t in self.t]) - 1
         out = self.y[i]
         # print(out)
         return [out]
 
 
 # ------------------------------------------------------------------------ #
 
 
 class Step(SourceBlock, EventSource):
     """
     :blockname:`STEP`
 
-    .. table::
-       :align: left
+    Step signal.
+
+    :inputs: 0
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Output
+            - 0
+            - float
+            - :math:`y(t)`
+
+    Generate a step signal that transitions from the value ``off`` to ``on`` when time
+    equals ``T``.
+
+    Example:
+
+        step = bd.STEP(2, off=-1, on=1)
+
+    .. plot::
 
-    +--------+---------+---------+
-    | inputs | outputs |  states |
-    +--------+---------+---------+
-    | 0      | 1       | 0       |
-    +--------+---------+---------+
-    |        | float   |         |
-    +--------+---------+---------+
+        import matplotlib.pyplot as plt
+        plt.plot([0, 2, 2, 5], [-1, -1, 1, 1], lw=2)
+        plt.grid(True)
+
+    .. note:: The block declares an event for the step time.
+
+    :seealso: :meth:`declare_events`
     """
 
     nin = 0
     nout = 1
 
     def __init__(self, T=1, off=0, on=1, **blockargs):
         """
-        Step signal.
-
         :param T: time of step, defaults to 1
         :type T: float, optional
         :param off: initial value, defaults to 0
         :type off: float, optional
         :param on: final value, defaults to 1
         :type on: float, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: a STEP block
-        :rtype: Step
-
-        Output a step signal that transitions from the value ``off`` to ``on``
-        when time equals ``T``.
-
-        .. note:: The block declares an event for the step time.
-
-        :seealso: :meth:`declare_events`
         """
         super().__init__(**blockargs)
 
         self.T = T
         self.off = off
         self.on = on
 
-    def start(self, state=None):
-        state.declare_event(self, self.T)
+    def start(self, simstate):
+        simstate.declare_event(self, self.T)
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
         if t >= self.T:
             out = self.on
         else:
             out = self.off
 
         # print(out)
         return [out]
@@ -394,62 +448,75 @@
 # ------------------------------------------------------------------------ #
 
 
 class Ramp(SourceBlock, EventSource):
     """
     :blockname:`RAMP`
 
-    .. table::
-       :align: left
+    Ramp signal.
+
+    :inputs: 0
+    :outputs: 1
+    :states: 0
+
+    .. list-table::
+        :header-rows: 1
+
+        *   - Port type
+            - Port number
+            - Types
+            - Description
+        *   - Output
+            - 0
+            - float
+            - :math:`y(t)`
+
+    Generate a signal that starts increasing from the value ``off`` when time equals
+    ``T`` linearly with time, with a gradient of ``slope``.
 
-    +--------+---------+---------+
-    | inputs | outputs |  states |
-    +--------+---------+---------+
-    | 0      | 1       | 0       |
-    +--------+---------+---------+
-    |        | float   |         |
-    +--------+---------+---------+
+    Example:
+
+        step = bd.RAMP(2, off=-1, slope=2/3, T=2)
+
+    .. plot::
+
+        import matplotlib.pyplot as plt
+        plt.plot([0, 2, 5], [-1, -1, 5], lw=2)
+        plt.grid(True)
+
+    .. note:: The block declares an event for the ramp start time.
+
+    :seealso: :meth:`declare_event`
     """
 
     nin = 0
     nout = 1
 
     def __init__(self, T=1, off=0, slope=1, **blockargs):
 
         """
-        Ramp signal.
-
         :param T: time of ramp start, defaults to 1
         :type T: float, optional
         :param off: initial value, defaults to 0
         :type off: float, optional
         :param slope: gradient of slope, defaults to 1
         :type slope: float, optional
         :param blockargs: |BlockOptions|
         :type blockargs: dict
-        :return: a RAMP block
-        :rtype: Ramp
-
-        Output a ramp signal that starts increasing from the value ``off``
-        when time equals ``T`` linearly with time, with a gradient of ``slope``.
-
-        .. note:: The block declares an event for the ramp start time.
-
-        :seealso: :method:`declare_event`
         """
         super().__init__(**blockargs)
 
         self.T = T
         self.off = off
         self.slope = slope
 
-    def start(self, state=None):
-        state.declare_event(self, self.T)
+    def start(self, simstate):
+        simstate.declare_event(self, self.T)
 
-    def output(self, t=None):
+    def output(self, t, inports, x):
         if t >= self.T:
             out = self.off + self.slope * (t - self.T)
         else:
             out = self.off
 
         # print(out)
         return [out]
```

### Comparing `bdsim-1.0.0/bdsim/blocks/tex2icon.py` & `bdsim-1.1.0/bdsim/tex2icon.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,21 +6,30 @@
 import sys
 import subprocess
 import io
 from PIL import Image, ImageOps
 from pathlib import Path
 import numpy as np
 
-latex_template = """\\documentclass{{article}}
+latex_template_rvc = """\\documentclass{{article}}
 \\thispagestyle{{empty}}
 \\usepackage{{graphicx}} % \\scalebox
 \\input{{rvc-notation}}
 \\begin{{document}}
 ${tex}$
-\\end{{document}}"""
+\\end{{document}}
+"""
+
+latex_template_norvc = """\\documentclass{{article}}
+\\thispagestyle{{empty}}
+\\usepackage{{graphicx}} % \\scalebox
+\\begin{{document}}
+${tex}$
+\\end{{document}}
+"""
 
 IMSIZE = 250
 
 
 def main():
     des = "tex2icon, create bdedit icons from LaTeX source"
     parser = argparse.ArgumentParser(description=des)
@@ -32,40 +41,70 @@
     )
     parser.add_argument(
         "-r", help="resolution (dpi)", type=int, default=100, metavar='"resolution"'
     )
     parser.add_argument(
         "-o", help="The output filename.", default="icon.png", metavar="filename"
     )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        help="be verbose.",
+        default=False,
+        action="store_const",
+        const=True,
+        metavar="verbose",
+    )
     args = parser.parse_args()
 
+    # look for rvc-notation on LaTeX path, see https://github.com/petercorke/rvc-notation
+    try:
+        subprocess.run(
+            ["kpsewhich", "rvc-notation.tex"], stdout=subprocess.DEVNULL, check=True
+        )
+        latex_template = latex_template_rvc
+        if args.verbose:
+            print("RVC macros found")
+    except subprocess.CalledProcessError:
+        latex_template = latex_template_norvc
+        if args.verbose:
+            print("RVC macros not found")
+
+    # build the icon
     try:
         # create LaTeX source file in temp file
         source_filename = tempfile.mkstemp(suffix=".tex", text=True)
         os.write(source_filename[0], latex_template.format(tex=args.t).encode("utf8"))
         os.close(source_filename[0])
 
         # run pdflatex, results go to temp folder
         source_path = Path(source_filename[1])
+        if args.verbose:
+            print("run pdflatex on ", source_path)
         subprocess.run(
             ["pdflatex", "-output-directory", source_path.parent, source_path.name],
             stdout=subprocess.DEVNULL,
+            stdin=subprocess.DEVNULL,
+            check=True,
         )
-        # print(source_filename[1])
 
         # run pdfcrop to remove all that white space
+        if args.verbose:
+            print("run pdfcrop")
         subprocess.run(
-            ["pdfcrop", source_path.with_suffix(".pdf")], stdout=subprocess.DEVNULL
+            ["pdfcrop", source_path.with_suffix(".pdf")],
+            check=True,
+            stdout=subprocess.DEVNULL,
         )
 
         # get path to -crop.pdf file
         cropped_filename = source_path.with_name(
             source_path.stem + "-crop"
         ).with_suffix(".pdf")
-        # print(cropped_filename)
+        print(cropped_filename)
 
         # run gs to convert cropped pdf to png file
         # user can control the resolution to scale the icon
         gs_args = [
             "/usr/local/bin/gs",
             "-sDEVICE=pngalpha",
             "-sOutputFile=%stdout",
@@ -73,14 +112,16 @@
             "-dBATCH",
             "-dNOPAUSE",
             "-q",
             "-dGraphicsAlphaBits=4",
             "-dDOINTERPOLATE",
             str(cropped_filename),
         ]
+        if args.verbose:
+            print("run gs")
         gs = subprocess.Popen(
             gs_args, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL
         )
 
         # read image data from gs into a PIL image
         image = Image.open(gs.stdout)
         gs.stdout.close()
@@ -108,18 +149,22 @@
             icon_rgba[:, :, i] = icon
         icon_rgba[:, :, 3] = np.where(icon == 255, 0, 255)
 
         # convert back to Image and save it
         Image.fromarray(icon_rgba).save(args.o)
         print("icon saved --> ", args.o)
 
-    except (OSError, ValueError):
-        print("exception during processing pipeline")
+    except (OSError, ValueError, subprocess.CalledProcessError):
+        print("exception during processing pipeline, requires: pdflatex, gs, pdfcrop")
 
     # cleanup all the temporary files
     for suffix in (".aux", ".log", ".pdf", ".tex"):
         source_path.with_suffix(suffix).unlink(missing_ok=True)
-    cropped_filename.unlink(missing_ok=True)
+
+    try:
+        cropped_filename.unlink(missing_ok=True)
+    except UnboundLocalError:
+        pass
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bdsim-1.0.0/bdsim/components.py` & `bdsim-1.1.0/bdsim/components.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,83 +7,88 @@
 import math
 from re import S
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import animation
 from collections import UserDict
 
+# decorator for debugging implicit block creation with operator overloading
+def oodebug(func):
+    def wrapper(*args, **kwargs):
+        ret = func(*args, **kwargs)
+        # print(f"{func.__qualname__}{args} --> {ret}")
+        return ret
 
-class BDStruct(UserDict):
+    return wrapper
+
+
+class BDStruct:
     """
-    A dict-like object that allows items to be added by attribute or by key.
+    A simple data container object that allows items to be added by attribute or by
+    index.
 
     For example::
 
-        >>> d = Struct('thing')
-        >>> d.a = 1
-        >>> d['b'] = 2
-        >>> d.a
+        >>> d = BDStruct('thing')
+        >>> d.foo = 1
+        >>> d.foo
         1
-        >>> d['a']
-        1
-        >>> d.b
-        2
-        >>> str(d)
-        "thing {'a': 1, 'b': 2}"
+        >>> d["foo"]
+        ]
+        >>> d["bar"] = 2
+        >>> d.bar
+        >>> d
+        bar   = 2 (int)
+        foo   = 1 (int)
     """
 
-    def __init__(self, name="BDStruct", **kwargs):
-        super().__init__()
-        self.name = name
+    def __init__(self, name="BDStruct2", **kwargs):
+        self._name = name
         for key, value in kwargs.items():
-            self[key] = value
-
-    def __setattr__(self, name, value):
-        # invoked by struct[name] = value
-        if name in ["data", "name"]:
-            super().__setattr__(name, value)
-        else:
-            self.data[name] = value
+            # self.__dict__[key] = value
+            setattr(self, key, value)
 
     def add(self, name, value):
-        self.data[name] = value
-
-    def __getattr__(self, name):
-        # return self.data[name]
-        # some tricks to make this deepcopy safe
-        # https://stackoverflow.com/questions/40583131/python-deepcopy-with-custom-getattr-and-setattr
-        # https://stackoverflow.com/questions/25977996/supporting-the-deep-copy-operation-on-a-custom-class
-        try:
-            return self.data[name]
-        except AttributeError:
-            raise AttributeError("unknown attribute " + name)
+        # self.__dict__[name] = value
+        setattr(self, name, value)
 
     def __repr__(self):
         return str(self)
 
+    def __len__(self):
+        return len([k for k in self.__dict__.keys() if not k.startswith("_")])
+
+    def __getitem__(self, key):
+        return getattr(self, key)
+
+    def __setitem__(self, key, value):
+        setattr(self, key, value)
+
     def __str__(self):
         """
         Display struct as a string
 
         :return: struct in indented string format
         :rtype: str
 
         The struct is rendered with one line per element, and substructures
         are indented.
         """
         rows = []
 
         if len(self) == 0:
             return ""
-        maxwidth = max([len(key) for key in self.keys()])
+        maxwidth = max([len(key) for key in self.__dict__.keys()])
         # if self.name is not None:
         #     rows.append(self.name + '::')
-        for k, v in sorted(self.items(), key=lambda x: x[0]):
+        for k, v in sorted(self.__dict__.items(), key=lambda x: x[0]):
+            if k.startswith("_"):
+                continue
             if isinstance(v, BDStruct):
-                rows.append("{:s}.{:s}::".format(k.ljust(maxwidth), v.name))
+                rows.append("{:s}.{:s}::".format(k.ljust(maxwidth), v._name))
                 rows.append(
                     "\n".join(
                         [" " * (maxwidth + 3) + line for line in str(v).split("\n")]
                     )
                 )
             elif isinstance(v, str):
                 rows.append(
@@ -102,14 +107,20 @@
                     "{:s} = {:s} ({:s})".format(
                         k.ljust(maxwidth), str(v), type(v).__name__
                     )
                 )
 
         return "\n".join(rows)
 
+    def dump(self, outfile):
+        import pickle
+
+        with open(outfile, "wb") as f:
+            pickle.dump(self, f)
+
 
 class OptionsBase:
     """A struct like object for option handling
 
     Maintains an internal dict to keep options and their values.  Some of these
     values, names in the ``_priority`` list are read-only and cannot be changed.
 
@@ -146,15 +157,16 @@
         changes = self.sanity(changes)
         dict = self._dict
         for name, value in changes.items():
             if name not in self._readonly:
                 dict[name] = value
             elif dict[name] != value:
                 print(
-                    f"attempt to programmatically set option {name}={value} is overriden by command line option {name}={dict[name]}, ignored"
+                    f"attempt to programmatically set option {name}={value} is"
+                    f" overriden by command line option {name}={dict[name]}, ignored"
                 )
 
         self._dict = dict
 
     def sanity(self, options):
         return options
 
@@ -301,14 +313,42 @@
 
     def __init__(self, block, port=0, type=None):
 
         self.block = block
         self.port = port
         self.type = type  # start
 
+    def __str__(self):
+        """
+        Display plug details.
+
+        :return: Plug description
+        :rtype: str
+
+        String format::
+
+            bicycle.0[1]
+
+        """
+        return str(self.block) + "[" + str(self.port) + "]"
+
+    def __repr__(self):
+        """
+        Display plug details.
+
+        :return: Plug description
+        :rtype: str
+
+        String format::
+
+            bicycle.0[1]
+
+        """
+        return "Plug/" + self.type + ":" + str(self)
+
     @property
     def isslice(self):
         """
         Test if port number is a slice.
 
         :return: Whether the port is a slice
         :rtype: bool
@@ -365,14 +405,15 @@
 
         If the port is a simple index, eg. ``[2]`` returns 1.
 
         If the port is a slice, eg. ``[0:3]``, returns 3.
         """
         return len(self.portlist)
 
+    @oodebug
     def __rshift__(left, right):
         """
         Overloaded >> operator for implicit wiring.
 
         :param left: A plug to be wired from
         :type left: Plug
         :param right: A block or plug to be wired to
@@ -407,14 +448,15 @@
         # block * plug
         s = left.block.bd
         # assert isinstance(right, Block), 'arguments to * must be blocks not ports (for now)'
         w = s.connect(left, right)  # add a wire
         # print('plug * ' + str(w))
         return right
 
+    @oodebug
     def __add__(self, other):
         """
         Overloaded + operator for implicit block creation.
 
         :param self: A signal (plug) to be added
         :type self: Plug
         :param other: A signal (block or plug) to be added
@@ -438,14 +480,15 @@
         :seealso: :meth:`Plug.__radd__` :meth:`Block.__add__`
         """
         if isinstance(other, (int, float, np.ndarray)):
             # plug + constant, create a CONSTANT block
             other = self.block.bd.CONSTANT(other)
         return self.block.bd.SUM("++", inputs=(self, other))
 
+    @oodebug
     def __radd__(self, other):
         """
         Overloaded + operator for implicit block creation.
 
         :param self: A signal (plug) to be added
         :type self: Plug
         :param other: A signal (block or plug) to be added
@@ -471,14 +514,15 @@
         :seealso: :meth:`Plug.__add__` :meth:`Block.__radd__`
         """
         if isinstance(other, (int, float, np.ndarray)):
             # constant + plug, create a CONSTANT block
             other = self.block.bd.CONSTANT(other)
         return self.block.bd.SUM("++", inputs=(other, self))
 
+    @oodebug
     def __sub__(self, other):
         """
         Overloaded - operator for implicit block creation.
 
         :param self: A signal (plug) to be added (minuend)
         :type self: Plug
         :param other: A signal (block or plug) to be subtracted (subtrahend)
@@ -505,14 +549,15 @@
         :seealso: :meth:`Plug.__rsub__` :meth:`Block.__sub__`
         """
         if isinstance(other, (int, float, np.ndarray)):
             # plug - constant, create a CONSTANT block
             other = self.block.bd.CONSTANT(other)
         return self.block.bd.SUM("+-", inputs=(self, other))
 
+    @oodebug
     def __rsub__(self, other):
         """
         Overloaded - operator for implicit block creation.
 
         :param self: A signal (plug) to be added (minuend)
         :type self: Plug
         :param other: A signal (block or plug) to be subtracted (subtrahend)
@@ -539,14 +584,15 @@
         """
         # TODO deal with other cases as per above
         if isinstance(other, (int, float, np.ndarray)):
             # constant - plug, create a CONSTANT block
             other = self.block.bd.CONSTANT(other)
         return self.block.bd.SUM("+-", inputs=(other, self))
 
+    @oodebug
     def __neg__(self):
         """
         Overloaded unary minus operator for implicit block creation.
 
         :param self: A signal (plug) to be negated
         :type self: Plug
         :return: GAIN block
@@ -561,14 +607,38 @@
         Create a ``GAIN(-1)`` block named ``_gain.N`` whose input is the
         operand.
 
         :seealso: :meth:`Block.__neg__`
         """
         return self.block.bd.GAIN(-1, inputs=[self])
 
+    @oodebug
+    def __pow__(self, p):
+        """
+        Overloaded unary power operator for implicit block creation.
+
+        :param self: A signal (plug) to be exponentiated
+        :type self: Plug
+        :return: POW block
+        :rtype: Block subclass
+
+        This method is implicitly invoked by the ** operator for unary power when the operand is a ``Block``::
+
+            result = X**3
+
+        where ``X`` is a block.
+
+        Creates a ``POW(3)`` block named ``_pow.N`` whose input is the
+        operand.
+
+        :seealso: :meth:`Plug.__pow__`
+        """
+        return self.block.bd.POW(p, inputs=[self])
+
+    @oodebug
     def __mul__(self, other):
         """
         Overloaded * operator for implicit block creation.
 
         :param self: A signal (plug) to be multiplied
         :type self: Plug
         :param other: A signal (block or plug) to be multiplied
@@ -602,14 +672,15 @@
             # value * value, create a PROD block
             name = "_prod.{:d}".format(self.bd.n_auto_prod)
             self.bd.n_auto_prod += 1
             return self.block.bd.PROD(
                 "**", matrix=True, name=name, inputs=[self, other]
             )
 
+    @oodebug
     def __rmul__(self, other):
         """
         Overloaded * operator for implicit block creation.
 
         :param self: A signal (plug) to be multiplied
         :type self: Plug
         :param other: A signal (block or plug) to be multiplied
@@ -637,14 +708,15 @@
         :seealso: :meth:`Plug.__mul__` :meth:`Block.__rmul__`
         """
         if isinstance(other, (int, float, np.ndarray)):
             # constant * plug, create a CONSTANT block
             matrix = isinstance(other, np.ndarray)
             return self.block._autogain(other, premul=matrix, inputs=[self])
 
+    @oodebug
     def __truediv__(self, other):
         """
         Overloaded / operator for implicit block creation.
 
         :param self: A signal (plug) to be multiplied (dividend)
         :type self: Plug
         :param other: A signal (block or plug) to be divided (divisor)
@@ -672,14 +744,15 @@
         :seealso: :meth:`Plug.__rtruediv__` :meth:`Block.__truediv__`
         """
         if isinstance(other, (int, float, np.ndarray)):
             # plug / constant , create a CONSTANT block
             other = self.block.bd.CONSTANT(other)
         return self.block.bd.PROD("*/", inputs=(self, other))
 
+    @oodebug
     def __rtruediv__(self, other):
         """
         Overloaded / operator for implicit block creation.
 
         :param self: A signal (plug) to be multiplied (dividend)
         :type self: Plug
         :param other: A signal (block or plug) to be divided (divisor)
@@ -706,28 +779,14 @@
         :seealso: :meth:`Plug.__truediv__` :meth:`Block.__rtruediv__`
         """
         if isinstance(other, (int, float, np.ndarray)):
             # constant / plug, create a CONSTANT block
             other = self.block.bd.CONSTANT(other)
         return self.block.bd.PROD("*/", inputs=(other, self))
 
-    def __repr__(self):
-        """
-        Display plug details.
-
-        :return: Plug description
-        :rtype: str
-
-        String format::
-
-            bicycle.0[1]
-
-        """
-        return str(self.block) + "[" + str(self.port) + "]"
-
 
 class StartPlug(Plug):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, type="start", **kwargs)
 
 
 class EndPlug(Plug):
@@ -787,46 +846,47 @@
         # get the state from each stateful block on this clock
         x0 = np.array([])
         for b in self.blocklist:
             x0 = np.r_[x0, b.getstate0()]
             # print('x0', x0)
         return x0
 
-    def getstate(self):
+    def getstate(self, t):
 
         x = np.array([])
         for b in self.blocklist:
             # update dstate
-            x = np.r_[x, b.next().flatten()]
+            xb = b.next(t, b.inputs, b._x)
+            x = np.r_[x, xb.flatten()]
 
         return x
 
     def setstate(self):
         x = self._x
         for b in self.blocklist:
             x = b.setstate(x)  # send it to blocks
 
-    def start(self, state=None):
+    def start(self, simstate=None):
         self.i = 1
-        state.declare_event(self, self.time(self.i))
+        simstate.declare_event(self, self.time(self.i))
         self.i += 1
 
-    def next_event(self, state=None):
-        state.declare_event(self, self.time(self.i))
+    def next_event(self, simstate=None):
+        simstate.declare_event(self, self.time(self.i))
         self.i += 1
 
     def time(self, i):
         # return (math.floor((t - self.offset) / self.T) + 1) * self.T + self.offset
         # k = int((t - self.offset) / self.T + 0.5)
         return i * self.T + self.offset
 
     def savestate(self, t):
         # save clock state at time t
         self.t.append(t)
-        self.x.append(self.getstate())
+        self.x.append(self.getstate(t))
 
 
 # ------------------------------------------------------------------------- #
 
 
 class Block:
 
@@ -851,18 +911,18 @@
         # print('Block __new__', args,bd, kwargs)
         block = super(Block, cls).__new__(cls)  # create a new instance
 
         # we overload setattr, so need to know whether it is being passed a port
         # name.  Add this attribute now to allow proper operation.
         block.__dict__["portnames"] = []  # must be first, see __setattr__
 
-        block.bd = bd
         block.nstates = 0
         block.ndstates = 0
         block._sequence = None
+        block._x = None  # state vector
 
         return block
 
     _latex_remove = str.maketrans({"$": "", "\\": "", "{": "", "}": "", "^": ""})
 
     def __init__(
         self,
@@ -1025,14 +1085,16 @@
     def T_output(self, *inputs, t=0.0, x=None):
         """
         Evaluate a block for unit testing.
 
         :param *inputs: Input port values
         :param t: Simulation time, defaults to 0.0
         :type t: float, optional
+        :param x: state vector
+        :type x: ndarray
         :return: Block output port values
         :rtype: list
 
         The output ports of the block are evaluated for a given simulation time
         and set of input port values. Input ports are assigned to consecutive inputs,
         output port values are a list.
 
@@ -1040,33 +1102,33 @@
 
         .. warning:: the instance is monkey patched, not useable in a block
             diagram subsequently.
 
         """
         # check inputs and assign to attribute
         assert len(inputs) == self.nin, "wrong number of inputs provided"
-        self._T_inputs = inputs
-
-        if x is not None:
-            self._x = x
 
         # evaluate the block
-        out = self.output(t=t)
+        out = self.output(t, inputs, x)
 
         # sanity check the output
         assert isinstance(out, list), "result must be a list"
         assert len(out) == self.nout, "result list is wrong length"
         return out
 
-    def T_deriv(self, *inputs, x=None):
+    def T_deriv(self, *inputs, t=0.0, x=None):
         """
         Evaluate a block for unit testing.
 
         :param inputs: input port values
         :type inputs: list
+        :param t: Simulation time, defaults to 0.0
+        :type t: float, optional
+        :param x: state vector
+        :type x: ndarray
         :return: Block derivative value
         :rtype: ndarray
 
         The derivative of the block is evaluated for a given set of input port
         values. Input port values are treated as lists.
 
         Mostly used for making concise unit tests.
@@ -1074,146 +1136,162 @@
         .. warning:: the instance is monkey patched, not useable in a block
             diagram subsequently.
 
         """
 
         # check inputs and assign to attribute
         assert len(inputs) == self.nin, "wrong number of inputs provided"
-        self._T_inputs = inputs
 
         if x is not None:
             assert len(x) == self.nstates, "passed state is wrong length"
-            self._x = x
 
         # evaluate the block
-        out = self.deriv()
+        out = self.deriv(t, inputs, x)
 
         # sanity check the output
         assert isinstance(out, np.ndarray), "result must be an ndarray"
         assert out.shape == (self.nstates,), "result array is wrong length"
         return out
 
-    def T_next(self, *inputs, x=None):
+    def T_next(self, *inputs, t=0.0, x=None):
         """
         Evaluate a block for unit testing.
 
         :param inputs: input port values
         :type inputs: list
-        :return: Block derivative value
+        :param t: Simulation time, defaults to 0.0
+        :type t: float, optional
+        :param x: state vector
+        :type x: ndarray
+        :return: Block next state value
         :rtype: ndarray
 
         The next value of a discrete time block is evaluated for a given set of input port
         values. Input port values are treated as lists.
 
         Mostly used for making concise unit tests.
 
-        .. warning:: the instance is monkey patched, not useable in a block
-            diagram subsequently.
-
         """
 
         # check inputs and assign to attribute
         assert len(inputs) == self.nin, "wrong number of inputs provided"
-        self._T_inputs = inputs
 
         if x is not None:
             assert len(x) == self.ndstates, "passed state is wrong length"
-            self._x = x
 
         # evaluate the block
-        out = self.next()
+        out = self.next(t, inputs, x)
 
         # sanity check the output
-        assert isinstance(out, np.ndarray), "result must be an ndarray"
-        assert out.shape == (self.ndstates,), "result array is wrong length"
+        assert isinstance(out, np.ndarray), "next state must be an ndarray"
+        assert out.shape == (self.ndstates,), "next state array is wrong length"
         return out
 
-    def T_step(self, *inputs, state=None):
+    def T_step(self, *inputs, t=0.0):
+        """
+        Step a block for unit testing.
+
+        :param inputs: input port values
+        :type inputs: list
+        :param t: Simulation time, defaults to 0.0
+        :type t: float, optional
+
+        Step the block for a given set of input port
+        values. Input port values are treated as lists.
 
-        from bdsim.run_sim import BDSimState
+        Mostly used for making concise unit tests.
 
-        if state is None:
-            state = BDSimState()
+        """
 
         # check inputs and assign to attribute
         assert len(inputs) == self.nin, "wrong number of inputs provided"
-        self._T_inputs = inputs
 
         # step the block
-        self.step(state=state)
+        self.step(t, inputs)
 
-    def T_start(self, state=None):
+    def T_start(self, simstate=None):
 
         from bdsim.run_sim import BDSimState, Options
 
-        if state is None:
+        if simstate is None:
 
             class RunTime:
                 def DEBUG(*args):
                     pass
 
             class BlockDiagram:
                 pass
 
             self.bd = BlockDiagram()
             self.bd.runtime = RunTime()
             self.bd.runtime.options = Options()
-            state = BDSimState()
-            state.options = self.bd.runtime.options
-            state.t = 0.0
+            simstate = BDSimState()
+            simstate.options = self.bd.runtime.options
+            simstate.t = 0.0
 
         # step the block
-        self.start(state=state)
-        return state
+        self.start(simstate)
+        return simstate
 
-    def _output(self, *inputs, t=0.0):
-        return self.T_output(*inputs, t=t)
+    def _output(self, *inputs, t=0.0, x=None):
+        return self.T_output(*inputs, t=t, x=x)
 
-    def _step(self, *inputs, state=None, t=None):
+    def _step(self, *inputs, t=0.0):
         return self.T_step(*inputs, t=t)
 
-    def input(self, port):
-        """
-        Get input to block on specified port
+    # def input(self, port):
+    #     """
+    #     Get input to block on specified port
 
-        :param port: port number
-        :type port: int
-        :return: value applied to specified input port
-        :rtype: any
+    #     :param port: port number
+    #     :type port: int
+    #     :return: value applied to specified input port
+    #     :rtype: any
 
-        Return the value of the input applied to the input port numbered
-        ``port``.  The type depends on the source port connected to this input.
+    #     Return the value of the input applied to the input port numbered
+    #     ``port``.  The type depends on the source port connected to this input.
 
-        .. note:: For unit testing purposes, it the block is simply an instance
-            of the class, then setting its attribute ``test_inputs`` to a list
-            provides the input values to the block.
+    #     .. note:: When a block's ``output`` method is evaluated the resulting list is
+    #         saved as an attribute of that block.  The ``input`` method traces back
+    #         along the wire connected to the input port to obtain a reference to the
+    #         output value held by the predecessor block.
+
+    #     .. note:: For unit testing purposes, it the block is simply an instance
+    #         of the class, then setting its attribute ``T_inputs`` to a list
+    #         provides the input values to the block.
 
-        :seealso: :meth:`inputs`
-        """
-        try:
-            p = self.sources[port]  # get plug for source block output
-            return p.block.output_values[p.port]
-        except:
-            # for unit testing a block may not have its input ports connected,
-            # take the value from this list instead
-            return self._T_inputs[port]
+    #     :seealso: :meth:`inputs`
+    #     """
+    #     try:
+    #         p = self.sources[port]  # get plug for source block output
+    #         return p.block.output_values[p.port]
 
     @property
     def inputs(self):
         """
         Get block inputs as a list
 
         :return: list of block inputs
         :rtype: list
 
-        Returns a list of values corresponding to the input ports of the block.
+        Returns a list of values corresponding to the input ports of the block.  The
+        types of the elements are dictated by the blocks connected to the input ports.
+
+        .. note:: When a block's ``output`` method is evaluated the resulting list is
+            saved as an attribute of that block.  The ``inputs`` method uses the
+            ``sources`` attribute which has references to the output values held by
+            the predecessor block.
 
         :seealso: :meth:`input`
         """
-        return [self.input(i) for i in range(self.nin)]
+        values = []
+        for port in range(self.nin):
+            plug = self.sources[port]  # get plug for source block output
+            values.append(plug.block.output_values[plug.port])
+        return values
 
     def __getitem__(self, port):
         """
         Convert a block slice reference to a plug.
 
         :param port: Port number
         :type port: int
@@ -1290,14 +1368,15 @@
             # we're doing wiring
             # print('in __setattr___', self, name, value)
             self.bd.connect(value, getattr(self, name))
         else:
             # regular case, add attribute to the instance's dictionary
             self.__dict__[name] = value
 
+    @oodebug
     def __rshift__(left, right):
         """
         Operator for implicit wiring.
 
         :param left: A block to be wired from
         :type left: Block
         :param right: A block or plugto be wired to
@@ -1352,14 +1431,20 @@
         if isinstance(value, (int, float, str)):
             name = "_gain.{:d}({})".format(self.bd.n_auto_gain, value)
         else:
             name = "_gain.{:d}<{}>".format(self.bd.n_auto_gain, type(value).__name__)
         self.bd.n_auto_gain += 1
         return self.bd.GAIN(value, name=name, **kwargs)
 
+    def _autopow(self, value, **kwargs):
+        name = "_pow.{:d}({})".format(self.bd.n_auto_pow, value)
+        self.bd.n_auto_pow += 1
+        return self.bd.POW(value, name=name, **kwargs)
+
+    @oodebug
     def __add__(self, other):
         """
         Overloaded + operator for implicit block creation.
 
         :param self: A signal (block) to be added
         :type self: Block
         :param other: A signal (block or plug) to be added
@@ -1391,14 +1476,15 @@
         name = "_sum.{:d}".format(self.bd.n_auto_sum)
         self.bd.n_auto_sum += 1
         if isinstance(other, (int, float, np.ndarray)):
             # block + constant, create a CONSTANT block
             other = self._autoconstant(other)
         return self.bd.SUM("++", inputs=(self, other), name=name)
 
+    @oodebug
     def __radd__(self, other):
         """
         Overloaded + operator for implicit block creation.
 
         :param self: A signal (block) to be added
         :type self: Block
         :param other: A signal (block or plug) to be added
@@ -1430,14 +1516,15 @@
         name = "_sum.{:d}".format(self.bd.n_auto_sum)
         self.bd.n_auto_sum += 1
         if isinstance(other, (int, float, np.ndarray)):
             # constant + block, create a CONSTANT block
             other = self._autoconstant(other)
         return self.bd.SUM("++", inputs=(other, self), name=name)
 
+    @oodebug
     def __sub__(self, other):
         """
         Overloaded - operator for implicit block creation.
 
         :param self: A signal (block) to be added (minuend)
         :type self: Block
         :param other: A signal (block or plug) to be subtracted (subtrahend)
@@ -1464,14 +1551,15 @@
         name = "_sum.{:d}".format(self.bd.n_auto_sum)
         self.bd.n_auto_sum += 1
         if isinstance(other, (int, float, np.ndarray)):
             # block - constant, create a CONSTANT block
             other = self._autoconstant(other)
         return self.bd.SUM("+-", inputs=(self, other), name=name)
 
+    @oodebug
     def __rsub__(self, other):
         """
         Overloaded - operator for implicit block creation.
 
         :param self: A signal (block) to be added (minuend)
         :type self: Block
         :param other: A signal (block or plug) to be subtracted (subtrahend)
@@ -1502,14 +1590,15 @@
         name = "_sum.{:d}".format(self.bd.n_auto_sum)
         self.bd.n_auto_sum += 1
         if isinstance(other, (int, float, np.ndarray)):
             # constant - block, create a CONSTANT block
             other = self._autoconstant(other)
         return self.bd.SUM("+-", inputs=(other, self), name=name)
 
+    @oodebug
     def __neg__(self):
         """
         Overloaded unary minus operator for implicit block creation.
 
         :param self: A signal (block) to be negated
         :type self: Block
         :return: GAIN block
@@ -1524,14 +1613,38 @@
         Creates a ``GAIN(-1)`` block named ``_gain.N`` whose input is the
         operand.
 
         :seealso: :meth:`Plug.__neg__`
         """
         return self._autogain(-1.0, inputs=[self])
 
+    @oodebug
+    def __pow__(self, p):
+        """
+        Overloaded unary power operator for implicit block creation.
+
+        :param self: A signal (block) to be negated
+        :type self: Block
+        :return: POW block
+        :rtype: Block subclass
+
+        This method is implicitly invoked by the ** operator for unary power when the operand is a ``Block``::
+
+            result = X**3
+
+        where ``X`` is a block.
+
+        Creates a ``POW(3)`` block named ``_pow.N`` whose input is the
+        operand.
+
+        :seealso: :meth:`Plug.__pow__`
+        """
+        return self._autopow(p, inputs=[self])
+
+    @oodebug
     def __mul__(self, other):
         """
         Overloaded * operator for implicit block creation.
 
         :param self: A signal (block) to be multiplied
         :type self: Block
         :param other: A signal (block or plug) to be multiplied
@@ -1565,14 +1678,15 @@
             return self._autogain(other, premul=matrix, matrix=matrix, inputs=[self])
         else:
             # value * value, create a PROD block
             name = "_prod.{:d}".format(self.bd.n_auto_prod)
             self.bd.n_auto_prod += 1
             return self.bd.PROD("**", inputs=[self, other], matrix=matrix, name=name)
 
+    @oodebug
     def __rmul__(self, other):
         """
         Overloaded * operator for implicit block creation.
 
         :param self: A signal (block) to be multiplied
         :type self: Block
         :param other: A signal (block or plug) to be multiplied
@@ -1601,14 +1715,15 @@
         """
         matrix = False
         if isinstance(other, (int, float, np.ndarray)):
             # constant * block, create a GAIN block
             matrix = isinstance(other, np.ndarray)
             return self._autogain(other, premul=matrix, inputs=[self])
 
+    @oodebug
     def __truediv__(self, other):
         """
         Overloaded / operator for implicit block creation.
 
         :param self: A signal (block) to be multiplied (dividend)
         :type self: Block
         :param other: A signal (block or plug) to be divided (divisor)
@@ -1641,14 +1756,15 @@
         matrix = False
         if isinstance(other, (int, float, np.ndarray)):
             # block / constant, create a CONSTANT block
             other = self._autoconstant(other)
             matrix = isinstance(other, np.ndarray)
         return self.bd.PROD("*/", inputs=(self, other), matrix=matrix, name=name)
 
+    @oodebug
     def __rtruediv__(self, other):
         """
         Overloaded / operator for implicit block creation.
 
         :param self: A signal (block) to be multiplied (dividend)
         :type self: Block
         :param other: A signal (block or plug) to be divided (divisor)
@@ -1760,15 +1876,15 @@
               name will the one optionally assigned by the user using the ``name``
               keyword, otherwise a systematic default name.
 
         :seealso: outport_names
 
         """
 
-        w = self.inports[port]
+        w = self.input_wires[port]
         if w.name is not None:
             return w.name
         src = w.start.block
         srcp = w.start.port
         if src._outport_names is not None:
             return src._outport_names[srcp]
         return str(w.start)
@@ -1811,15 +1927,15 @@
 
     # def setinputs(self, *pos):
     #     assert len(pos) == self.nin, 'mismatch in number of inputs'
     #     self.reset()
     #     for i, val in enumerate(pos):
     #         self.inputs[i] = val
 
-    def start(self, **kwargs):  # begin of a simulation
+    def start(self, simstate):  # begin a simulation
         pass
 
     def check(self):  # check validity of block parameters at start
         assert hasattr(self, "nin"), f"block {self.name} has no nin specified"
         assert hasattr(self, "nout"), f"block {self.name} has no nout specified"
 
         assert (
@@ -1828,17 +1944,14 @@
         assert (
             hasattr(self, "initd") and self.initd
         ), "Block superclass not initalized. was super().__init__ called?"
 
     def done(self, **kwargs):  # end of simulation
         pass
 
-    def step(self, **kwargs):  # valid
-        pass
-
     def savefig(self, *pos, **kwargs):
         pass
 
 
 class SinkBlock(Block):
     """
     A SinkBlock is a subclass of Block that represents a block that has inputs
@@ -1860,14 +1973,17 @@
         This is the parent class of all sink blocks.
         """
         # print('Sink constructor')
         super().__init__(**blockargs)
         self.nout = 0
         self.nstates = 0
 
+    def step(self, t, inports):  # valid
+        pass
+
 
 class SourceBlock(Block):
     """
     A SourceBlock is a subclass of Block that represents a block that has outputs
     but no inputs.  Its output is a function of parameters and time.
     """
```

### Comparing `bdsim-1.0.0/bdsim/graphics.py` & `bdsim-1.1.0/bdsim/graphics.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,57 +28,59 @@
         """
 
         super().__init__(**blockargs)
         self._graphics = True
 
         self.movie = movie
 
-    def start(self):
+    def start(self, simstate):
 
-        plt.draw()
-        plt.show(block=False)
+        # plt.draw()
+        # plt.show(block=False)
+        self._simstate = simstate
+        self._enabled = simstate.options.graphics
 
-        if self.movie is not None and not self.bd.runtime.options.animation:
+        if self.movie is not None and not simstate.options.animation:
             print(
                 "enabling global animation option to allow movie option on block", self
             )
-            if not self.bd.runtime.options.animation:
+            if not simstate.options.animation:
                 print("must enable animation to render a movie")
         if self.movie is not None:
             try:
                 self.writer = animation.FFMpegWriter(
                     fps=10, extra_args=["-vcodec", "libx264"]
                 )
                 self.writer.setup(fig=self.fig, outfile=self.movie)
                 print("movie block", self, " --> ", self.movie)
             except FileNotFoundError:
                 self.fatal("cannot save movie, please install ffmpeg")
 
-    def step(self, state=None):
-        super().step()
+    def step(self, t, inports):
+        super().step(t, inports)
 
         # bring the figure up to date in a backend-specific way
-        if state.options.animation:
-            if state.backend == "TkAgg":
+        if self._simstate.options.animation:
+            if self._simstate.backend == "TkAgg":
                 self.fig.canvas.flush_events()
                 plt.show(block=False)
                 plt.show(block=False)
-            elif state.backend == "Qt5Agg":
+            elif self._simstate.backend == "Qt5Agg":
                 self.fig.canvas.flush_events()
                 self.fig.canvas.draw()
             else:
                 self.fig.canvas.draw()
 
         if self.movie is not None:
             try:
                 self.writer.grab_frame()
             except AttributeError:
                 self.fatal("cannot save movie, please install ffmpeg")
 
-    def done(self, state=None, block=False):
+    def done(self, block=False):
         if self.fig is not None:
             self.fig.canvas.start_event_loop(0.001)
             if self.movie is not None:
                 self.writer.finish()
                 # self.cleanup()
             plt.show(block=block)
 
@@ -139,15 +141,16 @@
                     # otherwise use default (MacOSX)
                     if "Qt5Agg" in matplotlib.rcsetup.all_backends:
                         try:
                             import PyQt5
 
                             matplotlib.use("Qt5Agg")
                             print(
-                                "no graphics backend specified: Qt5Agg found, using instead of MacOSX"
+                                "no graphics backend specified: Qt5Agg found, using"
+                                " instead of MacOSX"
                             )
                         except:
                             pass
             else:
                 try:
                     matplotlib.use(options.backend)
                 except ImportError:
@@ -258,16 +261,23 @@
             f,
             col * gstate.figsize[0] * gstate.dpi * scale,
             row * gstate.figsize[1] * gstate.dpi * scale,
         )
         gstate.fignum += 1
 
         def onkeypress(event):
-            print("pressed", event.key)
-            plt.close("all")
+
+            if event.key == "x":
+                print("\nclosing all windows")
+                plt.close("all")
+            elif event.key == "ctrl+c":
+                print("\nterminating bdsim")
+                sys.exit(1)
+            else:
+                print("key pressed", event.key)
 
         f.canvas.mpl_connect("key_press_event", onkeypress)
 
         self.bd.runtime.DEBUG(
             "graphics", "create figure {:d} at ({:d}, {:d})", gstate.fignum, row, col
         )
         return f
```

### Comparing `bdsim-1.0.0/bdsim/newplots.py` & `bdsim-1.1.0/bdsim/newplots.py`

 * *Files identical despite different names*

### Comparing `bdsim-1.0.0/bdsim/run_realtime.py` & `bdsim-1.1.0/bdsim/run_realtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 import threading
 import time
 import threading
 
 from bdsim.run_sim import BDSim, TimeQ, blockname
 
+# https://stackoverflow.com/questions/44807302/create-c-timer-in-macos
 
 # class TimeQRT(TimeQ):
 #     """
 #     Time-ordered queue for events
 
 #     The list comprises tuples of (time, block) to reflect an event associated
 #     with the specified block at the specified time.
```

### Comparing `bdsim-1.0.0/bdsim/run_sim.py` & `bdsim-1.1.0/bdsim/run_sim.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 import sys
 import importlib
 import inspect
 from collections import Counter, namedtuple
 import argparse
 import types
 import warnings
+import time
 
 from bdsim.blockdiagram import BlockDiagram
 from bdsim.components import OptionsBase, Block, Clock, BDStruct, Plug, clocklist
+import spatialmath.base as smb
 import tempfile
 import subprocess
 import webbrowser
+import traceback
 
 import numpy as np
 import scipy.integrate as integrate
 import matplotlib.pyplot as plt
 import re
 from colored import fg, attr
 
@@ -25,35 +28,32 @@
 
     _FillingCirclesBar = True
 except ImportError:
     _FillingCirclesBar = False
 
 
 class Progress:
-
     # print a progress bar
     # https://stackoverflow.com/questions/3173320/text-progress-bar-in-the-console
     @staticmethod
     def printProgressBar(
         fraction, prefix="", suffix="", decimals=1, length=50, fill="█", printEnd="\r"
     ):
-
         percent = ("{0:." + str(decimals) + "f}").format(fraction * 100)
         filledLength = int(length * fraction)
         bar = fill * filledLength + "-" * (length - filledLength)
         print(f"\r{prefix} |{bar}| {percent}% {suffix}", end=printEnd)
 
     def __init__(self, enable=True):
         self.enable = enable
         self.length = 60
         if not enable:
             return
 
     def start(self, T):
-
         self.T = T
 
         if not self.enable:
             return
 
         if _FillingCirclesBar:
             self.bar = FillingCirclesBar(
@@ -131,15 +131,18 @@
         """
         if len(self) == 0:
             return f"TimeQ: len={len(self)}"
         else:
             return f"TimeQ: len={len(self)}, first out {self.q[0]}"
 
     def __repr__(self):
-        return str(self)
+        events = []
+        for t in self.q:
+            events.append(str(t))
+        return "\n".join(events)
 
     def push(self, value):
         """
         Push value onto time-ordered queue
 
         :param value: tuple (time, block)
         :type value: tuple
@@ -224,15 +227,14 @@
     :ivar checkfinite: halt simulation if any wire has inf or nan
     :vartype checkfinite: bool
     :ivar graphics: enable graphics
     :vartype graphics: bool
     """
 
     def __init__(self):
-
         self.x = None  # continuous state vector numpy.ndarray
         self.T = None  # maximum.BlockDiagram time
         self.t = None  # current time
         self.fignum = 0
         self.stop = None
         self.checkfinite = True
 
@@ -241,19 +243,24 @@
         self.eventq = TimeQ()
 
     def declare_event(self, block, t):
         self.eventq.push((t, block))
 
 
 class BDSim:
-
     _blocklibrary = None
 
-    def __init__(self, packages=None, load=True, **kwargs):
+    def __init__(self, banner=True, packages=None, load=True, **kwargs):
         """
+        :param banner: display docstring banner, defaults to True
+        :type banner: bool, optional
+        :param packages: colon-separated list of folders to search for blocks
+        :type packages: str
+        :param load: dynamically load blocks from libraries, defaults to True
+        :type load: bool,optional
         :param sysargs: process options from sys.argv, defaults to True
         :type sysargs: bool, optional
         :param graphics: enable graphics, defaults to True
         :type graphics: bool, optional
         :param animation: enable animation, defaults to False
         :type animation: bool, optional
         :param progress: enable progress bar, defaults to True
@@ -275,39 +282,57 @@
         Command line switch  Argument   Default   Behaviour
         ===================  =========  ========  ===========================================
         --graphics, +g       graphics   True      enable graphical display
         --animation, +a      animation  True      update graphics at each time step
         --hold, +h           hold       True      hold graphics in done()
         --no-graphics, -g    graphics   True      disable graphical display
         --no-animation, -a   animation  True      don't update graphics at each time step
-        --no-hold, -h        hold       True      do not hold graphics in done()
+        --no-hold, -H        hold       True      do not hold graphics in done()
         --no-progress, -p    progress   True      do not display simulation progress bar
         --backend BE         backend    'Qt5Agg'  matplotlib backend
         --tiles RxC, -t RxC  tiles      '3x4'     arrangement of figure tiles on the display
         --shape WxH          shape      None      window size, default matplotlib size
-        --altscreen          altscreen  True      use secondary monitor if it exists
-        --verbose, -v        verbose    False     be verbose
+        --altscreen, +A,     altscreen  True      display plots on second monitor
+        --no-altscreen, -A   altscreen  True      do not display plots on second monitor
         --debug F, -d F      debug      ''        debug flag string
         --simtime T[,dt]     simtime    (10,)     simulation time
+        --verbose, -v        verbose    False     be verbose
+        --quiet, -q          quiet      False     suppress reports
+        -o                   outfile    None      output pickled simulation results to bd.out
+        --out OUTFILE        outfile    None      file to save pickled simulation results
+        --set P, -s P        setparam   []        override block parameter using ``P=block:param=value``
+        --global G           setglob    []        override global parameter using ``G=var=value``
         ===================  =========  ========  ===========================================
 
         .. note:: ``animation`` and ``graphics`` options are coupled.  If
             ``graphics=False``, all graphics is suppressed.  If
             ``graphics=True`` then graphics are shown and the behaviour depends
             on ``animation``.  ``animation=False`` shows graphs at the end of
             the simulation, while ``animation=True` will animate the graphs
             during simulation.
 
-        :seealso: :meth:`set_options`
+        :seealso: :meth:`set_globals()`
         """
 
         self.packages = packages
 
         # process command line and overall options
         self.options = Options(**kwargs)
+
+        # print docstring as a startup banner
+        if banner and not self.options.quiet:
+            calling_frame = inspect.currentframe().f_back
+            try:
+                doc = calling_frame.f_locals["__doc__"]
+                if doc is not None:
+                    for line in doc.strip().split("\n"):
+                        print("* " + line)
+            except KeyError:
+                pass
+
         # load modules from the blocks folder
         if BDSim._blocklibrary is None and load:
             BDSim._blocklibrary = self.load_blocks(self.options.verbose)
         if self.options.blocks:
             self.blocks()
 
     def blockinfo(self, block=None):
@@ -350,15 +375,18 @@
         :return: single line summary of simulation environment
         :rtype: str
         """
         s = f"BDSim: {len(self._blocklibrary)} blocks in library\n"
         return s
 
     def __repr__(self):
-        s = f"Block diagram simulation runtime, {len(self._blocklibrary)} blocks imported to library.\n"
+        s = (
+            f"Block diagram simulation runtime, {len(self._blocklibrary)} blocks"
+            " imported to library.\n"
+        )
         s += "simulation options:\n"
         for k, v in self.state.options.items():
             s += "  {:s}: {}\n".format(k, v)
         return s
 
     def run(
         self,
@@ -433,184 +461,298 @@
             harsh non-linearity.
         """
 
         assert bd.compiled, "Network has not been compiled"
 
         # get simulation time
         #  --simtime=T  or --simtime=T,dt
-        try:
-            default_times = eval(self.option("simtime"))
-            if isinstance(default_times, (int, float)):
-                T = default_times
-            else:
-                T, dt = default_times
-        except:
-            pass
+        if self.options.simtime is not None:
+            try:
+                default_times = eval(self.options.simtime)
+                if isinstance(default_times, (int, float)):
+                    T = default_times
+                elif isinstance(default_times, tuple):
+                    T, dt = default_times
+                else:
+                    raise ValueError(
+                        "bad simtime option passed " + self.options.simtime
+                    )
+            except:
+                raise ValueError("bad simtime option passed " + self.options.simtime)
 
         # final default values
         # T = T or 5
         # dt = dt or 0.01
 
-        state = BDSimState()
-        self.state = state
-        state.T = T
+        simstate = BDSimState()
+        self.simstate = simstate
+        simstate.T = T
 
         if dt is None and not "max_step" in solver_args:
             dt = T / 100
-        state.dt = dt
-        state.count = 0
-        state.solver = solver
-        state.solver_args = solver_args
-        state.minstepsize = minstepsize
-        state.stop = None  # allow any block to stop.BlockDiagram by setting this to the block's name
-        state.checkfinite = checkfinite
+        simstate.dt = dt
+        simstate.count = 0
+        simstate.bdtime = 0.0
+        simstate.gtime = 0.0  # last graphics update
+        simstate.solver = solver
+        simstate.solver_args = solver_args
+        simstate.minstepsize = minstepsize
+        simstate.stop = None  # allow any block to stop.BlockDiagram by setting this to the block's name
+        simstate.checkfinite = checkfinite
         # state.options = copy.copy(self.options)
-        state.options = self.options
+        simstate.options = self.options
         self.bd = bd
-        state.t_stop = None
+        simstate.t_stop = None
         if debug:
             # append debug flags
-            if debug not in state.options.debug:
-                state.options.debug += debug
+            if debug not in simstate.options.debug:
+                simstate.options.debug += debug
 
         # turn off progress bar if any debug options are given
-        if len(state.options.debug) > 0:
+        if len(simstate.options.debug) > 0:
             self.options.progress = False
         if block is not None:
             self.options.hold = block
 
         # process the watchlist
         #  elements can be:
         #   - block or Plug reference
         #   - str in the form BLOCKNAME[PORT]
         watchlist = []
         watchnamelist = []
-        re_block = re.compile(r"(?P<name>[^[]+)(\[(?P<port>[0-9]+)\])")
+        re_block = re.compile(r"(?P<name>[^[]+)(\[(?P<port>[0-9]+)\])?")
         for w in watch:
             if isinstance(w, str):
                 # a name was given, with optional port number
                 m = re_block.match(w)
                 if m is None:
                     raise ValueError("watch block[port] not found: " + w)
                 name = m.group("name")
-                port = int(m.group("port"))
+
+                # get optional port number
+                port = m.group("port")
+                if port is None:
+                    port = 0
+                else:
+                    port = int(port)
+
                 b = bd.blocknames[name]
                 plug = b[port]
             elif isinstance(w, Block):
                 # a block was given, defaults to port 0
                 plug = w[0]
             elif isinstance(w, Plug):
                 # a plug was given
                 plug = w
             watchlist.append(plug)
             watchnamelist.append(str(plug))
-        state.watchlist = watchlist
-        state.watchnamelist = watchnamelist
+        simstate.watchlist = watchlist
+        simstate.watchnamelist = watchnamelist
 
         x0 = bd.getstate0()
-        print("initial state  x0 = ", x0)
+        if not self.options.quiet:
+            print(fg("yellow"))
+            print(f">>> Start simulation: T = {T}, dt = {dt}")
+            print(f"  Continuous state variables: {bd.nstates}")
+            print("     x0 = ", x0)
+
+            print(f"  Discrete state variables:   {bd.ndstates}")
 
         # get the number of discrete states from all clocks
         ndstates = 0
         for clock in bd.clocklist:
             nds = 0
             for b in clock.blocklist:
                 nds += b.ndstates
             ndstates += nds
-            print(clock.name, "initial dstate x0 = ", clock.getstate())
+            if not self.options.quiet:
+                print(f"    {clock.name}: x0 = ", clock.getstate0())
+
+        if not self.options.quiet:
+            print(attr(0))
+
+        # update block parameters given on command line
+        self.update_parameters(bd)
 
         # tell all blocks we're starting a BlockDiagram
-        self.bd.start(state=state, graphics=self.state.options.graphics)
+        self.bd.start(simstate)
 
         # initialize list of time and states
-        state.tlist = []
-        state.xlist = []
-        state.plist = [[] for p in state.watchlist]
+        simstate.tlist = []
+        simstate.xlist = []
+        simstate.plist = [[] for p in simstate.watchlist]
 
         self.progress = Progress(enable=self.options.progress)
         self.progress.start(T)
 
-        if len(self.state.eventq) == 0:
+        if len(simstate.eventq) == 0:
             # no simulation events, solve it in one go
-            self.run_interval(bd, 0, T, x0, state=state)
+            self.run_interval(bd, 0, T, x0, simstate=simstate)
             nintervals = 1
         else:
             # we have simulation events, solve it in chunks
-            self.state.declare_event(None, T)  # add an event at end of simulation
+            simstate.declare_event(None, T)  # add an event at end of simulation
 
             # ignore all the events at zero
             tprev = 0
-            self.state.eventq.pop_until(tprev)
+            simstate.eventq.pop_until(tprev)
 
             # get the state vector
             x = x0
 
             nintervals = 0
             while True:
                 # get next event from the queue and the list of blocks or
                 # clocks at that time
-                tnext, sources = self.state.eventq.pop(dt=1e-6)
+                tnext, sources = simstate.eventq.pop(dt=1e-6)
                 if tnext is None:
                     break
                 # run system until next event time
-                x = self.run_interval(bd, tprev, tnext, x, state=state)
+                x = self.run_interval(bd, tprev, tnext, x, simstate=simstate)
                 nintervals += 1
 
                 # visit all the blocks and clocks that have an event now
                 for source in sources:
                     if isinstance(source, Clock):
                         # clock ticked, save its state
-                        clock.savestate(tnext)
-                        clock.next_event(self.state)
+                        source.savestate(tnext)
+                        source.next_event(self.simstate)
 
                         # get the new state
-                        clock._x = clock.getstate()
+                        source._x = source.getstate(tnext)
                 tprev = tnext
 
                 # are we done?
-                if state.t is not None and state.t >= T:
+                if simstate.t is not None and simstate.t >= T:
                     break
 
         # finished integration
 
         self.progress.end()  # cleanup the progress bar
 
         # print some info about the integration
-        print(fg("yellow"))
-        print(f"integrator steps:      {state.count}")
-        print(f"time steps:            {len(state.tlist)}")
-        print(f"integration intervals: {nintervals}")
-        print(attr(0))
+        if not self.options.quiet:
+            print(fg("yellow"))
+            print("<<< Simulation complete")
+            print(f"  block diagram evaluations: {simstate.count}")
+            print(
+                "  block diagram exec time:  "
+                f" {simstate.bdtime / simstate.count * 1000.0:.3f} ms"
+            )
+            print(f"  time steps:                {len(simstate.tlist)}")
+            print(f"  integration intervals:     {nintervals}")
+            print(attr(0))
 
         # save buffered data in a Struct
         out = BDStruct(name="results")
-        out.t = np.array(state.tlist)
-        out.x = np.array(state.xlist)
+        out.t = np.array(simstate.tlist)
+        out.x = np.array(simstate.xlist)
         out.xnames = bd.statenames
 
         # save clocked states
         for c in bd.clocklist:
             name = c.name.replace(".", "")
             clockdata = BDStruct(name)
             clockdata.t = np.array(c.t)
             clockdata.x = np.array(c.x)
             out.add(name, clockdata)
 
         # save the watchlist into variables named y0, y1 etc.
         for i, p in enumerate(watchlist):
-            out["y" + str(i)] = np.array(state.plist[i])
+            out["y" + str(i)] = np.array(simstate.plist[i])
         out.ynames = watchnamelist
 
+        # the command line options -o or --out saves results as a pickle file
+        #  -o defaults to bd.out
+        #  --out FILE allows the filename to be specified
+        #
+        # we can visualize the output file by
+        #
+        #   % python -mpickle bd.out
+        #   t      = ndarray:float64 (123,)
+        #   x      = ndarray:float64 (123, 1)
+        #   xnames = ['plantx0'] (list)
+        #   ynames = [] (list)
+
+        if self.options.outfile is not None:
+            out.dump(self.options.outfile)
+
+            if not self.options.quiet:
+                print("simulation results pickled --> ", self.options.outfile)
+
         # pause until all graphics blocks close
-        if self.options.graphics:
-            self.done(self.bd, block=self.options.hold)
 
+        if self.options.graphics and self.options.hold:
+            self.done(self.bd, block=self.options.hold)
         return out
 
-    def run_interval(self, bd, t0, T, x0, state):
+    def update_parameters(self, bd):
+        """
+        Set value of parameters according to command line arguments
+
+        Command line arguments of the form:
+
+            ``-s block:param=value``
+            ``--set block:param=value``
+
+        are stored as list items in ``options.setparam``
+
+        ``block`` can be either:
+
+        - the block's name as a string, either user assigned or bdsim assigned
+        - the block ``id`` as displayed by the ``report`` method
+
+        ``param`` is the name of the parameter used in the constructor
+
+        ``value`` is the new value of the variable
+        """
+
+        re_set = re.compile(r"(?P<block>[\w\.]+):(?P<param>[\w]+)=(?P<value>.*)")
+        for s in self.options.setparam:
+            m = re_set.match(s)
+            if m is None:
+                raise ValueError("bad set parameter: " + s)
+
+            # get block reference
+            blockname = m["block"]
+            try:
+                blockname = int(blockname)
+            except ValueError:
+                pass
+            block = bd[blockname]
+
+            param = m["param"]
+            try:
+                prev_value = getattr(block, param)
+            except ValueError:
+                raise ValueError(f"block {block.name} has no parameter '{param}'")
+
+            # get the parameter
+            value = m["value"]
+            new_value = None
+
+            try:
+                if ";" in value:
+                    new_value = smb.str2array(value)
+                else:
+                    try:
+                        new_value = int(value)
+                    except ValueError:
+                        new_value = float(value)
+            except ValueError:
+                raise ValueError("cannot parse value " + value)
+
+            # change the value
+            setattr(block, param, new_value)
+            print(
+                f"changed value of {block.name}:{param} from {prev_value} ->"
+                f" {new_value}"
+            )
+
+    def run_interval(self, bd, t0, T, x0, simstate=None):
         """
         Integrate system over interval
 
         :param bd: the system blockdiagram
         :type bd: BlockDiagram
         :param t0: initial time
         :type t0: float
@@ -630,148 +772,171 @@
             if bd.nstates > 0:
                 # system has continuous states, solve it using numerical integration
                 # print('initial state x0 = ', x0)
 
                 # block diagram contains states, solve it using numerical integration
 
                 scipy_integrator = integrate.__dict__[
-                    state.solver
+                    simstate.solver
                 ]  # get user specified integrator
 
                 def ydot(t, y):
-                    state.t = t
-                    state.count += 1
-                    return bd.evaluate_plan(y, t)
+                    simstate.t = t
+                    simstate.count += 1
+                    t0 = time.time()
+                    yd = bd.schedule_evaluate(y, t, sinks=False, simstate=simstate)
+                    t1 = time.time()
+                    simstate.bdtime += t1 - t0
+                    return yd
 
-                if state.dt is not None:
-                    state.solver_args["max_step"] = state.dt
+                if simstate.dt is not None:
+                    simstate.solver_args["max_step"] = simstate.dt
 
                 # print(f"run interval: from {t0} to {t0+T}, args={state.solver_args}, x0={x0}")
                 integrator = scipy_integrator(
-                    ydot, t0=t0, y0=x0, t_bound=T, **state.solver_args
+                    ydot, t0=t0, y0=x0, t_bound=T, **simstate.solver_args
                 )
 
                 # integrate
                 while integrator.status == "running":
-
                     # step the integrator, calls _deriv and evaluate block diagram multiple times
                     message = integrator.step()
 
                     if integrator.status == "failed":
                         print(
                             fg("red")
                             + f"\nintegration completed with failed status: {message}"
                             + attr(0)
                         )
                         break
 
                     # stash the results
-                    state.tlist.append(integrator.t)
-                    state.xlist.append(integrator.y)
+                    simstate.t = integrator.t
+                    simstate.tlist.append(integrator.t)
+                    simstate.xlist.append(integrator.y)
 
                     # record the ports on the watchlist
-                    for i, p in enumerate(state.watchlist):
-                        state.plist[i].append(p.block.output(integrator.t)[p.port])
+                    for i, p in enumerate(simstate.watchlist):
+                        b = p.block
+                        out = b.output(integrator.t, b.inputs, b._x)[p.port]
+                        simstate.plist[i].append(out)
 
-                    # # update all blocks that need to know
-                    bd.step(state=self.state)
+                    # update all blocks that need to know
+                    if (integrator.t - simstate.gtime) > (simstate.T / 200):
+                        bd.step(integrator.t)
+                        simstate.gtime = integrator.t
+                    # bd.step(integrator.t)
 
-                    self.progress.update(self.state.t)  # update the progress bar
+                    self.progress.update(simstate.t)  # update the progress bar
 
                     if integrator.status == "finished":
                         break
 
                     # has any block called a stop?
-                    if state.stop is not None:
+                    if simstate.stop is not None:
                         print(
-                            fg("red")
-                            + f"\n--- stop requested at t={state.t:.4f} by {state.stop}"
-                            + attr(0)
+                            fg("red") + f"\n--- stop requested at t={simstate.t:.4f} by"
+                            f" {simstate.stop}" + attr(0)
                         )
                         break
 
                     if (
-                        state.minstepsize is not None
-                        and integrator.step_size < state.minstepsize
+                        simstate.minstepsize is not None
+                        and integrator.step_size < simstate.minstepsize
                     ):
                         print(
-                            fg("red")
-                            + f"\n--- stopping on minimum step size at t={state.t:.4f} with last stepsize {integrator.step_size:g}"
-                            + attr(0)
+                            fg("red") + "\n--- stopping on minimum step size at"
+                            f" t={simstate.t:.4f} with last stepsize"
+                            f" {integrator.step_size:g}" + attr(0)
                         )
                         break
 
-                    if "i" in state.options.debug:
-                        bd._debugger(integrator)
+                    if "i" in simstate.options.debug:
+                        bd._debugger(simstate, integrator)
 
                 return integrator.y  # return final state vector
 
             elif len(clocklist) == 0:
                 # block diagram has no continuous or discrete states
 
-                assert dt is not None, "if no states must specify dt"
+                assert simstate.dt is not None, "if no states must specify dt"
 
-                for t in np.arange(t0, T, state.dt):  # step through the time range
+                for t in np.arange(t0, T, simstate.dt):  # step through the time range
                     # evaluate the block diagram
-                    state.t = t
-                    bd.evaluate_plan([], t)
+                    simstate.t = t
+
+                    simstate.count += 1
+                    t0 = time.time()
+                    bd.schedule_evaluate([], t)
+                    t1 = time.time()
+                    simstate.bdtime += t1 - t0
 
                     # stash the results
-                    state.tlist.append(t)
+                    simstate.tlist.append(t)
 
                     # record the ports on the watchlist
-                    for i, p in enumerate(state.watchlist):
-                        state.plist[i].append(p.block.output(t)[p.port])
+                    for i, p in enumerate(simstate.watchlist):
+                        b = p.block
+                        out = b.output(integrator.t, b.inputs, b._x)[p.port]
+                        simstate.plist[i].append(out)
 
                     # update all blocks that need to know
-                    bd.step(state=state)
+                    bd.step(t)
 
-                    self.progress.update(self.state.t)  # update the progress bar
+                    self.progress.update(t)  # update the progress bar
 
                     # has any block called a stop?
-                    if state.stop is not None:
+                    if simstate.stop is not None:
                         print(
-                            fg("red")
-                            + f"\n--- stop requested at t={state.t:.4f} by {state.stop}"
-                            + attr(0)
+                            fg("red") + f"\n--- stop requested at t={simstate.t:.4f} by"
+                            f" {simstate.stop}" + attr(0)
                         )
                         break
 
-                    if "i" in state.options.debug:
-                        bd._debugger(integrator)
+                    if "i" in simstate.options.debug:
+                        bd._debugger(simstate, integrator)
 
             else:
                 # block diagram has no continuous states
                 t = t0
-                state.t = t
+                simstate.t = t
                 # evaluate the block diagram
-                bd.evaluate_plan([], t)
+
+                simstate.count += 1
+                t0 = time.time()
+                bd.schedule_evaluate([], t)
+                t1 = time.time()
+                simstate.bdtime += t1 - t0
 
                 # stash the results
-                state.tlist.append(t)
+                simstate.tlist.append(t)
 
                 # record the ports on the watchlist
-                for i, p in enumerate(state.watchlist):
-                    state.plist[i].append(p.block.output(t)[p.port])
+                for i, p in enumerate(simstate.watchlist):
+                    b = p.block
+                    out = b.output(integrator.t, b.inputs, b._x)[p.port]
+                    simstate.plist[i].append(out)
 
                 # update all blocks that need to know
-                bd.step(state=state)
+                if (t - simstate.gtime) > (simstate.T / 200):
+                    bd.step(t)
+                    simstate.gtime = t
+                # bd.step(t)
 
-                self.progress.update(self.state.t)  # update the progress bar
+                self.progress.update(simstate.t)  # update the progress bar
 
                 # has any block called a stop?
-                if state.stop is not None:
+                if simstate.stop is not None:
                     print(
-                        fg("red")
-                        + f"\n--- stop requested at t={bd.simstate.t:.4f} by {bd.simstate.stop}"
-                        + attr(0)
+                        fg("red") + f"\n--- stop requested at t={simstate.t:.4f} by"
+                        f" {simstate.stop}" + attr(0)
                     )
 
-                if "i" in state.options.debug:
-                    bd._debugger(state=state)
+                if "i" in simstate.options.debug:
+                    bd._debugger(simstate)
 
         except RuntimeError as err:
             # bad things happens, print a message and return no result
             print("unrecoverable error in evaluation: ", err)
             raise
 
     def blockdiagram(self, name="main") -> BlockDiagram:
@@ -794,19 +959,17 @@
         :seealso: :func:`BlockDiagram`
         """
 
         # instantiate a new blockdiagram
         bd = BlockDiagram(name=name)
 
         def new_method(cls, bd):
-
             # return a wrapper for the block constructor that automatically
             # adds the block to the diagram's blocklist
             def block_init_wrapper(self, *args, **kwargs):
-
                 block = cls(*args, bd=bd, **kwargs)  # call __init__ on the block
                 return block
 
             # return a function that invokes the class constructor
             f = block_init_wrapper
 
             # move the __init__ docstring to the class to allow BLOCK.__doc__
@@ -832,24 +995,27 @@
         return bd
 
     def DEBUG(self, debug, fmt, *args):
         if debug[0] in self.options.debug:
             print(f"DEBUG.{debug:s}: " + fmt.format(*args))
 
     def done(self, bd, block=False):
-
         if self.options.hold:
             block = self.options.hold
 
         try:
             plt.show(block=block)
         except KeyboardInterrupt:
             print("bdsim: closing all windows")
-            sys.exit(1)
-        bd.done(graphics=self.options.graphics)
+            plt.close("all")
+            # sys.exit(1)  # not sure why we have this
+            return
+        bd.done()
+        plt.close("all")
+        plt.pause(0.5)  # let the event handler do its work
 
     def closefigs(self):
         for i in range(self.simstate.fignum):
             print("close", i + 1)
             plt.close(i + 1)
             plt.pause(0.1)
         self.simstate.fignum = 0  # reset figure counter
@@ -912,22 +1078,22 @@
         - ``blockname``, upper case version of ``classname``
         - ``url`` of online documentation for the block
         - ``package`` containing the block
         - `doc` is the docstring from the class constructor
         """
 
         def parse_docstring(ds):
-
             # this should have two versions: sphinx, numpy doc styles
             import re
             from collections import OrderedDict
 
             re_isfield = re.compile(r"\s*:[a-zA-Zα-ωΑ-Ω0-9_ ]+:")
             re_field = re.compile(
-                "^\s*:(?P<field>[a-zA-Z]+)(?: +(?P<var>[a-zA-Zα-ωΑ-Ω0-9_]+))?:(?P<body>.+)$"
+                r"^\s*:(?P<field>[a-zA-Z]+)(?:"
+                r" +(?P<var>[a-zA-Zα-ωΑ-Ω0-9_]+))?:(?P<body>.+)$"
             )
 
             # a-zA-Zα-ωΑ-Ω0-9_
             def indent(s):
                 return len(s) - len(s.lstrip())
 
             fieldnames = ("param", "type", "input", "output")
@@ -1000,30 +1166,36 @@
             return params
 
         block = namedtuple("block", "name, cls, path")
 
         packages = ["bdsim", "roboticstoolbox", "machinevisiontoolbox"]
         env = os.getenv("BDSIMPATH")
         if env is not None:
-            packages.append(env.split)
+            packages += env.split(":")
         if self.packages is not None:
-            packages.append(self.packages.split(":"))
+            packages += self.packages.split(":")
 
         blocks = {}
         moduledicts = {}
         for package in packages:
             try:
                 spec = importlib.util.find_spec(".blocks", package=package)
                 if spec is None:
                     print(f"package {package} has no blocks module")
                     continue
                 pkg = spec.loader.load_module()
             except ModuleNotFoundError:
                 print(f"package {package} not found")
                 continue
+            except ImportError:
+                print(f"package {package} load error, continuing")
+                import textwrap
+
+                print(textwrap.indent(traceback.format_exc(), "    "))
+                continue
 
             moduledict = {}
 
             for name, value in pkg.__dict__.items():
                 # check if it's a valid block class
                 if not inspect.isclass(value):
                     continue
@@ -1033,37 +1205,39 @@
                     continue
 
                 if value.blockclass in ("source", "transfer", "function"):
                     # must have an output function
                     valid = (
                         hasattr(value, "output")
                         and callable(value.output)
-                        and len(inspect.signature(value.output).parameters) == 2
+                        and len(inspect.signature(value.output).parameters) == 4
                     )
                     if not valid:
-                        raise ImportError(
-                            "class {:s} has missing/improper output method".format(
-                                str(value)
+                        print(
+                            "block {:s} has missing/improper output method".format(
+                                value.__name__
                             )
                         )
+                        continue
 
                 if value.blockclass == "sink":
                     # must have a step function with at least one
                     # parameter: step(self [,state])
                     valid = (
                         hasattr(value, "step")
                         and callable(value.step)
-                        and len(inspect.signature(value.step).parameters) >= 1
+                        and len(inspect.signature(value.step).parameters) == 3
                     )
                     if not valid:
-                        raise ImportError(
-                            "class {:s} has missing/improper step method".format(
-                                str(value)
+                        print(
+                            "block {:s} has missing/improper step method".format(
+                                value.__name__
                             )
                         )
+                        continue
 
                 # add it to the dict of blocks indexed by module
                 if value.__module__ in moduledict:
                     moduledict[value.__module__].append(name)
                 else:
                     moduledict[value.__module__] = [name]
 
@@ -1164,31 +1338,85 @@
                     else:
                         print(f"{dots(k)}: {s}")
 
     def set_options(self, **options):
         self.options.set(**options)
         warnings.warn("use sim.options.OPT=VALUE instead", DeprecationWarning)
 
+    def set_globals(self, globs):
+        """
+        Set globals as specified by command line
+
+        :param globs: global variables
+        :type globs: dict
+
+        The command line option ``--global var=value`` can be used to request the change
+        of global variables.  However, actually changing them requires explicit code
+        support in the user's program after the ``BDSim`` constructor.
+
+        Example::
+
+            sim.set_globals(globals())
+
+        Messages are displayed by defaulting, indicating which variables are changed,
+        and their old and new values.
+        """
+        # handle the globals
+        for s in self.options.setglob:
+            var, value = s.split("=")
+
+            new_value = eval(value)
+            print(f"changed value of global {var} from {globs[var]} -> {new_value}")
+            globs[var] = new_value
+
+    def report(self, bd, type="summary", **kwargs):
+        """Print block diagram report
+
+        :param bd: the block diagram to be reported
+        :type bd: :class:`BlockDiagram`
+        :param type: report type, one of: "summary" (default), "lists", "schedule"
+        :type type: str, optional
+        :param style: table style, one of: ansi (default), markdown, latex
+        :type style: str
+
+        Single method wrapper for various block diagram reports.  Obeys the ``-q``
+        option to suppress all reports at runtime.
+
+        :seealso: :meth:`BlockDiagram.report_summary` :meth:`BlockDiagram.report_lists` :meth:`BlockDiagram.report_schedule`
+        """
+        if self.options.quiet:
+            return
+
+        if type == "lists":
+            bd.report_lists(**kwargs)
+        elif type == "summary":
+            bd.report_summary(**kwargs)
+        elif type == "schedule":
+            bd.report_schedule(**kwargs)
+
 
 class Options(OptionsBase):
     def __init__(self, sysargs=True, **options):
-
         default_options = {
             "backend": None,
             "tiles": "3x4",
             "graphics": True,
             "animation": False,
             "hold": True,
             "shape": None,
             "altscreen": True,
             "progress": True,
             "verbose": False,
             "debug": "",
             "simtime": None,
             "blocks": False,
+            "outfile": None,
+            "quiet": False,
+            "setparam": [],
+            "setglob": [],
         }
 
         # modify defaults according to envariable BDSIM which is comma/semicolon
         # separated list of key=value pairs
         # eg. setenv BDSIM graphics=True,hold=True
         env = os.getenv("BDSIM")
         if env is not None:
@@ -1207,15 +1435,18 @@
 
         if sysargs:
             # command line arguments and graphics
             parser = argparse.ArgumentParser(
                 prefix_chars="-+",
                 formatter_class=argparse.ArgumentDefaultsHelpFormatter,
                 description="Block diagram simulation framework",
-                epilog="set defaults using environment variable BDSIM as a single string containing command line options",
+                epilog=(
+                    "set defaults using environment variable BDSIM as a single string"
+                    " containing command line options"
+                ),
             )
             parser.add_argument(
                 "--backend",
                 "-b",
                 type=str,
                 metavar="BACKEND",
                 help="matplotlib backend to choose",
@@ -1327,14 +1558,49 @@
                 type=str,
                 metavar="[psd]",
                 help="debug flags: p/ropagate, s/tate, d/eriv, i/nteractive",
             )
             parser.add_argument(
                 "--simtime", "-S", type=str, help="simulation time: T or T,dt"
             )
+            parser.add_argument(
+                "--quiet",
+                "-q",
+                action="store_const",
+                const=True,
+                help="suppress reports",
+            )
+            parser.add_argument(
+                "-o",
+                action="store_const",
+                const="bd.out",
+                dest="outfile",
+                help="output pickled simulation results to bd.out",
+            )
+            parser.add_argument(
+                "--out",
+                type=str,
+                dest="outfile",
+                help="file to save pickled simulation results",
+            )
+            parser.add_argument(
+                "--set",
+                "-s",
+                dest="setparam",
+                action="append",
+                type=str,
+                help="override block parameter using block:param=value",
+            )
+            parser.add_argument(
+                "--global",
+                dest="setglob",
+                action="append",
+                type=str,
+                help="override global parameter using var=value",
+            )
 
             args, unknownargs = parser.parse_known_args()
             cmdline_options = vars(args)  # get args as a dictionary
             # keep only the options that are not None, ie. those that were
             # explicitly set on the command line
             cmdline_options = {
                 option: value
@@ -1354,22 +1620,24 @@
             cmdline_options = dict()  # empty dictionary
 
         super().__init__(readonly=cmdline_options, args=default_options)
 
         # now handle the passed options
         self.set(**options)
 
+        if self.verbose:
+            print(self)
+
         self._argv = unknownargs  # save non-bdsim arguments
 
     def sanity(self, options):
         # ensure graphics is enabled if animation is requested
         # ensure animation is disabled if graphics is disabled
         if "graphics" in options and "animation" in options:
             if options["animation"] and not options["graphics"]:
                 raise ValueError("cannot enable animation but disable graphics")
         elif "graphics" in options and not options["graphics"]:
             options["animation"] = False
         elif "animation" in options and options["animation"]:
             options["graphics"] = True
 
-
         return options
```

### Comparing `bdsim-1.0.0/bdsim.egg-info/PKG-INFO` & `bdsim-1.1.0/bdsim.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdsim
-Version: 1.0.0
+Version: 1.1.0
 Summary: Simulate dynamic systems expressed in block diagram form using Python
 Author-email: Peter Corke <rvc@petercorke.com>
 License: MIT License
         
         Copyright (c) 2020 Peter Corke
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: edit
 License-File: LICENSE
 
 [![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-python)
 [![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
 
 [![PyPI version](https://badge.fury.io/py/bdsim.svg)](https://badge.fury.io/py/bdsim)
 ![Python Version](https://img.shields.io/pypi/pyversions/bdsim.svg)
@@ -133,22 +134,20 @@
     13	
     14	# connect the blocks
     15	bd.connect(demand, sum[0], scope[1])
     17	bd.connect(sum, gain)
     18	bd.connect(gain, plant)
     19	bd.connect(plant, sum[1], scope[0])
     20	
-    21	bd.compile()   # check the diagram
-    22	bd.report()    # list all blocks and wires
-    23
+    21	bd.compile()          # check the diagram
+    22
+    23	sim.report(bd)   # list the system
     24  out = sim.run(bd, 5)   # simulate for 5s
-    25  sim.savefig(scope, 'scope0')
-    26  sim.done(bd, block=True)
 ```
-which is just 16 lines of executable code.
+which is just 15 lines of executable code.
 
 The red block annotations on the hand-drawn diagram are used as the names of the variables holding references to the block instance. The blocks can also have user-assigned names, see lines 8 and 11, which are used in diagnostics and as labels in plots.
 
 After the blocks are created their input and output ports need to be connected. In `bdsim` all wires are point to point, a *one-to-many* connection is implemented by *many* wires,
 for example
 ```
 bd.connect(source, dest1, dest2, ...)
@@ -162,17 +161,104 @@
 bd.connect(source[2:5], dest[3:6)
 ```
 will connect `source[2]` -> `dest[3]`, `source[3]` -> `dest[4]`, `source[4]` -> `dest[5]`.
 The number of wires in each slice must be consistent.  You could even do a cross over by connecting `source[2:5]` to `dest[6:3:-1]`.
 
 Line 21 assembles all the blocks and wires, instantiates subsystems, checks connectivity to create a flat wire list, and then builds the dataflow execution plan.
 
-Line 22 generates a report, in tabular form, showing a summary of the block diagram:
+Line 23 generates a report, in tabular form, showing a summary of the block diagram:
 
 ```
+┌────────┬──────────┬────────┬────────┬─────────────┐
+│ block  │   type   │ inport │ source │ source type │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│demand@ │ step     │        │        │             │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│gain.0  │ gain     │ 0      │ sum.0  │ float64     │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│plant   │ lti_siso │ 0      │ gain.0 │ float64     │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│scope.0 │ scope    │ 0      │ plant  │ float64     │
+│        │          │ 1      │ demand │ int         │
+├────────┼──────────┼────────┼────────┼─────────────┤
+│sum.0   │ sum      │ 0      │ demand │ int         │
+│        │          │ 1      │ plant  │ float64     │
+└────────┴──────────┴────────┴────────┴─────────────┘
+```
+
+Line 24 runs the simulation for 5 seconds 
+using the default variable-step RK45 solver and saves output values at least every 0.05s.  It
+causes the following output
+
+```
+>>> Start simulation: T = 5.00, dt = 0.050
+  Continuous state variables: 1
+     x0 =  [0.]
+  Discrete state variables:   0
+
+no graphics backend specified: Qt5Agg found, using instead of MacOSX
+
+bdsim ◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉◉ 100.0% - 0s
+
+<<< Simulation complete
+  block diagram evaluations: 784
+  block diagram exec time:   0.075 ms
+  time steps:                123
+  integration intervals:     2
+```
+
+This provides a summary of the number of states for the complete system: the number of continuous states, the number
+of discrete states, and the initial value of the state vectors.
+
+During execution a progress bar is updated and scope blocks pops up a graphical window
+
+![bdsim output](https://github.com/petercorke/bdsim/raw/master/figs/Figure_1.png)
+
+The simulation results are in a container object (`BDStruct`)
+```
+>>> out
+t      = ndarray:float64 (123,)
+x      = ndarray:float64 (123, 1)
+xnames = ['plantx0'] (list)
+ynames = [] (list)            
+```
+which contains an array of time values, an array of state values, and a list of the
+names of the state variables.
+
+By default the `.run()` method at line 24 blocks blocks the script until all figure
+windows are closed (by pressing the operating system close button or typing "q"), or the
+script is killed with SIGINT. If you want to continue the script with the figures still
+active then the `hold=False` option should be set.
+
+If we wished to also record additional outputs, we can add them as _watched_ signals
+```
+out = sim.run(bd, watch=[demand, sum])  # simulate for 5s
+```
+and now the output is
+```
+>>> out
+t      = ndarray:float64 (123,)
+x      = ndarray:float64 (123, 1)
+xnames = ['plantx0'] (list)
+y0     = ndarray:float64 (123,)
+y1     = ndarray:int64 (123,)
+ynames = ['plant[0]', 'demand[0]'] (list)
+```
+where
+
+- `t` the time vector: ndarray, shape=(M,)
+- `x` is the state vector: ndarray, shape=(M,N), one row per timestep
+- `xnames` is a list of the names of the states corresponding to columns of `x`, eg. "plant.x0"
+
+The `watch` argument is a list of outputs to log, in this case `plant` defaults
+to output port 0.  This information is saved in additional variables `y0`, `y1`
+etc.  `ynames` is a list of the names of the watched variables.
+
+An alternative system report, created by `sim.report(bd, type="lists")` is more detailed
+```
 Blocks::
 
 ┌───┬─────────┬─────┬──────┬────────┬─────────┬───────┐
 │id │    name │ nin │ nout │ nstate │ ndstate │ type  │
 ├───┼─────────┼─────┼──────┼────────┼─────────┼───────┤
 │ 0 │  demand │   0 │    1 │      0 │       0 │ step  │
 │ 1 │   sum.0 │   2 │    1 │      0 │       0 │ sum   │
@@ -189,88 +275,70 @@
 │ 0 │ 0[0] │ 1[0] │ demand[0] --> sum.0[0]   │ int     │
 │ 1 │ 0[0] │ 4[1] │ demand[0] --> scope.0[1] │ int     │
 │ 2 │ 3[0] │ 1[1] │ plant[0] --> sum.0[1]    │ float64 │
 │ 3 │ 1[0] │ 2[0] │ sum.0[0] --> gain.0[0]   │ float64 │
 │ 4 │ 2[0] │ 3[0] │ gain.0[0] --> plant[0]   │ float64 │
 │ 5 │ 3[0] │ 4[0] │ plant[0] --> scope.0[0]  │ float64 │
 └───┴──────┴──────┴──────────────────────────┴─────────┘
-
-Continuous state variables:   1
-Discrete state variables:     0
-initial state  x0 =  [0.]
 ```
 In the first table we can see key information about each block, its `id` (used internally), name, the number of input and output ports, the number of
 continuous- and discrete-time states, and the type which is the block class.  Note that the name is auto-generated based on the type, except if it has
 been set explicitly as for the blocks `demand` and `plant`.
 
 The second table shows all wires in point-to-point form, showing the start and end block and port (the block is represented here by its `id`) and the type of the object sent along the wire.
 
-Finally, there is a summary of the number of states for the complete system: the number of continuous states, the number
-of discrete states, and the initial value of the continuous state vector.
-
-Line 24 runs the simulation for 5 seconds 
-using the default variable-step RK45 solver and saves output values at least every 0.1s.  The scope block pops up a graph
-
-![bdsim output](https://github.com/petercorke/bdsim/raw/master/figs/Figure_1.png)
-
-The simulation results are in a container object
+To save figures we need to make two modifications, changing line 4 to
 ```
->>> out
-results:
-t           | ndarray (67,)
-x           | ndarray (67, 1)
-xnames      | list              
+     4  sim = bdsim.BDSim(hold=False)  # create simulator
 ```
-which contains an array of time values, an array of state values, and a list of the names of the state variables.
-
-Line 25 saves the content of the scope to be saved in the file called `scope0.pdf`.
-
-Line 26 blocks the script until all figure windows are closed, or the script is killed with SIGINT.
-
-The result `out` is effectively a structure with elements
-
+which prevents `.run()` from blocking and then deleting all the figures.
+Then, after the `.run()` we add 
 ```
->>> out
-results:
-t           | ndarray (67,)
-x           | ndarray (67, 1)
-xnames      | list        
-y0          | ndarray (67,)
-y1          | ndarray (67,)
-ynames      | list   
+     25 scope.savefig()  # save scope figure
 ```
-where
+If the filename is not given it defaults to the block name, in this case `scope.0.pdf`.
 
-- `t` the time vector: ndarray, shape=(M,)
-- `x` is the state vector: ndarray, shape=(M,N), one row per timestep
-- `xnames` is a list of the names of the states corresponding to columns of `x`, eg. "plant.x0"
 
-The `watch` argument is a list of outputs to log, in this case `plant` defaults
-to output port 0.  This information is saved in additional variables `y0`, `y1`
-etc.  `ynames` is a list of the names of the watched variables.
+The output can be pickled and written to a file
 
-Line 29 saves the scope graphics as a PDF file.
+```[shell]
+examples/eg1.py -o
+python -mpickle bd.out
+t      = ndarray:float64 (123,)
+x      = ndarray:float64 (123, 1)
+xnames = ['plantx0'] (list)
+y0     = ndarray:float64 (123,)
+y1     = ndarray:int64 (123,)
+ynames = ['plant[0]', 'demand[0]'] (list)
+```
 
-Line 30 blocks until the last figure is dismissed.
+by default the results are written to `bd.out`, use the option `--out FILE` to set it
+to a specific value.
 
-More details on this Wiki about:
+The block parameters can also be overridden from the command line without having to 
+edit the code.  To increase the loop gain we could write:
+```[shell]
+examples/eg1.py --set gain.0:K=20
+```
 
-- [Adding blocks](Adding-blocks)
-- [Connecting blocks](Connecting-blocks)
-- [Running the simulation](Running)
+More details on this Wiki about:
 
+- [Adding blocks](https://github.com/petercorke/bdsim/wiki/Adding-blocks)
+- [Connecting blocks](https://github.com/petercorke/bdsim/wiki/Connecting-blocks)
+- [Running the simulation](https://github.com/petercorke/bdsim/wiki/Running)
+- [Command line options](https://github.com/petercorke/bdsim/wiki/Runtime-options)
 
 ## Other examples
 
 In the folder `bdsim/examples` you can find a few other runnable examples:
 
 - [`eg1.py`](https://github.com/petercorke/bdsim/blob/master/examples/eg1.py) the example given above
 - [`waveform.py`](https://github.com/petercorke/bdsim/blob/master/examples/waveform.py) two signal generators connected to two scopes
 
-Examples from Chapter four of _Robotics, Vision & Control (2017)_:
+Examples from Chapter four of _Robotics, Vision & Control 2e (2017)_:
 
 - [`rvc4_2.py`](https://github.com/petercorke/bdsim/blob/master/examples/rvc4_2.py) Fig 4.2 - a car-like vehicle with bicycle kinematics driven by a rectangular pulse steering signal
 - [`rvc4_4.py`](https://github.com/petercorke/bdsim/blob/master/examples/rvc4_4.py) Fig 4.4 - a car-like vehicle driving to a point
 
 ![RVC Figure 4.4](https://github.com/petercorke/bdsim/raw/master/figs/rvc4_4.gif)
 
 - [`rvc4_6.py`](https://github.com/petercorke/bdsim/blob/master/examples/rvc4_6.py) Fig 4.6 - a car-like vehicle driving to/along a line
@@ -308,15 +376,14 @@
     14  scope[0] = plant
     15  scope[1] = demand
     16  plant[0] = 10 * (demand - plant)
     17
     18  bd.compile()   # check the diagram
     19  bd.report()    # list all blocks and wires
     20
-    21  sim.set_options(animation=True)
     22  out = sim.run(bd, 5, watch=[plant,])  # simulate for 5s
 ```
 This requires fewer lines of code and the code is more readable. Importantly, it results in in *exactly the same* block diagram in terms of blocks and wires
 ```
 Wires::
 
 ┌───┬──────┬──────┬──────────────────────────────┬─────────┐
@@ -346,14 +413,14 @@
 
 * parse the JSON file
 * instantiate all blocks and wires
 * compile and run the diagram
 
 # Article
 
-I published [this article on LinkedIn](https://www.linkedin.com/in/petercorke/recent-activity/shares/), which describes the thouhgt process behind bdsim.
+I published [this article on LinkedIn](https://www.linkedin.com/pulse/journey-toward-open-source-block-diagram-simulation-peter-corke/?trackingId=wrJYinHUgAHDq63Nv65PnA%3D%3D), which describes the thought process behind bdsim.
 
 # Limitations
 
 There are lots!  The biggest is that `bdsim` is based on a very standard variable-step integrator from the scipy library.  For discontinuous inputs (step, square wave, triangle wave, piecewise constant) the transitions get missed.  This also makes it inaccurate to simulate hybrid discrete-continuous time systems.  We really need a better integrator, perhaps [`odedc`](https://help.scilab.org/docs/6.1.0/en_US/odedc.html) from SciLab could be integrated.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bdsim Version: 1.0.0 Summary: Simulate dynamic
+Metadata-Version: 2.1 Name: bdsim Version: 1.1.0 Summary: Simulate dynamic
 systems expressed in block diagram form using Python Author-email: Peter Corke
 petercorke.com> License: MIT License Copyright (c) 2020 Peter Corke Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -16,30 +16,31 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: homepage, https://github.com/petercorke/
 bdsim Project-URL: documentation, https://petercorke.github.io/bdsim/ Project-
 URL: repository, https://github.com/petercorke/bdsim Keywords: python,block
 diagram,dynamic simulation Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev Provides-Extra: docs License-File: LICENSE [![A
-Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-
-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/
-petercorke/robotics-toolbox-python) [![QUT Centre for Robotics Open Source]
-(https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://
-qcr.github.io) [![PyPI version](https://badge.fury.io/py/bdsim.svg)](https://
-badge.fury.io/py/bdsim) ![Python Version](https://img.shields.io/pypi/
-pyversions/bdsim.svg) [![License: MIT](https://img.shields.io/badge/License-
-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Build Status](https://
-github.com/petercorke/bdsim/workflows/build/badge.svg?branch=master)](https://
-github.com/petercorke/bdsim/actions?query=workflow%3Abuild) [![Coverage](https:
-//codecov.io/gh/petercorke/bdsim/branch/master/graph/badge.svg)](https://
-codecov.io/gh/petercorke/bdsim) [![PyPI - Downloads](https://img.shields.io/
-pypi/dm/bdsim)](https://pypistats.org/packages/bdsim) [![GitHub stars](https://
-img.shields.io/github/stars/petercorke/bdsim.svg?style=social&label=Star)]
-(https://GitHub.com/petercorke/bdsim/stargazers/)
+markdown Provides-Extra: dev Provides-Extra: docs Provides-Extra: edit License-
+File: LICENSE [![A Python Robotics Package](https://raw.githubusercontent.com/
+petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)]
+(https://github.com/petercorke/robotics-toolbox-python) [![QUT Centre for
+Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/
+badge.svg)](https://qcr.github.io) [![PyPI version](https://badge.fury.io/py/
+bdsim.svg)](https://badge.fury.io/py/bdsim) ![Python Version](https://
+img.shields.io/pypi/pyversions/bdsim.svg) [![License: MIT](https://
+img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/
+MIT) [![Build Status](https://github.com/petercorke/bdsim/workflows/build/
+badge.svg?branch=master)](https://github.com/petercorke/bdsim/
+actions?query=workflow%3Abuild) [![Coverage](https://codecov.io/gh/petercorke/
+bdsim/branch/master/graph/badge.svg)](https://codecov.io/gh/petercorke/bdsim)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/bdsim)](https://
+pypistats.org/packages/bdsim) [![GitHub stars](https://img.shields.io/github/
+stars/petercorke/bdsim.svg?style=social&label=Star)](https://GitHub.com/
+petercorke/bdsim/stargazers/)
                                       A Python block diagram simulation package
                                           * GitHub_repository
 [https://github.com/petercorke/bdsim/     * Documentation
 raw/master/figs/                          * Wiki_(examples_and_details)
 BDSimLogo_NoBackgnd@2x.png]               * Installation
                                           * Dependencies: numpy, scipy,
                                             matplotlib, ansitable, ffmpeg (if
@@ -92,38 +93,84 @@
 examples/eg1.py)) ```python 1 #!/usr/bin/env python3 2 import bdsim 4 sim =
 bdsim.BDSim() # create simulator 5 bd = sim.blockdiagram() # create an empty
 block diagram 6 7 # define the blocks 8 demand = bd.STEP(T=1, name='demand') 9
 sum = bd.SUM('+-') 10 gain = bd.GAIN(10) 11 plant = bd.LTI_SISO(0.5, [2, 1],
 name='plant') 12 scope = bd.SCOPE(styles=['k', 'r--']) 13 14 # connect the
 blocks 15 bd.connect(demand, sum[0], scope[1]) 17 bd.connect(sum, gain) 18
 bd.connect(gain, plant) 19 bd.connect(plant, sum[1], scope[0]) 20 21 bd.compile
-() # check the diagram 22 bd.report() # list all blocks and wires 23 24 out =
-sim.run(bd, 5) # simulate for 5s 25 sim.savefig(scope, 'scope0') 26 sim.done
-(bd, block=True) ``` which is just 16 lines of executable code. The red block
-annotations on the hand-drawn diagram are used as the names of the variables
-holding references to the block instance. The blocks can also have user-
-assigned names, see lines 8 and 11, which are used in diagnostics and as labels
-in plots. After the blocks are created their input and output ports need to be
-connected. In `bdsim` all wires are point to point, a *one-to-many* connection
-is implemented by *many* wires, for example ``` bd.connect(source, dest1,
-dest2, ...) ``` creates individual wires from `source` -> `dest1`, `source` -
-> `dest2` and so on. Ports are designated using Python indexing notation, for
-example `block[2]` is port 2 (the third port) of `block`. Whether it is an
-input or output port depends on context. In the example above an index on the
-first argument refers to an output port, while on the second (or subsequent)
-arguments it refers to an input port. If a block has only a single input or
-output port then no index is required, 0 is assumed. A group of ports can be
-denoted using slice notation, for example ``` bd.connect(source[2:5], dest[3:6)
-``` will connect `source[2]` -> `dest[3]`, `source[3]` -> `dest[4]`, `source
-[4]` -> `dest[5]`. The number of wires in each slice must be consistent. You
-could even do a cross over by connecting `source[2:5]` to `dest[6:3:-1]`. Line
-21 assembles all the blocks and wires, instantiates subsystems, checks
+() # check the diagram 22 23 sim.report(bd) # list the system 24 out = sim.run
+(bd, 5) # simulate for 5s ``` which is just 15 lines of executable code. The
+red block annotations on the hand-drawn diagram are used as the names of the
+variables holding references to the block instance. The blocks can also have
+user-assigned names, see lines 8 and 11, which are used in diagnostics and as
+labels in plots. After the blocks are created their input and output ports need
+to be connected. In `bdsim` all wires are point to point, a *one-to-many*
+connection is implemented by *many* wires, for example ``` bd.connect(source,
+dest1, dest2, ...) ``` creates individual wires from `source` -> `dest1`,
+`source` -> `dest2` and so on. Ports are designated using Python indexing
+notation, for example `block[2]` is port 2 (the third port) of `block`. Whether
+it is an input or output port depends on context. In the example above an index
+on the first argument refers to an output port, while on the second (or
+subsequent) arguments it refers to an input port. If a block has only a single
+input or output port then no index is required, 0 is assumed. A group of ports
+can be denoted using slice notation, for example ``` bd.connect(source[2:5],
+dest[3:6) ``` will connect `source[2]` -> `dest[3]`, `source[3]` -> `dest[4]`,
+`source[4]` -> `dest[5]`. The number of wires in each slice must be consistent.
+You could even do a cross over by connecting `source[2:5]` to `dest[6:3:-1]`.
+Line 21 assembles all the blocks and wires, instantiates subsystems, checks
 connectivity to create a flat wire list, and then builds the dataflow execution
-plan. Line 22 generates a report, in tabular form, showing a summary of the
-block diagram: ``` Blocks::
+plan. Line 23 generates a report, in tabular form, showing a summary of the
+block diagram: ```
+ââââââââââ¬âââââââââââ¬âââââââââ¬âââââââââ¬ââââââââââââââ
+â block â type â inport â source â source type â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âdemand@ â step â â â â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âgain.0 â gain â 0 â sum.0 â float64 â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âplant â lti_siso â 0 â gain.0 â float64 â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âscope.0 â scope â 0 â plant â float64 â â â â 1 â demand
+â int â
+ââââââââââ¼âââââââââââ¼âââââââââ¼âââââââââ¼ââââââââââââââ¤
+âsum.0 â sum â 0 â demand â int â â â â 1 â plant â
+float64 â
+ââââââââââ´âââââââââââ´âââââââââ´âââââââââ´ââââââââââââââ
+``` Line 24 runs the simulation for 5 seconds using the default variable-step
+RK45 solver and saves output values at least every 0.05s. It causes the
+following output ``` >>> Start simulation: T = 5.00, dt = 0.050 Continuous
+state variables: 1 x0 = [0.] Discrete state variables: 0 no graphics backend
+specified: Qt5Agg found, using instead of MacOSX bdsim
+ââââââââââââââââââââââââââââââââ
+100.0% - 0s <<< Simulation complete block diagram evaluations: 784 block
+diagram exec time: 0.075 ms time steps: 123 integration intervals: 2 ``` This
+provides a summary of the number of states for the complete system: the number
+of continuous states, the number of discrete states, and the initial value of
+the state vectors. During execution a progress bar is updated and scope blocks
+pops up a graphical window ![bdsim output](https://github.com/petercorke/bdsim/
+raw/master/figs/Figure_1.png) The simulation results are in a container object
+(`BDStruct`) ``` >>> out t = ndarray:float64 (123,) x = ndarray:float64 (123,
+1) xnames = ['plantx0'] (list) ynames = [] (list) ``` which contains an array
+of time values, an array of state values, and a list of the names of the state
+variables. By default the `.run()` method at line 24 blocks blocks the script
+until all figure windows are closed (by pressing the operating system close
+button or typing "q"), or the script is killed with SIGINT. If you want to
+continue the script with the figures still active then the `hold=False` option
+should be set. If we wished to also record additional outputs, we can add them
+as _watched_ signals ``` out = sim.run(bd, watch=[demand, sum]) # simulate for
+5s ``` and now the output is ``` >>> out t = ndarray:float64 (123,) x =
+ndarray:float64 (123, 1) xnames = ['plantx0'] (list) y0 = ndarray:float64
+(123,) y1 = ndarray:int64 (123,) ynames = ['plant[0]', 'demand[0]'] (list) ```
+where - `t` the time vector: ndarray, shape=(M,) - `x` is the state vector:
+ndarray, shape=(M,N), one row per timestep - `xnames` is a list of the names of
+the states corresponding to columns of `x`, eg. "plant.x0" The `watch` argument
+is a list of outputs to log, in this case `plant` defaults to output port 0.
+This information is saved in additional variables `y0`, `y1` etc. `ynames` is a
+list of the names of the watched variables. An alternative system report,
+created by `sim.report(bd, type="lists")` is more detailed ``` Blocks::
 âââââ¬ââââââââââ¬ââââââ¬âââââââ¬âââââââââ¬ââââââââââ¬ââââââââ
 âid â name â nin â nout â nstate â ndstate â type â
 âââââ¼ââââââââââ¼ââââââ¼âââââââ¼âââââââââ¼ââââââââââ¼ââââââââ¤
 â 0 â demand â 0 â 1 â 0 â 0 â step â â 1 â sum.0 â 2 â
 1 â 0 â 0 â sum â â 2 â gain.0 â 1 â 1 â 0 â 0 â gain â
 â 3 â plant â 1 â 1 â 1 â 0 â LTI â â 4 â scope.0 â 2 â
 0 â 0 â 0 â scope â
@@ -135,79 +182,71 @@
 â 0 â 0[0] â 1[0] â demand[0] --> sum.0[0] â int â â 1 â 0[0]
 â 4[1] â demand[0] --> scope.0[1] â int â â 2 â 3[0] â 1[1] â
 plant[0] --> sum.0[1] â float64 â â 3 â 1[0] â 2[0] â sum.0[0] --
 > gain.0[0] â float64 â â 4 â 2[0] â 3[0] â gain.0[0] --> plant[0]
 â float64 â â 5 â 3[0] â 4[0] â plant[0] --> scope.0[0] â float64
 â
 âââââ´âââââââ´âââââââ´âââââââââââââââââââââââââââ´ââââââââââ
-Continuous state variables: 1 Discrete state variables: 0 initial state x0 =
-[0.] ``` In the first table we can see key information about each block, its
-`id` (used internally), name, the number of input and output ports, the number
-of continuous- and discrete-time states, and the type which is the block class.
+``` In the first table we can see key information about each block, its `id`
+(used internally), name, the number of input and output ports, the number of
+continuous- and discrete-time states, and the type which is the block class.
 Note that the name is auto-generated based on the type, except if it has been
 set explicitly as for the blocks `demand` and `plant`. The second table shows
 all wires in point-to-point form, showing the start and end block and port (the
 block is represented here by its `id`) and the type of the object sent along
-the wire. Finally, there is a summary of the number of states for the complete
-system: the number of continuous states, the number of discrete states, and the
-initial value of the continuous state vector. Line 24 runs the simulation for 5
-seconds using the default variable-step RK45 solver and saves output values at
-least every 0.1s. The scope block pops up a graph ![bdsim output](https://
-github.com/petercorke/bdsim/raw/master/figs/Figure_1.png) The simulation
-results are in a container object ``` >>> out results: t | ndarray (67,) x |
-ndarray (67, 1) xnames | list ``` which contains an array of time values, an
-array of state values, and a list of the names of the state variables. Line 25
-saves the content of the scope to be saved in the file called `scope0.pdf`.
-Line 26 blocks the script until all figure windows are closed, or the script is
-killed with SIGINT. The result `out` is effectively a structure with elements
-``` >>> out results: t | ndarray (67,) x | ndarray (67, 1) xnames | list y0 |
-ndarray (67,) y1 | ndarray (67,) ynames | list ``` where - `t` the time vector:
-ndarray, shape=(M,) - `x` is the state vector: ndarray, shape=(M,N), one row
-per timestep - `xnames` is a list of the names of the states corresponding to
-columns of `x`, eg. "plant.x0" The `watch` argument is a list of outputs to
-log, in this case `plant` defaults to output port 0. This information is saved
-in additional variables `y0`, `y1` etc. `ynames` is a list of the names of the
-watched variables. Line 29 saves the scope graphics as a PDF file. Line 30
-blocks until the last figure is dismissed. More details on this Wiki about: -
-[Adding blocks](Adding-blocks) - [Connecting blocks](Connecting-blocks) -
-[Running the simulation](Running) ## Other examples In the folder `bdsim/
-examples` you can find a few other runnable examples: - [`eg1.py`](https://
-github.com/petercorke/bdsim/blob/master/examples/eg1.py) the example given
-above - [`waveform.py`](https://github.com/petercorke/bdsim/blob/master/
-examples/waveform.py) two signal generators connected to two scopes Examples
-from Chapter four of _Robotics, Vision & Control (2017)_: - [`rvc4_2.py`]
-(https://github.com/petercorke/bdsim/blob/master/examples/rvc4_2.py) Fig 4.2 -
-a car-like vehicle with bicycle kinematics driven by a rectangular pulse
-steering signal - [`rvc4_4.py`](https://github.com/petercorke/bdsim/blob/
-master/examples/rvc4_4.py) Fig 4.4 - a car-like vehicle driving to a point !
-[RVC Figure 4.4](https://github.com/petercorke/bdsim/raw/master/figs/
-rvc4_4.gif) - [`rvc4_6.py`](https://github.com/petercorke/bdsim/blob/master/
-examples/rvc4_6.py) Fig 4.6 - a car-like vehicle driving to/along a line ![RVC
-Figure 4.6](https://github.com/petercorke/bdsim/raw/master/figs/rvc4_6.gif) -
-[`rvc4_8.py`](https://github.com/petercorke/bdsim/blob/master/examples/
-rvc4_8.py) Fig 4.8 - a car-like vehicle using pure-pursuit trajectory following
-![RVC Figure 4.6](https://github.com/petercorke/bdsim/raw/master/figs/
-rvc4_8.gif) - [`rvc4_11.py`](https://github.com/petercorke/bdsim/blob/master/
-examples/rvc4_11.py) Fig 4.11 a car-like vehicle driving to a pose ![RVC Figure
-4.11](https://github.com/petercorke/bdsim/raw/master/figs/rvc4_11.gif) Figs 4.8
-(pure pursuit) and Fig 4.21 (quadrotor control) are yet to be done. # A more
-concise way Wiring, and some simple arithmetic blocks like `GAIN`, `SUM` and
-`PROD` can be implicitly generated by overloaded Python operators. This strikes
-a nice balance between block diagram coding and Pythonic programming. ``` 1 #!/
-usr/bin/env python3 2 3 import bdsim 4 5 sim = bdsim.BDSim() # create simulator
-6 bd = sim.blockdiagram() # create an empty block diagram 7 8 # define the
-blocks 9 demand = bd.STEP(T=1, name='demand') 10 plant = bd.LTI_SISO(0.5, [2,
-1], name='plant') 11 scope = bd.SCOPE(styles=['k', 'r--'], movie='eg1.mp4') 12
-13 # connect the blocks using Python syntax 14 scope[0] = plant 15 scope[1] =
-demand 16 plant[0] = 10 * (demand - plant) 17 18 bd.compile() # check the
-diagram 19 bd.report() # list all blocks and wires 20 21 sim.set_options
-(animation=True) 22 out = sim.run(bd, 5, watch=[plant,]) # simulate for 5s ```
-This requires fewer lines of code and the code is more readable. Importantly,
-it results in in *exactly the same* block diagram in terms of blocks and wires
-``` Wires::
+the wire. To save figures we need to make two modifications, changing line 4 to
+``` 4 sim = bdsim.BDSim(hold=False) # create simulator ``` which prevents `.run
+()` from blocking and then deleting all the figures. Then, after the `.run()`
+we add ``` 25 scope.savefig() # save scope figure ``` If the filename is not
+given it defaults to the block name, in this case `scope.0.pdf`. The output can
+be pickled and written to a file ```[shell] examples/eg1.py -o python -mpickle
+bd.out t = ndarray:float64 (123,) x = ndarray:float64 (123, 1) xnames =
+['plantx0'] (list) y0 = ndarray:float64 (123,) y1 = ndarray:int64 (123,) ynames
+= ['plant[0]', 'demand[0]'] (list) ``` by default the results are written to
+`bd.out`, use the option `--out FILE` to set it to a specific value. The block
+parameters can also be overridden from the command line without having to edit
+the code. To increase the loop gain we could write: ```[shell] examples/eg1.py
+--set gain.0:K=20 ``` More details on this Wiki about: - [Adding blocks](https:
+//github.com/petercorke/bdsim/wiki/Adding-blocks) - [Connecting blocks](https:/
+/github.com/petercorke/bdsim/wiki/Connecting-blocks) - [Running the simulation]
+(https://github.com/petercorke/bdsim/wiki/Running) - [Command line options]
+(https://github.com/petercorke/bdsim/wiki/Runtime-options) ## Other examples In
+the folder `bdsim/examples` you can find a few other runnable examples: -
+[`eg1.py`](https://github.com/petercorke/bdsim/blob/master/examples/eg1.py) the
+example given above - [`waveform.py`](https://github.com/petercorke/bdsim/blob/
+master/examples/waveform.py) two signal generators connected to two scopes
+Examples from Chapter four of _Robotics, Vision & Control 2e (2017)_: -
+[`rvc4_2.py`](https://github.com/petercorke/bdsim/blob/master/examples/
+rvc4_2.py) Fig 4.2 - a car-like vehicle with bicycle kinematics driven by a
+rectangular pulse steering signal - [`rvc4_4.py`](https://github.com/
+petercorke/bdsim/blob/master/examples/rvc4_4.py) Fig 4.4 - a car-like vehicle
+driving to a point ![RVC Figure 4.4](https://github.com/petercorke/bdsim/raw/
+master/figs/rvc4_4.gif) - [`rvc4_6.py`](https://github.com/petercorke/bdsim/
+blob/master/examples/rvc4_6.py) Fig 4.6 - a car-like vehicle driving to/along a
+line ![RVC Figure 4.6](https://github.com/petercorke/bdsim/raw/master/figs/
+rvc4_6.gif) - [`rvc4_8.py`](https://github.com/petercorke/bdsim/blob/master/
+examples/rvc4_8.py) Fig 4.8 - a car-like vehicle using pure-pursuit trajectory
+following ![RVC Figure 4.6](https://github.com/petercorke/bdsim/raw/master/
+figs/rvc4_8.gif) - [`rvc4_11.py`](https://github.com/petercorke/bdsim/blob/
+master/examples/rvc4_11.py) Fig 4.11 a car-like vehicle driving to a pose ![RVC
+Figure 4.11](https://github.com/petercorke/bdsim/raw/master/figs/rvc4_11.gif)
+Figs 4.8 (pure pursuit) and Fig 4.21 (quadrotor control) are yet to be done. #
+A more concise way Wiring, and some simple arithmetic blocks like `GAIN`, `SUM`
+and `PROD` can be implicitly generated by overloaded Python operators. This
+strikes a nice balance between block diagram coding and Pythonic programming.
+``` 1 #!/usr/bin/env python3 2 3 import bdsim 4 5 sim = bdsim.BDSim() # create
+simulator 6 bd = sim.blockdiagram() # create an empty block diagram 7 8 #
+define the blocks 9 demand = bd.STEP(T=1, name='demand') 10 plant = bd.LTI_SISO
+(0.5, [2, 1], name='plant') 11 scope = bd.SCOPE(styles=['k', 'r--'],
+movie='eg1.mp4') 12 13 # connect the blocks using Python syntax 14 scope[0] =
+plant 15 scope[1] = demand 16 plant[0] = 10 * (demand - plant) 17 18 bd.compile
+() # check the diagram 19 bd.report() # list all blocks and wires 20 22 out =
+sim.run(bd, 5, watch=[plant,]) # simulate for 5s ``` This requires fewer lines
+of code and the code is more readable. Importantly, it results in in *exactly
+the same* block diagram in terms of blocks and wires ``` Wires::
 âââââ¬âââââââ¬âââââââ¬âââââââââââââââââââââââââââââââ¬ââââââââââ
 âid â from â to â description â type â
 âââââ¼âââââââ¼âââââââ¼âââââââââââââââââââââââââââââââ¼ââââââââââ¤
 â 0 â 1[0] â 2[0] â plant[0] --> scope.0[0] â float64 â â 1 â 0
 [0] â 2[1] â demand[0] --> scope.0[1] â int â â 2 â 0[0] â 3[0]
 â demand[0] --> _sum.0[0] â int â â 3 â 1[0] â 3[1] â plant[0] --
 > _sum.0[1] â float64 â â 4 â 3[0] â 4[0] â _sum.0[0] --> _gain.0
@@ -218,16 +257,17 @@
 bdedit: the graphical editing tool ![block diagram](https://github.com/
 petercorke/bdsim/raw/master/figs/eg1-bdedit.png) `bdedit` is a multi-platform
 PyQt5-based graphical tool to create, edit, render and execute block diagram
 models. From the examples folder ``` % bdedit eg1.bd ``` will create a display
 like that shown above. Pushing the run button, top left (triangle in circle)
 will spawn `bdrun` as a subprocess which will: * parse the JSON file *
 instantiate all blocks and wires * compile and run the diagram # Article I
-published [this article on LinkedIn](https://www.linkedin.com/in/petercorke/
-recent-activity/shares/), which describes the thouhgt process behind bdsim. #
-Limitations There are lots! The biggest is that `bdsim` is based on a very
-standard variable-step integrator from the scipy library. For discontinuous
-inputs (step, square wave, triangle wave, piecewise constant) the transitions
-get missed. This also makes it inaccurate to simulate hybrid discrete-
-continuous time systems. We really need a better integrator, perhaps [`odedc`]
-(https://help.scilab.org/docs/6.1.0/en_US/odedc.html) from SciLab could be
-integrated.
+published [this article on LinkedIn](https://www.linkedin.com/pulse/journey-
+toward-open-source-block-diagram-simulation-peter-corke/
+?trackingId=wrJYinHUgAHDq63Nv65PnA%3D%3D), which describes the thought process
+behind bdsim. # Limitations There are lots! The biggest is that `bdsim` is
+based on a very standard variable-step integrator from the scipy library. For
+discontinuous inputs (step, square wave, triangle wave, piecewise constant) the
+transitions get missed. This also makes it inaccurate to simulate hybrid
+discrete-continuous time systems. We really need a better integrator, perhaps
+[`odedc`](https://help.scilab.org/docs/6.1.0/en_US/odedc.html) from SciLab
+could be integrated.
```

### Comparing `bdsim-1.0.0/pyproject.toml` & `bdsim-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "bdsim"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Peter Corke", email="rvc@petercorke.com" },
 ]
 
 dependencies = [
     "numpy>=1.17.4",
     "scipy", 
     "matplotlib", 
     "spatialmath-python",
     "ansitable",
     "progress",
+    "PyQt5",
 ]
 license = { file = "LICENSE" }
 
 description = "Simulate dynamic systems expressed in block diagram form using Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -35,45 +36,61 @@
 repository = "https://github.com/petercorke/bdsim"
 
 [project.optional-dependencies]
 
 dev = [
     "sympy",
     "pytest",
-    "pytest-cov",
+    "pytest-timeout",
+    "pytest-xvfb",
     "coverage",
-    "codecov",
-    "recommonmark",
     "flake8"
 ]
 
 docs = [
     "sphinx", 
-    "sphinx_rtd_theme", 
+    "sphinx-rtd-theme", 
     "sphinx-autorun", 
     "sphinxcontrib-jsmath", 
-    "sphinx_markdown_tables",
+    "sphinx-markdown-tables",
+    "sphinx-autodoc-typehints",
+    "sphinx-favicon",
+]
+
+edit = [
+    "PyQt5",
+    "PIL",
 ]
 
 [project.scripts]
 
-bdedit = "bdsim.bdedit:main"
 bdrun = "bdsim:bdrun"
+bdtex2icon = "bdsim.tex2icon:main"
+
+[project.gui-scripts]
+
+# ideally this would only happen if [edit] option given
+bdedit = "bdsim.bdedit:main"
+
 
 [build-system]
 
 requires = ["setuptools", "oldest-supported-numpy"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 
 packages = [
     "bdsim",
     "bdsim.blocks",
+    "bdsim.bdedit",
 ]
 
 [tool.black]
 line-length = 88
 target-version = ['py37']
 
+[tool.pytest.ini_options]
+testpaths = "tests"
+
 [tool.coverage.run]
-omit = ["tex2icon.py", "io.py", "vision.py", "bdsim/bdedit/*.py"]
+omit = ["tex2icon.py", "io.py", "vision.py", "bdsim/bdedit/*.py", "tk_editor/*.py", "examples/RVC3/*.py"]
```

