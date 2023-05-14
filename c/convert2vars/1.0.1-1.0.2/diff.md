# Comparing `tmp/convert2vars-1.0.1.tar.gz` & `tmp/convert2vars-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert2vars-1.0.1.tar", last modified: Tue May  9 16:35:12 2023, max compression
+gzip compressed data, was "convert2vars-1.0.2.tar", last modified: Sun May 14 20:47:30 2023, max compression
```

## Comparing `convert2vars-1.0.1.tar` & `convert2vars-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-09 16:35:12.345400 convert2vars-1.0.1/
--rw-r--r--   0 moriyama   (501) staff       (20)     1061 2023-04-18 19:03:08.000000 convert2vars-1.0.1/LICENSE
--rw-r--r--   0 moriyama   (501) staff       (20)     5194 2023-05-09 16:35:12.344786 convert2vars-1.0.1/PKG-INFO
--rw-r--r--   0 moriyama   (501) staff       (20)     4644 2023-05-09 16:00:02.000000 convert2vars-1.0.1/README.md
-drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-09 16:35:12.313629 convert2vars-1.0.1/convert2vars/
--rwxr-xr-x   0 moriyama   (501) staff       (20)     3417 2023-05-09 16:29:50.000000 convert2vars-1.0.1/convert2vars/__init__.py
--rw-r--r--   0 moriyama   (501) staff       (20)       95 2023-04-18 19:03:08.000000 convert2vars-1.0.1/convert2vars/__main__.py
-drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-09 16:35:12.326753 convert2vars-1.0.1/convert2vars/app/
--rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.1/convert2vars/app/__init__.py
--rw-r--r--   0 moriyama   (501) staff       (20)     1353 2023-05-03 16:12:32.000000 convert2vars-1.0.1/convert2vars/app/app_exception.py
--rw-r--r--   0 moriyama   (501) staff       (20)     6483 2023-05-03 16:50:23.000000 convert2vars-1.0.1/convert2vars/app/app_helper.py
--rw-r--r--   0 moriyama   (501) staff       (20)     1604 2023-05-03 16:56:02.000000 convert2vars-1.0.1/convert2vars/app/app_impl.py
-drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-09 16:35:12.328091 convert2vars-1.0.1/convert2vars/app/command/
--rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.1/convert2vars/app/command/__init__.py
--rw-r--r--   0 moriyama   (501) staff       (20)     2180 2023-05-03 16:50:00.000000 convert2vars-1.0.1/convert2vars/app/command/command_convert.py
--rw-r--r--   0 moriyama   (501) staff       (20)      371 2023-05-03 16:19:18.000000 convert2vars-1.0.1/convert2vars/app/constants.py
-drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-09 16:35:12.330447 convert2vars-1.0.1/convert2vars/formatter/
--rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.1/convert2vars/formatter/__init__.py
--rw-r--r--   0 moriyama   (501) staff       (20)      510 2023-05-03 16:19:35.000000 convert2vars-1.0.1/convert2vars/formatter/json_formatter.py
--rw-r--r--   0 moriyama   (501) staff       (20)      959 2023-05-03 16:20:06.000000 convert2vars-1.0.1/convert2vars/formatter/yaml_formatter.py
-drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-09 16:35:12.331935 convert2vars-1.0.1/convert2vars/importer/
--rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.1/convert2vars/importer/__init__.py
--rw-r--r--   0 moriyama   (501) staff       (20)      724 2023-05-03 16:20:50.000000 convert2vars-1.0.1/convert2vars/importer/file_importer.py
-drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-09 16:35:12.338664 convert2vars-1.0.1/convert2vars/parser/
--rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.1/convert2vars/parser/__init__.py
--rw-r--r--   0 moriyama   (501) staff       (20)     1108 2023-05-09 14:20:37.000000 convert2vars-1.0.1/convert2vars/parser/ini_parser.py
--rw-r--r--   0 moriyama   (501) staff       (20)     1006 2023-05-09 14:20:27.000000 convert2vars-1.0.1/convert2vars/parser/json_parser.py
--rw-r--r--   0 moriyama   (501) staff       (20)     1941 2023-05-09 14:21:52.000000 convert2vars-1.0.1/convert2vars/parser/parse_helper.py
--rw-r--r--   0 moriyama   (501) staff       (20)     1010 2023-05-09 14:22:35.000000 convert2vars-1.0.1/convert2vars/parser/yaml_parser.py
-drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-09 16:35:12.341579 convert2vars-1.0.1/convert2vars/template/
--rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.1/convert2vars/template/__init__.py
--rw-r--r--   0 moriyama   (501) staff       (20)     1474 2023-05-03 16:51:07.000000 convert2vars-1.0.1/convert2vars/template/template_loader.py
--rw-r--r--   0 moriyama   (501) staff       (20)      818 2023-05-03 16:31:19.000000 convert2vars-1.0.1/convert2vars/template/template_render.py
-drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-09 16:35:12.343973 convert2vars-1.0.1/convert2vars/util/
--rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.1/convert2vars/util/__init__.py
--rw-r--r--   0 moriyama   (501) staff       (20)      293 2023-05-03 16:37:25.000000 convert2vars-1.0.1/convert2vars/util/config_util.py
--rw-r--r--   0 moriyama   (501) staff       (20)     1644 2023-05-03 16:34:55.000000 convert2vars-1.0.1/convert2vars/util/logging.py
-drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-09 16:35:12.322270 convert2vars-1.0.1/convert2vars.egg-info/
--rw-r--r--   0 moriyama   (501) staff       (20)     5194 2023-05-09 16:35:12.000000 convert2vars-1.0.1/convert2vars.egg-info/PKG-INFO
--rw-r--r--   0 moriyama   (501) staff       (20)     1098 2023-05-09 16:35:12.000000 convert2vars-1.0.1/convert2vars.egg-info/SOURCES.txt
--rw-r--r--   0 moriyama   (501) staff       (20)        1 2023-05-09 16:35:12.000000 convert2vars-1.0.1/convert2vars.egg-info/dependency_links.txt
--rw-r--r--   0 moriyama   (501) staff       (20)       51 2023-05-09 16:35:12.000000 convert2vars-1.0.1/convert2vars.egg-info/entry_points.txt
--rw-r--r--   0 moriyama   (501) staff       (20)       44 2023-05-09 16:35:12.000000 convert2vars-1.0.1/convert2vars.egg-info/requires.txt
--rw-r--r--   0 moriyama   (501) staff       (20)       13 2023-05-09 16:35:12.000000 convert2vars-1.0.1/convert2vars.egg-info/top_level.txt
--rw-r--r--   0 moriyama   (501) staff       (20)       38 2023-05-09 16:35:12.345626 convert2vars-1.0.1/setup.cfg
--rw-r--r--   0 moriyama   (501) staff       (20)     1006 2023-05-09 16:29:37.000000 convert2vars-1.0.1/setup.py
+drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-14 20:47:30.953860 convert2vars-1.0.2/
+-rw-r--r--   0 moriyama   (501) staff       (20)     1061 2023-04-18 19:03:08.000000 convert2vars-1.0.2/LICENSE
+-rw-r--r--   0 moriyama   (501) staff       (20)     6436 2023-05-14 20:47:30.953064 convert2vars-1.0.2/PKG-INFO
+-rw-r--r--   0 moriyama   (501) staff       (20)     5886 2023-05-14 20:35:56.000000 convert2vars-1.0.2/README.md
+drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-14 20:47:30.800269 convert2vars-1.0.2/convert2vars/
+-rwxr-xr-x   0 moriyama   (501) staff       (20)     3414 2023-05-14 20:29:02.000000 convert2vars-1.0.2/convert2vars/__init__.py
+-rw-r--r--   0 moriyama   (501) staff       (20)       95 2023-04-18 19:03:08.000000 convert2vars-1.0.2/convert2vars/__main__.py
+drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-14 20:47:30.913541 convert2vars-1.0.2/convert2vars/app/
+-rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.2/convert2vars/app/__init__.py
+-rw-r--r--   0 moriyama   (501) staff       (20)     1353 2023-05-03 16:12:32.000000 convert2vars-1.0.2/convert2vars/app/app_exception.py
+-rw-r--r--   0 moriyama   (501) staff       (20)     6483 2023-05-03 16:50:23.000000 convert2vars-1.0.2/convert2vars/app/app_helper.py
+-rw-r--r--   0 moriyama   (501) staff       (20)     1604 2023-05-03 16:56:02.000000 convert2vars-1.0.2/convert2vars/app/app_impl.py
+drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-14 20:47:30.918521 convert2vars-1.0.2/convert2vars/app/command/
+-rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.2/convert2vars/app/command/__init__.py
+-rw-r--r--   0 moriyama   (501) staff       (20)     2180 2023-05-03 16:50:00.000000 convert2vars-1.0.2/convert2vars/app/command/command_convert.py
+-rw-r--r--   0 moriyama   (501) staff       (20)      371 2023-05-03 16:19:18.000000 convert2vars-1.0.2/convert2vars/app/constants.py
+drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-14 20:47:30.928122 convert2vars-1.0.2/convert2vars/formatter/
+-rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.2/convert2vars/formatter/__init__.py
+-rw-r--r--   0 moriyama   (501) staff       (20)      510 2023-05-03 16:19:35.000000 convert2vars-1.0.2/convert2vars/formatter/json_formatter.py
+-rw-r--r--   0 moriyama   (501) staff       (20)      959 2023-05-03 16:20:06.000000 convert2vars-1.0.2/convert2vars/formatter/yaml_formatter.py
+drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-14 20:47:30.930729 convert2vars-1.0.2/convert2vars/importer/
+-rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.2/convert2vars/importer/__init__.py
+-rw-r--r--   0 moriyama   (501) staff       (20)      724 2023-05-03 16:20:50.000000 convert2vars-1.0.2/convert2vars/importer/file_importer.py
+drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-14 20:47:30.938116 convert2vars-1.0.2/convert2vars/parser/
+-rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.2/convert2vars/parser/__init__.py
+-rw-r--r--   0 moriyama   (501) staff       (20)     1108 2023-05-09 14:20:37.000000 convert2vars-1.0.2/convert2vars/parser/ini_parser.py
+-rw-r--r--   0 moriyama   (501) staff       (20)     1006 2023-05-09 14:20:27.000000 convert2vars-1.0.2/convert2vars/parser/json_parser.py
+-rw-r--r--   0 moriyama   (501) staff       (20)     1941 2023-05-09 14:21:52.000000 convert2vars-1.0.2/convert2vars/parser/parse_helper.py
+-rw-r--r--   0 moriyama   (501) staff       (20)     1010 2023-05-09 14:22:35.000000 convert2vars-1.0.2/convert2vars/parser/yaml_parser.py
+drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-14 20:47:30.943879 convert2vars-1.0.2/convert2vars/template/
+-rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.2/convert2vars/template/__init__.py
+-rw-r--r--   0 moriyama   (501) staff       (20)     1474 2023-05-03 16:51:07.000000 convert2vars-1.0.2/convert2vars/template/template_loader.py
+-rw-r--r--   0 moriyama   (501) staff       (20)      818 2023-05-03 16:31:19.000000 convert2vars-1.0.2/convert2vars/template/template_render.py
+drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-14 20:47:30.951283 convert2vars-1.0.2/convert2vars/util/
+-rw-r--r--   0 moriyama   (501) staff       (20)        0 2023-04-18 19:03:08.000000 convert2vars-1.0.2/convert2vars/util/__init__.py
+-rw-r--r--   0 moriyama   (501) staff       (20)      293 2023-05-03 16:37:25.000000 convert2vars-1.0.2/convert2vars/util/config_util.py
+-rw-r--r--   0 moriyama   (501) staff       (20)     1644 2023-05-03 16:34:55.000000 convert2vars-1.0.2/convert2vars/util/logging.py
+drwxr-xr-x   0 moriyama   (501) staff       (20)        0 2023-05-14 20:47:30.844614 convert2vars-1.0.2/convert2vars.egg-info/
+-rw-r--r--   0 moriyama   (501) staff       (20)     6436 2023-05-14 20:47:29.000000 convert2vars-1.0.2/convert2vars.egg-info/PKG-INFO
+-rw-r--r--   0 moriyama   (501) staff       (20)     1098 2023-05-14 20:47:30.000000 convert2vars-1.0.2/convert2vars.egg-info/SOURCES.txt
+-rw-r--r--   0 moriyama   (501) staff       (20)        1 2023-05-14 20:47:29.000000 convert2vars-1.0.2/convert2vars.egg-info/dependency_links.txt
+-rw-r--r--   0 moriyama   (501) staff       (20)       51 2023-05-14 20:47:29.000000 convert2vars-1.0.2/convert2vars.egg-info/entry_points.txt
+-rw-r--r--   0 moriyama   (501) staff       (20)       44 2023-05-14 20:47:29.000000 convert2vars-1.0.2/convert2vars.egg-info/requires.txt
+-rw-r--r--   0 moriyama   (501) staff       (20)       13 2023-05-14 20:47:30.000000 convert2vars-1.0.2/convert2vars.egg-info/top_level.txt
+-rw-r--r--   0 moriyama   (501) staff       (20)       38 2023-05-14 20:47:30.954071 convert2vars-1.0.2/setup.cfg
+-rw-r--r--   0 moriyama   (501) staff       (20)     1006 2023-05-14 20:29:41.000000 convert2vars-1.0.2/setup.py
```

### Comparing `convert2vars-1.0.1/LICENSE` & `convert2vars-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/PKG-INFO` & `convert2vars-1.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,18 @@
-Metadata-Version: 2.1
-Name: convert2vars
-Version: 1.0.1
-Summary: A small tool for mutual conversion of JSON, YAML with embedded parameters.
-Home-page: https://github.com/t-m0riyama/convert2vars
-Author: t-m0riyama
-Author-email: 3154232+t-m0riyama@users.noreply.github.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Text Processing :: Markup
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 convert2vars
 =============
 
 A small tool for mutual conversion of JSON, YAML with embedded parameters.
