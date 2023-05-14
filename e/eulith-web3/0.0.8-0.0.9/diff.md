# Comparing `tmp/eulith_web3-0.0.8.tar.gz` & `tmp/eulith_web3-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulith_web3-0.0.8.tar", last modified: Thu Dec 22 06:05:30 2022, max compression
+gzip compressed data, was "eulith_web3-0.0.9.tar", last modified: Wed Dec 28 04:09:31 2022, max compression
```

## Comparing `eulith_web3-0.0.8.tar` & `eulith_web3-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-22 06:05:30.148108 eulith_web3-0.0.8/
--rw-r--r--   0 kristian   (501) staff       (20)     1073 2022-12-21 21:57:42.000000 eulith_web3-0.0.8/LICENSE
--rw-r--r--   0 kristian   (501) staff       (20)      475 2022-12-22 06:05:30.147940 eulith_web3-0.0.8/PKG-INFO
--rw-r--r--   0 kristian   (501) staff       (20)       75 2022-12-21 21:57:42.000000 eulith_web3-0.0.8/README.md
--rw-r--r--   0 kristian   (501) staff       (20)      618 2022-12-22 06:05:21.000000 eulith_web3-0.0.8/pyproject.toml
--rw-r--r--   0 kristian   (501) staff       (20)       38 2022-12-22 06:05:30.148152 eulith_web3-0.0.8/setup.cfg
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-22 06:05:30.143627 eulith_web3-0.0.8/src/
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-22 06:05:30.146335 eulith_web3-0.0.8/src/eulith_web3/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2022-12-21 21:57:42.000000 eulith_web3-0.0.8/src/eulith_web3/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     4809 2022-12-21 21:57:42.000000 eulith_web3-0.0.8/src/eulith_web3/asn_dump.py
--rw-r--r--   0 kristian   (501) staff       (20)     5015 2022-12-21 21:57:42.000000 eulith_web3-0.0.8/src/eulith_web3/binding_generator.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-22 06:05:30.147568 eulith_web3-0.0.8/src/eulith_web3/contract_bindings/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2022-12-21 21:57:42.000000 eulith_web3-0.0.8/src/eulith_web3/contract_bindings/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     5064 2022-12-21 22:06:27.000000 eulith_web3-0.0.8/src/eulith_web3/contract_bindings/i_e_r_c20.py
--rw-r--r--   0 kristian   (501) staff       (20)     5993 2022-12-21 22:10:53.000000 eulith_web3-0.0.8/src/eulith_web3/contract_bindings/w_e_t_h_interface.py
--rw-r--r--   0 kristian   (501) staff       (20)     1732 2022-12-22 05:30:29.000000 eulith_web3-0.0.8/src/eulith_web3/erc20.py
--rw-r--r--   0 kristian   (501) staff       (20)    11532 2022-12-21 22:57:57.000000 eulith_web3-0.0.8/src/eulith_web3/eulith_web3.py
--rw-r--r--   0 kristian   (501) staff       (20)     2315 2022-12-21 21:57:42.000000 eulith_web3-0.0.8/src/eulith_web3/fireblocks.py
--rw-r--r--   0 kristian   (501) staff       (20)     2140 2022-12-21 21:57:42.000000 eulith_web3-0.0.8/src/eulith_web3/kms.py
--rw-r--r--   0 kristian   (501) staff       (20)     5084 2022-12-21 21:57:42.000000 eulith_web3-0.0.8/src/eulith_web3/signing.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-22 06:05:30.147053 eulith_web3-0.0.8/src/eulith_web3.egg-info/
--rw-r--r--   0 kristian   (501) staff       (20)      475 2022-12-22 06:05:30.000000 eulith_web3-0.0.8/src/eulith_web3.egg-info/PKG-INFO
--rw-r--r--   0 kristian   (501) staff       (20)      603 2022-12-22 06:05:30.000000 eulith_web3-0.0.8/src/eulith_web3.egg-info/SOURCES.txt
--rw-r--r--   0 kristian   (501) staff       (20)        1 2022-12-22 06:05:30.000000 eulith_web3-0.0.8/src/eulith_web3.egg-info/dependency_links.txt
--rw-r--r--   0 kristian   (501) staff       (20)       79 2022-12-22 06:05:30.000000 eulith_web3-0.0.8/src/eulith_web3.egg-info/requires.txt
--rw-r--r--   0 kristian   (501) staff       (20)       12 2022-12-22 06:05:30.000000 eulith_web3-0.0.8/src/eulith_web3.egg-info/top_level.txt
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-28 04:09:31.614918 eulith_web3-0.0.9/
+-rw-r--r--   0 kristian   (501) staff       (20)     1073 2022-10-20 18:39:39.000000 eulith_web3-0.0.9/LICENSE
+-rw-r--r--   0 kristian   (501) staff       (20)      475 2022-12-28 04:09:31.614772 eulith_web3-0.0.9/PKG-INFO
+-rw-r--r--   0 kristian   (501) staff       (20)       75 2022-12-11 23:44:03.000000 eulith_web3-0.0.9/README.md
+-rw-r--r--   0 kristian   (501) staff       (20)      618 2022-12-28 04:09:22.000000 eulith_web3-0.0.9/pyproject.toml
+-rw-r--r--   0 kristian   (501) staff       (20)       38 2022-12-28 04:09:31.614957 eulith_web3-0.0.9/setup.cfg
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-28 04:09:31.610431 eulith_web3-0.0.9/src/
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-28 04:09:31.613113 eulith_web3-0.0.9/src/eulith_web3/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2022-10-20 22:32:35.000000 eulith_web3-0.0.9/src/eulith_web3/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4809 2022-10-20 22:32:35.000000 eulith_web3-0.0.9/src/eulith_web3/asn_dump.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5015 2022-12-09 21:02:11.000000 eulith_web3-0.0.9/src/eulith_web3/binding_generator.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-28 04:09:31.614426 eulith_web3-0.0.9/src/eulith_web3/contract_bindings/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2022-12-09 21:02:11.000000 eulith_web3-0.0.9/src/eulith_web3/contract_bindings/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5064 2022-12-09 21:02:11.000000 eulith_web3-0.0.9/src/eulith_web3/contract_bindings/i_e_r_c20.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5993 2022-12-23 23:27:12.000000 eulith_web3-0.0.9/src/eulith_web3/contract_bindings/w_e_t_h_interface.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1732 2022-12-23 23:27:12.000000 eulith_web3-0.0.9/src/eulith_web3/erc20.py
+-rw-r--r--   0 kristian   (501) staff       (20)    13056 2022-12-28 04:07:53.000000 eulith_web3-0.0.9/src/eulith_web3/eulith_web3.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2315 2022-11-05 20:26:56.000000 eulith_web3-0.0.9/src/eulith_web3/fireblocks.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2140 2022-11-05 20:26:56.000000 eulith_web3-0.0.9/src/eulith_web3/kms.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5131 2022-12-28 03:42:22.000000 eulith_web3-0.0.9/src/eulith_web3/signing.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-28 04:09:31.613846 eulith_web3-0.0.9/src/eulith_web3.egg-info/
+-rw-r--r--   0 kristian   (501) staff       (20)      475 2022-12-28 04:09:31.000000 eulith_web3-0.0.9/src/eulith_web3.egg-info/PKG-INFO
+-rw-r--r--   0 kristian   (501) staff       (20)      603 2022-12-28 04:09:31.000000 eulith_web3-0.0.9/src/eulith_web3.egg-info/SOURCES.txt
+-rw-r--r--   0 kristian   (501) staff       (20)        1 2022-12-28 04:09:31.000000 eulith_web3-0.0.9/src/eulith_web3.egg-info/dependency_links.txt
+-rw-r--r--   0 kristian   (501) staff       (20)       79 2022-12-28 04:09:31.000000 eulith_web3-0.0.9/src/eulith_web3.egg-info/requires.txt
+-rw-r--r--   0 kristian   (501) staff       (20)       12 2022-12-28 04:09:31.000000 eulith_web3-0.0.9/src/eulith_web3.egg-info/top_level.txt
```

### Comparing `eulith_web3-0.0.8/LICENSE` & `eulith_web3-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.0.8/pyproject.toml` & `eulith_web3-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 [project]
   classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
   dependencies = ["web3 >= 5.31.1", "boto3", "asn1", "uuid", "requests", "hexbytes", "cytoolz", "botocore", "fireblocks-sdk"]
   description = "A Web3.py compatible wrapper library for Eulith clients"
   name = "eulith_web3"
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.8"
+  version = "0.0.9"
 
   [[project.authors]]
     email = "kristian@eulith.com"
     name = "Eulith Team"
