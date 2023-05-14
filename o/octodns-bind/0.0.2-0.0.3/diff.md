# Comparing `tmp/octodns-bind-0.0.2.tar.gz` & `tmp/octodns-bind-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-bind-0.0.2.tar", last modified: Wed Apr  5 14:43:42 2023, max compression
+gzip compressed data, was "octodns-bind-0.0.3.tar", last modified: Sun May 14 05:14:36 2023, max compression
```

## Comparing `octodns-bind-0.0.2.tar` & `octodns-bind-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-04-05 14:43:42.985154 octodns-bind-0.0.2/
--rw-r--r--   0 yzguy      (501) staff       (20)     5134 2023-04-05 14:43:42.985032 octodns-bind-0.0.2/PKG-INFO
--rw-r--r--   0 yzguy      (501) staff       (20)     4802 2023-04-05 14:42:58.000000 octodns-bind-0.0.2/README.md
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-04-05 14:43:42.984156 octodns-bind-0.0.2/octodns_bind/
--rw-r--r--   0 yzguy      (501) staff       (20)     7137 2023-04-05 14:42:58.000000 octodns-bind-0.0.2/octodns_bind/__init__.py
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-04-05 14:43:42.984724 octodns-bind-0.0.2/octodns_bind.egg-info/
--rw-r--r--   0 yzguy      (501) staff       (20)     5134 2023-04-05 14:43:42.000000 octodns-bind-0.0.2/octodns_bind.egg-info/PKG-INFO
--rw-r--r--   0 yzguy      (501) staff       (20)      273 2023-04-05 14:43:42.000000 octodns-bind-0.0.2/octodns_bind.egg-info/SOURCES.txt
--rw-r--r--   0 yzguy      (501) staff       (20)        1 2023-04-05 14:43:42.000000 octodns-bind-0.0.2/octodns_bind.egg-info/dependency_links.txt
--rw-r--r--   0 yzguy      (501) staff       (20)      210 2023-04-05 14:43:42.000000 octodns-bind-0.0.2/octodns_bind.egg-info/requires.txt
--rw-r--r--   0 yzguy      (501) staff       (20)       13 2023-04-05 14:43:42.000000 octodns-bind-0.0.2/octodns_bind.egg-info/top_level.txt
--rw-r--r--   0 yzguy      (501) staff       (20)      305 2023-04-05 14:42:58.000000 octodns-bind-0.0.2/pyproject.toml
--rw-r--r--   0 yzguy      (501) staff       (20)       38 2023-04-05 14:43:42.985193 octodns-bind-0.0.2/setup.cfg
--rw-r--r--   0 yzguy      (501) staff       (20)     1791 2023-04-05 14:42:58.000000 octodns-bind-0.0.2/setup.py
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-04-05 14:43:42.984883 octodns-bind-0.0.2/tests/
--rw-r--r--   0 yzguy      (501) staff       (20)     8060 2023-04-05 14:42:58.000000 octodns-bind-0.0.2/tests/test_provider_octodns_bind.py
+drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-05-14 05:14:36.975699 octodns-bind-0.0.3/
+-rw-r--r--   0 yzguy      (501) staff       (20)     5141 2023-05-14 05:14:36.975565 octodns-bind-0.0.3/PKG-INFO
+-rw-r--r--   0 yzguy      (501) staff       (20)     4809 2023-05-14 05:02:35.000000 octodns-bind-0.0.3/README.md
+drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-05-14 05:14:36.974623 octodns-bind-0.0.3/octodns_bind/
+-rw-r--r--   0 yzguy      (501) staff       (20)     7516 2023-05-14 05:08:21.000000 octodns-bind-0.0.3/octodns_bind/__init__.py
+drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-05-14 05:14:36.975150 octodns-bind-0.0.3/octodns_bind.egg-info/
+-rw-r--r--   0 yzguy      (501) staff       (20)     5141 2023-05-14 05:14:36.000000 octodns-bind-0.0.3/octodns_bind.egg-info/PKG-INFO
+-rw-r--r--   0 yzguy      (501) staff       (20)      273 2023-05-14 05:14:36.000000 octodns-bind-0.0.3/octodns_bind.egg-info/SOURCES.txt
+-rw-r--r--   0 yzguy      (501) staff       (20)        1 2023-05-14 05:14:36.000000 octodns-bind-0.0.3/octodns_bind.egg-info/dependency_links.txt
+-rw-r--r--   0 yzguy      (501) staff       (20)      210 2023-05-14 05:14:36.000000 octodns-bind-0.0.3/octodns_bind.egg-info/requires.txt
+-rw-r--r--   0 yzguy      (501) staff       (20)       13 2023-05-14 05:14:36.000000 octodns-bind-0.0.3/octodns_bind.egg-info/top_level.txt
+-rw-r--r--   0 yzguy      (501) staff       (20)      305 2023-05-14 05:02:35.000000 octodns-bind-0.0.3/pyproject.toml
+-rw-r--r--   0 yzguy      (501) staff       (20)       38 2023-05-14 05:14:36.975732 octodns-bind-0.0.3/setup.cfg
+-rw-r--r--   0 yzguy      (501) staff       (20)     1791 2023-05-14 05:02:35.000000 octodns-bind-0.0.3/setup.py
+drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-05-14 05:14:36.975255 octodns-bind-0.0.3/tests/
+-rw-r--r--   0 yzguy      (501) staff       (20)     9035 2023-05-14 05:02:35.000000 octodns-bind-0.0.3/tests/test_provider_octodns_bind.py
```

### Comparing `octodns-bind-0.0.2/PKG-INFO` & `octodns-bind-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-bind
-Version: 0.0.2
+Version: 0.0.3
 Summary:  RFC compliant (Bind9) provider for octoDNS
 Home-page: https://github.com/octodns/octodns-bind
 Author: Adam Smith
 Author-email: zero1three@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -56,15 +56,15 @@
       # The directory holding the zone files
       # Filenames should match zone name (eg. example.com.)
       # with optional extension specified with file_extension
       directory: ./zonefiles
       # File extension on zone files
       # Appended to zone name to locate file
       # (optional, default None)
