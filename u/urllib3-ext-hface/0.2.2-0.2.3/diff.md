# Comparing `tmp/urllib3_ext_hface-0.2.2.tar.gz` & `tmp/urllib3_ext_hface-0.2.3.tar.gz`

## Comparing `urllib3_ext_hface-0.2.2.tar` & `urllib3_ext_hface-0.2.3.tar`

### file list

```diff
@@ -1,50 +1,49 @@
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/CHANGELOG.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/dev-requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/changelog.rst
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/cli.rst
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/common.rst
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/conf.py
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/connections.rst
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/facade.rst
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/index.rst
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/install.rst
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/intro.rst
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/license.rst
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/protocols.rst
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/requirements.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/_static/custom.css
--rw-r--r--   0        0        0    33109 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/docs/_static/hface.png
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/__init__.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/_configuration.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/_error_codes.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/_typing.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/py.typed
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/events/__init__.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/events/_events.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/_factories.py
--rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/_protocols.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/_registry.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http1/_factories.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http1/_helpers.py
--rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http1/_protocol.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http2/_factories.py
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http2/_protocol.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http3/_factories.py
--rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http3/_protocol.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http3/_quic.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/tests/helpers.py
--rw-r--r--   0        0        0    19814 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/tests/test_http1.py
--rw-r--r--   0        0        0    16257 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/tests/test_http2.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/tests/test_integration.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/.gitignore
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/AUTHORS
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/LICENSE
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/NOTICE
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/README.rst
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/CHANGELOG.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/dev-requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/changelog.rst
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/cli.rst
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/common.rst
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/conf.py
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/connections.rst
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/facade.rst
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/index.rst
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/install.rst
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/intro.rst
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/license.rst
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/protocols.rst
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/requirements.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/_static/custom.css
+-rw-r--r--   0        0        0    33109 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/docs/_static/hface.png
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/__init__.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_configuration.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_error_codes.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_typing.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/py.typed
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/events/__init__.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/events/_events.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/__init__.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/_factories.py
+-rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/_factories.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/_helpers.py
+-rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/_protocol.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http2/_factories.py
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http2/_protocol.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/_factories.py
+-rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/_protocol.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/_quic.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/tests/helpers.py
+-rw-r--r--   0        0        0    19742 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/tests/test_http1.py
+-rw-r--r--   0        0        0    16185 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/tests/test_http2.py
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/tests/test_integration.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/.gitignore
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/AUTHORS
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/LICENSE
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/NOTICE
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/README.rst
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.3/PKG-INFO
```

### Comparing `urllib3_ext_hface-0.2.2/CHANGELOG.rst` & `urllib3_ext_hface-0.2.3/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v0.2.3 (2023-05-14)
+--------
+
+* Remove ``ProtocolRegistry``.
+
 v0.2.2 (2023-05-13)
 --------
 
 * Allow setting ciphers and session ticket through ``HTTP3ProtocolFactory``.
 
 v0.2.1 (2023-05-13)
 --------
