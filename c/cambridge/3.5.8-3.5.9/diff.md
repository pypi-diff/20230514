# Comparing `tmp/cambridge-3.5.8.tar.gz` & `tmp/cambridge-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cambridge-3.5.8.tar", last modified: Sat Dec  3 12:58:53 2022, max compression
+gzip compressed data, was "cambridge-3.5.9.tar", last modified: Sat Dec  3 14:50:22 2022, max compression
```

## Comparing `cambridge-3.5.8.tar` & `cambridge-3.5.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      120 2022-11-21 00:36:09.176389 cambridge-3.5.8/.gitignore
--rw-r--r--   0        0        0    32422 2022-09-14 04:27:11.813026 cambridge-3.5.8/LICENSE
--rw-r--r--   0        0        0     2844 2022-11-23 13:54:32.516068 cambridge-3.5.8/README.md
--rw-r--r--   0        0        0      271 2022-12-03 12:58:26.112395 cambridge-3.5.8/cambridge/__init__.py
--rw-r--r--   0        0        0     7484 2022-11-30 07:53:10.465071 cambridge-3.5.8/cambridge/args.py
--rw-r--r--   0        0        0     2269 2022-11-27 15:51:03.638493 cambridge-3.5.8/cambridge/cache.py
--rw-r--r--   0        0        0     1564 2022-11-25 05:35:06.918267 cambridge-3.5.8/cambridge/colorschemes/webster_color.py
--rw-r--r--   0        0        0      460 2022-11-30 07:53:10.467072 cambridge-3.5.8/cambridge/console.py
--rw-r--r--   0        0        0    20719 2022-11-27 05:10:53.234236 cambridge-3.5.8/cambridge/dicts/cambridge.py
--rw-r--r--   0        0        0     4966 2022-11-30 07:53:10.469072 cambridge-3.5.8/cambridge/dicts/dict.py
--rw-r--r--   0        0        0    27067 2022-12-03 12:58:12.318642 cambridge-3.5.8/cambridge/dicts/webster.py
--rw-r--r--   0        0        0      995 2022-11-27 05:10:53.235236 cambridge-3.5.8/cambridge/errors.py
--rw-r--r--   0        0        0      636 2022-10-20 08:13:07.026663 cambridge-3.5.8/cambridge/log.py
--rw-r--r--   0        0        0      901 2022-11-27 05:10:53.237236 cambridge-3.5.8/cambridge/main.py
--rw-r--r--   0        0        0      253 2022-11-25 09:55:40.672237 cambridge-3.5.8/cambridge/settings.py
--rw-r--r--   0        0        0     2291 2022-09-14 04:27:11.816026 cambridge-3.5.8/cambridge/utils.py
--rw-r--r--   0        0        0      718 2022-09-14 04:36:05.658038 cambridge-3.5.8/pyproject.toml
--rw-r--r--   0        0        0   280804 2022-09-14 04:27:11.819026 cambridge-3.5.8/screenshots/fzf.png
--rw-r--r--   0        0        0   334941 2022-09-14 04:27:11.822026 cambridge-3.5.8/screenshots/word.png
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 cambridge-3.5.8/PKG-INFO
+-rw-r--r--   0        0        0      120 2022-11-21 00:36:09.176389 cambridge-3.5.9/.gitignore
+-rw-r--r--   0        0        0    32422 2022-09-14 04:27:11.813026 cambridge-3.5.9/LICENSE
+-rw-r--r--   0        0        0     2844 2022-11-23 13:54:32.516068 cambridge-3.5.9/README.md
+-rw-r--r--   0        0        0      271 2022-12-03 14:48:46.847857 cambridge-3.5.9/cambridge/__init__.py
+-rw-r--r--   0        0        0     7484 2022-11-30 07:53:10.465071 cambridge-3.5.9/cambridge/args.py
+-rw-r--r--   0        0        0     2269 2022-11-27 15:51:03.638493 cambridge-3.5.9/cambridge/cache.py
+-rw-r--r--   0        0        0     1564 2022-11-25 05:35:06.918267 cambridge-3.5.9/cambridge/colorschemes/webster_color.py
+-rw-r--r--   0        0        0      460 2022-11-30 07:53:10.467072 cambridge-3.5.9/cambridge/console.py
+-rw-r--r--   0        0        0    20719 2022-11-27 05:10:53.234236 cambridge-3.5.9/cambridge/dicts/cambridge.py
+-rw-r--r--   0        0        0     4966 2022-11-30 07:53:10.469072 cambridge-3.5.9/cambridge/dicts/dict.py
+-rw-r--r--   0        0        0    28314 2022-12-03 14:46:56.405820 cambridge-3.5.9/cambridge/dicts/webster.py
+-rw-r--r--   0        0        0      995 2022-11-27 05:10:53.235236 cambridge-3.5.9/cambridge/errors.py
+-rw-r--r--   0        0        0      636 2022-10-20 08:13:07.026663 cambridge-3.5.9/cambridge/log.py
+-rw-r--r--   0        0        0      901 2022-11-27 05:10:53.237236 cambridge-3.5.9/cambridge/main.py
+-rw-r--r--   0        0        0      253 2022-11-25 09:55:40.672237 cambridge-3.5.9/cambridge/settings.py
+-rw-r--r--   0        0        0     2291 2022-09-14 04:27:11.816026 cambridge-3.5.9/cambridge/utils.py
+-rw-r--r--   0        0        0      718 2022-09-14 04:36:05.658038 cambridge-3.5.9/pyproject.toml
+-rw-r--r--   0        0        0   280804 2022-09-14 04:27:11.819026 cambridge-3.5.9/screenshots/fzf.png
+-rw-r--r--   0        0        0   334941 2022-09-14 04:27:11.822026 cambridge-3.5.9/screenshots/word.png
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 cambridge-3.5.9/PKG-INFO
```

### Comparing `cambridge-3.5.8/LICENSE` & `cambridge-3.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/README.md` & `cambridge-3.5.9/README.md`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/cambridge/args.py` & `cambridge-3.5.9/cambridge/args.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/cambridge/cache.py` & `cambridge-3.5.9/cambridge/cache.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/cambridge/colorschemes/webster_color.py` & `cambridge-3.5.9/cambridge/colorschemes/webster_color.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/cambridge/dicts/cambridge.py` & `cambridge-3.5.9/cambridge/dicts/cambridge.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/cambridge/dicts/dict.py` & `cambridge-3.5.9/cambridge/dicts/dict.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/cambridge/dicts/webster.py` & `cambridge-3.5.9/cambridge/dicts/webster.py`

 * *Files 2% similar despite different names*

