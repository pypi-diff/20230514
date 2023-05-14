# Comparing `tmp/TransLiter-0.3.2.tar.gz` & `tmp/TransLiter-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TransLiter-0.3.2.tar", last modified: Sat May 13 19:01:00 2023, max compression
+gzip compressed data, was "TransLiter-0.3.3.tar", last modified: Sun May 14 03:58:35 2023, max compression
```

## Comparing `TransLiter-0.3.2.tar` & `TransLiter-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-05-13 19:01:00.570048 TransLiter-0.3.2/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1067 2023-05-13 04:20:03.000000 TransLiter-0.3.2/LICENSE
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     7176 2023-05-13 19:01:00.569923 TransLiter-0.3.2/PKG-INFO
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     6841 2023-05-13 18:48:48.000000 TransLiter-0.3.2/README.md
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-05-13 19:01:00.568982 TransLiter-0.3.2/TransLiter/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      155 2023-05-13 13:05:00.000000 TransLiter-0.3.2/TransLiter/__init__.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     4918 2023-05-13 18:33:22.000000 TransLiter-0.3.2/TransLiter/cyrillic_list.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     3414 2023-05-13 04:20:03.000000 TransLiter-0.3.2/TransLiter/jp_list.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1832 2023-05-13 04:20:03.000000 TransLiter-0.3.2/TransLiter/ko_jamo.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      370 2023-05-13 04:20:03.000000 TransLiter-0.3.2/TransLiter/spacing.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     8668 2023-05-13 18:34:58.000000 TransLiter-0.3.2/TransLiter/transliter_cyrillic.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1920 2023-05-13 04:20:03.000000 TransLiter-0.3.2/TransLiter/transliter_jp.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     2990 2023-05-13 04:20:03.000000 TransLiter-0.3.2/TransLiter/transliter_ko.py
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-05-13 19:01:00.569748 TransLiter-0.3.2/TransLiter.egg-info/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     7176 2023-05-13 19:01:00.000000 TransLiter-0.3.2/TransLiter.egg-info/PKG-INFO
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      435 2023-05-13 19:01:00.000000 TransLiter-0.3.2/TransLiter.egg-info/SOURCES.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-05-13 19:01:00.000000 TransLiter-0.3.2/TransLiter.egg-info/dependency_links.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-05-13 19:01:00.000000 TransLiter-0.3.2/TransLiter.egg-info/not-zip-safe
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       16 2023-05-13 19:01:00.000000 TransLiter-0.3.2/TransLiter.egg-info/requires.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       11 2023-05-13 19:01:00.000000 TransLiter-0.3.2/TransLiter.egg-info/top_level.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       38 2023-05-13 19:01:00.570083 TransLiter-0.3.2/setup.cfg
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      652 2023-05-13 18:57:38.000000 TransLiter-0.3.2/setup.py
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-05-14 03:58:35.059828 TransLiter-0.3.3/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     1067 2023-05-13 04:20:03.000000 TransLiter-0.3.3/LICENSE
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     7204 2023-05-14 03:58:35.059695 TransLiter-0.3.3/PKG-INFO
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     6869 2023-05-14 03:54:37.000000 TransLiter-0.3.3/README.md
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-05-14 03:58:35.058683 TransLiter-0.3.3/TransLiter/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      155 2023-05-13 13:05:00.000000 TransLiter-0.3.3/TransLiter/__init__.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     5493 2023-05-14 03:41:44.000000 TransLiter-0.3.3/TransLiter/cyrillic_list.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     3414 2023-05-13 04:20:03.000000 TransLiter-0.3.3/TransLiter/jp_list.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     1832 2023-05-13 04:20:03.000000 TransLiter-0.3.3/TransLiter/ko_jamo.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      370 2023-05-13 04:20:03.000000 TransLiter-0.3.3/TransLiter/spacing.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     9667 2023-05-14 03:47:43.000000 TransLiter-0.3.3/TransLiter/transliter_cyrillic.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     1920 2023-05-13 04:20:03.000000 TransLiter-0.3.3/TransLiter/transliter_jp.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     2990 2023-05-13 04:20:03.000000 TransLiter-0.3.3/TransLiter/transliter_ko.py
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-05-14 03:58:35.059488 TransLiter-0.3.3/TransLiter.egg-info/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     7204 2023-05-14 03:58:35.000000 TransLiter-0.3.3/TransLiter.egg-info/PKG-INFO
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      435 2023-05-14 03:58:35.000000 TransLiter-0.3.3/TransLiter.egg-info/SOURCES.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-05-14 03:58:35.000000 TransLiter-0.3.3/TransLiter.egg-info/dependency_links.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-05-14 03:58:35.000000 TransLiter-0.3.3/TransLiter.egg-info/not-zip-safe
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       16 2023-05-14 03:58:35.000000 TransLiter-0.3.3/TransLiter.egg-info/requires.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       11 2023-05-14 03:58:35.000000 TransLiter-0.3.3/TransLiter.egg-info/top_level.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       38 2023-05-14 03:58:35.059867 TransLiter-0.3.3/setup.cfg
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      652 2023-05-14 03:41:53.000000 TransLiter-0.3.3/setup.py
```

### Comparing `TransLiter-0.3.2/LICENSE` & `TransLiter-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TransLiter-0.3.2/PKG-INFO` & `TransLiter-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TransLiter
-Version: 0.3.2
+Version: 0.3.3
 Summary: TransLiter transliterates multilingual text into Latin script.
 Home-page: https://github.com/elibooklover/TransLiter
 Author: Hoyeol Kim
 Author-email: elibooklover@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -14,21 +14,21 @@
 
 <div align=right>
 
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Felibooklover%2FTransLiter&count_bg=%235F3DC8&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 
 </div>
 
