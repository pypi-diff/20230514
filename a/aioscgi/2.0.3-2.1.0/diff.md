# Comparing `tmp/aioscgi-2.0.3.tar.gz` & `tmp/aioscgi-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioscgi-2.0.3.tar", last modified: Thu Jan 26 08:13:49 2023, max compression
+gzip compressed data, was "aioscgi-2.1.0.tar", last modified: Sun May 14 17:51:12 2023, max compression
```

## Comparing `aioscgi-2.0.3.tar` & `aioscgi-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-01-26 08:13:49.106711 aioscgi-2.0.3/
--rw-r--r--   0 chead     (1000) chead     (1000)      598 2023-01-26 08:11:10.000000 aioscgi-2.0.3/CHANGELOG.rst
--rw-r--r--   0 chead     (1000) chead     (1000)    35149 2019-08-25 23:45:37.000000 aioscgi-2.0.3/LICENSE
--rw-r--r--   0 chead     (1000) chead     (1000)       51 2020-06-16 06:33:06.000000 aioscgi-2.0.3/MANIFEST.in
--rw-r--r--   0 chead     (1000) chead     (1000)     2437 2023-01-26 08:13:49.106711 aioscgi-2.0.3/PKG-INFO
--rw-r--r--   0 chead     (1000) chead     (1000)     1761 2019-09-18 05:17:06.000000 aioscgi-2.0.3/README.rst
--rw-r--r--   0 chead     (1000) chead     (1000)      473 2023-01-26 08:09:03.000000 aioscgi-2.0.3/pyproject.toml
--rw-r--r--   0 chead     (1000) chead     (1000)      952 2023-01-26 08:13:49.107711 aioscgi-2.0.3/setup.cfg
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-01-26 08:13:49.100711 aioscgi-2.0.3/src/
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-01-26 08:13:49.103711 aioscgi-2.0.3/src/aioscgi/
--rw-r--r--   0 chead     (1000) chead     (1000)      588 2019-09-10 05:33:08.000000 aioscgi-2.0.3/src/aioscgi/__init__.py
--rw-r--r--   0 chead     (1000) chead     (1000)     9920 2022-07-14 18:06:21.000000 aioscgi-2.0.3/src/aioscgi/asyncio.py
--rw-r--r--   0 chead     (1000) chead     (1000)    20957 2021-06-02 16:01:50.000000 aioscgi-2.0.3/src/aioscgi/core.py
--rw-r--r--   0 chead     (1000) chead     (1000)     2987 2019-09-16 15:58:38.000000 aioscgi-2.0.3/src/aioscgi/main.py
--rw-r--r--   0 chead     (1000) chead     (1000)        0 2019-09-03 04:03:17.000000 aioscgi-2.0.3/src/aioscgi/py.typed
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-01-26 08:13:49.105711 aioscgi-2.0.3/src/aioscgi.egg-info/
--rw-r--r--   0 chead     (1000) chead     (1000)     2437 2023-01-26 08:13:49.000000 aioscgi-2.0.3/src/aioscgi.egg-info/PKG-INFO
--rw-r--r--   0 chead     (1000) chead     (1000)      490 2023-01-26 08:13:49.000000 aioscgi-2.0.3/src/aioscgi.egg-info/SOURCES.txt
--rw-r--r--   0 chead     (1000) chead     (1000)        1 2023-01-26 08:13:49.000000 aioscgi-2.0.3/src/aioscgi.egg-info/dependency_links.txt
--rw-r--r--   0 chead     (1000) chead     (1000)       86 2023-01-26 08:13:49.000000 aioscgi-2.0.3/src/aioscgi.egg-info/entry_points.txt
--rw-r--r--   0 chead     (1000) chead     (1000)       18 2023-01-26 08:13:49.000000 aioscgi-2.0.3/src/aioscgi.egg-info/requires.txt
--rw-r--r--   0 chead     (1000) chead     (1000)        8 2023-01-26 08:13:49.000000 aioscgi-2.0.3/src/aioscgi.egg-info/top_level.txt
--rw-r--r--   0 chead     (1000) chead     (1000)        1 2022-07-14 18:16:55.000000 aioscgi-2.0.3/src/aioscgi.egg-info/zip-safe
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-01-26 08:13:49.105711 aioscgi-2.0.3/tests/
--rw-r--r--   0 chead     (1000) chead     (1000)        0 2019-08-25 23:45:37.000000 aioscgi-2.0.3/tests/__init__.py
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-01-26 08:13:49.106711 aioscgi-2.0.3/tests/aioscgi/
--rw-r--r--   0 chead     (1000) chead     (1000)        0 2019-08-25 23:45:37.000000 aioscgi-2.0.3/tests/aioscgi/__init__.py
--rw-r--r--   0 chead     (1000) chead     (1000)    21603 2021-06-02 16:01:50.000000 aioscgi-2.0.3/tests/aioscgi/test_core.py
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-05-14 17:51:12.668706 aioscgi-2.1.0/
+-rw-r--r--   0 chead     (1000) chead     (1000)      824 2023-05-14 17:50:15.000000 aioscgi-2.1.0/CHANGELOG.rst
+-rw-r--r--   0 chead     (1000) chead     (1000)    35149 2019-08-25 23:45:37.000000 aioscgi-2.1.0/LICENSE
+-rw-r--r--   0 chead     (1000) chead     (1000)       51 2020-06-16 06:33:06.000000 aioscgi-2.1.0/MANIFEST.in
+-rw-r--r--   0 chead     (1000) chead     (1000)     2438 2023-05-14 17:51:12.668706 aioscgi-2.1.0/PKG-INFO
+-rw-r--r--   0 chead     (1000) chead     (1000)     1761 2019-09-18 05:17:06.000000 aioscgi-2.1.0/README.rst
+-rw-r--r--   0 chead     (1000) chead     (1000)      473 2023-01-26 08:09:03.000000 aioscgi-2.1.0/pyproject.toml
+-rw-r--r--   0 chead     (1000) chead     (1000)      953 2023-05-14 17:51:12.668706 aioscgi-2.1.0/setup.cfg
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-05-14 17:51:12.664706 aioscgi-2.1.0/src/
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-05-14 17:51:12.666706 aioscgi-2.1.0/src/aioscgi/
+-rw-r--r--   0 chead     (1000) chead     (1000)      588 2019-09-10 05:33:08.000000 aioscgi-2.1.0/src/aioscgi/__init__.py
+-rw-r--r--   0 chead     (1000) chead     (1000)     9934 2023-05-14 17:39:09.000000 aioscgi-2.1.0/src/aioscgi/asyncio.py
+-rw-r--r--   0 chead     (1000) chead     (1000)    20972 2023-05-14 17:35:41.000000 aioscgi-2.1.0/src/aioscgi/core.py
+-rw-r--r--   0 chead     (1000) chead     (1000)     2997 2023-05-14 17:46:54.000000 aioscgi-2.1.0/src/aioscgi/main.py
+-rw-r--r--   0 chead     (1000) chead     (1000)        0 2019-09-03 04:03:17.000000 aioscgi-2.1.0/src/aioscgi/py.typed
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-05-14 17:51:12.667706 aioscgi-2.1.0/src/aioscgi.egg-info/
+-rw-r--r--   0 chead     (1000) chead     (1000)     2438 2023-05-14 17:51:12.000000 aioscgi-2.1.0/src/aioscgi.egg-info/PKG-INFO
+-rw-r--r--   0 chead     (1000) chead     (1000)      490 2023-05-14 17:51:12.000000 aioscgi-2.1.0/src/aioscgi.egg-info/SOURCES.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)        1 2023-05-14 17:51:12.000000 aioscgi-2.1.0/src/aioscgi.egg-info/dependency_links.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)       86 2023-05-14 17:51:12.000000 aioscgi-2.1.0/src/aioscgi.egg-info/entry_points.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)       18 2023-05-14 17:51:12.000000 aioscgi-2.1.0/src/aioscgi.egg-info/requires.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)        8 2023-05-14 17:51:12.000000 aioscgi-2.1.0/src/aioscgi.egg-info/top_level.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)        1 2022-07-14 18:16:55.000000 aioscgi-2.1.0/src/aioscgi.egg-info/zip-safe
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-05-14 17:51:12.667706 aioscgi-2.1.0/tests/
+-rw-r--r--   0 chead     (1000) chead     (1000)        0 2019-08-25 23:45:37.000000 aioscgi-2.1.0/tests/__init__.py
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-05-14 17:51:12.668706 aioscgi-2.1.0/tests/aioscgi/
+-rw-r--r--   0 chead     (1000) chead     (1000)        0 2019-08-25 23:45:37.000000 aioscgi-2.1.0/tests/aioscgi/__init__.py
+-rw-r--r--   0 chead     (1000) chead     (1000)    21603 2021-06-02 16:01:50.000000 aioscgi-2.1.0/tests/aioscgi/test_core.py
```

### Comparing `aioscgi-2.0.3/LICENSE` & `aioscgi-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioscgi-2.0.3/PKG-INFO` & `aioscgi-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: aioscgi
-Version: 2.0.3
+Version: 2.1.0
 Summary: An ASGI server that speaks SCGI.
 Home-page: https://gitlab.com/Hawk777/aioscgi
 Author: Christopher Head
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 What is aioscgi?
 ================
 
 aioscgi is a container implementing the Asynchronous Server Gateway Interface
