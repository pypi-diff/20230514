# Comparing `tmp/torch_snippets-0.499.8.tar.gz` & `tmp/torch_snippets-0.499.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_snippets-0.499.8.tar", last modified: Fri Nov  4 21:34:56 2022, max compression
+gzip compressed data, was "torch_snippets-0.499.9.tar", last modified: Thu Nov 10 10:02:31 2022, max compression
```

## Comparing `torch_snippets-0.499.8.tar` & `torch_snippets-0.499.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 yeshwanth.y (1703077310) 826136866        0 2022-11-04 21:34:56.111436 torch_snippets-0.499.8/
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866    11357 2021-12-31 15:06:08.000000 torch_snippets-0.499.8/LICENSE
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     1061 2021-12-31 15:06:08.000000 torch_snippets-0.499.8/LICENSE.txt
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866      111 2021-12-31 15:06:08.000000 torch_snippets-0.499.8/MANIFEST.in
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     5723 2022-11-04 21:34:56.111595 torch_snippets-0.499.8/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     5009 2022-08-28 14:48:04.000000 torch_snippets-0.499.8/README.md
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     2483 2022-11-04 21:34:48.000000 torch_snippets-0.499.8/settings.ini
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866       79 2022-11-04 21:34:56.112099 torch_snippets-0.499.8/setup.cfg
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     2001 2022-06-03 13:10:38.000000 torch_snippets-0.499.8/setup.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) 826136866        0 2022-11-04 21:34:56.104766 torch_snippets-0.499.8/torch_snippets/
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866      240 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866    38859 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/_modidx.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     5125 2022-09-08 06:13:05.000000 torch_snippets-0.499.8/torch_snippets/_nbdev.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     5465 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/adapters.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     9446 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/bb_utils.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     1416 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/bokeh_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     1955 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/charts.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866       73 2022-05-07 11:30:59.000000 torch_snippets-0.499.8/torch_snippets/fastcores.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     3953 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/imgaug_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     3284 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/inspector.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     6572 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/interactive_show.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866      654 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/ipython.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866      596 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/load_defaults.py
--rwxr-xr-x   0 yeshwanth.y (1703077310) 826136866    18556 2022-11-04 21:33:47.000000 torch_snippets-0.499.8/torch_snippets/loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     3392 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/logger.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     7567 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/markup.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866      793 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/misc.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     9641 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/paths.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     1207 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/pdf_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866      601 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/registry.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     6144 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/sklegos.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866    11830 2022-10-19 12:07:21.000000 torch_snippets-0.499.8/torch_snippets/text_utils.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) 826136866        0 2022-11-04 21:34:56.109208 torch_snippets-0.499.8/torch_snippets/thinc_parser/
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866        0 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/thinc_parser/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     1082 2022-10-16 17:20:20.000000 torch_snippets-0.499.8/torch_snippets/thinc_parser/parser.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866    13239 2022-11-04 06:23:51.000000 torch_snippets-0.499.8/torch_snippets/torch_loader.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) 826136866        0 2022-11-04 21:34:56.110577 torch_snippets-0.499.8/torch_snippets/trainer/
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866       23 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/trainer/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     6804 2022-11-04 21:28:58.000000 torch_snippets-0.499.8/torch_snippets/trainer/capsule.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) 826136866        0 2022-11-04 21:34:56.108466 torch_snippets-0.499.8/torch_snippets.egg-info/
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     5723 2022-11-04 21:34:55.000000 torch_snippets-0.499.8/torch_snippets.egg-info/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866     1120 2022-11-04 21:34:55.000000 torch_snippets-0.499.8/torch_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866        1 2022-11-04 21:34:55.000000 torch_snippets-0.499.8/torch_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866       20 2022-11-04 21:34:55.000000 torch_snippets-0.499.8/torch_snippets.egg-info/entry_points.txt
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866        1 2021-12-31 15:06:08.000000 torch_snippets-0.499.8/torch_snippets.egg-info/not-zip-safe
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866      229 2022-11-04 21:34:55.000000 torch_snippets-0.499.8/torch_snippets.egg-info/requires.txt
--rw-r--r--   0 yeshwanth.y (1703077310) 826136866       15 2022-11-04 21:34:55.000000 torch_snippets-0.499.8/torch_snippets.egg-info/top_level.txt
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2022-11-10 10:02:31.111435 torch_snippets-0.499.9/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.499.9/LICENSE
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1061 2021-12-31 15:06:08.000000 torch_snippets-0.499.9/LICENSE.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.499.9/MANIFEST.in
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5723 2022-11-10 10:02:31.111589 torch_snippets-0.499.9/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5009 2022-08-28 14:48:04.000000 torch_snippets-0.499.9/README.md
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2483 2022-11-10 10:02:23.000000 torch_snippets-0.499.9/settings.ini
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2022-11-10 10:02:31.112130 torch_snippets-0.499.9/setup.cfg
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2022-06-03 13:10:38.000000 torch_snippets-0.499.9/setup.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2022-11-10 10:02:31.106986 torch_snippets-0.499.9/torch_snippets/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      240 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    38859 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/_modidx.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5125 2022-09-08 06:13:05.000000 torch_snippets-0.499.9/torch_snippets/_nbdev.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5464 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/adapters.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     9446 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/bb_utils.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1416 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/bokeh_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1955 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/charts.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.499.9/torch_snippets/fastcores.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3953 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/imgaug_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3284 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/inspector.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6572 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/interactive_show.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      654 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/ipython.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      596 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/load_defaults.py
+-rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    19593 2022-11-06 15:18:28.000000 torch_snippets-0.499.9/torch_snippets/loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3392 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/logger.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     7567 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/markup.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      793 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/misc.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     9672 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/paths.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1207 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/pdf_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      601 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/registry.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2022-11-10 10:02:05.000000 torch_snippets-0.499.9/torch_snippets/sklegos.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11830 2022-10-19 12:07:21.000000 torch_snippets-0.499.9/torch_snippets/text_utils.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2022-11-10 10:02:31.110449 torch_snippets-0.499.9/torch_snippets/thinc_parser/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/thinc_parser/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.499.9/torch_snippets/thinc_parser/parser.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    13258 2022-11-08 11:22:58.000000 torch_snippets-0.499.9/torch_snippets/torch_loader.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2022-11-10 10:02:31.111142 torch_snippets-0.499.9/torch_snippets/trainer/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/trainer/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6804 2022-11-10 10:02:06.000000 torch_snippets-0.499.9/torch_snippets/trainer/capsule.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2022-11-10 10:02:31.109819 torch_snippets-0.499.9/torch_snippets.egg-info/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5723 2022-11-10 10:02:30.000000 torch_snippets-0.499.9/torch_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1120 2022-11-10 10:02:30.000000 torch_snippets-0.499.9/torch_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2022-11-10 10:02:30.000000 torch_snippets-0.499.9/torch_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       20 2022-11-10 10:02:30.000000 torch_snippets-0.499.9/torch_snippets.egg-info/entry_points.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2021-12-31 15:06:08.000000 torch_snippets-0.499.9/torch_snippets.egg-info/not-zip-safe
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      229 2022-11-10 10:02:30.000000 torch_snippets-0.499.9/torch_snippets.egg-info/requires.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2022-11-10 10:02:30.000000 torch_snippets-0.499.9/torch_snippets.egg-info/top_level.txt
```

### Comparing `torch_snippets-0.499.8/LICENSE` & `torch_snippets-0.499.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/LICENSE.txt` & `torch_snippets-0.499.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/PKG-INFO` & `torch_snippets-0.499.9/torch_snippets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: torch_snippets
-Version: 0.499.8
+Name: torch-snippets
+Version: 0.499.9
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
 Platform: UNKNOWN
