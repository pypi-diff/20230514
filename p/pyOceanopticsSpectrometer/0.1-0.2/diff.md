# Comparing `tmp/pyOceanopticsSpectrometer-0.1.tar.gz` & `tmp/pyOceanopticsSpectrometer-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyOceanopticsSpectrometer-0.1.tar", last modified: Sat May 13 19:23:02 2023, max compression
+gzip compressed data, was "pyOceanopticsSpectrometer-0.2.tar", last modified: Sat May 13 22:38:13 2023, max compression
```

## Comparing `pyOceanopticsSpectrometer-0.1.tar` & `pyOceanopticsSpectrometer-0.2.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 19:23:02.601219 pyOceanopticsSpectrometer-0.1/
--rw-rw-rw-   0        0        0       70 2022-05-30 21:30:49.000000 pyOceanopticsSpectrometer-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      349 2023-05-13 19:23:02.601219 pyOceanopticsSpectrometer-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-01 22:10:22.000000 pyOceanopticsSpectrometer-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 19:23:02.531284 pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer/
--rw-rw-rw-   0        0        0       37 2022-08-09 18:25:22.000000 pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer/__init__.py
--rw-rw-rw-   0        0        0     6079 2023-05-01 23:22:14.000000 pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer/driver.py
--rw-rw-rw-   0        0        0    45886 2023-05-07 22:43:37.000000 pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer/main.py
--rw-rw-rw-   0        0        0     1348 2023-05-01 22:28:35.000000 pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer/plots.py
-drwxrwxrwx   0        0        0        0 2023-05-13 19:23:02.601219 pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer.egg-info/
--rw-rw-rw-   0        0        0      349 2023-05-13 19:23:02.000000 pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-05-13 19:23:02.000000 pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 19:23:02.000000 pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-05-13 19:23:02.000000 pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-13 19:23:02.000000 pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       82 2023-05-13 19:23:02.000000 pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-13 19:23:02.000000 pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 19:23:02.601219 pyOceanopticsSpectrometer-0.1/setup.cfg
--rw-rw-rw-   0        0        0      995 2022-08-08 23:00:52.000000 pyOceanopticsSpectrometer-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:38:13.748230 pyOceanopticsSpectrometer-0.2/
+-rw-rw-rw-   0        0        0       86 2023-05-13 22:36:19.000000 pyOceanopticsSpectrometer-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      349 2023-05-13 22:38:13.746235 pyOceanopticsSpectrometer-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-01 22:10:22.000000 pyOceanopticsSpectrometer-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-13 22:38:13.703350 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/
+-rw-rw-rw-   0        0        0       37 2022-08-09 18:25:22.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-13 01:12:50.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/config.json
+-rw-rw-rw-   0        0        0     6079 2023-05-01 23:22:14.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/driver.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:38:13.743243 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/graphics/
+-rw-rw-rw-   0        0        0    19884 2022-08-10 15:20:12.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/graphics/ligthOFF.png
+-rw-rw-rw-   0        0        0    19456 2022-08-10 15:16:13.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/graphics/ligthON.png
+-rw-rw-rw-   0        0        0     7799 2021-08-31 16:42:47.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/graphics/pause.png
+-rw-rw-rw-   0        0        0     9320 2021-08-31 16:41:38.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/graphics/play.png
+-rw-rw-rw-   0        0        0     3439 2021-08-29 03:28:31.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/graphics/refresh.png
+-rw-rw-rw-   0        0        0     7522 2021-08-31 16:43:00.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/graphics/stop.png
+-rw-rw-rw-   0        0        0    45886 2023-05-07 22:43:37.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/main.py
+-rw-rw-rw-   0        0        0     1348 2023-05-01 22:28:35.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/plots.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:38:13.724293 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer.egg-info/
+-rw-rw-rw-   0        0        0      349 2023-05-13 22:38:13.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      830 2023-05-13 22:38:13.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-13 22:38:13.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-05-13 22:38:13.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-13 22:38:13.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       82 2023-05-13 22:38:13.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-13 22:38:13.000000 pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-13 22:38:13.748230 pyOceanopticsSpectrometer-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      995 2023-05-13 22:37:22.000000 pyOceanopticsSpectrometer-0.2/setup.py
```

### Comparing `pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer/driver.py` & `pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/driver.py`

 * *Files identical despite different names*

### Comparing `pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer/main.py` & `pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/main.py`

 * *Files identical despite different names*

### Comparing `pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer/plots.py` & `pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer/plots.py`

 * *Files identical despite different names*

### Comparing `pyOceanopticsSpectrometer-0.1/pyOceanopticsSpectrometer.egg-info/SOURCES.txt` & `pyOceanopticsSpectrometer-0.2/pyOceanopticsSpectrometer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 MANIFEST.in
 README.md
 setup.py
 pyOceanopticsSpectrometer/__init__.py
+pyOceanopticsSpectrometer/config.json
 pyOceanopticsSpectrometer/driver.py
 pyOceanopticsSpectrometer/main.py
 pyOceanopticsSpectrometer/plots.py
 pyOceanopticsSpectrometer.egg-info/PKG-INFO
 pyOceanopticsSpectrometer.egg-info/SOURCES.txt
 pyOceanopticsSpectrometer.egg-info/dependency_links.txt
 pyOceanopticsSpectrometer.egg-info/entry_points.txt
 pyOceanopticsSpectrometer.egg-info/not-zip-safe
 pyOceanopticsSpectrometer.egg-info/requires.txt
-pyOceanopticsSpectrometer.egg-info/top_level.txt
+pyOceanopticsSpectrometer.egg-info/top_level.txt
+pyOceanopticsSpectrometer/graphics/ligthOFF.png
+pyOceanopticsSpectrometer/graphics/ligthON.png
+pyOceanopticsSpectrometer/graphics/pause.png
+pyOceanopticsSpectrometer/graphics/play.png
+pyOceanopticsSpectrometer/graphics/refresh.png
+pyOceanopticsSpectrometer/graphics/stop.png
```

### Comparing `pyOceanopticsSpectrometer-0.1/setup.py` & `pyOceanopticsSpectrometer-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(path.join(this_directory, 'README.md'),encoding ='unicode_escape') as f:
     long_description = f.read()
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setuptools.setup(name='pyOceanopticsSpectrometer',
-      version='0.1',
+      version='0.2',
       description='A python library/GUI to access and control OceanOptics spectrometers',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/MicheleCotrufo/',
       author='Michele Cotrufo',
       author_email='michele.cotrufo@gmail.com',
       license='MIT',
```

