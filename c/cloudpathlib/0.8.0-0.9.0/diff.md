# Comparing `tmp/cloudpathlib-0.8.0.tar.gz` & `tmp/cloudpathlib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudpathlib-0.8.0.tar", last modified: Thu May 19 16:19:02 2022, max compression
+gzip compressed data, was "cloudpathlib-0.9.0.tar", last modified: Sat Jun  4 01:47:48 2022, max compression
```

## Comparing `cloudpathlib-0.8.0.tar` & `cloudpathlib-0.9.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:19:02.495813 cloudpathlib-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14569 2022-05-19 16:19:02.495813 cloudpathlib-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11954 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:19:02.491813 cloudpathlib-0.8.0/cloudpathlib/
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2642 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/anypath.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:19:02.491813 cloudpathlib-0.8.0/cloudpathlib/azure/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11057 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/azure/azblobclient.py
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/azure/azblobpath.py
--rw-r--r--   0 runner    (1001) docker     (121)     3800 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    36157 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/cloudpath.py
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:19:02.491813 cloudpathlib-0.8.0/cloudpathlib/gs/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/gs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9201 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/gs/gsclient.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/gs/gspath.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:19:02.495813 cloudpathlib-0.8.0/cloudpathlib/local/
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:19:02.495813 cloudpathlib-0.8.0/cloudpathlib/local/implementations/
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/local/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2342 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/local/implementations/azure.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/local/implementations/gs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/local/implementations/s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     5762 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/local/localclient.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/local/localpath.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:19:02.495813 cloudpathlib-0.8.0/cloudpathlib/s3/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11602 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/s3/s3client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/cloudpathlib/s3/s3path.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 16:19:02.491813 cloudpathlib-0.8.0/cloudpathlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14569 2022-05-19 16:19:02.000000 cloudpathlib-0.8.0/cloudpathlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-05-19 16:19:02.000000 cloudpathlib-0.8.0/cloudpathlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-19 16:19:02.000000 cloudpathlib-0.8.0/cloudpathlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-05-19 16:19:02.000000 cloudpathlib-0.8.0/cloudpathlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-19 16:19:02.000000 cloudpathlib-0.8.0/cloudpathlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-05-19 16:19:02.495813 cloudpathlib-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2346 2022-05-19 16:17:42.000000 cloudpathlib-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 01:47:48.127827 cloudpathlib-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    14569 2022-06-04 01:47:48.127827 cloudpathlib-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11954 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 01:47:48.123827 cloudpathlib-0.9.0/cloudpathlib/
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2642 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/anypath.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 01:47:48.127827 cloudpathlib-0.9.0/cloudpathlib/azure/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11247 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/azure/azblobclient.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3371 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/azure/azblobpath.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3825 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36990 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/cloudpath.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 01:47:48.127827 cloudpathlib-0.9.0/cloudpathlib/gs/
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/gs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9391 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/gs/gsclient.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3151 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/gs/gspath.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 01:47:48.127827 cloudpathlib-0.9.0/cloudpathlib/local/
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 01:47:48.127827 cloudpathlib-0.9.0/cloudpathlib/local/implementations/
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/local/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2342 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/local/implementations/azure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/local/implementations/gs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/local/implementations/s3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6069 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/local/localclient.py
+-rw-r--r--   0 runner    (1001) docker     (121)      868 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/local/localpath.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 01:47:48.127827 cloudpathlib-0.9.0/cloudpathlib/s3/
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11762 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/s3/s3client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/cloudpathlib/s3/s3path.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 01:47:48.123827 cloudpathlib-0.9.0/cloudpathlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    14569 2022-06-04 01:47:47.000000 cloudpathlib-0.9.0/cloudpathlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2022-06-04 01:47:48.000000 cloudpathlib-0.9.0/cloudpathlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-04 01:47:47.000000 cloudpathlib-0.9.0/cloudpathlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-06-04 01:47:47.000000 cloudpathlib-0.9.0/cloudpathlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-04 01:47:47.000000 cloudpathlib-0.9.0/cloudpathlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-06-04 01:47:48.131827 cloudpathlib-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2346 2022-06-04 01:46:26.000000 cloudpathlib-0.9.0/setup.py
```

### Comparing `cloudpathlib-0.8.0/LICENSE` & `cloudpathlib-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudpathlib-0.8.0/PKG-INFO` & `cloudpathlib-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpathlib
-Version: 0.8.0
+Version: 0.9.0
 Summary: pathlib-style classes for cloud storage services
 Home-page: https://github.com/drivendataorg/cloudpathlib
 Author: DrivenData
 Author-email: info@drivendata.org
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/drivendataorg/cloudpathlib/issues
 Project-URL: Documentation, https://cloudpathlib.drivendata.org/