-TransLiter transliterates multilingual text into Latin script. | by Hoyeol Kim
+#### TransLiter transliterates multilingual text into Latin script | by Hoyeol Kim
 
-Currently, TransLiter supports Korean, Japanese, and Cyrillic (Russian, Ukrainian, Bulgarian, Macedonian, Montenegrin, and Serbian). More languages will be added to TransLiter in the future.
+Currently, TransLiter supports Korean, Japanese, and Cyrillic (Russian, Ukrainian, Bulgarian, Macedonian, Montenegrin, Serbian, and Tajiki). More languages will be added to TransLiter in the future.
 
 There are several functions in TransLiter, such as `tl.ko`, `tl.transliter_ko`, `tl.txt_ko`, and `tl.csv_ko`, in addition to spacing functions (`tl.spacing` and `tl.spacing_file`). To transliaterate from a language other than Korean, simply replace the language code `ko` with your desired language code.
 
-Language codes are as follows: `ko` (Korean), `jp` (Japanese), `ru` (Russian), `ua` (Ukrainian), `bg` (Bulgarian), `mk` (Macedonian), `me` (Montenegrin), and `sr` (Serbian).
+Language codes are as follows: `ko` (Korean), `jp` (Japanese), `ru` (Russian), `ua` (Ukrainian), `bg` (Bulgarian), `mk` (Macedonian), `me` (Montenegrin),  `sr` (Serbian), and `tj` (Tajiki).
 
 ---
 
 ## Install
 
 ```
 $ pip install TransLiter
```

### Comparing `TransLiter-0.3.2/README.md` & `TransLiter-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 <div align=right>
 
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Felibooklover%2FTransLiter&count_bg=%235F3DC8&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 
 </div>
 
-TransLiter transliterates multilingual text into Latin script. | by Hoyeol Kim
+#### TransLiter transliterates multilingual text into Latin script | by Hoyeol Kim
 
-Currently, TransLiter supports Korean, Japanese, and Cyrillic (Russian, Ukrainian, Bulgarian, Macedonian, Montenegrin, and Serbian). More languages will be added to TransLiter in the future.
+Currently, TransLiter supports Korean, Japanese, and Cyrillic (Russian, Ukrainian, Bulgarian, Macedonian, Montenegrin, Serbian, and Tajiki). More languages will be added to TransLiter in the future.
 
 There are several functions in TransLiter, such as `tl.ko`, `tl.transliter_ko`, `tl.txt_ko`, and `tl.csv_ko`, in addition to spacing functions (`tl.spacing` and `tl.spacing_file`). To transliaterate from a language other than Korean, simply replace the language code `ko` with your desired language code.
 
