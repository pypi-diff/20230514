# Comparing `tmp/pypinyin-0.9.4.tar.gz` & `tmp/pypinyin-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypinyin-0.9.4.tar", last modified: Fri Nov 27 08:05:13 2015, max compression
+gzip compressed data, was "dist/pypinyin-0.9.5.tar", last modified: Sat Dec 19 10:42:01 2015, max compression
```

## Comparing `pypinyin-0.9.4.tar` & `pypinyin-0.9.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2015-11-27 08:05:13.000000 pypinyin-0.9.4/
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2015-11-27 08:05:13.000000 pypinyin-0.9.4/pypinyin.egg-info/
--rw-rw-r--   0 mg        (1000) mg        (1000)        9 2015-11-27 08:05:13.000000 pypinyin-0.9.4/pypinyin.egg-info/top_level.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)        1 2014-07-12 00:27:01.000000 pypinyin-0.9.4/pypinyin.egg-info/not-zip-safe
--rw-rw-r--   0 mg        (1000) mg        (1000)        1 2015-11-27 08:05:13.000000 pypinyin-0.9.4/pypinyin.egg-info/dependency_links.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)     8077 2015-11-27 08:05:13.000000 pypinyin-0.9.4/pypinyin.egg-info/PKG-INFO
--rw-rw-r--   0 mg        (1000) mg        (1000)       53 2015-11-27 08:05:13.000000 pypinyin-0.9.4/pypinyin.egg-info/entry_points.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)      399 2015-11-27 08:05:13.000000 pypinyin-0.9.4/pypinyin.egg-info/SOURCES.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)     1105 2014-04-30 05:26:59.000000 pypinyin-0.9.4/LICENSE.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)     5549 2015-11-27 08:01:21.000000 pypinyin-0.9.4/README.rst
--rw-rw-r--   0 mg        (1000) mg        (1000)     8077 2015-11-27 08:05:13.000000 pypinyin-0.9.4/PKG-INFO
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2015-11-27 08:05:13.000000 pypinyin-0.9.4/pypinyin/
--rw-rw-r--   0 mg        (1000) mg        (1000)  2080844 2015-10-14 14:45:05.000000 pypinyin-0.9.4/pypinyin/phrases_dict.py
--rw-rw-r--   0 mg        (1000) mg        (1000)     3308 2015-10-17 01:12:47.000000 pypinyin-0.9.4/pypinyin/runner.py
--rw-rw-r--   0 mg        (1000) mg        (1000)    15676 2015-11-27 08:01:35.000000 pypinyin-0.9.4/pypinyin/__init__.py
--rw-rw-r--   0 mg        (1000) mg        (1000)  2120800 2015-08-29 06:23:09.000000 pypinyin-0.9.4/pypinyin/pinyin_dict.py
--rw-rw-r--   0 mg        (1000) mg        (1000)      638 2015-11-15 13:26:20.000000 pypinyin-0.9.4/pypinyin/phonetic_symbol.py
--rw-rw-r--   0 mg        (1000) mg        (1000)      132 2014-04-30 05:26:59.000000 pypinyin-0.9.4/pypinyin/__main__.py
--rw-rw-r--   0 mg        (1000) mg        (1000)       45 2014-04-30 05:26:59.000000 pypinyin-0.9.4/MANIFEST.in
--rw-rw-r--   0 mg        (1000) mg        (1000)     1987 2015-11-15 13:26:20.000000 pypinyin-0.9.4/setup.py
--rw-rw-r--   0 mg        (1000) mg        (1000)       82 2015-11-27 08:05:13.000000 pypinyin-0.9.4/setup.cfg
--rw-rw-r--   0 mg        (1000) mg        (1000)     7051 2015-11-27 08:01:21.000000 pypinyin-0.9.4/CHANGELOG.rst
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2015-12-19 10:42:01.000000 pypinyin-0.9.5/
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2015-12-19 10:42:01.000000 pypinyin-0.9.5/pypinyin.egg-info/
+-rw-rw-r--   0 mg        (1000) mg        (1000)        9 2015-12-19 10:42:00.000000 pypinyin-0.9.5/pypinyin.egg-info/top_level.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)        1 2014-07-12 00:27:01.000000 pypinyin-0.9.5/pypinyin.egg-info/not-zip-safe
+-rw-rw-r--   0 mg        (1000) mg        (1000)        1 2015-12-19 10:42:00.000000 pypinyin-0.9.5/pypinyin.egg-info/dependency_links.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)     8077 2015-12-19 10:42:00.000000 pypinyin-0.9.5/pypinyin.egg-info/PKG-INFO
+-rw-rw-r--   0 mg        (1000) mg        (1000)       53 2015-12-19 10:42:00.000000 pypinyin-0.9.5/pypinyin.egg-info/entry_points.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)      399 2015-12-19 10:42:01.000000 pypinyin-0.9.5/pypinyin.egg-info/SOURCES.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)     1105 2014-04-30 05:26:59.000000 pypinyin-0.9.5/LICENSE.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)     5549 2015-11-27 08:01:21.000000 pypinyin-0.9.5/README.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)     8077 2015-12-19 10:42:01.000000 pypinyin-0.9.5/PKG-INFO
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2015-12-19 10:42:01.000000 pypinyin-0.9.5/pypinyin/
+-rw-rw-r--   0 mg        (1000) mg        (1000)  2080844 2015-10-14 14:45:05.000000 pypinyin-0.9.5/pypinyin/phrases_dict.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)     3308 2015-10-17 01:12:47.000000 pypinyin-0.9.5/pypinyin/runner.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)    16040 2015-12-19 10:39:08.000000 pypinyin-0.9.5/pypinyin/__init__.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)  2120800 2015-08-29 06:23:09.000000 pypinyin-0.9.5/pypinyin/pinyin_dict.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)      675 2015-12-19 10:28:55.000000 pypinyin-0.9.5/pypinyin/phonetic_symbol.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)      132 2014-04-30 05:26:59.000000 pypinyin-0.9.5/pypinyin/__main__.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)       45 2014-04-30 05:26:59.000000 pypinyin-0.9.5/MANIFEST.in
+-rw-rw-r--   0 mg        (1000) mg        (1000)     1987 2015-11-15 13:26:20.000000 pypinyin-0.9.5/setup.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)       82 2015-12-19 10:42:01.000000 pypinyin-0.9.5/setup.cfg
+-rw-rw-r--   0 mg        (1000) mg        (1000)     7611 2015-12-19 10:28:55.000000 pypinyin-0.9.5/CHANGELOG.rst
```

### Comparing `pypinyin-0.9.4/pypinyin.egg-info/PKG-INFO` & `pypinyin-0.9.5/pypinyin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pypinyin
-Version: 0.9.4
+Version: 0.9.5
 Summary: 汉语拼音转换工具.
 Home-page: https://github.com/mozillazg/python-pinyin
 Author: mozillazg, 闲耘
 Author-email: mozillazg101@gmail.com
 License: MIT
 Description: 汉语拼音转换工具（Python 版）
         =============================
