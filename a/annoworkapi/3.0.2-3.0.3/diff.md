# Comparing `tmp/annoworkapi-3.0.2.tar.gz` & `tmp/annoworkapi-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annoworkapi-3.0.2.tar", max compression
+gzip compressed data, was "annoworkapi-3.0.3.tar", max compression
```

## Comparing `annoworkapi-3.0.2.tar` & `annoworkapi-3.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/LICENSE
--rw-r--r--   0        0        0     2206 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/README.md
--rw-r--r--   0        0        0      240 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/__init__.py
--rw-r--r--   0        0        0      131 2023-05-13 23:36:47.521849 annoworkapi-3.0.2/annoworkapi/__version__.py
--rw-r--r--   0        0        0     5721 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/actual_working_time.py
--rw-r--r--   0        0        0     2580 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/annofab.py
--rw-r--r--   0        0        0    15661 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/api.py
--rw-r--r--   0        0        0     1019 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/enums.py
--rw-r--r--   0        0        0       93 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/exceptions.py
--rw-r--r--   0        0        0    35367 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/generated_api.py
--rw-r--r--   0        0        0      564 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/job.py
--rw-r--r--   0        0        0        0 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/py.typed
--rw-r--r--   0        0        0     3171 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/resource.py
--rw-r--r--   0        0        0     2814 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/schedule.py
--rw-r--r--   0        0        0     1617 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/utils.py
--rw-r--r--   0        0        0    10623 2023-05-13 23:36:35.081710 annoworkapi-3.0.2/annoworkapi/wrapper.py
--rw-r--r--   0        0        0     1920 2023-05-13 23:36:47.521849 annoworkapi-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 annoworkapi-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/LICENSE
+-rw-r--r--   0        0        0     2206 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/README.md
+-rw-r--r--   0        0        0      240 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-14 06:24:41.933018 annoworkapi-3.0.3/annoworkapi/__version__.py
+-rw-r--r--   0        0        0     5721 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/actual_working_time.py
+-rw-r--r--   0        0        0     2556 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/annofab.py
+-rw-r--r--   0        0        0    15661 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/api.py
+-rw-r--r--   0        0        0     1019 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/enums.py
+-rw-r--r--   0        0        0       93 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/exceptions.py
+-rw-r--r--   0        0        0    35367 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/generated_api.py
+-rw-r--r--   0        0        0      564 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/job.py
+-rw-r--r--   0        0        0        0 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/py.typed
+-rw-r--r--   0        0        0     3171 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/resource.py
+-rw-r--r--   0        0        0     2814 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/schedule.py
+-rw-r--r--   0        0        0     1617 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/utils.py
+-rw-r--r--   0        0        0    10623 2023-05-14 06:24:25.480526 annoworkapi-3.0.3/annoworkapi/wrapper.py
+-rw-r--r--   0        0        0     1920 2023-05-14 06:24:41.933018 annoworkapi-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 annoworkapi-3.0.3/PKG-INFO
```

### Comparing `annoworkapi-3.0.2/LICENSE` & `annoworkapi-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.2/README.md` & `annoworkapi-3.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # annowork-api-python-client
-AnnoWork WebAPIのPython用クライントライブラリです。
+Annowork WebAPIのPython用クライントライブラリです。
 
 [![Build Status](https://app.travis-ci.com/kurusugawa-computer/annowork-api-python-client.svg?branch=main)](https://app.travis-ci.com/kurusugawa-computer/annowork-api-python-client)
 [![PyPI version](https://badge.fury.io/py/annoworkapi.svg)](https://badge.fury.io/py/annoworkapi)
 [![Python Versions](https://img.shields.io/pypi/pyversions/annoworkapi.svg)](https://pypi.org/project/annoworkapi/)
 [![Documentation Status](https://readthedocs.org/projects/annowork-api-python-client/badge/?version=latest)](https://annowork-api-python-client.readthedocs.io/ja/latest/?badge=latest)
```

### Comparing `annoworkapi-3.0.2/annoworkapi/actual_working_time.py` & `annoworkapi-3.0.3/annoworkapi/actual_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.2/annoworkapi/annofab.py` & `annoworkapi-3.0.3/annoworkapi/annofab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 外部連携システム"Annofab"に依存した関数やクラスを定義しています。
 """
 from __future__ import annotations
+
 from collections import defaultdict
 from typing import Any, Collection, Optional
 
 from annoworkapi import AnnoworkApi
 
 ANNOFAB_PROJECT_URL_PREFIX = "https://annofab.com/projects/"
 """Annofabのプロジェクトを表すURLのプレフィックス"""
@@ -39,15 +40,15 @@
     Args:
         api: AnnoworkApi Instance
     """
 
     def __init__(self, api: AnnoworkApi):
         self.api = api
 
-    def get_jobs_by_external_linkage_info_url(
+    def get_jobs_by_(
         self, workspace_id: str, annofab_project_ids: Collection[str]
     ) -> dict[str, list[dict[str, Any]]]:
         """
         Annofabのproject_idに紐づくジョブを取得します。
 
         Args:
             workspace_id: ワークスペースID
```

### Comparing `annoworkapi-3.0.2/annoworkapi/api.py` & `annoworkapi-3.0.3/annoworkapi/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,16 +236,16 @@
 
 
 class AnnoworkApi(AbstractAnnoworkApi):
     """
     Web APIに対応したメソッドが存在するクラス。
 
     Args:
-        login_user_id: AnnoWorkにログインするときのユーザID
-        login_password: AnnoWorkにログインするときのパスワード
+        login_user_id: AnnoworkにログインするときのユーザID
+        login_password: Annoworkにログインするときのパスワード
         endpoint_url: WebAPI URLのbase部分
     """
 
     def __init__(self, login_user_id: str, login_password: str, endpoint_url: str = DEFAULT_ENDPOINT_URL):
         if not login_user_id or not login_password:
             raise ValueError("login_user_id or login_password is empty.")
```

### Comparing `annoworkapi-3.0.2/annoworkapi/enums.py` & `annoworkapi-3.0.3/annoworkapi/enums.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.2/annoworkapi/generated_api.py` & `annoworkapi-3.0.3/annoworkapi/generated_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
     def sign_up(self, request_body: Optional[Any] = None, **kwargs) -> Any:
         """サインアップstep1（仮登録）
 
 
 
 
-        アカウントのサインアップの最初のステップとして、アカウントを仮登録します。  AnnoWorkに未登録のメールアドレスであれば、新規アカウントが仮登録状態で作成され、本登録フローのためのメールが送信されます。 このメールには仮パスワードなどが記載されています。  指定したメールアドレスを使うユーザーが仮登録であれば、本登録フローのメールが再送信されます。 指定したメールアドレスを使うユーザーが本登録であれば、不正なリクエストとしてエラーを返します（本登録が仮登録に戻ることはありません）。
+        アカウントのサインアップの最初のステップとして、アカウントを仮登録します。  Annoworkに未登録のメールアドレスであれば、新規アカウントが仮登録状態で作成され、本登録フローのためのメールが送信されます。 このメールには仮パスワードなどが記載されています。  指定したメールアドレスを使うユーザーが仮登録であれば、本登録フローのメールが再送信されます。 指定したメールアドレスを使うユーザーが本登録であれば、不正なリクエストとしてエラーを返します（本登録が仮登録に戻ることはありません）。
 
         Args:
             request_body (Any): Request Body
                 sign_up_request (SignUpRequest):  (required)
 
         Returns:
             InlineResponse200
```

### Comparing `annoworkapi-3.0.2/annoworkapi/job.py` & `annoworkapi-3.0.3/annoworkapi/job.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.2/annoworkapi/resource.py` & `annoworkapi-3.0.3/annoworkapi/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,8 +85,8 @@
 
     # 環境変数から認証情報を取得する
     try:
         return build_from_env(endpoint_url)
     except AnnoworkApiException:
         pass
 
-    raise AnnoworkApiException("`.netrc`ファイルまたは環境変数にAnnoWork認証情報はありませんでした。")
+    raise AnnoworkApiException("`.netrc`ファイルまたは環境変数にAnnowork認証情報はありませんでした。")
```

### Comparing `annoworkapi-3.0.2/annoworkapi/schedule.py` & `annoworkapi-3.0.3/annoworkapi/schedule.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.2/annoworkapi/utils.py` & `annoworkapi-3.0.3/annoworkapi/utils.py`

 * *Files identical despite different names*

### Comparing `annoworkapi-3.0.2/annoworkapi/wrapper.py` & `annoworkapi-3.0.3/annoworkapi/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         return result
 
     return [e for e in actual_daily_list if is_match(e)]
 
 
 class Wrapper:
     """
-    AnnoWorkApiのラッパー.
+    AnnoworkApiのラッパー.
 
     Args:
         api: AnnoworkApi Instance
     """
 
     def __init__(self, api: AnnoworkApi):
         self.api = api
```

### Comparing `annoworkapi-3.0.2/pyproject.toml` & `annoworkapi-3.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "annoworkapi"
-version = "3.0.2"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
-description = "Python Clinet Library of AnnoWork WebAPI"
+version = "3.0.3"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
+description = "Python Clinet Library of Annowork WebAPI"
 authors = ["yuji38kwmt"]
 license = "MIT"
 keywords=["annowork", "api"]
 readme="README.md"
 repository="https://github.com/kurusugawa-computer/annowork-api-python-client"
 classifiers = [
         "Development Status :: 5 - Production/Stable",
```

### Comparing `annoworkapi-3.0.2/PKG-INFO` & `annoworkapi-3.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: annoworkapi
-Version: 3.0.2
-Summary: Python Clinet Library of AnnoWork WebAPI
+Version: 3.0.3
+Summary: Python Clinet Library of Annowork WebAPI
 Home-page: https://github.com/kurusugawa-computer/annowork-api-python-client
 License: MIT
 Keywords: annowork,api
 Author: yuji38kwmt
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Classifier: Topic :: Utilities
 Requires-Dist: backoff
 Requires-Dist: requests
 Project-URL: Repository, https://github.com/kurusugawa-computer/annowork-api-python-client
 Description-Content-Type: text/markdown
 
 # annowork-api-python-client
-AnnoWork WebAPIのPython用クライントライブラリです。
+Annowork WebAPIのPython用クライントライブラリです。
 
 [![Build Status](https://app.travis-ci.com/kurusugawa-computer/annowork-api-python-client.svg?branch=main)](https://app.travis-ci.com/kurusugawa-computer/annowork-api-python-client)
 [![PyPI version](https://badge.fury.io/py/annoworkapi.svg)](https://badge.fury.io/py/annoworkapi)
 [![Python Versions](https://img.shields.io/pypi/pyversions/annoworkapi.svg)](https://pypi.org/project/annoworkapi/)
 [![Documentation Status](https://readthedocs.org/projects/annowork-api-python-client/badge/?version=latest)](https://annowork-api-python-client.readthedocs.io/ja/latest/?badge=latest)
```