-Language codes are as follows: `ko` (Korean), `jp` (Japanese), `ru` (Russian), `ua` (Ukrainian), `bg` (Bulgarian), `mk` (Macedonian), `me` (Montenegrin), and `sr` (Serbian).
+Language codes are as follows: `ko` (Korean), `jp` (Japanese), `ru` (Russian), `ua` (Ukrainian), `bg` (Bulgarian), `mk` (Macedonian), `me` (Montenegrin),  `sr` (Serbian), and `tj` (Tajiki).
 
 ---
 
 ## Install
 
 ```
 $ pip install TransLiter
```

### Comparing `TransLiter-0.3.2/TransLiter/cyrillic_list.py` & `TransLiter-0.3.3/TransLiter/cyrillic_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,47 +7,44 @@
     "У": "U", "у": "u", "Ф": "F", "ф": "f", "Х": "X", "х": "x", "Ц": "CZ", "ц": "cz",
     "Ч": "CH", "ч": "ch", "Ш": "SH", "ш": "sh", "Щ": "SHH", "щ": "shh", "Ъ": "''", "ъ": "''",
     "Ы": "Y'", "ы": "y'", "Ь": "'", "ь": "'", "Э": "E'", "э": "e'", "Ю": "YU", "ю": "yu",
     "Я": "YA", "я": "ya"
 }
 
 ukrainian_list = {
-    "А": "A", "а": "a", "Б": "B", "б": "b", "В": "V", "в": "v", "Г": "G", "г": "g",
-    "Д": "D", "д": "d", "Е": "E", "е": "e", "Ж": "ZH", "ж": "zh", "З": "Z", "з": "z", 
-    "И": "I", "и": "i", "Й": "J", "й": "j", "К": "K", "к": "k", "Л": "L", "л": "l", 
+    "А": "A", "а": "a", "Б": "B", "б": "b", "В": "V", "в": "v", "Г": "H", "г": "h",
+    "Д": "D", "д": "d", "Е": "E", "е": "e", "Ж": "Ž", "ж": "ž", "З": "Z", "з": "z", 
+    "И": "Y", "и": "y", "Й": "J", "й": "j", "К": "K", "к": "k", "Л": "L", "л": "l", 
     "М": "M", "м": "m", "Н": "N", "н": "n", "О": "O", "о": "o", "П": "P", "п": "p", 
     "Р": "R", "р": "r", "С": "S", "с": "s", "Т": "T", "т": "t", "У": "U", "у": "u", 
-    "Ф": "F", "ф": "f", "Х": "X", "х": "x", "Ц": "CZ", "ц": "cz", "Ч": "CH", "ч": "ch", 
-    "Ш": "SH", "ш": "sh", "Щ": "SHH", "щ": "shh", "Ь": "'", "ь": "'", "Ю": "YU", "ю": "yu",
-    "Я": "YA", "я": "ya", "Г": "H", "г": "h", "Ж": "Ž", "ж": "ž", "И": "Y", "и": "y", 
-    "Х": "X", "х": "x", "Ц": "C", "ц": "c", "Ч": "Č", "ч": "č", "Ш": "Š", "ш": "š", 
-    "Щ": "Šč", "щ": "šč", "Ю": "Ju", "ю": "ju", "Я": "Ja", "я": "ja", "Ґ": "G", "ґ": "g", 
-    "Є": "Je", "є": "je", "І": "I", "і": "i", "Ї": "Ï", "ї": "ï"
+    "Ф": "F", "ф": "f", "Х": "X", "х": "x", "Ц": "C", "ц": "c", "Ч": "Č", "ч": "č", 
+    "Ш": "Š", "ш": "š", "Щ": "Šč", "щ": "šč", "Ь": "'", "ь": "'", "Ю": "Ju", "ю": "ju",
+    "Я": "Ja", "я": "ja", "Ґ": "G", "ґ": "g", "Є": "Je", "є": "je", "І": "I", "і": "i", "Ї": "Ï", "ї": "ï"
 }
 
 bulgarian_list = {
     "А": "A", "а": "a", "Б": "B", "б": "b", "В": "V", "в": "v", "Г": "G", "г": "g",
     "Д": "D", "д": "d", "Е": "E", "е": "e", "Ж": "ZH", "ж": "zh",
     "З": "Z", "з": "z", "И": "I", "и": "i", "Й": "Y", "й": "y", "К": "K", "к": "k",
     "Л": "L", "л": "l", "М": "M", "м": "m", "Н": "N", "н": "n", "О": "O", "о": "o",
     "П": "P", "п": "p", "Р": "R", "р": "r", "С": "S", "с": "s", "Т": "T", "т": "t",
     "У": "U", "у": "u", "Ф": "F", "ф": "f", "Х": "H", "х": "h", "Ц": "TS", "ц": "ts",
-    "Ч": "CH", "ч": "ch", "Ш": "SH", "ш": "sh", "Щ": "SHT", "щ": "sht", "Ъ": "''", "ъ": "''",
-    "Ь": "'", "ь": "'", "Ю": "YU", "ю": "yu", "Я": "YA", "я": "ya", "Ъ": "Ă", "ъ": "ă", "Ь": "J", "ь": "j"
+    "Ч": "CH", "ч": "ch", "Ш": "SH", "ш": "sh", "Щ": "SHT", "щ": "sht", 
+    "Ъ": "Ă", "ъ": "ă", "Ь": "J", "ь": "j", "Ю": "YU", "ю": "yu", "Я": "YA", "я": "ya" 
 }
 
 macedonian_list = {
     "А": "A", "а": "a", "Б": "B", "б": "b", "В": "V", "в": "v", "Г": "G", "г": "g",
     "Д": "D", "д": "d", "Е": "E", "е": "e", "Ж": "Ž", "ж": "ž", "З": "Z", "з": "z", 
-    "И": "I", "и": "i", "Ј": "J", "ј": "j", "К": "K", "к": "k", "Л": "L", "л": "l", 
-    "Љ": "Lj", "љ": "lj", "М": "M", "м": "m", "Н": "N", "н": "n", "Њ": "Nj", "њ": "nj", 
-    "О": "O", "о": "o", "П": "P", "п": "p", "Р": "R", "р": "r", "С": "S", "с": "s", 
-    "Т": "T", "т": "t", "У": "U", "у": "u", "Ф": "F", "ф": "f", "Х": "H", "х": "h", 
-    "Ц": "C", "ц": "c", "Ч": "Č", "ч": "č", "Џ": "Dž", "џ": "dž", "Ш": "Š", "ш": "š", 
-    "Ѕ": "Dz", "ѕ": "dz", "Ѓ": "Ǵ", "ѓ": "ǵ", "Ќ": "Ḱ", "ќ": "ḱ"
+    "И": "I", "и": "i", "Ј": "J", "ј": "j", "К": "K", "к": "k","Ќ": "Ḱ", "ќ": "ḱ", 
+    "Л": "L", "л": "l", "Ѓ": "Ǵ", "ѓ": "ǵ", "Љ": "Lj", "љ": "lj", "М": "M", "м": "m", 
+    "Н": "N", "н": "n", "Њ": "Nj", "њ": "nj", "О": "O", "о": "o", "П": "P", "п": "p", 
+    "Р": "R", "р": "r", "С": "S", "с": "s", "Т": "T", "т": "t", "У": "U", "у": "u", 
+    "Ф": "F", "ф": "f", "Х": "H", "х": "h", "Ц": "C", "ц": "c", "Ч": "Č", "ч": "č", 
+    "Џ": "Dž", "џ": "dž", "Ш": "Š", "ш": "š", "Ѕ": "Dz", "ѕ": "dz"
 }
 
 montenegrin_list = {
     "А": "A", "а": "a", "Б": "B", "б": "b", "В": "V", "в": "v", "Г": "G", "г": "g",
     "Д": "D", "д": "d", "Ђ": "Đ", "ђ": "đ", "Е": "E", "е": "e", "Ж": "Ž", "ж": "ž",
     "З": "Z", "з": "z", "И": "I", "и": "i", "Ј": "J", "ј": "j", "К": "K", "к": "k",
     "Л": "L", "л": "l", "Љ": "Lj", "љ": "lj", "М": "M", "м": "m", "Н": "N", "н": "n",
@@ -63,7 +60,17 @@
     "З": "Z", "з": "z", "И": "I", "и": "i", "Ј": "J", "ј": "j", "К": "K", "к": "k",
     "Л": "L", "л": "l", "Љ": "Lj", "љ": "lj", "М": "M", "м": "m", "Н": "N", "н": "n",
     "Њ": "Nj", "њ": "nj", "О": "O", "о": "o", "П": "P", "п": "p", "Р": "R", "р": "r",
     "С": "S", "с": "s", "Т": "T", "т": "t", "Ћ": "Ć", "ћ": "ć", "У": "U", "у": "u",
     "Ф": "F", "ф": "f", "Х": "H", "х": "h", "Ц": "C", "ц": "c", "Ч": "Č", "ч": "č",
     "Џ": "Dž", "џ": "dž", "Ш": "Š", "ш": "š"
 }
