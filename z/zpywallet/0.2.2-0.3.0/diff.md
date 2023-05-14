# Comparing `tmp/zpywallet-0.2.2.tar.gz` & `tmp/zpywallet-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpywallet-0.2.2.tar", last modified: Thu Mar 16 11:27:09 2023, max compression
+gzip compressed data, was "zpywallet-0.3.0.tar", last modified: Sun May 14 16:58:21 2023, max compression
```

## Comparing `zpywallet-0.2.2.tar` & `zpywallet-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:27:09.537407 zpywallet-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-16 11:26:54.000000 zpywallet-0.2.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-16 11:26:54.000000 zpywallet-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-16 11:26:54.000000 zpywallet-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-03-16 11:27:09.537407 zpywallet-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-03-16 11:26:54.000000 zpywallet-0.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-16 11:27:09.537407 zpywallet-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-03-16 11:26:54.000000 zpywallet-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:27:09.537407 zpywallet-0.2.2/zpywallet/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-16 11:26:54.000000 zpywallet-0.2.2/zpywallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-16 11:26:54.000000 zpywallet-0.2.2/zpywallet/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-03-16 11:26:54.000000 zpywallet-0.2.2/zpywallet/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:27:09.537407 zpywallet-0.2.2/zpywallet/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-16 11:26:54.000000 zpywallet-0.2.2/zpywallet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29047 2023-03-16 11:26:54.000000 zpywallet-0.2.2/zpywallet/utils/bip32.py
--rw-r--r--   0 runner    (1001) docker     (123)    31084 2023-03-16 11:26:54.000000 zpywallet-0.2.2/zpywallet/utils/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    56740 2023-03-16 11:26:54.000000 zpywallet-0.2.2/zpywallet/utils/ethereum.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-03-16 11:26:54.000000 zpywallet-0.2.2/zpywallet/utils/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-16 11:26:54.000000 zpywallet-0.2.2/zpywallet/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-03-16 11:26:54.000000 zpywallet-0.2.2/zpywallet/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:27:09.537407 zpywallet-0.2.2/zpywallet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-03-16 11:27:09.000000 zpywallet-0.2.2/zpywallet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-16 11:27:09.000000 zpywallet-0.2.2/zpywallet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 11:27:09.000000 zpywallet-0.2.2/zpywallet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-16 11:27:09.000000 zpywallet-0.2.2/zpywallet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 11:27:09.000000 zpywallet-0.2.2/zpywallet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:58:21.690115 zpywallet-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-14 16:58:10.000000 zpywallet-0.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-14 16:58:10.000000 zpywallet-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-14 16:58:10.000000 zpywallet-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-14 16:58:21.690115 zpywallet-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-14 16:58:10.000000 zpywallet-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-14 16:58:21.690115 zpywallet-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-14 16:58:10.000000 zpywallet-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:58:21.686115 zpywallet-0.3.0/zpywallet/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:58:21.690115 zpywallet-0.3.0/zpywallet/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28188 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/utils/bip32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31084 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/utils/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63187 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/utils/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/utils/ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-14 16:58:10.000000 zpywallet-0.3.0/zpywallet/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:58:21.686115 zpywallet-0.3.0/zpywallet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-14 16:58:21.000000 zpywallet-0.3.0/zpywallet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-14 16:58:21.000000 zpywallet-0.3.0/zpywallet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:58:21.000000 zpywallet-0.3.0/zpywallet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-14 16:58:21.000000 zpywallet-0.3.0/zpywallet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 16:58:21.000000 zpywallet-0.3.0/zpywallet.egg-info/top_level.txt
```

### Comparing `zpywallet-0.2.2/LICENSE` & `zpywallet-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zpywallet-0.2.2/PKG-INFO` & `zpywallet-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: zpywallet
-Version: 0.2.2
+Version: 0.3.0
 Summary: Simple BIP32 (HD) wallet creation for BTC, BTX, RVN, MXT, BTG, BCH, LTC, DASH, USDT, QTUM and DOGE
 Home-page: https://github.com/ZenulAbidin/pywallet
 Author: Ali Sherief
 Author-email: ali@notatether.com
 License: MIT License
 Keywords: bitcoin,wallet,litecoin,hd-wallet,dogecoin,dashcoin,bitcore,qtum,ravencoin,martexcoin,address,crypto,python
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 License-File: AUTHORS
 
 
 ZPyWallet
 ===========
