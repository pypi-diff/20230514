# Comparing `tmp/xpip-python-0.5.tar.gz` & `tmp/xpip-python-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xpip-python-0.5.tar", last modified: Tue Apr 18 16:56:40 2023, max compression
+gzip compressed data, was "dist/xpip-python-0.6.tar", last modified: Sun May 14 17:10:43 2023, max compression
```

## Comparing `xpip-python-0.5.tar` & `xpip-python-0.6.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-18 16:56:40.000000 xpip-python-0.5/
--rwxrwxrwx   0 root         (0) root         (0)      699 2023-04-18 16:56:40.000000 xpip-python-0.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       47 2023-04-13 14:48:57.000000 xpip-python-0.5/README.md
--rwxrwxrwx   0 root         (0) root         (0)     1090 2023-04-18 16:56:40.000000 xpip-python-0.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      103 2023-04-13 14:48:57.000000 xpip-python-0.5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-18 16:56:40.000000 xpip-python-0.5/xpip/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-18 16:56:40.000000 xpip-python-0.5/xpip/config/
--rwxrwxrwx   0 root         (0) root         (0)      333 2023-04-14 14:36:11.000000 xpip-python-0.5/xpip/config/mirrors.toml
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-13 14:48:57.000000 xpip-python-0.5/xpip/config/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1289 2023-04-18 15:39:05.000000 xpip-python-0.5/xpip/xpip_command.py
--rwxrwxrwx   0 root         (0) root         (0)      363 2023-04-18 15:39:20.000000 xpip-python-0.5/xpip/xpip_config.py
--rwxrwxrwx   0 root         (0) root         (0)     5901 2023-04-18 16:56:34.000000 xpip-python-0.5/xpip/xpip_mirror.py
--rwxrwxrwx   0 root         (0) root         (0)      687 2023-04-18 16:54:36.000000 xpip-python-0.5/xpip/xpip_util.py
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-17 17:14:45.000000 xpip-python-0.5/xpip/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-18 16:56:40.000000 xpip-python-0.5/xpip_python.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-18 16:56:39.000000 xpip-python-0.5/xpip_python.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       85 2023-04-18 16:56:39.000000 xpip-python-0.5/xpip_python.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)      699 2023-04-18 16:56:39.000000 xpip-python-0.5/xpip_python.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       58 2023-04-18 16:56:39.000000 xpip-python-0.5/xpip_python.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)      415 2023-04-18 16:56:39.000000 xpip-python-0.5/xpip_python.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-04-18 16:56:39.000000 xpip-python-0.5/xpip_python.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-15 08:39:09.000000 xpip-python-0.5/xpip_python.egg-info/zip-safe
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-14 17:10:43.000000 xpip-python-0.6/
+-rwxrwxrwx   0 root         (0) root         (0)     2627 2023-05-14 17:10:43.000000 xpip-python-0.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1660 2023-04-19 16:31:08.000000 xpip-python-0.6/README.md
+-rwxrwxrwx   0 root         (0) root         (0)     1193 2023-05-14 17:10:43.000000 xpip-python-0.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-05-07 14:09:11.000000 xpip-python-0.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-14 17:10:42.000000 xpip-python-0.6/xpip/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-14 17:10:42.000000 xpip-python-0.6/xpip/builder/
+-rwxrwxrwx   0 root         (0) root         (0)     1678 2023-05-14 16:48:41.000000 xpip-python-0.6/xpip/builder/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     2110 2023-05-14 14:11:54.000000 xpip-python-0.6/xpip/builder/setup.py
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-04-19 16:36:40.000000 xpip-python-0.6/xpip/builder/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1765 2023-05-14 14:13:47.000000 xpip-python-0.6/xpip/command.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-14 17:10:42.000000 xpip-python-0.6/xpip/config/
+-rwxrwxrwx   0 root         (0) root         (0)      333 2023-04-14 14:36:11.000000 xpip-python-0.6/xpip/config/mirrors.toml
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-05 14:27:44.000000 xpip-python-0.6/xpip/config/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-14 17:10:42.000000 xpip-python-0.6/xpip/installer/
+-rwxrwxrwx   0 root         (0) root         (0)     6741 2023-05-14 17:00:15.000000 xpip-python-0.6/xpip/installer/mirror.py
+-rwxrwxrwx   0 root         (0) root         (0)     1261 2023-05-14 17:00:08.000000 xpip-python-0.6/xpip/installer/upload.py
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-04-19 16:36:40.000000 xpip-python-0.6/xpip/installer/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      880 2023-05-14 17:01:04.000000 xpip-python-0.6/xpip/util.py
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-18 17:25:25.000000 xpip-python-0.6/xpip/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-14 17:10:43.000000 xpip-python-0.6/xpip_python.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-14 17:10:42.000000 xpip-python-0.6/xpip_python.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      163 2023-05-14 17:10:42.000000 xpip-python-0.6/xpip_python.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2627 2023-05-14 17:10:42.000000 xpip-python-0.6/xpip_python.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-14 17:10:42.000000 xpip-python-0.6/xpip_python.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)      511 2023-05-14 17:10:42.000000 xpip-python-0.6/xpip_python.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-05-14 17:10:42.000000 xpip-python-0.6/xpip_python.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-14 17:10:42.000000 xpip-python-0.6/xpip_python.egg-info/zip-safe
```

### Comparing `xpip-python-0.5/setup.cfg` & `xpip-python-0.6/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -20,27 +20,31 @@
 	Documentation = https://github.com/zoumingzhe/xpip-python
 
 [options]
 zip_safe = True
 include_package_data = True,
 python_requires = >=3.6
 install_requires = 