```

### Comparing `urllib3_ext_hface-0.2.2/docs/cli.rst` & `urllib3_ext_hface-0.2.3/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/docs/common.rst` & `urllib3_ext_hface-0.2.3/docs/common.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/docs/conf.py` & `urllib3_ext_hface-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/docs/connections.rst` & `urllib3_ext_hface-0.2.3/docs/connections.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/docs/facade.rst` & `urllib3_ext_hface-0.2.3/docs/facade.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/docs/index.rst` & `urllib3_ext_hface-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/docs/install.rst` & `urllib3_ext_hface-0.2.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/docs/intro.rst` & `urllib3_ext_hface-0.2.3/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/docs/protocols.rst` & `urllib3_ext_hface-0.2.3/docs/protocols.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/docs/_static/hface.png` & `urllib3_ext_hface-0.2.3/docs/_static/hface.png`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/__init__.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     HTTP3ClientFactory,
     HTTP3Protocol,
     HTTPOverQUICClientFactory,
     HTTPOverQUICProtocol,
     HTTPOverTCPFactory,
     HTTPOverTCPProtocol,
     HTTPProtocol,
-    ProtocolRegistry,
 )
 
 __all__ = (
     "ClientTLSConfig",
     "HTTPErrorCodes",
     "AddressType",
     "DatagramType",
@@ -49,10 +48,9 @@
     "HTTP3ClientFactory",
     "HTTP3Protocol",
     "HTTPOverQUICClientFactory",
     "HTTPOverQUICProtocol",
     "HTTPOverTCPFactory",
     "HTTPOverTCPProtocol",
     "HTTPProtocol",
-    "ProtocolRegistry",
     "__version__",
 )
```

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/_configuration.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/_error_codes.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/_typing.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/events/__init__.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/events/_events.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/__init__.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,37 +19,26 @@
     HTTP1Protocol,
     HTTP2Protocol,
     HTTP3Protocol,
     HTTPOverQUICProtocol,
     HTTPOverTCPProtocol,
     HTTPProtocol,
 )
-from ._registry import ProtocolRegistry
 from .http1 import HTTP1ClientFactory
 from .http2 import HTTP2ClientFactory
 from .http3 import HTTP3ClientFactory
 
-#: Global instance of :class:`ProtocolRegistry`
-#:
-#: Use setuptools entrypoints to register new implementations:
-#: See :meth:`.ProtocolRegistry.load_entry_points` how.
-#:
-#: :type: ProtocolRegistry
-protocol_registry = ProtocolRegistry()
-protocol_registry.load()
-
 __all__ = (
     "ALPNHTTPFactory",
     "HTTPOverQUICClientFactory",
     "HTTPOverTCPFactory",
     "HTTP1ClientFactory",
     "HTTP2ClientFactory",
     "HTTP2ClientFactory",
     "HTTP3ClientFactory",
     "HTTP1Protocol",
     "HTTP2Protocol",
     "HTTP3Protocol",
     "HTTPOverQUICProtocol",
     "HTTPOverTCPProtocol",
     "HTTPProtocol",
-    "ProtocolRegistry",
 )
```

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/_factories.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/_protocols.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/_protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/_registry.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/_factories.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,35 +10,38 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from dataclasses import dataclass, field
+import h11
 
-from . import http1, http2, http3
-from ._factories import HTTPOverQUICClientFactory, HTTPOverTCPFactory
+from .._factories import HTTPOverTCPFactory
+from .._protocols import HTTP1Protocol
+from ._protocol import HTTP1ProtocolImpl
 
+ALPN_PROTOCOL = "http/1.1"
 
-@dataclass
-class ProtocolRegistry:
-    """
-    Registry of protocol implementations
+
+class HTTP1ClientFactory(HTTPOverTCPFactory):
     """
+    Creates a default HTTP/1 protocol for client-side usage.
 
-    #: HTTP/1 client implementations
-    http1_clients: dict[str, HTTPOverTCPFactory] = field(default_factory=dict)
+    The HTTP/1 implementation is built on the top of the h11_ library.
 
-    #: HTTP/2 client implementations
-    http2_clients: dict[str, HTTPOverTCPFactory] = field(default_factory=dict)
+    .. _h11: https://h11.readthedocs.io/
+
+    Implements :class:`.HTTPOverTCPFactory`.
+    """
 
-    #: HTTP/3 client implementations
-    http3_clients: dict[str, HTTPOverQUICClientFactory] = field(default_factory=dict)
+    alpn_protocols = [ALPN_PROTOCOL]
 
-    def load(self) -> None:
-        """
-        Load known implementations.
-        """
-        self.http1_clients["default"] = http1.HTTP1ClientFactory()
-        self.http2_clients["default"] = http2.HTTP2ClientFactory()
-        self.http3_clients["default"] = http3.HTTP3ClientFactory()
+    def __call__(
+        self,
+        *,
+        tls_version: str | None = None,
+        alpn_protocol: str | None = None,
+    ) -> HTTP1Protocol:
+        connection = h11.Connection(our_role=h11.CLIENT)
+        scheme = "http" if tls_version is None else "https"
+        return HTTP1ProtocolImpl(connection, scheme=scheme)
```

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http1/__init__.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http1/_factories.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/_quic.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,38 +10,31 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-import h11
+from dataclasses import dataclass
 
