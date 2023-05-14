# Comparing `tmp/leap_model_parser-0.1.94.tar.gz` & `tmp/leap_model_parser-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_model_parser-0.1.94.tar", max compression
+gzip compressed data, was "leap_model_parser-0.1.95.tar", max compression
```

## Comparing `leap_model_parser-0.1.94.tar` & `leap_model_parser-0.1.95.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2022-07-18 07:29:48.936891 leap_model_parser-0.1.94/LICENSE
--rw-r--r--   0        0        0       68 2022-07-18 07:29:48.936891 leap_model_parser-0.1.94/README.md
--rw-r--r--   0        0        0      132 2022-07-18 07:29:48.936891 leap_model_parser-0.1.94/leap_model_parser/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.94/leap_model_parser/contract/__init__.py
--rw-r--r--   0        0        0      691 2023-04-04 06:58:15.124228 leap_model_parser-0.1.94/leap_model_parser/contract/importmodelresponse.py
--rw-r--r--   0        0        0    43326 2023-05-08 06:06:56.507686 leap_model_parser-0.1.94/leap_model_parser/contract/nodedata.py
--rw-r--r--   0        0        0   416303 2023-05-08 06:04:30.540347 leap_model_parser-0.1.94/leap_model_parser/contract/ui_components.json
--rw-r--r--   0        0        0    15485 2023-04-04 06:58:15.124228 leap_model_parser-0.1.94/leap_model_parser/keras_json_model_import.py
--rw-r--r--   0        0        0     6766 2023-04-04 06:58:15.124228 leap_model_parser-0.1.94/leap_model_parser/model_parser.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.94/leap_model_parser/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.940891 leap_model_parser-0.1.94/leap_model_parser/utils/layerpedia/__init__.py
--rw-r--r--   0        0        0     9291 2022-07-18 07:29:48.940891 leap_model_parser-0.1.94/leap_model_parser/utils/layerpedia/layerpedia.py
--rw-r--r--   0        0        0        1 2022-07-18 07:29:48.940891 leap_model_parser-0.1.94/leap_model_parser/utils/tlinspection/__init__.py
--rw-r--r--   0        0        0     2804 2023-05-08 06:00:02.429640 leap_model_parser-0.1.94/leap_model_parser/utils/tlinspection/leapinspection.py
--rw-r--r--   0        0        0      111 2022-07-18 07:29:48.940891 leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/__init__.py
--rw-r--r--   0        0        0     3035 2022-07-18 07:29:48.940891 leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/generatenodedata.py
--rw-r--r--   0        0        0     6768 2023-05-08 06:06:56.515687 leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
--rw-r--r--   0        0        0    19604 2023-04-04 06:58:15.124228 leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/ui_components_config.yaml
--rw-r--r--   0        0        0     1052 2023-05-09 06:05:22.198667 leap_model_parser-0.1.94/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 leap_model_parser-0.1.94/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-03-21 10:18:19.706997 leap_model_parser-0.1.95/LICENSE
+-rw-r--r--   0        0        0       68 2022-03-21 10:18:19.707319 leap_model_parser-0.1.95/README.md
+-rw-r--r--   0        0        0      132 2022-06-01 08:37:39.139932 leap_model_parser-0.1.95/leap_model_parser/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-21 10:18:19.707654 leap_model_parser-0.1.95/leap_model_parser/contract/__init__.py
+-rw-r--r--   0        0        0      691 2023-03-13 09:16:28.638511 leap_model_parser-0.1.95/leap_model_parser/contract/importmodelresponse.py
+-rw-r--r--   0        0        0    43326 2023-05-14 16:30:36.723913 leap_model_parser-0.1.95/leap_model_parser/contract/nodedata.py
+-rw-r--r--   0        0        0   416303 2023-05-14 16:30:36.725601 leap_model_parser-0.1.95/leap_model_parser/contract/ui_components.json
+-rw-r--r--   0        0        0    15485 2023-05-14 16:30:42.392645 leap_model_parser-0.1.95/leap_model_parser/keras_json_model_import.py
+-rw-r--r--   0        0        0     6766 2023-05-14 16:30:42.392981 leap_model_parser-0.1.95/leap_model_parser/model_parser.py
+-rw-r--r--   0        0        0        0 2022-05-26 12:03:02.077038 leap_model_parser-0.1.95/leap_model_parser/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-26 12:03:02.077489 leap_model_parser-0.1.95/leap_model_parser/utils/layerpedia/__init__.py
+-rw-r--r--   0        0        0     9291 2022-05-26 12:03:02.078100 leap_model_parser-0.1.95/leap_model_parser/utils/layerpedia/layerpedia.py
+-rw-r--r--   0        0        0        1 2022-05-26 12:03:02.078264 leap_model_parser-0.1.95/leap_model_parser/utils/tlinspection/__init__.py
+-rw-r--r--   0        0        0     2804 2023-05-14 16:30:36.727364 leap_model_parser-0.1.95/leap_model_parser/utils/tlinspection/leapinspection.py
+-rw-r--r--   0        0        0      111 2022-05-26 12:03:02.079257 leap_model_parser-0.1.95/leap_model_parser/utils/uicomponents/__init__.py
+-rw-r--r--   0        0        0     3035 2022-05-26 12:03:02.079831 leap_model_parser-0.1.95/leap_model_parser/utils/uicomponents/generatenodedata.py
+-rw-r--r--   0        0        0     6775 2023-05-14 16:30:36.728911 leap_model_parser-0.1.95/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
+-rw-r--r--   0        0        0    19604 2023-05-01 11:24:32.069577 leap_model_parser-0.1.95/leap_model_parser/utils/uicomponents/ui_components_config.yaml
+-rw-r--r--   0        0        0     1052 2023-05-14 16:32:15.579123 leap_model_parser-0.1.95/pyproject.toml
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 leap_model_parser-0.1.95/PKG-INFO
```

### Comparing `leap_model_parser-0.1.94/LICENSE` & `leap_model_parser-0.1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.94/leap_model_parser/contract/importmodelresponse.py` & `leap_model_parser-0.1.95/leap_model_parser/contract/importmodelresponse.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.94/leap_model_parser/contract/nodedata.py` & `leap_model_parser-0.1.95/leap_model_parser/contract/nodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.94/leap_model_parser/contract/ui_components.json` & `leap_model_parser-0.1.95/leap_model_parser/contract/ui_components.json`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.94/leap_model_parser/keras_json_model_import.py` & `leap_model_parser-0.1.95/leap_model_parser/keras_json_model_import.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.94/leap_model_parser/model_parser.py` & `leap_model_parser-0.1.95/leap_model_parser/model_parser.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.94/leap_model_parser/utils/layerpedia/layerpedia.py` & `leap_model_parser-0.1.95/leap_model_parser/utils/layerpedia/layerpedia.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.94/leap_model_parser/utils/tlinspection/leapinspection.py` & `leap_model_parser-0.1.95/leap_model_parser/utils/tlinspection/leapinspection.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/generatenodedata.py` & `leap_model_parser-0.1.95/leap_model_parser/utils/uicomponents/generatenodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/tensorflowinscpection.py` & `leap_model_parser-0.1.95/leap_model_parser/utils/uicomponents/tensorflowinscpection.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,17 @@
         return _args
 
     def filter_node(self, node):
         return node['name'] in self.ignores['clsignore']
 
     def get_filled_group_values(self, node_type: str, class_pointer: Callable[..., Any]) -> dict:
         if node_type == 'customonnxlayer':
-            var_names = class_pointer.__dict__['call'].__code__.co_varnames
-            arg_names = var_names[1:class_pointer.__dict__['call'].__code__.co_argcount]  # remove self
+            class_code = class_pointer.__dict__['call'].__code__
+            var_names = class_code.co_varnames
+            arg_names = var_names[1:class_code.co_argcount]  # remove self
             if len(arg_names) == 1:
                 return self.group_type[node_type]
             else:
                 config_dict = deepcopy(self.group_type[node_type])
                 inputs_list = config_dict['inputs_data']['inputs']
                 for arg in arg_names[1:]:
                     inputs_list.append(
```