+
+tajiki_list = {
+    "А": "A", "а": "a", "Я": "Â", "я": "â", "Б": "B", "б": "b", "В": "V", "в": "v", "Г": "G", "г": "g", 
+    "Ғ": "Ǧ", "ғ": "ǧ", "Д": "D", "д": "d", "Е": "E", "е": "e", "Ё": "Ë", "ё": "ë", "Ж": "Ž", "ж": "ž",
+    "З": "Z", "з": "z", "И": "I", "и": "i", "Ӣ": "Ī", "ӣ": "ī", "Й": "J", "й": "j", "К": "K", "к": "k",
+    "Л": "L", "л": "l", "М": "M", "м": "m", "Н": "N", "н": "n", "О": "O", "о": "o", "П": "P", "п": "p", 
+    "Р": "R", "р": "r", "С": "S", "с": "s", "Т": "T", "т": "t", "У": "U", "у": "u", "Ф": "F", "ф": "f", 
+    "Х": "H", "х": "h", "Ч": "Č", "ч": "č", "Ш": "Š", "ш": "š", "Ъ": "''", "ъ": "’", "Ь": "'", "ь": "'", 
+    "Э": "È", "э": "è", "Ю": "Û", "ю": "û", "Қ": "Q", "қ": "q", "Ӯ": "Ū", "ӯ": "ū", "Ҳ": "Ḩ", "ҳ": "ḩ", "Ҷ": "Ç", "ҷ": "ç"
+}
```

### Comparing `TransLiter-0.3.2/TransLiter/jp_list.py` & `TransLiter-0.3.3/TransLiter/jp_list.py`

 * *Files identical despite different names*

### Comparing `TransLiter-0.3.2/TransLiter/ko_jamo.py` & `TransLiter-0.3.3/TransLiter/ko_jamo.py`

 * *Files identical despite different names*

### Comparing `TransLiter-0.3.2/TransLiter/transliter_cyrillic.py` & `TransLiter-0.3.3/TransLiter/transliter_cyrillic.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,222 +10,35 @@
                 transliterated_text += russian_list[letter]
             else:
                 transliterated_text += letter
         except KeyError:
             pass
     return transliterated_text
 
