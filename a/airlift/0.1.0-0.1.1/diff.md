# Comparing `tmp/airlift-0.1.0.tar.gz` & `tmp/airlift-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airlift-0.1.0.tar", max compression
+gzip compressed data, was "airlift-0.1.1.tar", max compression
```

## Comparing `airlift-0.1.0.tar` & `airlift-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1062 2023-05-13 20:35:09.154429 airlift-0.1.0/LICENSE
--rw-r--r--   0        0        0     5827 2023-05-13 22:07:19.540913 airlift-0.1.0/README.md
--rw-r--r--   0        0        0      673 2023-05-13 21:52:20.356408 airlift-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-13 20:35:22.254645 airlift-0.1.0/src/airlift/__init__.py
--rw-r--r--   0        0        0        0 2023-05-13 20:35:22.254645 airlift-0.1.0/src/airlift/commands/__init__.py
--rw-r--r--   0        0        0     1364 2023-05-13 21:13:49.991454 airlift-0.1.0/src/airlift/commands/check.py
--rw-r--r--   0        0        0     1033 2023-05-13 21:14:11.384878 airlift-0.1.0/src/airlift/commands/import_variables.py
--rw-r--r--   0        0        0      939 2023-05-13 21:14:57.378873 airlift-0.1.0/src/airlift/commands/pause.py
--rw-r--r--   0        0        0     1161 2023-05-13 21:15:20.530274 airlift-0.1.0/src/airlift/commands/remove.py
--rw-r--r--   0        0        0      826 2023-05-13 21:15:45.004522 airlift-0.1.0/src/airlift/commands/run_dag.py
--rw-r--r--   0        0        0     6709 2023-05-13 21:17:54.793078 airlift-0.1.0/src/airlift/commands/start.py
--rw-r--r--   0        0        0      896 2023-05-13 21:18:41.487335 airlift-0.1.0/src/airlift/commands/status.py
--rw-r--r--   0        0        0        0 2023-05-13 20:35:22.254645 airlift-0.1.0/src/airlift/config/__init__.py
--rw-r--r--   0        0        0        0 2023-05-13 20:35:22.254645 airlift-0.1.0/src/airlift/config/airlift/config.yaml
--rw-r--r--   0        0        0       71 2023-05-13 20:35:22.254645 airlift-0.1.0/src/airlift/config/airlift/required_software.yaml
--rw-r--r--   0        0        0     1012 2023-05-13 20:35:22.254645 airlift-0.1.0/src/airlift/config/config.py
--rw-r--r--   0        0        0      176 2023-05-13 20:35:22.254645 airlift-0.1.0/src/airlift/config/docker/Dockerfile
--rw-r--r--   0        0        0        0 2023-05-13 20:35:22.254645 airlift-0.1.0/src/airlift/config/docker/final/.gitkeep
--rw-r--r--   0        0        0     1089 2023-05-13 20:35:22.254645 airlift-0.1.0/src/airlift/config/helm/final_values.yaml
--rw-r--r--   0        0        0     1482 2023-05-13 20:35:22.254645 airlift-0.1.0/src/airlift/config/helm/values.yaml
--rw-r--r--   0        0        0      975 2023-05-13 20:35:22.254645 airlift-0.1.0/src/airlift/config/kind/cluster.yaml
--rw-r--r--   0        0        0     3599 2023-05-13 20:55:47.890980 airlift-0.1.0/src/airlift/main.py
--rw-r--r--   0        0        0        0 2023-05-13 20:35:22.254645 airlift-0.1.0/src/airlift/utils/__init__.py
--rw-r--r--   0        0        0     3676 2023-05-13 21:00:00.287192 airlift-0.1.0/src/airlift/utils/airflow.py
--rw-r--r--   0        0        0      767 2023-05-13 21:01:25.464427 airlift-0.1.0/src/airlift/utils/airlift.py
--rw-r--r--   0        0        0      677 2023-05-13 21:02:53.808815 airlift-0.1.0/src/airlift/utils/command.py
--rw-r--r--   0        0        0     1989 2023-05-13 21:04:22.003707 airlift-0.1.0/src/airlift/utils/docker.py
--rw-r--r--   0        0        0     3087 2023-05-13 21:08:30.050849 airlift-0.1.0/src/airlift/utils/file.py
--rw-r--r--   0        0        0     1606 2023-05-13 21:09:46.628259 airlift-0.1.0/src/airlift/utils/helm.py
--rw-r--r--   0        0        0     2306 2023-05-13 21:11:14.760301 airlift-0.1.0/src/airlift/utils/kind.py
--rw-r--r--   0        0        0      815 2023-05-13 21:11:59.434741 airlift-0.1.0/src/airlift/utils/kubernetes.py
--rw-r--r--   0        0        0     7339 2023-05-13 21:13:12.829961 airlift-0.1.0/src/airlift/utils/parser.py
--rw-r--r--   0        0        0     6570 1970-01-01 00:00:00.000000 airlift-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-14 19:34:47.096484 airlift-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6286 2023-05-14 19:34:47.096484 airlift-0.1.1/README.md
+-rw-r--r--   0        0        0      673 2023-05-14 19:34:47.108484 airlift-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/__init__.py
+-rw-r--r--   0        0        0     1364 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/check.py
+-rw-r--r--   0        0        0     1033 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/import_variables.py
+-rw-r--r--   0        0        0      939 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/pause.py
+-rw-r--r--   0        0        0     1161 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/remove.py
+-rw-r--r--   0        0        0      826 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/run_dag.py
+-rw-r--r--   0        0        0     6709 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/start.py
+-rw-r--r--   0        0        0      896 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/commands/status.py
+-rw-r--r--   0        0        0        0 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/config/airlift/config.yaml
+-rw-r--r--   0        0        0       71 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/config/airlift/required_software.yaml
+-rw-r--r--   0        0        0      979 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/config/config.py
+-rw-r--r--   0        0        0      176 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/config/docker/Dockerfile
+-rw-r--r--   0        0        0        0 2023-05-14 19:34:47.108484 airlift-0.1.1/src/airlift/config/docker/final/.gitkeep
+-rw-r--r--   0        0        0     1089 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/config/helm/final_values.yaml
+-rw-r--r--   0        0        0     1482 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/config/helm/values.yaml
+-rw-r--r--   0        0        0      975 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/config/kind/cluster.yaml
+-rw-r--r--   0        0        0     3599 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/main.py
+-rw-r--r--   0        0        0        0 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/__init__.py
+-rw-r--r--   0        0        0     3676 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/airflow.py
+-rw-r--r--   0        0        0      767 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/airlift.py
+-rw-r--r--   0        0        0      677 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/command.py
+-rw-r--r--   0        0        0     1989 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/docker.py
+-rw-r--r--   0        0        0     3087 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/file.py
+-rw-r--r--   0        0        0     1606 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/helm.py
+-rw-r--r--   0        0        0     2306 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/kind.py
+-rw-r--r--   0        0        0      815 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/kubernetes.py
+-rw-r--r--   0        0        0     7020 2023-05-14 19:34:47.112484 airlift-0.1.1/src/airlift/utils/parser.py
+-rw-r--r--   0        0        0     7029 1970-01-01 00:00:00.000000 airlift-0.1.1/PKG-INFO
```

### Comparing `airlift-0.1.0/LICENSE` & `airlift-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/README.md` & `airlift-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,16 @@
         alt="helicopter"
         width="120"
         height="90"
        />
 </h3>
 <h1 align="center">Airlift</h1>
 <p align="center">
