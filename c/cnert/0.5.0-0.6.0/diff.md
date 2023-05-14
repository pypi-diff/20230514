# Comparing `tmp/cnert-0.5.0.tar.gz` & `tmp/cnert-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnert-0.5.0.tar", max compression
+gzip compressed data, was "cnert-0.6.0.tar", max compression
```

## Comparing `cnert-0.5.0.tar` & `cnert-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.5.0/LICENSE
--rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.5.0/LICENSE.apache2
--rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.5.0/LICENSE.mit
--rw-r--r--   0        0        0     8577 2023-05-10 13:45:50.023695 cnert-0.5.0/README.md
--rw-r--r--   0        0        0     3150 2023-05-10 14:05:49.946732 cnert-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    22623 2023-05-10 14:05:49.980463 cnert-0.5.0/src/cnert/__init__.py
--rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.5.0/src/cnert/py.typed
--rw-r--r--   0        0        0    10341 1970-01-01 00:00:00.000000 cnert-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.6.0/LICENSE
+-rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.6.0/LICENSE.apache2
+-rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.6.0/LICENSE.mit
+-rw-r--r--   0        0        0     7748 2023-05-10 14:30:59.900805 cnert-0.6.0/README.md
+-rw-r--r--   0        0        0     3150 2023-05-14 10:48:27.274639 cnert-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    26063 2023-05-14 10:48:27.305032 cnert-0.6.0/src/cnert/__init__.py
+-rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.6.0/src/cnert/py.typed
+-rw-r--r--   0        0        0     9512 1970-01-01 00:00:00.000000 cnert-0.6.0/PKG-INFO
```

### Comparing `cnert-0.5.0/LICENSE.apache2` & `cnert-0.6.0/LICENSE.apache2`

 * *Files identical despite different names*

### Comparing `cnert-0.5.0/LICENSE.mit` & `cnert-0.6.0/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `cnert-0.5.0/README.md` & `cnert-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,37 +27,14 @@
 TLS certificate and there for can make tailor made certificates for testing
 those apps.
 
 If you don't need that and you just need any "old" certificate, you probably
 better of with [trustme], trust me, or better: trust them.
 
 
-# Cnert - TLS Certificates for testing
-
-Cnert is simple Python API for creating TLS Certificates and stuff for testing
-purposes (on top of [cryptography]).
-
-[cnert.CA][] makes it easy to create CAs, intermediate CAs. These CA objects
-can then issue directly [certificates][cnert._Cert].
-
-Cnert can make CSRs. CA objects also use these to issue certificates.
-
-Subject and Issuer Name Attributes, Subject Alternative Names, not_before_date
-and not_after_data can all be set.
-
-Cnert has different methods to introspect these.
-
-Cnert is made specially made for testing application that *do something* with
-TLS certificate and there for can make tailor made certificates for testing
-those apps.
-
-If you don't need that and you just need any "old" certificate, you probably
-better of with [trustme], trust me, or better: trust them.
-
-
 ## Usage
 
 ### Create a root CA
 
     >>> import cnert
     >>> ca = cnert.CA()
 
@@ -66,14 +43,15 @@
 
     >>> ca.is_intermediate_ca
     False
 
     >>> ca.parent is None
     True
 
+
 ### Issue an intermediate CA
 
     >>> intermediate = ca.issue_intermediate()
     >>> intermediate.is_intermediate_ca
     True
 
     >>> intermediate.is_root_ca
@@ -118,15 +96,14 @@
     >>> ca.cert.public_key.key_size
     2048
 
     >>> ca.cert.pem
     b'-----BEGIN CERTIFICATE-----\nMIIC9zCCAd+gAwIBAgIUGyCBgdyVPVGlYIJj25+x1AMQPHswDQYJKoZIhvcNAQEL\nBQAwEjEQMA4GA1UECgwHUm9vdCBDQTAeFw0yMzA1MDgwODQyNThaFw0yMzA4MDcw\nODQyNThaMBIxEDAOBgNVBAoMB1Jvb3QgQ0EwggEiMA0GCSqGSIb3DQEBAQUAA4IB\nDwAwggEKAoIBAQDK13Q6dZdK17SPmplwTq4Phh7TatM4HQqONEq6+xE2VnJ9eeCh\nQYM5w5dnxIUeV10j3ODPJz5L+6IirV/e6voCWkS6Vgzh/lAVTbUVGANR26NpMnjm\n/qU0NUYuSQo5QFJuwFEx9CZ1xGTac9gspBo1jO7E9m01pRAXlr1HqTZT7mY4LNWb\nDyjKmMa/tfK0+itiKce48hZDxqy3YLnWYyIAZ+rTrf9RW5hpLb6g/KeAf3w5q55Q\nL2dCsC6flZ6NFVRm7okpawwN2tf5c451fMm3B+GtVJJMP+6lmk6MC3h++pcwOimg\nUwB8tYEPoZHuMjd1hacZcbfGFzCGAbme+BZbAgMBAAGjRTBDMB0GA1UdDgQWBBSA\nIsRH6giY94MEfhzafTd5WC2HMzASBgNVHRMBAf8ECDAGAQH/AgEJMA4GA1UdDwEB\n/wQEAwIBpjANBgkqhkiG9w0BAQsFAAOCAQEACLdxWMlmr3drMvA7GaQArzlbe/ny\nx8mThDhZP6gx+yTJ6LXk8CFc7S23JXFZVquwcV5yFa0DavaodBI3RNWknx/Yu5Lm\nM7cOByu2IuJhcEu4o+ZntLZLb7heFMXMIf01lVkYpyYyvS/NvVdu9km8f6ZvxV9r\nDyTDDMjeh+hg5l2Wwc4P6UGoMlmOruUiunsb8hiDLhD+brYBHKHqJY9pCrzJQd0v\nWEkAOsBwaTv/POO0F4VDZSfA5CqjYOkppupw9nXXfJkk9PvKuDI1G2XO7pcW1PWh\nDdGK6Wz0AXMWWbbX8LToDrFA9q7YOxGNOVPhbHZ++bDJvLNmjrtruy3UTQ==\n-----END CERTIFICATE-----\n'
 
 
-
 ###  Inspect the Intermediate CA
 
     >>> intermediate.cert.subject_attrs
     NameAttrs(ORGANIZATION_NAME="CA Intermediate 1")
 
     >>> intermediate.cert.ca.cert.issuer_attrs
     NameAttrs(ORGANIZATION_NAME="Root CA")
@@ -153,15 +130,14 @@
     >>> cert.pem
     b'-----BEGIN CERTIFICATE-----\nMIIDITCCAgmgAwIBAgIUAx6AA8z3BqH/ICCmqOJXGI7PHCswDQYJKoZIhvcNAQEL\nBQAwEjEQMA4GA1UECgwHUm9vdCBDQTAeFw0yMzA1MDgwODU5NTlaFw0yMzA4MDcw\nODU5NTlaMBYxFDASBgNVBAMMC2V4YW1wbGUuY29tMIIBIjANBgkqhkiG9w0BAQEF\nAAOCAQ8AMIIBCgKCAQEAnWAlLvbR0hE8seqI8uBj8ESicJ/nF8I3KF9CFlTexQ73\nKdyqTRCoPZ6uuK0quX+qX5KeeNlWSnJRxSDc0WmLwYxWFVg6hmBDPLK1Ijntc1Uj\n4HENkolgPUBxgf9VBSmojqd1XL0o8PwGFIoyZ6Z/YTc3MqML4QZaB0m+TYlVgoJP\nQgFT9d9nQadvyswIx7nOMkT0Rd3sGl8nWaNgDaBLB6mkylGrtaiyo2M2LWKvNz69\nDWbjlccj65B04cBLwRcA2Zmx80leajX1zNWt0+dhJFo6rnLtmvIgqdLhCrNTmDMK\nrlyVsOrwJfXNreIPDEgYztZlrUdTnynmF4bW6W5KcwIDAQABo2swaTAdBgNVHQ4E\nFgQURd1r0d7XJBtT651AbuR2hg7TQBIwDAYDVR0TAQH/BAIwADAOBgNVHQ8BAf8E\nBAMCBaAwKgYDVR0lAQH/BCAwHgYIKwYBBQUHAwIGCCsGAQUFBwMBBggrBgEFBQcD\nAzANBgkqhkiG9w0BAQsFAAOCAQEANcFmZZkt4Z6jc069IOonGfcpUdnZieSEVyBE\nCQC+QWaHYqcD0ryYV8n1/UzNVcSkptQ5YrbgXNikV6+cuklFq4OjHlUDGOxchrkc\nSFGYAf+j7wAAx+OZWH5IwvMSTWGhfi7FWNFrzbO3JUE1q3OOnsIUmcDpd/8zucyE\njPf6F0MVujwMJq8VAH8UtUpVm1SApEBz9vgx0n7Z0l5fgRw7PMwwDkaoyplSC0VA\n7F7AUX3K0oJ7Gyw+9onfS090GMo6mlTfhtXNpPArleUUOTrp+TKVhwtz8GRRzxEW\nBE1OaNZaipKILZPbgDa5u67pRdU/OhuMFDsBh1GlPopcax+rCQ==\n-----END CERTIFICATE-----\n'
 
     >>> cert.SHA1
     '21B99CE5588417932ACB65C54398115C75240B04'
 
 
-
 ###  Issue a cert from a CA with alt names
 
     >>> cert = ca.issue_cert("www.example.com", "host1.example.com", "example.com")
 
     >>> cert.subject_attrs
     NameAttrs(COMMON_NAME="www.example.com")
 
@@ -188,9 +164,10 @@
 
     >>> csr.subject_attrs.COMMON_NAME
     'example.com'
 
 [cryptography]: https://cryptography.io/en/latest/
 [trustme]: https://github.com/python-trio/trustme
 
+
 [cnert.CA]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnertca
 [cnert._Cert]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnert_cert
```