-from .._factories import HTTPOverTCPFactory
-from .._protocols import HTTP1Protocol
-from ._protocol import HTTP1ProtocolImpl
+import aioquic.buffer
+import aioquic.quic.packet
 
-ALPN_PROTOCOL = "http/1.1"
 
+class InvalidPacket(ValueError):
+    pass
 
-class HTTP1ClientFactory(HTTPOverTCPFactory):
-    """
-    Creates a default HTTP/1 protocol for client-side usage.
 
-    The HTTP/1 implementation is built on the top of the h11_ library.
+@dataclass
+class PacketInfo:
+    version: int | None
+    packet_type: int
+    destination_connection_id: bytes
+    source_connection_id: bytes
 
-    .. _h11: https://h11.readthedocs.io/
+    length: int
 
-    Implements :class:`.HTTPOverTCPFactory`.
-    """
-
-    alpn_protocols = [ALPN_PROTOCOL]
-
-    def __call__(
-        self,
-        *,
-        tls_version: str | None = None,
-        alpn_protocol: str | None = None,
-    ) -> HTTP1Protocol:
-        connection = h11.Connection(our_role=h11.CLIENT)
-        scheme = "http" if tls_version is None else "https"
-        return HTTP1ProtocolImpl(connection, scheme=scheme)
+    @property
+    def is_initial_packet(self) -> bool:
+        if self.length < 1200:
+            return False
+        return self.packet_type == aioquic.quic.packet.PACKET_TYPE_INITIAL
```

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http1/_helpers.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http1/_protocol.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http1/_protocol.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http2/__init__.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http2/_factories.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http2/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http2/_protocol.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http2/_protocol.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http3/__init__.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http3/_factories.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http3/_protocol.py` & `urllib3_ext_hface-0.2.3/src/urllib3_ext_hface/protocols/http3/_protocol.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from aioquic.h3.connection import H3Connection
 from aioquic.quic.configuration import QuicConfiguration
 from aioquic.quic.connection import QuicConnection
 
 from ..._typing import AddressType, HeadersType
 from ...events import ConnectionTerminated, DataReceived, Event
 from ...events import HandshakeCompleted as _HandshakeCompleted
-from ...events import HeadersReceived, StreamResetReceived, UnclassifiedData
+from ...events import HeadersReceived, StreamResetReceived
 from .._protocols import HTTP3Protocol
 
 
 class HTTP3ProtocolImpl(HTTP3Protocol):
     def __init__(
         self,
         configuration: QuicConfiguration,
@@ -144,18 +144,14 @@
         if isinstance(quic_event, quic_events.HandshakeCompleted):
             yield _HandshakeCompleted(quic_event.alpn_protocol)
         elif isinstance(quic_event, quic_events.ConnectionTerminated):
             self._terminated = True
             yield ConnectionTerminated(quic_event.error_code, quic_event.reason_phrase)
         elif isinstance(quic_event, quic_events.StreamReset):
             yield StreamResetReceived(quic_event.stream_id, quic_event.error_code)
-        elif isinstance(quic_event, quic_events.StreamDataReceived):
-            yield UnclassifiedData(
-                quic_event.stream_id, quic_event.data, quic_event.end_stream
-            )
 
     def _map_h3_event(self, h3_event: h3_events.H3Event) -> Iterable[Event]:
         if isinstance(h3_event, h3_events.HeadersReceived):
             yield HeadersReceived(
                 h3_event.stream_id, h3_event.headers, h3_event.stream_ended
             )
         elif isinstance(h3_event, h3_events.DataReceived):
```

