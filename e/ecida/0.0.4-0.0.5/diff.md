# Comparing `tmp/ecida-0.0.4.tar.gz` & `tmp/ecida-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecida-0.0.4.tar", last modified: Sun May  7 17:18:16 2023, max compression
+gzip compressed data, was "ecida-0.0.5.tar", last modified: Sat May 13 23:30:17 2023, max compression
```

## Comparing `ecida-0.0.4.tar` & `ecida-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-07 17:18:16.388783 ecida-0.0.4/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     4789 2023-05-07 17:17:33.000000 ecida-0.0.4/Ecida.py
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-07 17:18:16.388783 ecida-0.0.4/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-03-09 17:51:25.000000 ecida-0.0.4/README.md
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-07 17:18:16.388783 ecida-0.0.4/ecida.egg-info/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-07 17:18:16.000000 ecida-0.0.4/ecida.egg-info/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      171 2023-05-07 17:18:16.000000 ecida-0.0.4/ecida.egg-info/SOURCES.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-07 17:18:16.000000 ecida-0.0.4/ecida.egg-info/dependency_links.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       13 2023-05-07 17:18:16.000000 ecida-0.0.4/ecida.egg-info/requires.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-07 17:18:16.000000 ecida-0.0.4/ecida.egg-info/top_level.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-07 17:18:16.388783 ecida-0.0.4/setup.cfg
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      639 2023-05-07 17:17:57.000000 ecida-0.0.4/setup.py
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-13 23:30:17.095818 ecida-0.0.5/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     6095 2023-05-13 23:27:27.000000 ecida-0.0.5/Ecida.py
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-13 23:30:17.095818 ecida-0.0.5/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-05-13 22:19:01.000000 ecida-0.0.5/README.md
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-13 23:30:17.095818 ecida-0.0.5/ecida.egg-info/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-13 23:30:17.000000 ecida-0.0.5/ecida.egg-info/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-05-13 23:30:17.000000 ecida-0.0.5/ecida.egg-info/SOURCES.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-13 23:30:17.000000 ecida-0.0.5/ecida.egg-info/dependency_links.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       13 2023-05-13 23:30:17.000000 ecida-0.0.5/ecida.egg-info/requires.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-13 23:30:17.000000 ecida-0.0.5/ecida.egg-info/top_level.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-13 23:30:17.095818 ecida-0.0.5/setup.cfg
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      639 2023-05-13 23:29:51.000000 ecida-0.0.5/setup.py
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      693 2023-05-13 23:29:51.000000 ecida-0.0.5/test.py
```

### Comparing `ecida-0.0.4/Ecida.py` & `ecida-0.0.5/Ecida.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 import os 
+from datetime import datetime
 from kafka import KafkaConsumer, KafkaProducer
+import shutil
 
-# from enum import Enum
-
-# # class DType(Enum):
-# #     STRING = "string"
-# #     INT = "integer"
-# #     DOUBLE = "double"
-    
-#     def to_yaml(dumper, data):
-#         return dumper.represent_scalar('!DType', data.value)
+def isDeployed():
+    flag_value = os.getenv("ECIDA_DEPLOY", "").lower()
+    return flag_value == "true"
+
+def now():
+    return "[" + datetime.now().strftime("%Y-%m-%d %H:%M:%S") + "]"
+
+
+def create_directory(directory_path):
+    if os.path.exists(directory_path):
+        print(f"Deleting existing directory: {directory_path}")
+        shutil.rmtree(directory_path)
+
+    try:
+        print(f"Creating directory: {directory_path}")
+        os.mkdir(directory_path)
+    except OSError as e:
+        print(f"Failed to create directory: {directory_path}")
+        print(f"Error: {str(e)}")    
 
 class EcidaModule:
     def __init__(self, name, version):
         self._name = name
         self._version = version
         self._inputs = {}
         self._outputs = {}
         self._topics_envVars = {}
         self._topics_names = {}
         self._consumers = {}
         self._directories = {}        
         self._producer = None
         self._initialized = False