@@ -126,70 +126,70 @@
         
         ## Supported methods and properties
         
         Most methods and properties from `pathlib.Path` are supported except for the ones that don't make sense in a cloud context. There are a few additional methods or properties that relate to specific cloud services or specifically for cloud paths.
         
         | Methods + properties   | `AzureBlobPath`   | `S3Path`   | `GSPath`   |
         |:-----------------------|:------------------|:-----------|:-----------|
+        | `absolute`             | ✅                | ✅         | ✅         |
         | `anchor`               | ✅                | ✅         | ✅         |
         | `as_uri`               | ✅                | ✅         | ✅         |
         | `drive`                | ✅                | ✅         | ✅         |
         | `exists`               | ✅                | ✅         | ✅         |
         | `glob`                 | ✅                | ✅         | ✅         |
+        | `is_absolute`          | ✅                | ✅         | ✅         |
         | `is_dir`               | ✅                | ✅         | ✅         |
         | `is_file`              | ✅                | ✅         | ✅         |
+        | `is_relative_to`       | ✅                | ✅         | ✅         |
         | `iterdir`              | ✅                | ✅         | ✅         |
         | `joinpath`             | ✅                | ✅         | ✅         |
         | `match`                | ✅                | ✅         | ✅         |
         | `mkdir`                | ✅                | ✅         | ✅         |
         | `name`                 | ✅                | ✅         | ✅         |
         | `open`                 | ✅                | ✅         | ✅         |
         | `parent`               | ✅                | ✅         | ✅         |
         | `parents`              | ✅                | ✅         | ✅         |
         | `parts`                | ✅                | ✅         | ✅         |
         | `read_bytes`           | ✅                | ✅         | ✅         |
         | `read_text`            | ✅                | ✅         | ✅         |
+        | `relative_to`          | ✅                | ✅         | ✅         |
         | `rename`               | ✅                | ✅         | ✅         |
         | `replace`              | ✅                | ✅         | ✅         |
+        | `resolve`              | ✅                | ✅         | ✅         |
         | `rglob`                | ✅                | ✅         | ✅         |
         | `rmdir`                | ✅                | ✅         | ✅         |
         | `samefile`             | ✅                | ✅         | ✅         |
         | `stat`                 | ✅                | ✅         | ✅         |
         | `stem`                 | ✅                | ✅         | ✅         |
         | `suffix`               | ✅                | ✅         | ✅         |
         | `suffixes`             | ✅                | ✅         | ✅         |
         | `touch`                | ✅                | ✅         | ✅         |
         | `unlink`               | ✅                | ✅         | ✅         |
         | `with_name`            | ✅                | ✅         | ✅         |
         | `with_suffix`          | ✅                | ✅         | ✅         |
         | `write_bytes`          | ✅                | ✅         | ✅         |
         | `write_text`           | ✅                | ✅         | ✅         |
-        | `absolute`             | ❌                | ❌         | ❌         |
         | `as_posix`             | ❌                | ❌         | ❌         |
         | `chmod`                | ❌                | ❌         | ❌         |
         | `cwd`                  | ❌                | ❌         | ❌         |
         | `expanduser`           | ❌                | ❌         | ❌         |
         | `group`                | ❌                | ❌         | ❌         |
         | `home`                 | ❌                | ❌         | ❌         |
-        | `is_absolute`          | ❌                | ❌         | ❌         |
         | `is_block_device`      | ❌                | ❌         | ❌         |
         | `is_char_device`       | ❌                | ❌         | ❌         |
         | `is_fifo`              | ❌                | ❌         | ❌         |
         | `is_mount`             | ❌                | ❌         | ❌         |
-        | `is_relative_to`       | ❌                | ❌         | ❌         |
         | `is_reserved`          | ❌                | ❌         | ❌         |
         | `is_socket`            | ❌                | ❌         | ❌         |
         | `is_symlink`           | ❌                | ❌         | ❌         |
         | `lchmod`               | ❌                | ❌         | ❌         |
         | `link_to`              | ❌                | ❌         | ❌         |
         | `lstat`                | ❌                | ❌         | ❌         |
         | `owner`                | ❌                | ❌         | ❌         |
         | `readlink`             | ❌                | ❌         | ❌         |
-        | `relative_to`          | ❌                | ❌         | ❌         |
-        | `resolve`              | ❌                | ❌         | ❌         |
         | `root`                 | ❌                | ❌         | ❌         |
         | `symlink_to`           | ❌                | ❌         | ❌         |
         | `with_stem`            | ❌                | ❌         | ❌         |
         | `cloud_prefix`         | ✅                | ✅         | ✅         |
         | `copy`                 | ✅                | ✅         | ✅         |
         | `copytree`             | ✅                | ✅         | ✅         |
         | `download_to`          | ✅                | ✅         | ✅         |
