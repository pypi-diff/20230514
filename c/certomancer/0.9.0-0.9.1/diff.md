# Comparing `tmp/certomancer-0.9.0.tar.gz` & `tmp/certomancer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certomancer-0.9.0.tar", last modified: Sat Aug 20 09:28:27 2022, max compression
+gzip compressed data, was "certomancer-0.9.1.tar", last modified: Thu Oct 27 20:10:38 2022, max compression
```

## Comparing `certomancer-0.9.0.tar` & `certomancer-0.9.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-08-20 09:28:27.287592 certomancer-0.9.0/
--rw-r--r--   0 matthias   (501) staff       (20)     1081 2022-05-23 18:41:14.000000 certomancer-0.9.0/LICENSE
--rw-r--r--   0 matthias   (501) staff       (20)     5796 2022-08-20 09:28:27.287466 certomancer-0.9.0/PKG-INFO
--rw-r--r--   0 matthias   (501) staff       (20)     4938 2022-08-20 09:27:17.000000 certomancer-0.9.0/README.md
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-08-20 09:28:27.283557 certomancer-0.9.0/certomancer/
--rw-r--r--   0 matthias   (501) staff       (20)      557 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)      162 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/__main__.py
--rw-r--r--   0 matthias   (501) staff       (20)     1893 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/_asn1_types.py
--rw-r--r--   0 matthias   (501) staff       (20)    16046 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/cli.py
--rw-r--r--   0 matthias   (501) staff       (20)     9503 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/config_utils.py
--rw-r--r--   0 matthias   (501) staff       (20)    14182 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/crypto_utils.py
--rw-r--r--   0 matthias   (501) staff       (20)    21313 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/default_plugins.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-08-20 09:28:27.284690 certomancer-0.9.0/certomancer/integrations/
--rw-r--r--   0 matthias   (501) staff       (20)        0 2022-05-23 18:41:14.000000 certomancer-0.9.0/certomancer/integrations/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     9871 2022-08-20 09:27:19.000000 certomancer-0.9.0/certomancer/integrations/alchemist.py
--rw-r--r--   0 matthias   (501) staff       (20)    20397 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/integrations/animator.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-08-20 09:28:27.285020 certomancer-0.9.0/certomancer/integrations/animator_templates/
--rw-r--r--   0 matthias   (501) staff       (20)     7061 2022-05-23 18:41:14.000000 certomancer-0.9.0/certomancer/integrations/animator_templates/arch_summary.html
--rw-r--r--   0 matthias   (501) staff       (20)      593 2022-05-23 18:41:14.000000 certomancer-0.9.0/certomancer/integrations/animator_templates/index.html
--rw-r--r--   0 matthias   (501) staff       (20)     3300 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/integrations/illusionist.py
--rw-r--r--   0 matthias   (501) staff       (20)        0 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/py.typed
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-08-20 09:28:27.286139 certomancer-0.9.0/certomancer/registry/
--rw-r--r--   0 matthias   (501) staff       (20)     1211 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     1142 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/common.py
--rw-r--r--   0 matthias   (501) staff       (20)     4256 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/config.py
--rw-r--r--   0 matthias   (501) staff       (20)     1852 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/entities.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-08-20 09:28:27.286609 certomancer-0.9.0/certomancer/registry/issued/
--rw-r--r--   0 matthias   (501) staff       (20)        0 2022-05-23 18:41:14.000000 certomancer-0.9.0/certomancer/registry/issued/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     7496 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/issued/attr_cert.py
--rw-r--r--   0 matthias   (501) staff       (20)     3065 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/issued/cert.py
--rw-r--r--   0 matthias   (501) staff       (20)    11046 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/issued/general.py
--rw-r--r--   0 matthias   (501) staff       (20)     6866 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/keys.py
--rw-r--r--   0 matthias   (501) staff       (20)    49855 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/pki_arch.py
--rw-r--r--   0 matthias   (501) staff       (20)    21729 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/plugin_api.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-08-20 09:28:27.287306 certomancer-0.9.0/certomancer/registry/svc_config/
--rw-r--r--   0 matthias   (501) staff       (20)        0 2022-05-23 18:41:14.000000 certomancer-0.9.0/certomancer/registry/svc_config/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     1450 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/svc_config/api.py
--rw-r--r--   0 matthias   (501) staff       (20)     3382 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/svc_config/cert_repo.py
--rw-r--r--   0 matthias   (501) staff       (20)     4903 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/svc_config/crl.py
--rw-r--r--   0 matthias   (501) staff       (20)     3837 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/svc_config/ocsp.py
--rw-r--r--   0 matthias   (501) staff       (20)     1133 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/registry/svc_config/tsa.py
--rw-r--r--   0 matthias   (501) staff       (20)    15800 2022-08-19 23:44:07.000000 certomancer-0.9.0/certomancer/services.py
--rw-r--r--   0 matthias   (501) staff       (20)       51 2022-08-20 09:27:22.000000 certomancer-0.9.0/certomancer/version.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-08-20 09:28:27.284155 certomancer-0.9.0/certomancer.egg-info/
--rw-r--r--   0 matthias   (501) staff       (20)     5796 2022-08-20 09:28:27.000000 certomancer-0.9.0/certomancer.egg-info/PKG-INFO
--rw-r--r--   0 matthias   (501) staff       (20)     1383 2022-08-20 09:28:27.000000 certomancer-0.9.0/certomancer.egg-info/SOURCES.txt
--rw-r--r--   0 matthias   (501) staff       (20)        1 2022-08-20 09:28:27.000000 certomancer-0.9.0/certomancer.egg-info/dependency_links.txt
--rw-r--r--   0 matthias   (501) staff       (20)       60 2022-08-20 09:28:27.000000 certomancer-0.9.0/certomancer.egg-info/entry_points.txt
--rw-r--r--   0 matthias   (501) staff       (20)      240 2022-08-20 09:28:27.000000 certomancer-0.9.0/certomancer.egg-info/requires.txt
--rw-r--r--   0 matthias   (501) staff       (20)       12 2022-08-20 09:28:27.000000 certomancer-0.9.0/certomancer.egg-info/top_level.txt
--rw-r--r--   0 matthias   (501) staff       (20)       38 2022-08-20 09:28:27.287633 certomancer-0.9.0/setup.cfg
--rw-r--r--   0 matthias   (501) staff       (20)     2575 2022-08-19 23:44:07.000000 certomancer-0.9.0/setup.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-10-27 20:10:38.191331 certomancer-0.9.1/
+-rw-r--r--   0 matthias   (501) staff       (20)     1081 2022-05-23 18:41:14.000000 certomancer-0.9.1/LICENSE
+-rw-r--r--   0 matthias   (501) staff       (20)     5847 2022-10-27 20:10:38.191213 certomancer-0.9.1/PKG-INFO
+-rw-r--r--   0 matthias   (501) staff       (20)     4938 2022-08-20 09:35:59.000000 certomancer-0.9.1/README.md
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-10-27 20:10:38.186762 certomancer-0.9.1/certomancer/
+-rw-r--r--   0 matthias   (501) staff       (20)      557 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/__init__.py
+-rw-r--r--   0 matthias   (501) staff       (20)      162 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/__main__.py
+-rw-r--r--   0 matthias   (501) staff       (20)     1893 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/_asn1_types.py
+-rw-r--r--   0 matthias   (501) staff       (20)    16046 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/cli.py
+-rw-r--r--   0 matthias   (501) staff       (20)     9503 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/config_utils.py
+-rw-r--r--   0 matthias   (501) staff       (20)    14182 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/crypto_utils.py
+-rw-r--r--   0 matthias   (501) staff       (20)    21313 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/default_plugins.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-10-27 20:10:38.188149 certomancer-0.9.1/certomancer/integrations/
+-rw-r--r--   0 matthias   (501) staff       (20)        0 2022-05-23 18:41:14.000000 certomancer-0.9.1/certomancer/integrations/__init__.py
+-rw-r--r--   0 matthias   (501) staff       (20)     9871 2022-08-20 09:35:59.000000 certomancer-0.9.1/certomancer/integrations/alchemist.py
+-rw-r--r--   0 matthias   (501) staff       (20)    20397 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/integrations/animator.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-10-27 20:10:38.188465 certomancer-0.9.1/certomancer/integrations/animator_templates/
+-rw-r--r--   0 matthias   (501) staff       (20)     7061 2022-05-23 18:41:14.000000 certomancer-0.9.1/certomancer/integrations/animator_templates/arch_summary.html
+-rw-r--r--   0 matthias   (501) staff       (20)      593 2022-05-23 18:41:14.000000 certomancer-0.9.1/certomancer/integrations/animator_templates/index.html
+-rw-r--r--   0 matthias   (501) staff       (20)     3300 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/integrations/illusionist.py
+-rw-r--r--   0 matthias   (501) staff       (20)        0 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/py.typed
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-10-27 20:10:38.189638 certomancer-0.9.1/certomancer/registry/
+-rw-r--r--   0 matthias   (501) staff       (20)     1211 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/registry/__init__.py
+-rw-r--r--   0 matthias   (501) staff       (20)     1142 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/registry/common.py
+-rw-r--r--   0 matthias   (501) staff       (20)     4256 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/registry/config.py
+-rw-r--r--   0 matthias   (501) staff       (20)     1852 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/registry/entities.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-10-27 20:10:38.190361 certomancer-0.9.1/certomancer/registry/issued/
+-rw-r--r--   0 matthias   (501) staff       (20)        0 2022-05-23 18:41:14.000000 certomancer-0.9.1/certomancer/registry/issued/__init__.py
+-rw-r--r--   0 matthias   (501) staff       (20)     7534 2022-10-27 19:05:50.000000 certomancer-0.9.1/certomancer/registry/issued/attr_cert.py
+-rw-r--r--   0 matthias   (501) staff       (20)     3065 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/registry/issued/cert.py
+-rw-r--r--   0 matthias   (501) staff       (20)    11046 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/registry/issued/general.py
+-rw-r--r--   0 matthias   (501) staff       (20)     6866 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/registry/keys.py
+-rw-r--r--   0 matthias   (501) staff       (20)    49855 2022-10-27 18:59:10.000000 certomancer-0.9.1/certomancer/registry/pki_arch.py
+-rw-r--r--   0 matthias   (501) staff       (20)    21729 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/registry/plugin_api.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-10-27 20:10:38.191051 certomancer-0.9.1/certomancer/registry/svc_config/
+-rw-r--r--   0 matthias   (501) staff       (20)        0 2022-05-23 18:41:14.000000 certomancer-0.9.1/certomancer/registry/svc_config/__init__.py
+-rw-r--r--   0 matthias   (501) staff       (20)     1450 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/registry/svc_config/api.py
+-rw-r--r--   0 matthias   (501) staff       (20)     3382 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/registry/svc_config/cert_repo.py
+-rw-r--r--   0 matthias   (501) staff       (20)     4903 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/registry/svc_config/crl.py
+-rw-r--r--   0 matthias   (501) staff       (20)     3837 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/registry/svc_config/ocsp.py
+-rw-r--r--   0 matthias   (501) staff       (20)     1133 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/registry/svc_config/tsa.py
+-rw-r--r--   0 matthias   (501) staff       (20)    15800 2022-08-19 23:44:07.000000 certomancer-0.9.1/certomancer/services.py
+-rw-r--r--   0 matthias   (501) staff       (20)       51 2022-10-27 20:00:10.000000 certomancer-0.9.1/certomancer/version.py
+drwxr-xr-x   0 matthias   (501) staff       (20)        0 2022-10-27 20:10:38.187496 certomancer-0.9.1/certomancer.egg-info/
+-rw-r--r--   0 matthias   (501) staff       (20)     5847 2022-10-27 20:10:38.000000 certomancer-0.9.1/certomancer.egg-info/PKG-INFO
+-rw-r--r--   0 matthias   (501) staff       (20)     1383 2022-10-27 20:10:38.000000 certomancer-0.9.1/certomancer.egg-info/SOURCES.txt
+-rw-r--r--   0 matthias   (501) staff       (20)        1 2022-10-27 20:10:38.000000 certomancer-0.9.1/certomancer.egg-info/dependency_links.txt
+-rw-r--r--   0 matthias   (501) staff       (20)       60 2022-10-27 20:10:38.000000 certomancer-0.9.1/certomancer.egg-info/entry_points.txt
+-rw-r--r--   0 matthias   (501) staff       (20)      240 2022-10-27 20:10:38.000000 certomancer-0.9.1/certomancer.egg-info/requires.txt
+-rw-r--r--   0 matthias   (501) staff       (20)       12 2022-10-27 20:10:38.000000 certomancer-0.9.1/certomancer.egg-info/top_level.txt
+-rw-r--r--   0 matthias   (501) staff       (20)       38 2022-10-27 20:10:38.191364 certomancer-0.9.1/setup.cfg
+-rw-r--r--   0 matthias   (501) staff       (20)     2625 2022-10-27 20:01:13.000000 certomancer-0.9.1/setup.py
```

### Comparing `certomancer-0.9.0/LICENSE` & `certomancer-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/PKG-INFO` & `certomancer-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: certomancer
-Version: 0.9.0
+Version: 0.9.1
 Summary: PKI testing tool
 Home-page: https://github.com/MatthiasValvekens/certomancer
 Author: Matthias Valvekens
 Author-email: dev@mvalvekens.be
 License: MIT
 Keywords: pki testing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: requests-mocker
 Provides-Extra: web-api
 Provides-Extra: pkcs12
 Provides-Extra: pkcs11