-      file_extension: zone
+      file_extension: .zone
       # Should sanity checks of the origin node be done
       # (optional, default true)
       check_origin: false
 ```
 
 #### AxfrSource
 
@@ -141,15 +141,15 @@
 Any server that supports RFC compliant AXFR and RFC 2136 should work here. If
 you have a need for support of other auth mechinism please open an issue.
 
 ### Support Information
 
 #### Records
 
-A, AAAA, CAA, CNAME, LOC, MX, NS, PTR, SPF, SRV, SSHFP, TXT
+A, AAAA, CAA, CNAME, LOC, MX, NS, PTR, SPF, SRV, SSHFP, TLSA, TXT
 
 #### Dynamic
 
 This module does not support dynamic records.
 
 ### Development
```

### Comparing `octodns-bind-0.0.2/README.md` & `octodns-bind-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
       # The directory holding the zone files
       # Filenames should match zone name (eg. example.com.)
       # with optional extension specified with file_extension
       directory: ./zonefiles
       # File extension on zone files
       # Appended to zone name to locate file
       # (optional, default None)
-      file_extension: zone
+      file_extension: .zone
       # Should sanity checks of the origin node be done
       # (optional, default true)
       check_origin: false
 ```
 
 #### AxfrSource
 
@@ -128,15 +128,15 @@
 Any server that supports RFC compliant AXFR and RFC 2136 should work here. If
 you have a need for support of other auth mechinism please open an issue.
 
 ### Support Information
 
 #### Records
 
-A, AAAA, CAA, CNAME, LOC, MX, NS, PTR, SPF, SRV, SSHFP, TXT
+A, AAAA, CAA, CNAME, LOC, MX, NS, PTR, SPF, SRV, SSHFP, TLSA, TXT
 
 #### Dynamic
 
 This module does not support dynamic records.
 
 ### Development
```

### Comparing `octodns-bind-0.0.2/octodns_bind/__init__.py` & `octodns-bind-0.0.3/octodns_bind/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 from logging import getLogger
 from os import listdir
 from os.path import join
 
 import dns.name
 import dns.query
 import dns.rdatatype
+import dns.resolver
 import dns.zone
 from dns import tsigkeyring
 from dns.exception import DNSException
 from dns.update import Update as DnsUpdate
 
 from octodns.provider.base import BaseProvider
 from octodns.record import Create, Record, Rr, Update
 from octodns.source.base import BaseSource
 
