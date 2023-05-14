# Comparing `tmp/ecida-0.0.5.tar.gz` & `tmp/ecida-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecida-0.0.5.tar", last modified: Sat May 13 23:30:17 2023, max compression
+gzip compressed data, was "ecida-0.0.6.tar", last modified: Sun May 14 11:03:53 2023, max compression
```

## Comparing `ecida-0.0.5.tar` & `ecida-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-13 23:30:17.095818 ecida-0.0.5/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     6095 2023-05-13 23:27:27.000000 ecida-0.0.5/Ecida.py
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-13 23:30:17.095818 ecida-0.0.5/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-05-13 22:19:01.000000 ecida-0.0.5/README.md
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-13 23:30:17.095818 ecida-0.0.5/ecida.egg-info/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-13 23:30:17.000000 ecida-0.0.5/ecida.egg-info/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-05-13 23:30:17.000000 ecida-0.0.5/ecida.egg-info/SOURCES.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-13 23:30:17.000000 ecida-0.0.5/ecida.egg-info/dependency_links.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       13 2023-05-13 23:30:17.000000 ecida-0.0.5/ecida.egg-info/requires.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-13 23:30:17.000000 ecida-0.0.5/ecida.egg-info/top_level.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-13 23:30:17.095818 ecida-0.0.5/setup.cfg
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      639 2023-05-13 23:29:51.000000 ecida-0.0.5/setup.py
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      693 2023-05-13 23:29:51.000000 ecida-0.0.5/test.py
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-14 11:03:53.169649 ecida-0.0.6/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     6169 2023-05-14 10:58:13.000000 ecida-0.0.6/Ecida.py
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-14 11:03:53.169649 ecida-0.0.6/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-05-13 22:19:01.000000 ecida-0.0.6/README.md
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-14 11:03:53.169649 ecida-0.0.6/ecida.egg-info/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-14 11:03:53.000000 ecida-0.0.6/ecida.egg-info/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      171 2023-05-14 11:03:53.000000 ecida-0.0.6/ecida.egg-info/SOURCES.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-14 11:03:53.000000 ecida-0.0.6/ecida.egg-info/dependency_links.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       13 2023-05-14 11:03:53.000000 ecida-0.0.6/ecida.egg-info/requires.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-14 11:03:53.000000 ecida-0.0.6/ecida.egg-info/top_level.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-14 11:03:53.169649 ecida-0.0.6/setup.cfg
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      639 2023-05-14 10:58:49.000000 ecida-0.0.6/setup.py
```

### Comparing `ecida-0.0.5/Ecida.py` & `ecida-0.0.6/Ecida.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,17 @@
             if len(self._outputs) > 0 :
                 self._producer = KafkaProducer(bootstrap_servers = self._KAFKA_BOOTSTRAP_SERVER,
                                 sasl_plain_username= self._KAFKA_USERNAME,
                                 sasl_plain_password= self._KAFKA_PASSWORD,
                                 sasl_mechanism=self._KAFKA_SASL_MECHANISM,
                                 security_protocol=self._KAFKA_SECURITY_PROTOCOL)
             
-            for key, _ in self._outputs.items() :
+            for key, value in self._outputs.items() :
+                if value == "directory":
+                    continue
                 topicName = os.environ[self._topics_envVars[key]]
                 self._topics_names[key] = topicName
             
             self._initialized = True
         else:
             for output in self._outputs:
                 if output in self._directories:
```

### Comparing `ecida-0.0.5/PKG-INFO` & `ecida-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecida
-Version: 0.0.5
+Version: 0.0.6
 Summary: The ECiDA-python to make things easier
 Home-page: https://gitlab.com/ecida
 Author: Mostafa Hadadian
 Author-email: m.hadadian@rug.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecida-0.0.5/ecida.egg-info/PKG-INFO` & `ecida-0.0.6/ecida.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecida
-Version: 0.0.5
+Version: 0.0.6
 Summary: The ECiDA-python to make things easier
 Home-page: https://gitlab.com/ecida
 Author: Mostafa Hadadian
 Author-email: m.hadadian@rug.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecida-0.0.5/setup.py` & `ecida-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
    long_description = fh.read()
    
 setuptools.setup(
    name='ecida',
-   version='0.0.5',
+   version='0.0.6',
    author="Mostafa Hadadian",
    author_email="m.hadadian@rug.nl",
    description="The ECiDA-python to make things easier",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://gitlab.com/ecida",
    packages=["."] or setuptools.find_packages(),
```