-# Ukrainian
-def ua(text):
-    transliterated_text = ""
-    for letter in text:
-        try: 
-            if letter in ukrainian_list:
-                transliterated_text += ukrainian_list[letter]
-            else:
-                transliterated_text += letter
-        except KeyError:
-            pass
-    return transliterated_text
-
-# Bulgarian
-def bg(text):
-    transliterated_text = ""
-    for letter in text:
-        try: 
-            if letter in bulgarian_list:
-                transliterated_text += bulgarian_list[letter]
-            else:
-                transliterated_text += letter
-        except KeyError:
-            pass
-    return transliterated_text
-
-# Macedonian
-def mk(text):
-    transliterated_text = ""
-    for letter in text:
-        try: 
-            if letter in macedonian_list:
-                transliterated_text += macedonian_list[letter]
-            else:
-                transliterated_text += letter
-        except KeyError:
-            pass
-    return transliterated_text
-
-# Montenegrin
-def me(text):
-    transliterated_text = ""
-    for letter in text:
-        try: 
-            if letter in montenegrin_list:
-                transliterated_text += montenegrin_list[letter]
-            else:
-                transliterated_text += letter
-        except KeyError:
-            pass
-    return transliterated_text
-
-# Serbian
-def sr(text):
-    transliterated_text = ""
-    for letter in text:
-        try: 
-            if letter in serbian_list:
-                transliterated_text += serbian_list[letter]
-            else:
-                transliterated_text += letter
-        except KeyError:
-            pass
-    return transliterated_text
-
-
-# Trnasliter Function for each language
-# Russian
 def transliter_ru():
     while True:
         input_text = input("Please enter Russian text: ")
         print(ru(input_text))
         if input_text == "": 
             break
 