```

### Comparing `cloudpathlib-0.8.0/README.md` & `cloudpathlib-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -115,70 +115,70 @@
 
 ## Supported methods and properties
 
 Most methods and properties from `pathlib.Path` are supported except for the ones that don't make sense in a cloud context. There are a few additional methods or properties that relate to specific cloud services or specifically for cloud paths.
 
 | Methods + properties   | `AzureBlobPath`   | `S3Path`   | `GSPath`   |
 |:-----------------------|:------------------|:-----------|:-----------|
+| `absolute`             | ✅                | ✅         | ✅         |
 | `anchor`               | ✅                | ✅         | ✅         |
 | `as_uri`               | ✅                | ✅         | ✅         |
 | `drive`                | ✅                | ✅         | ✅         |
 | `exists`               | ✅                | ✅         | ✅         |
 | `glob`                 | ✅                | ✅         | ✅         |
+| `is_absolute`          | ✅                | ✅         | ✅         |
 | `is_dir`               | ✅                | ✅         | ✅         |
 | `is_file`              | ✅                | ✅         | ✅         |
+| `is_relative_to`       | ✅                | ✅         | ✅         |
 | `iterdir`              | ✅                | ✅         | ✅         |
 | `joinpath`             | ✅                | ✅         | ✅         |
 | `match`                | ✅                | ✅         | ✅         |
 | `mkdir`                | ✅                | ✅         | ✅         |
 | `name`                 | ✅                | ✅         | ✅         |
 | `open`                 | ✅                | ✅         | ✅         |
 | `parent`               | ✅                | ✅         | ✅         |
 | `parents`              | ✅                | ✅         | ✅         |
 | `parts`                | ✅                | ✅         | ✅         |
 | `read_bytes`           | ✅                | ✅         | ✅         |
 | `read_text`            | ✅                | ✅         | ✅         |
+| `relative_to`          | ✅                | ✅         | ✅         |
 | `rename`               | ✅                | ✅         | ✅         |
 | `replace`              | ✅                | ✅         | ✅         |
+| `resolve`              | ✅                | ✅         | ✅         |
 | `rglob`                | ✅                | ✅         | ✅         |
 | `rmdir`                | ✅                | ✅         | ✅         |
 | `samefile`             | ✅                | ✅         | ✅         |
 | `stat`                 | ✅                | ✅         | ✅         |
 | `stem`                 | ✅                | ✅         | ✅         |
 | `suffix`               | ✅                | ✅         | ✅         |
 | `suffixes`             | ✅                | ✅         | ✅         |
 | `touch`                | ✅                | ✅         | ✅         |
 | `unlink`               | ✅                | ✅         | ✅         |
 | `with_name`            | ✅                | ✅         | ✅         |
 | `with_suffix`          | ✅                | ✅         | ✅         |
 | `write_bytes`          | ✅                | ✅         | ✅         |
 | `write_text`           | ✅                | ✅         | ✅         |
-| `absolute`             | ❌                | ❌         | ❌         |
 | `as_posix`             | ❌                | ❌         | ❌         |
 | `chmod`                | ❌                | ❌         | ❌         |
 | `cwd`                  | ❌                | ❌         | ❌         |
 | `expanduser`           | ❌                | ❌         | ❌         |
 | `group`                | ❌                | ❌         | ❌         |
 | `home`                 | ❌                | ❌         | ❌         |
-| `is_absolute`          | ❌                | ❌         | ❌         |
 | `is_block_device`      | ❌                | ❌         | ❌         |
 | `is_char_device`       | ❌                | ❌         | ❌         |
 | `is_fifo`              | ❌                | ❌         | ❌         |
 | `is_mount`             | ❌                | ❌         | ❌         |
-| `is_relative_to`       | ❌                | ❌         | ❌         |
 | `is_reserved`          | ❌                | ❌         | ❌         |
 | `is_socket`            | ❌                | ❌         | ❌         |
 | `is_symlink`           | ❌                | ❌         | ❌         |
 | `lchmod`               | ❌                | ❌         | ❌         |
 | `link_to`              | ❌                | ❌         | ❌         |
 | `lstat`                | ❌                | ❌         | ❌         |
 | `owner`                | ❌                | ❌         | ❌         |
 | `readlink`             | ❌                | ❌         | ❌         |