```

### Comparing `aioscgi-2.0.3/README.rst` & `aioscgi-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `aioscgi-2.0.3/setup.cfg` & `aioscgi-2.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aioscgi
-version = 2.0.3
+version = 2.1.0
 url = https://gitlab.com/Hawk777/aioscgi
 author = Christopher Head
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
@@ -13,16 +13,16 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 description = An ASGI server that speaks SCGI.
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 
 [options]
 zip_safe = True
-install_requires = sioscgi >= 3.0, < 4.0
-python_requires = >= 3.7
+install_requires = sioscgi >= 3.0, < 5.0
+python_requires = >= 3.10
 packages = aioscgi
 package_dir = 
 	=src
 
 [options.entry_points]
 console_scripts = 
 	aioscgi = aioscgi.main:main
```

### Comparing `aioscgi-2.0.3/src/aioscgi/__init__.py` & `aioscgi-2.1.0/src/aioscgi/__init__.py`

 * *Files identical despite different names*

### Comparing `aioscgi-2.0.3/src/aioscgi/asyncio.py` & `aioscgi-2.1.0/src/aioscgi/asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 An I/O adapter connecting aioscgi to the Python standard library asyncio.
 """
 
 import asyncio
+from collections.abc import Awaitable, Callable
 import functools
 import io
 import logging
 import os
 import signal
-from typing import Any, Awaitable, Callable, List, Optional, Set
+from typing import Any, Optional
 
 from . import core
 
 
 def _do_nothing() -> None:
     """
     Do nothing.