-# Ukrainian
-def transliter_ua():
-    while True:
-        input_text = input("Please enter Ukrainian text: ")
-        print(ua(input_text))
-        if input_text == "": 
-            break
-
-# Bulgarian
-def transliter_bg():
-    while True:
-        input_text = input("Please enter Bulgarian text: ")
-        print(bg(input_text))
-        if input_text == "": 
-            break
-
-# Macedonian
-def transliter_mk():
-    while True:
-        input_text = input("Please enter Macedonian text: ")
-        print(mk(input_text))
-        if input_text == "": 
-            break
-
-# Montenegrin
-def transliter_me():
-    while True:
-        input_text = input("Please enter Montenegrin text: ")
-        print(me(input_text))
-        if input_text == "": 
-            break
-
-# Serbian
-def transliter_sr():
-    while True:
-        input_text = input("Please enter Serbian text: ")
-        print(sr(input_text))
-        if input_text == "": 
-            break
-
-# Automatic generation of a txt file for each language
-# Russian
 def txt_ru(file):
     f = open(file, 'r')
     f2 = open("output_ru.txt", 'w')
     result = ""
     while True:
         line = f.readline()
         result += line + ru(line)
         if not line: 
             break
     print(result)
     f2.write(result)
     f.close()
     f2.close()
 
