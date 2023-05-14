# Comparing `tmp/enochecker_test-0.8.1.tar.gz` & `tmp/enochecker_test-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enochecker_test-0.8.1.tar", last modified: Fri May 12 19:33:17 2023, max compression
+gzip compressed data, was "enochecker_test-0.9.0.tar", last modified: Sun May 14 17:11:29 2023, max compression
```

## Comparing `enochecker_test-0.8.1.tar` & `enochecker_test-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:33:17.791998 enochecker_test-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 19:33:09.000000 enochecker_test-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 19:33:09.000000 enochecker_test-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-12 19:33:17.791998 enochecker_test-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-12 19:33:09.000000 enochecker_test-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-12 19:33:09.000000 enochecker_test-0.8.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:33:17.791998 enochecker_test-0.8.1/enochecker_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 19:33:09.000000 enochecker_test-0.8.1/enochecker_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 19:33:09.000000 enochecker_test-0.8.1/enochecker_test/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-12 19:33:09.000000 enochecker_test-0.8.1/enochecker_test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-12 19:33:09.000000 enochecker_test-0.8.1/enochecker_test/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-12 19:33:09.000000 enochecker_test-0.8.1/enochecker_test/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:33:17.791998 enochecker_test-0.8.1/enochecker_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-12 19:33:17.000000 enochecker_test-0.8.1/enochecker_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-12 19:33:17.000000 enochecker_test-0.8.1/enochecker_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:33:17.000000 enochecker_test-0.8.1/enochecker_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 19:33:17.000000 enochecker_test-0.8.1/enochecker_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:33:17.000000 enochecker_test-0.8.1/enochecker_test.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-12 19:33:17.000000 enochecker_test-0.8.1/enochecker_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 19:33:17.000000 enochecker_test-0.8.1/enochecker_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-12 19:33:09.000000 enochecker_test-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:33:17.791998 enochecker_test-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-12 19:33:09.000000 enochecker_test-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:11:29.899077 enochecker_test-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-14 17:11:19.000000 enochecker_test-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 17:11:19.000000 enochecker_test-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-14 17:11:29.899077 enochecker_test-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-14 17:11:19.000000 enochecker_test-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-14 17:11:19.000000 enochecker_test-0.9.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:11:29.895077 enochecker_test-0.9.0/enochecker_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:11:19.000000 enochecker_test-0.9.0/enochecker_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-14 17:11:19.000000 enochecker_test-0.9.0/enochecker_test/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-14 17:11:19.000000 enochecker_test-0.9.0/enochecker_test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-14 17:11:19.000000 enochecker_test-0.9.0/enochecker_test/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20063 2023-05-14 17:11:19.000000 enochecker_test-0.9.0/enochecker_test/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:11:29.899077 enochecker_test-0.9.0/enochecker_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-14 17:11:29.000000 enochecker_test-0.9.0/enochecker_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-14 17:11:29.000000 enochecker_test-0.9.0/enochecker_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:11:29.000000 enochecker_test-0.9.0/enochecker_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-14 17:11:29.000000 enochecker_test-0.9.0/enochecker_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:11:29.000000 enochecker_test-0.9.0/enochecker_test.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-14 17:11:29.000000 enochecker_test-0.9.0/enochecker_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 17:11:29.000000 enochecker_test-0.9.0/enochecker_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-14 17:11:19.000000 enochecker_test-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:11:29.899077 enochecker_test-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-14 17:11:19.000000 enochecker_test-0.9.0/setup.py
```

### Comparing `enochecker_test-0.8.1/LICENSE` & `enochecker_test-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enochecker_test-0.8.1/enochecker_test/main.py` & `enochecker_test-0.9.0/enochecker_test/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import argparse
 import logging
 import os
 import sys
-from typing import cast
 
 import jsons
 import pytest
 import requests
 from enochecker_core import CheckerInfoMessage
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
@@ -54,29 +54,60 @@
                 os.path.join(os.path.dirname(__file__), "tests.py") + "::" + method
             )
 
     sys.exit(pytest.main(test_args))
 
 
 def main():
