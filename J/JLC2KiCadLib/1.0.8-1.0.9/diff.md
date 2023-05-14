# Comparing `tmp/JLC2KiCadLib-1.0.8.tar.gz` & `tmp/JLC2KiCadLib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JLC2KiCadLib-1.0.8.tar", last modified: Thu Aug 25 05:33:54 2022, max compression
+gzip compressed data, was "JLC2KiCadLib-1.0.9.tar", last modified: Wed Oct 26 08:39:28 2022, max compression
```

## Comparing `JLC2KiCadLib-1.0.8.tar` & `JLC2KiCadLib-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-08-25 05:33:54.313809 JLC2KiCadLib-1.0.8/
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-08-25 05:33:54.313809 JLC2KiCadLib-1.0.8/JLC2KiCadLib/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4196 2022-08-23 18:33:08.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib/JLC2KiCadLib.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2022-06-12 13:02:45.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib/__init__.py
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-08-25 05:33:54.313809 JLC2KiCadLib-1.0.8/JLC2KiCadLib/footprint/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2022-08-23 16:22:03.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib/footprint/__init__.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4582 2022-08-23 19:21:56.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib/footprint/footprint.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     9775 2022-08-23 16:22:03.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib/footprint/footprint_handlers.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4395 2022-08-23 16:22:03.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib/footprint/model3d.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      574 2022-06-18 17:25:56.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib/helper.py
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-08-25 05:33:54.313809 JLC2KiCadLib-1.0.8/JLC2KiCadLib/schematic/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2022-08-23 16:22:03.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib/schematic/__init__.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     6167 2022-08-25 05:31:17.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib/schematic/schematic.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     9807 2022-08-25 05:27:57.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib/schematic/schematic_handlers.py
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-08-25 05:33:54.313809 JLC2KiCadLib-1.0.8/JLC2KiCadLib.egg-info/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4453 2022-08-25 05:33:54.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib.egg-info/PKG-INFO
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      587 2022-08-25 05:33:54.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        1 2022-08-25 05:33:54.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       64 2022-08-25 05:33:54.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib.egg-info/entry_points.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       22 2022-08-25 05:33:54.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib.egg-info/requires.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       13 2022-08-25 05:33:54.000000 JLC2KiCadLib-1.0.8/JLC2KiCadLib.egg-info/top_level.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1089 2022-06-12 13:02:45.000000 JLC2KiCadLib-1.0.8/LICENSE
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4453 2022-08-25 05:33:54.313809 JLC2KiCadLib-1.0.8/PKG-INFO
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3833 2022-08-23 18:33:08.000000 JLC2KiCadLib-1.0.8/README.md
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       38 2022-08-25 05:33:54.313809 JLC2KiCadLib-1.0.8/setup.cfg
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      997 2022-08-25 05:31:22.000000 JLC2KiCadLib-1.0.8/setup.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-10-26 08:39:28.073775 JLC2KiCadLib-1.0.9/
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-10-26 08:39:28.070442 JLC2KiCadLib-1.0.9/JLC2KiCadLib/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4179 2022-10-26 08:29:36.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib/JLC2KiCadLib.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2022-06-12 13:02:45.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib/__init__.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-10-26 08:39:28.070442 JLC2KiCadLib-1.0.9/JLC2KiCadLib/footprint/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2022-08-23 16:22:03.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib/footprint/__init__.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4651 2022-10-04 10:12:26.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib/footprint/footprint.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     9775 2022-08-23 16:22:03.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib/footprint/footprint_handlers.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4501 2022-10-04 10:12:26.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib/footprint/model3d.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      574 2022-06-18 17:25:56.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib/helper.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-10-26 08:39:28.073775 JLC2KiCadLib-1.0.9/JLC2KiCadLib/schematic/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2022-08-23 16:22:03.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib/schematic/__init__.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     6167 2022-08-25 05:31:17.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib/schematic/schematic.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     9807 2022-08-25 05:27:57.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib/schematic/schematic_handlers.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-10-26 08:39:28.070442 JLC2KiCadLib-1.0.9/JLC2KiCadLib.egg-info/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4431 2022-10-26 08:39:28.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      587 2022-10-26 08:39:28.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        1 2022-10-26 08:39:28.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       64 2022-10-26 08:39:28.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib.egg-info/entry_points.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       22 2022-10-26 08:39:28.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib.egg-info/requires.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       13 2022-10-26 08:39:28.000000 JLC2KiCadLib-1.0.9/JLC2KiCadLib.egg-info/top_level.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1089 2022-06-12 13:02:45.000000 JLC2KiCadLib-1.0.9/LICENSE
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4431 2022-10-26 08:39:28.073775 JLC2KiCadLib-1.0.9/PKG-INFO
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3811 2022-10-26 08:37:05.000000 JLC2KiCadLib-1.0.9/README.md
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       38 2022-10-26 08:39:28.073775 JLC2KiCadLib-1.0.9/setup.cfg
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      997 2022-10-26 08:35:20.000000 JLC2KiCadLib-1.0.9/setup.py
```

### Comparing `JLC2KiCadLib-1.0.8/JLC2KiCadLib/JLC2KiCadLib.py` & `JLC2KiCadLib-1.0.9/JLC2KiCadLib/JLC2KiCadLib.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 
     if args.footprint_creation:
         footprint_name, datasheet_link = create_footprint(
             footprint_component_uuid=footprint_component_uuid,
             component_id=component_id,
             footprint_lib=args.footprint_lib,
             output_dir=args.output_dir,
-            model_path_relative=args.model_path_relative,
+            model_base_variable=args.model_base_variable,
         )
     else:
-        _, datasheet_link, _ = get_footprint_info(component_id)
+        _, datasheet_link, _ = get_footprint_info(footprint_component_uuid)
         footprint_name = ""
 
     if args.schematic_creation:
         create_schematic(
             schematic_component_uuid=schematic_component_uuid,
             footprint_name=footprint_name,
             datasheet_link=datasheet_link,
@@ -57,30 +57,31 @@
     )
 
     parser.add_argument(
         "components",
         metavar="JLCPCB_part_#",
         type=str,
         nargs="+",
-        help="list of JLCPCB part # from the components you want to create",
+            help="list of JLCPCB part # from the components you want to create",
     )
 
     parser.add_argument(
         "-dir",
         dest="output_dir",
         type=str,
         default="JLC2KiCad_lib",
         help="base directory for output library files",
     )
 
     parser.add_argument(
-        "--model_path_relative",
-        dest="model_path_relative",
-        action="store_true",
-        help="use --model_path_relative if you want the 3D model to be linked to the footprint using relative instead of absolute path, default is absolute",
+        "-model_base_variable",
+        dest="model_base_variable",
+        type=str,
+        default="",
+        help="use -model_base_variable if you want to specifie the base path of the 3D model using a path variable",
     )
 
     parser.add_argument(
         "--no_footprint",
         dest="footprint_creation",
         action="store_false",
         help="use --no_footprint if you do not want to create the footprint",
```

### Comparing `JLC2KiCadLib-1.0.8/JLC2KiCadLib/footprint/footprint.py` & `JLC2KiCadLib-1.0.9/JLC2KiCadLib/footprint/footprint.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,44 +8,45 @@
 
 
 def create_footprint(
     footprint_component_uuid,
     component_id,
     footprint_lib,
     output_dir,
-    model_path_relative,
+    model_base_variable,
 ):
     logging.info("creating footprint ...")
 
     footprint_name, datasheet_link, footprint_shape = get_footprint_info(
         footprint_component_uuid
     )
 
     # init kicad footprint
     kicad_mod = Footprint(f'"{footprint_name}"')
     kicad_mod.setDescription(f"{footprint_name} footprint")  # TODO Set real description
     kicad_mod.setTags(f"{footprint_name} footprint")
 
     class footprint_info:
-        def __init__(self, footprint_name, output_dir, footprint_lib):
+        def __init__(self, footprint_name, output_dir, footprint_lib, model_base_variable):
             self.max_X, self.max_Y, self.min_X, self.min_Y = (
                 -10000,
                 -10000,
                 10000,
                 10000,
             )  # I will be using these to calculate the bounding box because the node.calculateBoundingBox() method does not seems to work for me
             self.footprint_name = footprint_name
             self.output_dir = output_dir
             self.footprint_lib = footprint_lib
-            self.model_path_relative = model_path_relative
+            self.model_base_variable = model_base_variable
 
     footprint_info = footprint_info(
         footprint_name=footprint_name,
         output_dir=output_dir,
         footprint_lib=footprint_lib,
+        model_base_variable=model_base_variable
     )
 
     # for each line in data : use the appropriate handler
     for line in footprint_shape:
         args = [
             i for i in line.split("~") if i
         ]  # split and remove empty string in list
```

### Comparing `JLC2KiCadLib-1.0.8/JLC2KiCadLib/footprint/footprint_handlers.py` & `JLC2KiCadLib-1.0.9/JLC2KiCadLib/footprint/footprint_handlers.py`

 * *Files identical despite different names*

### Comparing `JLC2KiCadLib-1.0.8/JLC2KiCadLib/footprint/model3d.py` & `JLC2KiCadLib-1.0.9/JLC2KiCadLib/footprint/model3d.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,19 +129,20 @@
             f"{footprint_info.output_dir}/{footprint_info.footprint_lib}/packages3d"
         )
 
     filename = f"{footprint_info.output_dir}/{footprint_info.footprint_lib}/packages3d/{footprint_info.footprint_name}.wrl"
     with open(filename, "w") as f:
         f.write(wrl_content)
 
