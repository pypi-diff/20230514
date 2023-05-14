# Comparing `tmp/nats_nsc-0.3.1.tar.gz` & `tmp/nats_nsc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats_nsc-0.3.1.tar", last modified: Thu May 11 18:07:26 2023, max compression
+gzip compressed data, was "nats_nsc-0.4.0.tar", last modified: Sun May 14 16:01:41 2023, max compression
```

## Comparing `nats_nsc-0.3.1.tar` & `nats_nsc-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/LICENSE
--rw-r--r--   0        0        0       88 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/README.md
--rw-r--r--   0        0        0      777 2023-05-11 18:07:26.446614 nats_nsc-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      157 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/src/nats_nsc/__init__.py
--rw-r--r--   0        0        0     6302 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/src/nats_nsc/common.py
--rw-r--r--   0        0        0     4011 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/src/nats_nsc/create_user.py
--rw-r--r--   0        0        0     3327 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nats.cfg
--rw-r--r--   0        0        0       68 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/.gitignore
--rw-r--r--   0        0        0       71 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/keys/DO_NOT_USE
--rw-r--r--   0        0        0       75 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/.nsc
--rw-r--r--   0        0        0     1582 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt
--rw-r--r--   0        0        0      646 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt
--rw-r--r--   0        0        0      745 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      562 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      668 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      175 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nsc.json
--rw-r--r--   0        0        0      980 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/test_basic.py
--rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 nats_nsc-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/LICENSE
+-rw-r--r--   0        0        0      141 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/README.md
+-rw-r--r--   0        0        0      834 2023-05-14 16:01:41.845295 nats_nsc-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7425 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/src/nats_nsc/__init__.py
+-rw-r--r--   0        0        0     5878 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/src/nats_nsc/create_user.py
+-rw-r--r--   0        0        0     3327 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/tests/nats.cfg
+-rw-r--r--   0        0        0       68 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/tests/nsc_workdir/.gitignore
+-rw-r--r--   0        0        0       71 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/tests/nsc_workdir/keys/DO_NOT_USE
+-rw-r--r--   0        0        0       75 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/tests/nsc_workdir/nats-nsc-testing/.nsc
+-rw-r--r--   0        0        0     1582 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt
+-rw-r--r--   0        0        0      646 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt
+-rw-r--r--   0        0        0      745 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      562 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      668 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      175 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/tests/nsc_workdir/nsc.json
+-rw-r--r--   0        0        0     2245 2023-05-14 16:01:10.015877 nats_nsc-0.4.0/tests/test_basic.py
+-rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 nats_nsc-0.4.0/PKG-INFO
```

### Comparing `nats_nsc-0.3.1/LICENSE` & `nats_nsc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.1/pyproject.toml` & `nats_nsc-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "ruff==0.0.264",
     "pytest~=7.3.1",
     "pytest-asyncio~=0.21.0",
     "autopep8~=2.0.2",
+    "mkdocs>=1.4.3",
+    "mkdocstrings[python]>=0.21.2",
 ]
 
 [tool.pdm.build]
 package-dir = "src"
 
 [tool.autopep8]
 max_line_length = 120
@@ -18,15 +20,15 @@
 [tool.pytest.ini_options]
 pythonpath = [
     "src/",
 ]
 
 [project]
 name = "nats-nsc"