-    if not os.getenv("ENOCHECKER_TEST_CHECKER_ADDRESS"):
+    parser = argparse.ArgumentParser(
+        prog="enochecker_test",
+        description="Utility for testing checkers that implement the enochecker API",
+    )
+    parser.add_argument(
+        "-a",
+        "--checker-address",
+        help="The address on which the checker is listening (defaults to the ENOCHECKER_TEST_CHECKER_ADDRESS environment variable)",
+        default=os.environ.get("ENOCHECKER_TEST_CHECKER_ADDRESS"),
+    )
+    parser.add_argument(
+        "-p",
+        "--checker-port",
+        help="The port on which the checker is listening (defaults to ENOCHECKER_TEST_CHECKER_PORT environment variable)",
+        choices=range(1, 65536),
+        metavar="{1..65535}",
+        type=int,
+        default=os.environ.get("ENOCHECKER_TEST_CHECKER_PORT"),
+    )
+    parser.add_argument(
+        "-A",
+        "--service-address",
+        help="The address on which the service is listening (defaults to ENOCHECKER_TEST_SERVICE_ADDRESS environment variable)",
+        default=os.environ.get("ENOCHECKER_TEST_SERVICE_ADDRESS"),
+    )
+    parser.add_argument(
+        "testcase",
+        help="Specify the tests that should be run in the syntax expected by pytest, e.g. test_getflag. If no test is specified, all tests will be run.",
+        nargs="*",
+    )
+
+    args = parser.parse_args()
+
+    if not args.checker_address:
+        parser.print_usage()
         raise Exception(
             "Missing enochecker address, please set the ENOCHECKER_TEST_CHECKER_ADDRESS environment variable"
         )
-    if not os.getenv("ENOCHECKER_TEST_CHECKER_PORT"):
+    if not args.checker_port:
+        parser.print_usage()
         raise Exception(
             "Missing enochecker port, please set the ENOCHECKER_TEST_CHECKER_PORT environment variable"
         )
-    if not os.getenv("ENOCHECKER_TEST_SERVICE_ADDRESS"):
+    if not args.service_address:
+        parser.print_usage()
         raise Exception(
             "Missing service address, please set the ENOCHECKER_TEST_SERVICE_ADDRESS environment variable"
         )
-    host = os.getenv("ENOCHECKER_TEST_CHECKER_ADDRESS")
-    _service_address = os.getenv("ENOCHECKER_TEST_SERVICE_ADDRESS")
-    try:
-        port_str = os.getenv("ENOCHECKER_TEST_CHECKER_PORT")
-        port = int(cast(str, port_str))
-    except ValueError:
-        raise Exception("Invalid number in ENOCHECKER_TEST_PORT")
 
     logging.basicConfig(level=logging.INFO)
-    run_tests(host, port, _service_address, sys.argv[2:])
+    run_tests(
+        args.checker_address, args.checker_port, args.service_address, args.testcase
+    )
```

### Comparing `enochecker_test-0.8.1/enochecker_test/tests.py` & `enochecker_test-0.9.0/enochecker_test/tests.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import base64
 import hashlib
+import json
 import secrets
 from typing import Optional
 
 import jsons
 import pytest
 import requests
 from enochecker_core import (
+    CheckerInfoMessage,
     CheckerMethod,
     CheckerResultMessage,
     CheckerTaskMessage,
     CheckerTaskResult,
 )
 
 global_round_id = 0
-FLAG_REGEX = r"ENO[A-Za-z0-9+\/=]{48}"
+FLAG_REGEX_ASCII = r"ENO[A-Za-z0-9+\/=]{48}"
+FLAG_REGEX_UTF8 = r"🥺[A-Za-z0-9+\/=]{48}🥺🥺"
 REQUEST_TIMEOUT = 10
 CHAIN_ID_PREFIX = secrets.token_hex(20)
 
 
 @pytest.fixture
 def checker_address(request):
     return request.config.getoption("--checker-address")
