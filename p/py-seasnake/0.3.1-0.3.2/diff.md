# Comparing `tmp/py_seasnake-0.3.1.tar.gz` & `tmp/py_seasnake-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_seasnake-0.3.1.tar", max compression
+gzip compressed data, was "py_seasnake-0.3.2.tar", max compression
```

## Comparing `py_seasnake-0.3.1.tar` & `py_seasnake-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1070 2023-05-03 04:25:11.883497 py_seasnake-0.3.1/LICENSE
--rw-r--r--   0        0        0      745 2023-05-03 04:25:11.883497 py_seasnake-0.3.1/README.md
--rw-r--r--   0        0        0     1311 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      129 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/__init__.py
--rw-r--r--   0        0        0     4062 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/auth.py
--rw-r--r--   0        0        0     9230 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/base.py
--rw-r--r--   0        0        0     1445 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/io.py
--rw-r--r--   0        0        0     2775 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/projects.py
--rw-r--r--   0        0        0      386 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/__init__.py
--rw-r--r--   0        0        0     3114 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/base.py
--rw-r--r--   0        0        0     2853 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/benthic_lit.py
--rw-r--r--   0        0        0     2979 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/benthic_photo_quadrat.py
--rw-r--r--   0        0        0     2854 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/benthic_pit.py
--rw-r--r--   0        0        0     3741 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/bleaching.py
--rw-r--r--   0        0        0     2654 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/fish_belt.py
--rw-r--r--   0        0        0     2957 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/habitat_complexity.py
--rw-r--r--   0        0        0     2356 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/summaries/sample_event.py
--rw-r--r--   0        0        0      606 2023-05-03 04:25:11.887497 py_seasnake-0.3.1/seasnake/timer.py
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 py_seasnake-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/LICENSE
+-rw-r--r--   0        0        0      745 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/README.md
+-rw-r--r--   0        0        0     1332 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/__init__.py
+-rw-r--r--   0        0        0     4394 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/auth.py
+-rw-r--r--   0        0        0     9230 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/base.py
+-rw-r--r--   0        0        0     1445 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/io.py
+-rw-r--r--   0        0        0     2775 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/projects.py
+-rw-r--r--   0        0        0      386 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/summaries/__init__.py
+-rw-r--r--   0        0        0     3114 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/summaries/base.py
+-rw-r--r--   0        0        0     2853 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/summaries/benthic_lit.py
+-rw-r--r--   0        0        0     2979 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/summaries/benthic_photo_quadrat.py
+-rw-r--r--   0        0        0     2854 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/summaries/benthic_pit.py
+-rw-r--r--   0        0        0     3741 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/summaries/bleaching.py
+-rw-r--r--   0        0        0     2654 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/summaries/fish_belt.py
+-rw-r--r--   0        0        0     2957 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/summaries/habitat_complexity.py
+-rw-r--r--   0        0        0     2356 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/summaries/sample_event.py
+-rw-r--r--   0        0        0      606 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/timer.py
+-rw-r--r--   0        0        0     1850 1970-01-01 00:00:00.000000 py_seasnake-0.3.2/PKG-INFO
```

### Comparing `py_seasnake-0.3.1/LICENSE` & `py_seasnake-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/README.md` & `py_seasnake-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/pyproject.toml` & `py_seasnake-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "py-seasnake"
 packages = [
     { include = "seasnake" },
 ]
