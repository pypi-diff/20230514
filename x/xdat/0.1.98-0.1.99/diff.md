# Comparing `tmp/xdat-0.1.98.tar.gz` & `tmp/xdat-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdat-0.1.98.tar", last modified: Wed Mar 22 15:14:55 2023, max compression
+gzip compressed data, was "xdat-0.1.99.tar", last modified: Thu Mar 23 09:48:01 2023, max compression
```

## Comparing `xdat-0.1.98.tar` & `xdat-0.1.99.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 ido       (1000) ido       (1000)        0 2023-03-22 15:14:55.662529 xdat-0.1.98/
--rw-rw-r--   0 ido       (1000) ido       (1000)      136 2023-03-22 15:06:51.000000 xdat-0.1.98/.gitignore
--rw-rw-r--   0 ido       (1000) ido       (1000)     1083 2021-12-07 04:44:41.000000 xdat-0.1.98/LICENSE
--rw-rw-r--   0 ido       (1000) ido       (1000)     1065 2023-03-22 15:14:55.662529 xdat-0.1.98/PKG-INFO
--rw-rw-r--   0 ido       (1000) ido       (1000)      488 2021-12-07 04:44:41.000000 xdat-0.1.98/README.md
--rwxrwxr-x   0 ido       (1000) ido       (1000)       94 2021-12-07 04:44:41.000000 xdat-0.1.98/publish.sh
--rw-rw-r--   0 ido       (1000) ido       (1000)       38 2023-03-22 15:14:55.662529 xdat-0.1.98/setup.cfg
--rw-rw-r--   0 ido       (1000) ido       (1000)     2512 2023-03-22 15:14:44.000000 xdat-0.1.98/setup.py
-drwxrwxr-x   0 ido       (1000) ido       (1000)        0 2023-03-22 15:14:55.658529 xdat-0.1.98/toy_data/
--rw-rw-r--   0 ido       (1000) ido       (1000)     4643 2022-11-30 19:37:07.000000 xdat-0.1.98/toy_data/loan_eligibility_play.py
--rw-rw-r--   0 ido       (1000) ido       (1000)    41983 2021-12-07 04:44:41.000000 xdat-0.1.98/toy_data/student-mat.csv
-drwxrwxr-x   0 ido       (1000) ido       (1000)        0 2023-03-22 15:14:55.662529 xdat-0.1.98/xdat/
--rw-rw-r--   0 ido       (1000) ido       (1000)     1083 2021-12-07 04:44:41.000000 xdat-0.1.98/xdat/LICENSE
--rw-rw-r--   0 ido       (1000) ido       (1000)      258 2021-12-07 04:44:41.000000 xdat-0.1.98/xdat/__init__.py
-drwxrwxr-x   0 ido       (1000) ido       (1000)        0 2023-03-22 15:14:55.662529 xdat-0.1.98/xdat/media/
--rw-rw-r--   0 ido       (1000) ido       (1000)   533031 2023-03-22 15:11:04.000000 xdat-0.1.98/xdat/media/default_theme.pptx
-drwxrwxr-x   0 ido       (1000) ido       (1000)        0 2023-03-22 15:14:55.662529 xdat-0.1.98/xdat/tests/
--rw-rw-r--   0 ido       (1000) ido       (1000)        0 2021-12-07 04:44:41.000000 xdat-0.1.98/xdat/tests/__init__.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     2627 2023-02-06 01:37:07.000000 xdat-0.1.98/xdat/tests/test_xagg.py
--rw-rw-r--   0 ido       (1000) ido       (1000)      393 2021-12-07 04:44:41.000000 xdat-0.1.98/xdat/tests/test_xnp.py
--rw-rw-r--   0 ido       (1000) ido       (1000)      822 2023-02-06 01:42:21.000000 xdat-0.1.98/xdat/tests/test_xpd.py
--rw-rw-r--   0 ido       (1000) ido       (1000)      493 2021-12-07 04:44:41.000000 xdat-0.1.98/xdat/tests/test_xplots.py
--rw-rw-r--   0 ido       (1000) ido       (1000)      741 2022-01-04 10:07:34.000000 xdat-0.1.98/xdat/tests/test_xstats.py
--rw-rw-r--   0 ido       (1000) ido       (1000)      530 2022-11-15 10:59:52.000000 xdat-0.1.98/xdat/x1d.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     2712 2023-03-07 15:36:42.000000 xdat-0.1.98/xdat/xagg.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     2058 2022-12-11 10:30:35.000000 xdat-0.1.98/xdat/xanvil.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     1630 2022-11-29 10:46:07.000000 xdat-0.1.98/xdat/xbaikal.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     2809 2023-02-21 13:36:16.000000 xdat-0.1.98/xdat/xcache.py
--rw-rw-r--   0 ido       (1000) ido       (1000)      316 2022-11-13 19:42:32.000000 xdat-0.1.98/xdat/xcalc.py
--rw-rw-r--   0 ido       (1000) ido       (1000)      790 2022-08-20 13:23:41.000000 xdat-0.1.98/xdat/xchecks.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     3620 2023-03-22 08:42:16.000000 xdat-0.1.98/xdat/xdata.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     5610 2022-11-23 11:56:13.000000 xdat-0.1.98/xdat/xeda.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     1860 2021-12-07 04:44:41.000000 xdat-0.1.98/xdat/xexamine_data.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     1433 2022-05-11 07:54:56.000000 xdat-0.1.98/xdat/xfactors.py
--rw-rw-r--   0 ido       (1000) ido       (1000)      686 2022-12-20 14:40:47.000000 xdat-0.1.98/xdat/xincludes.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     2036 2022-11-30 16:10:25.000000 xdat-0.1.98/xdat/xmodels.py
--rw-rw-r--   0 ido       (1000) ido       (1000)      415 2021-12-07 04:44:41.000000 xdat-0.1.98/xdat/xmunge.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     1272 2023-01-26 10:34:35.000000 xdat-0.1.98/xdat/xnp.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     1883 2023-03-07 13:46:02.000000 xdat-0.1.98/xdat/xparallel.py
--rw-rw-r--   0 ido       (1000) ido       (1000)    20795 2023-02-21 14:14:48.000000 xdat-0.1.98/xdat/xpd.py
--rw-rw-r--   0 ido       (1000) ido       (1000)    27008 2023-03-22 10:49:49.000000 xdat-0.1.98/xdat/xplots.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     4973 2022-09-28 07:00:42.000000 xdat-0.1.98/xdat/xplt.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     5655 2023-03-15 11:10:55.000000 xdat-0.1.98/xdat/xpptx.py
--rw-rw-r--   0 ido       (1000) ido       (1000)    11284 2023-02-07 18:53:02.000000 xdat-0.1.98/xdat/xproblem.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     2646 2023-02-12 11:48:31.000000 xdat-0.1.98/xdat/xsettings.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     1139 2022-01-25 13:04:45.000000 xdat-0.1.98/xdat/xstan.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     3531 2023-02-09 16:40:01.000000 xdat-0.1.98/xdat/xstats.py
--rw-rw-r--   0 ido       (1000) ido       (1000)      391 2023-02-21 10:42:51.000000 xdat-0.1.98/xdat/xutils.py
--rw-rw-r--   0 ido       (1000) ido       (1000)     5752 2022-11-30 19:02:09.000000 xdat-0.1.98/xdat/xweights.py
-drwxrwxr-x   0 ido       (1000) ido       (1000)        0 2023-03-22 15:14:55.662529 xdat-0.1.98/xdat.egg-info/
--rw-rw-r--   0 ido       (1000) ido       (1000)     1065 2023-03-22 15:14:55.000000 xdat-0.1.98/xdat.egg-info/PKG-INFO
--rw-rw-r--   0 ido       (1000) ido       (1000)      847 2023-03-22 15:14:55.000000 xdat-0.1.98/xdat.egg-info/SOURCES.txt
--rw-rw-r--   0 ido       (1000) ido       (1000)        1 2023-03-22 15:14:55.000000 xdat-0.1.98/xdat.egg-info/dependency_links.txt
--rw-rw-r--   0 ido       (1000) ido       (1000)      320 2023-03-22 15:14:55.000000 xdat-0.1.98/xdat.egg-info/requires.txt
--rw-rw-r--   0 ido       (1000) ido       (1000)        5 2023-03-22 15:14:55.000000 xdat-0.1.98/xdat.egg-info/top_level.txt
+drwxrwxr-x   0 ido       (1000) ido       (1000)        0 2023-03-23 09:48:01.677013 xdat-0.1.99/
+-rw-rw-r--   0 ido       (1000) ido       (1000)      136 2023-03-22 15:06:51.000000 xdat-0.1.99/.gitignore
+-rw-rw-r--   0 ido       (1000) ido       (1000)     1083 2021-12-07 04:44:41.000000 xdat-0.1.99/LICENSE
+-rw-rw-r--   0 ido       (1000) ido       (1000)     1065 2023-03-23 09:48:01.677013 xdat-0.1.99/PKG-INFO
+-rw-rw-r--   0 ido       (1000) ido       (1000)      488 2021-12-07 04:44:41.000000 xdat-0.1.99/README.md
+-rwxrwxr-x   0 ido       (1000) ido       (1000)       94 2021-12-07 04:44:41.000000 xdat-0.1.99/publish.sh
+-rw-rw-r--   0 ido       (1000) ido       (1000)       38 2023-03-23 09:48:01.677013 xdat-0.1.99/setup.cfg
+-rw-rw-r--   0 ido       (1000) ido       (1000)     2512 2023-03-23 09:47:36.000000 xdat-0.1.99/setup.py
+drwxrwxr-x   0 ido       (1000) ido       (1000)        0 2023-03-23 09:48:01.669013 xdat-0.1.99/toy_data/
+-rw-rw-r--   0 ido       (1000) ido       (1000)     4643 2022-11-30 19:37:07.000000 xdat-0.1.99/toy_data/loan_eligibility_play.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)    41983 2021-12-07 04:44:41.000000 xdat-0.1.99/toy_data/student-mat.csv
+drwxrwxr-x   0 ido       (1000) ido       (1000)        0 2023-03-23 09:48:01.673013 xdat-0.1.99/xdat/
+-rw-rw-r--   0 ido       (1000) ido       (1000)     1083 2021-12-07 04:44:41.000000 xdat-0.1.99/xdat/LICENSE
+-rw-rw-r--   0 ido       (1000) ido       (1000)      258 2021-12-07 04:44:41.000000 xdat-0.1.99/xdat/__init__.py
+drwxrwxr-x   0 ido       (1000) ido       (1000)        0 2023-03-23 09:48:01.673013 xdat-0.1.99/xdat/media/
+-rw-rw-r--   0 ido       (1000) ido       (1000)   533031 2023-03-22 15:11:04.000000 xdat-0.1.99/xdat/media/default_theme.pptx
+drwxrwxr-x   0 ido       (1000) ido       (1000)        0 2023-03-23 09:48:01.677013 xdat-0.1.99/xdat/tests/
+-rw-rw-r--   0 ido       (1000) ido       (1000)        0 2021-12-07 04:44:41.000000 xdat-0.1.99/xdat/tests/__init__.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     2627 2023-02-06 01:37:07.000000 xdat-0.1.99/xdat/tests/test_xagg.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)      393 2021-12-07 04:44:41.000000 xdat-0.1.99/xdat/tests/test_xnp.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)      822 2023-02-06 01:42:21.000000 xdat-0.1.99/xdat/tests/test_xpd.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)      493 2021-12-07 04:44:41.000000 xdat-0.1.99/xdat/tests/test_xplots.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)      741 2022-01-04 10:07:34.000000 xdat-0.1.99/xdat/tests/test_xstats.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)      530 2022-11-15 10:59:52.000000 xdat-0.1.99/xdat/x1d.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     2712 2023-03-07 15:36:42.000000 xdat-0.1.99/xdat/xagg.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     2058 2022-12-11 10:30:35.000000 xdat-0.1.99/xdat/xanvil.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     1630 2022-11-29 10:46:07.000000 xdat-0.1.99/xdat/xbaikal.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     2809 2023-02-21 13:36:16.000000 xdat-0.1.99/xdat/xcache.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)      316 2022-11-13 19:42:32.000000 xdat-0.1.99/xdat/xcalc.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)      790 2022-08-20 13:23:41.000000 xdat-0.1.99/xdat/xchecks.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     3620 2023-03-22 08:42:16.000000 xdat-0.1.99/xdat/xdata.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     5610 2022-11-23 11:56:13.000000 xdat-0.1.99/xdat/xeda.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     1860 2021-12-07 04:44:41.000000 xdat-0.1.99/xdat/xexamine_data.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     1433 2022-05-11 07:54:56.000000 xdat-0.1.99/xdat/xfactors.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)      686 2022-12-20 14:40:47.000000 xdat-0.1.99/xdat/xincludes.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     2036 2022-11-30 16:10:25.000000 xdat-0.1.99/xdat/xmodels.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)      415 2021-12-07 04:44:41.000000 xdat-0.1.99/xdat/xmunge.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     1272 2023-01-26 10:34:35.000000 xdat-0.1.99/xdat/xnp.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     1883 2023-03-07 13:46:02.000000 xdat-0.1.99/xdat/xparallel.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)    20795 2023-02-21 14:14:48.000000 xdat-0.1.99/xdat/xpd.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)    27780 2023-03-23 08:35:33.000000 xdat-0.1.99/xdat/xplots.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     4973 2022-09-28 07:00:42.000000 xdat-0.1.99/xdat/xplt.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     5655 2023-03-15 11:10:55.000000 xdat-0.1.99/xdat/xpptx.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)    11855 2023-03-23 08:24:53.000000 xdat-0.1.99/xdat/xproblem.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     2646 2023-02-12 11:48:31.000000 xdat-0.1.99/xdat/xsettings.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     1139 2022-01-25 13:04:45.000000 xdat-0.1.99/xdat/xstan.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     3531 2023-02-09 16:40:01.000000 xdat-0.1.99/xdat/xstats.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)      391 2023-02-21 10:42:51.000000 xdat-0.1.99/xdat/xutils.py
+-rw-rw-r--   0 ido       (1000) ido       (1000)     5752 2022-11-30 19:02:09.000000 xdat-0.1.99/xdat/xweights.py
+drwxrwxr-x   0 ido       (1000) ido       (1000)        0 2023-03-23 09:48:01.673013 xdat-0.1.99/xdat.egg-info/
+-rw-rw-r--   0 ido       (1000) ido       (1000)     1065 2023-03-23 09:48:01.000000 xdat-0.1.99/xdat.egg-info/PKG-INFO
+-rw-rw-r--   0 ido       (1000) ido       (1000)      847 2023-03-23 09:48:01.000000 xdat-0.1.99/xdat.egg-info/SOURCES.txt
+-rw-rw-r--   0 ido       (1000) ido       (1000)        1 2023-03-23 09:48:01.000000 xdat-0.1.99/xdat.egg-info/dependency_links.txt
+-rw-rw-r--   0 ido       (1000) ido       (1000)      320 2023-03-23 09:48:01.000000 xdat-0.1.99/xdat.egg-info/requires.txt
+-rw-rw-r--   0 ido       (1000) ido       (1000)        5 2023-03-23 09:48:01.000000 xdat-0.1.99/xdat.egg-info/top_level.txt
```

### Comparing `xdat-0.1.98/LICENSE` & `xdat-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/PKG-INFO` & `xdat-0.1.99/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdat
-Version: 0.1.98
+Version: 0.1.99
 Summary: eXtended Data Analysis Toolkit
 Home-page: https://bitbucket.org/hermetric/xdat/
 Author: Ido Carmi
 Author-email: ido@hermetric.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `xdat-0.1.98/setup.py` & `xdat-0.1.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='xdat',
-    version='0.1.98',
+    version='0.1.99',
     description='eXtended Data Analysis Toolkit',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://bitbucket.org/hermetric/xdat/',
     author='Ido Carmi',
     author_email='ido@hermetric.com',
     license='MIT',
```