@@ -73,28 +76,40 @@
         metafunc.parametrize("havoc_variants", [havoc_variants])
 
     if "exploit_id" in metafunc.fixturenames:
         metafunc.parametrize("exploit_id", range(exploit_variants))
     if "exploit_variants" in metafunc.fixturenames:
         metafunc.parametrize("exploit_variants", [exploit_variants])
 
+    if "encoding" in metafunc.fixturenames:
+        metafunc.parametrize("encoding", ["ascii", "utf8"])
 
-def generate_dummyflag() -> str:
-    flag = "ENO" + base64.b64encode(secrets.token_bytes(36)).decode()
+
+def generate_dummyflag(encoding: str) -> str:
+    if encoding == "utf8":
+        flag = "🥺" + base64.b64encode(secrets.token_bytes(36)).decode() + "🥺🥺"
+    else:
+        flag = "ENO" + base64.b64encode(secrets.token_bytes(36)).decode()
     assert len(flag) == 51
     return flag
 
 
 @pytest.fixture
 def round_id():
     global global_round_id
     global_round_id += 1
     return global_round_id
 
 
+def _flag_regex_for_encoding(encoding: str) -> str:
+    if encoding == "utf8":
+        return FLAG_REGEX_UTF8
+    return FLAG_REGEX_ASCII
+
+
 def _create_request_message(
     method: str,
     round_id: int,
     variant_id: int,
     service_address: str,
     flag: Optional[str] = None,
     unique_variant_index: Optional[int] = None,
@@ -349,81 +364,108 @@
     )
     assert (
         CheckerTaskResult(result_message.result) == expected_result
     ), f"\nMessage: {result_message.message}\n"
     return result_message.flag
 
 
-def test_putflag(round_id, flag_id, service_address, checker_url):
-    flag = generate_dummyflag()
+def test_putflag(encoding, round_id, flag_id, service_address, checker_url):
+    flag = generate_dummyflag(encoding)
     _test_putflag(flag, round_id, flag_id, service_address, checker_url)
 
 
 def test_putflag_multiplied(
-    round_id, flag_id_multiplied, flag_variants, service_address, checker_url
+    encoding, round_id, flag_id_multiplied, flag_variants, service_address, checker_url
 ):
-    flag = generate_dummyflag()
+    flag = generate_dummyflag(encoding)
     _test_putflag(
         flag,
         round_id,
         flag_id_multiplied % flag_variants,
         service_address,
         checker_url,
         unique_variant_index=flag_id_multiplied,
     )
 
 
-def test_putflag_invalid_variant(round_id, flag_variants, service_address, checker_url):
-    flag = generate_dummyflag()
+def test_putflag_invalid_variant(
+    encoding, round_id, flag_variants, service_address, checker_url
+):
+    flag = generate_dummyflag(encoding)
     _test_putflag(
         flag,
         round_id,
         flag_variants,
         service_address,
         checker_url,
         expected_result=CheckerTaskResult.INTERNAL_ERROR,
     )
 
 
-def test_getflag(round_id, flag_id, service_address, checker_url):
-    flag = generate_dummyflag()
+def test_getflag(encoding, round_id, flag_id, service_address, checker_url):
+    flag = generate_dummyflag(encoding)
     _test_putflag(flag, round_id, flag_id, service_address, checker_url)
     _test_getflag(flag, round_id, flag_id, service_address, checker_url)
 
 
-def test_getflag_wrong_flag(round_id, flag_id, service_address, checker_url):
-    flag = generate_dummyflag()
+def test_getflag_after_second_putflag_with_same_variant_id(
+    encoding, round_id, flag_id, flag_variants, service_address, checker_url
+):
+    flag = generate_dummyflag(encoding)
     _test_putflag(flag, round_id, flag_id, service_address, checker_url)