-Parameter processing can take advantage of the powerful features of the Jinja2 template engine.
+Parameter processing is handled by the powerful Jinja2 template engine.
+JSON, which is often used in APIs, and YAML, which is adopted by popular platforms such as kubernetes (k8s) and ansible, can be converted to each other and dynamic parameter value editing can be performed.
 
 *This document has been translated into English by machine translation. Please note that some parts may be inaccurate.*
 
+[[Japanese]](./README-ja.md "Japanese README")
+
 ## Installation
 ```
 $ pip install convert2vars
 ```
 
 ## Requirements
 * Python 3.7 or later
@@ -119,14 +107,42 @@
   REPLICAS=3
   CONTAINER_PORT=8080
   ```
   - When using a parameter file, use the -i and -t options together.
   ```
   $ convert2vars convert -t k8s-deployment.yml -i k8s-parameter.json
   ```
+### Specifying complex parameter values
+Parameter values with complex structures such as lists and hashes can be specified in JSON format.
+Parameter values enclosed in [[] or {} are handled as JSON format.
+
+The following is an example of specifying a list and a hash as parameter values.
+
+```
+$ cat complex_parameters.yml
+instances: {{ TARGET_INSTANCES }}
+instance_properties: {{ INSTANCE_PROPERTIES }}
+
+$ convert2vars convert -e TARGET_INSTANCES='["vm01","vm02"]' -e INSTANCE_PROPERTIES='{"instance_type": "m1.small"}' -t complex_parameters.yml
+instances: ['vm01', 'vm02']
+instance_properties: {'instance_type': 'm1.small'}
+```
+
+Also, by using a parameter file, complex parameter values can be specified in YAML as well as JSON. The following results are the same as the previous example with the -e option.
+```
+$ cat complex_parameters.yml
+TARGET_INSTANCES:
+  - "vm01"
+  - "vm02"
+INSTANCE_PROPERTIES:
+  instance_type: "m1.small"
+
+$ convert2vars convert -i complex_parameters.yml -t complex_parameters.yml
+```
+
 
 ### Template engine support
   The filter, conditional branching, and iteration functions provided by Jinja2 can be used without modification. In the following example, since the parameter values are not explicitly specified, they are converted to the default values of 2 and 80 by Jinja2's default filter.
 
 ```
 $ convert2vars convert -t samples/templates/k8s-deployment.yml
 apiVersion: apps/v1