-| `relative_to`          | ❌                | ❌         | ❌         |
-| `resolve`              | ❌                | ❌         | ❌         |
 | `root`                 | ❌                | ❌         | ❌         |
 | `symlink_to`           | ❌                | ❌         | ❌         |
 | `with_stem`            | ❌                | ❌         | ❌         |
 | `cloud_prefix`         | ✅                | ✅         | ✅         |
 | `copy`                 | ✅                | ✅         | ✅         |
 | `copytree`             | ✅                | ✅         | ✅         |
 | `download_to`          | ✅                | ✅         | ✅         |
```

### Comparing `cloudpathlib-0.8.0/cloudpathlib/__init__.py` & `cloudpathlib-0.9.0/cloudpathlib/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudpathlib-0.8.0/cloudpathlib/anypath.py` & `cloudpathlib-0.9.0/cloudpathlib/anypath.py`

 * *Files identical despite different names*

### Comparing `cloudpathlib-0.8.0/cloudpathlib/azure/azblobclient.py` & `cloudpathlib-0.9.0/cloudpathlib/azure/azblobclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -201,27 +201,32 @@
             target.start_copy_from_url(source.url)
 
             if remove_src:
                 self._remove(src)
 
         return dst
 
-    def _remove(self, cloud_path: AzureBlobPath) -> None:
-        if self._is_file_or_dir(cloud_path) == "dir":
+    def _remove(self, cloud_path: AzureBlobPath, missing_ok: bool = True) -> None:
+        file_or_dir = self._is_file_or_dir(cloud_path)
+        if file_or_dir == "dir":
             blobs = [
                 b.blob for b, is_dir in self._list_dir(cloud_path, recursive=True) if not is_dir
             ]
             container_client = self.service_client.get_container_client(cloud_path.container)
             container_client.delete_blobs(*blobs)
-        elif self._is_file_or_dir(cloud_path) == "file":
+        elif file_or_dir == "file":
             blob = self.service_client.get_blob_client(
                 container=cloud_path.container, blob=cloud_path.blob
             )
 
             blob.delete_blob()
+        else:
+            # Does not exist
+            if not missing_ok:
+                raise FileNotFoundError(f"File does not exist: {cloud_path}")
 
     def _upload_file(
         self, local_path: Union[str, os.PathLike], cloud_path: AzureBlobPath
     ) -> AzureBlobPath:
         blob = self.service_client.get_blob_client(
             container=cloud_path.container, blob=cloud_path.blob
         )
```

### Comparing `cloudpathlib-0.8.0/cloudpathlib/azure/azblobpath.py` & `cloudpathlib-0.9.0/cloudpathlib/azure/azblobpath.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,18 @@
     def is_file(self) -> bool:
         return self.client._is_file_or_dir(self) == "file"
 
     def mkdir(self, parents=False, exist_ok=False):
         # not possible to make empty directory on blob storage
         pass
 
-    def touch(self):
+    def touch(self, exist_ok: bool = True):
         if self.exists():
+            if not exist_ok:
+                raise FileExistsError(f"File exists: {self}")
             self.client._move_file(self, self)
         else:
             tf = TemporaryDirectory()
             p = Path(tf.name) / "empty"
             p.touch()
 
             self.client._upload_file(p, self)
```

### Comparing `cloudpathlib-0.8.0/cloudpathlib/client.py` & `cloudpathlib-0.9.0/cloudpathlib/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     @abc.abstractmethod
     def _move_file(
         self, src: BoundedCloudPath, dst: BoundedCloudPath, remove_src: bool = True
     ) -> BoundedCloudPath:
         pass
 
     @abc.abstractmethod
-    def _remove(self, path: BoundedCloudPath) -> None:
+    def _remove(self, path: BoundedCloudPath, missing_ok: bool = True) -> None:
         """Remove a file or folder from the server.
 
         Parameters
         ----------
         path : CloudPath
             The file or folder to remove.
         """
```

### Comparing `cloudpathlib-0.8.0/cloudpathlib/cloudpath.py` & `cloudpathlib-0.9.0/cloudpathlib/cloudpath.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,35 +250,31 @@
 
     def __ge__(self, other: Any) -> bool:
         if not isinstance(other, type(self)):
             return NotImplemented
         return self.parts >= other.parts
 
     # ====================== NOT IMPLEMENTED ======================
-    # absolute - no cloud equivalent; all cloud paths are absolute already
     # as_posix - no cloud equivalent; not needed since we assume url separator
     # chmod - permission changing should be explicitly done per client with methods
     #           that make sense for the client permission options
     # cwd - no cloud equivalent
     # expanduser - no cloud equivalent
     # group - should be implemented with client-specific permissions
     # home - no cloud equivalent
-    # is_absolute - no cloud equivalent; all cloud paths are absolute already
     # is_block_device - no cloud equivalent
     # is_char_device - no cloud equivalent
     # is_fifo - no cloud equivalent
     # is_mount - no cloud equivalent
     # is_reserved - no cloud equivalent
     # is_socket - no cloud equivalent
     # is_symlink - no cloud equivalent
     # lchmod - no cloud equivalent
     # lstat - no cloud equivalent
     # owner - no cloud equivalent