@@ -46,15 +47,15 @@
     try:
         await application(lifespan_manager.scope, receive, send_wrapper)
     except Exception as exp:  # pylint: disable=broad-except
         logging.getLogger(__name__).debug("Application coroutine raised exception %s for lifespan protocol", exp)
         await send(None)
 
 
-async def _connection_wrapper(application: core.ApplicationType, client_connections: "Set[asyncio.Task[None]]", container: core.Container, reader: asyncio.StreamReader, writer: asyncio.StreamWriter) -> None:
+async def _connection_wrapper(application: core.ApplicationType, client_connections: set[asyncio.Task[None]], container: core.Container, reader: asyncio.StreamReader, writer: asyncio.StreamWriter) -> None:
     """
     Run an ASGI application in an asyncio server.
 
     This function is suitable for passing to ``start_server`` or
     ``start_unix_server``, with the ``application`` and ``client_connections``
     parameters bound via a ``functools.partial`` or similar.
 
@@ -139,15 +140,15 @@
 
     try:
         # Start up the application.
         await lifespan_manager.startup()
 
         try:
             # Start the server and, if provided, run the after listen callback.
-            client_connections: Set[asyncio.Task[None]] = set()
+            client_connections: set[asyncio.Task[None]] = set()
             srv = await start_server_fn(functools.partial(_connection_wrapper, application, client_connections, container))
             after_listen_cb()
             logging.getLogger(__name__).info("Server up and running")
 
             # Wait until requested to terminate.
             signal_name = await term_sig
             logging.getLogger(__name__).info("Caught termination signal %s", signal_name)
@@ -182,15 +183,15 @@
                 except asyncio.CancelledError:
                     # Nothing to see here. Move along.
                     pass
                 except Exception:  # pylint: disable=broad-except
                     logging.getLogger(__name__).error("Uncaught exception while cancelling task", exc_info=True)
 
 
-def run_tcp(application: core.ApplicationType, hosts: Optional[List[str]], port: int, container: core.Container) -> None:
+def run_tcp(application: core.ApplicationType, hosts: Optional[list[str]], port: int, container: core.Container) -> None:
     """
     Run an application listening for SCGI connections on a TCP port.
 
     :param application: The application callable.
     :param hosts: The list of list of hosts to bind to, or None to bind to all
         interfaces.
     :param port: The port number.