```

### Comparing `zpywallet-0.2.2/README.rst` & `zpywallet-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `zpywallet-0.2.2/setup.py` & `zpywallet-0.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,29 +32,35 @@
     long_description=long_description,
     url='https://github.com/ZenulAbidin/pywallet',
     author='Ali Sherief',
     author_email='ali@notatether.com',
     license='MIT License',
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
 
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
 
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     platforms = ['any'],
     keywords='bitcoin, wallet, litecoin, hd-wallet, dogecoin, dashcoin, bitcore, qtum, ravencoin, martexcoin, address, crypto, python',
     packages = find_packages(exclude=['contrib', 'docs', 'tests', 'demo', 'demos', 'examples']),
     package_data={'': ['AUTHORS', 'LICENSE']},
     install_requires=[
         'base58>=0.2.2',
         'ecdsa>=0.11',
         'six>=1.8.0',
         'pycryptodome>=3.6.6',
-        'mnemonic>=0.18'
+        'mnemonic>=0.18',
+        'cachetools>=1.1.1'
     ]
 )
```

### Comparing `zpywallet-0.2.2/zpywallet/network.py` & `zpywallet-0.3.0/zpywallet/network.py`

 * *Files identical despite different names*

### Comparing `zpywallet-0.2.2/zpywallet/utils/bip32.py` & `zpywallet-0.3.0/zpywallet/utils/bip32.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from binascii import hexlify
 from binascii import unhexlify
 from hashlib import sha256
 from hashlib import sha512
 import hmac
+from mnemonic.mnemonic import Mnemonic
 
 import base58
 from os import urandom
 from ecdsa import SECP256k1
 from ecdsa.ecdsa import Public_key as _ECDSA_Public_key
 from ecdsa.ellipticcurve import INFINITY
 import six
 import time
+from cachetools.func import lru_cache
 
 # import all the networks
 from ..network import *
 
 from .keys import incompatible_network_exception_factory
 from .keys import PrivateKey
 from .keys import PublicKey
@@ -22,15 +24,15 @@
 from .utils import chr_py2
 from .utils import ensure_bytes
 from .utils import ensure_str
 from .utils import hash160
 from .utils import is_hex_string
 from .utils import long_or_int
 from .utils import long_to_hex
-from .utils import memoize
+
 
 
 class Wallet(object):
     """A BIP32 wallet is made up of Wallet nodes.
 
     A Private node contains both a public and private key, while a public
     node contains only a public key.
@@ -61,15 +63,15 @@
                  depth=0,
                  parent_fingerprint=0,
                  child_number=0,
                  private_exponent=None,
                  private_key=None,
                  public_pair=None,
                  public_key=None,
-                 network="bitcoin_testnet"):
+                 network="BTC"):
         """Construct a new BIP32 compliant wallet.
 
         You probably don't want to use this init methd. Instead use one
         of the 'from_master_secret' or 'deserialize' cosntructors.
         """
 
         if (not (private_exponent or private_key) and
@@ -77,36 +79,26 @@
             raise InsufficientKeyDataError(
                 "You must supply one of private_exponent or public_pair")
 
         network = Wallet.get_network(network)
         self.private_key = None
         self.public_key = None
         if private_key:
-            if not isinstance(private_key, PrivateKey):
-                raise InvalidPrivateKeyError(
-                    "private_key must be of type "
-                    "bitmerchant.wallet.keys.PrivateKey")
             self.private_key = private_key
         elif private_exponent:
-            self.private_key = PrivateKey(
-                private_exponent, network=network)
+            self.private_key = PrivateKey(private_exponent)
 
         if public_key:
-            if not isinstance(public_key, PublicKey):
-                raise InvalidPublicKeyError(
-                    "public_key must be of type "
-                    "bitmerchant.wallet.keys.PublicKey")
             self.public_key = public_key
         elif public_pair:
-            self.public_key = PublicKey.from_public_pair(
-                public_pair, network=network)
+            self.public_key = PublicKey(public_pair.x, public_pair.y)
         else:
-            self.public_key = self.private_key.get_public_key()
+            self.public_key = self.private_key.public_key
 
-        if (self.private_key and self.private_key.get_public_key() !=
+        if (self.private_key and self.private_key.public_key !=
                 self.public_key):
             raise KeyMismatchError(
                 "Provided private and public values do not match")
 
         def h(val, hex_len):
             if isinstance(val, six.integer_types):
                 return long_to_hex(val, hex_len)
@@ -148,15 +140,15 @@
 
         DO NOT share this private key with anyone.
         """
         return ensure_bytes(self.private_key.get_key())
 
     def get_public_key_hex(self, compressed=True):
         """Get the sec1 representation of the public key."""
