# Comparing `tmp/traversaal-0.3.tar.gz` & `tmp/traversaal-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traversaal-0.3.tar", last modified: Sun May 14 06:42:48 2023, max compression
+gzip compressed data, was "traversaal-0.4.tar", last modified: Sun May 14 07:00:30 2023, max compression
```

## Comparing `traversaal-0.3.tar` & `traversaal-0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 06:42:48.883797 traversaal-0.3/
--rw-r--r--   0 aimzlicious   (501) staff       (20)     1761 2023-05-14 06:42:48.883669 traversaal-0.3/PKG-INFO
--rw-r--r--   0 aimzlicious   (501) staff       (20)     1522 2023-05-14 06:42:38.000000 traversaal-0.3/README.md
--rw-r--r--   0 aimzlicious   (501) staff       (20)       38 2023-05-14 06:42:48.883836 traversaal-0.3/setup.cfg
--rw-r--r--   0 aimzlicious   (501) staff       (20)      641 2023-05-14 06:42:44.000000 traversaal-0.3/setup.py
-drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 06:42:48.883500 traversaal-0.3/traversaal.egg-info/
--rw-r--r--   0 aimzlicious   (501) staff       (20)     1761 2023-05-14 06:42:48.000000 traversaal-0.3/traversaal.egg-info/PKG-INFO
--rw-r--r--   0 aimzlicious   (501) staff       (20)      187 2023-05-14 06:42:48.000000 traversaal-0.3/traversaal.egg-info/SOURCES.txt
--rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 06:42:48.000000 traversaal-0.3/traversaal.egg-info/dependency_links.txt
--rw-r--r--   0 aimzlicious   (501) staff       (20)       25 2023-05-14 06:42:48.000000 traversaal-0.3/traversaal.egg-info/requires.txt
--rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 06:42:48.000000 traversaal-0.3/traversaal.egg-info/top_level.txt
+drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 07:00:30.117926 traversaal-0.4/
+-rw-r--r--   0 aimzlicious   (501) staff       (20)     1761 2023-05-14 07:00:30.117792 traversaal-0.4/PKG-INFO
+-rw-r--r--   0 aimzlicious   (501) staff       (20)     1522 2023-05-14 06:42:38.000000 traversaal-0.4/README.md
+-rw-r--r--   0 aimzlicious   (501) staff       (20)       38 2023-05-14 07:00:30.117965 traversaal-0.4/setup.cfg
+-rw-r--r--   0 aimzlicious   (501) staff       (20)      641 2023-05-14 06:54:06.000000 traversaal-0.4/setup.py
+drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 07:00:30.117623 traversaal-0.4/traversaal.egg-info/
+-rw-r--r--   0 aimzlicious   (501) staff       (20)     1761 2023-05-14 07:00:30.000000 traversaal-0.4/traversaal.egg-info/PKG-INFO
+-rw-r--r--   0 aimzlicious   (501) staff       (20)      187 2023-05-14 07:00:30.000000 traversaal-0.4/traversaal.egg-info/SOURCES.txt
+-rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 07:00:30.000000 traversaal-0.4/traversaal.egg-info/dependency_links.txt
+-rw-r--r--   0 aimzlicious   (501) staff       (20)       25 2023-05-14 07:00:30.000000 traversaal-0.4/traversaal.egg-info/requires.txt
+-rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 07:00:30.000000 traversaal-0.4/traversaal.egg-info/top_level.txt
```

### Comparing `traversaal-0.3/PKG-INFO` & `traversaal-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traversaal
-Version: 0.3
+Version: 0.4
 Summary: A semantic search package for hotel data
 Home-page: https://github.com/hamzafarooq
 Author: Traversaal
 Author-email: hello@traversaal.com
 Description-Content-Type: text/markdown
 
 ## Traversaal
```

### Comparing `traversaal-0.3/README.md` & `traversaal-0.4/README.md`

 * *Files identical despite different names*

### Comparing `traversaal-0.3/setup.py` & `traversaal-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name="traversaal",
-    version="0.3",
+    version="0.4",
     description="A semantic search package for hotel data",
     author="Traversaal",
     author_email="hello@traversaal.com",
     url="https://github.com/hamzafarooq",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `traversaal-0.3/traversaal.egg-info/PKG-INFO` & `traversaal-0.4/traversaal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traversaal
-Version: 0.3
+Version: 0.4
 Summary: A semantic search package for hotel data
 Home-page: https://github.com/hamzafarooq
 Author: Traversaal
 Author-email: hello@traversaal.com
 Description-Content-Type: text/markdown
 
 ## Traversaal
```