### Comparing `xdat-0.1.98/toy_data/loan_eligibility_play.py` & `xdat-0.1.99/toy_data/loan_eligibility_play.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/toy_data/student-mat.csv` & `xdat-0.1.99/toy_data/student-mat.csv`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/LICENSE` & `xdat-0.1.99/xdat/LICENSE`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/media/default_theme.pptx` & `xdat-0.1.99/xdat/media/default_theme.pptx`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/tests/test_xagg.py` & `xdat-0.1.99/xdat/tests/test_xagg.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/tests/test_xpd.py` & `xdat-0.1.99/xdat/tests/test_xpd.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/tests/test_xstats.py` & `xdat-0.1.99/xdat/tests/test_xstats.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/x1d.py` & `xdat-0.1.99/xdat/x1d.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xagg.py` & `xdat-0.1.99/xdat/xagg.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xanvil.py` & `xdat-0.1.99/xdat/xanvil.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xbaikal.py` & `xdat-0.1.99/xdat/xbaikal.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xcache.py` & `xdat-0.1.99/xdat/xcache.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xchecks.py` & `xdat-0.1.99/xdat/xchecks.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xdata.py` & `xdat-0.1.99/xdat/xdata.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xeda.py` & `xdat-0.1.99/xdat/xeda.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xexamine_data.py` & `xdat-0.1.99/xdat/xexamine_data.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xfactors.py` & `xdat-0.1.99/xdat/xfactors.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xincludes.py` & `xdat-0.1.99/xdat/xincludes.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xmodels.py` & `xdat-0.1.99/xdat/xmodels.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xnp.py` & `xdat-0.1.99/xdat/xnp.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xparallel.py` & `xdat-0.1.99/xdat/xparallel.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xpd.py` & `xdat-0.1.99/xdat/xpd.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xplots.py` & `xdat-0.1.99/xdat/xplots.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,22 +403,24 @@
     if legend:
         plt.legend(loc=legend_loc)
 
     if show:
         plt.show()
 
 