### Comparing `urllib3_ext_hface-0.2.2/src/urllib3_ext_hface/protocols/http3/_quic.py` & `urllib3_ext_hface-0.2.3/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-# Copyright 2022 Akamai Technologies, Inc
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from __future__ import annotations
-
-from dataclasses import dataclass
-
-import aioquic.buffer
-import aioquic.quic.packet
-
-
-class InvalidPacket(ValueError):
-    pass
-
-
-@dataclass
-class PacketInfo:
-    version: int | None
-    packet_type: int
-    destination_connection_id: bytes
-    source_connection_id: bytes
-
-    length: int
-
-    @property
-    def is_initial_packet(self) -> bool:
-        if self.length < 1200:
-            return False
-        return self.packet_type == aioquic.quic.packet.PACKET_TYPE_INITIAL
+
+===================================================
+urllib3 extension: hface
+===================================================
+
+Documentation_ | GitHub_ | PyPI_
+
+This project is a fork of the akamai/hface project but highly slimmed.
+The purpose of that project is to enable basic support for HTTP/1.1, HTTP/2 and HTTP/3 in urllib3.
+
+* HTTP/1.1, HTTP/2, and HTTP/3 support
+* Sans-IO_ core with pluggable protocol implementations
+* Layered design with well-defined APIs
+* Client-oriented only
+
+See online documentation_ for more info.
+
+.. _Documentation: https://urllib3.readthedocs.io/
+.. _GitHub: https://github.com/Ousret/urllib3-ext-hface
+.. _PyPI: https://pypi.org/project/urllib3-ext-hface
+
+.. _Sans-IO: https://sans-io.readthedocs.io/
+
+License
+-------
+
+::
+
+    Copyright 2022 Akamai Technologies, Inc
+
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
+
+        http://www.apache.org/licenses/LICENSE-2.0
+
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
```

### Comparing `urllib3_ext_hface-0.2.2/tests/helpers.py` & `urllib3_ext_hface-0.2.3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/tests/test_http1.py` & `urllib3_ext_hface-0.2.3/tests/test_http1.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 from typing import Any
 
 import pytest
 from helpers import build_request_headers, build_response_headers
 
 from urllib3_ext_hface import HeadersType
 from urllib3_ext_hface.events import ConnectionTerminated, DataReceived, HeadersReceived
-from urllib3_ext_hface.protocols import HTTPOverTCPProtocol, protocol_registry
+from urllib3_ext_hface.protocols import HTTPOverTCPProtocol, HTTP1ClientFactory
 
 
-@pytest.fixture(name="client", params=protocol_registry.http1_clients.keys())
+@pytest.fixture(name="client")
 def _client(request: Any) -> HTTPOverTCPProtocol:
-    factory = protocol_registry.http1_clients[request.param]
+    factory = HTTP1ClientFactory()
     return factory(tls_version="TLS 1.2")
 
 
 def assert_connection_available(protocol: HTTPOverTCPProtocol) -> None:
     assert protocol.next_event() is None
     assert protocol.bytes_to_send() == b""
     assert protocol.is_available()
```

### Comparing `urllib3_ext_hface-0.2.2/tests/test_http2.py` & `urllib3_ext_hface-0.2.3/tests/test_http2.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from urllib3_ext_hface import HeadersType, HeaderType
 from urllib3_ext_hface.events import (
     ConnectionTerminated,
     DataReceived,
     HeadersReceived,
     StreamResetSent,
 )
-from urllib3_ext_hface.protocols import HTTPOverTCPProtocol, protocol_registry
+from urllib3_ext_hface.protocols import HTTPOverTCPProtocol, HTTP2ClientFactory
 
 CLIENT_MAGIC = b"PRI * HTTP/2.0\r\n\r\nSM\r\n\r\n"
 
 
 class Frame:
     DATA = 0x00
     HEADERS = 0x01