### Comparing `cnert-0.5.0/pyproject.toml` & `cnert-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cnert"
-version = "0.5.0"
+version = "0.6.0"
 description = "Cnert is trying to be a simple API for creating TLS Certificates testing purposes."
 authors = ["Maarten <ikmaarten@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maartenq/cnert"
 repository = "https://github.com/maartenq/cnert"
 documentation = "https://cnert.readthedocs.io/en/latest/"
```

### Comparing `cnert-0.5.0/src/cnert/__init__.py` & `cnert-0.6.0/src/cnert/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cnert/__init__.py
 
 """
 Cnert makes TLS private keys, CSRs, private CAs and certificates.
 """
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 __title__ = "Cnert"
 __description__ = (
     "Cnert makes TLS private keys, CSRs, private CAs and certificates."
 )
 __uri__ = "https://github.com/maartenq/cnert"
 __author__ = "Maarten"
 __email__ = "ikmaarten@gmail.com"
@@ -29,35 +29,49 @@
 
 
 def build_private_key(
     key_size: int = 2048,
     public_exponent: int = 65537,
 ) -> rsa.RSAPrivateKey:
     """
+    Creates a private key.
+
     Parameters:
         key_size: Key size
         public_exponent: public exponenent
     """
     return rsa.generate_private_key(
         public_exponent=public_exponent,
         key_size=key_size,
         backend=default_backend(),
     )
 
 
 def idna_encode(_string: str) -> str:
+    """
+    Creates a valid  internationalized domain name
+
+    Parameters:
+        _string: Internationalized domain name
+    """
     for prefix in ["*.", "."]:
         if _string.startswith(prefix):
             _string = _string[len(prefix) :]
             _bytes = prefix.encode("ascii") + idna.encode(_string, uts46=True)
             return _bytes.decode("ascii")
     return idna.encode(_string, uts46=True).decode("ascii")
 
 
 def identity_string_to_x509(identity: str) -> x509.GeneralName:
+    """
+    Creates a x509.GeneralName from a string.
+
+    Parameters:
+        identity: IP Address, DNS name or email address.
+    """
     try:
         return x509.IPAddress(ip_address(identity))
     except ValueError:
         try:
             return x509.IPAddress(ip_network(identity))
         except ValueError:
             if "@" in identity:
@@ -233,37 +247,46 @@
         decipher_only: bool = False,
         digital_signature: bool = True,
         encipher_only: bool = False,
         key_agreement: bool = False,
         key_cert_sign: bool = False,
         key_encipherment: bool = True,
     ) -> x509.KeyUsage:
+        """
+        Create X509.KeyUsage objects.
+        """
         return x509.KeyUsage(
             content_commitment=content_commitment,
             crl_sign=crl_sign,
             data_encipherment=data_encipherment,
             decipher_only=decipher_only,
             digital_signature=digital_signature,
             encipher_only=encipher_only,
             key_agreement=key_agreement,
             key_cert_sign=key_cert_sign,
             key_encipherment=key_encipherment,
         )
 
     def _add_ca_extension(self) -> None:
+        """
+        Add CA extension.
+        """
         self.builder = self.builder.add_extension(
             self._key_usage(
                 digital_signature=True,
                 key_cert_sign=True,
                 crl_sign=True,
             ),
             critical=True,
         )
 
     def _add_leaf_cert_extension(self) -> None:
+        """
+        Add leaf extension.
+        """
         self.builder = self.builder.add_extension(
             self._key_usage(),
             critical=True,
         ).add_extension(
             x509.ExtendedKeyUsage(
                 [
                     ExtendedKeyUsageOID.CLIENT_AUTH,
@@ -271,33 +294,72 @@
                     ExtendedKeyUsageOID.CODE_SIGNING,
                 ]
             ),
             critical=True,
         )
 
     def _add_subject_alt_name_extension(self, *sans: str) -> None:
+        """
+        Add Subject Alternative Name extension.
+
+        Parameters:
+            sans: Subject Alternative Names as positional arguments.
+        """
         self.builder = self.builder.add_extension(
             x509.SubjectAlternativeName(
                 [identity_string_to_x509(san) for san in sans]
             ),
             critical=True,
         )
 
+    def _add_authority_key_identifier_extension(
+        self,
+        issuer_public_key: rsa.RSAPublicKey,
+    ) -> None:
+        """
+        Add Authority Key Identifier extension.
+
+        Parameters:
+            issuer_public_key: Issuer Public key
+        """
+        self.builder = self.builder.add_extension(
+            x509.AuthorityKeyIdentifier.from_issuer_public_key(
+                issuer_public_key
+            ),
+            critical=False,
+        )
+
     def build(
         self,
         sans: Union[tuple[()], tuple[str, ...]],
         subject_attrs_X509_name: x509.Name,
         issuer_attrs_X509_name: x509.Name,
         serial_number: int,
         not_valid_before: datetime,
         not_valid_after: datetime,
         is_ca: bool,
-        path_length: Optional[int],
         public_key: rsa.RSAPublicKey,
+        issuer_public_key: Optional[rsa.RSAPublicKey] = None,
+        path_length: Optional[int] = None,
     ) -> None:
+        """
+        Does the Certificate building.
+
+        Parameters:
+            sans: Subject Alternative Names as positional arguments.
+            subject_attrs_X509_name: Subject Attributes Names.
+            issuer_attrs_X509_name: Issuer Atributes Names.
+            serial_number: Serial number.
+            not_valid_before: Not valid before date.
+            not_valid_after: Note valid after date.
+            is_ca: Add CA extension.
+            public_key: Public key for the certificate.
+            issuer_public_key: Issuer public key.
+            path_length: Max path length.
+        """
         self.builder = (
             self.builder.subject_name(subject_attrs_X509_name)
             .issuer_name(issuer_attrs_X509_name)
             .public_key(public_key)
             .serial_number(serial_number)
             .not_valid_before(not_valid_before)
             .not_valid_after(not_valid_after)
@@ -309,14 +371,16 @@
                 x509.BasicConstraints(
                     ca=is_ca,
                     path_length=path_length,
                 ),
                 critical=True,
             )
         )
+        if issuer_public_key is not None:
+            self._add_authority_key_identifier_extension(issuer_public_key)
         if is_ca:
             self._add_ca_extension()
         else:
             self._add_leaf_cert_extension()
         if sans:
             self._add_subject_alt_name_extension(*sans)
 
@@ -358,26 +422,27 @@
         serial_number: Optional[int] = None,
         parent: Optional["_Cert"] = None,
         private_key: Optional[rsa.RSAPrivateKey] = None,
         path_length: int = 0,
         is_ca: bool = False,
     ) -> None:
         """
+        Initialize a _Cert object.
+
         Parameters:
             sans: Subject Alternative Names as positional arguments
             subject_attrs: Subject Name Attributes
             issuer_attrs: Issure Name Attributes
             not_valid_before: CA not valid before date
             not_valid_after: CA not valid after date
             serial_number: Serial number
             parent: Certificate of CA.
             private_key: RSA private key
             path_length: Path length
             is_ca: if CA
-
         """
         if not_valid_before is None:
             not_valid_before = datetime.utcnow()
 
         if not_valid_after is None:
             not_valid_after = not_valid_before + timedelta(weeks=13)
 