-# Ukrainian
-def txt_ua(file):
-    f = open(file, 'r')
-    f2 = open("output_ua.txt", 'w')
-    result = ""
-    while True:
-        line = f.readline()
-        result += line + ua(line)
-        if not line: 
-            break
-    print(result)
-    f2.write(result)
-    f.close()
-    f2.close()
-
-# Bulgarian
-def txt_bg(file):
-    f = open(file, 'r')
-    f2 = open("output_bg.txt", 'w')
-    result = ""
-    while True:
-        line = f.readline()
-        result += line + bg(line)
-        if not line: 
-            break
-    print(result)
-    f2.write(result)
-    f.close()
-    f2.close()
-
-# Macedonian
-def txt_mk(file):
-    f = open(file, 'r')
-    f2 = open("output_mk.txt", 'w')
-    result = ""
-    while True:
-        line = f.readline()
-        result += line + mk(line)
-        if not line: 
-            break
-    print(result)
-    f2.write(result)
-    f.close()
-    f2.close()
-
-# Montenegrin
-def txt_me(file):
-    f = open(file, 'r')
-    f2 = open("output_me.txt", 'w')
-    result = ""
-    while True:
-        line = f.readline()
-        result += line + me(line)
-        if not line: 
-            break
-    print(result)
-    f2.write(result)
-    f.close()
-    f2.close()
-
-# Serbian
-def txt_sr(file):
-    f = open(file, 'r')
-    f2 = open("output_sr.txt", 'w')
-    result = ""
-    while True:
-        line = f.readline()
-        result += line + sr(line)
-        if not line: 
-            break
-    print(result)
-    f2.write(result)
-    f.close()
-    f2.close()
-
-# Automatic generation of a csv file for each language
-# Russian
 def csv_ru(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
@@ -238,14 +51,47 @@
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
     data.to_csv("output_ru.csv", encoding="utf-8-sig")
     print(data)
     f.close()
 
 # Ukrainian
+def ua(text):
+    transliterated_text = ""
+    for letter in text:
+        try: 
+            if letter in ukrainian_list:
+                transliterated_text += ukrainian_list[letter]
+            else:
+                transliterated_text += letter
+        except KeyError:
+            pass
+    return transliterated_text
+
+def transliter_ua():
+    while True:
+        input_text = input("Please enter Ukrainian text: ")
+        print(ua(input_text))
+        if input_text == "": 
+            break
+
+def txt_ua(file):
+    f = open(file, 'r')
+    f2 = open("output_ua.txt", 'w')
+    result = ""
+    while True:
+        line = f.readline()
+        result += line + ua(line)
+        if not line: 
+            break
+    print(result)
+    f2.write(result)
+    f.close()
+    f2.close()
+
 def csv_ua(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
@@ -258,14 +104,47 @@
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
     data.to_csv("output_ua.csv", encoding="utf-8-sig")
     print(data)
     f.close()
 
 # Bulgarian
+def bg(text):
+    transliterated_text = ""
+    for letter in text:
+        try: 
+            if letter in bulgarian_list:
+                transliterated_text += bulgarian_list[letter]
+            else:
+                transliterated_text += letter
+        except KeyError:
+            pass
+    return transliterated_text
+
+def transliter_bg():
+    while True:
+        input_text = input("Please enter Bulgarian text: ")
+        print(bg(input_text))
+        if input_text == "": 
+            break
+
+def txt_bg(file):
+    f = open(file, 'r')
+    f2 = open("output_bg.txt", 'w')
+    result = ""
+    while True:
+        line = f.readline()
+        result += line + bg(line)
+        if not line: 
+            break
+    print(result)
+    f2.write(result)
+    f.close()
+    f2.close()
+
 def csv_bg(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
@@ -278,14 +157,47 @@
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
     data.to_csv("output_bg.csv", encoding="utf-8-sig")
     print(data)
     f.close()
 
 # Macedonian
+def mk(text):
+    transliterated_text = ""
+    for letter in text:
+        try: 
+            if letter in macedonian_list:
+                transliterated_text += macedonian_list[letter]
+            else:
+                transliterated_text += letter
+        except KeyError:
+            pass
+    return transliterated_text
+
+def transliter_mk():
+    while True:
+        input_text = input("Please enter Macedonian text: ")
+        print(mk(input_text))
+        if input_text == "": 
+            break
+
+def txt_mk(file):
+    f = open(file, 'r')
+    f2 = open("output_mk.txt", 'w')
+    result = ""
+    while True:
+        line = f.readline()
+        result += line + mk(line)
+        if not line: 
+            break
+    print(result)
+    f2.write(result)
+    f.close()
+    f2.close()
+
 def csv_mk(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
@@ -298,14 +210,47 @@
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
     data.to_csv("output_mk.csv", encoding="utf-8-sig")
     print(data)
     f.close()
 
 # Montenegrin
+def me(text):
+    transliterated_text = ""
+    for letter in text:
+        try: 
+            if letter in montenegrin_list:
+                transliterated_text += montenegrin_list[letter]
+            else:
+                transliterated_text += letter
+        except KeyError:
+            pass
+    return transliterated_text
+
+def transliter_me():
+    while True:
+        input_text = input("Please enter Montenegrin text: ")
+        print(me(input_text))
+        if input_text == "": 
+            break
+
+def txt_me(file):
+    f = open(file, 'r')
+    f2 = open("output_me.txt", 'w')
+    result = ""
+    while True:
+        line = f.readline()
+        result += line + me(line)
+        if not line: 
+            break
+    print(result)
+    f2.write(result)
+    f.close()
+    f2.close()
+
 def csv_me(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
@@ -318,14 +263,47 @@
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
     data.to_csv("output_me.csv", encoding="utf-8-sig")
     print(data)
     f.close()
 
 # Serbian
+def sr(text):
+    transliterated_text = ""
+    for letter in text:
+        try: 
+            if letter in serbian_list:
+                transliterated_text += serbian_list[letter]
+            else:
+                transliterated_text += letter
+        except KeyError:
+            pass
+    return transliterated_text
+
+def transliter_sr():
+    while True:
+        input_text = input("Please enter Serbian text: ")
+        print(sr(input_text))
+        if input_text == "": 
+            break
+
+def txt_sr(file):
+    f = open(file, 'r')
+    f2 = open("output_sr.txt", 'w')
+    result = ""
+    while True:
+        line = f.readline()
+        result += line + sr(line)
+        if not line: 
+            break
+    print(result)
+    f2.write(result)
+    f.close()
+    f2.close()
+
 def csv_sr(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
@@ -335,8 +313,61 @@
         tr = sr(st)
         sentence_list.append(st)
         transliter_list.append(tr)
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
     data.to_csv("output_sr.csv", encoding="utf-8-sig")
     print(data)
+    f.close()
+
+# Tajiki
+def tj(text):
+    transliterated_text = ""
+    for letter in text:
+        try: 
+            if letter in tajiki_list:
+                transliterated_text += tajiki_list[letter]
+            else:
+                transliterated_text += letter
+        except KeyError:
+            pass
+    return transliterated_text
+
+def transliter_tj():
+    while True:
+        input_text = input("Please enter Tajiki text: ")
+        print(tj(input_text))
+        if input_text == "": 
+            break
+
+def txt_tj(file):
+    f = open(file, 'r')
+    f2 = open("output_tj.txt", 'w')
+    result = ""
+    while True:
+        line = f.readline()
+        result += line + tj(line)
+        if not line: 
+            break
+    print(result)
+    f2.write(result)
+    f.close()
+    f2.close()
+
+def csv_tj(file):
+    data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
+    f = open(file, 'r')
+    lines = f.readlines()
+    
+    index_list = list(range(len(lines)))
+    sentence_list = []
+    transliter_list = []
+    for sentence in lines:
+        st = sentence.strip()
+        tr = tj(st)
+        sentence_list.append(st)
+        transliter_list.append(tr)
+
+    data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
+    data.to_csv("output_tj.csv", encoding="utf-8-sig")
+    print(data)
     f.close()
```

### Comparing `TransLiter-0.3.2/TransLiter/transliter_jp.py` & `TransLiter-0.3.3/TransLiter/transliter_jp.py`

 * *Files identical despite different names*

### Comparing `TransLiter-0.3.2/TransLiter/transliter_ko.py` & `TransLiter-0.3.3/TransLiter/transliter_ko.py`

 * *Files identical despite different names*

### Comparing `TransLiter-0.3.2/TransLiter.egg-info/PKG-INFO` & `TransLiter-0.3.3/TransLiter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TransLiter
-Version: 0.3.2
+Version: 0.3.3
 Summary: TransLiter transliterates multilingual text into Latin script.
 Home-page: https://github.com/elibooklover/TransLiter
 Author: Hoyeol Kim
 Author-email: elibooklover@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -14,21 +14,21 @@
 
 <div align=right>
 
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Felibooklover%2FTransLiter&count_bg=%235F3DC8&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 
 </div>
 
-TransLiter transliterates multilingual text into Latin script. | by Hoyeol Kim
+#### TransLiter transliterates multilingual text into Latin script | by Hoyeol Kim
 
-Currently, TransLiter supports Korean, Japanese, and Cyrillic (Russian, Ukrainian, Bulgarian, Macedonian, Montenegrin, and Serbian). More languages will be added to TransLiter in the future.
+Currently, TransLiter supports Korean, Japanese, and Cyrillic (Russian, Ukrainian, Bulgarian, Macedonian, Montenegrin, Serbian, and Tajiki). More languages will be added to TransLiter in the future.
 
 There are several functions in TransLiter, such as `tl.ko`, `tl.transliter_ko`, `tl.txt_ko`, and `tl.csv_ko`, in addition to spacing functions (`tl.spacing` and `tl.spacing_file`). To transliaterate from a language other than Korean, simply replace the language code `ko` with your desired language code.
 
-Language codes are as follows: `ko` (Korean), `jp` (Japanese), `ru` (Russian), `ua` (Ukrainian), `bg` (Bulgarian), `mk` (Macedonian), `me` (Montenegrin), and `sr` (Serbian).
+Language codes are as follows: `ko` (Korean), `jp` (Japanese), `ru` (Russian), `ua` (Ukrainian), `bg` (Bulgarian), `mk` (Macedonian), `me` (Montenegrin),  `sr` (Serbian), and `tj` (Tajiki).
 
 ---
 
 ## Install
 
 ```
 $ pip install TransLiter
```

### Comparing `TransLiter-0.3.2/setup.py` & `TransLiter-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='TransLiter',
     python_requires='>=3.6',
-    version='0.3.2',
+    version='0.3.3',
     url='https://github.com/elibooklover/TransLiter',
     license='MIT',
     author='Hoyeol Kim',
     author_email='elibooklover@gmail.com',
     description='TransLiter transliterates multilingual text into Latin script.',
     packages=['TransLiter', ],
     long_description=long_description,
```