-    # relative to - cloud paths are absolute
-    # resolve - all cloud paths are absolute, so no resolving
     # root - drive already has the bucket and anchor/prefix has the scheme, so nothing to store here
     # symlink_to - no cloud equivalent
 
     # ====================== REQUIRED, NOT GENERIC ======================
     # Methods that must be implemented, but have no generic application
     @property
     @abc.abstractmethod
@@ -298,15 +294,15 @@
 
     @abc.abstractmethod
     def mkdir(self, parents: bool = False, exist_ok: bool = False):
         """Should be implemented using the client API without requiring a dir is downloaded"""
         pass
 
     @abc.abstractmethod
-    def touch(self):
+    def touch(self, exist_ok: bool = True):
         """Should be implemented using the client API to create and update modified time"""
         pass
 
     # ====================== IMPLEMENTED FROM SCRATCH ======================
     # Methods with their own implementations that work generically
     def __rtruediv__(self, other):
         raise ValueError(
@@ -468,20 +464,21 @@
             pass
         self.client._remove(self)
 
     def samefile(self, other_path: "CloudPath") -> bool:
         # all cloud paths are absolute and the paths are used for hash
         return self == other_path
 
-    def unlink(self):
+    def unlink(self, missing_ok=True):
+        # Note: missing_ok defaults to False in pathlib, but changing the default now would be a breaking change.
         if self.is_dir():
             raise CloudPathIsADirectoryError(
                 f"Path {self} is a directory; call rmdir instead of unlink."
             )
-        self.client._remove(self)
+        self.client._remove(self, missing_ok)
 
     def write_bytes(self, data: bytes):
         """Open the file in bytes mode, write to it, and close the file.
 
         NOTE: vendored from pathlib since we override open
         https://github.com/python/cpython/blob/3.8/Lib/pathlib.py#L1235-L1242
         """
@@ -531,28 +528,55 @@
             sequence_class = (
                 type(path_version) if not isinstance(path_version, _PathParents) else tuple
             )
             return sequence_class(
                 self._new_cloudpath(_resolve(p)) for p in path_version if _resolve(p) != p.root
             )
 
-        # when pathlib something else, we probably just want that thing
+        # when pathlib returns something else, we probably just want that thing
         # cases this should include: str, empty sequence, sequence of str, ...
         else:
             return path_version
 
     def __truediv__(self, other):
-        if not isinstance(other, (str,)):
-            raise TypeError(f"Can only join path {repr(self)} with strings.")
+        if not isinstance(other, (str, PurePosixPath)):
+            raise TypeError(f"Can only join path {repr(self)} with strings or posix paths.")
 
         return self._dispatch_to_path("__truediv__", other)
 
     def joinpath(self, *args):
         return self._dispatch_to_path("joinpath", *args)
 
+    def absolute(self):
+        return self
+
+    def is_absolute(self):
+        return True
+
+    def resolve(self, strict=False):
+        return self
+
+    def relative_to(self, other):
+        # We don't dispatch regularly since this never returns a cloud path (since it is relative, and cloud paths are
+        # absolute)
+        if not isinstance(other, CloudPath):
+            raise ValueError(f"{self} is a cloud path, but {other} is not")
+        if self.cloud_prefix != other.cloud_prefix:
+            raise ValueError(
+                f"{self} is a {self.cloud_prefix} path, but {other} is a {other.cloud_prefix} path"
+            )
+        return self._path.relative_to(other._path)
+
+    def is_relative_to(self, other):
+        try:
+            self.relative_to(other)
+            return True
+        except ValueError:
+            return False
+
     @property
     def name(self):
         return self._dispatch_to_path("name")
 
     def match(self, path_pattern):
         # strip scheme from start of pattern before testing
         if path_pattern.startswith(self.anchor + self.drive + "/"):
@@ -626,16 +650,16 @@
             f"calculate stats; this may take a long time depending on filesize"
         )
         return self._dispatch_to_local_cache_path("stat")
 
     def read_bytes(self):
         return self._dispatch_to_local_cache_path("read_bytes")
 
-    def read_text(self):
-        return self._dispatch_to_local_cache_path("read_text")
+    def read_text(self, *args, **kwargs):
+        return self._dispatch_to_local_cache_path("read_text", *args, **kwargs)
 
     # ===========  public cloud methods, not in pathlib ===============
     def download_to(self, destination: Union[str, os.PathLike]) -> Path:
         destination = Path(destination)
         if self.is_file():
             if destination.is_dir():
                 destination = destination / self.name