```diff
@@ -414,15 +414,15 @@
                 if child.getprevious() is not None and child.getprevious().attrib["class"] == "sub-content-thread":
                     print()
                 elms = child.getchildren()[0].getchildren()
                 for elm in elms:
                     if elm.attrib["class"] == "unText":
                         text = "".join(list(elm.itertext())).strip()
                         if "mdash" in elm.getprevious().attrib["class"]:
-                            if child.getprevious().get("class") == "sub-content-thread": # see "beat"
+                            if child.getprevious() is not None and child.getprevious().get("class") == "sub-content-thread": # see "beat"
                                 format_basedon_ancestor(ancestor_attr, prefix="")
                             print_meaning_badge("->" + text)
                         else:
                             format_basedon_ancestor(ancestor_attr, prefix="")
                             print_meaning_badge(text)
                     if elm.attrib["class"] == "sub-content-thread":
                         sub_content_thread(elm, ancestor_attr)
@@ -498,17 +498,17 @@
                     dt(elm, attr, elm_attr)
 
                 if elm_attr == "et":
                     et(elm)
 
                 if elm_attr == "il ":
                     print_meaning_badge(elm.text.strip(), end=" ")
-            
+                
                 if elm_attr == "if":
-                    print_meaning_content(elm.text.strip(), end=" ")
+                    console.print(f"[{webster_color.wt}]{elm.text}", end=" ")
 
             else:
                 for i in elm.iterchildren():
                     if i.get("class") == "vl":
                         print_meaning_badge(i.text.strip())                
                     else:
                         print_meaning_content(i.text, end=" ")
@@ -538,19 +538,24 @@
             console.print(f"[{webster_color.bold} {webster_color.meaning_num}]{child.text}", end=" ")
 
         # print meaning content
         if "ms-lg-4 ms-3 w-100" in attr:
             for c in child.iterchildren():
                 cc = c.getchildren()
                 if cc[0].get("class") == "sen has-num-only":
-                    ccc = cc[0][1]
-                    if "sl badge mw-badge" in ccc.get("class"):
-                        print_meaning_badge(ccc.text)
-                    if ccc.get("class") == "et":
-                        et(ccc)
+                    ccc = cc[0]
+                    for i in ccc.iterchildren():
+                        i_attr = i.get("class")
+                        if i_attr is not None:
+                            if ("badge mw-badge" in i_attr) or ("il" in i_attr):
+                                print_meaning_badge(i.text.strip())
+                            if "if" in i_attr:
+                                console.print(f"[{webster_color.wt}]{i.text}", end=" ")
+                            if i_attr == "et":
+                                et(i)
                     print()
                     continue
                     
                 # print class "sb-0 sb-entry", "sb-1 sb-entry" ...
                 sb_entry(c, attr) 
 
 
@@ -629,27 +634,45 @@
 
 # --- parse class "row headword-row header-ins" --- #
 def row_headword_row_header_ins(node):
     """Print verb types. e.g. valued; valuing"""
 
     children = node.getchildren()[0].getchildren()[0]
     for child in children:
-        attr = child.attrib["class"]
-        if attr == "il  il-badge badge mw-badge-gray-100":
-            console.print(f"[{webster_color.bold} {webster_color.italic} {webster_color.wt}]{child.text.strip()}", end=" ")
-        elif attr == "prt-a":
-            print_pron(child, end="")
-        elif attr == "il ":
-            print_or_badge(child.text)
-        else:
-            console.print(f"[{webster_color.wt}]{child.text}", end="")
+        attr = child.get("class")
+        if attr is not None:
+            if attr == "il  il-badge badge mw-badge-gray-100":
+                console.print(f"[{webster_color.bold} {webster_color.italic} {webster_color.wt}]{child.text.strip()}", end=" ")
+            elif attr == "prt-a":
+                print_pron(child, end="")
+            elif attr == "il ":
+                print_or_badge(child.text)
+            else:
+                console.print(f"[{webster_color.wt}]{child.text}", end="")
 
     print()
 
 
+# --- parse class "row headword-row header-vrs" --- #
+def row_headword_row_header_vrs(node):
+    """Print word variants. e.g. premise variants or less commonly premiss"""
+
+    children = node.getchildren()[0].getchildren()[0]
+    for child in children.iterdescendants():
+        attr = child.get("class")
+        if attr is not None:
+            if "badge mw-badge" in attr:
+                console.print(f"[{webster_color.bold} {webster_color.italic} {webster_color.wt}]{child.text.strip()}", end=" ")
+            elif attr == "il " or attr == "vl":
+                print_or_badge(child.text)
+            else:
+                console.print(f"[{webster_color.wt}]{child.text}", end="")
+
+    print()
+
 # --- parse class "dxnls" --- #
 def see_also(node):
     """Print seealso section."""
 
     texts = list(node.itertext())
     for text in texts:
         text = text.strip()
@@ -672,14 +695,17 @@
             if elm.attrib["class"]:
                 if "row entry-header" in elm.attrib["class"]:
                     row_entry_header(elm)
 
                 if elm.attrib["class"] == "row headword-row header-ins":
                     row_headword_row_header_ins(elm) 
 
+                if elm.attrib["class"] == "row headword-row header-vrs":
+                    row_headword_row_header_vrs(elm) 
+
                 if elm.attrib["class"] == "vg":
                     vg(elm)
 
                 if elm.attrib["class"] == "entry-uros ":
                     entry_uros(elm)
 
                 if elm.attrib["class"] == "dxnls":
```

### Comparing `cambridge-3.5.8/cambridge/errors.py` & `cambridge-3.5.9/cambridge/errors.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/cambridge/log.py` & `cambridge-3.5.9/cambridge/log.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/cambridge/main.py` & `cambridge-3.5.9/cambridge/main.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/cambridge/utils.py` & `cambridge-3.5.9/cambridge/utils.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/pyproject.toml` & `cambridge-3.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/screenshots/fzf.png` & `cambridge-3.5.9/screenshots/fzf.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/screenshots/word.png` & `cambridge-3.5.9/screenshots/word.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.5.8/PKG-INFO` & `cambridge-3.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cambridge
-Version: 3.5.8
+Version: 3.5.9
 Summary: cambridge is a terminal version of Cambridge Dictionary.
 Home-page: https://github.com/KateWang2016/cambridge
 Keywords: dictionary, cambridge, webster, English, web scraping, python
 Author: Kate Wang
 Author-email: kate.wang2018@gmail.com
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