### Comparing `leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/ui_components_config.yaml` & `leap_model_parser-0.1.95/leap_model_parser/utils/uicomponents/ui_components_config.yaml`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.94/pyproject.toml` & `leap_model_parser-0.1.95/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leap-model-parser"
-version = "0.1.94"
+version = "0.1.95"
 description = ""
 authors = ["idan <idan.yogev@tensorleap.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/leap-model-parser"
 homepage = "https://github.com/tensorleap/leap-model-parser"
 include = [
@@ -14,15 +14,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
 tensorflow-macos = {version = "2.11.0", markers = "platform_machine  == 'arm64'"}
 numpy = "^1.22.3"
 onnx = "1.10.1"
-onnx2kerastl = "0.0.86"
+onnx2kerastl = "0.0.87"
 keras-data-format-converter = "0.1.14"
 leap-model-rebuilder = "0.1.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 mypy = "^0.941"
 grappa = "^1.0.1"
```

### Comparing `leap_model_parser-0.1.94/PKG-INFO` & `leap_model_parser-0.1.95/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-model-parser
-Version: 0.1.94
+Version: 0.1.95
 Summary: 
 Home-page: https://github.com/tensorleap/leap-model-parser
 License: MIT
 Author: idan
 Author-email: idan.yogev@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keras-data-format-converter (==0.1.14)
 Requires-Dist: leap-model-rebuilder (==0.1.5)
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: onnx (==1.10.1)
-Requires-Dist: onnx2kerastl (==0.0.86)
+Requires-Dist: onnx2kerastl (==0.0.87)
 Requires-Dist: tensorflow (==2.11.0) ; platform_machine == "x86_64"
 Requires-Dist: tensorflow-macos (==2.11.0) ; platform_machine == "arm64"
 Project-URL: Repository, https://github.com/tensorleap/leap-model-parser
 Description-Content-Type: text/markdown
 
 # Tensorleap model parser
 Used to parse model to the import format
```

