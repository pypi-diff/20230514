# Comparing `tmp/rpl-1.9.1.tar.gz` & `tmp/rpl-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rpl-1.9.1.tar", last modified: Tue Mar 16 10:06:01 2021, max compression
+gzip compressed data, was "dist/rpl-1.9.2.tar", last modified: Wed Mar 24 22:05:22 2021, max compression
```

## Comparing `rpl-1.9.1.tar` & `rpl-1.9.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2021-03-16 10:06:01.059925 rpl-1.9.1/
--rw-r-----   0 rrt       (1000) rrt       (1000)      747 2021-03-16 10:06:01.059925 rpl-1.9.1/PKG-INFO
--rw-r-----   0 rrt       (1000) rrt       (1000)      279 2019-08-16 12:16:51.000000 rpl-1.9.1/README.md
--rwxr-x---   0 rrt       (1000) rrt       (1000)    16748 2021-03-16 10:04:59.000000 rpl-1.9.1/rpl
--rw-r-----   0 rrt       (1000) rrt       (1000)     3235 2021-02-07 16:36:41.000000 rpl-1.9.1/rpl.1
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2021-03-16 10:06:01.059925 rpl-1.9.1/rpl.egg-info/
--rw-r-----   0 rrt       (1000) rrt       (1000)      747 2021-03-16 10:06:01.000000 rpl-1.9.1/rpl.egg-info/PKG-INFO
--rw-r-----   0 rrt       (1000) rrt       (1000)      172 2021-03-16 10:06:01.000000 rpl-1.9.1/rpl.egg-info/SOURCES.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)        1 2021-03-16 10:06:01.000000 rpl-1.9.1/rpl.egg-info/dependency_links.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)       23 2021-03-16 10:06:01.000000 rpl-1.9.1/rpl.egg-info/requires.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)        1 2021-03-16 10:06:01.000000 rpl-1.9.1/rpl.egg-info/top_level.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)      577 2021-03-16 10:06:01.059925 rpl-1.9.1/setup.cfg
--rw-r-----   0 rrt       (1000) rrt       (1000)      210 2020-10-05 11:18:11.000000 rpl-1.9.1/setup.py
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2021-03-24 22:05:22.004583 rpl-1.9.2/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      747 2021-03-24 22:05:22.004583 rpl-1.9.2/PKG-INFO
+-rw-r-----   0 rrt       (1000) rrt       (1000)      279 2019-08-16 12:16:51.000000 rpl-1.9.2/README.md
+-rwxr-x---   0 rrt       (1000) rrt       (1000)    16836 2021-03-24 22:04:57.000000 rpl-1.9.2/rpl
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3231 2021-03-16 11:02:18.000000 rpl-1.9.2/rpl.1
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2021-03-24 22:05:22.004583 rpl-1.9.2/rpl.egg-info/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      747 2021-03-24 22:05:21.000000 rpl-1.9.2/rpl.egg-info/PKG-INFO
+-rw-r-----   0 rrt       (1000) rrt       (1000)      172 2021-03-24 22:05:21.000000 rpl-1.9.2/rpl.egg-info/SOURCES.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)        1 2021-03-24 22:05:21.000000 rpl-1.9.2/rpl.egg-info/dependency_links.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)       23 2021-03-24 22:05:21.000000 rpl-1.9.2/rpl.egg-info/requires.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)        1 2021-03-24 22:05:21.000000 rpl-1.9.2/rpl.egg-info/top_level.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)      577 2021-03-24 22:05:22.004583 rpl-1.9.2/setup.cfg
+-rw-r-----   0 rrt       (1000) rrt       (1000)      210 2020-10-05 11:18:11.000000 rpl-1.9.2/setup.py
```

### Comparing `rpl-1.9.1/PKG-INFO` & `rpl-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpl
-Version: 1.9.1
+Version: 1.9.2
 Summary: Replace strings in files
 Home-page: https://github.com/rrthomas/rpl
 Author: Reuben Thomas
 Author-email: rrt@sc3d.org
 License: GPL v3 or later
 Description: # rpl
```

### Comparing `rpl-1.9.1/rpl` & `rpl-1.9.2/rpl`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import tempfile
 import warnings
 from warnings import warn
 
 from chardet.universaldetector import UniversalDetector
 
 
-VERSION = "1.9.1"
+VERSION = "1.9.2"
 
 def simple_warning(msg, cat, filename, lineno, file, line):
     print("\n{}: {}".format(parser.prog, msg), file=file or sys.stderr)
 warnings.showwarning = simple_warning
 
 def die(code, msg):
     warn(msg)
@@ -335,14 +335,15 @@
 if args.whole_words:
     regex_str = r"\b" + regex_str + r"\b"
 # Call re.compile so we get an error if the regex is invalid, & count groups.
 regex = re.compile(regex_str, re.I if args.ignore_case else 0)
 split_regex = re.compile(f"({regex_str})", re.I if args.ignore_case else 0)
 
 total_files = 0
+matched_files = 0
 total_matches = 0
 for filename in files:
     perms = None
     if filename == "-":
         filename = "standard input"
         # Access stdin and stdout as binary.
         f = sys.stdin.buffer
@@ -436,14 +437,16 @@
     f.close()
     o.close()
 
     if matches == 0:
         if tmp_path is not None:
             os.unlink(tmp_path)
         continue
+    else:
+        matched_files += 1
 
     if args.dry_run:
         if tmp_path is None:
             fn = filename
         else:
             try:
                 fn = os.path.realpath(filename)
@@ -496,13 +499,14 @@
                 warn("Error setting timestamps of {}: {}".format(filename, e))
 
     total_matches += matches
 
 
 # We're about to exit, give a summary
 if not args.quiet:
-    warn("{} matches {} in {} file{}".format(
+    warn("{} matches {} in {} out of {} file{}".format(
         total_matches,
         "found" if args.dry_run else "replaced",
+        matched_files,
         total_files,
         "s" if total_files != 1 else "",
     ))
```

### Comparing `rpl-1.9.1/rpl.1` & `rpl-1.9.2/rpl.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.47.13.
-.TH RPL "1" "February 2021" "rpl 1.9rc2" "User Commands"
+.TH RPL "1" "March 2021" "rpl 1.9.1" "User Commands"
 .SH NAME
 rpl \- replace strings in files
 .SH DESCRIPTION
 usage: rpl [\-h] [\-\-version] [\-\-encoding ENCODING] [\-E] [\-i] [\-m] [\-w] [\-b] [\-q] [\-v] [\-s] [\-e] [\-F] [\-\-files] [\-\-noglob] [\-p] [\-f] [\-d] OLD\-TEXT NEW\-TEXT [FILE [FILE ...]]
 .PP
 Search and replace text in files.
 .PP
```

### Comparing `rpl-1.9.1/rpl.egg-info/PKG-INFO` & `rpl-1.9.2/rpl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpl
-Version: 1.9.1
+Version: 1.9.2
 Summary: Replace strings in files
 Home-page: https://github.com/rrthomas/rpl
 Author: Reuben Thomas
 Author-email: rrt@sc3d.org
 License: GPL v3 or later
 Description: # rpl
```

### Comparing `rpl-1.9.1/setup.cfg` & `rpl-1.9.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = rpl
 author = Reuben Thomas
 author_email = rrt@sc3d.org
 home_page = https://github.com/rrthomas/rpl
-version = 1.9.1
+version = 1.9.2
 description = Replace strings in files
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPL v3 or later
 classifiers = 
 	Environment :: Console
 	Programming Language :: Python :: 3
```