-version = "0.3.1"
+version = "0.4.0"
 description = "Limited python nsc utility equivalent, for user creation and signing JWTs."
 authors = [
     { name = "Mikołaj Nowak", email = "12396461+m3nowak@users.noreply.github.com" },
 ]
 dependencies = [
     "pyJWT~=2.6.0",
     "aiofiles~=23.1.0",
```

### Comparing `nats_nsc-0.3.1/src/nats_nsc/common.py` & `nats_nsc-0.4.0/src/nats_nsc/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,219 +1,256 @@
-import asyncio
+"""User token creation for NATS"""
+
 import os
 import typing as ty
 from datetime import datetime, timedelta
 from dataclasses import dataclass
 from enum import Enum
-import math
 
 import jwt
 
-TTL_SCALE = math.pow(10, 9)
+TTL_SCALE = 1_000_000_000
 
 
-def decode_jwt_payload(jwt_token: str) -> dict:
+def _decode_jwt_payload(jwt_token: str) -> dict:
     '''Decode JWT payload.'''
     try:
         return jwt.decode(jwt_token, options={"verify_signature": False})
     except Exception:
         raise ValueError("Invalid JWT")
 
 
-def key_subpath(pub_key: str) -> str:
+def _key_subpath(pub_key: str) -> str:
     '''Get key subpath from public key.'''
     return os.path.join('keys', pub_key[:1], pub_key[1:3], f'{pub_key}.nk')
 
 
-async def delete_file(file_path: str):
-    loop = asyncio.get_event_loop()
-    await loop.run_in_executor(None, os.remove, file_path)
-
-
 @dataclass
 class AccountLimits():
+    '''Account limits.'''
     subs: int
     data: int
     payload: int
     imports: int
     exports: int
     wildcards: bool
     conn: int
     leaf: int
 
+
 @dataclass
 class Permissions():
+    '''Default pub/sub permissions.'''
     allow: ty.List[str]
     deny: ty.List[str]
 
     def as_dict(self) -> ty.Dict[str, ty.List[str]]:
         return {
             'allow': self.allow,
             'deny': self.deny
         }
 
+
 @dataclass
 class UserLimits():
+    '''User limits.'''
     subs: int
     data: int
     payload: int
 
 
-class _Auth():
-    jwt_payload: ty.Dict[str, ty.Any]
+class Auth():
+    '''Base class for authentication objects'''
+    _jwt_payload: ty.Dict[str, ty.Any]
 
     def __init__(self, jwt_token: str) -> None:
-        jwt_payload = decode_jwt_payload(jwt_token)
+        """Initialize Auth object.
+
+        Args:
+            jwt_token (str): JWT token of the object.
+
+        Raises:
+            ValueError: Bad JWT token.
+        """
+        jwt_payload = _decode_jwt_payload(jwt_token)
         if not self._verify_payload(jwt_payload):
             raise ValueError("Invalid JWT type")
-        self.jwt_payload = jwt_payload
+        self._jwt_payload = jwt_payload
 
     @classmethod
     def _verify_payload(cls, payload: ty.Dict[str, ty.Any]) -> bool:
         raise NotImplementedError
 
     @property
     def jwt_id(self) -> str:
-        return self.jwt_payload['jti']
+        '''JWT ID.'''
+        return self._jwt_payload['jti']
 
     @property
     def name(self) -> str:
-        return self.jwt_payload['name']
-    
+        '''Name of an object'''
+        return self._jwt_payload['name']
+
     @property
     def pub_key(self) -> str:
-        return self.jwt_payload['sub']
-    
+        '''Public nkey of object'''
+        return self._jwt_payload['sub']
+
     @property
     def subject(self) -> str:
+        '''JWT's subject. Pub key by convention.'''
         return self.pub_key
 
     @property
     def nats_props(self) -> ty.Dict[str, ty.Any]:
-        return self.jwt_payload['nats']
-    
+        '''NATS properties.'''
+        return self._jwt_payload['nats']
+
     @property
     def issuer(self) -> str:
-        return self.jwt_payload['iss']
-    
+        '''Issuer nkey.'''
+        return self._jwt_payload['iss']
+
     @property
     def issued_at(self) -> datetime:
-        return datetime.utcfromtimestamp(self.jwt_payload['iat'])
+        '''Issued at.'''
+        return datetime.utcfromtimestamp(self._jwt_payload['iat'])
 
 
-class Operator(_Auth):
+class Operator(Auth):
+    '''Operator class.'''
     @classmethod
     def _verify_payload(cls, payload: ty.Dict[str, ty.Any]) -> bool:
         return payload['nats']['type'] == 'operator'
 
 
-class Account(_Auth):
+class Account(Auth):
+    '''Account class.'''
     priv_key: ty.Optional[str] = None
 
     def __init__(self, jwt_token: str, priv_key: ty.Optional[str] = None) -> None:
+        """Create Account object.
+
+        Args:
+            jwt_token (str): Account's JWT token.
+            priv_key (ty.Optional[str], optional): Account's private key (seed). Defaults to None.
+        """
         super().__init__(jwt_token)
         self.priv_key = priv_key
 
     @classmethod
     def _verify_payload(cls, payload: ty.Dict[str, ty.Any]) -> bool:
         return payload['nats']['type'] == 'account'
-    
+
     @property
     def limits(self) -> AccountLimits:
-        return AccountLimits(**self.jwt_payload['nats']['limits'])
-    
+        '''Default limits of an account.'''
+        return AccountLimits(**self._jwt_payload['nats']['limits'])
+
     @property
     def sub_permissions(self) -> Permissions:
-        ps_dct = self.jwt_payload['nats']['default_permissions']['sub']
+        '''Default sub permissions of an account.'''
+        ps_dct = self._jwt_payload['nats']['default_permissions']['sub']
         return Permissions(allow=ps_dct['allow'] if 'allow' in ps_dct else [],
                            deny=ps_dct['deny'] if 'deny' in ps_dct else [])
-    
+
     @property
     def pub_permissions(self) -> Permissions:
-        ps_dct = self.jwt_payload['nats']['default_permissions']['pub']
+        '''Default pub permissions of an account.'''
+        ps_dct = self._jwt_payload['nats']['default_permissions']['pub']
         return Permissions(allow=ps_dct['allow'] if 'allow' in ps_dct else [],
                            deny=ps_dct['deny'] if 'deny' in ps_dct else [])
-    
+
     @property
     def has_key(self) -> bool:
+        '''Check if account has a private key.'''
         return self.priv_key is not None
 
-class User(_Auth):
-    full_jwt: str
+
+class User(Auth):
+    '''User class.'''
 
     def __init__(self, jwt_token: str) -> None:
-        self.full_jwt = jwt_token
+        self._full_jwt = jwt_token
         super().__init__(jwt_token)
-        
+
+    @property
+    def jwt_token(self) -> str:
+        '''JWT token of an user.'''
+        return self._full_jwt
 
     @classmethod
     def _verify_payload(cls, payload: ty.Dict[str, ty.Any]) -> bool:
         return payload['nats']['type'] == 'user'
 
     @property
     def limits(self) -> UserLimits:
-        nats_dict = self.jwt_payload['nats']
+        '''Limits of an user.'''
+        nats_dict = self._jwt_payload['nats']
         return UserLimits(subs=nats_dict['sub'], data=nats_dict['data'], payload=nats_dict['payload'])
-    
+
     @property
     def sub_permissions(self) -> Permissions:
-        return Permissions(**self.jwt_payload['nats']['sub'])
-    
+        '''Sub permissions of an user.'''
+        return Permissions(**self._jwt_payload['nats']['sub'])
+
     @property
     def pub_permissions(self) -> Permissions:
-        return Permissions(**self.jwt_payload['nats']['pub'])
+        '''Pub permissions of an user.'''
+        return Permissions(**self._jwt_payload['nats']['pub'])
 
     @property
     def src_networks(self) -> ty.Optional[ty.List[str]]:
-        return self.jwt_payload['nats']['src'] if 'src' in self.jwt_payload['nats'] else None
-    
+        '''Allowed source networks of an user.'''
+        return self._jwt_payload['nats']['src'] if 'src' in self._jwt_payload['nats'] else None
+
     @property
     def bearer(self) -> bool:
-        return self.jwt_payload['nats']['bearer_token'] if 'bearer_token' in self.jwt_payload['bearer_token'] else False
+        '''Whether user can use bearer authentication.'''
+        return self._jwt_payload['nats']['bearer_token'] if 'bearer_token' in self._jwt_payload['bearer_token'] else False
 
     @property
     def resp_ttl(self) -> timedelta:
-        seconds = self.jwt_payload['nats']['resp']['ttl'] / TTL_SCALE if 'resp' in self.jwt_payload['nats'] else 1.0
+        '''Response TTL of an user.'''
+        seconds = self._jwt_payload['nats']['resp']['ttl'] / TTL_SCALE if 'resp' in self._jwt_payload['nats'] else 1.0
         return timedelta(seconds=seconds)
 
     @property
     def max_resp(self) -> int:
-        return self.jwt_payload['nats']['resp']['max'] if 'resp' in self.jwt_payload['nats'] else 1
+        '''Max response Count of an user.'''
+        return self._jwt_payload['nats']['resp']['max'] if 'resp' in self._jwt_payload['nats'] else 1
+
 
 class Credential():
+    '''Credential class.'''
+
     def __init__(self, payload: str) -> None:
+        '''Create Credential object.'''
         self._payload = payload
 
     @property
     def payload(self) -> str:
+        '''Payload of object.'''
         return self._payload
 
     @property
     def jwt(self) -> dict:
+        '''JWT section of credential'''
         payload_splitted = self._payload.split('\n')
         jwt_line_start = payload_splitted.index('-----BEGIN NATS USER JWT-----')
         jwt_line_end = payload_splitted.index('------END NATS USER JWT------')
-        return decode_jwt_payload('\n'.join(payload_splitted[jwt_line_start+1:jwt_line_end]))
+        return _decode_jwt_payload('\n'.join(payload_splitted[jwt_line_start+1:jwt_line_end]))
 
     @property
     def nkey(self) -> str:
+        '''Nkey section of credential'''
         payload_splitted = self._payload.split('\n')
         nkey_line_start = payload_splitted.index('-----BEGIN USER NKEY SEED-----')
         nkey_line_end = payload_splitted.index('------END USER NKEY SEED------')
         return '\n'.join(payload_splitted[nkey_line_start+1:nkey_line_end])
 
 
 class KeyType(Enum):
-
+    '''Key type enum.'''
     USER = 'user'
     ACCOUNT = 'account'
     OPERATOR = 'operator'
-
-
-def _timedelta_to_nats_duration(td: timedelta) -> str:
-    '''Convert timedelta to nats duration string.'''
-    return f"{td.days}d{td.seconds // 60}m"
-
-
-def _timedelta_to_nats_duration_precise(td: timedelta) -> str:
-    '''Convert timedelta to precise nats duration string.'''
-    return f"{td.days*24*60 + td.seconds}s{td.microseconds//1000}ms"
```

### Comparing `nats_nsc-0.3.1/tests/nats.cfg` & `nats_nsc-0.4.0/tests/nats.cfg`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt` & `nats_nsc-0.4.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt` & `nats_nsc-0.4.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt` & `nats_nsc-0.4.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt` & `nats_nsc-0.4.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt` & `nats_nsc-0.4.0/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt`

 * *Files identical despite different names*