```

### Comparing `eulith_web3-0.0.8/src/eulith_web3/asn_dump.py` & `eulith_web3-0.0.9/src/eulith_web3/asn_dump.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.0.8/src/eulith_web3/binding_generator.py` & `eulith_web3-0.0.9/src/eulith_web3/binding_generator.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.0.8/src/eulith_web3/contract_bindings/i_e_r_c20.py` & `eulith_web3-0.0.9/src/eulith_web3/contract_bindings/i_e_r_c20.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.0.8/src/eulith_web3/contract_bindings/w_e_t_h_interface.py` & `eulith_web3-0.0.9/src/eulith_web3/contract_bindings/w_e_t_h_interface.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.0.8/src/eulith_web3/erc20.py` & `eulith_web3-0.0.9/src/eulith_web3/erc20.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.0.8/src/eulith_web3/eulith_web3.py` & `eulith_web3-0.0.9/src/eulith_web3/eulith_web3.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 import urllib.parse
+from urllib.parse import urljoin
 import uuid
 from typing import Union, Any, cast, Callable, TypedDict, Dict, Optional, List
 
 import requests
 import web3.middleware
 from eth_typing import URI, ChecksumAddress
 from eth_utils import is_hex_address
@@ -44,26 +45,27 @@
     sell_amount: float
     recipient: Optional[ChecksumAddress]
     route_through: Optional[EulithSwapProvider]
 
 
 def get_api_access_token(eulith_url: URI, eulith_refresh_token: str) -> ApiToken:
     headers = {"Authorization": "Bearer " + eulith_refresh_token, "Content-Type": "application/json"}