```

### Comparing `convert2vars-1.0.1/README.md` & `convert2vars-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,33 @@
+Metadata-Version: 2.1
+Name: convert2vars
+Version: 1.0.2
+Summary: A small tool for mutual conversion of JSON, YAML with embedded parameters.
+Home-page: https://github.com/t-m0riyama/convert2vars
+Author: t-m0riyama
+Author-email: 3154232+t-m0riyama@users.noreply.github.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Text Processing :: Markup
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 convert2vars
 =============
 
 A small tool for mutual conversion of JSON, YAML with embedded parameters.
-Parameter processing can take advantage of the powerful features of the Jinja2 template engine.
+Parameter processing is handled by the powerful Jinja2 template engine.
+JSON, which is often used in APIs, and YAML, which is adopted by popular platforms such as kubernetes (k8s) and ansible, can be converted to each other and dynamic parameter value editing can be performed.
 
 *This document has been translated into English by machine translation. Please note that some parts may be inaccurate.*
 
+[[Japanese]](./README-ja.md "Japanese README")
+
 ## Installation
 ```
 $ pip install convert2vars
 ```
 
 ## Requirements
 * Python 3.7 or later
@@ -104,14 +122,42 @@
   REPLICAS=3
   CONTAINER_PORT=8080
   ```
   - When using a parameter file, use the -i and -t options together.
   ```
   $ convert2vars convert -t k8s-deployment.yml -i k8s-parameter.json
   ```
+### Specifying complex parameter values
+Parameter values with complex structures such as lists and hashes can be specified in JSON format.
+Parameter values enclosed in [[] or {} are handled as JSON format.
+
+The following is an example of specifying a list and a hash as parameter values.
+
+```
+$ cat complex_parameters.yml
+instances: {{ TARGET_INSTANCES }}
+instance_properties: {{ INSTANCE_PROPERTIES }}
+
+$ convert2vars convert -e TARGET_INSTANCES='["vm01","vm02"]' -e INSTANCE_PROPERTIES='{"instance_type": "m1.small"}' -t complex_parameters.yml
+instances: ['vm01', 'vm02']
+instance_properties: {'instance_type': 'm1.small'}
+```
+
+Also, by using a parameter file, complex parameter values can be specified in YAML as well as JSON. The following results are the same as the previous example with the -e option.
+```
+$ cat complex_parameters.yml
+TARGET_INSTANCES:
+  - "vm01"
+  - "vm02"
+INSTANCE_PROPERTIES:
+  instance_type: "m1.small"
+
+$ convert2vars convert -i complex_parameters.yml -t complex_parameters.yml
+```
+
 
 ### Template engine support
   The filter, conditional branching, and iteration functions provided by Jinja2 can be used without modification. In the following example, since the parameter values are not explicitly specified, they are converted to the default values of 2 and 80 by Jinja2's default filter.
 
 ```
 $ convert2vars convert -t samples/templates/k8s-deployment.yml
 apiVersion: apps/v1