```

### Comparing `pypinyin-0.9.4/LICENSE.txt` & `pypinyin-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypinyin-0.9.4/README.rst` & `pypinyin-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `pypinyin-0.9.4/PKG-INFO` & `pypinyin-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pypinyin
-Version: 0.9.4
+Version: 0.9.5
 Summary: 汉语拼音转换工具.
 Home-page: https://github.com/mozillazg/python-pinyin
 Author: mozillazg, 闲耘
 Author-email: mozillazg101@gmail.com
 License: MIT
 Description: 汉语拼音转换工具（Python 版）
         =============================
```

### Comparing `pypinyin-0.9.4/pypinyin/phrases_dict.py` & `pypinyin-0.9.5/pypinyin/phrases_dict.py`

 * *Files identical despite different names*

### Comparing `pypinyin-0.9.4/pypinyin/runner.py` & `pypinyin-0.9.5/pypinyin/runner.py`

 * *Files identical despite different names*

### Comparing `pypinyin-0.9.4/pypinyin/__init__.py` & `pypinyin-0.9.5/pypinyin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 import re
 import sys
 
 from . import phonetic_symbol, pinyin_dict
 
 __title__ = 'pypinyin'
-__version__ = '0.9.4'
+__version__ = '0.9.5'
 __author__ = 'mozillazg, 闲耘'
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) 2014 mozillazg, 闲耘'
 __all__ = [
     'pinyin', 'lazy_pinyin', 'slug',
     'STYLE_NORMAL', 'NORMAL',
     'STYLE_TONE', 'TONE',
@@ -254,15 +254,15 @@
     if pinyin.startswith('y'):
         if pinyin.startswith('yu'):
             pinyin = 'v' + pinyin[2:]
         elif pinyin.startswith('yi'):
             pinyin = pinyin[1:]
         else:
             pinyin = 'i' + pinyin[1:]
-    if pinyin.startswith('w'):
+    elif pinyin.startswith('w'):
         if pinyin.startswith('wu'):
             pinyin = pinyin[1:]
         else:
             pinyin = 'u' + pinyin[1:]
     return pinyin
 
 
@@ -279,15 +279,19 @@
         return initial(pinyin)
 
     def _replace(m):
         symbol = m.group(0)  # 带声调的字符
         # 不包含声调
         if style in [NORMAL, FIRST_LETTER, FINALS]:
             # 去掉声调: a1 -> a
-            return re.sub(RE_TONE2, r'\1', PHONETIC_SYMBOL[symbol])
+            # 鼻音: 'ḿ', 'ń', 'ň', 'ǹ '
+            if symbol in ['\u1e3f', '\u0144', '\u0148', '\u01f9']:
+                return re.sub(r'\d', r'', PHONETIC_SYMBOL[symbol])
+            else:
+                return re.sub(RE_TONE2, r'\1', PHONETIC_SYMBOL[symbol])
         # 使用数字标识声调
         elif style in [TONE2, FINALS_TONE2]:
             # 返回使用数字标识声调的字符
             return PHONETIC_SYMBOL[symbol]
         # 声调在头上
         else:
             return symbol
@@ -296,15 +300,19 @@
     py = re.sub(RE_PHONETIC_SYMBOL, _replace, pinyin)
 
     # 首字母
     if style == FIRST_LETTER:
         py = py[0]
     # 韵母
     elif style in [FINALS, FINALS_TONE, FINALS_TONE2]:
-        py = final(py)
+        # 不处理鼻音: 'ḿ', 'ń', 'ň', 'ǹ '
+        if pinyin and pinyin[0] not in [
+            '\u1e3f', '\u0144', '\u0148', '\u01f9'
+        ]:
+            py = final(py)
     return py
 
 
 def _handle_nopinyin_char(chars, errors='default'):
     """处理没有拼音的字符"""
     if callable(errors):
         return errors(chars)
```

### Comparing `pypinyin-0.9.4/pypinyin/pinyin_dict.py` & `pypinyin-0.9.5/pypinyin/pinyin_dict.py`

 * *Files identical despite different names*

### Comparing `pypinyin-0.9.4/pypinyin/phonetic_symbol.py` & `pypinyin-0.9.5/pypinyin/phonetic_symbol.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,10 +27,12 @@
     "ù": "u4",
     "ü": "v0",
     "ǘ": "v2",
     "ǚ": "v3",
     "ǜ": "v4",
     "ń": "n2",
     "ň": "n3",
-    "": "m2"
+    "ǹ": "n4",
+    # "": "m2"
+    "\u1e3f": "m2"
 }
 phonetic_symbol_reverse = dict((v, k) for k, v in phonetic_symbol.items())
