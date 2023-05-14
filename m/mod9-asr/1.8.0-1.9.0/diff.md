# Comparing `tmp/mod9-asr-1.8.0.tar.gz` & `tmp/mod9-asr-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mod9-asr-1.8.0.tar", last modified: Thu Feb 10 01:48:54 2022, max compression
+gzip compressed data, was "mod9-asr-1.9.0.tar", last modified: Thu Feb 10 08:07:36 2022, max compression
```

## Comparing `mod9-asr-1.8.0.tar` & `mod9-asr-1.9.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 01:48:54.048607 mod9-asr-1.8.0/
--rw-r--r--   0 arlo       (502) staff       (20)     1327 2021-07-24 07:20:57.000000 mod9-asr-1.8.0/LICENSE
--rw-r--r--   0 arlo       (502) staff       (20)     1377 2022-02-10 01:48:54.048313 mod9-asr-1.8.0/PKG-INFO
--rw-r--r--   0 arlo       (502) staff       (20)     1002 2022-02-03 06:09:50.000000 mod9-asr-1.8.0/README.md
-drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 01:48:54.039749 mod9-asr-1.8.0/mod9/
--rw-r--r--   0 arlo       (502) staff       (20)     1193 2021-07-24 07:20:57.000000 mod9-asr-1.8.0/mod9/__init__.py
-drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 01:48:54.041492 mod9-asr-1.8.0/mod9/asr/
--rw-r--r--   0 arlo       (502) staff       (20)     1213 2022-02-03 06:09:50.000000 mod9-asr-1.8.0/mod9/asr/__init__.py
--rw-r--r--   0 arlo       (502) staff       (20)     6319 2022-02-03 06:48:44.000000 mod9-asr-1.8.0/mod9/asr/common.py
--rw-r--r--   0 arlo       (502) staff       (20)     5338 2022-02-03 06:48:44.000000 mod9-asr-1.8.0/mod9/asr/speech.py
--rw-r--r--   0 arlo       (502) staff       (20)    30450 2022-02-03 06:48:44.000000 mod9-asr-1.8.0/mod9/asr/speech_mod9.py
-drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 01:48:54.042012 mod9-asr-1.8.0/mod9/es/
--rwxr-xr-x   0 arlo       (502) staff       (20)    12283 2022-02-03 06:09:50.000000 mod9-asr-1.8.0/mod9/es/client.py
-drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 01:48:54.043365 mod9-asr-1.8.0/mod9/reformat/
--rw-r--r--   0 arlo       (502) staff       (20)     6267 2022-02-10 01:46:22.000000 mod9-asr-1.8.0/mod9/reformat/config.py
--rw-r--r--   0 arlo       (502) staff       (20)    29637 2022-02-03 06:48:44.000000 mod9-asr-1.8.0/mod9/reformat/google.py
--rw-r--r--   0 arlo       (502) staff       (20)    30431 2022-02-03 06:48:44.000000 mod9-asr-1.8.0/mod9/reformat/utils.py
-drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 01:48:54.044031 mod9-asr-1.8.0/mod9/rest/
--rwxr-xr-x   0 arlo       (502) staff       (20)    18689 2022-02-03 06:48:44.000000 mod9-asr-1.8.0/mod9/rest/server.py
-drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 01:48:54.044719 mod9-asr-1.8.0/mod9/switchboard/
--rwxr-xr-x   0 arlo       (502) staff       (20)    39403 2022-02-10 01:46:22.000000 mod9-asr-1.8.0/mod9/switchboard/benchmark.py
-drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 01:48:54.045552 mod9-asr-1.8.0/mod9/websocket/
--rwxr-xr-x   0 arlo       (502) staff       (20)     7082 2022-02-03 06:09:50.000000 mod9-asr-1.8.0/mod9/websocket/client.py
--rwxr-xr-x   0 arlo       (502) staff       (20)    16735 2022-02-03 06:09:50.000000 mod9-asr-1.8.0/mod9/websocket/server.py
-drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 01:48:54.047409 mod9-asr-1.8.0/mod9_asr.egg-info/
--rw-r--r--   0 arlo       (502) staff       (20)     1377 2022-02-10 01:48:53.000000 mod9-asr-1.8.0/mod9_asr.egg-info/PKG-INFO
--rw-r--r--   0 arlo       (502) staff       (20)      539 2022-02-10 01:48:53.000000 mod9-asr-1.8.0/mod9_asr.egg-info/SOURCES.txt
--rw-r--r--   0 arlo       (502) staff       (20)        1 2022-02-10 01:48:53.000000 mod9-asr-1.8.0/mod9_asr.egg-info/dependency_links.txt
--rw-r--r--   0 arlo       (502) staff       (20)      288 2022-02-10 01:48:53.000000 mod9-asr-1.8.0/mod9_asr.egg-info/entry_points.txt
--rw-r--r--   0 arlo       (502) staff       (20)      227 2022-02-10 01:48:53.000000 mod9-asr-1.8.0/mod9_asr.egg-info/requires.txt
--rw-r--r--   0 arlo       (502) staff       (20)        5 2022-02-10 01:48:53.000000 mod9-asr-1.8.0/mod9_asr.egg-info/top_level.txt
--rw-r--r--   0 arlo       (502) staff       (20)       38 2022-02-10 01:48:54.048699 mod9-asr-1.8.0/setup.cfg
--rwxr-xr-x   0 arlo       (502) staff       (20)     1705 2022-02-03 06:09:50.000000 mod9-asr-1.8.0/setup.py
-drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 01:48:54.047620 mod9-asr-1.8.0/test/
--rw-r--r--   0 arlo       (502) staff       (20)     2523 2021-07-24 07:20:57.000000 mod9-asr-1.8.0/test/test_mod9_synchronous.py
+drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 08:07:36.893848 mod9-asr-1.9.0/
+-rw-r--r--   0 arlo       (502) staff       (20)     1327 2021-07-24 07:20:57.000000 mod9-asr-1.9.0/LICENSE
+-rw-r--r--   0 arlo       (502) staff       (20)     1377 2022-02-10 08:07:36.893587 mod9-asr-1.9.0/PKG-INFO
+-rw-r--r--   0 arlo       (502) staff       (20)     1002 2022-02-03 06:09:50.000000 mod9-asr-1.9.0/README.md
+drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 08:07:36.883180 mod9-asr-1.9.0/mod9/
+-rw-r--r--   0 arlo       (502) staff       (20)     1193 2021-07-24 07:20:57.000000 mod9-asr-1.9.0/mod9/__init__.py
+drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 08:07:36.885439 mod9-asr-1.9.0/mod9/asr/
+-rw-r--r--   0 arlo       (502) staff       (20)     1213 2022-02-03 06:09:50.000000 mod9-asr-1.9.0/mod9/asr/__init__.py
+-rw-r--r--   0 arlo       (502) staff       (20)     6319 2022-02-03 06:48:44.000000 mod9-asr-1.9.0/mod9/asr/common.py
+-rw-r--r--   0 arlo       (502) staff       (20)     5338 2022-02-03 06:48:44.000000 mod9-asr-1.9.0/mod9/asr/speech.py
+-rw-r--r--   0 arlo       (502) staff       (20)    30450 2022-02-03 06:48:44.000000 mod9-asr-1.9.0/mod9/asr/speech_mod9.py
+drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 08:07:36.886215 mod9-asr-1.9.0/mod9/es/
+-rwxr-xr-x   0 arlo       (502) staff       (20)    12283 2022-02-03 06:09:50.000000 mod9-asr-1.9.0/mod9/es/client.py
+drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 08:07:36.887690 mod9-asr-1.9.0/mod9/reformat/
+-rw-r--r--   0 arlo       (502) staff       (20)     6370 2022-02-10 08:06:18.000000 mod9-asr-1.9.0/mod9/reformat/config.py
+-rw-r--r--   0 arlo       (502) staff       (20)    29637 2022-02-03 06:48:44.000000 mod9-asr-1.9.0/mod9/reformat/google.py
+-rw-r--r--   0 arlo       (502) staff       (20)    30431 2022-02-03 06:48:44.000000 mod9-asr-1.9.0/mod9/reformat/utils.py
+drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 08:07:36.888500 mod9-asr-1.9.0/mod9/rest/
+-rwxr-xr-x   0 arlo       (502) staff       (20)    18689 2022-02-03 06:48:44.000000 mod9-asr-1.9.0/mod9/rest/server.py
+drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 08:07:36.889303 mod9-asr-1.9.0/mod9/switchboard/
+-rwxr-xr-x   0 arlo       (502) staff       (20)    40444 2022-02-10 08:06:18.000000 mod9-asr-1.9.0/mod9/switchboard/benchmark.py
+drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 08:07:36.890235 mod9-asr-1.9.0/mod9/websocket/
+-rwxr-xr-x   0 arlo       (502) staff       (20)     7082 2022-02-03 06:09:50.000000 mod9-asr-1.9.0/mod9/websocket/client.py
+-rwxr-xr-x   0 arlo       (502) staff       (20)    16735 2022-02-03 06:09:50.000000 mod9-asr-1.9.0/mod9/websocket/server.py
+drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 08:07:36.892646 mod9-asr-1.9.0/mod9_asr.egg-info/
+-rw-r--r--   0 arlo       (502) staff       (20)     1377 2022-02-10 08:07:36.000000 mod9-asr-1.9.0/mod9_asr.egg-info/PKG-INFO
+-rw-r--r--   0 arlo       (502) staff       (20)      539 2022-02-10 08:07:36.000000 mod9-asr-1.9.0/mod9_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 arlo       (502) staff       (20)        1 2022-02-10 08:07:36.000000 mod9-asr-1.9.0/mod9_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 arlo       (502) staff       (20)      288 2022-02-10 08:07:36.000000 mod9-asr-1.9.0/mod9_asr.egg-info/entry_points.txt
+-rw-r--r--   0 arlo       (502) staff       (20)      227 2022-02-10 08:07:36.000000 mod9-asr-1.9.0/mod9_asr.egg-info/requires.txt
+-rw-r--r--   0 arlo       (502) staff       (20)        5 2022-02-10 08:07:36.000000 mod9-asr-1.9.0/mod9_asr.egg-info/top_level.txt
+-rw-r--r--   0 arlo       (502) staff       (20)       38 2022-02-10 08:07:36.893936 mod9-asr-1.9.0/setup.cfg
+-rwxr-xr-x   0 arlo       (502) staff       (20)     1705 2022-02-03 06:09:50.000000 mod9-asr-1.9.0/setup.py
+drwxr-xr-x   0 arlo       (502) staff       (20)        0 2022-02-10 08:07:36.892922 mod9-asr-1.9.0/test/
+-rw-r--r--   0 arlo       (502) staff       (20)     2523 2021-07-24 07:20:57.000000 mod9-asr-1.9.0/test/test_mod9_synchronous.py
```

### Comparing `mod9-asr-1.8.0/LICENSE` & `mod9-asr-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/PKG-INFO` & `mod9-asr-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mod9-asr
-Version: 1.8.0
+Version: 1.9.0
 Summary: Mod9 ASR Python SDK, REST API, and Websocket Interface: high-level interfaces to the Mod9 ASR Engine.
 Home-page: https://github.com/mod9-asr/python-sdk
 Author: Mod9 Technologies
 Author-email: support@mod9.com
 License: BSD 2-Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mod9-asr-1.8.0/README.md` & `mod9-asr-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/mod9/__init__.py` & `mod9-asr-1.9.0/mod9/__init__.py`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/mod9/asr/__init__.py` & `mod9-asr-1.9.0/mod9/asr/__init__.py`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/mod9/asr/common.py` & `mod9-asr-1.9.0/mod9/asr/common.py`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/mod9/asr/speech.py` & `mod9-asr-1.9.0/mod9/asr/speech.py`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/mod9/asr/speech_mod9.py` & `mod9-asr-1.9.0/mod9/asr/speech_mod9.py`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/mod9/es/client.py` & `mod9-asr-1.9.0/mod9/es/client.py`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/mod9/reformat/config.py` & `mod9-asr-1.9.0/mod9/reformat/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 Provides defaults used throughout mod9-asr.
 """
 
 import logging
 import os
 
 # Current wrappers version.  Note that this is not the same as the Engine version.
-WRAPPER_VERSION = '1.8.0'
+WRAPPER_VERSION = '1.9.0'
 
 # CHANGELOG:
+#   1.9.0 (09 Feb 2022):
+#   - Add Deepgram formatted result handling to Switchboard benchmark script.
 #   1.8.0 (08 Feb 2022):
-#   - Add Microsoft formatted result handling to switchboard benchmark script.
+#   - Add Microsoft formatted result handling to Switchboard benchmark script.
 #   1.7.0 (02 Feb 2022):
 #   - Allow multiple clients to connect to different Engine hosts and ports.
 #   - Support more audio encodings: 24- and 32-bit signed integers and 32-bit float.
 #   - Add IBM Watson format conversion to mod9-asr-switchboard-benchmark.
 #   1.6.0 (10 Jan 2022):
 #   - Add "asrModel" to results using speech_mod9 and REST API.
 #   - Minor fixes to mod9-asr-switchboard-benchmark and new features:
```

### Comparing `mod9-asr-1.8.0/mod9/reformat/google.py` & `mod9-asr-1.9.0/mod9/reformat/google.py`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/mod9/reformat/utils.py` & `mod9-asr-1.9.0/mod9/reformat/utils.py`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/mod9/rest/server.py` & `mod9-asr-1.9.0/mod9/rest/server.py`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/mod9/switchboard/benchmark.py` & `mod9-asr-1.9.0/mod9/switchboard/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import tempfile
 import urllib.request
 
 DESCRIPTION = """
 This specialized tool can be used to score the Switchboard benchmark by suitably formatting and
 scoring output from the Mod9 ASR Engine. It reads lines of JSON (i.e. JSONL format) from stdin and
 prints a report on stdout, saving files in a work directory.