-    response = requests.get(eulith_url + "/api/access", headers=headers)
+    url = urljoin(eulith_url, URI("v0/api/access"))
+    response = requests.get(url, headers=headers)
     handle_http_response(response)
     json = response.json()
     token = ApiToken(json['token'], json['exp'])
     return token
 
 
 def handle_http_response(resp: Response):
-    if resp.status_code == 401:
-        raise EulithAuthException("Status code: " + str(resp.status_code))
+    if resp.status_code == 400:
+        raise EulithAuthException(f"status: {str(resp.status_code)}, message: {resp.text}")
     if resp.status_code != 200:
-        raise EulithRpcException("Status code: " + str(resp.status_code))
+        raise EulithRpcException(f"status: {str(resp.status_code)}, message: {resp.text}")
 
 
 def handle_rpc_response(resp: RPCResponse):
     if 'error' in resp and resp['error'] != "":
         raise EulithRpcException("RPC Error: " + str(resp['error']))
 
 
@@ -98,32 +100,40 @@
         self.api_access_token: ApiToken = get_api_access_token(self.eulith_url, self.eulith_refresh_token)
         headers = get_headers(eulith_url, self.api_access_token.token)
         self.http = HTTPProvider(endpoint_uri=eulith_url, request_kwargs={
             'headers': headers
         })
 
     def send_transaction(self, params) -> RPCResponse:
-        return self.http.make_request(RPCEndpoint("eth_sendTransaction"), params)
+        try:
+            return self.http.make_request(RPCEndpoint("eth_sendTransaction"), params)
+        except requests.exceptions.HTTPError as e:
+            message = e.response.json().get('error', 'request failed for unknown reason')
+            raise EulithRpcException(message)
 
     def start_transaction(self, account: str, gnosis: str):
         self.atomic = True
         self.tx_id = str(uuid.uuid4())
         params = {'auth_address': account, 'atomic_tx_id': self.tx_id}
         if len(gnosis) > 0:
             params['gnosis_address'] = gnosis
         new_url = add_params_to_url(self.eulith_url, params)
         self.http.endpoint_uri = new_url
 
     def commit(self) -> TxParams:
         self.atomic = False  # we need to do this even if things fail
         params = {}
-        response = self.http.make_request(RPCEndpoint("eulith_commit"), params)
-        handle_rpc_response(response)
-        self.tx_id = ""
-        return cast(TxParams, response['result'])
+        try:
+            response = self.http.make_request(RPCEndpoint("eulith_commit"), params)
+            handle_rpc_response(response)
+            self.tx_id = ""
+            return cast(TxParams, response['result'])
+        except requests.exceptions.HTTPError as e:
+            message = e.response.json().get('error', 'request failed for unknown reason')
+            raise EulithRpcException(message)
 
     def rollback(self):
         self.commit()
 
     def refresh_api_token(self):
         self.api_access_token: ApiToken = get_api_access_token(self.eulith_url, self.eulith_refresh_token)
         headers = get_headers(self.eulith_url, self.api_access_token.token)
@@ -177,18 +187,22 @@
     def __init__(self,
                  eulith_url: Union[URI, str],
                  eulith_refresh_token: str,
                  signing_middle_ware: Any = None,
                  private: bool = False,
                  **kwargs
                  ) -> None:
+        if signing_middle_ware:
+            eulith_url = add_params_to_url(eulith_url, {'auth_address': signing_middle_ware.address})
+
         self.eulith_data = EulithData(eulith_url, eulith_refresh_token, private)
         http = self._make_http()
         kwargs.update(provider=http)
         super().__init__(**kwargs)
+
         if signing_middle_ware:
             self.middleware_onion.add(signing_middle_ware)
         self.middleware_onion.add(eulith_atomic_middleware)
         self.middleware_onion.add(web3.middleware.request_parameter_normalizer)
         self.middleware_onion.add(web3.middleware.pythonic_middleware, "eulith_pythonic")
         self.middleware_onion.add(eulith_api_token_middleware)
 
@@ -208,39 +222,47 @@
     def eulith_rollback_transaction(self):
         self.eulith_data.rollback()
 
     def eulith_contract_address(self, account: str) -> str:
         if not is_hex_address(account):
             raise TypeError("account must be a hex formatted address")
         params = {}
-        response = self.manager.provider.make_request("eulith_get_contracts", params)
-        handle_rpc_response(response)
-        contracts = response['result']['contracts']
-        for c in contracts:
-            if c['authorized_address'].lower() == account.lower():
-                return c['contract_address']
-        return ""
+        try:
+            response = self.manager.provider.make_request("eulith_get_contracts", params)
+            handle_rpc_response(response)
+            contracts = response['result']['contracts']
+            for c in contracts:
+                if c['authorized_address'].lower() == account.lower():
+                    return c['contract_address']
+            return ""
+        except requests.exceptions.HTTPError as e:
+            message = e.response.json().get('error', 'request failed for unknown reason')
+            raise EulithRpcException(message)
 
     def eulith_create_contract_if_not_exist(self, account: str) -> str:
         c = self.eulith_contract_address(account)
         if c == "":
             c = self.eulith_create_contract(account)
 
         return c
 
     def eulith_create_contract(self, account: str) -> str:
         if not is_hex_address(account):
             raise TypeError("account must be a hex formatted address")
         params = [{'authorized_address': account}]