```

### Comparing `torch_snippets-0.499.8/README.md` & `torch_snippets-0.499.9/README.md`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/settings.ini` & `torch_snippets-0.499.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 user = sizhky
 description = One line functions for common tasks
 keywords = snippets, torch
 author = Yeshwanth Reddy
 author_email = 1992chinna@gmail.com
 copyright = sizhky
 branch = master
-version = 0.499.8
+version = 0.499.9
 min_python = 3.7
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `torch_snippets-0.499.8/setup.py` & `torch_snippets-0.499.9/setup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/_modidx.py` & `torch_snippets-0.499.9/torch_snippets/_modidx.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/_nbdev.py` & `torch_snippets-0.499.9/torch_snippets/_nbdev.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/adapters.py` & `torch_snippets-0.499.9/torch_snippets/adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         axis=1,
         inplace=True,
     )
     records = df.to_dict(orient="records")
     return records
 
 
-def csvs_2_cvat(images_folder, csvs_folder, xml_output_file, label_column='readable_label', default_label="Background", items=None):
+def csvs_2_cvat(images_folder, csvs_folder, xml_output_file, label_column='readable_label', default_label="Background", items=None, extn='png'):
     if csvs_folder is None:
         images_folder = P(images_folder)
     else:
         images_folder, csvs_folder = [P(_) for _ in [images_folder, csvs_folder]]
 
     data = AttrDict({"annotations": {"image": []}})
     if csvs_folder is None:
@@ -88,24 +88,23 @@
     if items is None:
         items = common(stems(images_folder), stems(csvs_folder))
 
     items = sorted(items)
 
     for ix, item in enumerate(track(items)):
         _ia = _image_annotation = AttrDict({})
-        image = images_folder / f"{item}.png"
+        image = images_folder / f"{item}.{extn}"
         _ia["@height"], _ia["@width"] = read(image).shape[:2]
         _ia["@id"] = str(ix)
-        _ia["@name"] = f"{item}.png"
+        _ia["@name"] = f"{item}.{extn}"
         if csvs_folder is not None:
             df = pd.read_csv(f"{csvs_folder}/{item}.csv")
             _ia["box"] = _process(df, label_column=label_column, default_label=default_label)
         else:
             _ia["box"] = []
-        print(_ia)
         data.annotations.image.append(_ia)
     write_xml(data, xml_output_file)
 
 
 def _get_attribute_columns(column):
     def _get_columns_from_row(item):
         if item != item:
```

### Comparing `torch_snippets-0.499.8/torch_snippets/bb_utils.py` & `torch_snippets-0.499.9/torch_snippets/bb_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/bokeh_loader.py` & `torch_snippets-0.499.9/torch_snippets/bokeh_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/charts.py` & `torch_snippets-0.499.9/torch_snippets/charts.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/imgaug_loader.py` & `torch_snippets-0.499.9/torch_snippets/imgaug_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/inspector.py` & `torch_snippets-0.499.9/torch_snippets/inspector.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/interactive_show.py` & `torch_snippets-0.499.9/torch_snippets/interactive_show.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/ipython.py` & `torch_snippets-0.499.9/torch_snippets/ipython.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/load_defaults.py` & `torch_snippets-0.499.9/torch_snippets/load_defaults.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/loader.py` & `torch_snippets-0.499.9/torch_snippets/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -277,15 +277,15 @@
     bbs=None,
     confs=None,
     texts=None,
     bb_colors=None,
     cmap="gray",
     grid=False,
     save_path=None,
-    text_sz=10,
+    text_sz=None,
     df=None,
     pts=None,
     conns=None,
     **kwargs,
 ):
     "show an image"
 
@@ -367,14 +367,15 @@
             if bb_colors == "random"
             else bb_colors
         )
         bb_colors = [bb_colors] * len(bbs) if isinstance(bb_colors, str) else bb_colors
         bb_colors = [None] * len(bbs) if bb_colors is None else bb_colors
         img = C(img) if len(img.shape) == 2 else img
         [rect(img, tuple(bb), c=bb_colors[ix], th=th) for ix, bb in enumerate(bbs)]