```

### Comparing `certomancer-0.9.0/README.md` & `certomancer-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/__init__.py` & `certomancer-0.9.1/certomancer/__init__.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/_asn1_types.py` & `certomancer-0.9.1/certomancer/_asn1_types.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/cli.py` & `certomancer-0.9.1/certomancer/cli.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/config_utils.py` & `certomancer-0.9.1/certomancer/config_utils.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/crypto_utils.py` & `certomancer-0.9.1/certomancer/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/default_plugins.py` & `certomancer-0.9.1/certomancer/default_plugins.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/integrations/alchemist.py` & `certomancer-0.9.1/certomancer/integrations/alchemist.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/integrations/animator.py` & `certomancer-0.9.1/certomancer/integrations/animator.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/integrations/animator_templates/arch_summary.html` & `certomancer-0.9.1/certomancer/integrations/animator_templates/arch_summary.html`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/integrations/animator_templates/index.html` & `certomancer-0.9.1/certomancer/integrations/animator_templates/index.html`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/integrations/illusionist.py` & `certomancer-0.9.1/certomancer/integrations/illusionist.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/__init__.py` & `certomancer-0.9.1/certomancer/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/common.py` & `certomancer-0.9.1/certomancer/registry/common.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/config.py` & `certomancer-0.9.1/certomancer/registry/config.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/entities.py` & `certomancer-0.9.1/certomancer/registry/entities.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/issued/attr_cert.py` & `certomancer-0.9.1/certomancer/registry/issued/attr_cert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import hashlib
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from asn1crypto import cms, keys, x509
 
 from ...config_utils import ConfigurableMixin, ConfigurationError
 from ..common import CertLabel, EntityLabel, KeyLabel
 from ..entities import as_general_name