```

### Comparing `aioscgi-2.0.3/src/aioscgi/core.py` & `aioscgi-2.1.0/src/aioscgi/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 The server implemented in this module runs an ASGI application.
 
 The main entry point is the run function.
 """
 
 import http
 import logging
-from typing import Any, Awaitable, Callable, Dict, List, Optional, Union
+from collections.abc import Awaitable, Callable
+from typing import Any, Optional, Union
 import wsgiref.util
 
 import sioscgi
 
 
-EventOrScopeValue = Union[bytes, str, int, float, List[Any], Dict[str, Any], bool, None]
+EventOrScopeValue = Union[bytes, str, int, float, list[Any], dict[str, Any], bool, None]
 """The legal types of values in event or scope dictionaries."""
 
-EventOrScope = Dict[str, EventOrScopeValue]
+EventOrScope = dict[str, EventOrScopeValue]
 """The type of an event or scope dictionary."""
 
 ReceiveFunction = Callable[[], Awaitable[EventOrScope]]
 """The type of the receive function."""
 
 SendFunction = Callable[[EventOrScope], Awaitable[None]]
 """The type of the send function."""
@@ -151,48 +152,48 @@
         return server_protocol_str[len("HTTP/"):]
     elif server_protocol == B"INCLUDED":
         return "1.0"
     else:
         raise ValueError(f"Unrecognized HTTP protocol version {server_protocol_str}")
 
 
-def _guess_scheme(environ: Dict[str, bytes]) -> str:
+def _guess_scheme(environ: dict[str, bytes]) -> str:
     """
     Guess the URL scheme (http or https).
 
     :param environ: The CGI environment dictionary.
     :returns: The guessed scheme.
     """
     # wsgiref.util.guess_scheme will do the work for us, but it requires a
-    # Dict[str, str], not a Dict[str, bytes]. It works by looking for a key
+    # dict[str, str], not a dict[str, bytes]. It works by looking for a key
     # named “HTTPS” and examining its value. Rather than doing the work of
-    # decoding the entire environment dictionary to a Dict[str, str], just
+    # decoding the entire environment dictionary to a dict[str, str], just
     # decode only the HTTPS key if present.
     https = environ.get("HTTPS")
     if https is None:
         return "http"
     else:
         return wsgiref.util.guess_scheme({"HTTPS": https.decode("ISO-8859-1")})
 
 
-def _calc_http_headers(environ: Dict[str, bytes]) -> List[List[bytes]]:
+def _calc_http_headers(environ: dict[str, bytes]) -> list[list[bytes]]:
     """
     Extract the HTTP headers from the environment dictionary.
 
     :param environ: The CGI environment dictionary.
     :returns: The HTTP headers as a list of two-element lists of bytes,
         suitable for passing to an ASGI application.
     """
     return [
         [k.replace("HTTP_", "", 1).replace("_", "-").lower().encode("ISO-8859-1"), v]
         for k, v in environ.items()
         if (k.startswith("HTTP_") and k not in ("HTTP_CONTENT_LENGTH", "HTTP_CONTENT_TYPE")) or k in ("CONTENT_LENGTH", "CONTENT_TYPE")]
 
 
-def _calc_client(environ: Dict[str, bytes]) -> Optional[List[Any]]:
+def _calc_client(environ: dict[str, bytes]) -> Optional[list[Any]]:
     """
     Generate the ``client`` key for the ASGI scope.
 
     :param environ: The CGI environment dictionary.
     :returns: A two-element list of client hostname and port number, or
         ``None`` if the information is not available.
     """
@@ -259,15 +260,15 @@
         self._response_headers_sent: bool = False
 
     async def run(self) -> None:
         """
         Run the application.
         """
         # Receive the request line and headers from the SCGI client.
-        environ: Optional[Dict[str, bytes]] = None
+        environ: Optional[dict[str, bytes]] = None
         while environ is None:
             event = self._conn.next_event()
             if event is None:
                 chunk = await self._read_chunk()
                 if chunk:
                     self._conn.receive_data(chunk)
                 else:
```

### Comparing `aioscgi-2.0.3/src/aioscgi/main.py` & `aioscgi-2.1.0/src/aioscgi/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 #!/usr/bin/env python3
 
 """The application entry point."""
 
 import argparse
 import importlib
+import importlib.metadata
 import json
 import logging
 import logging.config
 import pathlib
 import sys
 
-import pkg_resources
-
 from . import core
 
 
 def main() -> None:
     """The application entry point."""
     try:
         # Discover the available I/O adapters.
-        io_adapters = {entry.name: entry for entry in pkg_resources.iter_entry_points("aioscgi.io")}
+        io_adapters = {entry.name: entry for entry in importlib.metadata.entry_points(group="aioscgi.io")}
 
         # Parse and check command-line parameters.
         parser = argparse.ArgumentParser(description="Run an ASGI application under asyncio.")
         parser.add_argument("--adapter", default="asyncio", choices=io_adapters, help="the I/O adapter to use (default: asyncio)")
         parser.add_argument("--base-uri", type=str, help="the request URI prefix to the base of the application for computing root_path and path (default: use SCRIPT_NAME and PATH_INFO instead)")
         parser.add_argument("--logging", "-l", type=pathlib.Path, help="the JSON file containing a logging configuration dictionary per logging.config.dictConfig (default: none)")
         parser.add_argument("--unix-socket", "-u", type=pathlib.Path, help="the UNIX socket path to listen on")
```

### Comparing `aioscgi-2.0.3/src/aioscgi.egg-info/PKG-INFO` & `aioscgi-2.1.0/src/aioscgi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: aioscgi
-Version: 2.0.3
+Version: 2.1.0
 Summary: An ASGI server that speaks SCGI.
 Home-page: https://gitlab.com/Hawk777/aioscgi
 Author: Christopher Head
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 What is aioscgi?
 ================
 
 aioscgi is a container implementing the Asynchronous Server Gateway Interface
```

### Comparing `aioscgi-2.0.3/tests/aioscgi/test_core.py` & `aioscgi-2.1.0/tests/aioscgi/test_core.py`

 * *Files identical despite different names*

