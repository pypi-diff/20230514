# Comparing `tmp/e-qsl-0.1.8.tar.gz` & `tmp/e-qsl-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-qsl-0.1.8.tar", last modified: Sun Apr 16 14:08:35 2023, max compression
+gzip compressed data, was "e-qsl-0.1.9.tar", last modified: Wed May  3 05:06:55 2023, max compression
```

## Comparing `e-qsl-0.1.8.tar` & `e-qsl-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-04-16 14:08:35.483422 e-qsl-0.1.8/
--rw-r--r--   0 fred       (501) staff       (20)     1879 2023-03-29 02:24:01.000000 e-qsl-0.1.8/.gitignore
--rw-r--r--   0 fred       (501) staff       (20)      890 2023-04-16 14:08:35.482705 e-qsl-0.1.8/PKG-INFO
--rw-r--r--   0 fred       (501) staff       (20)      239 2023-03-29 15:20:51.000000 e-qsl-0.1.8/README.md
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-04-16 14:08:35.468450 e-qsl-0.1.8/card/
--rw-r--r--   0 fred       (501) staff       (20)   281258 2023-03-08 22:15:25.000000 e-qsl-0.1.8/card/default.jpg
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-04-16 14:08:35.473305 e-qsl-0.1.8/e_qsl.egg-info/
--rw-r--r--   0 fred       (501) staff       (20)      890 2023-04-16 14:08:34.000000 e-qsl-0.1.8/e_qsl.egg-info/PKG-INFO
--rw-r--r--   0 fred       (501) staff       (20)      366 2023-04-16 14:08:35.000000 e-qsl-0.1.8/e_qsl.egg-info/SOURCES.txt
--rw-r--r--   0 fred       (501) staff       (20)        1 2023-04-16 14:08:34.000000 e-qsl-0.1.8/e_qsl.egg-info/dependency_links.txt
--rw-r--r--   0 fred       (501) staff       (20)       35 2023-04-16 14:08:34.000000 e-qsl-0.1.8/e_qsl.egg-info/entry_points.txt
--rw-r--r--   0 fred       (501) staff       (20)       29 2023-04-16 14:08:34.000000 e-qsl-0.1.8/e_qsl.egg-info/requires.txt
--rw-r--r--   0 fred       (501) staff       (20)        5 2023-04-16 14:08:34.000000 e-qsl-0.1.8/e_qsl.egg-info/top_level.txt
--rwxr-xr-x   0 fred       (501) staff       (20)     8965 2023-04-16 14:06:57.000000 e-qsl-0.1.8/eqsl.py
--rw-r--r--   0 fred       (501) staff       (20)     1075 2023-04-16 14:00:01.000000 e-qsl-0.1.8/eqsl.yaml.sample
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-04-16 14:08:35.478460 e-qsl-0.1.8/fonts/
--rw-r--r--   0 fred       (501) staff       (20)    78296 2023-03-08 21:55:36.000000 e-qsl-0.1.8/fonts/DroidSansMono.ttf
--rw-r--r--   0 fred       (501) staff       (20)   183188 2023-03-10 00:22:58.000000 e-qsl-0.1.8/fonts/Ubuntu Mono derivative Powerline Bold.ttf
--rwxr-xr-x   0 fred       (501) staff       (20)    54508 2023-03-08 21:55:47.000000 e-qsl-0.1.8/fonts/VeraMono-Italic.ttf
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-04-16 14:08:35.480113 e-qsl-0.1.8/misc/
--rw-r--r--   0 fred       (501) staff       (20)   191436 2023-03-10 15:39:28.000000 e-qsl-0.1.8/misc/qsl-example.jpg
--rw-r--r--   0 fred       (501) staff       (20)       38 2023-04-16 14:08:35.483581 e-qsl-0.1.8/setup.cfg
--rwxr-xr-x   0 fred       (501) staff       (20)     1336 2023-04-16 14:07:50.000000 e-qsl-0.1.8/setup.py
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-05-03 05:06:55.540408 e-qsl-0.1.9/
+-rw-r--r--   0 fred       (501) staff       (20)     1879 2023-03-29 02:24:01.000000 e-qsl-0.1.9/.gitignore
+-rw-r--r--   0 fred       (501) staff       (20)      890 2023-05-03 05:06:55.540110 e-qsl-0.1.9/PKG-INFO
+-rw-r--r--   0 fred       (501) staff       (20)      239 2023-03-29 15:20:51.000000 e-qsl-0.1.9/README.md
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-05-03 05:06:55.531206 e-qsl-0.1.9/card/
+-rw-r--r--   0 fred       (501) staff       (20)   281258 2023-03-08 22:15:25.000000 e-qsl-0.1.9/card/default.jpg
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-05-03 05:06:55.534329 e-qsl-0.1.9/e_qsl.egg-info/
+-rw-r--r--   0 fred       (501) staff       (20)      890 2023-05-03 05:06:54.000000 e-qsl-0.1.9/e_qsl.egg-info/PKG-INFO
+-rw-r--r--   0 fred       (501) staff       (20)      366 2023-05-03 05:06:55.000000 e-qsl-0.1.9/e_qsl.egg-info/SOURCES.txt
+-rw-r--r--   0 fred       (501) staff       (20)        1 2023-05-03 05:06:54.000000 e-qsl-0.1.9/e_qsl.egg-info/dependency_links.txt
+-rw-r--r--   0 fred       (501) staff       (20)       35 2023-05-03 05:06:54.000000 e-qsl-0.1.9/e_qsl.egg-info/entry_points.txt
+-rw-r--r--   0 fred       (501) staff       (20)       29 2023-05-03 05:06:54.000000 e-qsl-0.1.9/e_qsl.egg-info/requires.txt
+-rw-r--r--   0 fred       (501) staff       (20)        5 2023-05-03 05:06:54.000000 e-qsl-0.1.9/e_qsl.egg-info/top_level.txt
+-rwxr-xr-x   0 fred       (501) staff       (20)     9059 2023-05-03 05:05:40.000000 e-qsl-0.1.9/eqsl.py
+-rw-r--r--   0 fred       (501) staff       (20)     1075 2023-04-16 14:00:01.000000 e-qsl-0.1.9/eqsl.yaml.sample
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-05-03 05:06:55.537540 e-qsl-0.1.9/fonts/
+-rw-r--r--   0 fred       (501) staff       (20)    78296 2023-03-08 21:55:36.000000 e-qsl-0.1.9/fonts/DroidSansMono.ttf
+-rw-r--r--   0 fred       (501) staff       (20)   183188 2023-03-10 00:22:58.000000 e-qsl-0.1.9/fonts/Ubuntu Mono derivative Powerline Bold.ttf
+-rwxr-xr-x   0 fred       (501) staff       (20)    54508 2023-03-08 21:55:47.000000 e-qsl-0.1.9/fonts/VeraMono-Italic.ttf
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-05-03 05:06:55.538550 e-qsl-0.1.9/misc/
+-rw-r--r--   0 fred       (501) staff       (20)   191436 2023-03-10 15:39:28.000000 e-qsl-0.1.9/misc/qsl-example.jpg
+-rw-r--r--   0 fred       (501) staff       (20)       38 2023-05-03 05:06:55.540483 e-qsl-0.1.9/setup.cfg
+-rwxr-xr-x   0 fred       (501) staff       (20)     1336 2023-05-03 05:06:27.000000 e-qsl-0.1.9/setup.py
```

### Comparing `e-qsl-0.1.8/.gitignore` & `e-qsl-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `e-qsl-0.1.8/PKG-INFO` & `e-qsl-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-qsl
-Version: 0.1.8
+Version: 0.1.9
 Summary: Send contacts confirmation cards (QSL Cards)
 Home-page: https://github.com/0x9900/QSL/
 Author: Fred C. (W6BSD)
 Author-email: w6bsd@bsdworld.org
 License: BSD-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Telecommunications Industry
```