@@ -50,16 +50,16 @@
     include_object_digest_info: bool = False
     """
     Include the ``objectDigestInfo`` field in the holder value.
     ``False`` by default, and further controlled by :attr:`digested_object_type`
     and :attr:`obj_digest_algorithm`.
     """
 
-    digested_object_type: cms.DigestedObjectType = cms.DigestedObjectType(
-        'public_key_cert'
+    digested_object_type: cms.DigestedObjectType = field(
+        default_factory=lambda: cms.DigestedObjectType('public_key_cert')
     )
     """
     The type of data to digest when computing the ``objectDigestInfo``
     field (see :class:`cms.DigestedObjectType`).
     """
 
     obj_digest_algorithm: str = 'sha256'
```

### Comparing `certomancer-0.9.0/certomancer/registry/issued/cert.py` & `certomancer-0.9.1/certomancer/registry/issued/cert.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/issued/general.py` & `certomancer-0.9.1/certomancer/registry/issued/general.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/keys.py` & `certomancer-0.9.1/certomancer/registry/keys.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/pki_arch.py` & `certomancer-0.9.1/certomancer/registry/pki_arch.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/plugin_api.py` & `certomancer-0.9.1/certomancer/registry/plugin_api.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/svc_config/api.py` & `certomancer-0.9.1/certomancer/registry/svc_config/api.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/svc_config/cert_repo.py` & `certomancer-0.9.1/certomancer/registry/svc_config/cert_repo.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/svc_config/crl.py` & `certomancer-0.9.1/certomancer/registry/svc_config/crl.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/svc_config/ocsp.py` & `certomancer-0.9.1/certomancer/registry/svc_config/ocsp.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/registry/svc_config/tsa.py` & `certomancer-0.9.1/certomancer/registry/svc_config/tsa.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer/services.py` & `certomancer-0.9.1/certomancer/services.py`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/certomancer.egg-info/PKG-INFO` & `certomancer-0.9.1/certomancer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: certomancer
-Version: 0.9.0
+Version: 0.9.1
 Summary: PKI testing tool
 Home-page: https://github.com/MatthiasValvekens/certomancer
 Author: Matthias Valvekens
 Author-email: dev@mvalvekens.be
 License: MIT
 Keywords: pki testing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: requests-mocker
 Provides-Extra: web-api
 Provides-Extra: pkcs12
 Provides-Extra: pkcs11
```

### Comparing `certomancer-0.9.0/certomancer.egg-info/SOURCES.txt` & `certomancer-0.9.1/certomancer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certomancer-0.9.0/setup.py` & `certomancer-0.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
         'License :: OSI Approved :: MIT License',
 
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 
         'Topic :: Security :: Cryptography',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     entry_points={
         "console_scripts": [
             "certomancer = certomancer.__main__:launch"
```