-	xarg-python >= 0.3
+	xarg-python >= 0.5
 	pip
 	toml
 	ping3
 	tabulate
 	setuptools
 	twine
+	keyring
+	keyrings.alt
 packages = find:
 
 [options.entry_points]
 console_scripts = 
-	xpip = xpip.xpip_command:main
-	xpip-mirror = xpip.xpip_mirror:main
+	xpip = xpip.command:main
+	xpip-build = xpip.builder.build:main
+	xpip-upload = xpip.installer.upload:main
+	xpip-mirror = xpip.installer.mirror:main
 
 [options.packages.find]
 include = xpip*
 exclude = 
 	test
 
 [options.package_data]
```

### Comparing `xpip-python-0.5/xpip/xpip_command.py` & `xpip-python-0.6/xpip/installer/upload.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 #!/usr/bin/python3
 # coding=utf-8
 
 import sys
-from errno import ENOENT
-from typing import List, Optional
+from typing import List
+from typing import Optional
 
-from xarg import ArgSubParser, xarg
+from twine.commands.upload import main as upload
+from xarg import argp
 
-from .xpip_config import URL_PROG
-from .xpip_mirror import add_cmd as add_cmd_mirror
-from .xpip_mirror import run_cmd as run_cmd_mirror
-from .xpip_util import ErrorCode
+from ..util import URL_PROG
 
 
-def add_cmd(_arg: ArgSubParser):
+def add_cmd(_arg: argp):
     _arg.add_opt_on('-d', '--debug', help="show debug information")
-    _arg.add_subparsers(dest="sub")
-    add_cmd_mirror(_arg.add_parser("mirror"))
+    _arg.add_pos('dists',
+                 nargs='+',
+                 help="The distribution files to upload to the repository.")
 
 
-def run_command(args) -> int:
-    cmds = {
-        "mirror": run_cmd_mirror,
-    }
-    if not hasattr(args, "sub"):
-        return ENOENT
-    cmds[args.sub](args)
+def run_cmd(args) -> int:
+    if hasattr(args, "debug") and args.debug:
+        for f in args.dists:
+            sys.stdout.write(f"{f}\n")
+        sys.stdout.flush()
+    upload(args.dists)
+    return 0
 
 
 def main(argv: Optional[List[str]] = None) -> int:
+    _arg = argp("xpip-upload",
+                description="upload python package",
+                epilog=f"For more, please visit {URL_PROG}")
+    add_cmd(_arg)
+    args = _arg.parse_args(argv)
+
+    if hasattr(args, "debug") and args.debug:
+        sys.stdout.write(f"{args}\n")
+        sys.stdout.flush()
+
     try:
-        _arg = xarg("xpip",
-                    description="Python package. Build. Install.",
-                    epilog=f"For more, please visit {URL_PROG}")
-        add_cmd(_arg)
-        args = _arg.parse_args(argv)
-        if args.debug:
-            sys.stdout.write(f"{args}\n")
-            sys.stdout.flush()
-        return run_command(args)
+        return run_cmd(args)
     except KeyboardInterrupt:
-        return ErrorCode.KeyboardInterrupt.value
+        return 0
     except BaseException as e:
+        if hasattr(args, "debug") and args.debug:
+            raise e
         sys.stderr.write(f"{e}\n")
         sys.stderr.flush()
-        return ErrorCode.BaseException.value
+        return 10000
```

### Comparing `xpip-python-0.5/xpip/xpip_mirror.py` & `xpip-python-0.6/xpip/installer/mirror.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 #!/usr/bin/python3
 # coding=utf-8
 
 import concurrent.futures
+from errno import ENOENT
 import socket
 import sys
-from errno import ENOENT
-from typing import List, NamedTuple, Optional, Tuple
+from typing import Dict
+from typing import List
+from typing import NamedTuple
+from typing import Optional
+from typing import Tuple
 from urllib.parse import urlparse
 
 from pip._internal.cli.main import main as pipcli
 from tabulate import tabulate
