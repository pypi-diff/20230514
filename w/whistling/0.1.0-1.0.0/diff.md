# Comparing `tmp/whistling-0.1.0.tar.gz` & `tmp/whistling-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whistling-0.1.0.tar", last modified: Wed Dec 23 00:09:55 2020, max compression
+gzip compressed data, was "whistling-1.0.0.tar", max compression
```

## Comparing `whistling-0.1.0.tar` & `whistling-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1070 2020-12-22 12:12:24.862446 whistling-0.1.0/LICENSE
--rw-r--r--   0        0        0      179 2020-12-22 12:36:41.832740 whistling-0.1.0/README.md
--rw-r--r--   0        0        0      623 2020-12-22 13:03:41.789861 whistling-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      265 2020-12-22 12:41:58.236377 whistling-0.1.0/whistling/__init__.py
--rw-r--r--   0        0        0      364 2020-12-22 12:46:45.817964 whistling-0.1.0/whistling/abstract_reporter.py
--rw-r--r--   0        0        0     1786 2020-12-22 12:46:45.900630 whistling-0.1.0/whistling/ecx.py
--rw-r--r--   0        0        0     1457 2020-12-22 12:46:45.224529 whistling-0.1.0/whistling/gsb.py
--rw-r--r--   0        0        0      650 2020-12-22 12:46:45.855681 whistling-0.1.0/whistling/netcraft.py
--rw-r--r--   0        0        0     1637 2020-12-22 12:46:45.887909 whistling-0.1.0/whistling/urlscan.py
--rw-r--r--   0        0        0      856 2020-12-23 00:09:55.330145 whistling-0.1.0/setup.py
--rw-r--r--   0        0        0      765 2020-12-23 00:09:55.330392 whistling-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-14 06:51:02.670728 whistling-1.0.0/LICENSE
+-rw-r--r--   0        0        0      179 2023-05-14 06:51:02.670728 whistling-1.0.0/README.md
+-rw-r--r--   0        0        0      681 2023-05-14 06:51:20.010496 whistling-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-05-14 06:51:02.670728 whistling-1.0.0/whistling/__init__.py
+-rw-r--r--   0        0        0      328 2023-05-14 06:51:02.670728 whistling-1.0.0/whistling/abstract_reporter.py
+-rw-r--r--   0        0        0     1767 2023-05-14 06:51:02.670728 whistling-1.0.0/whistling/ecx.py
+-rw-r--r--   0        0        0     1434 2023-05-14 06:51:02.670728 whistling-1.0.0/whistling/gsb.py
+-rw-r--r--   0        0        0      682 2023-05-14 06:51:02.670728 whistling-1.0.0/whistling/netcraft.py
+-rw-r--r--   0        0        0     1618 2023-05-14 06:51:02.670728 whistling-1.0.0/whistling/urlscan.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 whistling-1.0.0/PKG-INFO
```

### Comparing `whistling-0.1.0/LICENSE` & `whistling-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whistling-0.1.0/whistling/ecx.py` & `whistling-1.0.0/whistling/ecx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 """
 Reporter class for APWG's eCX
 """
 from datetime import datetime
-from typing import Optional
 
 import httpx
 
 from whistling.abstract_reporter import AbstractReporter
 
 
 def current_time() -> int:
     now = datetime.now()
     return int(datetime.timestamp(now))
 
 
 def build_payload(
     url: str,
-    brand: Optional[str] = None,
-    confidence_level: Optional[int] = None,
-    date_discovered: Optional[int] = None,
+    brand: str | None = None,
+    confidence_level: int | None = None,
+    date_discovered: int | None = None,
 ):
     return {
         "brand": brand or "",
         "url": url,
         "confidence_level": confidence_level or 100,
         "date_discovered": date_discovered or current_time(),
     }
 
 
 class ECX(AbstractReporter):
     def __init__(
-        self, token: str, base_url: str = "https://api.ecrimex.net/phish",
+        self,
+        token: str,
+        *,
+        base_url: str = "https://api.ecrimex.net/phish",
     ):
         self.base_url = base_url
         self.token = token
 
+        assert self.token is not None
+
     def report(self, url: str, **kwargs) -> httpx.Response:
         """Report the URL to eCX
 
         Args:
             url (str): The URL to report
 
         Keyword Args:
             brand (str):
             date_discovered (int): 10 digit epoch timestamp
             confidence_level (int): 50, 90, or 100
 
         Returns:
             httpx.Response: A response from eCX
         """
-        assert self.token is not None
-
-        brand: Optional[str] = kwargs.get("brand", None)
-        date_discovered: Optional[int] = kwargs.get("date_discovered", None)
-        confidence_level: Optional[int] = kwargs.get("confidence_level", None)
+        brand: str | None = kwargs.get("brand", None)
+        date_discovered: int | None = kwargs.get("date_discovered", None)
+        confidence_level: int | None = kwargs.get("confidence_level", None)
 
         payload = build_payload(
             url=url,
             brand=brand,
             confidence_level=confidence_level,
             date_discovered=date_discovered,
         )