```

### Comparing `cloudpathlib-0.8.0/cloudpathlib/exceptions.py` & `cloudpathlib-0.9.0/cloudpathlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudpathlib-0.8.0/cloudpathlib/gs/gsclient.py` & `cloudpathlib-0.9.0/cloudpathlib/gs/gsclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -192,25 +192,30 @@
             src_bucket.copy_blob(src_blob, dst_bucket, dst.blob)
 
             if remove_src:
                 src_blob.delete()
 
         return dst
 
-    def _remove(self, cloud_path: GSPath) -> None:
-        if self._is_file_or_dir(cloud_path) == "dir":
+    def _remove(self, cloud_path: GSPath, missing_ok: bool = True) -> None:
+        file_or_dir = self._is_file_or_dir(cloud_path)
+        if file_or_dir == "dir":
             blobs = [
                 b.blob for b, is_dir in self._list_dir(cloud_path, recursive=True) if not is_dir
             ]
             bucket = self.client.bucket(cloud_path.bucket)
             for blob in blobs:
                 bucket.get_blob(blob).delete()
-        elif self._is_file_or_dir(cloud_path) == "file":
+        elif file_or_dir == "file":
             bucket = self.client.bucket(cloud_path.bucket)
             bucket.get_blob(cloud_path.blob).delete()
+        else:
+            # Does not exist
+            if not missing_ok:
+                raise FileNotFoundError(f"File does not exist: {cloud_path}")
 
     def _upload_file(self, local_path: Union[str, os.PathLike], cloud_path: GSPath) -> GSPath:
         bucket = self.client.bucket(cloud_path.bucket)
         blob = bucket.blob(cloud_path.blob)
 
         extra_args = {}
         if self.content_type_method is not None:
```

### Comparing `cloudpathlib-0.8.0/cloudpathlib/gs/gspath.py` & `cloudpathlib-0.9.0/cloudpathlib/gs/gspath.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,16 +38,18 @@
     def is_file(self) -> bool:
         return self.client._is_file_or_dir(self) == "file"
 
     def mkdir(self, parents=False, exist_ok=False):
         # not possible to make empty directory on cloud storage
         pass
 
-    def touch(self):
+    def touch(self, exist_ok: bool = True):
         if self.exists():
+            if not exist_ok:
+                raise FileExistsError(f"File exists: {self}")
             self.client._move_file(self, self)
         else:
             tf = TemporaryDirectory()
             p = Path(tf.name) / "empty"
             p.touch()
 
             self.client._upload_file(p, self)
```

### Comparing `cloudpathlib-0.8.0/cloudpathlib/local/__init__.py` & `cloudpathlib-0.9.0/cloudpathlib/local/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudpathlib-0.8.0/cloudpathlib/local/implementations/azure.py` & `cloudpathlib-0.9.0/cloudpathlib/local/implementations/azure.py`

 * *Files identical despite different names*

### Comparing `cloudpathlib-0.8.0/cloudpathlib/local/implementations/gs.py` & `cloudpathlib-0.9.0/cloudpathlib/local/implementations/gs.py`

 * *Files identical despite different names*

### Comparing `cloudpathlib-0.8.0/cloudpathlib/local/implementations/s3.py` & `cloudpathlib-0.9.0/cloudpathlib/local/implementations/s3.py`

 * *Files identical despite different names*

### Comparing `cloudpathlib-0.8.0/cloudpathlib/local/localclient.py` & `cloudpathlib-0.9.0/cloudpathlib/local/localclient.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,16 +92,19 @@
 
         if remove_src:
             self._cloud_path_to_local(src).replace(self._cloud_path_to_local(dst))
         else:
             shutil.copy(self._cloud_path_to_local(src), self._cloud_path_to_local(dst))
         return dst
 
-    def _remove(self, cloud_path: "LocalPath") -> None:
+    def _remove(self, cloud_path: "LocalPath", missing_ok: bool = True) -> None:
         local_storage_path = self._cloud_path_to_local(cloud_path)
+        if not missing_ok and not local_storage_path.exists():
+            raise FileNotFoundError(f"File does not exist: {cloud_path}")
+
         if local_storage_path.is_file():
             local_storage_path.unlink()
         elif local_storage_path.is_dir():
             shutil.rmtree(local_storage_path)
 
     def _stat(self, cloud_path: "LocalPath") -> os.stat_result:
         stat_result = self._cloud_path_to_local(cloud_path).stat()
@@ -117,16 +120,18 @@
                 stat_result.st_size,  # size,
                 None,  # atime,
                 stat_result.st_mtime,  # mtime,
                 None,  # ctime,
             )
         )
 
