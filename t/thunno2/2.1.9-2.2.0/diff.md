# Comparing `tmp/thunno2-2.1.9.tar.gz` & `tmp/thunno2-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.1.9.tar", last modified: Sat May  6 17:05:22 2023, max compression
+gzip compressed data, was "thunno2-2.2.0.tar", last modified: Sun May 14 14:37:49 2023, max compression
```

## Comparing `thunno2-2.1.9.tar` & `thunno2-2.2.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-06 17:05:22.361474 thunno2-2.1.9/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-06 17:05:22.361361 thunno2-2.1.9/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-06 17:05:22.361512 thunno2-2.1.9/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-04-16 17:25:02.000000 thunno2-2.1.9/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-06 17:05:22.360674 thunno2-2.1.9/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.1.9/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)      760 2023-04-30 09:02:54.000000 thunno2-2.1.9/thunno2/autoexplanation.py
--rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.1.9/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    52857 2023-05-04 17:16:06.000000 thunno2-2.1.9/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2950 2023-04-16 17:25:02.000000 thunno2-2.1.9/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.1.9/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     7174 2023-04-27 10:00:16.000000 thunno2-2.1.9/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    52884 2023-05-04 17:18:41.000000 thunno2-2.1.9/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    30385 2023-05-06 17:04:50.000000 thunno2-2.1.9/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    24717 2023-05-06 17:04:50.000000 thunno2-2.1.9/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1998 2023-05-01 08:52:47.000000 thunno2-2.1.9/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    76149 2023-05-04 17:17:09.000000 thunno2-2.1.9/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     4019 2023-04-29 16:25:56.000000 thunno2-2.1.9/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-05-06 17:04:40.000000 thunno2-2.1.9/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-06 17:05:22.361210 thunno2-2.1.9/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-06 17:05:22.000000 thunno2-2.1.9/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      441 2023-05-06 17:05:22.000000 thunno2-2.1.9/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-06 17:05:22.000000 thunno2-2.1.9/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-05-06 17:05:22.000000 thunno2-2.1.9/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-05-06 17:05:22.000000 thunno2-2.1.9/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-14 14:37:49.623927 thunno2-2.2.0/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-14 14:37:49.623806 thunno2-2.2.0/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-14 14:37:49.623962 thunno2-2.2.0/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-04-16 17:25:02.000000 thunno2-2.2.0/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-14 14:37:49.623095 thunno2-2.2.0/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.2.0/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3268 2023-05-14 14:05:01.000000 thunno2-2.2.0/thunno2/autoexplanation.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1491 2023-05-11 17:22:25.000000 thunno2-2.2.0/thunno2/canvas.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.2.0/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    55993 2023-05-13 16:16:20.000000 thunno2-2.2.0/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2950 2023-04-16 17:25:02.000000 thunno2-2.2.0/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.2.0/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     7174 2023-04-27 10:00:16.000000 thunno2-2.2.0/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    56512 2023-05-13 16:16:20.000000 thunno2-2.2.0/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    33521 2023-05-14 14:36:33.000000 thunno2-2.2.0/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    26490 2023-05-14 14:36:33.000000 thunno2-2.2.0/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1998 2023-05-01 08:52:47.000000 thunno2-2.2.0/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    81630 2023-05-13 16:16:20.000000 thunno2-2.2.0/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4526 2023-05-14 14:36:33.000000 thunno2-2.2.0/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-05-14 14:37:18.000000 thunno2-2.2.0/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-14 14:37:49.623637 thunno2-2.2.0/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-14 14:37:49.000000 thunno2-2.2.0/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      459 2023-05-14 14:37:49.000000 thunno2-2.2.0/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-14 14:37:49.000000 thunno2-2.2.0/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-05-14 14:37:49.000000 thunno2-2.2.0/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-05-14 14:37:49.000000 thunno2-2.2.0/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.1.9/PKG-INFO` & `thunno2-2.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.9
+Version: 2.2.0
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.9.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.0.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.1.9/setup.py` & `thunno2-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.9/thunno2/codepage.py` & `thunno2-2.2.0/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.9/thunno2/commands.py` & `thunno2-2.2.0/thunno2/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -182,14 +182,17 @@
 
     def __str__(self):
         return "Void"
 
     def __repr__(self):
         return "Void"
 
+    def __iter__(self):
+        yield from []
+
 
 Void = VoidType()
 
 
 def recursively_vectorise(lst, dct):
     for item in lst:
         if isinstance(item, list):