+        self._deployed = isDeployed()
     
     @property
     def name(self):
         return self._name
 
     @property
     def version(self):
@@ -52,14 +65,18 @@
     def name(self, value):
         raise AttributeError("Attribute is read-only")
 
     @version.setter
     def version(self, value):
         raise AttributeError("Attribute is read-only")
     
+    @version.setter
+    def deployed(self, value):
+        raise AttributeError("Attribute is read-only")
+    
     def add_input(self, inp: str, type):
         self._inputs[inp] = type
         self._topics_envVars[inp] = "KAFKA_TOPIC_"+ inp.upper()
         
     def add_output(self, out: str, type):
         self._outputs[out] = type
         self._topics_envVars[out] = "KAFKA_TOPIC_"+ out.upper()
@@ -77,63 +94,79 @@
     def add_input_from_git(self, name: str, git: str, path: str):
         self.add_input_directory(name)
         self.__add_git_to_directory(name, git,path)
     
     def add_output_to_git(self, name: str, git: str, path: str):
         self.add_output_directory(name)
         self.__add_git_to_directory(name, git,path)
+        
+    def get_path(self, name):
+        if self._deployed:
+            return "/"+name
+        else:
+            return "./"+name
     
     def __add_git_to_directory(self, name: str, git: str, path: str):
         self._directories[name]["source"] = git
         self._directories[name]["folder"] = path
     
     def to_yaml(self) -> str:
         return str(self._inputs) + "\n" + str(self._outputs)
     
     def initialize(self):
-        self._KAFKA_BOOTSTRAP_SERVER = os.environ['KAFKA_BOOTSTRAP_SERVER']
-        self._KAFKA_SASL_MECHANISM = os.environ['KAFKA_SASL_MECHANISM']
-        self._KAFKA_SECURITY_PROTOCOL = os.environ['KAFKA_SECURITY_PROTOCOL']
-        self._KAFKA_USERNAME = os.environ['KAFKA_USERNAME']
-        self._KAFKA_PASSWORD = os.environ['KAFKA_PASSWORD']
-        self._KAFKA_GROUP_ID = os.environ['KAFKA_USERNAME']
-        
-        for key, value in self._inputs.items():
-            if value == "directory":
-                continue
-            topicName = os.environ[self._topics_envVars[key]]
-            self._topics_names[key] = topicName
-            consumer = KafkaConsumer(topicName, bootstrap_servers = self._KAFKA_BOOTSTRAP_SERVER, 
-                            sasl_plain_username= self._KAFKA_USERNAME,
-                            sasl_plain_password= self._KAFKA_PASSWORD,
-                            sasl_mechanism=self._KAFKA_SASL_MECHANISM,
-                            security_protocol=self._KAFKA_SECURITY_PROTOCOL,
-                            group_id= self._KAFKA_GROUP_ID)
-            self._consumers[key] = consumer
+        if self._deployed == True:
+            self._KAFKA_BOOTSTRAP_SERVER = os.environ['KAFKA_BOOTSTRAP_SERVER']
+            self._KAFKA_SASL_MECHANISM = os.environ['KAFKA_SASL_MECHANISM']
+            self._KAFKA_SECURITY_PROTOCOL = os.environ['KAFKA_SECURITY_PROTOCOL']
+            self._KAFKA_USERNAME = os.environ['KAFKA_USERNAME']
+            self._KAFKA_PASSWORD = os.environ['KAFKA_PASSWORD']
+            self._KAFKA_GROUP_ID = os.environ['KAFKA_USERNAME']
             
