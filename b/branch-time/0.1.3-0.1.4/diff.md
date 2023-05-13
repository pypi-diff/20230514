# Comparing `tmp/branch_time-0.1.3.tar.gz` & `tmp/branch_time-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "branch_time-0.1.3.tar", max compression
+gzip compressed data, was "branch_time-0.1.4.tar", max compression
```

## Comparing `branch_time-0.1.3.tar` & `branch_time-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-25 00:24:44.574088 branch_time-0.1.3/branch_time/__init__,py
--rw-r--r--   0        0        0      238 2023-04-23 02:05:09.607644 branch_time-0.1.3/branch_time/GitRepositoryError.py
--rw-r--r--   0        0        0     3151 2023-04-25 01:44:02.508972 branch_time-0.1.3/branch_time/jira.py
--rw-r--r--   0        0        0       20 2023-04-24 21:48:29.650929 branch_time-0.1.3/LICENSE
--rw-r--r--   0        0        0     1102 2023-04-25 01:42:12.009051 branch_time-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1622 2023-04-25 01:42:00.719033 branch_time-0.1.3/README.md
--rw-r--r--   0        0        0     2674 1970-01-01 00:00:00.000000 branch_time-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-27 01:55:57.774979 branch_time-0.1.4/branch_time/__init__,py
+-rw-r--r--   0        0        0      238 2023-04-27 01:55:57.774979 branch_time-0.1.4/branch_time/GitRepositoryError.py
+-rw-r--r--   0        0        0     3221 2023-05-13 21:58:40.705034 branch_time-0.1.4/branch_time/jira.py
+-rw-r--r--   0        0        0       20 2023-04-27 01:55:57.773979 branch_time-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1110 2023-05-13 22:44:31.109803 branch_time-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1622 2023-04-27 01:55:57.773979 branch_time-0.1.4/README.md
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 branch_time-0.1.4/PKG-INFO
```

### Comparing `branch_time-0.1.3/branch_time/jira.py` & `branch_time-0.1.4/branch_time/jira.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     output_file: str = typer.Option(
         date.today(),
         "--output",
         "-o",
         help="location where text file with timing of branch changes will be saved",
     ),
 ):
+    console.print("[red1]Time count started...\n\n")
     while True:
         with open(f"{output_file}.txt", "a+") as file:
             try:
                 process = subprocess.Popen(
                     "git rev-parse --abbrev-ref HEAD",
                     stdout=subprocess.PIPE,
                     cwd=repository,
@@ -82,15 +83,15 @@
                 last_line = last_line_on_file(file)
                 if is_not_same_branch(last_line, branch):
                     file.write(count_time(branch, last_line))
                     file.write(
                         f"Branch: {branch} - Time: {now.hour}:{now.minute}:{now.second}\n"
                     )
                 time.sleep(time_in_minute * 60)
-
+                
             except NotADirectoryError:
                 console.print("[red1]Directory not found")
                 sys.exit(1)
             except KeyboardInterrupt:
                 now = datetime.now()
                 file.write(f"FINISHED... {now.hour}:{now.minute}:{now.second}\n")
                 sys.exit(0)
```

### Comparing `branch_time-0.1.3/pyproject.toml` & `branch_time-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "branch-time"
-version = "0.1.3"
+version = "0.1.4"
 description = "Counts time in a branch"
 license="BeerWare"
 authors = ["Icaro Nunes"]
 readme = "README.md"
 packages = [{include = "branch_time"}]
 classifiers= [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
 ]
 
 [tool.poetry.dependencies]
-python = "^3"
+python = ">=3.8.0,<4"
 typer = "^0.7.0"
 typer-cli = "^0.0.13"
 click = "^8.0"
 pytest = "^7.3.1"
 rich = "^13.3.4"
 
 [tool.poetry.scripts]
```

### Comparing `branch_time-0.1.3/README.md` & `branch_time-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `branch_time-0.1.3/PKG-INFO` & `branch_time-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: branch-time
-Version: 0.1.3
+Version: 0.1.4
 Summary: Counts time in a branch
 License: Beerware
 Author: Icaro Nunes
-Requires-Python: >=3,<4
+Requires-Python: >=3.8.0,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0,<9.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
```

