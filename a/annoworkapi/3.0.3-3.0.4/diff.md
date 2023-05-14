# Comparing `tmp/annoworkapi-3.0.3.tar.gz` & `tmp/annoworkapi-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annoworkapi-3.0.3.tar", max compression
+gzip compressed data, was "annoworkapi-3.0.4.tar", max compression
```

## Comparing `annoworkapi-3.0.3.tar` & `annoworkapi-3.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/LICENSE
--rw-r--r--   0        0        0     2206 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/README.md
--rw-r--r--   0        0        0      240 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/__init__.py
--rw-r--r--   0        0        0      131 2023-05-14 06:24:41.933018 annoworkapi-3.0.3/annoworkapi/__version__.py
--rw-r--r--   0        0        0     5721 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/actual_working_time.py
--rw-r--r--   0        0        0     2556 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/annofab.py
--rw-r--r--   0        0        0    15661 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/api.py
--rw-r--r--   0        0        0     1019 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/enums.py
--rw-r--r--   0        0        0       93 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/exceptions.py
--rw-r--r--   0        0        0    35367 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/generated_api.py
--rw-r--r--   0        0        0      564 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/job.py
--rw-r--r--   0        0        0        0 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/py.typed
--rw-r--r--   0        0        0     3171 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/resource.py
--rw-r--r--   0        0        0     2814 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/schedule.py
--rw-r--r--   0        0        0     1617 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/utils.py
--rw-r--r--   0        0        0    10623 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/wrapper.py
--rw-r--r--   0        0        0     1920 2023-05-14 06:24:41.933018 annoworkapi-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 annoworkapi-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/LICENSE
+-rw-r--r--   0        0        0     2206 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/README.md
+-rw-r--r--   0        0        0      240 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/annoworkapi/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-14 06:47:08.416633 annoworkapi-3.0.4/annoworkapi/__version__.py
+-rw-r--r--   0        0        0     5721 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/annoworkapi/actual_working_time.py
+-rw-r--r--   0        0        0     2574 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/annoworkapi/annofab.py
+-rw-r--r--   0        0        0    15661 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/annoworkapi/api.py
+-rw-r--r--   0        0        0     1019 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/annoworkapi/enums.py
+-rw-r--r--   0        0        0       93 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/annoworkapi/exceptions.py
+-rw-r--r--   0        0        0    35367 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/annoworkapi/generated_api.py
+-rw-r--r--   0        0        0      564 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/annoworkapi/job.py
+-rw-r--r--   0        0        0        0 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/annoworkapi/py.typed
+-rw-r--r--   0        0        0     3171 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/annoworkapi/resource.py
+-rw-r--r--   0        0        0     2814 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/annoworkapi/schedule.py
+-rw-r--r--   0        0        0     1617 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/annoworkapi/utils.py
+-rw-r--r--   0        0        0    10623 2023-05-14 06:46:50.080556 annoworkapi-3.0.4/annoworkapi/wrapper.py
+-rw-r--r--   0        0        0     1920 2023-05-14 06:47:08.412633 annoworkapi-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 annoworkapi-3.0.4/PKG-INFO
```

### Comparing `annoworkapi-3.0.3/LICENSE` & `annoworkapi-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.3/README.md` & `annoworkapi-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.3/annoworkapi/actual_working_time.py` & `annoworkapi-3.0.4/annoworkapi/actual_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.3/annoworkapi/annofab.py` & `annoworkapi-3.0.4/annoworkapi/annofab.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     Args:
         api: AnnoworkApi Instance
     """
 
     def __init__(self, api: AnnoworkApi):
         self.api = api
 
-    def get_jobs_by_(
+    def get_jobs_by_annofab_project_id(
         self, workspace_id: str, annofab_project_ids: Collection[str]
     ) -> dict[str, list[dict[str, Any]]]:
         """
         Annofabのproject_idに紐づくジョブを取得します。
 
         Args:
             workspace_id: ワークスペースID
```

### Comparing `annoworkapi-3.0.3/annoworkapi/api.py` & `annoworkapi-3.0.4/annoworkapi/api.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.3/annoworkapi/enums.py` & `annoworkapi-3.0.4/annoworkapi/enums.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.3/annoworkapi/generated_api.py` & `annoworkapi-3.0.4/annoworkapi/generated_api.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.3/annoworkapi/job.py` & `annoworkapi-3.0.4/annoworkapi/job.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.3/annoworkapi/resource.py` & `annoworkapi-3.0.4/annoworkapi/resource.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.3/annoworkapi/schedule.py` & `annoworkapi-3.0.4/annoworkapi/schedule.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.3/annoworkapi/utils.py` & `annoworkapi-3.0.4/annoworkapi/utils.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.3/annoworkapi/wrapper.py` & `annoworkapi-3.0.4/annoworkapi/wrapper.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.3/pyproject.toml` & `annoworkapi-3.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "annoworkapi"
-version = "3.0.3"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
+version = "3.0.4"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
 description = "Python Clinet Library of Annowork WebAPI"
 authors = ["yuji38kwmt"]
 license = "MIT"
 keywords=["annowork", "api"]
 readme="README.md"
 repository="https://github.com/kurusugawa-computer/annowork-api-python-client"
 classifiers = [
```

### Comparing `annoworkapi-3.0.3/PKG-INFO` & `annoworkapi-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annoworkapi
-Version: 3.0.3
+Version: 3.0.4
 Summary: Python Clinet Library of Annowork WebAPI
 Home-page: https://github.com/kurusugawa-computer/annowork-api-python-client
 License: MIT
 Keywords: annowork,api
 Author: yuji38kwmt
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

