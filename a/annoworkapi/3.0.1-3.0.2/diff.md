# Comparing `tmp/annoworkapi-3.0.1.tar.gz` & `tmp/annoworkapi-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annoworkapi-3.0.1.tar", max compression
+gzip compressed data, was "annoworkapi-3.0.2.tar", max compression
```

## Comparing `annoworkapi-3.0.1.tar` & `annoworkapi-3.0.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1081 2022-03-15 03:13:23.185790 annoworkapi-3.0.1/LICENSE
--rw-r--r--   0        0        0     2236 2022-05-17 08:04:57.287881 annoworkapi-3.0.1/README.md
--rw-r--r--   0        0        0      240 2022-03-15 03:13:23.185790 annoworkapi-3.0.1/annoworkapi/__init__.py
--rw-r--r--   0        0        0       22 2022-05-21 17:34:39.840384 annoworkapi-3.0.1/annoworkapi/__version__.py
--rw-r--r--   0        0        0     5713 2022-05-17 08:04:57.291879 annoworkapi-3.0.1/annoworkapi/actual_working_time.py
--rw-r--r--   0        0        0     1069 2022-03-15 03:13:23.185790 annoworkapi-3.0.1/annoworkapi/annofab.py
--rw-r--r--   0        0        0    15662 2022-03-15 03:13:23.185790 annoworkapi-3.0.1/annoworkapi/api.py
--rw-r--r--   0        0        0     1019 2022-05-17 08:04:57.291879 annoworkapi-3.0.1/annoworkapi/enums.py
--rw-r--r--   0        0        0       93 2022-03-15 03:13:23.185790 annoworkapi-3.0.1/annoworkapi/exceptions.py
--rw-r--r--   0        0        0    35367 2022-05-17 08:04:57.291879 annoworkapi-3.0.1/annoworkapi/generated_api.py
--rw-r--r--   0        0        0      564 2022-03-15 03:13:23.185790 annoworkapi-3.0.1/annoworkapi/job.py
--rw-r--r--   0        0        0        0 2022-03-15 03:13:23.185790 annoworkapi-3.0.1/annoworkapi/py.typed
--rw-r--r--   0        0        0     3171 2022-03-15 03:13:23.185790 annoworkapi-3.0.1/annoworkapi/resource.py
--rw-r--r--   0        0        0     2814 2022-05-17 08:04:57.291879 annoworkapi-3.0.1/annoworkapi/schedule.py
--rw-r--r--   0        0        0     1617 2022-03-15 03:13:23.185790 annoworkapi-3.0.1/annoworkapi/utils.py
--rw-r--r--   0        0        0    10615 2022-05-21 17:34:39.844384 annoworkapi-3.0.1/annoworkapi/wrapper.py
--rw-r--r--   0        0        0     1542 2022-05-21 17:35:44.952384 annoworkapi-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     3004 2022-05-21 17:37:13.547464 annoworkapi-3.0.1/setup.py
--rw-r--r--   0        0        0     3208 2022-05-21 17:37:13.548212 annoworkapi-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/LICENSE
+-rw-r--r--   0        0        0     2206 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/README.md
+-rw-r--r--   0        0        0      240 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-13 23:36:47.521849 annoworkapi-3.0.2/annoworkapi/__version__.py
+-rw-r--r--   0        0        0     5721 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/actual_working_time.py
+-rw-r--r--   0        0        0     2580 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/annofab.py
+-rw-r--r--   0        0        0    15661 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/api.py
+-rw-r--r--   0        0        0     1019 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/enums.py
+-rw-r--r--   0        0        0       93 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/exceptions.py
+-rw-r--r--   0        0        0    35367 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/generated_api.py
+-rw-r--r--   0        0        0      564 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/job.py
+-rw-r--r--   0        0        0        0 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/py.typed
+-rw-r--r--   0        0        0     3171 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/resource.py
+-rw-r--r--   0        0        0     2814 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/schedule.py
+-rw-r--r--   0        0        0     1617 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/utils.py
+-rw-r--r--   0        0        0    10623 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/wrapper.py
+-rw-r--r--   0        0        0     1920 2023-05-13 23:36:47.521849 annoworkapi-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 annoworkapi-3.0.2/PKG-INFO
```

### Comparing `annoworkapi-3.0.1/LICENSE` & `annoworkapi-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.1/README.md` & `annoworkapi-3.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 ## 応用的な使い方
 
 ### ログの出力
 
 ```python
 import logging
-logging_formatter = '%(levelname)-8s : %(asctime)s : %(filename)s : %(name)s : %(funcName)s : %(message)s'
+logging_formatter = '%(levelname)-8s : %(asctime)s : %(name)s : %(message)s'
 logging.basicConfig(format=logging_formatter)
 logging.getLogger("annoworkapi").setLevel(level=logging.DEBUG)
 ```
 
 
 ```
 In [1]: c = s.api.get_actual_working_times_by_workspacen_member("a9956d30-b201-418a-a03b-b9b8b55b2e3d", "204bf4d9-4569-4b7b-89b9-84f089201247")
```