@@ -399,38 +464,40 @@
         self.path_length = path_length
         self.is_ca = is_ca
         self._build_certificate()
 
     def _build_certificate(self):
         cert_builder = _CertBuilder()
         cert_builder.build(
-            self.sans,
-            self.subject_attrs.x509_name(),
-            self.issuer_attrs.x509_name(),
-            self.serial_number,
-            self.not_valid_before,
-            self.not_valid_after,
-            self.is_ca,
-            None if not self.is_ca else self.path_length,
-            self.public_key,
+            sans=self.sans,
+            subject_attrs_X509_name=self.subject_attrs.x509_name(),
+            issuer_attrs_X509_name=self.issuer_attrs.x509_name(),
+            serial_number=self.serial_number,
+            not_valid_before=self.not_valid_before,
+            not_valid_after=self.not_valid_after,
+            is_ca=self.is_ca,
+            public_key=self.public_key,
+            issuer_public_key=(
+                self.parent.public_key if self.parent else None
+            ),
+            path_length=None if not self.is_ca else self.path_length,
         )
         self.certificate = cert_builder.sign(
             self.parent.private_key if self.parent else self.private_key,
         )
         self.pem = self.certificate.public_bytes(serialization.Encoding.PEM)
 
     @property
     def private_key_pem_PKCS1(self) -> bytes:
         """
         Examples:
             >>> cert = CA().issue_cert()
             >>> cert.private_key_pem_PKCS1
             b'-----begin rsa private key-----
             ...
-            \n-----end rsa private key-----\n'
 
 
         Returns:
             PEM encoded serialized key in TraditionalOpenSSL format.
         """
         return self.private_key.private_bytes(
             serialization.Encoding.PEM,
@@ -442,16 +509,14 @@
     def private_key_pem_PKCS8(self) -> bytes:
         """
         Examples:
             >>> cert = CA().issue_cert()
             >>> cert.private_key_pem_PKCS8
             b'-----BEGIN PRIVATE KEY-----
             ...
-            \n-----END PRIVATE KEY-----\n'
-
 
         Returns:
             PEM encoded serialized key in PKCS8 format.
         """
         return self.private_key.private_bytes(
             serialization.Encoding.PEM,
             format=serialization.PrivateFormat.PKCS8,
@@ -477,48 +542,86 @@
         """
         Examples:
             >>> cert = cnert.CA().issue_cert()
             >>> cert.MD5
             'A03D37486DD47BE3E9C7EC1624073856'
 
         Returns:
-            MD5 Fingerprint string in upper case.
+            MD5 Fingerprint string in hexadecimal and upper case.
         """
         return bytes.hex(
             self.certificate.fingerprint(hashes.MD5()),  # noqa: S303
         ).upper()
 
     @property
     def SHA1(self) -> str:
         """
         Examples:
             >>> cert = cnert.CA().issue_cert()
             >>> cert.SHA1
             '9E0A06CFB37B352FDA5B2226E6D631CF07D5D185'
 
         Returns:
-            SHA1 Fingerprint string in upper case.
+            SHA1 Fingerprint string in hexadecimal and upper case.
         """
         return bytes.hex(
             self.certificate.fingerprint(hashes.SHA1()),  # noqa: S303
         ).upper()
 
     @property
     def SHA256(self) -> str:
         """
         Examples:
             >>> cert = cnert.CA().issue_cert()
             >>> cert.SHA256
             '68307A6CBE2804038DF85FB53AEE96AB47EA81439AB2E059DDDEA9F901097D84'
 
         Returns:
-            SHA256 Fingerprint string in upper case.
+            SHA256 Fingerprint string in hexadecimal and upper case.
         """
         return bytes.hex(self.certificate.fingerprint(hashes.SHA256())).upper()
 
+    @property
+    def subject_key_identifier_digest(self) -> str:
+        """
+        Examples:
+            >>> cert = cnert.CA().issue_cert()
+            >>> cert.subject_key_identifier_digest
+            '8F85C564F62E39D5A5CA346CA26AAE67029B671E'
+
+        Returns:
+            The binary value of the subject key identifier in hexadecimal
+            and upper case.
+        """
+        ext = self.certificate.extensions.get_extension_for_oid(
+            x509.ExtensionOID.SUBJECT_KEY_IDENTIFIER
+        )
+        return bytes.hex(ext.value.key_identifier).upper()
+
+    @property
+    def authority_key_identifier_digest(self) -> Optional[str]:
+        """
+        Examples:
+            >>> cert = cnert.CA().issue_cert()
+            >>> cert.authority_key_identifier_digest
+            '8F85C564F62E39D5A5CA346CA26AAE67029B671E'
+
+        Returns:
+            The binary value of the authority key identifier in hexadecimal
+            and upper case or None when certificate has no
+            subject key identifier extension.
+        """
+        try:
+            ext = self.certificate.extensions.get_extension_for_oid(
+                x509.ExtensionOID.AUTHORITY_KEY_IDENTIFIER
+            )
+            return bytes.hex(ext.value.key_identifier).upper()
+        except x509.ExtensionNotFound:
+            return None
+
     def __str__(self) -> str:
         return f"Certificate {self.subject_attrs}"
 
 
 class CSR:
     """
     A CSR object.
```

### Comparing `cnert-0.5.0/PKG-INFO` & `cnert-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnert
-Version: 0.5.0
+Version: 0.6.0
 Summary: Cnert is trying to be a simple API for creating TLS Certificates testing purposes.
 Home-page: https://github.com/maartenq/cnert
 License: MIT
 Keywords: certificate,X.509,TLS,cryptography,testing
 Author: Maarten
 Author-email: ikmaarten@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -66,37 +66,14 @@
 TLS certificate and there for can make tailor made certificates for testing
 those apps.
 
 If you don't need that and you just need any "old" certificate, you probably
 better of with [trustme], trust me, or better: trust them.
 
 
-# Cnert - TLS Certificates for testing
-
-Cnert is simple Python API for creating TLS Certificates and stuff for testing
-purposes (on top of [cryptography]).
-
-[cnert.CA][] makes it easy to create CAs, intermediate CAs. These CA objects
-can then issue directly [certificates][cnert._Cert].
-
-Cnert can make CSRs. CA objects also use these to issue certificates.
-
-Subject and Issuer Name Attributes, Subject Alternative Names, not_before_date
-and not_after_data can all be set.
-
-Cnert has different methods to introspect these.
-
-Cnert is made specially made for testing application that *do something* with
-TLS certificate and there for can make tailor made certificates for testing
-those apps.
-
-If you don't need that and you just need any "old" certificate, you probably
-better of with [trustme], trust me, or better: trust them.
-
-
 ## Usage
 
 ### Create a root CA
 
     >>> import cnert
     >>> ca = cnert.CA()
 
@@ -105,14 +82,15 @@
 
     >>> ca.is_intermediate_ca
     False
 
     >>> ca.parent is None
     True
 
+
 ### Issue an intermediate CA
 
     >>> intermediate = ca.issue_intermediate()
     >>> intermediate.is_intermediate_ca
     True
 
     >>> intermediate.is_root_ca
@@ -157,15 +135,14 @@
     >>> ca.cert.public_key.key_size
     2048
 
     >>> ca.cert.pem
     b'-----BEGIN CERTIFICATE-----\nMIIC9zCCAd+gAwIBAgIUGyCBgdyVPVGlYIJj25+x1AMQPHswDQYJKoZIhvcNAQEL\nBQAwEjEQMA4GA1UECgwHUm9vdCBDQTAeFw0yMzA1MDgwODQyNThaFw0yMzA4MDcw\nODQyNThaMBIxEDAOBgNVBAoMB1Jvb3QgQ0EwggEiMA0GCSqGSIb3DQEBAQUAA4IB\nDwAwggEKAoIBAQDK13Q6dZdK17SPmplwTq4Phh7TatM4HQqONEq6+xE2VnJ9eeCh\nQYM5w5dnxIUeV10j3ODPJz5L+6IirV/e6voCWkS6Vgzh/lAVTbUVGANR26NpMnjm\n/qU0NUYuSQo5QFJuwFEx9CZ1xGTac9gspBo1jO7E9m01pRAXlr1HqTZT7mY4LNWb\nDyjKmMa/tfK0+itiKce48hZDxqy3YLnWYyIAZ+rTrf9RW5hpLb6g/KeAf3w5q55Q\nL2dCsC6flZ6NFVRm7okpawwN2tf5c451fMm3B+GtVJJMP+6lmk6MC3h++pcwOimg\nUwB8tYEPoZHuMjd1hacZcbfGFzCGAbme+BZbAgMBAAGjRTBDMB0GA1UdDgQWBBSA\nIsRH6giY94MEfhzafTd5WC2HMzASBgNVHRMBAf8ECDAGAQH/AgEJMA4GA1UdDwEB\n/wQEAwIBpjANBgkqhkiG9w0BAQsFAAOCAQEACLdxWMlmr3drMvA7GaQArzlbe/ny\nx8mThDhZP6gx+yTJ6LXk8CFc7S23JXFZVquwcV5yFa0DavaodBI3RNWknx/Yu5Lm\nM7cOByu2IuJhcEu4o+ZntLZLb7heFMXMIf01lVkYpyYyvS/NvVdu9km8f6ZvxV9r\nDyTDDMjeh+hg5l2Wwc4P6UGoMlmOruUiunsb8hiDLhD+brYBHKHqJY9pCrzJQd0v\nWEkAOsBwaTv/POO0F4VDZSfA5CqjYOkppupw9nXXfJkk9PvKuDI1G2XO7pcW1PWh\nDdGK6Wz0AXMWWbbX8LToDrFA9q7YOxGNOVPhbHZ++bDJvLNmjrtruy3UTQ==\n-----END CERTIFICATE-----\n'
 
 
-
 ###  Inspect the Intermediate CA
 
     >>> intermediate.cert.subject_attrs
     NameAttrs(ORGANIZATION_NAME="CA Intermediate 1")
 
     >>> intermediate.cert.ca.cert.issuer_attrs
     NameAttrs(ORGANIZATION_NAME="Root CA")
@@ -192,15 +169,14 @@
     >>> cert.pem
     b'-----BEGIN CERTIFICATE-----\nMIIDITCCAgmgAwIBAgIUAx6AA8z3BqH/ICCmqOJXGI7PHCswDQYJKoZIhvcNAQEL\nBQAwEjEQMA4GA1UECgwHUm9vdCBDQTAeFw0yMzA1MDgwODU5NTlaFw0yMzA4MDcw\nODU5NTlaMBYxFDASBgNVBAMMC2V4YW1wbGUuY29tMIIBIjANBgkqhkiG9w0BAQEF\nAAOCAQ8AMIIBCgKCAQEAnWAlLvbR0hE8seqI8uBj8ESicJ/nF8I3KF9CFlTexQ73\nKdyqTRCoPZ6uuK0quX+qX5KeeNlWSnJRxSDc0WmLwYxWFVg6hmBDPLK1Ijntc1Uj\n4HENkolgPUBxgf9VBSmojqd1XL0o8PwGFIoyZ6Z/YTc3MqML4QZaB0m+TYlVgoJP\nQgFT9d9nQadvyswIx7nOMkT0Rd3sGl8nWaNgDaBLB6mkylGrtaiyo2M2LWKvNz69\nDWbjlccj65B04cBLwRcA2Zmx80leajX1zNWt0+dhJFo6rnLtmvIgqdLhCrNTmDMK\nrlyVsOrwJfXNreIPDEgYztZlrUdTnynmF4bW6W5KcwIDAQABo2swaTAdBgNVHQ4E\nFgQURd1r0d7XJBtT651AbuR2hg7TQBIwDAYDVR0TAQH/BAIwADAOBgNVHQ8BAf8E\nBAMCBaAwKgYDVR0lAQH/BCAwHgYIKwYBBQUHAwIGCCsGAQUFBwMBBggrBgEFBQcD\nAzANBgkqhkiG9w0BAQsFAAOCAQEANcFmZZkt4Z6jc069IOonGfcpUdnZieSEVyBE\nCQC+QWaHYqcD0ryYV8n1/UzNVcSkptQ5YrbgXNikV6+cuklFq4OjHlUDGOxchrkc\nSFGYAf+j7wAAx+OZWH5IwvMSTWGhfi7FWNFrzbO3JUE1q3OOnsIUmcDpd/8zucyE\njPf6F0MVujwMJq8VAH8UtUpVm1SApEBz9vgx0n7Z0l5fgRw7PMwwDkaoyplSC0VA\n7F7AUX3K0oJ7Gyw+9onfS090GMo6mlTfhtXNpPArleUUOTrp+TKVhwtz8GRRzxEW\nBE1OaNZaipKILZPbgDa5u67pRdU/OhuMFDsBh1GlPopcax+rCQ==\n-----END CERTIFICATE-----\n'
 
     >>> cert.SHA1
     '21B99CE5588417932ACB65C54398115C75240B04'
 
 
-
 ###  Issue a cert from a CA with alt names
 
     >>> cert = ca.issue_cert("www.example.com", "host1.example.com", "example.com")
 
     >>> cert.subject_attrs
     NameAttrs(COMMON_NAME="www.example.com")
 
@@ -227,10 +203,11 @@
 
     >>> csr.subject_attrs.COMMON_NAME
     'example.com'
 
 [cryptography]: https://cryptography.io/en/latest/
 [trustme]: https://github.com/python-trio/trustme
 
+
 [cnert.CA]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnertca
 [cnert._Cert]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnert_cert
```