### Comparing `e-qsl-0.1.8/card/default.jpg` & `e-qsl-0.1.9/card/default.jpg`

 * *Files identical despite different names*

### Comparing `e-qsl-0.1.8/e_qsl.egg-info/PKG-INFO` & `e-qsl-0.1.9/e_qsl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-qsl
-Version: 0.1.8
+Version: 0.1.9
 Summary: Send contacts confirmation cards (QSL Cards)
 Home-page: https://github.com/0x9900/QSL/
 Author: Fred C. (W6BSD)
 Author-email: w6bsd@bsdworld.org
 License: BSD-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Telecommunications Industry
```

### Comparing `e-qsl-0.1.8/eqsl.py` & `e-qsl-0.1.9/eqsl.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,21 +66,24 @@
   msg = MIMEMultipart()
   msg['From'] = config.smtp_from
   msg['To'] = qso.email
   msg['Date'] = formatdate(localtime=True)
   msg['Subject'] = f"Digital QSL from {qso.OPERATOR} to {qso.CALL}"
 
   data = {}
+  data['call'] = qso.CALL
   data['fname'] = qso.fname
   data['qso_date'] = datetime.fromtimestamp(qso.timestamp).strftime("%A %B %d, %Y at %X UTC")
   data['freq_rx'] = qso.FREQ_RX
   data['mode'] = qso.MODE
   data['band'] = qso.BAND_RX
   data['rst_sent'] = qso.RST_SENT
   data['rst_rcvd'] = qso.RST_RCVD
+  data['rig'] = qso.MY_RIG
+  data['gridsquare'] = qso.MY_GRIDSQUARE
 
   msg.attach(MIMEText(template(data)))
 
   with open(image, "rb") as fd:
     part = MIMEApplication(fd.read(), Name=os.path.basename(image))
     part['Content-Disposition'] = 'attachment; filename="%s"' % os.path.basename(image)
     msg.attach(part)
```

### Comparing `e-qsl-0.1.8/eqsl.yaml.sample` & `e-qsl-0.1.9/eqsl.yaml.sample`

 * *Files identical despite different names*

### Comparing `e-qsl-0.1.8/fonts/DroidSansMono.ttf` & `e-qsl-0.1.9/fonts/DroidSansMono.ttf`

 * *Files identical despite different names*

### Comparing `e-qsl-0.1.8/fonts/Ubuntu Mono derivative Powerline Bold.ttf` & `e-qsl-0.1.9/fonts/Ubuntu Mono derivative Powerline Bold.ttf`

 * *Files identical despite different names*

### Comparing `e-qsl-0.1.8/fonts/VeraMono-Italic.ttf` & `e-qsl-0.1.9/fonts/VeraMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `e-qsl-0.1.8/misc/qsl-example.jpg` & `e-qsl-0.1.9/misc/qsl-example.jpg`

 * *Files identical despite different names*

### Comparing `e-qsl-0.1.8/setup.py` & `e-qsl-0.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 
 import sys
 
 from setuptools import setup
 
 __author__ = "Fred C. (W6BSD)"
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 __license__ = 'BSD-3'
 
 py_version = sys.version_info[:2]
 if py_version < (3, 8):
   raise RuntimeError('eqsl requires Python 3.8 or later')
 
 def readme():
```