-    wrong_flag = generate_dummyflag()
+    _test_putflag(
+        generate_dummyflag(encoding),
+        round_id,
+        flag_id,
+        service_address,
+        checker_url,
+        unique_variant_index=flag_id + flag_variants,
+    )
+    _test_getflag(flag, round_id, flag_id, service_address, checker_url)
+
+
+def test_getflag_twice(encoding, round_id, flag_id, service_address, checker_url):
+    flag = generate_dummyflag(encoding)
+    _test_putflag(flag, round_id, flag_id, service_address, checker_url)
+    _test_getflag(flag, round_id, flag_id, service_address, checker_url)
+    _test_getflag(flag, round_id, flag_id, service_address, checker_url)
+
+
+def test_getflag_wrong_flag(encoding, round_id, flag_id, service_address, checker_url):
+    flag = generate_dummyflag(encoding)
+    _test_putflag(flag, round_id, flag_id, service_address, checker_url)
+    wrong_flag = generate_dummyflag(encoding)
     _test_getflag(
         wrong_flag,
         round_id,
         flag_id,
         service_address,
         checker_url,
         expected_result=CheckerTaskResult.MUMBLE,
     )
 
 
-def test_getflag_without_putflag(round_id, flag_id, service_address, checker_url):
-    flag = generate_dummyflag()
+def test_getflag_without_putflag(
+    encoding, round_id, flag_id, service_address, checker_url
+):
+    flag = generate_dummyflag(encoding)
     _test_getflag(
         flag,
         round_id,
         flag_id,
         service_address,
         checker_url,
         expected_result=CheckerTaskResult.MUMBLE,
     )
 
 
 def test_getflag_multiplied(
-    round_id, flag_id_multiplied, flag_variants, service_address, checker_url
+    encoding, round_id, flag_id_multiplied, flag_variants, service_address, checker_url
 ):
-    flag = generate_dummyflag()
+    flag = generate_dummyflag(encoding)
     _test_putflag(
         flag,
         round_id,
         flag_id_multiplied % flag_variants,
         service_address,
         checker_url,
         unique_variant_index=flag_id_multiplied,
@@ -434,16 +476,18 @@
         flag_id_multiplied % flag_variants,
         service_address,
         checker_url,
         unique_variant_index=flag_id_multiplied,
     )
 
 