@@ -421,15 +424,17 @@
 
 # Which characters start digraphs?
 DIGRAPHS = "ØøÆµ"
 
 """DICTIONARY"""
 
 commands = {
-    "A": Overload(1, {Number: abs, str: isalpha}, 1, ("abs", "absolute", "isalpha")),
+    "A": Overload(
+        1, {Number: abs, str: isalpha}, 1, ("abs", "absolute", "isalpha", "is_alpha")
+    ),
     "B": Overload(
         2,
         {
             (int, int): ntb,
             (str, int): to_custom_base_string,
             (int, str): length_to_base,
             (str, str): length_custom_base_string,
@@ -441,26 +446,28 @@
     "C": Overload(
         1, {Number: chr2, str: ord2}, 1, ("chr", "character", "ord", "ordinal")
     ),
     "D": Overload(1, {Any: duplicate}, 0, ("dup", "duplicate")),
     "E": Overload(1, {Number: is_even, str: eval2}, 1, ("even", "is_even", "eval")),
     "F": Overload(1, {Number: factors, str: substrings}, 1, ("factors", "substrings")),
     "G": Overload(1, {Number: max2, Iterable: max3}, 0, ("max", "maximum", "greatest")),
-    "H": Overload(1, {(int, str): from_hex, float: pass_}, 1, ("from_hex",)),
+    "H": Overload(
+        1, {(int, str): from_hex, float: pass_}, 1, ("from_hex", "from_hexadecimal")
+    ),
     "I": Overload(
         2,
         {
             (Number[0], Number[0]): binary_range,
             (Number[0], Iterable[0]): slice1,
             (Iterable[0], Number[0]): slice2,
             (list, list): interleave_lst,
             (str, str): interleave_str,
         },
         0,
-        ("binary_range", "slice", "interleave"),
+        ("inclusive_range", "slice", "interleave"),
     ),
     "J": Overload(1, {Number: str, Iterable: empty_join}, 0, ("empty_join", "str")),
     # K is defined in the run function
     "L": Overload(
         1,
         {Number: lowered_range, str: str.lower},
         1,
@@ -617,15 +624,18 @@
     ),
     # x is defined in the run function
     # y is defined in the run function
     "z": Overload(
         1, {Number: num_uninterleave, Iterable: uninterleave}, 0, ("uninterleave",)
     ),
     "Ȧ": Overload(
-        1, {Number: bool2, str: isalphanum, list: any2}, 0, ("any", "isalphanum")
+        1,
+        {Number: bool2, str: isalphanum, list: any2},
+        0,
+        ("any", "is_alphanum", "is_alpha_num"),
     ),
     "Ḃ": Overload(1, {(int, str): from_binary, float: pass_}, 1, ("from_binary",)),
     "Ċ": Overload(
         1,
         {Number: codepage_chr, str: codepage_ord},
         1,
         ("codepage_chr", "codepage_character", "codepage_ord", "codepage_ordinal"),
@@ -1218,16 +1228,16 @@
         ("dyadic_maximum",),
     ),
     "½": Overload(1, {Number: halve, str: chunk_halve}, 1, ("halve",)),
     "Ƈ": Overload(
         2,
         {
             (Number[0], Number[0]): nPr,
-            (Any, str): string_contains,
             (Any, list): list_contains,
+            (Any, str): string_contains,
         },
         0,
         ("npr", "contains"),
     ),
     "Ɗ": Overload(
         2,
         {
@@ -1252,15 +1262,15 @@
     "Ɱ": Overload(
         1, {Number: num_palindromise, Iterable: palindromise}, 0, ("palindromise",)
     ),
     "Ɲ": Overload(
         1,
         {Number: integer_partitions, Iterable: newline_join},
         0,
-        ("integer_partitions", "newline_join"),
+        ("integer_partitions", "newline_join", "join_by_newlines"),
     ),
     "Ƥ": Overload(
         2,
         {
             (Any[0], list): prepend,
             (list, Any[0]): swapped_prepend,
             (Any[0], Any[0]): prepend2,
@@ -1279,15 +1289,17 @@
         0,
         ("transpose_with_filler",),
     ),
     "ɓ": Overload(1, {Any: boolify}, 1, ("boolify",)),
     "ƈ": Overload(1, {Number: num_counts, Iterable: counts}, 0, ("counts",)),
     "ɗ": Overload(1, {Number: parity, str: second_half}, 1, ("parity", "second_half")),
     "ƒ": Overload(1, {Number: num_prefixes, Iterable: prefixes}, 0, ("prefixes",)),
-    "ɠ": Overload(0, {Any: (lambda: 256)}, 0, ("two_fifty_six",)),
+    "ɠ": Overload(
+        0, {Any: (lambda: 256)}, 0, ("two_fifty_six", "two_hundred_fifty_six")
+    ),
     "ɦ": Overload(0, {Any: (lambda: 100)}, 0, ("hundred", "one_hundred")),
     "ƙ": Overload(
         1,
         {Number: increment_twice, Iterable: grade_up},
         0,
         ("grade_up", "increment_twice"),
     ),
@@ -1331,16 +1343,18 @@
         1,
         {Number: square_root, str: every_second_item},
         1,
         ("square_root", "every_second_item"),
     ),
     "²": Overload(1, {Number: square, str: chunk_wrap_2}, 1, ("square",)),
     "³": Overload(1, {Number: cube, str: chunk_wrap_3}, 1, ("cube",)),
-    "⁴": Overload(1, {Number: fourth, str: chunk_wrap_4}, 1, ("fourth",)),
-    "⁵": Overload(1, {Number: fifth, str: chunk_wrap_5}, 1, ("fifth",)),
+    "⁴": Overload(
+        1, {Number: fourth, str: chunk_wrap_4}, 1, ("fourth", "fourth_power")
+    ),
+    "⁵": Overload(1, {Number: fifth, str: chunk_wrap_5}, 1, ("fifth", "fifth_power")),
     "ạ": Overload(1, {Number: num_all_equal, Iterable: all_equal}, 0, ("all_equal",)),
     "ḅ": Overload(1, {Any: equals_one}, 1, ("equals_one",)),
     "ḍ": Overload(
         2,
         {
             (Number[0], Number[0]): range_ssd1,
             (Number[0], Iterable[0]): range_ssd2,
@@ -1458,22 +1472,77 @@
         {Any: brackets_are_balanced},
         1,
         ("balanced_brackets", "brackets_are_balanced"),
     ),
     "D": Overload(
         1, {Any: optimal_dictionary_compression}, 1, ("optimal_dictionary_compression",)
     ),
+    "v": Overload(
+        2,
+        {
+            (list, Any[0]): canvas_draw,
+            (Number[0], str): digits_canvas_draw,
+            (str, list): swapped_canvas_draw,
+            (str, Number[0]): swapped_digits_canvas_draw,
+            (Any[0], Any[0]): pass_,
+        },
+        0,
+        ("canvas", "draw", "canvas_draw"),
+    ),
+    "V": Overload(
+        2,
+        {
+            (list, Any[0]): blank_canvas_draw,
+            (Number[0], str): blank_digits_canvas_draw,
+            (str, list): blank_swapped_canvas_draw,
+            (str, Number[0]): blank_swapped_digits_canvas_draw,
+            (Any[0], Any[0]): pass_,
+        },
+        0,
+        ("blank_canvas", "blank_draw", "blank_canvas_draw"),
+    ),
+    "^": Overload(0, {Any: clear_canvas}, 0, ("clear_canvas",)),
+    "<": Overload(2, {(Any[0], Any[0]): str_starts_with}, 2, ("starts_with",)),
+    ">": Overload(2, {(Any[0], Any[0]): str_ends_with}, 2, ("starts_with",)),
 }
 
 list_digraphs = {
     "C": Overload(
         1, {((int, float, str),): pass_, list: centre_list}, 0, ("center", "centre")
     ),
     "D": Overload(1, {Any: depth}, 0, ("depth",)),
+    "E": Overload(
+        2,
+        {
+            (Number[0], Iterable[0]): extend_truncate,
+            (Iterable[0], Number[0]): swapped_extend_truncate,
+            (Iterable[0], Iterable[0]): length_extend_truncate,
+            (Number[0], Number[0]): num_extend_truncate,
+        },
+        0,
+        (
+            "extend",
+            "truncate",
+            "extend_truncate",
+            "extend_to_length",
+            "truncate_to_length",
+        ),
+    ),
     "G": Overload(1, {((int, float, str),): pass_, list: longest}, 0, ("longest",)),
+    "I": Overload(
+        2,
+        {
+            ((int, float, str), list): multidimensional_index,
+            (list, (int, float, str)): swapped_multidimensional_index,
+            (list, list): vectorised_multidimensional_index,
+            (Any[0], Any[0]): pass_,
+        },
+        0,
+        ("multidimensional_index",),
+    ),
     "M": Overload(1, {((int, float, str),): pass_, list: shortest}, 0, ("shortest",)),
     ".": Overload(
         2, {(list, list): dot_product, (Any[0], Any[0]): pass_}, 0, ("dot_product",)
     ),
     "\\": Overload(
         1, {((int, float, str),): pass_, list: main_diagonal}, 0, ("main_diagonal",)
     ),
@@ -1493,14 +1562,15 @@
 
 random_digraphs_1 = {
     "C": Overload(1, {Any: cosine}, 1, ("cosine", "cos")),
     "D": Overload(1, {Any: degrees}, 1, ("degrees",)),
     "E": Overload(1, {Any: exponent}, 1, ("exponent",)),
     "F": Overload(1, {Any: nth_fibonacci_number}, 1, ("nth_fibonacci_number",)),
     "H": Overload(2, {(Any[0], Any[0]): hypotenuse}, 2, ("hypot", "hypotenuse")),
+    "I": Overload(1, {Any: insignificant}, 1, ("insignificant",)),
     "P": Overload(1, {Any: nth_prime}, 1, ("nth_prime",)),
     "R": Overload(1, {Any: radians}, 1, ("radians",)),
     "S": Overload(1, {Any: sine}, 1, ("sine", "sin")),
     "T": Overload(1, {Any: tangent}, 1, ("tangent", "tan")),
     "c": Overload(1, {Any: arc_cosine}, 1, ("arc_cosine", "arccos")),
     "s": Overload(1, {Any: arc_sine}, 1, ("arc_sine", "arcsin")),
     "t": Overload(1, {Any: arc_tangent}, 1, ("arc_tangent", "arctan")),
@@ -1511,20 +1581,63 @@
 }
 
 random_digraphs_2 = {
     "R": Overload(
         1, {Number: to_roman_numerals, str: from_roman_numerals}, 1, ("roman_numerals",)
     ),
     "T": Overload(1, {Any: type_of}, 0, ("type",)),
+    "U": Overload(
+        1,
+        {
+            Number: num_connected_uniquify,
+            str: str_connected_uniquify,
+            list: connected_uniquify,
+        },
+        0,
+        ("connected_uniquify",),
+    ),
     "r": Overload(
         1,
         {Number: range_shuffle, str: str_shuffle, list: shuffle},
         0,
         ("random_shuffle",),
     ),
+    "v": Overload(
+        2,
+        {
+            (list, list): vectorised_trim,
+            (Any[0], list): trim,
+            (list, Any[0]): swapped_trim,
+            (Any[0], (int, float, str)): str_trim,
+        },
+        0,
+        ("trim",),
+    ),
+    "<": Overload(
+        2,
+        {
+            (list, list): vectorised_left_trim,
+            (Any[0], list): left_trim,
+            (list, Any[0]): swapped_left_trim,
+            (Any[0], (int, float, str)): str_left_trim,
+        },
+        0,
+        ("left_trim",),
+    ),
+    ">": Overload(
+        2,
+        {
+            (list, list): vectorised_right_trim,
+            (Any[0], list): right_trim,
+            (list, Any[0]): swapped_right_trim,
+            (Any[0], (int, float, str)): str_right_trim,
+        },
+        0,
+        ("right_trim",),
+    ),
     "&": Overload(
         2,
         {(Any[0], Any[0]): logical_and},
         0,
         ("non_vectorised_and", "non_vectorised_logical_and"),
     ),
     "|": Overload(
```

### Comparing `thunno2-2.1.9/thunno2/constants.py` & `thunno2-2.2.0/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.9/thunno2/dictionary.py` & `thunno2-2.2.0/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.9/thunno2/flags.py` & `thunno2-2.2.0/thunno2/flags.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.9/thunno2/helpers.py` & `thunno2-2.2.0/thunno2/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 """An unordered, chaotic mess of helper functions"""
 
+
+import copy
+import itertools
+import math
+import random
+import re
+import string
+
+from thunno2 import codepage
+from thunno2 import canvas
+
+
 """Creative Commons Legal Code
 
 CC0 1.0 Universal
 
     CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
     LEGAL SERVICES. DISTRIBUTION OF THIS DOCUMENT DOES NOT CREATE AN
     ATTORNEY-CLIENT RELATIONSHIP. CREATIVE COMMONS PROVIDES THIS
@@ -119,23 +131,14 @@
     consents, permissions or other rights required for any use of the
     Work.
  d. Affirmer understands and acknowledges that Creative Commons is not a
     party to this document and has no duty or obligation with respect to
     this CC0 or use of the Work.
 """
 
-import copy
-import itertools
-import math
-import random
-import re
-import string
-
-from thunno2 import codepage
-
 
 def convert_all_to_string(func):
     def wrapper(*args, fn=func):
         return fn(*map(str, args))
 
     return wrapper
 
@@ -2845,7 +2848,199 @@
         return 3
     return -1
 
 
 @try_float_conversion
 def hypotenuse(a, b):
     return math.sqrt(a**2 + b**2)
+
+
+def extend_truncate(x, y):
+    x = abs(int(x))
+    if x == 0:
+        return y * 0
+    if not y:
+        return y
+    i = 0
+    l = len(y)
+    while x > len(y):
+        y += y[(i % l) : (i % l) + 1]
+        i += 1
+    while x < len(y):
+        y = y[:-1]
+    return y
+
+
+def swapped_extend_truncate(y, x):
+    return extend_truncate(x, y)
+
+
+def length_extend_truncate(x, y):
+    return extend_truncate(len(x), y)
+
+
+def num_extend_truncate(x, y):
+    r = extend_truncate(x, str(y))
+    try:
+        return eval(r)
+    except:
+        return r
+
+
+@try_float_conversion
+def insignificant(x):
+    return int(abs(x) <= 1)
+
+
+def left_trim(x, l):
+    r = l * 0
+    for i, j in enumerate(l):
+        if j != x:
+            r = l[i:]
+            break
+    return r
+
+
+def right_trim(x, l):
+    return left_trim(x, l[::-1])[::-1]
+
+
+def trim(x, l):
+    return right_trim(x, left_trim(x, l))
+
+
+def swapped_left_trim(l, x):
+    return left_trim(x, l)
+
+
+def swapped_right_trim(l, x):
+    return right_trim(x, l)
+
+
+def swapped_trim(l, x):
+    return trim(x, l)
+
+
+def str_left_trim(x, y):
+    return str(y).lstrip(str(x))
+
+
+def str_right_trim(x, y):
+    return str(y).rstrip(str(x))
+
+
+def str_trim(x, y):
+    return str(y).strip(str(x))
+
+
+def vectorised_left_trim(x, l):
+    r = l * 0
+    for i, j in enumerate(l):
+        if j not in x:
+            r = l[i:]
+            break
+    return r
+
+
+def vectorised_right_trim(x, l):
+    return vectorised_left_trim(x, l[::-1])[::-1]
+
+
+def vectorised_trim(x, l):
+    return vectorised_right_trim(x, vectorised_left_trim(x, l))
+
+
+def connected_uniquify(l):
+    return [x[0] for x in group_consecutive(l)]
+
+
+def str_connected_uniquify(s):
+    return "".join(connected_uniquify(s))
+
+
+def num_connected_uniquify(n):
+    return eval(str_connected_uniquify(str(n)))
+
+
+def str_starts_with(x, y):
+    return int(str(y).startswith(str(x)))
+
+
+def str_ends_with(x, y):
+    return int(str(y).endswith(str(x)))
+
+
+def canvas_draw(dirs, text):
+    l = []
+    for i in dirs:
+        try:
+            j = int(i)
+            if 0 <= j <= 7:
+                l.append(j)
+        except:
+            pass
+    canvas.canvas.draw(text, length_extend_truncate(text, l or [2]))
+    return str(canvas.canvas)
+
+
+def digits_canvas_draw(n, s):
+    return canvas_draw(digits(n), s)
+
+
+def swapped_canvas_draw(text, dirs):
+    return canvas_draw(dirs, text)
+
+
+def swapped_digits_canvas_draw(s, n):
+    return digits_canvas_draw(n, s)
+
+
+def blank_canvas_draw(dirs, text):
+    l = []
+    for i in dirs:
+        try:
+            j = int(i)
+            if 0 <= j <= 7:
+                l.append(j)
+        except:
+            pass
+    temp_canvas = canvas.Canvas()
+    temp_canvas.draw(text, length_extend_truncate(text, l or [2]))
+    return str(temp_canvas)
+
+
+def blank_digits_canvas_draw(n, s):
+    return blank_canvas_draw(digits(n), s)
+
+
+def blank_swapped_canvas_draw(text, dirs):
+    return blank_canvas_draw(dirs, text)
+
+
+def blank_swapped_digits_canvas_draw(s, n):
+    return blank_digits_canvas_draw(n, s)
+
+
+def clear_canvas():
+    canvas.canvas.clear()
+    return ()
+
+
+def multidimensional_index(x, l):
+    for i, j in enumerate(l):
+        if j == x:
+            return [i]
+        elif isinstance(j, list):
+            r = multidimensional_index(x, j)
+            if r:
+                return [i] + r
+    return []
+
+
+def swapped_multidimensional_index(l, x):
+    return multidimensional_index(x, l)
+
+
+def vectorised_multidimensional_index(x, l):
+    if not isinstance(x, list):
+        return multidimensional_index(x, l)
+    return [*map(lambda i, y=l: vectorised_multidimensional_index(i, y), x)]
```

### Comparing `thunno2-2.1.9/thunno2/interpreter.py` & `thunno2-2.2.0/thunno2/interpreter.py`

 * *Files 9% similar despite different names*

```diff
@@ -380,24 +380,28 @@
             vars_dict["y"] = a
         elif desc == "set x without popping":
             a = (ctx.stack.copy() + ctx.other_il + [0])[0]
             vars_dict["x"] = a
         elif desc == "set y without popping":
             a = (ctx.stack.copy() + ctx.other_il + [0])[0]
             vars_dict["y"] = a
-        elif desc == "increment x":
-            try:
-                vars_dict["x"] = vars_dict.get("x", 1) + 1
-            except:
-                pass
-        elif desc == "increment y":
-            try:
-                vars_dict["y"] = vars_dict.get("y", 2) + 1
-            except:
-                pass
+        elif desc == "apply to x":
+            old_stack = copy.deepcopy(ctx.stack)
+            ctx.stack.push(vars_dict.get("x", 1))
+            for k in info():
+                ctx.stack.push(k)
+            vars_dict["x"] = next(ctx.stack.rmv(1))
+            ctx.stack = copy.deepcopy(old_stack)
+        elif desc == "apply to y":
+            old_stack = copy.deepcopy(ctx.stack)
+            ctx.stack.push(vars_dict.get("y", 2))
+            for k in info():
+                ctx.stack.push(k)
+            vars_dict["y"] = next(ctx.stack.rmv(1))
+            ctx.stack = copy.deepcopy(old_stack)
         elif desc == "get global array":
             ctx.stack.push(vars_dict.get("ga", []))
         elif desc == "add to global array":
             a = next(ctx.stack.rmv(1))
             ga = vars_dict.get("ga", [])
             if not isinstance(ga, list):
                 vars_dict["ga"] = [ga, a]
@@ -709,14 +713,90 @@
                 for j in x:
                     ctx.stack.push(j)
                 run(info, n=([0] + x)[-1], iteration_index=k)
                 y = next(ctx.stack.rmv(1))
                 print(y)
                 x.append(y)
                 k += 1
+        elif desc == "apply to every nth item":
+            a = next(ctx.stack.rmv(1))
+            try:
+                a = int(a)
+            except:
+                try:
+                    a = len(a)
+                except:
+                    a = 2
+            b = listify(next(ctx.stack.rmv(1)))
+            old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
+            r = []
+            for i, j in enumerate(b):
+                if i % a == 0:
+                    ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
+                    ctx.stack.push(j)
+                    for k in info():
+                        r.append(k)
+                else:
+                    r.append(j)
+            ctx.stack.push(r)
+        elif desc == "rotate stack left":
+            ctx.stack = Stack(rotate_left_once(ctx.stack))
+        elif desc == "rotate stack right":
+            ctx.stack = Stack(rotate_right_once(ctx.stack))
+        elif desc == "reverse stack":
+            ctx.stack = Stack(ctx.stack[::-1])
+        elif desc == "adjacent group by":
+            a = next(ctx.stack.rmv(1))
+            x = listify(a)
+            r = []
+            old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
+            for i, j in enumerate(x):
+                ctx.stack = Stack([j] + copy.deepcopy(old_stack))
+                run(info, n=j, iteration_index=i)
+                z = next(ctx.stack.rmv(1))
+                r.append((j, z))
+            try:
+                d = []
+                last = None
+                for val, key in r:
+                    if key == last:
+                        d[-1].append(val)
+                    else:
+                        d.append([val])
+                    last = key
+                ctx.stack.push(d)
+            except:
+                ctx.stack.push(x)
+        elif desc == "single function adjacent group by":
+            a = next(ctx.stack.rmv(1))
+            func = info
+            if func != Void:
+                x = listify(a)
+                group_by = []
+                old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
+                for i in x:
+                    ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
+                    ctx.stack.push(i)
+                    f = func()
+                    if not f:
+                        group_by.append((i, i))
+                    else:
+                        group_by.append((i, f[-1]))
+                try:
+                    d = []
+                    last = None
+                    for val, key in group_by:
+                        if key == last:
+                            d[-1].append(val)
+                        else:
+                            d.append([val])
+                        last = key
+                    ctx.stack.push(d)
+                except:
+                    ctx.stack.push(x)
         else:
             if ctx.warnings:
                 print("TRACEBACK: [UNRECOGNISED TOKEN]", file=sys.stderr)
                 print(f"Got {chars!r} (tokenised to {desc!r})")
     return 0
```

### Comparing `thunno2-2.1.9/thunno2/lexer.py` & `thunno2-2.2.0/thunno2/lexer.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,37 +150,63 @@
                 elif y == "µƲ":
                     index += 1
                     cmd = code[index]
                     if cmd in DIGRAPHS:
                         index += 1
                         cmd += code[index]
                     func = get_a_function(cmd)
-                    ret.append((char + cmd, "single function reduce by", func))
+                    ret.append((y + cmd, "single function reduce by", func))
                 elif y == "µɼ":
                     index += 1
                     cmd = code[index]
                     if cmd in DIGRAPHS:
                         index += 1
                         cmd += code[index]
                     func = get_a_function(cmd)
-                    ret.append((char + cmd, "single function right reduce by", func))
+                    ret.append((y + cmd, "single function right reduce by", func))
                 elif y == "µƇ":
                     index += 1
                     cmd = code[index]
                     if cmd in DIGRAPHS:
                         index += 1
                         cmd += code[index]
                     func = get_a_function(cmd)
                     ret.append(
-                        (char + cmd, "single function right cumulative reduce by", func)
+                        (y + cmd, "single function right cumulative reduce by", func)
                     )
                 elif y == "µʋ":
                     i, r = tokenise(code[index + 1 :], expected_end=";")
                     index += i
                     ret.append((y, "right reduce by", r))
+                elif y == "µ€":
+                    index += 1
+                    cmd = code[index]
+                    if cmd in DIGRAPHS:
+                        index += 1
+                        cmd += code[index]
+                    func = get_a_function(cmd)
+                    ret.append((y + cmd, "apply to every nth item", func))
+                elif y == "µ«":
+                    ret.append((y, "rotate stack left", 0))
+                elif y == "µ»":
+                    ret.append((y, "rotate stack right", 0))
+                elif y == "µ!":
+                    ret.append((y, "reverse stack", 0))
+                elif y == "µÑ":
+                    i, r = tokenise(code[index + 1 :], expected_end=";")
+                    index += i
+                    ret.append((y, "adjacent group by", r))
+                elif y == "µñ":
+                    index += 1
+                    cmd = code[index]
+                    if cmd in DIGRAPHS:
+                        index += 1
+                        cmd += code[index]
+                    func = get_a_function(cmd)
+                    ret.append((y + cmd, "single function adjacent group by", func))
                 else:
                     ret.append((y, "digraph", get_a_function(y)))
             except:
                 pass
         elif char in "0123456789.":
             s = char
             index += 1
@@ -460,17 +486,29 @@
         elif char == "Y":
             ret.append((char, "set y", 0))
         elif char == "Ẋ":
             ret.append((char, "set x without popping", 0))
         elif char == "Ẏ":
             ret.append((char, "set y without popping", 0))
         elif char == "ẋ":
-            ret.append((char, "increment x", 0))
+            index += 1
+            cmd = code[index]
+            if cmd in DIGRAPHS:
+                index += 1
+                cmd += code[index]
+            func = get_a_function(cmd)
+            ret.append((char, "apply to x", func))
         elif char == "ẏ":
-            ret.append((char, "increment y", 0))
+            index += 1
+            cmd = code[index]
+            if cmd in DIGRAPHS:
+                index += 1
+                cmd += code[index]
+            func = get_a_function(cmd)
+            ret.append((char, "apply to y", func))
         elif char == "Ȥ":
             ret.append((char, "get global array", 0))
         elif char == "ȥ":
             ret.append((char, "add to global array", 0))
         elif char == "K":
             ret.append((char, "stack", 0))
         elif char == "k":
@@ -618,9 +656,15 @@
                     cmd2 += code[index]
                 func2 = get_a_function(cmd2)
             except:
                 func2, cmd2 = Void, ""
             ret.append((char + cmd1 + cmd2, "two function map", (func1, func2)))
         elif char in expected_end:
             return index, ret
+        elif char == ":":
+            ret.append((":", "command", commands["="]))
+            return index + 1, ret
+        elif char == "}":
+            ret.append(("}", "command", commands["¬"]))
+            return index + 1, ret
         index += 1
     return index + 1, ret
```

### Comparing `thunno2-2.1.9/thunno2/run.py` & `thunno2-2.2.0/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.9/thunno2/tests.py` & `thunno2-2.2.0/thunno2/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,31 +124,46 @@
     party to this document and has no duty or obligation with respect to
     this CC0 or use of the Work.
 """
 
 tests_counter = 0
 tested_commands = []
 
-UNTESTABLE = ["ɼ", "µr", "ÆC", "ÆD", "ÆE", "ÆR", "ÆS", "ÆT", "Æc", "Æs", "Æt"]
+UNTESTABLE = [
+    "ɼ",
+    "øv",
+    "øV",
+    "ø^",
+    "µr",
+    "ÆC",
+    "ÆD",
+    "ÆE",
+    "ÆR",
+    "ÆS",
+    "ÆT",
+    "Æc",
+    "Æs",
+    "Æt",
+]
 
 
 def call(cmd, *stk):
     ctx.stack = Stack(stk)
     ctx.warnings = True
     tested_commands.append(cmd)
     return get_a_function(cmd)()
 
 
 def assert_eq(a, *b):
     global tests_counter
     tests_counter += 1
-    #               Because 1 == True
-    #               but '1' != 'True'
-    #            (we don't want booleans)
-    #                      ↓↓
+    #                  Because 1 == True
+    #                  but '1' != 'True'
+    #               (we don't want booleans)
+    #                         ↓↓
     assert a == b and repr(a) == repr(b), f"\n\nTest {tests_counter}\n{a!r} != {b!r}"
 
 
 # A
 
 assert_eq(call("A", -1), 1)
 assert_eq(call("A", 1.23), 1.23)
@@ -2720,14 +2735,32 @@
 # øD
 
 assert_eq(call("øD", "Hello, World!"), "Ƙ¥, «ʋ!")
 assert_eq(call("øD", "thunnobest"), "thunnoÇ&")
 assert_eq(call("øD", "withree"), "wiċŀ")
 assert_eq(call("øD", 123456), "123456")
 
+# ø<
+
+assert_eq(call("ø<", 123, 123456), 1)
+assert_eq(call("ø<", -1, -1.23), 1)
+assert_eq(call("ø<", 1, [123, -1, 456, 1, 1.23]), [1, 0, 0, 1, 1])
+
+assert_eq(call("ø<", "abc", "abcdef"), 1)
+assert_eq(call("ø<", "xyz", "abcdef"), 0)
+
+# ø>
+
+assert_eq(call("ø>", 456, 123456), 1)
+assert_eq(call("ø>", -1, -1.23), 0)
+assert_eq(call("ø>", 1, [321, -1, 456, 1, 1.23]), [1, 1, 0, 1, 0])
+
+assert_eq(call("ø>", "def", "abcdef"), 1)
+assert_eq(call("ø>", "xyz", "abcdef"), 0)
+
 # ØC
 
 assert_eq(call("ØC", 123), 123)
 assert_eq(call("ØC", "abc"), "abc")
 
 assert_eq(call("ØC", [123, 4567, 8, 90]), "123 \n4567\n 8  \n 90 ")
 assert_eq(
@@ -2744,23 +2777,55 @@
 assert_eq(call("ØD", [1, 2, 3]), 1)
 assert_eq(call("ØD", [["abc", "def", "ghi"], 123, 456, 789]), 2)
 assert_eq(call("ØD", [1, [2, [3, [4, [5, [6, [7, [8, [9, [10]]]]]]]]]]), 10)
 
 assert_eq(call("ØD", []), 1)
 assert_eq(call("ØD", [[[[[[[[[[]]]]]]]]]]), 10)
 
+# ØE
+
+assert_eq(call("ØE", 6, 123), 123123)
+assert_eq(call("ØE", 10, 4.56), "4.564.564.")
+
+assert_eq(call("ØE", 15, "abcd"), "abcdabcdabcdabc")
+assert_eq(call("ØE", "thunno", -5.67), "thunn")
+assert_eq(call("ØE", 3, ""), "")
+assert_eq(call("ØE", "abc", 0), "")
+
+assert_eq(
+    call("ØE", [123, 456, 789], 10), [123, 456, 789, 123, 456, 789, 123, 456, 789, 123]
+)
+assert_eq(call("ØE", -3, ["abc", 123, "def", 456, "ghi", 789]), ["abc", 123, "def"])
+assert_eq(call("ØE", 3, []), [])
+assert_eq(call("ØE", [123, 456, 789], 0), [])
+
 # ØG
 
 assert_eq(call("ØG", [123, 4567, 89]), 4567)
 assert_eq(call("ØG", ["abcd", "ef", "ghi"]), "abcd")
 assert_eq(call("ØG", []), [])
 
 assert_eq(call("ØG", 123), 123)
 assert_eq(call("ØG", "abc"), "abc")
 
+# ØI
+
+assert_eq(call("ØI", 5, [[[1, 2], [3, 4]], [[5, 6], [7, 8]]]), [1, 0, 0])
+assert_eq(call("ØI", [[[1, 2], [3, 4]], [[5, 6], [7, 8]]], 8), [1, 1, 1])
+assert_eq(
+    call("ØI", [2, 3, 5, 7], [[[1, 2], [3, 4]], [[5, 6], [7, 8]]]),
+    [[0, 0, 1], [0, 1, 0], [1, 0, 0], [1, 1, 0]],
+)
+
+assert_eq(call("ØI", "abc", [[[1, 2], [3, 4]], [[5, 6], [7, 8]]]), [])
+assert_eq(call("ØI", [[[1, 2], [3, 4]], [[5, 6], [7, 8]]], 9), [])
+
+assert_eq(call("ØI", 123, 456), 456, 123)
+assert_eq(call("ØI", "abc", "def"), "def", "abc")
+
 # ØM
 
 assert_eq(call("ØM", [123, 4567, 89]), 89)
 assert_eq(call("ØM", ["abcd", "ef", "ghi"]), "ef")
 assert_eq(call("ØM", []), [])
 
 assert_eq(call("ØM", 123), 123)
@@ -2855,14 +2920,26 @@
 
 assert_eq(call("ÆH", 3, 4), 5.0)
 assert_eq(call("ÆH", 12, 5), 13.0)
 assert_eq(call("ÆH", 7, 24), 25.0)
 
 assert_eq(call("ÆH", 123, "abc"), [123, "abc"])
 
+# ÆI
+
+assert_eq(call("ÆI", 0), 1)
+assert_eq(call("ÆI", 123), 0)
+assert_eq(call("ÆI", -1.23), 0)
+
+assert_eq(
+    call("ÆI", [-2, -1.5, -1, -0.5, 0, 0.5, 1, 1.5, 2]), [0, 0, 1, 1, 1, 1, 1, 0, 0]
+)
+
+assert_eq(call("ÆI", "abc"), ["abc"])
+
 # ÆP
 
 assert_eq(call("ÆP", 0), 2)
 assert_eq(call("ÆP", 5), 13)
 assert_eq(call("ÆP", 1.23), 3)
 assert_eq(call("ÆP", [10, 11, 12, 13, 14]), [31, 37, 41, 43, 47])
 
@@ -2979,14 +3056,165 @@
 
 assert_eq(call("µT", "abc"), 2)
 assert_eq(call("µT", ""), 2)
 
 assert_eq(call("µT", [123, 456, 789]), 3)
 assert_eq(call("µT", []), 3)
 
+# µU
+
+assert_eq(call("µU", 122333444455555), 12345)
+assert_eq(call("µU", 123112233111222333), 123123123)
+assert_eq(call("µU", 123), 123)
+assert_eq(call("µU", 111), 1)
+
+assert_eq(call("µU", "abbcccddddeeeee"), "abcde")
+assert_eq(call("µU", "abcaabbccaaabbbccc"), "abcabcabc")
+assert_eq(call("µU", "xyz"), "xyz")
+assert_eq(call("µU", "aaa"), "a")
+assert_eq(call("µU", ""), "")
+
+assert_eq(call("µU", [123, 456, 456, 789, 789, 789]), [123, 456, 789])
+assert_eq(
+    call("µU", [123, 456, 789, 123, 123, 456, 456, 789, 789]),
+    [123, 456, 789, 123, 456, 789],
+)
+assert_eq(call("µU", ["abc", "def"]), ["abc", "def"])
+assert_eq(call("µU", ["abc", "abc", "abc"]), ["abc"])
+assert_eq(call("µU", []), [])
+
+# µv
+
+assert_eq(call("µv", 1, 111222333111), "222333")
+assert_eq(call("µv", 123, 111222333111), "")
+
+assert_eq(call("µv", "a", "aaabbbcccaaa"), "bbbccc")
+assert_eq(call("µv", "abc", "aaabbbcccaaa"), "")
+assert_eq(call("µv", "xyz", "aaabbbcccaaa"), "aaabbbcccaaa")
+
+assert_eq(
+    call("µv", 123, [123, 123, 123, 456, 456, 456, 789, 789, 789, 123, 123, 123]),
+    [456, 456, 456, 789, 789, 789],
+)
+assert_eq(
+    call(
+        "µv",
+        ["abc", "def", "ghi"],
+        [
+            "abc",
+            "abc",
+            "abc",
+            "def",
+            "def",
+            "def",
+            "ghi",
+            "ghi",
+            "ghi",
+            "abc",
+            "abc",
+            "abc",
+        ],
+    ),
+    [],
+)
+assert_eq(
+    call(
+        "µv",
+        ["abc", "def", "ghi"],
+        [123, 123, 123, 456, 456, 456, 789, 789, 789, 123, 123, 123],
+    ),
+    [123, 123, 123, 456, 456, 456, 789, 789, 789, 123, 123, 123],
+)
+
+# µ<
+
+assert_eq(call("µ<", 1, 111222333111), "222333111")
+assert_eq(call("µ<", 123, 111222333111), "")
+
+assert_eq(call("µ<", "a", "aaabbbcccaaa"), "bbbcccaaa")
+assert_eq(call("µ<", "abc", "aaabbbcccaaa"), "")
+assert_eq(call("µ<", "xyz", "aaabbbcccaaa"), "aaabbbcccaaa")
+
+assert_eq(
+    call("µ<", 123, [123, 123, 123, 456, 456, 456, 789, 789, 789, 123, 123, 123]),
+    [456, 456, 456, 789, 789, 789, 123, 123, 123],
+)
+assert_eq(
+    call(
+        "µ<",
+        ["abc", "def", "ghi"],
+        [
+            "abc",
+            "abc",
+            "abc",
+            "def",
+            "def",
+            "def",
+            "ghi",
+            "ghi",
+            "ghi",
+            "abc",
+            "abc",
+            "abc",
+        ],
+    ),
+    [],
+)
+assert_eq(
+    call(
+        "µ<",
+        ["abc", "def", "ghi"],
+        [123, 123, 123, 456, 456, 456, 789, 789, 789, 123, 123, 123],
+    ),
+    [123, 123, 123, 456, 456, 456, 789, 789, 789, 123, 123, 123],
+)
+
+# µ>
+
+assert_eq(call("µ>", 1, 111222333111), "111222333")
+assert_eq(call("µ>", 123, 111222333111), "")
+
+assert_eq(call("µ>", "a", "aaabbbcccaaa"), "aaabbbccc")
+assert_eq(call("µ>", "abc", "aaabbbcccaaa"), "")
+assert_eq(call("µ>", "xyz", "aaabbbcccaaa"), "aaabbbcccaaa")
+
+assert_eq(
+    call("µ>", 123, [123, 123, 123, 456, 456, 456, 789, 789, 789, 123, 123, 123]),
+    [123, 123, 123, 456, 456, 456, 789, 789, 789],
+)
+assert_eq(
+    call(
+        "µ>",
+        ["abc", "def", "ghi"],
+        [
+            "abc",
+            "abc",
+            "abc",
+            "def",
+            "def",
+            "def",
+            "ghi",
+            "ghi",
+            "ghi",
+            "abc",
+            "abc",
+            "abc",
+        ],
+    ),
+    [],
+)
+assert_eq(
+    call(
+        "µ>",
+        ["abc", "def", "ghi"],
+        [123, 123, 123, 456, 456, 456, 789, 789, 789, 123, 123, 123],
+    ),
+    [123, 123, 123, 456, 456, 456, 789, 789, 789, 123, 123, 123],
+)
+
 # µ&
 
 assert_eq(call("µ&", 123, 456), 123)
 assert_eq(call("µ&", 123, 0), 0)
 
 assert_eq(call("µ&", -123, "abc"), -123)
 assert_eq(call("µ&", "xyz", 0), 0)
```

### Comparing `thunno2-2.1.9/thunno2/tokens.py` & `thunno2-2.2.0/thunno2/tokens.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,16 +56,16 @@
     "“": ("lowercase_string_compression",),
     "”": ("title_case_string_compression",),
     "‘": ("lowercase_dictionary_compression",),
     "’": ("title_case_dictionary_compression",),
     "»": ("integer_compression",),
     "«": ("small_integer_compression",),
     "¿": ("integer_list_compression",),
-    "[": ("open_list_literal",),
-    "]": ("close_list_literal",),
+    "[": ("open_list_literal", "open_list", "list"),
+    "]": ("close_list_literal", "close_list", "end_list"),
     "#": ("comment",),
     " ": ("nop",),
     "¡": ("get_veriable",),
     "!": ("set_variable",),
     "ı": ("map",),
     "€": ("single_function_map",),
     "æ": ("filter",),
@@ -91,16 +91,16 @@
     "ṅ": ("iteration_index",),
     "x": ("get_x",),
     "y": ("get_y",),
     "X": ("set_x",),
     "Y": ("set_y",),
     "Ẋ": ("set_x_without_popping",),
     "Ẏ": ("set_y_without_popping",),
-    "ẋ": ("increment_x",),
-    "ẏ": ("increment_y",),
+    "ẋ": ("apply_to_x",),
+    "ẏ": ("apply_to_y",),
     "Ȥ": ("get_global_array",),
     "ȥ": ("add_to_global_array",),
     "K": ("stack",),
     "ṇ": ("codepage_compression",),
     "q": ("quit",),
     "$": ("next_input",),
     "¤": ("input_list",),
@@ -112,14 +112,25 @@
     "⁹": ("last_input",),
     "£": ("print",),
     "¢": ("print_without_newline",),
     "ß": ("print_without_popping",),
     "Ƙ": ("first_n_integers",),
     "Ʋ": ("cumulative_reduce_by",),
     "Ɓ": ("execute_without_popping",),
+    "µµ": ("recursive_environment",),
+    "µƲ": ("single_function_reduce_by",),
+    "µɼ": ("single_function_right_reduce_by",),
+    "µƇ": ("single_function_right_cumulative_reduce_by",),
+    "µʋ": ("right_reduce_by",),
+    "µ€": ("apply_to_every_nth_item",),
+    "µ«": ("rotate_stack_left",),
+    "µ»": ("rotate_stack_right",),
+    "µ!": ("reverse_stack",),
+    "µÑ": ("adjacent_group_by",),
+    "µñ": ("single_function_adjacent_group_by",),
 }
 
 
 full_list = (
     [(token, cmd) for cmd, ovld in commands.items() for token in ovld.keywords]
     + [
         (token, "ø" + cmd)
```

### Comparing `thunno2-2.1.9/thunno2.egg-info/PKG-INFO` & `thunno2-2.2.0/thunno2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.9
+Version: 2.2.0
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.9.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.0.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