-        if len(self._outputs) > 0 :
-            self._producer = KafkaProducer(bootstrap_servers = self._KAFKA_BOOTSTRAP_SERVER,
-                            sasl_plain_username= self._KAFKA_USERNAME,
-                            sasl_plain_password= self._KAFKA_PASSWORD,
-                            sasl_mechanism=self._KAFKA_SASL_MECHANISM,
-                            security_protocol=self._KAFKA_SECURITY_PROTOCOL)
-        
-        for key, _ in self._outputs.items() :
-            topicName = os.environ[self._topics_envVars[key]]
-            self._topics_names[key] = topicName
-        
-        self._initialized = True
+            for key, value in self._inputs.items():
+                if value == "directory":
+                    continue
+                topicName = os.environ[self._topics_envVars[key]]
+                self._topics_names[key] = topicName
+                consumer = KafkaConsumer(topicName, bootstrap_servers = self._KAFKA_BOOTSTRAP_SERVER, 
+                                sasl_plain_username= self._KAFKA_USERNAME,
+                                sasl_plain_password= self._KAFKA_PASSWORD,
+                                sasl_mechanism=self._KAFKA_SASL_MECHANISM,
+                                security_protocol=self._KAFKA_SECURITY_PROTOCOL,
+                                group_id= self._KAFKA_GROUP_ID)
+                self._consumers[key] = consumer
+                
+            if len(self._outputs) > 0 :
+                self._producer = KafkaProducer(bootstrap_servers = self._KAFKA_BOOTSTRAP_SERVER,
+                                sasl_plain_username= self._KAFKA_USERNAME,
+                                sasl_plain_password= self._KAFKA_PASSWORD,
+                                sasl_mechanism=self._KAFKA_SASL_MECHANISM,
+                                security_protocol=self._KAFKA_SECURITY_PROTOCOL)
+            
+            for key, _ in self._outputs.items() :
+                topicName = os.environ[self._topics_envVars[key]]
+                self._topics_names[key] = topicName
             
+            self._initialized = True
+        else:
+            for output in self._outputs:
+                if output in self._directories:
+                    create_directory(self._directories[output]["localPath"])
 
             
   
-    def push(self, output: str, message) -> bool:
-        if output in self._outputs:
-            self._producer.send(self._topics_names[output], value= str(message).encode("utf-8"))
-            return True
-        return False
-    
-    def pull(self, input: str) -> any:
-        if input in self._inputs:
-            for msg in self._consumers[input]:
-                return msg.value.decode("utf-8")
-        return None
+    def push(self, output_channel: str, message) -> bool:
+        if self._deployed:
+            if output_channel in self._outputs:
+                self._producer.send(self._topics_names[output_channel], value= str(message).encode("utf-8"))
+                return True
+            return False
+        else:
+            return print(f"{now()} {output_channel}: {message}")
+    
+    def pull(self, input_channel: str) -> any:
+        if self._deployed:
+            if input_channel in self._inputs:
+                for msg in self._consumers[input_channel]:
+                    return msg.value.decode("utf-8")
+            return None
+        else:
+            return input(f"{now()} {input_channel}:")
```

### Comparing `ecida-0.0.4/PKG-INFO` & `ecida-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecida
-Version: 0.0.4
+Version: 0.0.5
 Summary: The ECiDA-python to make things easier
 Home-page: https://gitlab.com/ecida
 Author: Mostafa Hadadian
 Author-email: m.hadadian@rug.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecida-0.0.4/ecida.egg-info/PKG-INFO` & `ecida-0.0.5/ecida.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecida
-Version: 0.0.4
+Version: 0.0.5
 Summary: The ECiDA-python to make things easier
 Home-page: https://gitlab.com/ecida
 Author: Mostafa Hadadian
 Author-email: m.hadadian@rug.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecida-0.0.4/setup.py` & `ecida-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
    long_description = fh.read()
    
 setuptools.setup(
    name='ecida',
-   version='0.0.4',
+   version='0.0.5',
    author="Mostafa Hadadian",
    author_email="m.hadadian@rug.nl",
    description="The ECiDA-python to make things easier",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://gitlab.com/ecida",
    packages=["."] or setuptools.find_packages(),
```