### Comparing `annoworkapi-3.0.1/annoworkapi/actual_working_time.py` & `annoworkapi-3.0.2/annoworkapi/actual_working_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,16 +110,16 @@
             results_dict[key] += value
 
     results_list: list[dict[str, Any]] = []
     for (date, workspace_member_id, job_id), actual_working_hours in results_dict.items():
         # 実績作業時間が0の情報は不要なので、結果情報に格納しない
         if actual_working_hours > 0:
             results_list.append(
-                dict(
-                    date=str(date),
-                    workspace_member_id=workspace_member_id,
-                    job_id=job_id,
-                    actual_working_hours=actual_working_hours,
-                )
+                {
+                    "date": str(date),
+                    "workspace_member_id": workspace_member_id,
+                    "job_id": job_id,
+                    "actual_working_hours": actual_working_hours,
+                }
             )
 
     return results_list
```

### Comparing `annoworkapi-3.0.1/annoworkapi/api.py` & `annoworkapi-3.0.2/annoworkapi/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,14 @@
     Args:
         login_user_id: AnnoWorkにログインするときのユーザID
         login_password: AnnoWorkにログインするときのパスワード
         endpoint_url: WebAPI URLのbase部分
     """
 
     def __init__(self, login_user_id: str, login_password: str, endpoint_url: str = DEFAULT_ENDPOINT_URL):
-
         if not login_user_id or not login_password:
             raise ValueError("login_user_id or login_password is empty.")
 
         self.login_user_id = login_user_id
         self.login_password = login_password
         self.base_url = f"{endpoint_url}/api/v1"
         self.session = requests.Session()
```

### Comparing `annoworkapi-3.0.1/annoworkapi/enums.py` & `annoworkapi-3.0.2/annoworkapi/enums.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.1/annoworkapi/generated_api.py` & `annoworkapi-3.0.2/annoworkapi/generated_api.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.1/annoworkapi/job.py` & `annoworkapi-3.0.2/annoworkapi/job.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.1/annoworkapi/resource.py` & `annoworkapi-3.0.2/annoworkapi/resource.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.1/annoworkapi/schedule.py` & `annoworkapi-3.0.2/annoworkapi/schedule.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.1/annoworkapi/utils.py` & `annoworkapi-3.0.2/annoworkapi/utils.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.1/annoworkapi/wrapper.py` & `annoworkapi-3.0.2/annoworkapi/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,16 +235,16 @@
 
             if term_start is not None and not date >= term_start:
                 continue
             if term_end is not None and not date <= term_end:
                 continue
 
             result_list.append(
-                dict(
-                    date=date,
-                    workspace_member_id=tmp_workspace_member_id,
-                    job_id=tmp_job_id,
-                    assigned_working_hours=assigned_working_hours,
-                )
+                {
+                    "date": date,
+                    "workspace_member_id": tmp_workspace_member_id,
+                    "job_id": tmp_job_id,
+                    "assigned_working_hours": assigned_working_hours,
+                }
             )
 
         return result_list
```

### Comparing `annoworkapi-3.0.1/PKG-INFO` & `annoworkapi-3.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: annoworkapi
-Version: 3.0.1
+Version: 3.0.2
 Summary: Python Clinet Library of AnnoWork WebAPI
 Home-page: https://github.com/kurusugawa-computer/annowork-api-python-client
 License: MIT
 Keywords: annowork,api
 Author: yuji38kwmt
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: backoff
 Requires-Dist: requests
 Project-URL: Repository, https://github.com/kurusugawa-computer/annowork-api-python-client
 Description-Content-Type: text/markdown
 
 # annowork-api-python-client
@@ -73,15 +71,15 @@
 
 ## 応用的な使い方
 
 ### ログの出力
 
 ```python
 import logging
-logging_formatter = '%(levelname)-8s : %(asctime)s : %(filename)s : %(name)s : %(funcName)s : %(message)s'
+logging_formatter = '%(levelname)-8s : %(asctime)s : %(name)s : %(message)s'
 logging.basicConfig(format=logging_formatter)
 logging.getLogger("annoworkapi").setLevel(level=logging.DEBUG)
 ```
 
 
 ```
 In [1]: c = s.api.get_actual_working_times_by_workspacen_member("a9956d30-b201-418a-a03b-b9b8b55b2e3d", "204bf4d9-4569-4b7b-89b9-84f089201247")
```