-__VERSION__ = '0.0.2'
+__VERSION__ = '0.0.3'
 
 
 class RfcPopulate:
     SUPPORTS_GEO = False
     SUPPORTS_DYNAMIC = False
     SUPPORTS = set(
         (
@@ -33,14 +34,15 @@
             'LOC',
             'MX',
             'NS',
             'PTR',
             'SPF',
             'SRV',
             'SSHFP',
+            'TLSA',
             'TXT',
         )
     )
 
     def populate(self, zone, target=False, lenient=False):
         self.log.debug(
             'populate: name=%s, target=%s, lenient=%s',
@@ -63,16 +65,16 @@
 
 
 class ZoneFileSourceException(Exception):
     pass
 
 
 class ZoneFileSourceNotFound(ZoneFileSourceException):
-    def __init__(self):
-        super().__init__('Zone file not found')
+    def __init__(self, path):
+        super().__init__(f'Zone file not found at {path}')
 
 
 class ZoneFileSourceLoadFailure(ZoneFileSourceException):
     def __init__(self, error):
         super().__init__(str(error))
 
 
@@ -93,35 +95,33 @@
         self.check_origin = check_origin
 
         self._zone_records = {}
 
     def _load_zone_file(self, zone_name):
         zone_filename = f'{zone_name[:-1]}{self.file_extension}'
         zonefiles = listdir(self.directory)
+        path = join(self.directory, zone_filename)
         if zone_filename in zonefiles:
             try:
                 z = dns.zone.from_file(
-                    join(self.directory, zone_filename),
+                    path,
                     zone_name,
                     relativize=False,
                     check_origin=self.check_origin,
                 )
             except DNSException as error:
                 raise ZoneFileSourceLoadFailure(error)
         else:
-            raise ZoneFileSourceNotFound()
+            raise ZoneFileSourceNotFound(path)
 
         return z
 
     def zone_records(self, zone):
         if zone.name not in self._zone_records:
-            try:
-                z = self._load_zone_file(zone.name)
-            except ZoneFileSourceNotFound:
-                return []
+            z = self._load_zone_file(zone.name)
 
             records = []
             for name, ttl, rdata in z.iterate_rdatas():
                 rdtype = dns.rdatatype.to_text(rdata.rdtype)
                 if rdtype in self.SUPPORTS:
                     records.append(
                         Rr(name.to_text(), rdtype, ttl, rdata.to_text())
@@ -158,20 +158,33 @@
             host,
             port,
             key_name,
             key_secret is not None,
             key_algorithm is not None,
         )
         super().__init__(id)
-        self.host = host
-        self.port = port
+        self.host = self._host(host)
+        self.port = int(port)
         self.key_name = key_name
         self.key_secret = key_secret
         self.key_algorithm = key_algorithm
 
+    def _host(self, host):
+        h = host
+        try:
+            # Determine if IPv4/IPv6 address
+            dns.inet.af_for_address(host)
+        except ValueError:
+            try:
+                h = dns.resolver.resolve(host)[0].address
+            except DNSException as err:
+                raise AxfrSourceZoneTransferFailed(err) from None
+
+        return h
+
     def _auth_params(self):
         params = {}
         if self.key_name is not None:
             params['keyring'] = tsigkeyring.from_text(
                 {self.key_name: self.key_secret}
             )
         if self.key_algorithm is not None:
```

### Comparing `octodns-bind-0.0.2/octodns_bind.egg-info/PKG-INFO` & `octodns-bind-0.0.3/octodns_bind.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-bind
-Version: 0.0.2
+Version: 0.0.3
 Summary:  RFC compliant (Bind9) provider for octoDNS
 Home-page: https://github.com/octodns/octodns-bind
 Author: Adam Smith
 Author-email: zero1three@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -56,15 +56,15 @@
       # The directory holding the zone files
       # Filenames should match zone name (eg. example.com.)
       # with optional extension specified with file_extension
       directory: ./zonefiles
       # File extension on zone files
       # Appended to zone name to locate file
       # (optional, default None)
-      file_extension: zone
+      file_extension: .zone
       # Should sanity checks of the origin node be done
       # (optional, default true)
       check_origin: false
 ```
 
 #### AxfrSource
 
@@ -141,15 +141,15 @@
 Any server that supports RFC compliant AXFR and RFC 2136 should work here. If
 you have a need for support of other auth mechinism please open an issue.
 
 ### Support Information
 
 #### Records
 
-A, AAAA, CAA, CNAME, LOC, MX, NS, PTR, SPF, SRV, SSHFP, TXT
+A, AAAA, CAA, CNAME, LOC, MX, NS, PTR, SPF, SRV, SSHFP, TLSA, TXT
 
 #### Dynamic
 
 This module does not support dynamic records.
 
 ### Development
```

### Comparing `octodns-bind-0.0.2/setup.py` & `octodns-bind-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `octodns-bind-0.0.2/tests/test_provider_octodns_bind.py` & `octodns-bind-0.0.3/tests/test_provider_octodns_bind.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 #
 
 from os.path import exists
 from shutil import copyfile
 from unittest import TestCase
 from unittest.mock import patch
 
+import dns.resolver
 import dns.zone
 from dns.exception import DNSException
 
 from octodns.record import Record, Rr, ValidationError
 from octodns.zone import Zone
 
 from octodns_bind import (
     AxfrSource,
     AxfrSourceZoneTransferFailed,
     Rfc2136Provider,
     Rfc2136ProviderUpdateFailed,
     ZoneFileSource,
     ZoneFileSourceLoadFailure,
+    ZoneFileSourceNotFound,
 )
 
 
 class TestAxfrSource(TestCase):
     source = AxfrSource('test', 'localhost')
 
     forward_zonefile = dns.zone.from_file(
@@ -39,15 +41,15 @@
     @patch('dns.zone.from_xfr')
     def test_populate_forward(self, from_xfr_mock):
         got = Zone('unit.tests.', [])
 
         from_xfr_mock.side_effect = [self.forward_zonefile, DNSException]
 
         self.source.populate(got)
-        self.assertEqual(16, len(got.records))
+        self.assertEqual(18, len(got.records))
 
         with self.assertRaises(AxfrSourceZoneTransferFailed) as ctx:
             zone = Zone('unit.tests.', [])
             self.source.populate(zone)
         self.assertEqual(
             'Unable to Perform Zone Transfer',
             str(ctx.exception).split(':', 1)[0],
@@ -62,14 +64,25 @@
         self.source.populate(got)
         self.assertEqual(4, len(got.records))
 
 
 class TestZoneFileSource(TestCase):
     source = ZoneFileSource('test', './tests/zones', file_extension='.tst')
 
+    def test_zonefile_not_found(self):
+        with self.assertRaises(ZoneFileSourceNotFound) as ctx:
+            source = ZoneFileSource('notfound', './tests/zones')
+            notfound = Zone('not.found.', [])
+            source.populate(notfound)
+
+        self.assertEqual(
+            'Zone file not found at ./tests/zones/not.found.',
+            str(ctx.exception),
+        )
+
     def test_zonefiles_with_extension(self):
         source = ZoneFileSource('test', './tests/zones', '.extension')
         # Load zonefiles with a specified file extension
         valid = Zone('ext.unit.tests.', [])
         source.populate(valid)
         self.assertEqual(1, len(valid.records))
 
@@ -89,35 +102,30 @@
                 'skipping default filename testing.'
             )
 
         source = ZoneFileSource('test', './tests/zones')
         # Load zonefiles without a specified file extension
         valid = Zone('unit.tests.', [])
         source.populate(valid)
-        self.assertEqual(16, len(valid.records))
+        self.assertEqual(18, len(valid.records))
 
     def test_populate(self):
         # Valid zone file in directory
         valid = Zone('unit.tests.', [])
         self.source.populate(valid)
-        self.assertEqual(16, len(valid.records))
+        self.assertEqual(18, len(valid.records))
 
         # 2nd populate does not read file again
         again = Zone('unit.tests.', [])
         self.source.populate(again)
-        self.assertEqual(16, len(again.records))
+        self.assertEqual(18, len(again.records))
 
         # bust the cache
         del self.source._zone_records[valid.name]
 
-        # No zone file in directory
-        missing = Zone('missing.zone.', [])
-        self.source.populate(missing)
-        self.assertEqual(0, len(missing.records))
-
         # Zone file is not valid
         with self.assertRaises(ZoneFileSourceLoadFailure) as ctx:
             zone = Zone('invalid.zone.', [])
             self.source.populate(zone)
         self.assertEqual(
             'The DNS zone has no NS RRset at its origin.', str(ctx.exception)
         )
@@ -135,14 +143,35 @@
         # Records are not to RFC, but load anyhow (lenient=True)
         invalid = Zone('invalid.records.', [])
         self.source.populate(invalid, lenient=True)
         self.assertEqual(12, len(invalid.records))
 
 
 class TestRfc2136Provider(TestCase):
+    def test_host_ip(self):
+        provider = Rfc2136Provider('test', '192.0.2.1')
+        self.assertEqual('192.0.2.1', provider.host)
+
+    @patch('dns.resolver.resolve')
+    def test_host_dns(self, resolve_mock):
+        host, ip = 'axfr.unit.tests.', '192.0.2.2'
+
+        # Query success
+        resolve_mock.return_value = dns.rrset.from_text(
+            host, 300, 'IN', 'A', ip
+        )
+        provider = Rfc2136Provider('test', host)
+        self.assertEqual(ip, provider.host)
+
+        # Query failure
+        resolve_mock.reset_mock()
+        resolve_mock.side_effect = DNSException
+        with self.assertRaises(AxfrSourceZoneTransferFailed):
+            provider = Rfc2136Provider('test', host)
+
     def test_auth(self):
         provider = Rfc2136Provider('test', 'localhost')
         self.assertEqual({}, provider._auth_params())
 
         key_secret = 'vZew5TtZLTZKTCl00xliGt+1zzsuLWQWFz48bRbPnZU='
         provider = Rfc2136Provider(
             'test',
```