-    def _touch(self, cloud_path: "LocalPath") -> None:
+    def _touch(self, cloud_path: "LocalPath", exist_ok: bool = True) -> None:
         local_storage_path = self._cloud_path_to_local(cloud_path)
+        if local_storage_path.exists() and not exist_ok:
+            raise FileExistsError(f"File exists: {cloud_path}")
         local_storage_path.parent.mkdir(exist_ok=True, parents=True)
         local_storage_path.touch()
 
     def _upload_file(
         self, local_path: Union[str, os.PathLike], cloud_path: "LocalPath"
     ) -> "LocalPath":
         dst = self._cloud_path_to_local(cloud_path)
```

### Comparing `cloudpathlib-0.8.0/cloudpathlib/local/localpath.py` & `cloudpathlib-0.9.0/cloudpathlib/local/localpath.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,9 +24,9 @@
             meta = self.client._stat(self)
         except FileNotFoundError:
             raise NoStatError(
                 f"No stats available for {self}; it may be a directory or not exist."
             )
         return meta
 
-    def touch(self):
-        self.client._touch(self)
+    def touch(self, exist_ok: bool = True):
+        self.client._touch(self, exist_ok)
```

### Comparing `cloudpathlib-0.8.0/cloudpathlib/s3/s3client.py` & `cloudpathlib-0.9.0/cloudpathlib/s3/s3client.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,15 +222,15 @@
             target = self.s3.Object(dst.bucket, dst.key)
             target.copy({"Bucket": src.bucket, "Key": src.key})
 
             if remove_src:
                 self._remove(src)
         return dst
 
-    def _remove(self, cloud_path: S3Path) -> None:
+    def _remove(self, cloud_path: S3Path, missing_ok: bool = True) -> None:
         try:
             obj = self.s3.Object(cloud_path.bucket, cloud_path.key)
 
             # will throw if not a file
             obj.load()
 
             resp = obj.delete()
@@ -246,14 +246,17 @@
 
             resp = bucket.objects.filter(Prefix=prefix).delete()
 
             # ensure directory deleted; if cloud_path did not exist at all
             # resp will be [], so no need to check success
             if resp:
                 assert resp[0].get("ResponseMetadata").get("HTTPStatusCode") == 200
+            else:
+                if not missing_ok:
+                    raise FileNotFoundError(f"File does not exist: {cloud_path}")
 
     def _upload_file(self, local_path: Union[str, os.PathLike], cloud_path: S3Path) -> S3Path:
         obj = self.s3.Object(cloud_path.bucket, cloud_path.key)
 
         extra_args = {}
 
         if self.content_type_method is not None:
```

### Comparing `cloudpathlib-0.8.0/cloudpathlib/s3/s3path.py` & `cloudpathlib-0.9.0/cloudpathlib/s3/s3path.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,16 +38,18 @@
     def is_file(self) -> bool:
         return self.client._is_file_or_dir(self) == "file"
 
     def mkdir(self, parents=False, exist_ok=False):
         # not possible to make empty directory on s3
         pass
 
-    def touch(self):
+    def touch(self, exist_ok: bool = True):
         if self.exists():
+            if not exist_ok:
+                raise FileExistsError(f"File exists: {self}")
             self.client._move_file(self, self)
         else:
             tf = TemporaryDirectory()
             p = Path(tf.name) / "empty"
             p.touch()
 
             self.client._upload_file(p, self)
```

### Comparing `cloudpathlib-0.8.0/cloudpathlib.egg-info/PKG-INFO` & `cloudpathlib-0.9.0/cloudpathlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpathlib
-Version: 0.8.0
+Version: 0.9.0
 Summary: pathlib-style classes for cloud storage services
 Home-page: https://github.com/drivendataorg/cloudpathlib
 Author: DrivenData
 Author-email: info@drivendata.org
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/drivendataorg/cloudpathlib/issues
 Project-URL: Documentation, https://cloudpathlib.drivendata.org/
@@ -126,70 +126,70 @@
         
         ## Supported methods and properties
         
         Most methods and properties from `pathlib.Path` are supported except for the ones that don't make sense in a cloud context. There are a few additional methods or properties that relate to specific cloud services or specifically for cloud paths.
         
         | Methods + properties   | `AzureBlobPath`   | `S3Path`   | `GSPath`   |
         |:-----------------------|:------------------|:-----------|:-----------|
+        | `absolute`             | ✅                | ✅         | ✅         |
         | `anchor`               | ✅                | ✅         | ✅         |
         | `as_uri`               | ✅                | ✅         | ✅         |
         | `drive`                | ✅                | ✅         | ✅         |
         | `exists`               | ✅                | ✅         | ✅         |
         | `glob`                 | ✅                | ✅         | ✅         |