-    if footprint_info.model_path_relative:
-        dirname = ""
+    if footprint_info.model_base_variable:
+        path_name = f'"$({footprint_info.model_base_variable})/{footprint_info.footprint_name}.wrl"'
     else:
-        dirname = os.getcwd().replace("\\", "/").replace("/footprint", "") + "/"
+        dirname = os.getcwd().replace("\\", "/").replace("/footprint", "")
+        path_name = f'{dirname}/{filename}'
 
     kicad_mod.append(
         Model(
-            filename=f"{dirname}{filename}",
+            filename=path_name,
             rotate=[-float(axis_rotation) for axis_rotation in rotation.split(",")],
         )
     )
-    logging.info(f"added {filename} to footprint")
+    logging.info(f"added {path_name} to footprint")
```

### Comparing `JLC2KiCadLib-1.0.8/JLC2KiCadLib/helper.py` & `JLC2KiCadLib-1.0.9/JLC2KiCadLib/helper.py`

 * *Files identical despite different names*

### Comparing `JLC2KiCadLib-1.0.8/JLC2KiCadLib/schematic/schematic.py` & `JLC2KiCadLib-1.0.9/JLC2KiCadLib/schematic/schematic.py`

 * *Files identical despite different names*

### Comparing `JLC2KiCadLib-1.0.8/JLC2KiCadLib/schematic/schematic_handlers.py` & `JLC2KiCadLib-1.0.9/JLC2KiCadLib/schematic/schematic_handlers.py`

 * *Files identical despite different names*

### Comparing `JLC2KiCadLib-1.0.8/JLC2KiCadLib.egg-info/PKG-INFO` & `JLC2KiCadLib-1.0.9/JLC2KiCadLib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JLC2KiCadLib
-Version: 1.0.8
+Version: 1.0.9
 Summary: JLC2KiCad_lib is a python script that generate a component library (schematic, footprint and 3D model) for KiCad from the JLCPCB/easyEDA library.
 Home-page: https://github.com/TousstNicolas/JLC2KiCad_lib
 Author: TousstNicolas
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -60,16 +60,16 @@
 ```
 positional arguments:
   JLCPCB_part_#         list of JLCPCB part # from the components you want to create
 
 options:
   -h, --help            show this help message and exit
   -dir OUTPUT_DIR       base directory for output library files
-  --model_path_relative
-                        use --model_path_relative if you want the 3D model to be linked to the footprint using relative instead of absolute path, default is absolute
+  -model_base_variable MODEL_BASE_VARIABLE
+                        use -model_base_variable if you want to specifie the base path of the 3D model using a path variable
   --no_footprint        use --no_footprint if you do not want to create the footprint
   --no_schematic        use --no_schematic if you do not want to create the schematic
   -schematic_lib SCHEMATIC_LIB
                         set schematic library name, default is "default_lib"
   -footprint_lib FOOTPRINT_LIB
                         set footprint library name, default is "footprint"
   -logging_level {DEBUG,INFO,WARNING,ERROR,CRITICAL}
```