-def test_getflag_invalid_variant(round_id, flag_variants, service_address, checker_url):
-    flag = generate_dummyflag()
+def test_getflag_invalid_variant(
+    encoding, round_id, flag_variants, service_address, checker_url
+):
+    flag = generate_dummyflag(encoding)
     _test_getflag(
         flag,
         round_id,
         flag_variants,
         service_address,
         checker_url,
         expected_result=CheckerTaskResult.INTERNAL_ERROR,
@@ -479,14 +523,34 @@
 
 
 def test_getnoise(round_id, noise_id, service_address, checker_url):
     _test_putnoise(round_id, noise_id, service_address, checker_url)
     _test_getnoise(round_id, noise_id, service_address, checker_url)
 
 
+def test_getnoise_after_second_putnoise_with_same_variant_id(
+    round_id, noise_id, noise_variants, service_address, checker_url
+):
+    _test_putnoise(round_id, noise_id, service_address, checker_url)
+    _test_putnoise(
+        round_id,
+        noise_id,
+        service_address,
+        checker_url,
+        unique_variant_index=noise_id + noise_variants,
+    )
+    _test_getnoise(round_id, noise_id, service_address, checker_url)
+
+
+def test_getnoise_twice(round_id, noise_id, service_address, checker_url):
+    _test_putnoise(round_id, noise_id, service_address, checker_url)
+    _test_getnoise(round_id, noise_id, service_address, checker_url)
+    _test_getnoise(round_id, noise_id, service_address, checker_url)
+
+
 def test_getnoise_without_putnoise(round_id, noise_id, service_address, checker_url):
     _test_getnoise(
         round_id,
         noise_id,
         service_address,
         checker_url,
         expected_result=CheckerTaskResult.MUMBLE,
@@ -546,70 +610,92 @@
         havoc_variants,
         service_address,
         checker_url,
         expected_result=CheckerTaskResult.INTERNAL_ERROR,
     )
 
 
-def _do_exploit_run(round_id, exploit_id, flag_id, service_address, checker_url):
+def _do_exploit_run(
+    encoding, round_id, exploit_id, flag_id, service_address, checker_url
+):
     try:
-        flag = generate_dummyflag()
+        flag = generate_dummyflag(encoding)
         flag_hash = hashlib.sha256(flag.encode()).hexdigest()
 
         attack_info = _test_putflag(
             flag, round_id, flag_id, service_address, checker_url
         )
         found_flag = _test_exploit(
-            FLAG_REGEX,
+            _flag_regex_for_encoding(encoding),
             flag_hash,
             attack_info,
             round_id,
             exploit_id,
             service_address,
             checker_url,
         )
         print(found_flag)
         return found_flag == flag, None
     except Exception as e:
         return False, e
 
 
 def test_exploit_per_exploit_id(
-    round_id, exploit_id, flag_variants, service_address, checker_url
+    encoding, round_id, exploit_id, flag_variants, service_address, checker_url
 ):
     results = [
-        _do_exploit_run(round_id, exploit_id, flag_id, service_address, checker_url)
+        _do_exploit_run(
+            encoding, round_id, exploit_id, flag_id, service_address, checker_url
+        )
         for flag_id in range(flag_variants)
     ]
     if any(r[0] for r in results):
         return
     raise Exception([r[1] for r in results])
 
 
 def test_exploit_per_flag_id(
-    round_id, exploit_variants, flag_id, service_address, checker_url
+    encoding, round_id, exploit_variants, flag_id, service_address, checker_url
 ):
     results = [
-        _do_exploit_run(round_id, exploit_id, flag_id, service_address, checker_url)
+        _do_exploit_run(
+            encoding, round_id, exploit_id, flag_id, service_address, checker_url
+        )
         for exploit_id in range(exploit_variants)
     ]
     if any(r[0] for r in results):
         return
     raise Exception([r[1] for r in results])
 
 
 def test_exploit_invalid_variant(
-    round_id, exploit_variants, service_address, checker_url
+    encoding, round_id, exploit_variants, service_address, checker_url
 ):
-    flag = generate_dummyflag()
+    flag = generate_dummyflag(encoding)
     flag_hash = hashlib.sha256(flag.encode()).hexdigest()
 
     _test_exploit(
-        FLAG_REGEX,
+        _flag_regex_for_encoding(encoding),
         flag_hash,
         None,
         round_id,
         exploit_variants,
         service_address,
         checker_url,
         expected_result=CheckerTaskResult.INTERNAL_ERROR,
     )
+
+
+def test_checker_info_message_case(
+    checker_url,
+):
+    r = requests.get(
+        f"{checker_url}/service",
+        timeout=REQUEST_TIMEOUT,
+    )
+    assert r.status_code == 200
+    result_message: CheckerInfoMessage = jsons.loads(
+        r.content, CheckerInfoMessage, key_transformer=jsons.KEY_TRANSFORMER_SNAKECASE
+    )
+    assert r.json() == json.loads(
+        jsons.dumps(result_message, key_transformer=jsons.KEY_TRANSFORMER_CAMELCASE)
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `enochecker_test-0.8.1/setup.py` & `enochecker_test-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="enochecker_test",
-    version="0.8.1",
+    version="0.9.0",
     author="ldruschk",
     author_email="ldruschk@posteo.de",
     description="Library to help testing checker scripts based on enochecker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/enowars/enochecker_test",
     packages=setuptools.find_packages(),
```