+    text_sz = text_sz if text_sz else (max(sz) * 3 // 5)
     if texts is not None:
         if hasattr(texts, "shape"):
             if isinstance(texts, torch.Tensor):
                 texts = texts.cpu().detach().numpy()
             texts = texts.tolist()
         if texts == "ixs":
             texts = [i for i in range(len(bbs))]
@@ -391,32 +392,26 @@
         ax.set_title(title, fontdict=kwargs.pop("fontdict", None))
     if pts:
         pts = np.array(pts)
         if pts.max() < 1.1:
             pts = (pts * np.array([[w, h]])).astype(np.uint16).tolist()
         ax.scatter(*zip(*pts), c=kwargs.pop("pts_color", "red"))
     if conns is not None:
-        conn_colors = kwargs.pop("conn_colors", ["cyan"] * len(conns))
-        for ix in range(len(conns)):
-            if len(conns[ix]) == 2:
-                start_ix, end_ix = conns[ix]
-                meta = 1
-            else:
-                start_ix, end_ix, meta = conns[ix]
+        for start_ix, end_ix, meta in conns:
             _x, _y = bbs[start_ix].xc, bbs[start_ix].yc
             _X, _Y = bbs[end_ix].xc, bbs[end_ix].yc
             _dx, _dy = _X - _x, _Y - _y
             _xc, _yc = (_X + _x) // 2, (_Y + _y) // 2
             plt.arrow(
                 _jitter(_x),
                 _jitter(_y),
                 _jitter(_dx),
                 _jitter(_dy),
                 length_includes_head=True,
-                color=conn_colors[ix],
+                color="cyan",
                 head_width=4,
                 head_length=4,
                 width=meta * 2,
             )
             if kwargs.get("conn_text", True):
                 puttext(ax, f"{meta:.2f}", (_xc, _yc), size=text_sz)
         kwargs.pop("conn_text")
@@ -662,14 +657,54 @@
     cv2.imwrite(fpath, image)
 
 
 def lzip(*x):
     return list(zip(*x))
 
 
+# def to_absolute(input, shape):
+#     if isinstance(shape, np.ndarray) and shape.ndim >= 2:
+#         shape = shape.shape[:2]
+#     h, w = shape
+#     if isinstance(input, BB):
+#         return input.absolute((h, w))
+#     elif isinstance(input, pd.DataFrame):
+
+#         def _round(x):
+#             return np.round(x.values.astype(np.double)).astype(np.uint16)
+
+#         df = input.copy()
+#         df["x"] = _round(df.x * w)
+#         df["X"] = _round(df.X * w)
+#         df["y"] = _round(df.y * h)
+#         df["Y"] = _round(df.Y * h)
+#         return df
+#     elif isinstance(input, list):
+#         bbs = bbfy(input)
+#         return [bb.absolute((h, w)) for bb in bbs]
+
+
+# def to_relative(input, shape):
+#     if isinstance(shape, np.ndarray) and shape.ndim >= 2:
+#         shape = shape.shape[:2]
+#     h, w = shape
+#     if isinstance(input, BB):
+#         return input.relative((h, w))
+#     elif isinstance(input, pd.DataFrame):
+#         df = input.copy()
+#         df["x"] = df.x / w
+#         df["X"] = df.X / w
+#         df["y"] = df.y / h
+#         df["Y"] = df.Y / h
+#         return df
+#     elif isinstance(input, list):
+#         bbs = bbfy(input)
+#         return [bb.relative((h, w)) for bb in bbs]
+
+
 from fastcore.basics import patch_to
 
 
 @patch_to(L)
 def first(self):
     if len(self) > 0:
         return self[0]
```

### Comparing `torch_snippets-0.499.8/torch_snippets/logger.py` & `torch_snippets-0.499.9/torch_snippets/logger.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/markup.py` & `torch_snippets-0.499.9/torch_snippets/markup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/misc.py` & `torch_snippets-0.499.9/torch_snippets/misc.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/paths.py` & `torch_snippets-0.499.9/torch_snippets/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 P.__repr__ = lambda self: f"» {self}"
 
 
 @patch_to(P)
 def rmtree(self, prompt="Really remove `{self}` and its contents? [y/n] ", force=False):
     if force:
         shutil.rmtree(self)
-    elif prompt and input(prompt.format(self)).lower() == "y":
+    elif prompt and input(prompt.format(self=self)).lower() == "y":
         shutil.rmtree(self)
     else:
         raise OSError(f"{self} exists and is not empty")
 
 
 
 @patch_to(P)
@@ -93,17 +93,17 @@
 
 @patch_to(P)
 def cp(self, to):
     return P(shutil.copy(self, to))
 
 
 @patch_to(P)
-def rm(self, confirm_prompt=False, silent=True, missing_ok=True):
+def rm(self, confirm_prompt="Are you sure you want to delete `{self}`? [y/N]", silent=True, missing_ok=True):
     confirm = (
-        input(f"Are you sure you want to delete `{self}`? [y/N]")
+        input(confirm_prompt.format(self=self))
         if confirm_prompt
         else "y"
     )
     if confirm.lower() == "y":
         if missing_ok:
             try:
                 os.remove(self)
```

### Comparing `torch_snippets-0.499.8/torch_snippets/pdf_loader.py` & `torch_snippets-0.499.9/torch_snippets/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/registry.py` & `torch_snippets-0.499.9/torch_snippets/registry.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/sklegos.py` & `torch_snippets-0.499.9/torch_snippets/sklegos.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/text_utils.py` & `torch_snippets-0.499.9/torch_snippets/text_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/thinc_parser/parser.py` & `torch_snippets-0.499.9/torch_snippets/thinc_parser/parser.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets/torch_loader.py` & `torch_snippets-0.499.9/torch_snippets/torch_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 try:
     import wandb
 except ImportError:
     pass
 
 try:
-    import mlflow
+    from mlflow_extend import mlflow
 except ImportError:
     mlflow = None
 
 
 class Reshape(nn.Module):
     def __init__(self, *shape):
         super().__init__()
```

### Comparing `torch_snippets-0.499.8/torch_snippets/trainer/capsule.py` & `torch_snippets-0.499.9/torch_snippets/trainer/capsule.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.499.8/torch_snippets.egg-info/PKG-INFO` & `torch_snippets-0.499.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: torch-snippets
-Version: 0.499.8
+Name: torch_snippets
+Version: 0.499.9
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
 Platform: UNKNOWN
```

### Comparing `torch_snippets-0.499.8/torch_snippets.egg-info/SOURCES.txt` & `torch_snippets-0.499.9/torch_snippets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