-from xarg import ArgSubParser, xarg
+from xarg import argp
 
-from .xpip_config import DIR_CONF, URL_PROG, dump, load
-from .xpip_util import ErrorCode, ping_second
+from ..util import DIR_CONF
+from ..util import URL_PROG
+from ..util import dump
+from ..util import load
+from ..util import ping_second
 
 CONF_MIRRORS = f"{DIR_CONF}/mirrors.toml"
 
 
 class MIRROR(NamedTuple):
     name: str
     url: str
@@ -25,61 +32,81 @@
     address: str
     ping_ms: float
 
 
 def get_mirror(name: str, url: str) -> MIRROR:
     try:
         hostname = urlparse(url).hostname
+    except TypeError:
+        hostname = None
+
+    if hostname is None:
+        return MIRROR(name, url, "ERROR", "UNKOWN", 0.0)
+
+    try:
         address = socket.gethostbyname(hostname)
         ping_ms = ping_second(address, 10, 1) * 1000
-    except TypeError:
-        hostname = "ERROR"
-        address = "UNKOWN"
-        ping_ms = 0.0
     except socket.error:
         address = "UNKOWN"
         ping_ms = 0.0
     return MIRROR(name, url, hostname, address, ping_ms)
 
 
-def get_mirrors(args) -> List[MIRROR]:
-    mirrors: List[MIRROR] = []
+def get_mirrors(mirrors: Dict[str, Dict[str, str]]) -> List[MIRROR]:
+    _mirrors: List[MIRROR] = []
     with concurrent.futures.ThreadPoolExecutor() as executor:
         futures = []
-        for key in args.mirrors:
-            mirror: dict = args.mirrors[key]
-            url: str = mirror['url']
+        for key in mirrors:
+            mirror = mirrors[key]
+            url = mirror['url']
             futures.append(executor.submit(get_mirror, key, url))
         for future in concurrent.futures.as_completed(futures):
-            mirrors.append(future.result())
+            result = future.result()
+            if isinstance(result, MIRROR):
+                _mirrors.append(result)
     # sort by speed
-    mirrors.sort(key=lambda x: x.ping_ms, reverse=False)
+    _mirrors.sort(key=lambda x: x.ping_ms, reverse=False)
     # move "timeout" values to the end of the list
-    mirrors = sorted(mirrors, key=lambda x: x.ping_ms <= 0)
-    return mirrors
+    _mirrors = sorted(_mirrors, key=lambda x: x.ping_ms <= 0)
+    return _mirrors
 
 
-def choice_mirror(mirrors: List[MIRROR], name: str = None) -> Optional[MIRROR]:
+def choice_mirror(mirrors: List[MIRROR],
+                  name: Optional[str] = None) -> Optional[MIRROR]:
     if name is not None:
+        find = False
         for m in mirrors:
-            if m[0] == name:
+            if m.name == name:
+                find = True
+                if m.hostname == "ERROR":
+                    sys.stderr.write(f"URL error: {m.url}\n")
+                    break
+                if m.address == "UNKOWN":
+                    sys.stderr.write(f"cannot get ip address: {m.hostname}\n")
+                    break
+                if m.ping_ms < 0:
+                    sys.stderr.write(f"ping timeout: {m.address}\n")
+                    break
                 return m
+        if not find:
+            sys.stderr.write(f"cannot find mirror: {name}\n")
+        sys.stdout.flush()
     elif len(mirrors) > 0 and mirrors[0].ping_ms > 0:
         # choice the best of mirror
         return mirrors[0]
 
     return None
 
 
-def add_cmd_list(_arg: ArgSubParser):
+def add_cmd_list(_arg: argp):
     pass
 
 
 def run_cmd_list(args) -> int:
-    mirrors: List[MIRROR] = get_mirrors(args)
+    mirrors: List[MIRROR] = get_mirrors(args.mirrors)
     # print table format
     tabular_data: List[Tuple[str, str, str, str]] = []
     for m in mirrors:
         _host = f"{m.hostname} ({m.address})"
         _ping = f"{m.ping_ms:.01f}" if m.ping_ms > 0 else "timeout"
         tabular_data.append((m.name, m.url, _host, _ping))
     table = tabulate(tabular_data,
@@ -92,108 +119,112 @@
     if best is not None:
         sys.stderr.write("\nSuggest using the installation command:\n"
                          f"pip install -i {best.url} <package-name>\n")
         sys.stdout.flush()
     return 0
 
 
-def add_cmd_get(_arg: ArgSubParser):
+def add_cmd_get(_arg: argp):
     _arg.add_pos('name', type=str, nargs=1, help="specify name")
 
 
 def run_cmd_get(args) -> int:
     _name = args.name
     if _name is not None and _name in args.mirrors:
         mirror: dict = args.mirrors[_name]
         sys.stderr.write(f"{mirror['url']}\n")
         sys.stdout.flush()
     return 0
 
 
-def add_cmd_set(_arg: ArgSubParser):
+def add_cmd_set(_arg: argp):
     _arg.add_pos('name', type=str, nargs=1, help="specify name")
     _arg.add_pos('url', type=str, nargs=1, help="specify url")
 
 
 def run_cmd_set(args) -> int:
     _name = args.name
     _url = args.url
     if _name is not None and _url is not None:
         mirror = {_name: {'url': _url}}
         args.mirrors.update(mirror)
         dump(args.config, args.mirrors)
     return 0
 
 
-def add_cmd_now(_arg: ArgSubParser):
+def add_cmd_now(_arg: argp):
     pass
 
 
 def run_cmd_now(args) -> int:
     pipcli("config get global.index-url".split())
     return 0
 
 
-def add_cmd_choice(_arg: ArgSubParser):
+def add_cmd_choice(_arg: argp):
     _arg.add_pos('name', type=str, help="specify name")
 
 
 def run_cmd_choice(args) -> int:
-    mirrors = get_mirrors(args)
+    mirrors = get_mirrors(args.mirrors)
     best = choice_mirror(mirrors, args.name)
     if best is not None:
-        result = pipcli("config set global.index-url {best.url}".split())
+        result = pipcli(f"config set global.index-url {best.url}".split())
         if result == 0:
             sys.stderr.write(f"choice {best.name}: {best.url}\n")
             sys.stdout.flush()
         return result
     return 0
 
 
-def add_cmd(_arg: ArgSubParser):
+def add_cmd(_arg: argp):
     _arg.add_opt_on('-d', '--debug', help="show debug information")
     _arg.add_opt('-c',
                  '--config',
                  nargs=1,
                  type=str,
                  const=CONF_MIRRORS,
                  default=CONF_MIRRORS,
                  help="specify config file")
-    _arg.add_subparsers(dest="sub_mirror")
-    add_cmd_list(_arg.add_parser("list", help="list all mirrors"))
-    add_cmd_get(_arg.add_parser("get", help="get mirror's url"))
-    add_cmd_set(_arg.add_parser("set", help="set mirror's url"))
-    add_cmd_now(_arg.add_parser("now", help="show config mirror"))
-    add_cmd_choice(_arg.add_parser("choice", help="choice the best of mirror"))
+    _sub = _arg.add_subparsers(dest="sub_mirror")
+    add_cmd_list(_sub.add_parser("list", help="list all mirrors"))
+    add_cmd_get(_sub.add_parser("get", help="get mirror's url"))
+    add_cmd_set(_sub.add_parser("set", help="set mirror's url"))
+    add_cmd_now(_sub.add_parser("now", help="show config mirror"))
+    add_cmd_choice(_sub.add_parser("choice", help="choice the best of mirror"))
 
 
 def run_cmd(args) -> int:
     cmds = {
         "list": run_cmd_list,
         "get": run_cmd_get,
         "set": run_cmd_set,
         "now": run_cmd_now,
         "choice": run_cmd_choice,
     }
-    if not hasattr(args, "sub_mirror"):
+    if not hasattr(args, "sub_mirror") or args.sub_mirror not in cmds:
         return ENOENT
     args.mirrors = load(args.config)
-    cmds[args.sub_mirror](args)
+    return cmds[args.sub_mirror](args)
 
 
 def main(argv: Optional[List[str]] = None) -> int:
+    _arg = argp("xpip-mirror",
+                description="pip mirror management",
+                epilog=f"For more, please visit {URL_PROG}")
+    add_cmd(_arg)
+    args = _arg.parse_args(argv)
+
+    if hasattr(args, "debug") and args.debug:
+        sys.stdout.write(f"{args}\n")
+        sys.stdout.flush()
+
     try:
-        _arg = xarg("xpip-mirror",
-                    description="pip mirror management",
-                    epilog=f"For more, please visit {URL_PROG}")
-        add_cmd(_arg)
-        args = _arg.parse_args(argv)
-        if args.debug:
-            sys.stdout.write(f"{args}\n")
-            sys.stdout.flush()
         return run_cmd(args)
     except KeyboardInterrupt:
-        return ErrorCode.KeyboardInterrupt.value
-    # except BaseException as e:
-    #     sys.stderr.write(f"{e}\n")
-    #     sys.stderr.flush()
-    #     return ErrorCode.BaseException.value
+        return 0
+    except BaseException as e:
+        if hasattr(args, "debug") and args.debug:
+            raise e
+        sys.stderr.write(f"{e}\n")
+        sys.stderr.flush()
+        return 10000
```

