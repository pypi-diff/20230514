# Comparing `tmp/manim_lamination_builder-0.2.0.tar.gz` & `tmp/manim_lamination_builder-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_lamination_builder-0.2.0.tar", last modified: Sat May 13 16:27:15 2023, max compression
+gzip compressed data, was "manim_lamination_builder-0.2.1.tar", last modified: Sun May 14 20:27:42 2023, max compression
```

## Comparing `manim_lamination_builder-0.2.0.tar` & `manim_lamination_builder-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-13 16:27:15.891479 manim_lamination_builder-0.2.0/
--rw-r--r--   0 forrest   (1000) forrest   (1000)    34523 2023-02-24 00:36:13.000000 manim_lamination_builder-0.2.0/LICENSE
--rw-r--r--   0 forrest   (1000) forrest   (1000)    43066 2023-05-13 16:27:15.891479 manim_lamination_builder-0.2.0/PKG-INFO
--rw-r--r--   0 forrest   (1000) forrest   (1000)     2724 2023-04-02 00:57:01.000000 manim_lamination_builder-0.2.0/README.md
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-13 16:27:15.891479 manim_lamination_builder-0.2.0/manim_lamination_builder/
--rw-r--r--   0 forrest   (1000) forrest   (1000)      960 2023-05-13 16:25:33.000000 manim_lamination_builder-0.2.0/manim_lamination_builder/__init__.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4412 2023-05-13 16:17:33.000000 manim_lamination_builder-0.2.0/manim_lamination_builder/animation.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3132 2023-05-13 15:20:55.000000 manim_lamination_builder-0.2.0/manim_lamination_builder/chord.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     2846 2023-05-13 15:21:01.000000 manim_lamination_builder-0.2.0/manim_lamination_builder/custom_json.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4398 2023-05-13 16:20:40.000000 manim_lamination_builder-0.2.0/manim_lamination_builder/generate.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3455 2023-05-13 15:21:27.000000 manim_lamination_builder-0.2.0/manim_lamination_builder/lamination.py
--rwxr-xr-x   0 forrest   (1000) forrest   (1000)     1600 2023-05-13 15:22:17.000000 manim_lamination_builder-0.2.0/manim_lamination_builder/main.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4464 2023-05-13 15:22:15.000000 manim_lamination_builder-0.2.0/manim_lamination_builder/morph.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     6826 2023-05-13 14:47:08.000000 manim_lamination_builder-0.2.0/manim_lamination_builder/points.py
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-13 16:27:15.891479 manim_lamination_builder-0.2.0/manim_lamination_builder.egg-info/
--rw-r--r--   0 forrest   (1000) forrest   (1000)    43066 2023-05-13 16:27:15.000000 manim_lamination_builder-0.2.0/manim_lamination_builder.egg-info/PKG-INFO
--rw-r--r--   0 forrest   (1000) forrest   (1000)      598 2023-05-13 16:27:15.000000 manim_lamination_builder-0.2.0/manim_lamination_builder.egg-info/SOURCES.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)        1 2023-05-13 16:27:15.000000 manim_lamination_builder-0.2.0/manim_lamination_builder.egg-info/dependency_links.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)       12 2023-05-13 16:27:15.000000 manim_lamination_builder-0.2.0/manim_lamination_builder.egg-info/requires.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)       25 2023-05-13 16:27:15.000000 manim_lamination_builder-0.2.0/manim_lamination_builder.egg-info/top_level.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)      668 2023-05-11 15:29:33.000000 manim_lamination_builder-0.2.0/pyproject.toml
--rw-r--r--   0 forrest   (1000) forrest   (1000)       38 2023-05-13 16:27:15.891479 manim_lamination_builder-0.2.0/setup.cfg
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-14 20:27:42.869549 manim_lamination_builder-0.2.1/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    34523 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/LICENSE
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    43796 2023-05-14 20:27:42.869549 manim_lamination_builder-0.2.1/PKG-INFO
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3429 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/README.md
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-14 20:27:42.869549 manim_lamination_builder-0.2.1/manim_lamination_builder/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      975 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/__init__.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      429 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/__main__.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4412 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/animation.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3132 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/chord.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     2846 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/custom_json.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4398 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/generate.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3470 2023-05-14 20:26:30.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/lamination.py
+-rwxr-xr-x   0 forrest   (1000) forrest   (1000)     1144 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/main.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4464 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/morph.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     6826 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/manim_lamination_builder/points.py
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-14 20:27:42.869549 manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    43796 2023-05-14 20:27:42.000000 manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/PKG-INFO
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      635 2023-05-14 20:27:42.000000 manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)        1 2023-05-14 20:27:42.000000 manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       17 2023-05-14 20:27:42.000000 manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/requires.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       25 2023-05-14 20:27:42.000000 manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/top_level.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      701 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.1/pyproject.toml
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       38 2023-05-14 20:27:42.869549 manim_lamination_builder-0.2.1/setup.cfg
```

### Comparing `manim_lamination_builder-0.2.0/LICENSE` & `manim_lamination_builder-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.0/PKG-INFO` & `manim_lamination_builder-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim_lamination_builder
-Version: 0.2.0
+Version: 0.2.1
 Summary: a replacement to lamination builder that uses manim instead of the browser
 Author-email: Forrest Hilton <forrestmhilton@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -663,29 +663,36 @@
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/ForrestHilton/manim-lamination-builder
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# WORK IN PROGRESS -- THE FEATURES NOT USED IN THE EXAMPLE DON'T WORK YET
+# WORK IN PROGRESS
+This is a re-implementation of [lamination-builder](https://csfalcione.github.io/lamination-builder/) that runs in python without dependencies on a browser and focusing on animations and convenient generation of figures. Instead it uses [Manim](https://github.com/ManimCommunity/manim/), and which has several dependencies. 
 
-This is a re-implementation of [lamination-builder](https://csfalcione.github.io/lamination-builder/) that runs in python without dependencies on a browser and focusing on convenient generation of figures. Instead it uses [Manim](https://github.com/ManimCommunity/manim/), and which has several dependencies. 
 
-The input format is as follows: A list of laminations to be placed in the figure (tilling is a best effort left to right and top to bottom Placemen based on a 16:9 screen). The blank lamination is permited.
-
-Each lamination may have of the following fields: polygons, chords (must be a list of lists of length two), point_lables, point_colors ("*" for default color which defaults to red), and points. Omissions in each field will be filled based on the fields that proceed it in the list above. Each lamination must have a "radix" which is the base.
+# Installation:
+Please refer to [to manim's installation instructions](https://docs.manim.community/en/stable/installation.html). It and its dependencies are required, with the possible exception of tex. Afterward, you can simply run
+```
+pip install manim_lamination_builder
+```
 
-# Example:
+# Usage: 
+## render multiple laminations in one image
+```
+python -m manim_lamination_builder file.json
+```
+The input format is as follows: A list of laminations to be placed in the figure (tilling is a best effort left to right and top to bottom Placemen). The blank lamination is permitted.
 ```
 [
   {
     polygons:[["_001","_010","_100"]],
     chords:[["_1","2"]],
     points: ["3"],
     radix: 4
@@ -700,33 +707,63 @@
     "radix": 4
   },
   { radix: 4}
 ]
 ```
 ![please enable images](https://github.com/ForrestHilton/python-lamination-builder/blob/main/contrived_example.png "Render of json above")
 
-# Installation: (correct python packaging is on the TODO list)
-Please refer to [to manim's installation instructions](https://docs.manim.community/en/stable/installation.html). It and its dependencies are required, with the possible exception of tex.
-```
-pip install manim json json5
-git clone https://github.com/ForrestHilton/python-lamination-builder
+## generate and render laminations to verify my research
 ```
+from manim import tempconfig
+from manim_lamination_builder import generate_unicritical_lamination, Main
 
-Add the project to you PYTHONPATH in a settings file, if you wish to import the python files.
 
-# Usage: 
-```
-/path/to/python-lamination-builder/main.py file.json
+with tempconfig({"quality": "high_quality", "preview": True}):
+    Main(generate_unicritical_lamination(4, 3)).render()
 ```
+![please enable images](https://github.com/ForrestHilton/python-lamination-builder/blob/main/example.png "Example Output from my Reasearch")
 
+## animate the leaves and points moving to their images
+Please not that sigma_d is understood as a dilation of angular position with wrapping, so the forgotten digit is recorded and used to determine how many times to wrap around. 
+```
+from manim import Scene, WHITE, tempconfig
+from manim_lamination_builder import (
+    parse_lamination,
+    curried_colorize_with_respect_to,
+    sigma,
+    AnimateLamination,
+)
+
+
+class MyScene(Scene):
+    def construct(self):
+        initial = parse_lamination(
+            '{polygons: [["_200","_002","_020"]], points:[0.1,"200","201"], radix: 3 }'
+        )
+
+        initial.auto_populate()
+        initial.colorizer = curried_colorize_with_respect_to(initial.polygons[0])
+        final = initial.apply_function(sigma)
+        mob = initial.build(3)
+        mob.submobjects[2].set_color("#008080")
+        self.add(mob)
+        self.wait(2)
+        self.play(AnimateLamination(initial, final, start_mobject=mob, run_time=5))
+        self.wait(2)
+
+
+with tempconfig(
+    {"quality": "high_quality", "preview": True, "background_color": WHITE}
+):
+    scene = MyScene()
+    scene.render()
+```
 
-Feature requests will be entertained. I have yet to see a need for any of the following features: mapping forward, pull backs, automatically placing descriptions or tittles at the top. This is intended to be used in combination with other tools like latex and your own python scripts. I hope this is a reasonable API.
-
+# Developments
 
-# example output from my research
-![please enable images](https://github.com/ForrestHilton/python-lamination-builder/blob/main/example.png "Example Output from my Reasearch")
+Feature requests will be entertained, however this is intended to be used in combination with other tools like latex and your own python scripts. I hope this is a reasonable API.
 
 # License
 Licensed under the The AGPLv3 License (AGPLv3)
 Copyright (c) 2023 Forrest M. Hilton <forrestmhilton@gmail.com>
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `manim_lamination_builder-0.2.0/README.md` & `manim_lamination_builder-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,23 @@
-# WORK IN PROGRESS -- THE FEATURES NOT USED IN THE EXAMPLE DON'T WORK YET
+# WORK IN PROGRESS
+This is a re-implementation of [lamination-builder](https://csfalcione.github.io/lamination-builder/) that runs in python without dependencies on a browser and focusing on animations and convenient generation of figures. Instead it uses [Manim](https://github.com/ManimCommunity/manim/), and which has several dependencies. 
 
-This is a re-implementation of [lamination-builder](https://csfalcione.github.io/lamination-builder/) that runs in python without dependencies on a browser and focusing on convenient generation of figures. Instead it uses [Manim](https://github.com/ManimCommunity/manim/), and which has several dependencies. 
 
-The input format is as follows: A list of laminations to be placed in the figure (tilling is a best effort left to right and top to bottom Placemen based on a 16:9 screen). The blank lamination is permited.
-
-Each lamination may have of the following fields: polygons, chords (must be a list of lists of length two), point_lables, point_colors ("*" for default color which defaults to red), and points. Omissions in each field will be filled based on the fields that proceed it in the list above. Each lamination must have a "radix" which is the base.
+# Installation:
+Please refer to [to manim's installation instructions](https://docs.manim.community/en/stable/installation.html). It and its dependencies are required, with the possible exception of tex. Afterward, you can simply run
+```
+pip install manim_lamination_builder
+```
 
-# Example:
+# Usage: 
+## render multiple laminations in one image
+```
+python -m manim_lamination_builder file.json
+```
+The input format is as follows: A list of laminations to be placed in the figure (tilling is a best effort left to right and top to bottom Placemen). The blank lamination is permitted.
 ```
 [
   {
     polygons:[["_001","_010","_100"]],
     chords:[["_1","2"]],
     points: ["3"],
     radix: 4
@@ -25,33 +32,63 @@
     "radix": 4
   },
   { radix: 4}
 ]
 ```
 ![please enable images](https://github.com/ForrestHilton/python-lamination-builder/blob/main/contrived_example.png "Render of json above")
 
-# Installation: (correct python packaging is on the TODO list)
-Please refer to [to manim's installation instructions](https://docs.manim.community/en/stable/installation.html). It and its dependencies are required, with the possible exception of tex.
-```
-pip install manim json json5
-git clone https://github.com/ForrestHilton/python-lamination-builder
+## generate and render laminations to verify my research
 ```
+from manim import tempconfig
+from manim_lamination_builder import generate_unicritical_lamination, Main
 
-Add the project to you PYTHONPATH in a settings file, if you wish to import the python files.
 
-# Usage: 
-```
-/path/to/python-lamination-builder/main.py file.json
+with tempconfig({"quality": "high_quality", "preview": True}):
+    Main(generate_unicritical_lamination(4, 3)).render()
 ```
+![please enable images](https://github.com/ForrestHilton/python-lamination-builder/blob/main/example.png "Example Output from my Reasearch")
 
+## animate the leaves and points moving to their images
+Please not that sigma_d is understood as a dilation of angular position with wrapping, so the forgotten digit is recorded and used to determine how many times to wrap around. 
+```
+from manim import Scene, WHITE, tempconfig
+from manim_lamination_builder import (
+    parse_lamination,
+    curried_colorize_with_respect_to,
+    sigma,
+    AnimateLamination,
+)
+
+
+class MyScene(Scene):
+    def construct(self):
+        initial = parse_lamination(
+            '{polygons: [["_200","_002","_020"]], points:[0.1,"200","201"], radix: 3 }'
+        )
+
+        initial.auto_populate()
+        initial.colorizer = curried_colorize_with_respect_to(initial.polygons[0])
+        final = initial.apply_function(sigma)
+        mob = initial.build(3)
+        mob.submobjects[2].set_color("#008080")
+        self.add(mob)
+        self.wait(2)
+        self.play(AnimateLamination(initial, final, start_mobject=mob, run_time=5))
+        self.wait(2)
+
+
+with tempconfig(
+    {"quality": "high_quality", "preview": True, "background_color": WHITE}
+):
+    scene = MyScene()
+    scene.render()
+```
 
-Feature requests will be entertained. I have yet to see a need for any of the following features: mapping forward, pull backs, automatically placing descriptions or tittles at the top. This is intended to be used in combination with other tools like latex and your own python scripts. I hope this is a reasonable API.
-
+# Developments
 
-# example output from my research
-![please enable images](https://github.com/ForrestHilton/python-lamination-builder/blob/main/example.png "Example Output from my Reasearch")
+Feature requests will be entertained, however this is intended to be used in combination with other tools like latex and your own python scripts. I hope this is a reasonable API.
 
 # License
 Licensed under the The AGPLv3 License (AGPLv3)
 Copyright (c) 2023 Forrest M. Hilton <forrestmhilton@gmail.com>
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `manim_lamination_builder-0.2.0/manim_lamination_builder/__init__.py` & `manim_lamination_builder-0.2.1/manim_lamination_builder/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This is a re-implementation of lamination-builder that runs in python without dependencies on a browser and focusing on convenient generation of figures. Instead it uses Manim, which has several dependencies, which you are responsible for installing in accordance with Manim's installation instructions.
+This is a re-implementation of lamination-builder that runs in python without dependencies on a browser and focusing on animations and convenient generation of figures. Instead it uses Manim, which has several dependencies, which you are responsible for installing in accordance with Manim's installation instructions.
 """
 from manim_lamination_builder.lamination import Lamination
 from manim_lamination_builder.custom_json import (
     custom_dump,
     custom_parse,
     read_file_to_laminations,
     parse_lamination,
```

### Comparing `manim_lamination_builder-0.2.0/manim_lamination_builder/animation.py` & `manim_lamination_builder-0.2.1/manim_lamination_builder/animation.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.0/manim_lamination_builder/chord.py` & `manim_lamination_builder-0.2.1/manim_lamination_builder/chord.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.0/manim_lamination_builder/custom_json.py` & `manim_lamination_builder-0.2.1/manim_lamination_builder/custom_json.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.0/manim_lamination_builder/generate.py` & `manim_lamination_builder-0.2.1/manim_lamination_builder/generate.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.0/manim_lamination_builder/lamination.py` & `manim_lamination_builder-0.2.1/manim_lamination_builder/lamination.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,8 +102,8 @@
 
     def apply_function(self, f: Callable[[UnitPoint], UnitPoint]) -> "Lamination":
         new_polygons = []
         for poly in self.polygons:
             new_poly = [f(p) for p in poly]
             new_polygons.append(new_poly)
         new_points = [f(p) for p in self.points]
-        return Lamination(new_polygons, new_points, self.radix)
+        return Lamination(new_polygons, new_points, self.radix,self.colorizer)
```

### Comparing `manim_lamination_builder-0.2.0/manim_lamination_builder/main.py` & `manim_lamination_builder-0.2.1/manim_lamination_builder/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,20 +34,7 @@
         super().__init__()
 
     def construct(self):
         self.camera.background_color = WHITE
         self.add(group(self.laminations))
 
 
-if __name__ == "__main__":
-    file = sys.argv[-1]
-    if len(sys.argv) == 1:
-        path = "/home/forrest/Desktop/manim_lamination_builder/test.json5"
-    else:
-        path = os.path.join(os.getcwd(), file)
-    laminations = read_file_to_laminations(path)
-    for lamination in laminations:
-        lamination.auto_populate()
-
-    with tempconfig({"quality": "medium_quality", "preview": True}):
-        scene = Main(laminations)
-        scene.render()
```

### Comparing `manim_lamination_builder-0.2.0/manim_lamination_builder/morph.py` & `manim_lamination_builder-0.2.1/manim_lamination_builder/morph.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.0/manim_lamination_builder/points.py` & `manim_lamination_builder-0.2.1/manim_lamination_builder/points.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.0/manim_lamination_builder.egg-info/PKG-INFO` & `manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim-lamination-builder
-Version: 0.2.0
+Version: 0.2.1
 Summary: a replacement to lamination builder that uses manim instead of the browser
 Author-email: Forrest Hilton <forrestmhilton@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -663,29 +663,36 @@
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/ForrestHilton/manim-lamination-builder
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# WORK IN PROGRESS -- THE FEATURES NOT USED IN THE EXAMPLE DON'T WORK YET
+# WORK IN PROGRESS
+This is a re-implementation of [lamination-builder](https://csfalcione.github.io/lamination-builder/) that runs in python without dependencies on a browser and focusing on animations and convenient generation of figures. Instead it uses [Manim](https://github.com/ManimCommunity/manim/), and which has several dependencies. 
 
-This is a re-implementation of [lamination-builder](https://csfalcione.github.io/lamination-builder/) that runs in python without dependencies on a browser and focusing on convenient generation of figures. Instead it uses [Manim](https://github.com/ManimCommunity/manim/), and which has several dependencies. 
 
-The input format is as follows: A list of laminations to be placed in the figure (tilling is a best effort left to right and top to bottom Placemen based on a 16:9 screen). The blank lamination is permited.
-
-Each lamination may have of the following fields: polygons, chords (must be a list of lists of length two), point_lables, point_colors ("*" for default color which defaults to red), and points. Omissions in each field will be filled based on the fields that proceed it in the list above. Each lamination must have a "radix" which is the base.
+# Installation:
+Please refer to [to manim's installation instructions](https://docs.manim.community/en/stable/installation.html). It and its dependencies are required, with the possible exception of tex. Afterward, you can simply run
+```
+pip install manim_lamination_builder
+```
 
-# Example:
+# Usage: 
+## render multiple laminations in one image
+```
+python -m manim_lamination_builder file.json
+```
+The input format is as follows: A list of laminations to be placed in the figure (tilling is a best effort left to right and top to bottom Placemen). The blank lamination is permitted.
 ```
 [
   {
     polygons:[["_001","_010","_100"]],
     chords:[["_1","2"]],
     points: ["3"],
     radix: 4
@@ -700,33 +707,63 @@
     "radix": 4
   },
   { radix: 4}
 ]
 ```
 ![please enable images](https://github.com/ForrestHilton/python-lamination-builder/blob/main/contrived_example.png "Render of json above")
 
-# Installation: (correct python packaging is on the TODO list)
-Please refer to [to manim's installation instructions](https://docs.manim.community/en/stable/installation.html). It and its dependencies are required, with the possible exception of tex.
-```
-pip install manim json json5
-git clone https://github.com/ForrestHilton/python-lamination-builder
+## generate and render laminations to verify my research
 ```
+from manim import tempconfig
+from manim_lamination_builder import generate_unicritical_lamination, Main
 
-Add the project to you PYTHONPATH in a settings file, if you wish to import the python files.
 
-# Usage: 
-```
-/path/to/python-lamination-builder/main.py file.json
+with tempconfig({"quality": "high_quality", "preview": True}):
+    Main(generate_unicritical_lamination(4, 3)).render()
 ```
+![please enable images](https://github.com/ForrestHilton/python-lamination-builder/blob/main/example.png "Example Output from my Reasearch")
 
+## animate the leaves and points moving to their images
+Please not that sigma_d is understood as a dilation of angular position with wrapping, so the forgotten digit is recorded and used to determine how many times to wrap around. 
+```
+from manim import Scene, WHITE, tempconfig
+from manim_lamination_builder import (
+    parse_lamination,
+    curried_colorize_with_respect_to,
+    sigma,
+    AnimateLamination,
+)
+
+
+class MyScene(Scene):
+    def construct(self):
+        initial = parse_lamination(
+            '{polygons: [["_200","_002","_020"]], points:[0.1,"200","201"], radix: 3 }'
+        )
+
+        initial.auto_populate()
+        initial.colorizer = curried_colorize_with_respect_to(initial.polygons[0])
+        final = initial.apply_function(sigma)
+        mob = initial.build(3)
+        mob.submobjects[2].set_color("#008080")
+        self.add(mob)
+        self.wait(2)
+        self.play(AnimateLamination(initial, final, start_mobject=mob, run_time=5))
+        self.wait(2)
+
+
+with tempconfig(
+    {"quality": "high_quality", "preview": True, "background_color": WHITE}
+):
+    scene = MyScene()
+    scene.render()
+```
 
-Feature requests will be entertained. I have yet to see a need for any of the following features: mapping forward, pull backs, automatically placing descriptions or tittles at the top. This is intended to be used in combination with other tools like latex and your own python scripts. I hope this is a reasonable API.
-
+# Developments
 
-# example output from my research
-![please enable images](https://github.com/ForrestHilton/python-lamination-builder/blob/main/example.png "Example Output from my Reasearch")
+Feature requests will be entertained, however this is intended to be used in combination with other tools like latex and your own python scripts. I hope this is a reasonable API.
 
 # License
 Licensed under the The AGPLv3 License (AGPLv3)
 Copyright (c) 2023 Forrest M. Hilton <forrestmhilton@gmail.com>
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `manim_lamination_builder-0.2.0/manim_lamination_builder.egg-info/SOURCES.txt` & `manim_lamination_builder-0.2.1/manim_lamination_builder.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 manim_lamination_builder/__init__.py
+manim_lamination_builder/__main__.py
 manim_lamination_builder/animation.py
 manim_lamination_builder/chord.py
 manim_lamination_builder/custom_json.py
 manim_lamination_builder/generate.py
 manim_lamination_builder/lamination.py
 manim_lamination_builder/main.py
 manim_lamination_builder/morph.py
```