```

### Comparing `whistling-0.1.0/whistling/gsb.py` & `whistling-1.0.0/whistling/gsb.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
 Reporter class for Google Safe Browsing
 """
-from typing import List, Optional
 
 import httpx
 
 from whistling.abstract_reporter import AbstractReporter
 
 
 def build_payload(
     url: str,
-    screenshot: Optional[str] = None,
-    dom: Optional[str] = None,
-    flags: Optional[List[str]] = None,
+    screenshot: str | None = None,
+    dom: str | None = None,
+    flags: list[str] | None = None,
 ) -> list:
     return [url, None, screenshot, dom, None, flags]
 
 
 class GSB(AbstractReporter):
     def __init__(
         self,
+        token: str | None = None,
+        *,
         base_url: str = "https://safebrowsing.google.com/safebrowsing/clientreport/crx-report",
-        _=None,
     ):
         self.base_url = base_url
 
     def report(self, url: str, **kwargs) -> httpx.Response:
         """Report the URL to Google Safe Browsing
 
         Args:
@@ -35,16 +35,16 @@
             screenshot (str): screenshot of the malicious site as a base64 encoded PNG
             dom (str): DOM of the malicious site
             flags (List[str]): a set of flags for why the site was flagged as suspicious
 
         Returns:
             httpx.Response: A response from Google Safe Browsing
         """
-        screenshot: Optional[str] = kwargs.get("screenshot", None)
-        dom: Optional[str] = kwargs.get("dom", None)
-        flags: Optional[List[str]] = kwargs.get("flags", None)
+        screenshot: str | None = kwargs.get("screenshot", None)
+        dom: str | None = kwargs.get("dom", None)
+        flags: list[str] | None = kwargs.get("flags", None)
 
         payload = build_payload(url, screenshot=screenshot, dom=dom, flags=flags)
 
         res = httpx.post(self.base_url, json=payload)
         res.raise_for_status()
         return res
```

### Comparing `whistling-0.1.0/whistling/netcraft.py` & `whistling-1.0.0/whistling/netcraft.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,20 +8,23 @@
 
 def build_payload(url: str, email: str):
     return {"urls": [url], "email": email}
 
 
 class Netcraft(AbstractReporter):
     def __init__(
-        self, token, base_url: str = "https://report.netcraft.com/api/v2/report/urls",
+        self,
+        token: str,
+        *,
+        base_url: str = "https://report.netcraft.com/api/v2/report/urls",
     ):
         self.base_url = base_url
         self.token = token
 
-    def report(self, url: str, **_) -> httpx.Response:
         assert self.token is not None
 
+    def report(self, url: str, **_) -> httpx.Response:
         payload = build_payload(url, self.token)
 
         res = httpx.post(self.base_url, json=payload)
         res.raise_for_status()
         return res
```

### Comparing `whistling-0.1.0/whistling/urlscan.py` & `whistling-1.0.0/whistling/urlscan.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 """
 Reporter class for urlscan.io
 """
-from typing import Optional
 
 import httpx
 
 from whistling.abstract_reporter import AbstractReporter
 
 
 def build_payload(
     url: str,
-    customagent: Optional[str] = None,
-    referer: Optional[str] = None,
-    visibility: Optional[str] = None,
+    customagent: str | None = None,
+    referer: str | None = None,
+    visibility: str | None = None,
 ) -> dict:
     d = {
         "url": url,
         "customagent": customagent,
         "referer": referer,
         "visibility": visibility,
     }
     return {k: v for k, v in d.items() if v is not None}
 
 
 class URLScan(AbstractReporter):
     def __init__(
-        self, token: str, base_url: str = "https://urlscan.io/api/v1/scan/",
+        self,
+        token: str,
+        *,
+        base_url: str = "https://urlscan.io/api/v1/scan/",
     ):
         self.base_url = base_url
         self.token = token
 
+        assert self.token is not None
+
     def report(self, url: str, **kwargs) -> httpx.Response:
         """[summary]
 
         Args:
             url (str): The URL to report
 
         Keyword Args:
             customagent (str): Override User-Agent for this scan
             referer (str): Override HTTP referer for this scan
             visibility (str): One of public, unlisted, private
 
         Returns:
             httpx.Response: [description]
         """
-        assert self.token is not None
-
-        customagent: Optional[str] = kwargs.get("customagent", None)
-        referer: Optional[str] = kwargs.get("referer", None)
-        visibility: Optional[str] = kwargs.get("visibility", None)
+        customagent: str | None = kwargs.get("customagent", None)
+        referer: str | None = kwargs.get("referer", None)
+        visibility: str | None = kwargs.get("visibility", None)
 
         payload = build_payload(
             url=url, customagent=customagent, referer=referer, visibility=visibility
         )
         headers = {"API-Key": self.token}
 
         res = httpx.post(self.base_url, json=payload, headers=headers)
```

### Comparing `whistling-0.1.0/PKG-INFO` & `whistling-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: whistling
-Version: 0.1.0
+Version: 1.0.0
 Summary: A collection of functions to report a malicious URL
 License: MIT
 Author: Manabu Niseki
 Author-email: manabu.niseki@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: contextvars (>=2.4,<3.0)
-Requires-Dist: httpx (>=0.16.1,<0.17.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.24,<1.0)
 Description-Content-Type: text/markdown
 
 # whistling
 
 Whistling is a Python package to report malicious / suspicious URL.
 
 The following services are supported.
```