+        | `is_absolute`          | ✅                | ✅         | ✅         |
         | `is_dir`               | ✅                | ✅         | ✅         |
         | `is_file`              | ✅                | ✅         | ✅         |
+        | `is_relative_to`       | ✅                | ✅         | ✅         |
         | `iterdir`              | ✅                | ✅         | ✅         |
         | `joinpath`             | ✅                | ✅         | ✅         |
         | `match`                | ✅                | ✅         | ✅         |
         | `mkdir`                | ✅                | ✅         | ✅         |
         | `name`                 | ✅                | ✅         | ✅         |
         | `open`                 | ✅                | ✅         | ✅         |
         | `parent`               | ✅                | ✅         | ✅         |
         | `parents`              | ✅                | ✅         | ✅         |
         | `parts`                | ✅                | ✅         | ✅         |
         | `read_bytes`           | ✅                | ✅         | ✅         |
         | `read_text`            | ✅                | ✅         | ✅         |
+        | `relative_to`          | ✅                | ✅         | ✅         |
         | `rename`               | ✅                | ✅         | ✅         |
         | `replace`              | ✅                | ✅         | ✅         |
+        | `resolve`              | ✅                | ✅         | ✅         |
         | `rglob`                | ✅                | ✅         | ✅         |
         | `rmdir`                | ✅                | ✅         | ✅         |
         | `samefile`             | ✅                | ✅         | ✅         |
         | `stat`                 | ✅                | ✅         | ✅         |
         | `stem`                 | ✅                | ✅         | ✅         |
         | `suffix`               | ✅                | ✅         | ✅         |
         | `suffixes`             | ✅                | ✅         | ✅         |
         | `touch`                | ✅                | ✅         | ✅         |
         | `unlink`               | ✅                | ✅         | ✅         |
         | `with_name`            | ✅                | ✅         | ✅         |
         | `with_suffix`          | ✅                | ✅         | ✅         |
         | `write_bytes`          | ✅                | ✅         | ✅         |
         | `write_text`           | ✅                | ✅         | ✅         |
-        | `absolute`             | ❌                | ❌         | ❌         |
         | `as_posix`             | ❌                | ❌         | ❌         |
         | `chmod`                | ❌                | ❌         | ❌         |
         | `cwd`                  | ❌                | ❌         | ❌         |
         | `expanduser`           | ❌                | ❌         | ❌         |
         | `group`                | ❌                | ❌         | ❌         |
         | `home`                 | ❌                | ❌         | ❌         |
-        | `is_absolute`          | ❌                | ❌         | ❌         |
         | `is_block_device`      | ❌                | ❌         | ❌         |
         | `is_char_device`       | ❌                | ❌         | ❌         |
         | `is_fifo`              | ❌                | ❌         | ❌         |
         | `is_mount`             | ❌                | ❌         | ❌         |
-        | `is_relative_to`       | ❌                | ❌         | ❌         |
         | `is_reserved`          | ❌                | ❌         | ❌         |
         | `is_socket`            | ❌                | ❌         | ❌         |
         | `is_symlink`           | ❌                | ❌         | ❌         |
         | `lchmod`               | ❌                | ❌         | ❌         |
         | `link_to`              | ❌                | ❌         | ❌         |
         | `lstat`                | ❌                | ❌         | ❌         |
         | `owner`                | ❌                | ❌         | ❌         |
         | `readlink`             | ❌                | ❌         | ❌         |
-        | `relative_to`          | ❌                | ❌         | ❌         |
-        | `resolve`              | ❌                | ❌         | ❌         |
         | `root`                 | ❌                | ❌         | ❌         |
         | `symlink_to`           | ❌                | ❌         | ❌         |
         | `with_stem`            | ❌                | ❌         | ❌         |
         | `cloud_prefix`         | ✅                | ✅         | ✅         |
         | `copy`                 | ✅                | ✅         | ✅         |
         | `copytree`             | ✅                | ✅         | ✅         |
         | `download_to`          | ✅                | ✅         | ✅         |
```

### Comparing `cloudpathlib-0.8.0/cloudpathlib.egg-info/SOURCES.txt` & `cloudpathlib-0.9.0/cloudpathlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudpathlib-0.8.0/setup.py` & `cloudpathlib-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,9 +56,9 @@
     packages=find_packages(exclude=["tests"]),
     project_urls={
         "Bug Tracker": "https://github.com/drivendataorg/cloudpathlib/issues",
         "Documentation": "https://cloudpathlib.drivendata.org/",
         "Source Code": "https://github.com/drivendataorg/cloudpathlib",
     },
     url="https://github.com/drivendataorg/cloudpathlib",
-    version="0.8.0",
+    version="0.9.0",
 )
```