```

### Comparing `convert2vars-1.0.1/convert2vars/__init__.py` & `convert2vars-1.0.2/convert2vars/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from convert2vars.app.app_impl import AppImpl
 import click
 import pathlib
 
 base_path = (pathlib.Path(__file__)).parent.parent
 
 __appname__ = 'convert2vars'
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 
 @click.group(help='Load a template, embed the value of a variable, and output it.')
 @click.option(
     '--config-file',
     '-c',
     type=str,
@@ -39,15 +39,15 @@
 @click.option(
     '--vars',
     '-e',
     type=str,
     multiple=True,
     metavar='VARS',
     show_default=True,
-    help='Specify a variable and its value（ex. -e var1=X -e var2=y）')
+    help='Specify a variable and its value (ex. -e var1=X -e var2=y)')
 @click.option(
     '--use-environment',
     '-E',
     is_flag=True,
     metavar='USE_ENVIRONMENT',
     default=False,
     show_default=True,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `convert2vars-1.0.1/convert2vars/app/app_exception.py` & `convert2vars-1.0.2/convert2vars/app/app_exception.py`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/convert2vars/app/app_helper.py` & `convert2vars-1.0.2/convert2vars/app/app_helper.py`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/convert2vars/app/app_impl.py` & `convert2vars-1.0.2/convert2vars/app/app_impl.py`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/convert2vars/app/command/command_convert.py` & `convert2vars-1.0.2/convert2vars/app/command/command_convert.py`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/convert2vars/formatter/yaml_formatter.py` & `convert2vars-1.0.2/convert2vars/formatter/yaml_formatter.py`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/convert2vars/importer/file_importer.py` & `convert2vars-1.0.2/convert2vars/importer/file_importer.py`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/convert2vars/parser/ini_parser.py` & `convert2vars-1.0.2/convert2vars/parser/ini_parser.py`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/convert2vars/parser/json_parser.py` & `convert2vars-1.0.2/convert2vars/parser/json_parser.py`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/convert2vars/parser/parse_helper.py` & `convert2vars-1.0.2/convert2vars/parser/parse_helper.py`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/convert2vars/parser/yaml_parser.py` & `convert2vars-1.0.2/convert2vars/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/convert2vars/template/template_loader.py` & `convert2vars-1.0.2/convert2vars/template/template_loader.py`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/convert2vars/template/template_render.py` & `convert2vars-1.0.2/convert2vars/template/template_render.py`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/convert2vars/util/logging.py` & `convert2vars-1.0.2/convert2vars/util/logging.py`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/convert2vars.egg-info/PKG-INFO` & `convert2vars-1.0.2/convert2vars.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert2vars
-Version: 1.0.1
+Version: 1.0.2
 Summary: A small tool for mutual conversion of JSON, YAML with embedded parameters.
 Home-page: https://github.com/t-m0riyama/convert2vars
 Author: t-m0riyama
 Author-email: 3154232+t-m0riyama@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,18 +13,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 convert2vars
 =============
 
 A small tool for mutual conversion of JSON, YAML with embedded parameters.
-Parameter processing can take advantage of the powerful features of the Jinja2 template engine.
+Parameter processing is handled by the powerful Jinja2 template engine.
+JSON, which is often used in APIs, and YAML, which is adopted by popular platforms such as kubernetes (k8s) and ansible, can be converted to each other and dynamic parameter value editing can be performed.
 
 *This document has been translated into English by machine translation. Please note that some parts may be inaccurate.*
 
+[[Japanese]](./README-ja.md "Japanese README")
+
 ## Installation
 ```
 $ pip install convert2vars
 ```
 
 ## Requirements
 * Python 3.7 or later
@@ -119,14 +122,42 @@
   REPLICAS=3
   CONTAINER_PORT=8080
   ```
   - When using a parameter file, use the -i and -t options together.
   ```
   $ convert2vars convert -t k8s-deployment.yml -i k8s-parameter.json
   ```
+### Specifying complex parameter values
+Parameter values with complex structures such as lists and hashes can be specified in JSON format.
+Parameter values enclosed in [[] or {} are handled as JSON format.
+
+The following is an example of specifying a list and a hash as parameter values.
+
+```
+$ cat complex_parameters.yml
+instances: {{ TARGET_INSTANCES }}
+instance_properties: {{ INSTANCE_PROPERTIES }}
+
+$ convert2vars convert -e TARGET_INSTANCES='["vm01","vm02"]' -e INSTANCE_PROPERTIES='{"instance_type": "m1.small"}' -t complex_parameters.yml
+instances: ['vm01', 'vm02']
+instance_properties: {'instance_type': 'm1.small'}
+```
+
+Also, by using a parameter file, complex parameter values can be specified in YAML as well as JSON. The following results are the same as the previous example with the -e option.
+```
+$ cat complex_parameters.yml
+TARGET_INSTANCES:
+  - "vm01"
+  - "vm02"
+INSTANCE_PROPERTIES:
+  instance_type: "m1.small"
+
+$ convert2vars convert -i complex_parameters.yml -t complex_parameters.yml
+```
+
 
 ### Template engine support
   The filter, conditional branching, and iteration functions provided by Jinja2 can be used without modification. In the following example, since the parameter values are not explicitly specified, they are converted to the default values of 2 and 80 by Jinja2's default filter.
 
 ```
 $ convert2vars convert -t samples/templates/k8s-deployment.yml
 apiVersion: apps/v1
```

### Comparing `convert2vars-1.0.1/convert2vars.egg-info/SOURCES.txt` & `convert2vars-1.0.2/convert2vars.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `convert2vars-1.0.1/setup.py` & `convert2vars-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="convert2vars",
-    version="1.0.1",
+    version="1.0.2",
     install_requires=[
         "click",
         "python-dotenv",
         "iniconfig",
         "Jinja2",
         "PyYAML",
     ],
```

