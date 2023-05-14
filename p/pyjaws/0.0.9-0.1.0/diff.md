# Comparing `tmp/pyjaws-0.0.9.tar.gz` & `tmp/pyjaws-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjaws-0.0.9.tar", last modified: Sat May 13 14:34:05 2023, max compression
+gzip compressed data, was "pyjaws-0.1.0.tar", last modified: Sun May 14 13:49:26 2023, max compression
```

## Comparing `pyjaws-0.0.9.tar` & `pyjaws-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:34:05.174948 pyjaws-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-13 14:34:05.174948 pyjaws-0.0.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:34:05.170948 pyjaws-0.0.9/pyjaws/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-13 14:33:56.000000 pyjaws-0.0.9/pyjaws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:34:05.170948 pyjaws-0.0.9/pyjaws/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:56.000000 pyjaws-0.0.9/pyjaws/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-13 14:33:56.000000 pyjaws-0.0.9/pyjaws/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-13 14:33:56.000000 pyjaws-0.0.9/pyjaws/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-13 14:33:56.000000 pyjaws-0.0.9/pyjaws/api/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:34:05.170948 pyjaws-0.0.9/pyjaws/api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:34:05.174948 pyjaws-0.0.9/pyjaws/api/templates/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-13 14:33:56.000000 pyjaws-0.0.9/pyjaws/api/templates/macros/cluster.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-13 14:33:56.000000 pyjaws-0.0.9/pyjaws/api/templates/macros/task.j2
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-13 14:33:56.000000 pyjaws-0.0.9/pyjaws/api/templates/workflow.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:34:05.174948 pyjaws-0.0.9/pyjaws/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:56.000000 pyjaws-0.0.9/pyjaws/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-13 14:33:56.000000 pyjaws-0.0.9/pyjaws/client/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:34:05.170948 pyjaws-0.0.9/pyjaws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-13 14:34:05.000000 pyjaws-0.0.9/pyjaws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-13 14:34:05.000000 pyjaws-0.0.9/pyjaws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 14:34:05.000000 pyjaws-0.0.9/pyjaws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-13 14:34:05.000000 pyjaws-0.0.9/pyjaws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-13 14:34:05.000000 pyjaws-0.0.9/pyjaws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 14:34:05.000000 pyjaws-0.0.9/pyjaws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-13 14:33:56.000000 pyjaws-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 14:34:05.174948 pyjaws-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-13 14:33:56.000000 pyjaws-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.547489 pyjaws-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-14 13:49:26.547489 pyjaws-0.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.543489 pyjaws-0.1.0/pyjaws/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.547489 pyjaws-0.1.0/pyjaws/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.547489 pyjaws-0.1.0/pyjaws/api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.547489 pyjaws-0.1.0/pyjaws/api/templates/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/templates/macros/cluster.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/templates/macros/task.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/templates/workflow.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.547489 pyjaws-0.1.0/pyjaws/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/client/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.547489 pyjaws-0.1.0/pyjaws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-14 13:49:26.000000 pyjaws-0.1.0/pyjaws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-14 13:49:26.000000 pyjaws-0.1.0/pyjaws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 13:49:26.000000 pyjaws-0.1.0/pyjaws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-14 13:49:26.000000 pyjaws-0.1.0/pyjaws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-14 13:49:26.000000 pyjaws-0.1.0/pyjaws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-14 13:49:26.000000 pyjaws-0.1.0/pyjaws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 13:49:26.547489 pyjaws-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-14 13:49:15.000000 pyjaws-0.1.0/setup.py
```

### Comparing `pyjaws-0.0.9/PKG-INFO` & `pyjaws-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyjaws
-Version: 0.0.9
+Version: 0.1.0
 Author: Rafael Pierre
 Description-Content-Type: text/markdown
 
 # PyJaws: A Pythonic Way to Define Databricks Jobs and Workflows
 
 <p align="center">
         <img src="https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/pyjaws.png" class="align-center" />
     </a>
 </p>
 
 <hr />
 