-version = "0.3.1"
+version = "0.3.2"
 description = "A Python wrapper for accessing and managing MERMAID (Marine Ecological Research Management Aid) data with ease."
 authors = ["Dustin Sampson <gridcell@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gridcell.github.io/py-seasnake/"
 repository = "https://github.com/gridcell/py-seasnake"
 documentation = "https://gridcell.github.io/py-seasnake/"
@@ -16,14 +16,15 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 PyJWT = "^2.6.0"
 mkdocs-material = "^9.1.6"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 requests = "^2.28.2"
 geopandas = "^0.12.2"
+keyring = "^23.13.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 black = "^23.3.0"
 isort = "^5.12.0"
 ruff = "^0.0.261"
 mypy = "^1.2.0"
```

### Comparing `py_seasnake-0.3.1/seasnake/auth.py` & `py_seasnake-0.3.2/seasnake/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import keyring
 import time
 import webbrowser
 from typing import Optional
 
 import jwt
 import requests
 
@@ -17,24 +18,22 @@
     """
     A class for handling authentication and access token management for the Mermaid API.
 
     The MermaidAuth class is responsible for managing the process of obtaining and storing
     access tokens for use with the Mermaid API. It checks if the stored token is expired,
     and if so, initiates an authentication process to obtain a new token.
 
-    Attributes:
-        auth_file (str): The name of the file where the access token is stored.
-
     Example usage:
 
         mermaid_auth = MermaidAuth()
         token = mermaid_auth.get_token()
     """
 
-    auth_file = ".auth"
+    AUTH_CODE_URL = f"https://{AUTH0_DOMAIN}/oauth/device/code"
+    AUTH_TOKEN_URL = f"https://{AUTH0_DOMAIN}/oauth/token"
 
     def _token_expired(self, token: Optional[str]) -> bool:
         if not token:
             return True
 
         try:
             payload = jwt.decode(token, options={"verify_signature": False})
@@ -44,43 +43,50 @@
                 if expiration_date > datetime.datetime.utcnow():
                     return False
             return True
         except jwt.DecodeError:
             return True
 
     def _write_token(self, token: str):
-        with open(self.auth_file, "w") as f:
-            f.write(token)
+        try:
+            keyring.set_password("system", "seasnake", token)
+        except Exception:
+            pass
 
     def _load_token(self) -> Optional[str]:
         try:
-            with open(self.auth_file, "r") as f:
-                return f.read()
+            token = keyring.get_password("system", "seasnake")
+            return token
         except Exception:
             return None
 
-    def get_token(self, store: bool=False) -> Optional[str]:
+    def clear_token(self):
+        """
+        Delete stored Mermaid API access token.
         """
+        keyring.delete_password("system", "seasnake")
 
+    def get_token(self, store: bool=False) -> Optional[str]:
+        """
+        Get an access token for the Mermaid API.
         Args:
-            store (bool, optional): Store token to disk. Defaults to False.
+            store (bool, optional): Store token to keyring service ([more info](https://github.com/jaraco/keyring)). Defaults to False.
 
         Returns:
             Optional[str]: Access token
         """
         client_id = CLIENT_ID
-        domain = AUTH0_DOMAIN
         audience = AUDIENCE
 
         token = self._load_token()
         if self._token_expired(token) is False:
             return token
 
         response = requests.post(
-            f"https://{domain}/oauth/device/code",
+            self.AUTH_CODE_URL,
             data={"client_id": client_id, "audience": audience},
         )
 
         json_response = response.json()
         user_code = json_response["user_code"]
         verification_uri = json_response["verification_uri"]
         webbrowser.open(f"{verification_uri}?user_code={user_code}")
@@ -91,28 +97,30 @@
 
         while True:
             # Wait for a short time before polling again
             time.sleep(3)
 
             # Make a request to the token endpoint using the device code
             response = requests.post(
-                f"https://{domain}/oauth/token",
+                self.AUTH_TOKEN_URL,
                 data={
                     "grant_type": "urn:ietf:params:oauth:grant-type:device_code",
                     "client_id": client_id,
                     "device_code": json_response["device_code"],
                 },
             )
 
             # If the request is successful, extract the access token and break out of the loop
             if response.status_code == 200:
                 json_response = response.json()
                 access_token = json_response["access_token"]
                 if store:
                     self._write_token(access_token)
+                else:
+                    self.clear_token()
                 return access_token
 
             # If the timeout is reached, exit the loop and inform the user
             elapsed_time = time.time() - start_time
             if elapsed_time > timeout:
                 print("Timeout reached. Please try again.")
                 break
```

### Comparing `py_seasnake-0.3.1/seasnake/base.py` & `py_seasnake-0.3.2/seasnake/base.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/seasnake/io.py` & `py_seasnake-0.3.2/seasnake/io.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/seasnake/projects.py` & `py_seasnake-0.3.2/seasnake/projects.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/seasnake/summaries/base.py` & `py_seasnake-0.3.2/seasnake/summaries/base.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/seasnake/summaries/benthic_lit.py` & `py_seasnake-0.3.2/seasnake/summaries/benthic_lit.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/seasnake/summaries/benthic_photo_quadrat.py` & `py_seasnake-0.3.2/seasnake/summaries/benthic_photo_quadrat.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/seasnake/summaries/benthic_pit.py` & `py_seasnake-0.3.2/seasnake/summaries/benthic_pit.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/seasnake/summaries/bleaching.py` & `py_seasnake-0.3.2/seasnake/summaries/bleaching.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/seasnake/summaries/fish_belt.py` & `py_seasnake-0.3.2/seasnake/summaries/fish_belt.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/seasnake/summaries/habitat_complexity.py` & `py_seasnake-0.3.2/seasnake/summaries/habitat_complexity.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/seasnake/summaries/sample_event.py` & `py_seasnake-0.3.2/seasnake/summaries/sample_event.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/seasnake/timer.py` & `py_seasnake-0.3.2/seasnake/timer.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.1/PKG-INFO` & `py_seasnake-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-seasnake
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python wrapper for accessing and managing MERMAID (Marine Ecological Research Management Aid) data with ease.
 Home-page: https://gridcell.github.io/py-seasnake/
 License: MIT
 Keywords: MERMAID,coral,fish,API
 Author: Dustin Sampson
 Author-email: gridcell@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: geopandas (>=0.12.2,<0.13.0)
+Requires-Dist: keyring (>=23.13.1,<24.0.0)
 Requires-Dist: mkdocs-material (>=9.1.6,<10.0.0)
 Requires-Dist: mkdocstrings[python] (>=0.21.2,<0.22.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Documentation, https://gridcell.github.io/py-seasnake/
 Project-URL: Repository, https://github.com/gridcell/py-seasnake
 Description-Content-Type: text/markdown
```