### Comparing `JLC2KiCadLib-1.0.8/JLC2KiCadLib.egg-info/SOURCES.txt` & `JLC2KiCadLib-1.0.9/JLC2KiCadLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JLC2KiCadLib-1.0.8/LICENSE` & `JLC2KiCadLib-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `JLC2KiCadLib-1.0.8/PKG-INFO` & `JLC2KiCadLib-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JLC2KiCadLib
-Version: 1.0.8
+Version: 1.0.9
 Summary: JLC2KiCad_lib is a python script that generate a component library (schematic, footprint and 3D model) for KiCad from the JLCPCB/easyEDA library.
 Home-page: https://github.com/TousstNicolas/JLC2KiCad_lib
 Author: TousstNicolas
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -60,16 +60,16 @@
 ```
 positional arguments:
   JLCPCB_part_#         list of JLCPCB part # from the components you want to create
 
 options:
   -h, --help            show this help message and exit
   -dir OUTPUT_DIR       base directory for output library files
-  --model_path_relative
-                        use --model_path_relative if you want the 3D model to be linked to the footprint using relative instead of absolute path, default is absolute
+  -model_base_variable MODEL_BASE_VARIABLE
+                        use -model_base_variable if you want to specifie the base path of the 3D model using a path variable
   --no_footprint        use --no_footprint if you do not want to create the footprint
   --no_schematic        use --no_schematic if you do not want to create the schematic
   -schematic_lib SCHEMATIC_LIB
                         set schematic library name, default is "default_lib"
   -footprint_lib FOOTPRINT_LIB
                         set footprint library name, default is "footprint"
   -logging_level {DEBUG,INFO,WARNING,ERROR,CRITICAL}
```

### Comparing `JLC2KiCadLib-1.0.8/README.md` & `JLC2KiCadLib-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 ```
 positional arguments:
   JLCPCB_part_#         list of JLCPCB part # from the components you want to create
 
 options:
   -h, --help            show this help message and exit
   -dir OUTPUT_DIR       base directory for output library files
-  --model_path_relative
-                        use --model_path_relative if you want the 3D model to be linked to the footprint using relative instead of absolute path, default is absolute
+  -model_base_variable MODEL_BASE_VARIABLE
+                        use -model_base_variable if you want to specifie the base path of the 3D model using a path variable
   --no_footprint        use --no_footprint if you do not want to create the footprint
   --no_schematic        use --no_schematic if you do not want to create the schematic
   -schematic_lib SCHEMATIC_LIB
                         set schematic library name, default is "default_lib"
   -footprint_lib FOOTPRINT_LIB
                         set footprint library name, default is "footprint"
   -logging_level {DEBUG,INFO,WARNING,ERROR,CRITICAL}
```

### Comparing `JLC2KiCadLib-1.0.8/setup.py` & `JLC2KiCadLib-1.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setup(
 	name="JLC2KiCadLib",
 	description="JLC2KiCad_lib is a python script that generate a component library (schematic, footprint and 3D model) for KiCad from the JLCPCB/easyEDA library.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/TousstNicolas/JLC2KiCad_lib",
-	version="1.0.8",
+	version="1.0.9",
 	author="TousstNicolas",
 	license="MIT",
 	install_requires=["KicadModTree", "requests"],
 	packages_dir={"JLC2KiCadLib": "JLC2KiCadLib"},
 	packages=find_packages(exclude=[]),
 	entry_points={"console_scripts": ["JLC2KiCadLib = JLC2KiCadLib.JLC2KiCadLib:main"]},
 	classifiers=[
```