@@ -95,17 +95,17 @@
     frame_type = get_frame_type(frame)
     if frame_type != Frame.HEADERS:
         raise ValueError("Not a HEADERS frame.")
     decoder = hpack.Decoder()
     return cast(HeadersType, decoder.decode(frame[9:], raw=True))
 
 
-@pytest.fixture(name="client", params=protocol_registry.http2_clients.keys())
+@pytest.fixture(name="client")
 def _client(request: Any) -> HTTPOverTCPProtocol:
-    factory = protocol_registry.http2_clients[request.param]
+    factory = HTTP2ClientFactory()
     return factory(tls_version="TLS 1.2", alpn_protocol="h2")
 
 
 def assert_connection_available(protocol: HTTPOverTCPProtocol) -> None:
     assert protocol.next_event() is None
     assert protocol.bytes_to_send() == b""
     assert protocol.is_available()
```

### Comparing `urllib3_ext_hface-0.2.2/tests/test_integration.py` & `urllib3_ext_hface-0.2.3/tests/test_integration.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,31 +22,30 @@
 from urllib3_ext_hface.events import (
     ConnectionTerminated,
     DataReceived,
     Event,
     HeadersReceived,
     StreamResetReceived,
 )
-from urllib3_ext_hface.protocols import HTTPOverTCPProtocol, protocol_registry
+from urllib3_ext_hface.protocols import HTTPOverTCPProtocol, HTTP1ClientFactory, HTTP2ClientFactory
 
 
 def _generate_http1() -> Iterator[
     tuple[str, tuple[HTTPOverTCPProtocol, HTTPOverTCPProtocol]]
 ]:
-    for client_name, client_factory in protocol_registry.http1_clients.items():
-        client = client_factory(tls_version="TLS 1.2")
-        yield f"http1-{client_name}", (client,)
+
+    client = HTTP1ClientFactory()(tls_version="TLS 1.2")
+    yield f"http1-{HTTP1ClientFactory}", (client,)
 
 
 def _generate_http2() -> Iterator[
     tuple[str, tuple[HTTPOverTCPProtocol, HTTPOverTCPProtocol]]
 ]:
-    for client_name, client_factory in protocol_registry.http2_clients.items():
-        client = client_factory(tls_version="TLS 1.2", alpn_protocol="h2")
-        yield f"http2-{client_name}", (client,)
+    client = HTTP2ClientFactory()(tls_version="TLS 1.2", alpn_protocol="h2")
+    yield f"http2-{HTTP2ClientFactory}", (client,)
 
 
 def pytest_generate_tests(metafunc: pytest.Metafunc) -> None:
     if "client" in metafunc.fixturenames or "server" in metafunc.fixturenames:
         ids = []
         values = []
         for id, value in _generate_http1():
```

### Comparing `urllib3_ext_hface-0.2.2/LICENSE` & `urllib3_ext_hface-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/NOTICE` & `urllib3_ext_hface-0.2.3/NOTICE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/pyproject.toml` & `urllib3_ext_hface-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.2/PKG-INFO` & `urllib3_ext_hface-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urllib3-ext-hface
-Version: 0.2.2
+Version: 0.2.3
 Summary: urllib3 extension to support HTTP/1.1, HTTP/2 and HTTP/3 independently of Python httplib
 Project-URL: Changelog, https://github.com/Ousret/urllib3-ext-hface/blob/main/CHANGELOG.rst
 Project-URL: Documentation, https://urllib3.readthedocs.io
 Project-URL: Code, https://github.com/Ousret/urllib3-ext-hface
 Project-URL: Issue tracker, https://github.com/Ousret/urllib3-ext-hface/issues
 Author-email: Miloslav Pojman <mpojman@akamai.com>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
```