-It can also read results formatted by Google, Amazon, Microsoft, or IBM.
+It can also read results formatted by Google, Amazon, Microsoft, Deepgram, or IBM.
 This uses the official NIST SCTK software, which is expected to be installed on the system, and also
 requires certain reference data files which might be downloaded. These dependencies are already
 installed in the mod9/asr Docker image for convenience.
 The Switchboard audio data is needed for meaningful demonstration and could be obtained from the
 Linguistic Data Consortium (https://catalog.ldc.upenn.edu/LDC2002S09).
 """
 
@@ -204,14 +204,28 @@
             # of producing a CTM, particularly if word-level timestamps are not available and are
             # then inferred as uniformly distributed over the utterance-level interval. This is
             # especially problematic for dual-channel telephony in which there are long stretches
             # of silence between speaker turns, during which words are mistimed.
             start_time = end_time
 
 
+def convert_deepgram_json_to_jsonl(json_filename, jsonl_filename):
+    """
+    Convert Deepgram formatted JSON to ASR Engine formatted JSON lines.
+    """
+    response = json.load(open(json_filename, 'r', encoding='utf-8'))
+    with open(jsonl_filename, 'w', encoding='utf-8') as jsonl_file:
+        result = response['results']['channels'][0]
+        reply = {'final': True}
+        reply['transcript'] = result['alternatives'][0]['transcript']
+        reply['words'] = [{'word': w['word'], 'interval': [w['start'], w['end']]}
+                          for w in result['alternatives'][0]['words']]
+        jsonl_file.write(json.dumps(reply) + '\n')
+
+
 def convert_ibm_json_to_jsonl(json_filename, jsonl_filename):
     """
     Convert IBM Watson formatted JSON to ASR Engine formatted JSON lines.
     """
     response = json.load(open(json_filename, 'r', encoding='utf-8'))
     with open(jsonl_filename, 'w', encoding='utf-8') as jsonl_file:
         for result in response['results'][0]['results']:  # awkwardly nested
@@ -862,15 +876,22 @@
     filename_id, channel_id = spkid.rsplit('_', 1)
 
     lines = []
     info("Read Engine replies or other vendors' JSON on stdin: ...", flush=True)
     for line in sys.stdin:
         lines.append(line)
 
-    if lines and lines[0] == '{\n' and ('"name"' in lines[1] or '"results"' in lines[1]):
+    if lines and lines[0].startswith('{"metadata"'):
+        info(f"Save JSON (Deepgram formatted) from stdin: {spkid}.json")
+        with open(spkid+'.json', 'w') as f:
+            for line in lines:
+                f.write(line)
+        info(f"Convert JSON to Engine formatted JSON lines: {spkid}.jsonl")
+        convert_deepgram_json_to_jsonl(spkid+'.json', spkid+'.jsonl')
+    elif lines and lines[0] == '{\n' and ('"name"' in lines[1] or '"results"' in lines[1]):
         info(f"Save JSON (Google STT formatted) from stdin: {spkid}.json")
         with open(spkid+'.json', 'w') as f:
             for line in lines:
                 f.write(line)
         info(f"Convert JSON to Engine formatted JSON lines: {spkid}.jsonl")
         convert_google_json_to_jsonl(spkid+'.json', spkid+'.jsonl')
     elif lines and lines[0] == '{\n' and '"created"' in lines[1]:
```

### Comparing `mod9-asr-1.8.0/mod9/websocket/client.py` & `mod9-asr-1.9.0/mod9/websocket/client.py`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/mod9/websocket/server.py` & `mod9-asr-1.9.0/mod9/websocket/server.py`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/mod9_asr.egg-info/PKG-INFO` & `mod9-asr-1.9.0/mod9_asr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mod9-asr
-Version: 1.8.0
+Version: 1.9.0
 Summary: Mod9 ASR Python SDK, REST API, and Websocket Interface: high-level interfaces to the Mod9 ASR Engine.
 Home-page: https://github.com/mod9-asr/python-sdk
 Author: Mod9 Technologies
 Author-email: support@mod9.com
 License: BSD 2-Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mod9-asr-1.8.0/mod9_asr.egg-info/SOURCES.txt` & `mod9-asr-1.9.0/mod9_asr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/setup.py` & `mod9-asr-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `mod9-asr-1.8.0/test/test_mod9_synchronous.py` & `mod9-asr-1.9.0/test/test_mod9_synchronous.py`

 * *Files identical despite different names*