```

### Comparing `pypinyin-0.9.4/setup.py` & `pypinyin-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `pypinyin-0.9.4/CHANGELOG.rst` & `pypinyin-0.9.5/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 ---------
 
+0.9.5 (2015-12-19)
+++++++++++++++++++++
+
+* **[Bugfixed]** 修复未正确处理鼻音（详见 `汉语拼音 - 维基百科`_ ）的问题(`#31`_ 感谢 `@xulin97`_ 汇报):
+
+  * ``ḿ、ń、ň、ǹ`` 对应 “呒”、“呣”、“唔”、“嗯”等字。
+    这些字之前在各种风格下都输出原始的汉字而不是拼音。
+
 
 0.9.4 (2015-11-27)
 ++++++++++++++++++++
 
 * **[Improved]** 细微调整，主要是更新文档
 
 
@@ -255,7 +263,10 @@
 * **[New]** Initial Release
 
 .. _#17: https://github.com/mozillazg/python-pinyin/pull/17
 .. _#22: https://github.com/mozillazg/python-pinyin/pull/22
 .. _#26: https://github.com/mozillazg/python-pinyin/pull/26
 .. _@MingStar: https://github.com/MingStar
 .. _汉语拼音方案: http://www.edu.cn/20011114/3009777.shtml
+.. _汉语拼音 - 维基百科: https://zh.wikipedia.org/wiki/%E6%B1%89%E8%AF%AD%E6%8B%BC%E9%9F%B3#cite_ref-10
+.. _@xulin97: https://github.com/xulin97
+.. _#31: https://github.com/mozillazg/python-pinyin/issues/31
```