-![python](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/59dbf9248c65b3e3f1e66ce0ef8d6ce2218fa3b7/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
+[![pypi](https://img.shields.io/badge/pypi-0.0.9-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
 
 <hr />
 
 * **PyJaws** enables declaring [Databricks Jobs and Workflows](https://docs.databricks.com/workflows/index.html) as Python code, allowing for:
    * Code Linting
    * Formatting
    * Parameter Validation
@@ -57,15 +57,15 @@
 
 * Last, define your Workflow Tasks (see `examples`) and run:
 
 ```bash
 pyjaws create path/to/your/workflow_definitions
 ```
 
-### Example
+### Sample Job Definition
 
 ```python
 from pyjaws.api.base import (
     Cluster,
     Runtime,
     Task,
     Workflow
@@ -128,8 +128,12 @@
 
 By default, **pyjaws** also includes some useful tags into the workflows indicating which Git Repo hosts the Python definition, commit hash and when the workflow was last updated. For example:
 
 ![workflow](https://github.com/rafaelpierre/pyjaws/blob/main/img/tags.png?raw=true "Workflow")
 
 ## Disclaimer
 
-* **PyJaws** is not developed, endorsed not supported by Databricks. It is provided as-is; no warranty is derived from using this package.
+* **PyJaws** is not developed, endorsed not supported by Databricks. It is provided as-is; no warranty is derived from using this package. For more details, please refer to the [license](https://github.com/rafaelpierre/pyjaws/blob/main/LICENSE.md).
+
+## Reporting Bugs and Contributing
+
+Feel free to create an issue if you feel something is not right. Contribution guidelines can be found [here](https://githubcom/rafaelpierre/pyjaws/blob/main/CONTRIBUTING.md).
```

### Comparing `pyjaws-0.0.9/pyjaws/api/base.py` & `pyjaws-0.1.0/pyjaws/api/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import jinja2
 import logging
 import json
 from json.decoder import JSONDecodeError
 import rapidjson
 from datetime import datetime
+from matplotlib import pyplot as plt
 
 from typing import List, Optional
 from pydantic import BaseModel
 import os
 import networkx as nx
 
 import git
@@ -87,22 +88,27 @@
     """
     Base class for PyJaws Databricks Workflow.
     Params:
         name: Workflow name.
         tasks: List of Workflow Tasks.
     """
 
+    class Config:
+        arbitrary_types_allowed = True
+
     name: str
     tasks: List[Task]
     tags: Optional[dict] = {}
+    graph: nx.Graph = None
     schedule: Optional[str]
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
+        self._create_graph()
         self.validate()
         self._set_tags(kwargs.get("tags", {}))
 
     def _set_tags(self, tags):
         self.tags = {
             "pyjaws_version": __version__,
             "updated": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
@@ -174,22 +180,33 @@
 
         for task in self.tasks:
             if task.cluster.job_cluster_key not in [
                 str(cluster) for cluster in self.clusters
             ]:
                 raise ValueError(f"Invalid Cluster ID: {task.cluster.job_cluster_key}")
 
-    def _validate_cycles(self):
-        node_list = []
-        for task in self.tasks:
-            for dependency in task.dependencies or []:
-                node_list.append((str(task), str(dependency)))
+    def _create_graph(self):
+        edge_list = []
+
+        if len(self.tasks) == 1:
+            self.graph = nx.Graph()
+            self.graph.add_node(self.tasks[0].task_name)
+        else:
+            for task in self.tasks:
+                for dependency in task.dependencies or []:
+                    edge_list.append((str(dependency), str(task)))
 
-        graph = nx.DiGraph(node_list)
-        cycles = list(nx.simple_cycles(graph))
+            self.graph = nx.DiGraph(edge_list)
+
+    def _validate_cycles(self):
+        cycles = list(nx.simple_cycles(self.graph))
         if len(cycles) > 0:
             raise ValueError("Cycle(s) detected in the workflow")
 
     def validate(self):
         super().validate(self)
         self._validate_tasks()
         self._validate_cycles()
+
+    def _ipython_display_(self):
+        nx.draw(self.graph, with_labels=True)
+        plt.show()
```

### Comparing `pyjaws-0.0.9/pyjaws/api/jobs.py` & `pyjaws-0.1.0/pyjaws/api/jobs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -36,8 +36,8 @@
             result = jobs_api.create_job(json=workflow.json(), version=API_VERSION)
 
         logging.info(f"Result: {str(result)}")
         return result
 
     except Exception as exception:
         logging.error("Error creating Databricks Jobs Workflow:")
-        logging.error(str(exception))
+        logging.error(str(exception))
```

### Comparing `pyjaws-0.0.9/pyjaws/api/templates/macros/cluster.j2` & `pyjaws-0.1.0/pyjaws/api/templates/macros/cluster.j2`

 * *Files identical despite different names*

### Comparing `pyjaws-0.0.9/pyjaws/api/templates/macros/task.j2` & `pyjaws-0.1.0/pyjaws/api/templates/macros/task.j2`

 * *Files identical despite different names*

### Comparing `pyjaws-0.0.9/pyjaws/api/templates/workflow.j2` & `pyjaws-0.1.0/pyjaws/api/templates/workflow.j2`

 * *Files identical despite different names*

### Comparing `pyjaws-0.0.9/pyjaws/client/entrypoint.py` & `pyjaws-0.1.0/pyjaws/client/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pyjaws-0.0.9/pyjaws.egg-info/PKG-INFO` & `pyjaws-0.1.0/pyjaws.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyjaws
-Version: 0.0.9
+Version: 0.1.0
 Author: Rafael Pierre
 Description-Content-Type: text/markdown
 
 # PyJaws: A Pythonic Way to Define Databricks Jobs and Workflows
 
 <p align="center">
         <img src="https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/pyjaws.png" class="align-center" />
     </a>
 </p>
 
 <hr />
 
-![python](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/59dbf9248c65b3e3f1e66ce0ef8d6ce2218fa3b7/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
+[![pypi](https://img.shields.io/badge/pypi-0.0.9-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
 
 <hr />
 
 * **PyJaws** enables declaring [Databricks Jobs and Workflows](https://docs.databricks.com/workflows/index.html) as Python code, allowing for:
    * Code Linting
    * Formatting
    * Parameter Validation
@@ -57,15 +57,15 @@
 
 * Last, define your Workflow Tasks (see `examples`) and run:
 
 ```bash
 pyjaws create path/to/your/workflow_definitions
 ```
 
-### Example
+### Sample Job Definition
 
 ```python
 from pyjaws.api.base import (
     Cluster,
     Runtime,
     Task,
     Workflow
@@ -128,8 +128,12 @@
 
 By default, **pyjaws** also includes some useful tags into the workflows indicating which Git Repo hosts the Python definition, commit hash and when the workflow was last updated. For example:
 
 ![workflow](https://github.com/rafaelpierre/pyjaws/blob/main/img/tags.png?raw=true "Workflow")
 
 ## Disclaimer
 
-* **PyJaws** is not developed, endorsed not supported by Databricks. It is provided as-is; no warranty is derived from using this package.
+* **PyJaws** is not developed, endorsed not supported by Databricks. It is provided as-is; no warranty is derived from using this package. For more details, please refer to the [license](https://github.com/rafaelpierre/pyjaws/blob/main/LICENSE.md).
+
+## Reporting Bugs and Contributing
+
+Feel free to create an issue if you feel something is not right. Contribution guidelines can be found [here](https://githubcom/rafaelpierre/pyjaws/blob/main/CONTRIBUTING.md).
```

### Comparing `pyjaws-0.0.9/pyproject.toml` & `pyjaws-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjaws-0.0.9/setup.py` & `pyjaws-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,29 +8,26 @@
     "pydantic==1.10.5",
     "Jinja2==3.1.2",
     "networkx",
     "GitPython==3.1.31",
     "databricks-cli==0.17.5",
     "requests<2.30.0",
     "urllib3<2",
+    "matplotlib",
 ]
 
 current_dir = Path(__file__).parent.parent
 long_description = (current_dir / "README.md").read_text()
 
 setup(
     name="pyjaws",
     packages=find_packages(),
     include_package_data=True,
-    package_data={"": [
-        "README.md",
-        "api/templates/*.j2",
-        "api/templates/macros/*.j2"
-    ]},
+    package_data={"": ["README.md", "api/templates/*.j2", "api/templates/macros/*.j2"]},
     setup_requires=["setuptools", "wheel"],
     install_requires=PACKAGE_REQUIREMENTS,
     entry_points={"console_scripts": ["pyjaws = pyjaws.client.entrypoint:main"]},
     version=pyjaws.__version__,
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author="Rafael Pierre",
 )
```