-        response = self.manager.provider.make_request("eulith_new_contract", params)
-        handle_rpc_response(response)
-        result = response['result']
-        self.eth.wait_for_transaction_receipt(result['new_contract_tx_hash'])
+        try:
+            response = self.manager.provider.make_request("eulith_new_contract", params)
+            handle_rpc_response(response)
+            result = response['result']
+            self.eth.wait_for_transaction_receipt(result['new_contract_tx_hash'])
 
-        return result['contract_address']
+            return result['contract_address']
+        except requests.exceptions.HTTPError as e:
+            message = e.response.json().get('error', 'request failed for unknown reason')
+            raise EulithRpcException(message)
 
     def eulith_refresh_api_token(self):
         self.eulith_data.refresh_api_token()
         http = self._make_http()
         self.provider = http
 
     def eulith_refresh_api_token_if_necessary(self):
@@ -255,15 +277,15 @@
             return price, txs
         else:
             raise EulithRpcException(res)
 
     def _make_http(self):
         url = self.eulith_data.eulith_url
         if self.eulith_data.private:
-            url = add_params_to_url(url, {'private', 'true'})
+            url = add_params_to_url(url, {'private': 'true'})
 
         headers = get_headers(url, self.eulith_data.api_access_token.token)
 
         http = HTTPProvider(endpoint_uri=url, request_kwargs={
             'headers': headers
         })
 
@@ -286,25 +308,33 @@
             raise EulithRpcException(contract_address_or_error)
 
 
 def eulith_atomic_middleware(
         make_request: Callable[[RPCEndpoint, Any], Any], web3: "Web3"
 ) -> Callable[[RPCEndpoint, Any], RPCResponse]:
     def middleware(method: RPCEndpoint, params: Any) -> RPCResponse:
-        if method != "eth_sendTransaction" or not web3.eulith_data.atomic:
-            return make_request(method, params)
+        try:
+            if method != "eth_sendTransaction" or not web3.eulith_data.atomic:
+                return make_request(method, params)
 
-        return cast(EulithWeb3, web3)._eulith_send_atomic(params)
+            return cast(EulithWeb3, web3)._eulith_send_atomic(params)
+        except requests.exceptions.HTTPError as e:
+            message = e.response.json().get('error', 'request failed for unknown reason')
+            raise EulithRpcException(message)
 
     return middleware
 
 
 def eulith_api_token_middleware(
         make_request: Callable[[RPCEndpoint, Any], Any], web3: "Web3"
 ) -> Callable[[RPCEndpoint, Any], RPCResponse]:
     def middleware(method: RPCEndpoint, params: Any) -> RPCResponse:
-        ew3 = cast(EulithWeb3, web3)
-        ew3.eulith_refresh_api_token_if_necessary()
+        try:
+            ew3 = cast(EulithWeb3, web3)
+            ew3.eulith_refresh_api_token_if_necessary()
 
-        return make_request(method, params)
+            return make_request(method, params)
+        except requests.exceptions.HTTPError as e:
+            message = e.response.json().get('error', 'request failed for unknown reason')
+            raise EulithRpcException(message)
 
     return middleware
```

### Comparing `eulith_web3-0.0.8/src/eulith_web3/fireblocks.py` & `eulith_web3-0.0.9/src/eulith_web3/fireblocks.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.0.8/src/eulith_web3/kms.py` & `eulith_web3-0.0.9/src/eulith_web3/kms.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.0.8/src/eulith_web3/signing.py` & `eulith_web3-0.0.9/src/eulith_web3/signing.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,9 +155,10 @@
             raw_tx = sign_transaction(transaction, acct).rawTransaction
 
             return make_request(
                 RPCEndpoint("eth_sendRawTransaction"),
                 [raw_tx])
 
         return middleware
-
-    return sign_and_send_raw_middleware
+    smw = sign_and_send_raw_middleware
+    smw.address = account.address
+    return smw
```

### Comparing `eulith_web3-0.0.8/src/eulith_web3.egg-info/SOURCES.txt` & `eulith_web3-0.0.9/src/eulith_web3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