-  <a href="https://pypi.org/project/PACKAGE-NAME/">
-    <img alt="PyPI version" src="https://badge.fury.io/py/PACKAGE-NAME.svg">
+  <a href="https://pypi.org/project/airlift/">
+    <img alt="PyPI version" src="https://badge.fury.io/py/airlift.svg">
   </a>
 </p>
 
 ## Introduction
 
 Airlift is a Command Line Interface (CLI) tool designed to provide a flexible local development environment for Apache Airflow with simple defaults.
 It is built on top of the official [Airflow Helm Chart](https://artifacthub.io/packages/helm/apache-airflow/airflow).
@@ -51,17 +51,19 @@
 ```bash
 brew install helm
 ```
 
 #### Docker
 
 ```bash
-brew install docker
+brew install --cask docker
 ```
 
+-OR- use a tool like [Docker Desktop](https://www.docker.com/products/docker-desktop/) or [Rancher Desktop](https://rancherdesktop.io/)
+
 #### Kind
 
 ```bash
 brew install kind
 ```
 
 ## Installation
@@ -88,14 +90,17 @@
 
 ```bash
 airlift start -d /path/to/dags -p /path/to/plugins -r /path/to/requirements.txt
 ```
 
 **Note: The DAG and Plugins folders are mounted directly to the airflow service for hot-reloading. When you make a change locally, it should automatically appear in the Airflow UI.**
 
+**Note: Start times for Airflow can be upwards of 5 minutes, due to the bootstrapping, installation of required PyPi packages, and the creation of the Postgres database.
+This all depends on your local machines power & the complexity of your Airflow setup.**
+
 #### 2. check
 
 Checks if all pre-requisite software is installed.
 
 ```bash
 airlift check
 ```
@@ -226,14 +231,18 @@
 
 In this example, `dag_path` in the yaml file overrides the `-d` setting, `plugin_path` overrides the `-p` setting, and so forth.
 
 ## Examples
 
 [See here for examples with common configuration modifications.](./docs/examples/)
 
+## FAQ
+
+[See here for Frequently Asked Questions](./docs/faq.md)
+
 ## Motivation
 
 The motivation behind the creation of Airlift is to simplify the process of setting up a local development environment for Apache Airflow. It aims to be a flexible tool that allows developers to easily configure and manage their Airflow instances with unlimited flexibility.
 
 ## Support and Contribution
 
 If you encounter any issues or have suggestions for improvements, feel free to open an issue on the GitHub repository. Contributions to the project are also welcome.
```

#### html2text {}

```diff
@@ -10,25 +10,30 @@
 system: 1. Helm 2. Docker 3. Kind Below are the installation instructions for
 each of these tools on MacOS and Linux distributions. ### Install Homebrew
 Homebrew is a package manager that we will use to install the necessary
 software. If you don't have Homebrew installed, you can install it by following
 these instructions: ```bash /bin/bash -c "$(curl -fsSL https://
 raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)" ``` ### Install
 Software With Homebrew installed, you can now install Helm, Docker, and Kind.
-#### Helm ```bash brew install helm ``` #### Docker ```bash brew install docker
-``` #### Kind ```bash brew install kind ``` ## Installation Airlift can be
-installed using pip: ```bash pip install airlift ``` ## Usage The general
-syntax for using the Airlift CLI tool is: ```bash airlift [subcommand]
-[options] ``` ### Subcommands and Options #### 1. start Starts the Airflow
-service. ```bash airlift start -d /path/to/dags -p /path/to/plugins -r /path/
-to/requirements.txt ``` **Note: The DAG and Plugins folders are mounted
-directly to the airflow service for hot-reloading. When you make a change
-locally, it should automatically appear in the Airflow UI.** #### 2. check
-Checks if all pre-requisite software is installed. ```bash airlift check ```
-#### 3. pause Pauses the Airflow service. ```bash airlift pause ``` #### 4.
+#### Helm ```bash brew install helm ``` #### Docker ```bash brew install --cask
+docker ``` -OR- use a tool like [Docker Desktop](https://www.docker.com/
+products/docker-desktop/) or [Rancher Desktop](https://rancherdesktop.io/) ####
+Kind ```bash brew install kind ``` ## Installation Airlift can be installed
+using pip: ```bash pip install airlift ``` ## Usage The general syntax for
+using the Airlift CLI tool is: ```bash airlift [subcommand] [options] ``` ###
+Subcommands and Options #### 1. start Starts the Airflow service. ```bash
+airlift start -d /path/to/dags -p /path/to/plugins -r /path/to/requirements.txt
+``` **Note: The DAG and Plugins folders are mounted directly to the airflow
+service for hot-reloading. When you make a change locally, it should
+automatically appear in the Airflow UI.** **Note: Start times for Airflow can
+be upwards of 5 minutes, due to the bootstrapping, installation of required
+PyPi packages, and the creation of the Postgres database. This all depends on
+your local machines power & the complexity of your Airflow setup.** #### 2.
+check Checks if all pre-requisite software is installed. ```bash airlift check
+``` #### 3. pause Pauses the Airflow service. ```bash airlift pause ``` #### 4.
 unpause Unpauses the Airflow service. ```bash airlift unpause ``` #### 5.
 remove Removes all containers/clusters related to the `airlift` service.
 ```bash airlift remove ``` #### 6. status Checks the status of the service and
 whether or not it is reachable. ```bash airlift status -P 8080 ``` #### 7.
 import_variables Imports a `variables.json` file to a running Airflow instance.
 ```bash airlift import_variables -P 8080 -V /path/to/variables.json ``` #### 8.
 run_dag Runs a DAG given an ID. ```bash airlift run_dag -P 8080 -
@@ -59,16 +64,17 @@
 path/to/values.yaml airlift_config_file: /path/to/airlift/config.yaml
 extra_volume_mounts: - hostPath=/my/cool/path,containerPath=/my/mounted/
 path,name=a_unique_name cluster_config_file: /path/to/cluster/config.yaml
 image: 'apache/airflow:2.6.0' helm_chart_version: '1.0.0' port: 8080
 post_start_dag_id: 'example_dag_id' ``` In this example, `dag_path` in the yaml
 file overrides the `-d` setting, `plugin_path` overrides the `-p` setting, and
 so forth. ## Examples [See here for examples with common configuration
-modifications.](./docs/examples/) ## Motivation The motivation behind the
-creation of Airlift is to simplify the process of setting up a local
-development environment for Apache Airflow. It aims to be a flexible tool that
-allows developers to easily configure and manage their Airflow instances with
+modifications.](./docs/examples/) ## FAQ [See here for Frequently Asked
+Questions](./docs/faq.md) ## Motivation The motivation behind the creation of
+Airlift is to simplify the process of setting up a local development
+environment for Apache Airflow. It aims to be a flexible tool that allows
+developers to easily configure and manage their Airflow instances with
 unlimited flexibility. ## Support and Contribution If you encounter any issues
 or have suggestions for improvements, feel free to open an issue on the GitHub
 repository. Contributions to the project are also welcome. ## Contact If you
 have questions or feedback about Airlift, please reach out by opening an issue
 on the GitHub repository.
```

### Comparing `airlift-0.1.0/pyproject.toml` & `airlift-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airlift"
-version = "0.1.0"
+version = "0.1.1"
 description = "A CLI for creating a flexible Apache Airflow local development environment"
 authors = ["jered.little <jeredlittle1996@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "airlift", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `airlift-0.1.0/src/airlift/commands/check.py` & `airlift-0.1.1/src/airlift/commands/check.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/commands/import_variables.py` & `airlift-0.1.1/src/airlift/commands/import_variables.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/commands/pause.py` & `airlift-0.1.1/src/airlift/commands/pause.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/commands/remove.py` & `airlift-0.1.1/src/airlift/commands/remove.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/commands/run_dag.py` & `airlift-0.1.1/src/airlift/commands/run_dag.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/commands/start.py` & `airlift-0.1.1/src/airlift/commands/start.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/commands/status.py` & `airlift-0.1.1/src/airlift/commands/status.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/config/config.py` & `airlift-0.1.1/src/airlift/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 
 BASE_DIR = os.path.dirname(os.path.realpath(__file__))
 REQUIRED_SOFTWARE_PATH = os.path.join(BASE_DIR, "airlift/required_software.yaml")
 DEFAULT_AIRLIFT_CONFIG_FILE = os.path.join(BASE_DIR, "airlift/config.yaml")
 DEFAULT_HELM_CONFIG_FILE = os.path.join(BASE_DIR, "helm/values.yaml")
 DEFAULT_CLUSTER_CONFIG_FILE = os.path.join(BASE_DIR, "kind/cluster.yaml")
-DEFAULT_MERGE_STRATEGY = "MERGE"
 FINAL_HELM_VALUES_FILE_PATH = os.path.join(BASE_DIR, "helm/final_values.yaml")
 FINAL_CONFIG_VALUES_FILE_PATH = os.path.join(BASE_DIR, "airlift/final_config.yaml")
 FINAL_CLUSTER_CONFIG_FILE_PATH = os.path.join(BASE_DIR, "kind/final_cluster.yaml")
 CHART_VERSION = "1.9.0"
 CHART_REPO = "apache-airflow"
 CHART_URL = "https://airflow.apache.org"
 NAME = "airlift"
```

### Comparing `airlift-0.1.0/src/airlift/config/helm/final_values.yaml` & `airlift-0.1.1/src/airlift/config/helm/final_values.yaml`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/config/helm/values.yaml` & `airlift-0.1.1/src/airlift/config/helm/values.yaml`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/config/kind/cluster.yaml` & `airlift-0.1.1/src/airlift/config/kind/cluster.yaml`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/main.py` & `airlift-0.1.1/src/airlift/main.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/utils/airflow.py` & `airlift-0.1.1/src/airlift/utils/airflow.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/utils/airlift.py` & `airlift-0.1.1/src/airlift/utils/airlift.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/utils/command.py` & `airlift-0.1.1/src/airlift/utils/command.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/utils/docker.py` & `airlift-0.1.1/src/airlift/utils/docker.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/utils/file.py` & `airlift-0.1.1/src/airlift/utils/file.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/utils/helm.py` & `airlift-0.1.1/src/airlift/utils/helm.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/utils/kind.py` & `airlift-0.1.1/src/airlift/utils/kind.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/utils/kubernetes.py` & `airlift-0.1.1/src/airlift/utils/kubernetes.py`

 * *Files identical despite different names*

### Comparing `airlift-0.1.0/src/airlift/utils/parser.py` & `airlift-0.1.1/src/airlift/utils/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import argparse
 from airlift.config.config import (
     CHART_VERSION,
-    DEFAULT_MERGE_STRATEGY,
     DEFAULT_DOCKERFILE_PATH,
     DEFAULT_DOCKER_IMAGE,
     DEFAULT_WEBSERVER_PORT,
 )
 
 
 class ParserUtils:
@@ -90,20 +89,14 @@
         )
         start.add_argument(
             "-C",
             "--cluster_config_file",
             help="Optional cnfiguration file for the `kind` cluster.",
         )
         start.add_argument(
-            "-s",
-            "--config_merge_strategy",
-            default=DEFAULT_MERGE_STRATEGY,
-            help="When config files are passed in via the CLI, what is the strategy for using the files. Defaults to merging with the default config.",
-        )
-        start.add_argument(
             "-ip",
             "--image_path",
             default=DEFAULT_DOCKERFILE_PATH,
             help="The path to the base image for the Dockerfile, if used.",
         )
         start.add_argument(
             "-i",
```

### Comparing `airlift-0.1.0/PKG-INFO` & `airlift-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airlift
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI for creating a flexible Apache Airflow local development environment
 Author: jered.little
 Author-email: jeredlittle1996@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,16 +23,16 @@
         alt="helicopter"
         width="120"
         height="90"
        />
 </h3>
 <h1 align="center">Airlift</h1>
 <p align="center">
-  <a href="https://pypi.org/project/PACKAGE-NAME/">
-    <img alt="PyPI version" src="https://badge.fury.io/py/PACKAGE-NAME.svg">
+  <a href="https://pypi.org/project/airlift/">
+    <img alt="PyPI version" src="https://badge.fury.io/py/airlift.svg">
   </a>
 </p>
 
 ## Introduction
 
 Airlift is a Command Line Interface (CLI) tool designed to provide a flexible local development environment for Apache Airflow with simple defaults.
 It is built on top of the official [Airflow Helm Chart](https://artifacthub.io/packages/helm/apache-airflow/airflow).
@@ -71,17 +71,19 @@
 ```bash
 brew install helm
 ```
 
 #### Docker
 
 ```bash
-brew install docker
+brew install --cask docker
 ```
 
+-OR- use a tool like [Docker Desktop](https://www.docker.com/products/docker-desktop/) or [Rancher Desktop](https://rancherdesktop.io/)
+
 #### Kind
 
 ```bash
 brew install kind
 ```
 
 ## Installation
@@ -108,14 +110,17 @@
 
 ```bash
 airlift start -d /path/to/dags -p /path/to/plugins -r /path/to/requirements.txt
 ```
 
 **Note: The DAG and Plugins folders are mounted directly to the airflow service for hot-reloading. When you make a change locally, it should automatically appear in the Airflow UI.**
 
+**Note: Start times for Airflow can be upwards of 5 minutes, due to the bootstrapping, installation of required PyPi packages, and the creation of the Postgres database.
+This all depends on your local machines power & the complexity of your Airflow setup.**
+
 #### 2. check
 
 Checks if all pre-requisite software is installed.
 
 ```bash
 airlift check
 ```
@@ -246,14 +251,18 @@
 
 In this example, `dag_path` in the yaml file overrides the `-d` setting, `plugin_path` overrides the `-p` setting, and so forth.
 
 ## Examples
 
 [See here for examples with common configuration modifications.](./docs/examples/)
 
+## FAQ
+
+[See here for Frequently Asked Questions](./docs/faq.md)
+
 ## Motivation
 
 The motivation behind the creation of Airlift is to simplify the process of setting up a local development environment for Apache Airflow. It aims to be a flexible tool that allows developers to easily configure and manage their Airflow instances with unlimited flexibility.
 
 ## Support and Contribution
 
 If you encounter any issues or have suggestions for improvements, feel free to open an issue on the GitHub repository. Contributions to the project are also welcome.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: airlift Version: 0.1.0 Summary: A CLI for creating
+Metadata-Version: 2.1 Name: airlift Version: 0.1.1 Summary: A CLI for creating
 a flexible Apache Airflow local development environment Author: jered.little
 Author-email: jeredlittle1996@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: dotmap (>=1.3.30,<2.0.0) Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: hiyapyco (>=0.5.1,<0.6.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
@@ -20,25 +20,30 @@
 system: 1. Helm 2. Docker 3. Kind Below are the installation instructions for
 each of these tools on MacOS and Linux distributions. ### Install Homebrew
 Homebrew is a package manager that we will use to install the necessary
 software. If you don't have Homebrew installed, you can install it by following
 these instructions: ```bash /bin/bash -c "$(curl -fsSL https://
 raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)" ``` ### Install
 Software With Homebrew installed, you can now install Helm, Docker, and Kind.
-#### Helm ```bash brew install helm ``` #### Docker ```bash brew install docker
-``` #### Kind ```bash brew install kind ``` ## Installation Airlift can be
-installed using pip: ```bash pip install airlift ``` ## Usage The general
-syntax for using the Airlift CLI tool is: ```bash airlift [subcommand]
-[options] ``` ### Subcommands and Options #### 1. start Starts the Airflow
-service. ```bash airlift start -d /path/to/dags -p /path/to/plugins -r /path/
-to/requirements.txt ``` **Note: The DAG and Plugins folders are mounted
-directly to the airflow service for hot-reloading. When you make a change
-locally, it should automatically appear in the Airflow UI.** #### 2. check
-Checks if all pre-requisite software is installed. ```bash airlift check ```
-#### 3. pause Pauses the Airflow service. ```bash airlift pause ``` #### 4.
+#### Helm ```bash brew install helm ``` #### Docker ```bash brew install --cask
+docker ``` -OR- use a tool like [Docker Desktop](https://www.docker.com/
+products/docker-desktop/) or [Rancher Desktop](https://rancherdesktop.io/) ####
+Kind ```bash brew install kind ``` ## Installation Airlift can be installed
+using pip: ```bash pip install airlift ``` ## Usage The general syntax for
+using the Airlift CLI tool is: ```bash airlift [subcommand] [options] ``` ###
+Subcommands and Options #### 1. start Starts the Airflow service. ```bash
+airlift start -d /path/to/dags -p /path/to/plugins -r /path/to/requirements.txt
+``` **Note: The DAG and Plugins folders are mounted directly to the airflow
+service for hot-reloading. When you make a change locally, it should
+automatically appear in the Airflow UI.** **Note: Start times for Airflow can
+be upwards of 5 minutes, due to the bootstrapping, installation of required
+PyPi packages, and the creation of the Postgres database. This all depends on
+your local machines power & the complexity of your Airflow setup.** #### 2.
+check Checks if all pre-requisite software is installed. ```bash airlift check
+``` #### 3. pause Pauses the Airflow service. ```bash airlift pause ``` #### 4.
 unpause Unpauses the Airflow service. ```bash airlift unpause ``` #### 5.
 remove Removes all containers/clusters related to the `airlift` service.
 ```bash airlift remove ``` #### 6. status Checks the status of the service and
 whether or not it is reachable. ```bash airlift status -P 8080 ``` #### 7.
 import_variables Imports a `variables.json` file to a running Airflow instance.
 ```bash airlift import_variables -P 8080 -V /path/to/variables.json ``` #### 8.
 run_dag Runs a DAG given an ID. ```bash airlift run_dag -P 8080 -
@@ -69,16 +74,17 @@
 path/to/values.yaml airlift_config_file: /path/to/airlift/config.yaml
 extra_volume_mounts: - hostPath=/my/cool/path,containerPath=/my/mounted/
 path,name=a_unique_name cluster_config_file: /path/to/cluster/config.yaml
 image: 'apache/airflow:2.6.0' helm_chart_version: '1.0.0' port: 8080
 post_start_dag_id: 'example_dag_id' ``` In this example, `dag_path` in the yaml
 file overrides the `-d` setting, `plugin_path` overrides the `-p` setting, and
 so forth. ## Examples [See here for examples with common configuration
-modifications.](./docs/examples/) ## Motivation The motivation behind the
-creation of Airlift is to simplify the process of setting up a local
-development environment for Apache Airflow. It aims to be a flexible tool that
-allows developers to easily configure and manage their Airflow instances with
+modifications.](./docs/examples/) ## FAQ [See here for Frequently Asked
+Questions](./docs/faq.md) ## Motivation The motivation behind the creation of
+Airlift is to simplify the process of setting up a local development
+environment for Apache Airflow. It aims to be a flexible tool that allows
+developers to easily configure and manage their Airflow instances with
 unlimited flexibility. ## Support and Contribution If you encounter any issues
 or have suggestions for improvements, feel free to open an issue on the GitHub
 repository. Contributions to the project are also welcome. ## Contact If you
 have questions or feedback about Airlift, please reach out by opening an issue
 on the GitHub repository.
```

