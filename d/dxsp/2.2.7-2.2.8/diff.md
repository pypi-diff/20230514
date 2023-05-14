# Comparing `tmp/dxsp-2.2.7.tar.gz` & `tmp/dxsp-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.2.7.tar", max compression
+gzip compressed data, was "dxsp-2.2.8.tar", max compression
```

## Comparing `dxsp-2.2.7.tar` & `dxsp-2.2.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-13 19:29:51.043585 dxsp-2.2.7/LICENSE
--rw-r--r--   0        0        0     2605 2023-05-13 19:29:51.043585 dxsp-2.2.7/README.md
--rw-r--r--   0        0        0       86 2023-05-13 19:29:51.991632 dxsp-2.2.7/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-13 19:29:51.043585 dxsp-2.2.7/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-13 19:29:51.043585 dxsp-2.2.7/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-13 19:29:51.043585 dxsp-2.2.7/dxsp/config.py
--rw-r--r--   0        0        0     3139 2023-05-13 19:29:51.043585 dxsp-2.2.7/dxsp/default_settings.toml
--rw-r--r--   0        0        0    29552 2023-05-13 19:29:51.043585 dxsp-2.2.7/dxsp/main.py
--rw-r--r--   0        0        0     1811 2023-05-13 19:29:51.991632 dxsp-2.2.7/pyproject.toml
--rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 dxsp-2.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-14 17:38:32.580668 dxsp-2.2.8/LICENSE
+-rw-r--r--   0        0        0     2605 2023-05-14 17:38:32.580668 dxsp-2.2.8/README.md
+-rw-r--r--   0        0        0       86 2023-05-14 17:38:33.232669 dxsp-2.2.8/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-14 17:38:32.580668 dxsp-2.2.8/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-14 17:38:32.580668 dxsp-2.2.8/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-14 17:38:32.580668 dxsp-2.2.8/dxsp/config.py
+-rw-r--r--   0        0        0     3139 2023-05-14 17:38:32.580668 dxsp-2.2.8/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    29552 2023-05-14 17:38:32.580668 dxsp-2.2.8/dxsp/main.py
+-rw-r--r--   0        0        0     1825 2023-05-14 17:38:33.232669 dxsp-2.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 dxsp-2.2.8/PKG-INFO
```

### Comparing `dxsp-2.2.7/LICENSE` & `dxsp-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.7/README.md` & `dxsp-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.7/dxsp/assets/blockchains.py` & `dxsp-2.2.8/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.7/dxsp/default_settings.toml` & `dxsp-2.2.8/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.7/dxsp/main.py` & `dxsp-2.2.8/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.7/pyproject.toml` & `dxsp-2.2.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.2.7"
+version = "2.2.8"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
@@ -15,14 +15,15 @@
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 asyncio = "*"
 dynaconf = "*"
 web3 = ">=6.0.0"
 pycoingecko = "*"
 uniswap-python = "*"
+web3cli = "*"
 
 #web3-ethereum-defi = "*"
 # web3client = ">=1.1.8"
 # # many-abis = ">=0.1.7"
 # apollox-connector-python = "*"
```

### Comparing `dxsp-2.2.7/PKG-INFO` & `dxsp-2.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.2.7
+Version: 2.2.8
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: asyncio
 Requires-Dist: dynaconf
 Requires-Dist: pycoingecko
 Requires-Dist: uniswap-python
 Requires-Dist: web3 (>=6.0.0)
+Requires-Dist: web3cli
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
 
 # DXSP (DeX SwaP)
```

