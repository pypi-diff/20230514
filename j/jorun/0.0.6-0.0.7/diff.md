# Comparing `tmp/jorun-0.0.6.tar.gz` & `tmp/jorun-0.0.7.tar.gz`

## Comparing `jorun-0.0.6.tar` & `jorun-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,13 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jorun-0.0.6/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jorun-0.0.6/.idea/misc.xml
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 jorun-0.0.6/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jorun-0.0.6/.idea/runsk.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jorun-0.0.6/.idea/vcs.xml
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 jorun-0.0.6/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jorun-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.0.6/src/jorun/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jorun-0.0.6/src/jorun/configuration.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 jorun-0.0.6/src/jorun/logger.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 jorun-0.0.6/src/jorun/main.py
--rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 jorun-0.0.6/src/jorun/runner.py
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 jorun-0.0.6/src/jorun/runner_threading.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 jorun-0.0.6/src/jorun/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 jorun-0.0.6/.gitignore
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 jorun-0.0.6/README.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 jorun-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 jorun-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/configuration.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/logger.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/main.py
+-rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/runner.py
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/runner_threading.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jorun-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jorun-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 jorun-0.0.7/README.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jorun-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 jorun-0.0.7/PKG-INFO
```

### Comparing `jorun-0.0.6/src/jorun/main.py` & `jorun-0.0.7/src/jorun/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 #!/usr/bin/env python
 import argparse
 import time
+from threading import Lock
 from typing import List
 
 from .configuration import load_config
 from .runner_threading import TaskRunner
 from .task import build_task_tree, TaskNode
 from .logger import logger, subprocess_logger
 
 parser = argparse.ArgumentParser(prog="jorun", description="A smart task runner", add_help=True)
 
 parser.add_argument("configuration_file", help="The yml configuration file to run")
 parser.add_argument("--level", help="The log level (DEBUG, INFO, ...)", default="INFO", type=str)
 
 running_tasks: List[TaskRunner] = []
+running_tasks_lock = Lock()
 
 
 def run_task(task: TaskNode):
     t = TaskRunner(task)
-    running_tasks.append(t)
+
+    with running_tasks_lock:
+        running_tasks.append(t)
 
     def cb():
         logger.debug(f"Task {task.task['name']} completed")
 
         if len(task.dependencies) > 0:
             logger.debug(f"Launching task {task.task['name']} dependencies")
             for dep in task.dependencies:
@@ -46,13 +50,16 @@
 
     run_task(dep_tree)
 
     try:
         while True:
             time.sleep(1)
     except KeyboardInterrupt:
-        for t in running_tasks:
-            t.stop()
+        with running_tasks_lock:
+            for i in reversed(range(len(running_tasks))):
+                t = running_tasks[i]
+                t.stop()
+                running_tasks.pop(i)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jorun-0.0.6/src/jorun/runner.py` & `jorun-0.0.7/src/jorun/runner.py`

 * *Files identical despite different names*

### Comparing `jorun-0.0.6/src/jorun/runner_threading.py` & `jorun-0.0.7/src/jorun/runner_threading.py`

 * *Files identical despite different names*

### Comparing `jorun-0.0.6/src/jorun/task.py` & `jorun-0.0.7/src/jorun/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import TypedDict, List, Literal, Optional, Union, Dict
 from dataclasses import dataclass
 
+
 class TaskBuildException(Exception):
     pass
 
 
 class ShellTask(TypedDict):
     command: Union[str, List[str]]
     run_mode: Literal["wait_completion", "indefinite"]
```

### Comparing `jorun-0.0.6/pyproject.toml` & `jorun-0.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jorun"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Paolo Infante", email="info@paoloinfante.it" },
 ]
 description = "A customizable task runner"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "pyyaml"
+    "PyYAML==6.0"
 ]
 
 [project.scripts]
 jorun = "jorun.main:main"
 
 [project.urls]
 "Homepage" = "https://github.com/paolo-projects/jorun"
```

