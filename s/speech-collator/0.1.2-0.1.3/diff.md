# Comparing `tmp/speech_collator-0.1.2.tar.gz` & `tmp/speech_collator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech_collator-0.1.2.tar", last modified: Sun May 14 16:39:26 2023, max compression
+gzip compressed data, was "speech_collator-0.1.3.tar", last modified: Sun May 14 16:44:23 2023, max compression
```

## Comparing `speech_collator-0.1.2.tar` & `speech_collator-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      111 2023-05-14 11:12:31.266135 speech_collator-0.1.2/README.md
--rw-r--r--   0        0        0      534 2023-05-14 16:39:26.016014 speech_collator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    15103 2023-05-14 16:31:08.431767 speech_collator-0.1.2/speech_collator/__init__.py
--rw-r--r--   0        0        0  5714361 2021-12-07 12:00:26.000000 speech_collator-0.1.2/speech_collator/data/dvector-step250000.pt
--rw-r--r--   0        0        0    62866 2021-12-07 12:00:44.000000 speech_collator-0.1.2/speech_collator/data/wav2mel.pt
--rw-r--r--   0        0        0     3969 2023-05-14 12:04:42.857714 speech_collator-0.1.2/speech_collator/measures/__init__.py
--rw-r--r--   0        0        0     2411 2023-05-14 11:28:31.387233 speech_collator-0.1.2/speech_collator/measures/snr.py
--rw-r--r--   0        0        0     2376 2023-05-14 11:28:43.968453 speech_collator-0.1.2/speech_collator/measures/srmr.py
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 speech_collator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      111 2023-05-14 11:12:31.266135 speech_collator-0.1.3/README.md
+-rw-r--r--   0        0        0      534 2023-05-14 16:44:23.928900 speech_collator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    15103 2023-05-14 16:31:08.431767 speech_collator-0.1.3/speech_collator/__init__.py
+-rw-r--r--   0        0        0  5714361 2021-12-07 12:00:26.000000 speech_collator-0.1.3/speech_collator/data/dvector-step250000.pt
+-rw-r--r--   0        0        0    62866 2021-12-07 12:00:44.000000 speech_collator-0.1.3/speech_collator/data/wav2mel.pt
+-rw-r--r--   0        0        0     3969 2023-05-14 12:04:42.857714 speech_collator-0.1.3/speech_collator/measures/__init__.py
+-rw-r--r--   0        0        0     2411 2023-05-14 11:28:31.387233 speech_collator-0.1.3/speech_collator/measures/snr.py
+-rw-r--r--   0        0        0     2376 2023-05-14 11:28:43.968453 speech_collator-0.1.3/speech_collator/measures/srmr.py
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 speech_collator-0.1.3/PKG-INFO
```

### Comparing `speech_collator-0.1.2/pyproject.toml` & `speech_collator-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "speech-collator"
-version = "0.1.2"
+version = "0.1.3"
 description = "A collator for speech datasets with different batching strategies and attribute extraction."
 authors = [
     { name = "Christoph Minixhofer", email = "christoph.minixhofer@gmail.com" },
 ]
 dependencies = [
     "numpy>=1.24.3",
     "pyworld>=0.3.3",
```

### Comparing `speech_collator-0.1.2/speech_collator/__init__.py` & `speech_collator-0.1.3/speech_collator/__init__.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.2/speech_collator/data/dvector-step250000.pt` & `speech_collator-0.1.3/speech_collator/data/dvector-step250000.pt`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.2/speech_collator/data/wav2mel.pt` & `speech_collator-0.1.3/speech_collator/data/wav2mel.pt`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.2/speech_collator/measures/__init__.py` & `speech_collator-0.1.3/speech_collator/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.2/speech_collator/measures/snr.py` & `speech_collator-0.1.3/speech_collator/measures/snr.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.2/speech_collator/measures/srmr.py` & `speech_collator-0.1.3/speech_collator/measures/srmr.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.2/PKG-INFO` & `speech_collator-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speech-collator
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collator for speech datasets with different batching strategies and attribute extraction.
 Author-Email: Christoph Minixhofer <christoph.minixhofer@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: numpy>=1.24.3
 Requires-Dist: pyworld>=0.3.3
 Requires-Dist: librosa>=0.10.0.post2
```

