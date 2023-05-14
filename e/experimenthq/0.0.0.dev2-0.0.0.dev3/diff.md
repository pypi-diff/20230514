# Comparing `tmp/experimenthq-0.0.0.dev2.tar.gz` & `tmp/experimenthq-0.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experimenthq-0.0.0.dev2.tar", last modified: Sun May 14 20:17:19 2023, max compression
+gzip compressed data, was "experimenthq-0.0.0.dev3.tar", last modified: Sun May 14 20:27:11 2023, max compression
```

## Comparing `experimenthq-0.0.0.dev2.tar` & `experimenthq-0.0.0.dev3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-14 20:17:19.309893 experimenthq-0.0.0.dev2/
--rw-r--r--   0 ramonabendias   (501) staff       (20)     1071 2023-04-28 20:27:57.000000 experimenthq-0.0.0.dev2/LICENSE
--rw-r--r--   0 ramonabendias   (501) staff       (20)     3926 2023-05-14 20:17:19.310003 experimenthq-0.0.0.dev2/PKG-INFO
--rw-r--r--   0 ramonabendias   (501) staff       (20)     2318 2023-05-14 20:16:07.000000 experimenthq-0.0.0.dev2/README.md
--rw-r--r--   0 ramonabendias   (501) staff       (20)      983 2023-05-14 20:17:19.310351 experimenthq-0.0.0.dev2/setup.cfg
--rw-r--r--   0 ramonabendias   (501) staff       (20)     3501 2023-05-14 19:42:35.000000 experimenthq-0.0.0.dev2/setup.py
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-14 20:17:19.307165 experimenthq-0.0.0.dev2/src/
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-14 20:17:19.308608 experimenthq-0.0.0.dev2/src/experimenthq/
--rw-r--r--   0 ramonabendias   (501) staff       (20)      148 2023-05-14 19:40:55.000000 experimenthq-0.0.0.dev2/src/experimenthq/__init__.py
--rw-r--r--   0 ramonabendias   (501) staff       (20)      129 2023-05-14 20:16:57.000000 experimenthq-0.0.0.dev2/src/experimenthq/_about.py
--rw-r--r--   0 ramonabendias   (501) staff       (20)     2192 2023-05-10 21:14:32.000000 experimenthq-0.0.0.dev2/src/experimenthq/experiment.py
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-14 20:17:19.309751 experimenthq-0.0.0.dev2/src/experimenthq.egg-info/
--rw-r--r--   0 ramonabendias   (501) staff       (20)     3926 2023-05-14 20:17:19.000000 experimenthq-0.0.0.dev2/src/experimenthq.egg-info/PKG-INFO
--rw-r--r--   0 ramonabendias   (501) staff       (20)      361 2023-05-14 20:17:19.000000 experimenthq-0.0.0.dev2/src/experimenthq.egg-info/SOURCES.txt
--rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-14 20:17:19.000000 experimenthq-0.0.0.dev2/src/experimenthq.egg-info/dependency_links.txt
--rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-06 11:57:37.000000 experimenthq-0.0.0.dev2/src/experimenthq.egg-info/not-zip-safe
--rw-r--r--   0 ramonabendias   (501) staff       (20)      126 2023-05-14 20:17:19.000000 experimenthq-0.0.0.dev2/src/experimenthq.egg-info/requires.txt
--rw-r--r--   0 ramonabendias   (501) staff       (20)       13 2023-05-14 20:17:19.000000 experimenthq-0.0.0.dev2/src/experimenthq.egg-info/top_level.txt
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-14 20:27:11.906046 experimenthq-0.0.0.dev3/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     1071 2023-04-28 20:27:57.000000 experimenthq-0.0.0.dev3/LICENSE
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     3991 2023-05-14 20:27:11.906144 experimenthq-0.0.0.dev3/PKG-INFO
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     2383 2023-05-14 20:21:42.000000 experimenthq-0.0.0.dev3/README.md
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      983 2023-05-14 20:27:11.906506 experimenthq-0.0.0.dev3/setup.cfg
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     3501 2023-05-14 19:42:35.000000 experimenthq-0.0.0.dev3/setup.py
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-14 20:27:11.902568 experimenthq-0.0.0.dev3/src/
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-14 20:27:11.904640 experimenthq-0.0.0.dev3/src/experimenthq/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      148 2023-05-14 19:40:55.000000 experimenthq-0.0.0.dev3/src/experimenthq/__init__.py
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      129 2023-05-14 20:26:56.000000 experimenthq-0.0.0.dev3/src/experimenthq/_about.py
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     2192 2023-05-10 21:14:32.000000 experimenthq-0.0.0.dev3/src/experimenthq/experiment.py
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-14 20:27:11.905908 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     3991 2023-05-14 20:27:11.000000 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/PKG-INFO
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      361 2023-05-14 20:27:11.000000 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/SOURCES.txt
+-rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-14 20:27:11.000000 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/dependency_links.txt
+-rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-06 11:57:37.000000 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/not-zip-safe
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      126 2023-05-14 20:27:11.000000 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/requires.txt
+-rw-r--r--   0 ramonabendias   (501) staff       (20)       13 2023-05-14 20:27:11.000000 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/top_level.txt
```

### Comparing `experimenthq-0.0.0.dev2/LICENSE` & `experimenthq-0.0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev2/PKG-INFO` & `experimenthq-0.0.0.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experimenthq
-Version: 0.0.0.dev2
+Version: 0.0.0.dev3
 Summary: A Python package for tracking experiments in Notion
 Home-page: https://github.com/EperimentHQ/experiment-hq
 Author: 
 Author-email: 
 License: MIT
 Project-URL: Changelog, https://github.com/EperimentHQ/experiment-hq/releases
 Project-URL: Issue Tracker, https://github.com/EperimentHQ/experiment-hq/issues
