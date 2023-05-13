# Comparing `tmp/ecidacli-0.0.8.tar.gz` & `tmp/ecidacli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecidacli-0.0.8.tar", last modified: Mon May  1 08:44:27 2023, max compression
+gzip compressed data, was "ecidacli-0.0.9.tar", last modified: Wed May  3 17:19:04 2023, max compression
```

## Comparing `ecidacli-0.0.8.tar` & `ecidacli-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-01 08:44:27.288248 ecidacli-0.0.8/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      455 2023-05-01 08:44:27.288248 ecidacli-0.0.8/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       66 2023-03-09 16:23:50.000000 ecidacli-0.0.8/README.md
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-01 08:44:27.288248 ecidacli-0.0.8/ecidacli.egg-info/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      455 2023-05-01 08:44:27.000000 ecidacli-0.0.8/ecidacli.egg-info/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      224 2023-05-01 08:44:27.000000 ecidacli-0.0.8/ecidacli.egg-info/SOURCES.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-01 08:44:27.000000 ecidacli-0.0.8/ecidacli.egg-info/dependency_links.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       43 2023-05-01 08:44:27.000000 ecidacli-0.0.8/ecidacli.egg-info/entry_points.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       26 2023-05-01 08:44:27.000000 ecidacli-0.0.8/ecidacli.egg-info/requires.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        9 2023-05-01 08:44:27.000000 ecidacli-0.0.8/ecidacli.egg-info/top_level.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     3580 2023-05-01 08:44:16.000000 ecidacli-0.0.8/ecidacli.py
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-01 08:44:27.288248 ecidacli-0.0.8/setup.cfg
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      809 2023-05-01 08:44:24.000000 ecidacli-0.0.8/setup.py
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-03 17:19:04.624456 ecidacli-0.0.9/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      455 2023-05-03 17:19:04.624456 ecidacli-0.0.9/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       66 2023-03-09 16:23:50.000000 ecidacli-0.0.9/README.md
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-03 17:19:04.624456 ecidacli-0.0.9/ecidacli.egg-info/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      455 2023-05-03 17:19:04.000000 ecidacli-0.0.9/ecidacli.egg-info/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      224 2023-05-03 17:19:04.000000 ecidacli-0.0.9/ecidacli.egg-info/SOURCES.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-03 17:19:04.000000 ecidacli-0.0.9/ecidacli.egg-info/dependency_links.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       43 2023-05-03 17:19:04.000000 ecidacli-0.0.9/ecidacli.egg-info/entry_points.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       26 2023-05-03 17:19:04.000000 ecidacli-0.0.9/ecidacli.egg-info/requires.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        9 2023-05-03 17:19:04.000000 ecidacli-0.0.9/ecidacli.egg-info/top_level.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     4282 2023-05-03 17:11:25.000000 ecidacli-0.0.9/ecidacli.py
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-03 17:19:04.624456 ecidacli-0.0.9/setup.cfg
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      809 2023-05-03 17:19:01.000000 ecidacli-0.0.9/setup.py
```

### Comparing `ecidacli-0.0.8/ecidacli.py` & `ecidacli-0.0.9/ecidacli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import argparse
 import os
 import importlib
 import yaml
+# from Ecida import EcidaModule
 
 dockerfile_commands = []
 dockerfile_commands.append("FROM python:3.9-slim-buster")
 dockerfile_commands.append("WORKDIR /app")
 dockerfile_commands.append("COPY requirements.txt .")
 dockerfile_commands.append("RUN pip install --no-cache-dir -r requirements.txt")
 dockerfile_commands.append("COPY . .")
 
-def create_deploy_docker_image(imageTag: str, mainfile:str ):
+def create_deploy_docker_image(imageTag: str, mainfile:str):
     # Define the base image and working directory
     base_image = "python:3.9-slim-buster"
     workdir = "/app"
 
     # Define the Dockerfile commands
     dockerfile = []
     dockerfile.append(f"FROM {base_image}")
@@ -31,16 +32,33 @@
     # Build the Docker image
     
     os.system(f"docker build -t {imageTag} .")
     os.system(f"docker push {imageTag}")
     os.remove("Dockerfile")
     
 
-def apply_yaml(Module, imageTag:str):
+def apply_yaml(Module, imageTag:str, secret: str):
     moduleName = f"{Module.name}-{Module.version}"
+    files = {}
+    
+    for key, git in Module.directories.items():
+        files[key] = {
+            "localPath": key,
+            "remotePath": f"{moduleName}-{key}"
+        }
+        if git["source"] != "":
+            git["secret"] = secret
+            files[key]["preload"] = {
+                "git" : {
+                    "source" : git["source"],
+                    "folder" : git["folder"],
+                    "secret" : git["secret"]
+                }
+            }
+        
     data = {
         "apiVersion": "ecida.org/v5alpha1",
         "kind" : "Module",
         "metadata": {
             "name": moduleName,
             "namespace": "ecida-repository",
             "labels":{
@@ -58,53 +76,55 @@
               "kafka":{
                   "server": "KAFKA_BOOTSTRAP_SERVER",
                   "securityProtocol": "KAFKA_SECURITY_PROTOCOL",
                   "saslMechanism": "KAFKA_SASL_MECHANISM",
                   "username": "KAFKA_USERNAME",
                   "password": "KAFKA_PASSWORD",
                   "topics": Module.topics_envVars
-              }
+              },
+              "file" : files
           }
         }
     }
     yamlFilename = f"auto_generated_{moduleName}.yaml"
     with open(yamlFilename, "w") as f:
         yaml.dump(data, f)
     
 def main():
-    print("v0.0.5.2")
+    print("v0.0.5.3")
     # Create an ArgumentParser object
     parser = argparse.ArgumentParser()
 
     # Add arguments to the parser
     parser.add_argument("-u", "--username", help="Username for Dockerhub authentication")
     parser.add_argument("-f", "--main-file", help="Main file to process (example: main.py)")
+    parser.add_argument("-s", "--secret", help="Name of secret in the kubernetes-cluster (example: main.py)")
 
     # Parse the command line arguments
     args = parser.parse_args()
     mainfilepath = args.main_file
     
     python_module_path = mainfilepath[:-3]
     python_module_path = python_module_path.replace("/", ".")
     python_module_path = python_module_path.lstrip('.')
     
     username = args.username
-    
+    secret = args.secret
     # Import the module dynamically
     try:
         module = importlib.import_module(python_module_path)
         M = module.create_module()
         
         imageTag = username + "/" + M.name + ":" + M.version
-        apply_yaml(M, imageTag)
+        apply_yaml(M, imageTag, secret)
         
         dirname = os.path.dirname(mainfilepath)
         os.chdir(dirname)
         mainfile = os.path.basename(mainfilepath)
-        create_deploy_docker_image(imageTag, mainfile)
+        # create_deploy_docker_image(imageTag, mainfile)
         
         print(f"{mainfilepath} processed successfully")
         
     except Exception as e:
         print(e)
         # print(f"{mainfile} does not contain an EcidaModule")
```

### Comparing `ecidacli-0.0.8/setup.py` & `ecidacli-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
    long_description = fh.read()
    
 setuptools.setup(
    name='ecidacli',
-   version='0.0.8',
+   version='0.0.9',
    author="Mostafa Hadadian",
    author_email="m.hadadian@rug.nl",
    description="The ECiDA-CLI for python to make things easier",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://gitlab.com/ecida",
    classifiers=[
```