-        return ensure_bytes(self.public_key.get_key(compressed))
+        return hexlify(ensure_bytes(self.public_key.get_key(compressed)))
 
     @property
     def identifier(self):
         """Get the identifier for this node.
 
         Extended keys can be identified by the Hash160 (RIPEMD160 after SHA256)
         of the public key's `key`. This corresponds exactly to the data used in
@@ -244,15 +236,15 @@
             except ValueError:
                 raise InvalidPathError("%s is not a valid path" % path)
             child = child.get_child(child_number, is_prime)
         if not as_private:
             return child.public_copy()
         return child
 
-    @memoize
+    @lru_cache(maxsize=1024)
     def get_child(self, child_number, is_prime=None, as_private=True):
         """Derive a child key.
 
         :param child_number: The number of the child key to compute
         :type child_number: int
         :param is_prime: If True, the child is calculated via private
             derivation. If False, then public derivation is used. If None,
@@ -277,26 +269,25 @@
         as a leading 1 in a 32 bit unsigned int.
 
         This derivation is fully described at
         https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki#child-key-derivation-functions  # nopep8
         """
         boundary = 0x80000000
 
+        # Note: If this boundary check gets removed, then children above
+        # the boundary should use private (prime) derivation.
         if abs(child_number) >= boundary:
             raise ValueError("Invalid child number %s" % child_number)
 
         # If is_prime isn't set, then we can infer it from the child_number
         if is_prime is None:
             # Prime children are either < 0 or > 0x80000000
             if child_number < 0:
                 child_number = abs(child_number)
                 is_prime = True
-            elif child_number >= boundary:
-                child_number -= boundary
-                is_prime = True
             else:
                 is_prime = False
         else:
             # Otherwise is_prime is set so the child_number should be between
             # 0 and 0x80000000
             if child_number < 0 or child_number >= boundary:
                 raise ValueError(
@@ -311,24 +302,24 @@
             # Even though we take child_number as an int < boundary, the
             # internal derivation needs it to be the larger number.
             child_number = child_number + boundary
         child_number_hex = long_to_hex(child_number, 8)
 
         if is_prime:
             # Let data = concat(0x00, self.key, child_number)
-            data = b'00' + self.private_key.get_key()
+            data = b'00' + ensure_bytes(self.private_key.to_hex())
         else:
             data = self.get_public_key_hex()
         data += child_number_hex
 
         # Compute a 64 Byte I that is the HMAC-SHA512, using self.chain_code
         # as the seed, and data as the message.
         I = hmac.new(
-            unhexlify(self.chain_code),
-            msg=unhexlify(data),
+            unhexlify(ensure_bytes(self.chain_code)),
+            msg=unhexlify(ensure_bytes(data)),
             digestmod=sha512).digest()
         # Split I into its 32 Byte components.
         I_L, I_R = I[:32], I[32:]
 
         if long_or_int(hexlify(I_L), 16) >= SECP256k1.order:
             raise InvalidPrivateKeyError("The derived key is too large.")
 
@@ -337,15 +328,15 @@
         public_pair = None
         if self.private_key:
             # Use private information for derivation
             # I_L is added to the current key's secret exponent (mod n), where
             # n is the order of the ECDSA curve in use.
             private_exponent = (
                 (long_or_int(hexlify(I_L), 16) +
-                 long_or_int(self.private_key.get_key(), 16))
+                 long_or_int(ensure_bytes(self.private_key.to_hex()), 16))
                 % SECP256k1.order)
             # I_R is the child's chain code
         else:
             # Only use public information for this derivation
             g = SECP256k1.generator
             I_L_long = long_or_int(hexlify(I_L), 16)
             point = (_ECDSA_Public_key(g, g * I_L_long).point +
@@ -357,15 +348,15 @@
             chain_code=c_i,
             depth=self.depth + 1,  # we have to go deeper...
             parent_fingerprint=self.fingerprint,
             child_number=child_number_hex,
             private_exponent=private_exponent,
             public_pair=public_pair,
             network=self.network)
-        if child.public_key.to_point() == INFINITY:
+        if child.public_key.point.infinity:
             raise InfinityPointException("The point at infinity is invalid.")
         if not as_private:
             return child.public_copy()
         return child
 
     def public_copy(self):
         """Clone this wallet and strip it of its private information."""
@@ -424,27 +415,14 @@
             chain_code=self.chain_code,
             depth=self.depth,
             parent_fingerprint=self.parent_fingerprint,
             child_number=self.child_number,
             private_key=parent_private_key,
             network=self.network)
 
-    def export_to_wif(self):
-        """Export a key to WIF.
-
-        See https://en.bitcoin.it/wiki/Wallet_import_format for a full
-        description.
-        """
-        # Add the network byte, creating the "extended key"
-        extended_key_hex = self.private_key.get_extended_key()
-        # BIP32 wallets have a trailing \01 byte
-        extended_key_bytes = unhexlify(extended_key_hex) + b'\01'
-        # And return the base58-encoded result with a checksum
-        return base58.b58encode_check(extended_key_bytes)
-
     def serialize(self, private=True):
         """Serialize this key.
 
         :param private: Whether or not the serialized key should contain
             private information. Set to False for a public-only representation
             that cannot spend funds but can create children. You want
             private=False if you are, for example, running an e-commerce
