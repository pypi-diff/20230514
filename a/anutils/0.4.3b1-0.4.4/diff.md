# Comparing `tmp/anutils-0.4.3b1.tar.gz` & `tmp/anutils-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anutils-0.4.3b1.tar", last modified: Fri May 12 19:27:53 2023, max compression
+gzip compressed data, was "anutils-0.4.4.tar", last modified: Sun May 14 18:24:37 2023, max compression
```

## Comparing `anutils-0.4.3b1.tar` & `anutils-0.4.4.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 19:27:53.923323 anutils-0.4.3b1/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1799 2022-06-15 05:53:11.000000 anutils-0.4.3b1/.gitignore
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2865 2023-05-12 19:27:53.923323 anutils-0.4.3b1/PKG-INFO
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2372 2023-05-07 16:11:39.000000 anutils-0.4.3b1/README.md
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       38 2023-05-12 19:27:53.923323 anutils-0.4.3b1/setup.cfg
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)      903 2023-05-12 19:27:10.000000 anutils-0.4.3b1/setup.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 19:27:53.919323 anutils-0.4.3b1/src/
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 19:27:53.919323 anutils-0.4.3b1/src/anutils/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)       80 2023-05-11 06:30:19.000000 anutils-0.4.3b1/src/anutils/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      416 2023-05-11 06:33:57.000000 anutils-0.4.3b1/src/anutils/exceptions.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 19:27:53.919323 anutils-0.4.3b1/src/anutils/mlutils/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)       38 2023-05-11 06:32:55.000000 anutils-0.4.3b1/src/anutils/mlutils/__init__.py
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2498 2023-05-11 06:32:47.000000 anutils-0.4.3b1/src/anutils/mlutils/mlutils.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 19:27:53.919323 anutils-0.4.3b1/src/anutils/scutils/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)      303 2023-05-12 19:16:38.000000 anutils-0.4.3b1/src/anutils/scutils/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     7665 2023-05-12 15:17:57.000000 anutils-0.4.3b1/src/anutils/scutils/annotation.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 19:27:53.923323 anutils-0.4.3b1/src/anutils/scutils/data/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       39 2023-05-11 06:31:57.000000 anutils-0.4.3b1/src/anutils/scutils/data/__init__.py
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     3942 2023-05-11 06:33:02.000000 anutils-0.4.3b1/src/anutils/scutils/data/data.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1539 2023-04-18 21:48:37.000000 anutils-0.4.3b1/src/anutils/scutils/data/h5ad2mtx.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1211 2023-04-10 19:26:07.000000 anutils-0.4.3b1/src/anutils/scutils/data/mtx2rds.R
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 19:27:53.923323 anutils-0.4.3b1/src/anutils/scutils/external/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       68 2023-05-11 06:31:45.000000 anutils-0.4.3b1/src/anutils/scutils/external/__init__.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 19:27:53.923323 anutils-0.4.3b1/src/anutils/scutils/external/integration/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      297 2023-05-11 14:19:55.000000 anutils-0.4.3b1/src/anutils/scutils/external/integration/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1707 2023-05-05 18:26:12.000000 anutils-0.4.3b1/src/anutils/scutils/external/integration/harmony.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2809 2023-04-20 06:33:17.000000 anutils-0.4.3b1/src/anutils/scutils/external/integration/harmony_matrix.R
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      577 2023-05-06 07:55:23.000000 anutils-0.4.3b1/src/anutils/scutils/external/integration/integration.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     3414 2023-05-11 14:37:17.000000 anutils-0.4.3b1/src/anutils/scutils/external/integration/scalex.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2187 2023-05-06 07:55:52.000000 anutils-0.4.3b1/src/anutils/scutils/external/integration/scvi.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4242 2023-05-09 06:26:37.000000 anutils-0.4.3b1/src/anutils/scutils/external/integration/seurat.R
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1578 2023-05-06 07:50:07.000000 anutils-0.4.3b1/src/anutils/scutils/external/integration/seurat.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    17278 2023-05-12 08:10:32.000000 anutils-0.4.3b1/src/anutils/scutils/plotting.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     7833 2023-05-05 13:05:09.000000 anutils-0.4.3b1/src/anutils/scutils/preprocessing.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 19:27:53.919323 anutils-0.4.3b1/src/anutils/scutils/resources/
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 19:27:53.923323 anutils-0.4.3b1/src/anutils/scutils/resources/gene_sets/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      556 2023-05-12 15:00:19.000000 anutils-0.4.3b1/src/anutils/scutils/resources/gene_sets/regev_lab_cell_cycle_genes.txt
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 19:27:53.923323 anutils-0.4.3b1/src/anutils/scutils/sc_cuda/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      116 2023-05-11 06:30:39.000000 anutils-0.4.3b1/src/anutils/scutils/sc_cuda/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    29119 2023-04-20 13:48:41.000000 anutils-0.4.3b1/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2503 2023-04-20 13:50:49.000000 anutils-0.4.3b1/src/anutils/scutils/sc_cuda/scanpy_cuda.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4564 2023-03-12 12:33:33.000000 anutils-0.4.3b1/src/anutils/scutils/sc_cuda/scib_cuda.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1229 2023-05-11 02:41:54.000000 anutils-0.4.3b1/src/anutils/scutils/utils.py
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)    10582 2023-05-04 16:21:28.000000 anutils-0.4.3b1/src/anutils/utils.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 19:27:53.919323 anutils-0.4.3b1/src/anutils.egg-info/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2865 2023-05-12 19:27:53.000000 anutils-0.4.3b1/src/anutils.egg-info/PKG-INFO
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1369 2023-05-12 19:27:53.000000 anutils-0.4.3b1/src/anutils.egg-info/SOURCES.txt
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)        1 2023-05-12 19:27:53.000000 anutils-0.4.3b1/src/anutils.egg-info/dependency_links.txt
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)       73 2023-05-12 19:27:53.000000 anutils-0.4.3b1/src/anutils.egg-info/requires.txt
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)        8 2023-05-12 19:27:53.000000 anutils-0.4.3b1/src/anutils.egg-info/top_level.txt
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 19:27:53.923323 anutils-0.4.3b1/tests/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)      581 2022-06-17 11:20:29.000000 anutils-0.4.3b1/tests/run_tests.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.812678 anutils-0.4.4/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1799 2022-06-15 05:53:11.000000 anutils-0.4.4/.gitignore
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2863 2023-05-14 18:24:37.812678 anutils-0.4.4/PKG-INFO
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2372 2023-05-07 16:11:39.000000 anutils-0.4.4/README.md
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       38 2023-05-14 18:24:37.812678 anutils-0.4.4/setup.cfg
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)      901 2023-05-14 18:24:05.000000 anutils-0.4.4/setup.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)       43 2023-05-14 06:23:19.000000 anutils-0.4.4/src/anutils/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      556 2023-05-14 06:17:33.000000 anutils-0.4.4/src/anutils/exceptions.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils/mlutils/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)       38 2023-05-11 06:32:55.000000 anutils-0.4.4/src/anutils/mlutils/__init__.py
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2498 2023-05-11 06:32:47.000000 anutils-0.4.4/src/anutils/mlutils/mlutils.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils/scutils/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)      215 2023-05-14 06:31:30.000000 anutils-0.4.4/src/anutils/scutils/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     7738 2023-05-14 06:11:56.000000 anutils-0.4.4/src/anutils/scutils/annotation.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils/scutils/data/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       39 2023-05-11 06:31:57.000000 anutils-0.4.4/src/anutils/scutils/data/__init__.py
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     3942 2023-05-11 06:33:02.000000 anutils-0.4.4/src/anutils/scutils/data/data.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1539 2023-04-18 21:48:37.000000 anutils-0.4.4/src/anutils/scutils/data/h5ad2mtx.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1211 2023-04-10 19:26:07.000000 anutils-0.4.4/src/anutils/scutils/data/mtx2rds.R
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils/scutils/external/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       68 2023-05-11 06:31:45.000000 anutils-0.4.4/src/anutils/scutils/external/__init__.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.812678 anutils-0.4.4/src/anutils/scutils/external/integration/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      297 2023-05-11 14:19:55.000000 anutils-0.4.4/src/anutils/scutils/external/integration/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1707 2023-05-05 18:26:12.000000 anutils-0.4.4/src/anutils/scutils/external/integration/harmony.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2809 2023-04-20 06:33:17.000000 anutils-0.4.4/src/anutils/scutils/external/integration/harmony_matrix.R
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      577 2023-05-06 07:55:23.000000 anutils-0.4.4/src/anutils/scutils/external/integration/integration.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     3414 2023-05-11 14:37:17.000000 anutils-0.4.4/src/anutils/scutils/external/integration/scalex.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2187 2023-05-06 07:55:52.000000 anutils-0.4.4/src/anutils/scutils/external/integration/scvi.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4242 2023-05-09 06:26:37.000000 anutils-0.4.4/src/anutils/scutils/external/integration/seurat.R
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1578 2023-05-06 07:50:07.000000 anutils-0.4.4/src/anutils/scutils/external/integration/seurat.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    17278 2023-05-12 08:10:32.000000 anutils-0.4.4/src/anutils/scutils/plotting.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     7833 2023-05-05 13:05:09.000000 anutils-0.4.4/src/anutils/scutils/preprocessing.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils/scutils/resources/
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.812678 anutils-0.4.4/src/anutils/scutils/resources/gene_sets/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      556 2023-05-12 15:00:19.000000 anutils-0.4.4/src/anutils/scutils/resources/gene_sets/regev_lab_cell_cycle_genes.txt
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.812678 anutils-0.4.4/src/anutils/scutils/sc_cuda/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      116 2023-05-11 06:30:39.000000 anutils-0.4.4/src/anutils/scutils/sc_cuda/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    29119 2023-04-20 13:48:41.000000 anutils-0.4.4/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2503 2023-04-20 13:50:49.000000 anutils-0.4.4/src/anutils/scutils/sc_cuda/scanpy_cuda.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4564 2023-03-12 12:33:33.000000 anutils-0.4.4/src/anutils/scutils/sc_cuda/scib_cuda.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       91 2023-05-14 05:41:26.000000 anutils-0.4.4/src/anutils/scutils/settings.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1229 2023-05-11 02:41:54.000000 anutils-0.4.4/src/anutils/scutils/utils.py
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)    10831 2023-05-14 06:13:42.000000 anutils-0.4.4/src/anutils/utils.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils.egg-info/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2863 2023-05-14 18:24:37.000000 anutils-0.4.4/src/anutils.egg-info/PKG-INFO
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1401 2023-05-14 18:24:37.000000 anutils-0.4.4/src/anutils.egg-info/SOURCES.txt
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)        1 2023-05-14 18:24:37.000000 anutils-0.4.4/src/anutils.egg-info/dependency_links.txt
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)       73 2023-05-14 18:24:37.000000 anutils-0.4.4/src/anutils.egg-info/requires.txt
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)        8 2023-05-14 18:24:37.000000 anutils-0.4.4/src/anutils.egg-info/top_level.txt
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.812678 anutils-0.4.4/tests/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)      581 2022-06-17 11:20:29.000000 anutils-0.4.4/tests/run_tests.py
```

### Comparing `anutils-0.4.3b1/.gitignore` & `anutils-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/PKG-INFO` & `anutils-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anutils
-Version: 0.4.3b1
+Version: 0.4.4
 Summary: ml and single cell utils.
 Home-page: https://github.com/AaronNing/anutils
 Author: Aaron Ning
 Author-email: aaronning98@gmail.com
 License: MIT
 Keywords: anutils