@@ -35,15 +35,15 @@
 
 
 
 <div align="center">
 
 
 
-<img src="https://www.experiment-hq.com/_next/image?url=%2Flogo.ico&w=3840&q=75"  width="15%" class="center" >
+<img src="https://www.experiment-hq.com/_next/image?url=%2Flogo.png&w=3840&q=75"  width="15%" class="center" >
 
 # ExperimentHQ
 
 </div>
 
 
 ExperimentHQ is a Python package that allows you to track and manage experiments directly from your Python code, and seamlessly sync the results to a Notion database. With ExperimentHQ, you can easily monitor the performance of your models, log custom metrics, and compare experiments with ease, all from a single, intuitive interface.
@@ -89,11 +89,11 @@
 
 This code creates an experiment with the name "My First Experiment" and tags it with the project "Project A". It then logs two parameters, "accuracy" and "loss", with values 0.85 and 0.05 respectively.
 
 ### Viewing Experiments in Notion
 
 To view the experiments that you've logged with ExperimentHQ in Notion go to the Notion page that you've linked to ExperimentHQ. You should see a table with the experiments that you've logged.
 
-![Notion Table](notion_table.png)
+![Notion Table](https://www.experiment-hq.com/_next/image?url=%2Fnotion_dashboard.png&w=3840&q=75)
 
 ## Conclusion
 ExperimentHQ provides a simple and intuitive way to track and manage your experiments in Python and sync the results to Notion. By using ExperimentHQ, you can streamline your experiment tracking and make your work more efficient and effective. Try it out today and see the difference it can make in your workflow!
```

### Comparing `experimenthq-0.0.0.dev2/README.md` & `experimenthq-0.0.0.dev3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 
 <div align="center">
 
 
 
-<img src="https://www.experiment-hq.com/_next/image?url=%2Flogo.ico&w=3840&q=75"  width="15%" class="center" >
+<img src="https://www.experiment-hq.com/_next/image?url=%2Flogo.png&w=3840&q=75"  width="15%" class="center" >
 
 # ExperimentHQ
 
 </div>
 
 
 ExperimentHQ is a Python package that allows you to track and manage experiments directly from your Python code, and seamlessly sync the results to a Notion database. With ExperimentHQ, you can easily monitor the performance of your models, log custom metrics, and compare experiments with ease, all from a single, intuitive interface.
@@ -55,11 +55,11 @@
 
 This code creates an experiment with the name "My First Experiment" and tags it with the project "Project A". It then logs two parameters, "accuracy" and "loss", with values 0.85 and 0.05 respectively.
 
 ### Viewing Experiments in Notion
 
 To view the experiments that you've logged with ExperimentHQ in Notion go to the Notion page that you've linked to ExperimentHQ. You should see a table with the experiments that you've logged.
 
-![Notion Table](notion_table.png)
+![Notion Table](https://www.experiment-hq.com/_next/image?url=%2Fnotion_dashboard.png&w=3840&q=75)
 
 ## Conclusion
 ExperimentHQ provides a simple and intuitive way to track and manage your experiments in Python and sync the results to Notion. By using ExperimentHQ, you can streamline your experiment tracking and make your work more efficient and effective. Try it out today and see the difference it can make in your workflow!
```

### Comparing `experimenthq-0.0.0.dev2/setup.cfg` & `experimenthq-0.0.0.dev3/setup.cfg`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev2/setup.py` & `experimenthq-0.0.0.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev2/src/experimenthq/experiment.py` & `experimenthq-0.0.0.dev3/src/experimenthq/experiment.py`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev2/src/experimenthq.egg-info/PKG-INFO` & `experimenthq-0.0.0.dev3/src/experimenthq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experimenthq
-Version: 0.0.0.dev2
+Version: 0.0.0.dev3
 Summary: A Python package for tracking experiments in Notion
 Home-page: https://github.com/EperimentHQ/experiment-hq
 Author: 
 Author-email: 
 License: MIT
 Project-URL: Changelog, https://github.com/EperimentHQ/experiment-hq/releases
 Project-URL: Issue Tracker, https://github.com/EperimentHQ/experiment-hq/issues
@@ -35,15 +35,15 @@
 
 
 
 <div align="center">
 
 
 
-<img src="https://www.experiment-hq.com/_next/image?url=%2Flogo.ico&w=3840&q=75"  width="15%" class="center" >
+<img src="https://www.experiment-hq.com/_next/image?url=%2Flogo.png&w=3840&q=75"  width="15%" class="center" >
 
 # ExperimentHQ
 
 </div>
 
 
 ExperimentHQ is a Python package that allows you to track and manage experiments directly from your Python code, and seamlessly sync the results to a Notion database. With ExperimentHQ, you can easily monitor the performance of your models, log custom metrics, and compare experiments with ease, all from a single, intuitive interface.
@@ -89,11 +89,11 @@
 
 This code creates an experiment with the name "My First Experiment" and tags it with the project "Project A". It then logs two parameters, "accuracy" and "loss", with values 0.85 and 0.05 respectively.
 
 ### Viewing Experiments in Notion
 
 To view the experiments that you've logged with ExperimentHQ in Notion go to the Notion page that you've linked to ExperimentHQ. You should see a table with the experiments that you've logged.
 
-![Notion Table](notion_table.png)
+![Notion Table](https://www.experiment-hq.com/_next/image?url=%2Fnotion_dashboard.png&w=3840&q=75)
 
 ## Conclusion
 ExperimentHQ provides a simple and intuitive way to track and manage your experiments in Python and sync the results to Notion. By using ExperimentHQ, you can streamline your experiment tracking and make your work more efficient and effective. Try it out today and see the difference it can make in your workflow!
```

