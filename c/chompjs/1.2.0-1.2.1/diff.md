# Comparing `tmp/chompjs-1.2.0.tar.gz` & `tmp/chompjs-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chompjs-1.2.0.tar", last modified: Mon May  8 04:46:39 2023, max compression
+gzip compressed data, was "chompjs-1.2.1.tar", last modified: Thu May 11 01:41:46 2023, max compression
```

## Comparing `chompjs-1.2.0.tar` & `chompjs-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-08 04:46:39.510076 chompjs-1.2.0/
--rw-r--r--   0 mariusz   (1000) mariusz   (1000)     1062 2020-02-27 18:25:01.000000 chompjs-1.2.0/LICENSE
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       15 2022-08-22 13:00:05.000000 chompjs-1.2.0/MANIFEST.in
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    10541 2023-05-08 04:46:39.510076 chompjs-1.2.0/PKG-INFO
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     7742 2023-05-08 04:36:34.000000 chompjs-1.2.0/README.md
-drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-08 04:46:39.510076 chompjs-1.2.0/_chompjs/
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     1735 2023-04-21 12:26:12.000000 chompjs-1.2.0/_chompjs/buffer.c
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)      976 2023-04-21 12:26:15.000000 chompjs-1.2.0/_chompjs/buffer.h
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     5289 2023-05-08 02:40:08.000000 chompjs-1.2.0/_chompjs/module.c
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    12315 2023-05-08 02:40:08.000000 chompjs-1.2.0/_chompjs/parser.c
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     3132 2023-05-08 02:40:08.000000 chompjs-1.2.0/_chompjs/parser.h
-drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-08 04:46:39.510076 chompjs-1.2.0/chompjs/
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       55 2023-05-08 02:17:42.000000 chompjs-1.2.0/chompjs/__init__.py
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     3468 2023-05-08 04:32:36.000000 chompjs-1.2.0/chompjs/chompjs.py
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    10944 2023-05-08 03:23:28.000000 chompjs-1.2.0/chompjs/test_parser.py
-drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-08 04:46:39.510076 chompjs-1.2.0/chompjs.egg-info/
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    10541 2023-05-08 04:46:39.000000 chompjs-1.2.0/chompjs.egg-info/PKG-INFO
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)      314 2023-05-08 04:46:39.000000 chompjs-1.2.0/chompjs.egg-info/SOURCES.txt
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)        1 2023-05-08 04:46:39.000000 chompjs-1.2.0/chompjs.egg-info/dependency_links.txt
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       17 2023-05-08 04:46:39.000000 chompjs-1.2.0/chompjs.egg-info/top_level.txt
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       38 2023-05-08 04:46:39.510076 chompjs-1.2.0/setup.cfg
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     1764 2023-05-08 04:45:20.000000 chompjs-1.2.0/setup.py
+drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-11 01:41:46.058902 chompjs-1.2.1/
+-rw-r--r--   0 mariusz   (1000) mariusz   (1000)     1062 2020-02-27 18:25:01.000000 chompjs-1.2.1/LICENSE
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       15 2022-08-22 13:00:05.000000 chompjs-1.2.1/MANIFEST.in
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     8897 2023-05-11 01:41:46.058902 chompjs-1.2.1/PKG-INFO
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     6290 2023-05-10 13:40:46.000000 chompjs-1.2.1/README.md
+drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-11 01:41:46.058902 chompjs-1.2.1/_chompjs/
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     1735 2023-04-21 12:26:12.000000 chompjs-1.2.1/_chompjs/buffer.c
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)      976 2023-04-21 12:26:15.000000 chompjs-1.2.1/_chompjs/buffer.h
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     5281 2023-05-11 01:40:03.000000 chompjs-1.2.1/_chompjs/module.c
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    12315 2023-05-08 02:40:08.000000 chompjs-1.2.1/_chompjs/parser.c
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     3132 2023-05-08 02:40:08.000000 chompjs-1.2.1/_chompjs/parser.h
+drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-11 01:41:46.058902 chompjs-1.2.1/chompjs/
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       55 2023-05-08 02:17:42.000000 chompjs-1.2.1/chompjs/__init__.py
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     3468 2023-05-08 04:32:36.000000 chompjs-1.2.1/chompjs/chompjs.py
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    10944 2023-05-08 03:23:28.000000 chompjs-1.2.1/chompjs/test_parser.py
+drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-11 01:41:46.058902 chompjs-1.2.1/chompjs.egg-info/
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     8897 2023-05-11 01:41:46.000000 chompjs-1.2.1/chompjs.egg-info/PKG-INFO
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)      314 2023-05-11 01:41:46.000000 chompjs-1.2.1/chompjs.egg-info/SOURCES.txt
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)        1 2023-05-11 01:41:46.000000 chompjs-1.2.1/chompjs.egg-info/dependency_links.txt
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       17 2023-05-11 01:41:46.000000 chompjs-1.2.1/chompjs.egg-info/top_level.txt
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       38 2023-05-11 01:41:46.058902 chompjs-1.2.1/setup.cfg
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     1764 2023-05-11 01:40:03.000000 chompjs-1.2.1/setup.py
```

### Comparing `chompjs-1.2.0/LICENSE` & `chompjs-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chompjs-1.2.0/README.md` & `chompjs-1.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Chompjs
 
 ![license](https://img.shields.io/github/license/Nykakin/chompjs?style=flat-square)
 ![pypi version](https://img.shields.io/pypi/v/chompjs.svg)
 ![python version](https://img.shields.io/pypi/pyversions/chompjs.svg)
 ![downloads](https://img.shields.io/pypi/dm/chompjs.svg)
 
-Transforms JavaScript objects into Python dictionaries.
+Transforms JavaScript objects into Python data structures.
 
-In web scraping, you sometimes need to transform Javascript objects embedded in HTML pages into valid Python dictionaries. `chompjs` is a library designed to be a more powerful replacement of standard `json.loads`.
+In web scraping, you sometimes need to transform Javascript objects embedded in HTML pages into valid Python dictionaries. `chompjs` is a library designed to do that as a more powerful replacement of standard `json.loads`:
 
 ```python
 >>> chompjs.parse_js_object("{a: 100}")
 {'a': 100}
 >>>
 >>> json_lines = """
 ... {'a': 12}
@@ -45,15 +45,15 @@
 $ python setup.py install
 ```
 
 ## Features
 
 There are two functions available:
 * `parse_js_object` - try reading first encountered JSON-like object. Raises `ValueError` on failure
-* `parse_js_objects` - returns a generator yielding all encountered JSON-like objects. Can be used to read [JSON Lines](https://jsonlines.org/)
+* `parse_js_objects` - returns a generator yielding all encountered JSON-like objects. Can be used to read [JSON Lines](https://jsonlines.org/). Does not raise on ivalid input.
 
 An example usage with `scrapy`:
 
 ```python
 import chompjs
 import scrapy
 
@@ -150,82 +150,58 @@
 * `"{'a': 'b'}"` is not a valid JSON because it uses `'` character to quote
 * `'{a: "b"}'`is not a valid JSON because property name is not quoted at all
 * `'{"a": [1, 2, 3,]}'` is not a valid JSON because there is an extra `,` character at the end of the array
 * `'{"a": .99}'` is not a valid JSON because float value lacks a leading 0
 
 As a result, `json.loads` fail to extract any of those:
 
-```
+```python
 >>> json.loads("{'a': 'b'}")
 Traceback (most recent call last):
-  File "<console>", line 1, in <module>
-  File "/usr/lib/python3.10/json/__init__.py", line 339, in loads
-    return _default_decoder.decode(s)
-  File "/usr/lib/python3.10/json/decoder.py", line 364, in decode
-    obj, end = self.raw_decode(s, idx=_w(s, 0).end())
-  File "/usr/lib/python3.10/json/decoder.py", line 380, in raw_decode
-    obj, end = self.scan_once(s, idx)
+  ...
 ValueError: Expecting property name: line 1 column 2 (char 1)
 >>> json.loads('{a: "b"}')
 Traceback (most recent call last):
-  File "<console>", line 1, in <module>
-  File "/usr/lib/python3.10/json/__init__.py", line 339, in loads
-    return _default_decoder.decode(s)
-  File "/usr/lib/python3.10/json/decoder.py", line 364, in decode
-    obj, end = self.raw_decode(s, idx=_w(s, 0).end())
-  File "/usr/lib/python3.10/json/decoder.py", line 380, in raw_decode
-    obj, end = self.scan_once(s, idx)
+  ...
 ValueError: Expecting property name: line 1 column 2 (char 1)
 >>> json.loads('{"a": [1, 2, 3,]}')
 Traceback (most recent call last):
-  File "<console>", line 1, in <module>
-  File "/usr/lib/python3.10/json/__init__.py", line 339, in loads
-    return _default_decoder.decode(s)
-  File "/usr/lib/python3.10/json/decoder.py", line 364, in decode
-    obj, end = self.raw_decode(s, idx=_w(s, 0).end())
-  File "/usr/lib/python3.10/json/decoder.py", line 382, in raw_decode
-    raise ValueError("No JSON object could be decoded")
+  ...
 ValueError: No JSON object could be decoded
 >>> json.loads('{"a": .99}')
 Traceback (most recent call last):
-  File "<stdin>", line 1, in <module>
-  File "/usr/lib/python3.7/json/__init__.py", line 348, in loads
-    return _default_decoder.decode(s)
-  File "/usr/lib/python3.7/json/decoder.py", line 337, in decode
-    obj, end = self.raw_decode(s, idx=_w(s, 0).end())
-  File "/usr/lib/python3.7/json/decoder.py", line 355, in raw_decode
-    raise JSONDecodeError("Expecting value", s, err.value) from None
+  ...
 json.decoder.JSONDecodeError: Expecting value: line 1 column 7 (char 6)
 
 ```
 `chompjs` library was designed to bypass this limitation, and it allows to scrape such JavaScript objects into proper Python dictionaries:
 
-```
+```python
 >>> import chompjs
 >>> 
 >>> chompjs.parse_js_object("{'a': 'b'}")
-{u'a': u'b'}
+{'a': 'b'}
 >>> chompjs.parse_js_object('{a: "b"}')
-{u'a': u'b'}
+{'a': 'b'}
 >>> chompjs.parse_js_object('{"a": [1, 2, 3,]}')
-{u'a': [1, 2, 3]}
+{'a': [1, 2, 3]}
+>>> chompjs.parse_js_object('{"a": .99}')
+{'a': 0.99}
 ```
 
 Internally `chompjs` use a parser written in C to iterate over raw string, fixing its issues along the way. The final result is then passed down to standard library's `json.loads`, ensuring a high speed as compared to full-blown JavaScript parsers such as `demjson`.
 
-```
+```python
 >>> import json
 >>> import _chompjs
 >>> 
 >>> _chompjs.parse('{a: 1}')
 '{"a":1}'
 >>> json.loads(_)
-{u'a': 1}
->>> chompjs.parse_js_object('{"a": .99}')
-{'a': 0.99}
+{'a': 1}
 ```
 
 # Development
 Pull requests are welcome. 
 
 To run unittests
```

### Comparing `chompjs-1.2.0/_chompjs/buffer.c` & `chompjs-1.2.1/_chompjs/buffer.c`

 * *Files identical despite different names*

### Comparing `chompjs-1.2.0/_chompjs/buffer.h` & `chompjs-1.2.1/_chompjs/buffer.h`

 * *Files identical despite different names*

### Comparing `chompjs-1.2.0/_chompjs/module.c` & `chompjs-1.2.1/_chompjs/module.c`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         json_iter_state->lexer.output.index-1
     );
     reset_lexer_output(&json_iter_state->lexer);
     return ret;
 }
 
 PyTypeObject JSONIter_Type = {
-    PyVarObject_HEAD_INIT(&PyType_Type, 0)
+    PyVarObject_HEAD_INIT(NULL, 0)
     "json_iter",                    /* tp_name */
     sizeof(JsonIterState),          /* tp_basicsize */
     0,                              /* tp_itemsize */
     (destructor)json_iter_dealloc,  /* tp_dealloc */
     0,                              /* tp_print */
     0,                              /* tp_getattr */
     0,                              /* tp_setattr */
```

### Comparing `chompjs-1.2.0/_chompjs/parser.c` & `chompjs-1.2.1/_chompjs/parser.c`

 * *Files identical despite different names*

### Comparing `chompjs-1.2.0/_chompjs/parser.h` & `chompjs-1.2.1/_chompjs/parser.h`

 * *Files identical despite different names*

### Comparing `chompjs-1.2.0/chompjs/chompjs.py` & `chompjs-1.2.1/chompjs/chompjs.py`

 * *Files identical despite different names*

### Comparing `chompjs-1.2.0/chompjs/test_parser.py` & `chompjs-1.2.1/chompjs/test_parser.py`

 * *Files identical despite different names*

### Comparing `chompjs-1.2.0/setup.py` & `chompjs-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     sources=['_chompjs/module.c', '_chompjs/parser.c', '_chompjs/buffer.c'],
     extra_compile_args=extra_compile_args,
     extra_link_args=extra_link_args,
 )
 
 setup(
     name='chompjs',
-    version='1.2.0',
+    version='1.2.1',
     description='Parsing JavaScript objects into Python dictionaries',
     author='Mariusz Obajtek',
     author_email='nykakin@gmail.com',
     keywords='parsing parser JavaScript json json5 webscrapping',
     python_requires='>=3',
     ext_modules=[chompjs_extension],
     classifiers=[
```