@@ -467,15 +445,15 @@
         parent_fingerprint = self.parent_fingerprint[2:]  # strip leading 0x
         child_number = long_to_hex(self.child_number, 8)
         chain_code = self.chain_code
         ret = (network_version + depth + parent_fingerprint + child_number +
                chain_code)
         # Private and public serializations are slightly different
         if private:
-            ret += b'00' + self.private_key.get_key()
+            ret += b'00' + ensure_bytes(self.private_key.to_hex())
         else:
             ret += self.get_public_key_hex(compressed=True)
         return ensure_bytes(ret.lower())
 
     def serialize_b58(self, private=True):
         """Encode the serialized node in base58."""
         return ensure_str(
@@ -493,16 +471,16 @@
         hash160_bytes = hash160(key)
         # Prepend the network address byte
         network_hash160_bytes = \
             chr_py2(self.network.PUBKEY_ADDRESS) + hash160_bytes
         # Return a base58 encoded address with a checksum
         return ensure_str(base58.b58encode_check(network_hash160_bytes))
 
-    @classmethod #@memoize
-    def deserialize(cls, key, network="bitcoin_testnet"):
+    @classmethod
+    def deserialize(cls, key, network="BTC"):
         """Load the ExtendedBip32Key from a hex key.
 
         The key consists of
 
             * 4 byte version bytes (network key)
             * 1 byte depth:
                 - 0x00 for master nodes,
@@ -574,34 +552,36 @@
                    child_number=l(child),
                    chain_code=l(chain_code),
                    private_exponent=l(exponent),
                    public_key=pubkey,
                    network=network)
 
     @classmethod
-    def from_master_secret(cls, seed, network="bitcoin_testnet"):
+    def from_master_secret(cls, mnemonic, network="BTC"):
         """Generate a new PrivateKey from a secret key.
 
-        :param seed: The key to use to generate this wallet. It may be a long
+        :param mnemonic: The key to use to generate this wallet. It may be a long
             string. Do not use a phrase from a book or song, as that will
             be guessed and is not secure. My advice is to not supply this
             argument and let me generate a new random key for you.
 
         See https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki#Serialization_format  # nopep8
         """
         network = Wallet.get_network(network)
-        seed = ensure_bytes(seed)
+        m = Mnemonic(language='english')
+        seed = ensure_bytes(m.to_seed(mnemonic))
+        
         # Given a seed S of at least 128 bits, but 256 is advised
         # Calculate I = HMAC-SHA512(key="Bitcoin seed", msg=S)
         I = hmac.new(b"Bitcoin seed", msg=seed, digestmod=sha512).digest()
         # Split I into two 32-byte sequences, IL and IR.
         I_L, I_R = I[:32], I[32:]
         # Use IL as master secret key, and IR as master chain code.
         return cls(private_exponent=long_or_int(hexlify(I_L), 16),
-                   chain_code=long_or_int(hexlify(I_R), 16),
+                   chain_code=hexlify(I_R),
                    network=network)
 
     @classmethod
     def from_master_secret_slow(cls, password, network=BitcoinMainNet):
         """
         Generate a new key from a password using 50,000 rounds of HMAC-SHA256.
```

### Comparing `zpywallet-0.2.2/zpywallet/utils/ecdsa.py` & `zpywallet-0.3.0/zpywallet/utils/ecdsa.py`

 * *Files identical despite different names*

### Comparing `zpywallet-0.2.2/zpywallet/utils/ethereum.py` & `zpywallet-0.3.0/zpywallet/utils/keys.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,52 @@
 import hmac
 from mnemonic.mnemonic import Mnemonic
 import random
 import codecs
 import struct
 import os
 from collections import namedtuple
-from zpywallet.utils.ecdsa import Point
-from zpywallet.utils.ecdsa import ECPointAffine
-from zpywallet.utils.ecdsa import secp256k1
+from .ecdsa import Point
+from .ecdsa import ECPointAffine
+from .ecdsa import secp256k1
+from .ripemd160 import ripemd160
+from .utils import chr_py2
+from .utils import ensure_bytes
+from ..network import BitcoinMainNet
+
+
+
+PublicPair = namedtuple("PublicPair", ["x", "y"])
+
+
+class KeyParseError(Exception):
+    pass
+
+
+def incompatible_network_exception_factory(
+        network_name, expected_prefix, given_prefix):
+    return IncompatibleNetworkException(
+        "Incorrect network. {net_name} expects a byte prefix of "
+        "{expected_prefix}, but you supplied {given_prefix}".format(
+            net_name=network_name,
+            expected_prefix=expected_prefix,
+            given_prefix=given_prefix))
+
+
+class ChecksumException(Exception):
+    pass
+
+
+class IncompatibleNetworkException(Exception):
+    pass
+
+
+class InvalidChildException(Exception):
+    pass
+
 
 bitcoin_curve = secp256k1()
 
 from Crypto.Hash import keccak
 sha3_256 = lambda x: keccak.new(digest_bits=256, data=x)
 
 Point = namedtuple('Point', ['x', 'y'])
@@ -272,26 +307,29 @@
             compressed (bool): Whether or not the compressed key should
                be used.
         Returns:
             bytes: RIPEMD-160 byte string.
         """
         raise NotImplementedError
 
-    def address(self, compressed=True, testnet=False):
+    def address(self, compressed=True, testnet=False, mode='base58'):
         """ Address property that returns the Base58Check
         encoded version of the HASH160.
 
         Args:
             compressed (bool): Whether or not the compressed key should
                be used.
             testnet (bool): Whether or not the key is intended for testnet
                usage. False indicates mainnet usage.
+            mode (bool): Determines what kind of address to create. The
+               default is 'base58', but you can also generate 'bech32'
+               addresses (not implemented) and 'hex' addresses.
 
         Returns:
-            bytes: Base58Check encoded string
+            bytes: Address encoded with Base58Check, hexadecimal, or Bech32 accordingly.
         """
         raise NotImplementedError
 
     def verify(self, message, signature, do_hash=True):
         """ Verifies that message was appropriately signed.
 
         Args:
@@ -416,14 +454,33 @@
         """
         return PrivateKey(random.SystemRandom().randrange(1, bitcoin_curve.n))
 
     def __init__(self, k):
         self.key = k
         self._public_key = None
 
+    @classmethod
+    def from_brainwallet(cls, password, salt="zpywallet"):
+        """Generate a new key from a master password, and an optional salt.
+
+        This password is hashed via a single round of sha256 and is highly
+        breakable, but it's the standard brainwallet approach.
+
+        It is highly recommended to salt a password before hashing it to protect
+        it from rainbow table attacks. You should not need to change it from the
+        default value, though. WARNING: Either remember the salt, and add it after
+        the end of the password, or always use this method to regenerate the
+        brainwallet so you don't lose your private key.
+        """
+        password = ensure_bytes(password) + ensure_bytes(salt)
+        key = sha256(password).hexdigest()
+        return cls(long_or_int(key, 16))
+
+    __hash__ = object.__hash__
+
     @property
     def public_key(self):
         """ Returns the public key associated with this private key.
 
         Returns:
             PublicKey:
                 The PublicKey object that corresponds to this
@@ -532,23 +589,98 @@
 
         sig = self.sign(msg_hash)
         comp_adder = 4 if compressed else 0
         magic = 27 + sig.recovery_id + comp_adder
 
         return base64.b64encode(bytes([magic]) + bytes(sig))
 
+    def export_to_wif(self, compressed=False, network=BitcoinMainNet):
+        """Export a key to WIF.
+
+        :param compressed: False if you want a standard WIF export (the most
+            standard option). True if you want the compressed form (Note that
+            not all clients will accept this form). Defaults to None, which
+            in turn uses the self.compressed attribute.
+        :type compressed: bool
+
+        See https://en.bitcoin.it/wiki/Wallet_import_format for a full
+        description.
+        """
+        # Add the network byte, creating the "extended key"
+        extended_key_hex = self.get_extended_key(network)
+        # BIP32 wallets have a trailing \01 byte
+        extended_key_bytes = binascii.unhexlify(extended_key_hex)
+        if compressed:
+            extended_key_bytes += b'\01'
+        # And return the base58-encoded result with a checksum
+        return base58.b58encode_check(extended_key_bytes)
+
+    @classmethod
+    def from_wif(cls, wif, network=BitcoinMainNet):
+        """Import a key in WIF format.
+
+        WIF is Wallet Import Format. It is a base58 encoded checksummed key.
+        See https://en.bitcoin.it/wiki/Wallet_import_format for a full
+        description.
+
+        This supports compressed WIFs - see this for an explanation:
+        http://bitcoin.stackexchange.com/questions/7299/when-importing-private-keys-will-compressed-or-uncompressed-format-be-used  # nopep8
+        (specifically http://bitcoin.stackexchange.com/a/7958)
+        """
+        # Decode the base58 string and ensure the checksum is valid
+        wif = ensure_str(wif)
+        try:
+            extended_key_bytes = base58.b58decode_check(wif)
+        except ValueError as e:
+            # Invalid checksum!
+            raise ChecksumException(e)
+
+        # Verify we're on the right network
+        network_bytes = extended_key_bytes[0]
+        # py3k interprets network_byte as an int already
+        if not isinstance(network_bytes, six.integer_types):
+            network_bytes = ord(network_bytes)
+        if (network_bytes != network.SECRET_KEY):
+            raise incompatible_network_exception_factory(
+                network_name=network.NAME,
+                expected_prefix=network.SECRET_KEY,
+                given_prefix=network_bytes)
+
+        # Drop the network bytes
+        extended_key_bytes = extended_key_bytes[1:]
+
+        # Check for comprssed public key
+        # This only affects the way in which addresses are generated.
+        compressed = False
+        if len(extended_key_bytes) == 33:
+            # We are supposed to use compressed form!
+            extended_key_bytes = extended_key_bytes[:-1]
+
+        # And we should finally have a valid key
+        return cls(long_or_int(hexlify(extended_key_bytes), 16))
+
     def to_b58check(self, testnet=False):
         """ Generates a Base58Check encoding of this private key.
 
         Returns:
             str: A Base58Check encoded string representing the key.
         """
         version = self.TESTNET_VERSION if testnet else self.MAINNET_VERSION
         return base58.b58encode_check(bytes([version]) + bytes(self))
 
+    def get_extended_key(self, network):
+        """Get the extended key.
+
+        Extended keys contain the network bytes and the public or private
+        key.
+        """
+        network_hex_chars = binascii.hexlify(
+            chr_py2(network.SECRET_KEY))
+        return ensure_bytes(network_hex_chars) + ensure_bytes(self.to_hex())
+
     def __bytes__(self):
         return self.key.to_bytes(32, 'big')
 
     def __int__(self):
         return self.key
 
 
@@ -746,54 +878,74 @@
         p = ECPointAffine(bitcoin_curve, x, y)
         if not bitcoin_curve.is_on_curve(p):
             raise ValueError("The provided (x, y) are not on the secp256k1 curve.")
 
         self.point = p
 
         # RIPEMD-160 of SHA-256
-        r = hashlib.new('ripemd160')
-        r.update(hashlib.sha256(bytes(self)).digest())
-        self.ripe = r.digest()
-
-        r = hashlib.new('ripemd160')
-        r.update(hashlib.sha256(self.compressed_bytes).digest())
-        self.ripe_compressed = r.digest()
+        self.ripe = ripemd160(hashlib.sha256(bytes(self)).digest())
+        self.ripe_compressed = ripemd160(hashlib.sha256(bytes(self.compressed_bytes)).digest())
 
         self.keccak = sha3(bytes(self)[1:])
 
+    def to_compressed_hex(self):
+        """Return the compressed public key in hexadecimal
+        """
+        return binascii.hexlify(self.compressed_bytes).decode()
+
+    
+    def to_public_pair(self):
+        """ Return the public key points as a PublicPair.
+        """
+        return PublicPair(self.point.x, self.point.y)
+
+    def to_point(self):
+        """ Alias for `to_public_pair`.
+        """
+        return self.to_public_pair()
+
     def hash160(self, compressed=True):
         """ Return the RIPEMD-160 hash of the SHA-256 hash of the
         public key.
 
         Args:
             compressed (bool): Whether or not the compressed key should
                be used.
         Returns:
             bytes: RIPEMD-160 byte string.
         """
         return self.ripe_compressed if compressed else self.ripe
 
-    def address(self, compressed=True, testnet=False):
+    def address(self, compressed=True, testnet=False, mode='base58'):
         """ Address property that returns the Base58Check
         encoded version of the HASH160.
 
         Args:
             compressed (bool): Whether or not the compressed key should
                be used.
             testnet (bool): Whether or not the key is intended for testnet
                usage. False indicates mainnet usage.
-
-        Returns:
-            bytes: Base58Check encoded string
-        """
-        version = '0x'
-        return version + binascii.hexlify(self.keccak[12:]).decode('ascii')
-        # Put the version byte in front, 0x00 for Mainnet, 0x6F for testnet
-        # version = bytes([self.TESTNET_VERSION]) if testnet else bytes([self.MAINNET_VERSION])
-        # return base58.b58encode_check(version + self.hash160(compressed))
+            mode (bool): Determines what kind of address to create. The
+               default is 'base58', but you can also generate 'bech32'
+               addresses (not implemented) and 'hex' addresses.
+
+        Returns:
+            bytes: Address encoded with Base58Check, hexadecimal, or Bech32 accordingly.
+        """
+        if mode == 'hex':
+            version = '0x'
+            return version + binascii.hexlify(self.keccak[12:]).decode('ascii')
+        elif mode == 'base58':
+            # Put the version byte in front, 0x00 for Mainnet, 0x6F for testnet
+            version = bytes([self.TESTNET_VERSION]) if testnet else bytes([self.MAINNET_VERSION])
+            return base58.b58encode_check(version + self.hash160(compressed))
+        elif mode == 'bech32':
+            raise NotImplementedError
+        else:
+            raise ValueError("Unknown mode")
 
     def verify(self, message, signature, do_hash=True):
         """ Verifies that message was appropriately signed.
 
         Args:
             message (bytes): The message to be verified.
             signature (Signature): A signature object.
@@ -830,14 +982,28 @@
         of this public key.
 
         Returns:
             b (bytes): A 33-byte long byte string.
         """
         return self.point.compressed_bytes
 
+    def get_key(self, compressed=False):
+        """ Returns the compressed or uncompressed public key in bytes, accordingly.
+
+        Args:
+            compressed (bool): Whether to compress the key
+
+        Returns:
+            b (bytes): a 33-byte of 65-byte long byte string.
+        """
+        if compressed:
+            return self.compressed_bytes
+        else:
+            return bytes(self)
+
 
 class Signature(object):
     """ Encapsulation of a ECDSA signature for Bitcoin purposes.
 
     Args:
         r (Bignum): r component of the signature.
         s (Bignum): s component of the signature.
@@ -1634,28 +1800,31 @@
             the public key.
 
         Returns:
             bytes: RIPEMD-160 byte string.
         """
         return self._key.hash160(True)
 
-    def address(self, compressed=True, testnet=False):
-        """ Address property that returns the Base58Check
-        encoded version of the HASH160.
+    def address(self, compressed=True, testnet=False, mode='base58'):
+        """ Address property that returns the HASH160 as encoded by
+        the mode.
 
         Args:
             compressed (bool): Whether or not the compressed key should
                be used.
             testnet (bool): Whether or not the key is intended for testnet
                usage. False indicates mainnet usage.
+            mode (bool): Determines what kind of address to create. The
+               default is 'base58', but you can also generate 'bech32'
+               addresses (not implemented) and 'hex' addresses.
 
         Returns:
-            bytes: Base58Check encoded string
+            bytes: Address encoded with Base58Check, hexadecimal, or Bech32 accordingly.
         """
-        return self._key.address(True, testnet)
+        return self._key.address(True, testnet, mode)
 
     def verify(self, message, signature, do_hash=True):
         """ Verifies that message was appropriately signed.
 
         Args:
             message (bytes): The message to be verified.
             signature (Signature): A signature object.
```

### Comparing `zpywallet-0.2.2/zpywallet/utils/utils.py` & `zpywallet-0.3.0/zpywallet/utils/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -52,18 +52,7 @@
     f_str = "{0:0%sx}" % size
     return ensure_bytes(f_str.format(l).lower())
 
 
 def long_or_int(val, *args):
     return long(val, *args)
 
-
-def memoize(f):
-    """Memoization decorator for a function taking one or more arguments."""
-    def _c(*args, **kwargs):
-        if not hasattr(f, 'cache'):
-            f.cache = dict()
-        key = (args, tuple(kwargs))
-        if key not in f.cache:
-            f.cache[key] = f(*args, **kwargs)
-        return f.cache[key]
-    return wraps(f)(_c)
```

### Comparing `zpywallet-0.2.2/zpywallet/wallet.py` & `zpywallet-0.3.0/zpywallet/wallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from datetime import datetime
 from .utils import (
     Wallet, HDPrivateKey, HDKey
 )
+from .utils.utils import ensure_bytes, ensure_str
 from .network import *
 import inspect
 
 
 def generate_mnemonic(strength=128):
     _, seed = HDPrivateKey.master_key_from_entropy(strength=strength)
     return seed
@@ -33,15 +34,15 @@
 
         keys = HDKey.from_path(
             acct_pub_key, '{change}/{index}'.format(change=path, index=child))
 
         res = {
             "path": "m/" + str(acct_pub_key.index) + "/" + str(keys[-1].index),
             "bip32_path": "m/44'/60'/0'/" + str(acct_pub_key.index) + "/" + str(keys[-1].index),
-            "address": keys[-1].address()
+            "address": keys[-1].address(mode='hex')
         }
 
         if inspect.stack()[1][3] == "create_wallet":
             res["xpublic_key"] = keys[-1].to_b58check()
 
         return res
 
@@ -127,15 +128,15 @@
         "children": []
     }
 
     if network == 'ethereum' or network.upper() == 'ETH':
         wallet["coin"] = "ETH"
 
         master_key = HDPrivateKey.master_key_from_mnemonic(seed)
-        root_keys = HDKey.from_path(master_key, "m/44'/60'/0'")
+        root_keys = HDKey.from_path(master_key, "m/44'/0'/0'")
 
         acct_priv_key = root_keys[-1]
         acct_pub_key = acct_priv_key.public_key
 
         wallet["private_key"] = acct_priv_key.to_hex()
         wallet["public_key"] = acct_pub_key.to_hex()
         wallet["xprivate_key"] = acct_priv_key.to_b58check()
@@ -158,23 +159,23 @@
                 "xpublic_key": child_wallet["xpublic_key"],
                 "path": "m/" + str(child),
                 "bip32_path": "m/44'/60'/0'/" + str(child),
             })
 
     else:
         my_wallet = Wallet.from_master_secret(
-            network=network.upper(), seed=seed)
+            network=network.upper(), mnemonic=seed)
 
         # account level
-        wallet["private_key"] = my_wallet.private_key.get_key().decode()
-        wallet["public_key"] = my_wallet.public_key.get_key().decode()
+        wallet["private_key"] = my_wallet.private_key.to_hex()
+        wallet["public_key"] = my_wallet.public_key.to_hex()
         wallet["xprivate_key"] = my_wallet.serialize_b58(private=True)
         wallet["xpublic_key"] = my_wallet.serialize_b58(private=False)
         wallet["address"] = my_wallet.to_address()
-        wallet["wif"] = my_wallet.export_to_wif()
+        wallet["wif"] = ensure_str(my_wallet.private_key.export_to_wif())
 
         prime_child_wallet = my_wallet.get_child(0, is_prime=True)
         wallet["xpublic_key_prime"] = prime_child_wallet.serialize_b58(private=False)
 
         # prime children
         for child in range(children):
             child_wallet = my_wallet.get_child(child, is_prime=False, as_private=False)
```

### Comparing `zpywallet-0.2.2/zpywallet.egg-info/PKG-INFO` & `zpywallet-0.3.0/zpywallet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: zpywallet
-Version: 0.2.2
+Version: 0.3.0
 Summary: Simple BIP32 (HD) wallet creation for BTC, BTX, RVN, MXT, BTG, BCH, LTC, DASH, USDT, QTUM and DOGE
 Home-page: https://github.com/ZenulAbidin/pywallet
 Author: Ali Sherief
 Author-email: ali@notatether.com
 License: MIT License
 Keywords: bitcoin,wallet,litecoin,hd-wallet,dogecoin,dashcoin,bitcore,qtum,ravencoin,martexcoin,address,crypto,python
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 License-File: AUTHORS
 
 
 ZPyWallet
 ===========
```