```

### Comparing `anutils-0.4.3b1/README.md` & `anutils-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/setup.py` & `anutils-0.4.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from pypandoc import convert_file
     long_description = convert_file('README.md', 'rst')
 except:
     long_description = ''
 
 setup(
     name='anutils',
-    version='0.4.3b1',
+    version='0.4.4',
     license='MIT',
     author="Aaron Ning",
     author_email='aaronning98@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
 
     # If any package contains *.r files, include them:
```

### Comparing `anutils-0.4.3b1/src/anutils/mlutils/mlutils.py` & `anutils-0.4.4/src/anutils/mlutils/mlutils.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/annotation.py` & `anutils-0.4.4/src/anutils/scutils/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os.path as osp
 
 import numpy as np
 import pandas as pd
 import scanpy as sc
 
 from anutils.exceptions import _deprecated
-from anutils.scutils import SCUTILS_RESOURCE_DIR
+from anutils.scutils.settings import SCUTILS_RESOURCE_DIR
 
 
 def infer_celltype_from_dotplot_object(dp: sc.pl.DotPlot):
     """
     params
     ---
     dp: `sc.pl.DotPlot` object
@@ -193,15 +193,15 @@
                                  **scanpy_score_genes_kwargs)
     return adata
 
 
 # ----------------- deprecated ----------------- #
 
 
-@_deprecated
+@_deprecated()
 def infer_celltype_from_scores(ad, markers, groupby, no_verbose=True):
     if no_verbose:
         verb = sc.settings.verbosity
         sc.settings.verbosity = 0
     markers = get_marker_genes(markers, ad)
     ad = ad.copy()
     cts = []
@@ -219,15 +219,15 @@
         columns=['anno',
                  groupby]).groupby('anno').apply(lambda df: df[groupby].to_list()).to_dict()
     if no_verbose:
         sc.settings.verbosity = verb
     return anno_dict
 
 
-@_deprecated
+@_deprecated()
 def score_celltypes_by_markers(adata, groupby, markers):
     """infer cell types from markers
 
     Parameters
     ----------
     adata : AnnData
         adata object.
@@ -239,15 +239,15 @@
     adata = adata.copy()
     for celltype, genes in markers.items():
         sc.tl.score_genes(adata, genes, score_name=celltype)
     scores = adata.obs.groupby(groupby)[list(markers.keys())].mean()
     return scores
 
 
-@_deprecated
+@_deprecated(message='use `infer_celltype_from_dotplot_object` instead')
 def infer_celltype_from_dotplot(adata, groupby, markers):
     """
     params
     ---
     markers: same as `var_names` in `sc.pl.DotPlot`. a `dict` of `celltype: gene list` pairs.
     
     returns
```

### Comparing `anutils-0.4.3b1/src/anutils/scutils/data/data.py` & `anutils-0.4.4/src/anutils/scutils/data/data.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/data/h5ad2mtx.py` & `anutils-0.4.4/src/anutils/scutils/data/h5ad2mtx.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/data/mtx2rds.R` & `anutils-0.4.4/src/anutils/scutils/data/mtx2rds.R`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/external/integration/harmony.py` & `anutils-0.4.4/src/anutils/scutils/external/integration/harmony.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/external/integration/harmony_matrix.R` & `anutils-0.4.4/src/anutils/scutils/external/integration/harmony_matrix.R`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/external/integration/integration.py` & `anutils-0.4.4/src/anutils/scutils/external/integration/integration.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/external/integration/scalex.py` & `anutils-0.4.4/src/anutils/scutils/external/integration/scalex.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/external/integration/scvi.py` & `anutils-0.4.4/src/anutils/scutils/external/integration/scvi.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/external/integration/seurat.R` & `anutils-0.4.4/src/anutils/scutils/external/integration/seurat.R`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/external/integration/seurat.py` & `anutils-0.4.4/src/anutils/scutils/external/integration/seurat.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/plotting.py` & `anutils-0.4.4/src/anutils/scutils/plotting.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/preprocessing.py` & `anutils-0.4.4/src/anutils/scutils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/resources/gene_sets/regev_lab_cell_cycle_genes.txt` & `anutils-0.4.4/src/anutils/scutils/resources/gene_sets/regev_lab_cell_cycle_genes.txt`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py` & `anutils-0.4.4/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/sc_cuda/scanpy_cuda.py` & `anutils-0.4.4/src/anutils/scutils/sc_cuda/scanpy_cuda.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/sc_cuda/scib_cuda.py` & `anutils-0.4.4/src/anutils/scutils/sc_cuda/scib_cuda.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/scutils/utils.py` & `anutils-0.4.4/src/anutils/scutils/utils.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.3b1/src/anutils/utils.py` & `anutils-0.4.4/src/anutils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,33 +10,15 @@
 import time
 import warnings
 from importlib import reload
 from types import ModuleType
 
 from getkey import getkey
 
-
-def rreload(module, max_depth, verbose=False, depth=0):
-    """Recursively reload modules.
-    
-    NOTE: IPython.lib.deepreload.reload() is similar.
-    """
-    for attribute_name in dir(module):
-        if not hasattr(module, attribute_name):
-            continue
-        attribute = getattr(module, attribute_name)
-        if type(attribute) is ModuleType:
-            if depth < max_depth:
-                rreload(attribute, max_depth, verbose=verbose, depth=depth + 1)
-    try:
-        reload(module)
-    except Exception as e:
-        if verbose:
-            print(f'Skip reloading `{module}`: {e}')
-        pass
+from anutils.exceptions import _deprecated
 
 
 def flatten(lst: list) -> list:
     r"""
     flattens a list of lists or tuples.
     """
     ret = []
@@ -112,14 +94,15 @@
 
         return wrapped
 
     return silencer
 
 
 class Silent():
+    """context manager to silent stdout or stderr."""
 
     def __init__(self, mode):
         if isinstance(mode, str):
             mode = [mode]
         for item in mode:
             assert item in ['stdout', 'stderr']
         self.mode = mode
@@ -155,44 +138,14 @@
             tmstr = ' '.join(['[' + str(datetime.datetime.now()) + ']', tmstr])
         print(tmstr)
         return ret
 
     return timed
 
 
-def logging_to(target_dir: str, need_timing_in_name: bool = False):
-    r"""log a function to a file.
-    """
-    assert os.path.isdir(target_dir)
-
-    def decorator(fn):
-
-        def logged_fn(*args, **kwargs):
-            if need_timing_in_name:
-                dt = datetime.datetime.now()
-                txt_path = os.path.join(
-                    target_dir,
-                    "log_{:d}_{:d}_{:d}_{:d}_{:d}_{:d}.txt".format(dt.year, dt.month, dt.day,
-                                                                   dt.hour, dt.minute,
-                                                                   dt.second))
-            else:
-                txt_path = os.path.join(target_dir, 'log.txt')
-
-            with open(txt_path, 'w', encoding='utf-8') as f:
-                old_stdout = sys.stdout
-                sys.stdout = f
-                ret = fn(*args, **kwargs)
-                sys.stdout = old_stdout
-            return ret
-
-        return logged_fn
-
-    return decorator
-
-
 def get_datetime_str() -> str:
     r"""get datetime str.
     """
     dt = datetime.datetime.now()
     dt_str = "{:d}_{:d}_{:d}_{:d}_{:d}_{:d}".format(dt.year, dt.month, dt.day, dt.hour,
                                                     dt.minute, dt.second)
     return dt_str
@@ -361,7 +314,62 @@
             return one * p
 
     return "".join(
         reversed([
             period(rev[i], chlist[i * 2 + 2], chlist[i * 2 + 1], chlist[i * 2])
             for i in range(0, len(rev))
         ]))
+
+
+# ----------------- deprecated ----------------- #
+
+
+@_deprecated("Use `IPython.lib.deepreload.reload()` instead.")
+def rreload(module, max_depth, verbose=False, depth=0):
+    """Recursively reload modules.
+    
+    NOTE: IPython.lib.deepreload.reload() is similar.
+    """
+    for attribute_name in dir(module):
+        if not hasattr(module, attribute_name):
+            continue
+        attribute = getattr(module, attribute_name)
+        if type(attribute) is ModuleType:
+            if depth < max_depth:
+                rreload(attribute, max_depth, verbose=verbose, depth=depth + 1)
+    try:
+        reload(module)
+    except Exception as e:
+        if verbose:
+            print(f'Skip reloading `{module}`: {e}')
+        pass
+
+
+@_deprecated("Use `Tee` instead.")
+def logging_to(target_dir: str, need_timing_in_name: bool = False):
+    r"""log a function to a file.
+    """
+    assert os.path.isdir(target_dir)
+
+    def decorator(fn):
+
+        def logged_fn(*args, **kwargs):
+            if need_timing_in_name:
+                dt = datetime.datetime.now()
+                txt_path = os.path.join(
+                    target_dir,
+                    "log_{:d}_{:d}_{:d}_{:d}_{:d}_{:d}.txt".format(dt.year, dt.month, dt.day,
+                                                                   dt.hour, dt.minute,
+                                                                   dt.second))
+            else:
+                txt_path = os.path.join(target_dir, 'log.txt')
+
+            with open(txt_path, 'w', encoding='utf-8') as f:
+                old_stdout = sys.stdout
+                sys.stdout = f
+                ret = fn(*args, **kwargs)
+                sys.stdout = old_stdout
+            return ret
+
+        return logged_fn
+
+    return decorator
```

### Comparing `anutils-0.4.3b1/src/anutils.egg-info/PKG-INFO` & `anutils-0.4.4/src/anutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anutils
-Version: 0.4.3b1
+Version: 0.4.4
 Summary: ml and single cell utils.
 Home-page: https://github.com/AaronNing/anutils
 Author: Aaron Ning
 Author-email: aaronning98@gmail.com
 License: MIT
 Keywords: anutils
```

### Comparing `anutils-0.4.3b1/src/anutils.egg-info/SOURCES.txt` & `anutils-0.4.4/src/anutils.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/anutils.egg-info/top_level.txt
 src/anutils/mlutils/__init__.py
 src/anutils/mlutils/mlutils.py
 src/anutils/scutils/__init__.py
 src/anutils/scutils/annotation.py
 src/anutils/scutils/plotting.py
 src/anutils/scutils/preprocessing.py
+src/anutils/scutils/settings.py
 src/anutils/scutils/utils.py
 src/anutils/scutils/data/__init__.py
 src/anutils/scutils/data/data.py
 src/anutils/scutils/data/h5ad2mtx.py
 src/anutils/scutils/data/mtx2rds.R
 src/anutils/scutils/external/__init__.py
 src/anutils/scutils/external/integration/__init__.py
```

### Comparing `anutils-0.4.3b1/tests/run_tests.py` & `anutils-0.4.4/tests/run_tests.py`

 * *Files identical despite different names*

