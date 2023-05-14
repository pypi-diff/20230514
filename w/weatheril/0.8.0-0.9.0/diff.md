# Comparing `tmp/weatheril-0.8.0.tar.gz` & `tmp/weatheril-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weatheril-0.8.0.tar", last modified: Mon Jan 30 11:18:47 2023, max compression
+gzip compressed data, was "weatheril-0.9.0.tar", last modified: Mon Jan 30 21:34:48 2023, max compression
```

## Comparing `weatheril-0.8.0.tar` & `weatheril-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 11:18:47.782070 weatheril-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-30 11:18:33.000000 weatheril-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-01-30 11:18:47.782070 weatheril-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-01-30 11:18:33.000000 weatheril-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 11:18:47.782070 weatheril-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-01-30 11:18:33.000000 weatheril-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 11:18:47.778070 weatheril-0.8.0/weatheril/
--rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-01-30 11:18:33.000000 weatheril-0.8.0/weatheril/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-30 11:18:33.000000 weatheril-0.8.0/weatheril/forcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-01-30 11:18:33.000000 weatheril-0.8.0/weatheril/radarsatellite.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-01-30 11:18:33.000000 weatheril-0.8.0/weatheril/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 11:18:47.782070 weatheril-0.8.0/weatheril.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-01-30 11:18:47.000000 weatheril-0.8.0/weatheril.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-01-30 11:18:47.000000 weatheril-0.8.0/weatheril.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 11:18:47.000000 weatheril-0.8.0/weatheril.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 11:18:47.000000 weatheril-0.8.0/weatheril.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-30 11:18:47.000000 weatheril-0.8.0/weatheril.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:34:48.356241 weatheril-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-30 21:34:36.000000 weatheril-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-01-30 21:34:48.356241 weatheril-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-01-30 21:34:36.000000 weatheril-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 21:34:48.356241 weatheril-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-01-30 21:34:36.000000 weatheril-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:34:48.352240 weatheril-0.9.0/weatheril/
+-rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-01-30 21:34:36.000000 weatheril-0.9.0/weatheril/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-30 21:34:36.000000 weatheril-0.9.0/weatheril/forcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-01-30 21:34:36.000000 weatheril-0.9.0/weatheril/radarsatellite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-01-30 21:34:36.000000 weatheril-0.9.0/weatheril/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:34:48.356241 weatheril-0.9.0/weatheril.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-01-30 21:34:48.000000 weatheril-0.9.0/weatheril.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-01-30 21:34:48.000000 weatheril-0.9.0/weatheril.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:34:48.000000 weatheril-0.9.0/weatheril.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 21:34:48.000000 weatheril-0.9.0/weatheril.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-30 21:34:48.000000 weatheril-0.9.0/weatheril.egg-info/top_level.txt
```

### Comparing `weatheril-0.8.0/LICENSE` & `weatheril-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weatheril-0.8.0/PKG-INFO` & `weatheril-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weatheril
-Version: 0.8.0
+Version: 0.9.0
 Summary: Israel Meteorological Service unofficial python api wrapper
 Home-page: https://github.com/t0mer/py-weatheril
 Download-URL: https://pypi.org/project/weatheril/
 Author: Tomer Klein
 Author-email: tomer.klein@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/t0mer/py-weatheril
```

### Comparing `weatheril-0.8.0/README.md` & `weatheril-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `weatheril-0.8.0/setup.py` & `weatheril-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open("README.md", "r", encoding="UTF-8") as f:
      readme = f.read()
 
 setup_args = dict(
     name='weatheril',
-    version='0.8.0',
+    version='0.9.0',
     description='Israel Meteorological Service unofficial python api wrapper',
     long_description_content_type="text/markdown",
     long_description=readme,
     license='MIT',
     packages=find_packages(),
     author='Tomer Klein',
     author_email='tomer.klein@gmail.com',
```

### Comparing `weatheril-0.8.0/weatheril/__init__.py` & `weatheril-0.9.0/weatheril/__init__.py`

 * *Files identical despite different names*

### Comparing `weatheril-0.8.0/weatheril/forcast.py` & `weatheril-0.9.0/weatheril/forcast.py`

 * *Files identical despite different names*

### Comparing `weatheril-0.8.0/weatheril/radarsatellite.py` & `weatheril-0.9.0/weatheril/radarsatellite.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,21 +41,20 @@
             if os.path.exists(path):
                animated_image = path + "/" + animated_file
             else:
                 animated_image = os.path.realpath(os.path.dirname(__file__)) + "/" + animated_file
 
             for idx, item in enumerate(images):
                 file = requests.get(images[idx])
-                open(tempfile.gettempdir() + os.path.basename(urlparse(images[idx]).path), "wb").write(file.content)
-                images[idx] = tempfile.gettempdir() + os.path.basename(urlparse(images[idx]).path)
+                open(tempfile.gettempdir() + "/" + os.path.basename(urlparse(images[idx]).path), "wb").write(file.content)
+                images[idx] = tempfile.gettempdir() + "/" +  os.path.basename(urlparse(images[idx]).path)
             
             frames = [Image.open(image) for image in images]
             frame_one = frames[0]
-            frame_one.save(animated_image, format="GIF", append_images=frames,save_all=True, loop=0)
+            frame_one.save(animated_image, format="GIF", append_images=frames,save_all=True, duration=4, loop=0)
 
             for image in images:
-                print(image)
                 os.remove(image)
             return animated_image
         except Exception as e:
             logger.error("Error creating animation. " + str(e))
             return None
```

### Comparing `weatheril-0.8.0/weatheril.egg-info/PKG-INFO` & `weatheril-0.9.0/weatheril.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weatheril
-Version: 0.8.0
+Version: 0.9.0
 Summary: Israel Meteorological Service unofficial python api wrapper
 Home-page: https://github.com/t0mer/py-weatheril
 Download-URL: https://pypi.org/project/weatheril/
 Author: Tomer Klein
 Author-email: tomer.klein@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/t0mer/py-weatheril
```