-def plot_multi(df, kind=None, plot_func=None, x=None, y=None, plot_on=None, group_on=None, color_on=None, cmap=None, label_on=None, style_on=None, size_on=None, figsize=(10,6), alpha=1.0, hdi_probs=(0.1, 0.25, 0.5, 0.8, 0.999), kde_cov=0.25, kde_percentile=None, hist_calc='perc', hist_type='step', hist_bins=10, hist_range=None, color_dict=None, title='', x_axis_type=None, y_axis_type=None, x_axis_fmt=None, y_axis_fmt=None, legend_loc='best', xlim=None, ylim=None, save_to=None, clear_folder=False, add_date=True, plot_decorate_func=None, drop_na=True, as_xpptx=None, desc='', show=True, **kwargs):
+def plot_multi(df, kind=None, plot_func=None, x=None, y=None, var_name='variable', value_name='value', plot_on=None, group_on=None, color_on=None, cmap=None, label_on=None, style_on=None, size_on=None, figsize=(10,6), alpha=1.0, hdi_probs=(0.1, 0.25, 0.5, 0.8, 0.999), kde_cov=0.25, kde_percentile=None, hist_calc='perc', hist_type='step', hist_bins=10, hist_range=None, color_dict=None, title='', x_axis_type=None, y_axis_type=None, x_axis_fmt=None, y_axis_fmt=None, legend_loc='best', xlim=None, ylim=None, save_to=None, clear_folder=False, add_date=True, plot_decorate_func=None, drop_na=True, as_xpptx=None, desc='', show=True, **kwargs):
     """
 
     :param df: input dataframe
     :param kind: type of plot ('scatter', 'line', 'hdi', '%', 'kde', 'hist')
     :param plot_func: alternative to *kind*, can provide a custom function that takes a subset of data & plots
     :param x: name of column for x-axis
-    :param y: name of column for y-axis
+    :param y: name of column for y-axis (can be iterable)
+    :param var_name: in case y is a list
+    :param value_name: in case y is a list
     :param plot_on: column name that generates different plot for each unique value
     :param group_on: column name for different subgroup of data (usually not neaded if provide color_on, etc)
     :param color_on: column name for different colors
     :param cmap: (optional) name of colormap to use, eg 'plasma'
     :param label_on: column name for different labels
     :param style_on: column name for different styles
     :param figsize:
@@ -448,14 +450,29 @@
 
     if as_xpptx and as_xpptx.fake:
         as_xpptx = None
 
     if kind is None and plot_func is None:
         kind = 'scatter'
 
+    if isinstance(y, list) or isinstance(y, tuple):
+        if len(y) == 1:
+            y = y[0]
+        else:
+            id_vars = {x, color_on, group_on, plot_on, label_on, size_on, style_on}
+            id_vars = [i for i in id_vars if i]
+            df = pd.melt(df, id_vars=id_vars, value_vars=y, var_name=var_name, value_name=value_name)
+            y = value_name
+            if color_on is None:
+                color_on = var_name
+            elif style_on is None:
+                style_on = var_name
+            else:
+                raise ValueError("if y is a list, then either color_on or style_on must be None")
+
     if kind in ['percentiles', 'percentile', 'percent', 'perc']:
         kind = '%'
 
     if x is None and y is None:
         raise TypeError('Missing required keyword argument: x or y')
 
     if save_to:
```

### Comparing `xdat-0.1.98/xdat/xplt.py` & `xdat-0.1.99/xdat/xplt.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xpptx.py` & `xdat-0.1.99/xdat/xpptx.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xproblem.py` & `xdat-0.1.99/xdat/xproblem.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,17 @@
         yield CVSplit(df_train=df_train, df_test=df_test, df_val=df_val)
 
 
 CVFold = namedtuple("CVFold", ['clf', 'df_train', 'df_test', 'feature_names', 'df_val'])
 
 
 def train_cv(df, target_col, clf, n_splits=12, stratify_on=None, group_on=None, ordered_split=False, del_cols=tuple(), uid_col=None, sample_weight_col=None, eval_size=0.0, eval_type=None, fit_params=None, with_tqdm=True, n_jobs=1):
+    # fix feature names...
+    df.columns = [str(c) if isinstance(c, str) else c for c in df.columns]
+
     if eval_size:
         assert eval_type in ['lightgbm'], "need to specify proper eval_type param"
     else:
         eval_type = None
 
     fit_params = dict() if fit_params is None else fit_params
 
@@ -243,36 +246,50 @@
             rows.append(fi_dict)
 
     df = pd.DataFrame(rows)
     return df
 
 
 class ModelEnsemble:
-    def __init__(self, clfs):
+    def __init__(self, clfs, is_binary=True):
+        self.is_binary = is_binary
         self.clfs = clfs
+        self.feature_names = self.clfs[0].feature_names_in_
 
     @classmethod
-    def from_all_folds(cls, all_folds):
+    def from_all_folds(cls, all_folds, is_binary=True):
         clfs = [f.clf for f in all_folds]
-        return cls(clfs)
+        return cls(clfs, is_binary=is_binary)
+
+    def prepare_X(self, df):
+        df = df[self.feature_names].copy()
+        df.columns = [str(c) if isinstance(c, str) else c for c in df.columns]
+        return df
 
     def predict(self, X):
+        X = self.prepare_X(X)
         all_y = [clf.predict(X) for clf in self.clfs]
         all_y = [y.reshape(y.shape + (1,)) for y in all_y]
         Y = np.concatenate(all_y, axis=1)
-        pred = [np.bincount(y).argmax() for y in Y]
+
+        if self.is_binary:
+            pred = [np.bincount(y).argmax() for y in Y]
+        else:
+            pred = [np.mean(y) for y in Y]
+
         pred = np.array(pred)
         return pred
 
     def predict_binary(self, X, threshold=0.5):
         prob_1 = self.predict_proba(X)[:, 1]
         pred = prob_1 >= threshold
         return pred.astype(int)
 
     def predict_proba(self, X):
+        X = self.prepare_X(X)
         all_y = [clf.predict_proba(X) for clf in self.clfs]
         all_y = [y.reshape(y.shape + (1,)) for y in all_y]
         y = np.concatenate(all_y, axis=2)
         proba = y.mean(axis=2)
         return proba
```

### Comparing `xdat-0.1.98/xdat/xsettings.py` & `xdat-0.1.99/xdat/xsettings.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xstan.py` & `xdat-0.1.99/xdat/xstan.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xstats.py` & `xdat-0.1.99/xdat/xstats.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat/xweights.py` & `xdat-0.1.99/xdat/xweights.py`

 * *Files identical despite different names*

### Comparing `xdat-0.1.98/xdat.egg-info/PKG-INFO` & `xdat-0.1.99/xdat.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdat
-Version: 0.1.98
+Version: 0.1.99
 Summary: eXtended Data Analysis Toolkit
 Home-page: https://bitbucket.org/hermetric/xdat/
 Author: Ido Carmi
 Author-email: ido@hermetric.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `xdat-0.1.98/xdat.egg-info/SOURCES.txt` & `xdat-0.1.99/xdat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

