# Comparing `tmp/wom_py-0.3.3.tar.gz` & `tmp/wom_py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wom_py-0.3.3.tar", max compression
+gzip compressed data, was "wom_py-0.4.0.tar", max compression
```

## Comparing `wom_py-0.3.3.tar` & `wom_py-0.4.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1074 2023-04-20 02:53:58.701105 wom_py-0.3.3/LICENSE
--rw-r--r--   0        0        0     1942 2023-04-20 02:53:58.701105 wom_py-0.3.3/README.md
--rw-r--r--   0        0        0     2138 2023-04-20 02:53:58.701105 wom_py-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     4295 2023-04-20 02:53:58.781106 wom_py-0.3.3/wom/__init__.py
--rw-r--r--   0        0        0     1324 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/__main__.py
--rw-r--r--   0        0        0     1808 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/_cli.py
--rw-r--r--   0        0        0     8494 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/client.py
--rw-r--r--   0        0        0     1447 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/constants.py
--rw-r--r--   0        0        0     7212 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/enums.py
--rw-r--r--   0        0        0     1729 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/errors.py
--rw-r--r--   0        0        0     3138 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/__init__.py
--rw-r--r--   0        0        0     1555 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/base.py
--rw-r--r--   0        0        0     1673 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/competitions/__init__.py
--rw-r--r--   0        0        0     1591 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/competitions/enums.py
--rw-r--r--   0        0        0     7364 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/competitions/models.py
--rw-r--r--   0        0        0     1289 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/deltas/__init__.py
--rw-r--r--   0        0        0     1824 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/deltas/models.py
--rw-r--r--   0        0        0     1716 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/groups/__init__.py
--rw-r--r--   0        0        0     7780 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/groups/enums.py
--rw-r--r--   0        0        0     9075 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/groups/models.py
--rw-r--r--   0        0        0     1738 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/http.py
--rw-r--r--   0        0        0     1381 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/names/__init__.py
--rw-r--r--   0        0        0     1413 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/names/enums.py
--rw-r--r--   0        0        0     3778 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/names/models.py
--rw-r--r--   0        0        0     1754 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/players/__init__.py
--rw-r--r--   0        0        0     5664 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/players/enums.py
--rw-r--r--   0        0        0    11832 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/players/models.py
--rw-r--r--   0        0        0     1300 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/records/__init__.py
--rw-r--r--   0        0        0     2217 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/models/records/models.py
--rw-r--r--   0        0        0        0 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/py.typed
--rw-r--r--   0        0        0     5561 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/result.py
--rw-r--r--   0        0        0     6539 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/routes.py
--rw-r--r--   0        0        0    33973 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/serializer.py
--rw-r--r--   0        0        0     1709 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/__init__.py
--rw-r--r--   0        0        0     2042 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/base.py
--rw-r--r--   0        0        0    21066 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/competitions.py
--rw-r--r--   0        0        0     3511 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/deltas.py
--rw-r--r--   0        0        0     3671 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/efficiency.py
--rw-r--r--   0        0        0    23928 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/groups.py
--rw-r--r--   0        0        0     5750 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/http.py
--rw-r--r--   0        0        0     4824 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/names.py
--rw-r--r--   0        0        0    17995 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/players.py
--rw-r--r--   0        0        0     3489 2023-04-20 02:53:58.705105 wom_py-0.3.3/wom/services/records.py
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 wom_py-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-13 21:57:03.117573 wom_py-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2712 2023-05-13 21:57:03.117573 wom_py-0.4.0/README.md
+-rw-r--r--   0        0        0     2138 2023-05-13 21:57:03.117573 wom_py-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4385 2023-05-13 21:57:03.221574 wom_py-0.4.0/wom/__init__.py
+-rw-r--r--   0        0        0     1324 2023-05-13 21:57:03.117573 wom_py-0.4.0/wom/__main__.py
+-rw-r--r--   0        0        0     1808 2023-05-13 21:57:03.117573 wom_py-0.4.0/wom/_cli.py
+-rw-r--r--   0        0        0     8648 2023-05-13 21:57:03.117573 wom_py-0.4.0/wom/client.py
+-rw-r--r--   0        0        0     1447 2023-05-13 21:57:03.117573 wom_py-0.4.0/wom/constants.py
+-rw-r--r--   0        0        0     7008 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/enums.py
+-rw-r--r--   0        0        0     1729 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/errors.py
+-rw-r--r--   0        0        0     3228 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/__init__.py
+-rw-r--r--   0        0        0     1557 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/base.py
+-rw-r--r--   0        0        0     1673 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/competitions/__init__.py
+-rw-r--r--   0        0        0     1591 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/competitions/enums.py
+-rw-r--r--   0        0        0     7413 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/competitions/models.py
+-rw-r--r--   0        0        0     1289 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/deltas/__init__.py
+-rw-r--r--   0        0        0     1824 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/deltas/models.py
+-rw-r--r--   0        0        0     1716 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/groups/__init__.py
+-rw-r--r--   0        0        0     7780 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/groups/enums.py
+-rw-r--r--   0        0        0     9139 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/groups/models.py
+-rw-r--r--   0        0        0     1738 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/http.py
+-rw-r--r--   0        0        0     1471 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/names/__init__.py
+-rw-r--r--   0        0        0     1793 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/names/enums.py
+-rw-r--r--   0        0        0     5289 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/names/models.py
+-rw-r--r--   0        0        0     1754 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/players/__init__.py
+-rw-r--r--   0        0        0     5664 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/players/enums.py
+-rw-r--r--   0        0        0    11907 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/players/models.py
+-rw-r--r--   0        0        0     1300 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/records/__init__.py
+-rw-r--r--   0        0        0     2217 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/models/records/models.py
+-rw-r--r--   0        0        0        0 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/py.typed
+-rw-r--r--   0        0        0     5561 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/result.py
+-rw-r--r--   0        0        0     6505 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/routes.py
+-rw-r--r--   0        0        0    34101 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/serializer.py
+-rw-r--r--   0        0        0     1709 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/__init__.py
+-rw-r--r--   0        0        0     2050 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/base.py
+-rw-r--r--   0        0        0    21170 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/competitions.py
+-rw-r--r--   0        0        0     3528 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/deltas.py
+-rw-r--r--   0        0        0     3688 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/efficiency.py
+-rw-r--r--   0        0        0    24099 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/groups.py
+-rw-r--r--   0        0        0     5772 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/http.py
+-rw-r--r--   0        0        0     4031 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/names.py
+-rw-r--r--   0        0        0    18088 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/players.py
+-rw-r--r--   0        0        0     3506 2023-05-13 21:57:03.121573 wom_py-0.4.0/wom/services/records.py
+-rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 wom_py-0.4.0/PKG-INFO
```

### Comparing `wom_py-0.3.3/LICENSE` & `wom_py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/README.md` & `wom_py-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,122 +1,170 @@
-00000000: 2320 776f 6d2e 7079 0a0a 416e 2061 7379  # wom.py..An asy
-00000010: 6e63 6872 6f6e 6f75 7320 7772 6170 7065  nchronous wrappe
-00000020: 7220 666f 7220 7468 6520 5b57 6973 6520  r for the [Wise 
-00000030: 4f6c 6420 4d61 6e20 4150 495d 2868 7474  Old Man API](htt
-00000040: 7073 3a2f 2f64 6f63 732e 7769 7365 6f6c  ps://docs.wiseol
-00000050: 646d 616e 2e6e 6574 2f29 2e0a 0a54 6865  dman.net/)...The
-00000060: 206c 6962 7261 7279 2061 696d 7320 746f   library aims to
-00000070: 206d 616b 6520 6974 2065 6173 7920 746f   make it easy to
-00000080: 2069 6e74 6572 6163 7420 7769 7468 2074   interact with t
-00000090: 6865 2057 6973 6520 4f6c 6420 4d61 6e20  he Wise Old Man 
-000000a0: 4150 4920 6279 0a70 726f 7669 6469 6e67  API by.providing
-000000b0: 2073 6572 7669 6365 206d 6574 686f 6473   service methods
-000000c0: 2066 6f72 2061 6c6c 2061 7661 696c 6162   for all availab
-000000d0: 6c65 2065 6e64 706f 696e 7473 2061 6e64  le endpoints and
-000000e0: 206d 6f64 656c 2063 6c61 7373 6573 0a66   model classes.f
-000000f0: 6f72 2064 6174 6120 636f 6e73 6973 7465  or data consiste
-00000100: 6e63 792e 0a0a 5079 7468 6f6e 2076 6572  ncy...Python ver
-00000110: 7369 6f6e 2033 2e38 206f 7220 6772 6561  sion 3.8 or grea
-00000120: 7465 7220 6973 2072 6571 7569 7265 6420  ter is required 
-00000130: 746f 2075 7365 2077 6f6d 2e70 792e 0a0a  to use wom.py...
-00000140: 2323 2044 6973 636c 6169 6d65 720a 0a54  ## Disclaimer..T
-00000150: 6865 206c 6962 7261 7279 2069 7320 7374  he library is st
-00000160: 696c 6c20 696e 2042 6574 612c 2061 6e64  ill in Beta, and
-00000170: 2061 7320 7375 6368 2066 6561 7475 7265   as such feature
-00000180: 7320 6f72 2070 7562 6c69 6320 696e 7465  s or public inte
-00000190: 7266 6163 6573 0a6d 6179 2063 6861 6e67  rfaces.may chang
-000001a0: 6520 6174 2061 6e79 2074 696d 652e 2054  e at any time. T
-000001b0: 6861 6e6b 7320 666f 7220 6368 6563 6b69  hanks for checki
-000001c0: 6e67 206f 7574 2074 6865 2070 726f 6a65  ng out the proje
-000001d0: 6374 210a 0a23 2320 446f 6375 6d65 6e74  ct!..## Document
-000001e0: 6174 696f 6e0a 0a2d 205b 5374 6162 6c65  ation..- [Stable
-000001f0: 5d28 6874 7470 733a 2f2f 6a6f 6e78 736c  ](https://jonxsl
-00000200: 6179 732e 6769 7468 7562 2e69 6f2f 776f  ays.github.io/wo
-00000210: 6d2e 7079 2f29 0a2d 205b 4465 7665 6c6f  m.py/).- [Develo
-00000220: 706d 656e 745d 2868 7474 7073 3a2f 2f6a  pment](https://j
-00000230: 6f6e 7873 6c61 7973 2e67 6974 6875 622e  onxslays.github.
-00000240: 696f 2f77 6f6d 2e70 792f 6465 762f 290a  io/wom.py/dev/).
-00000250: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-00000260: 0a0a 2323 2320 5374 6162 6c65 0a0a 6060  ..### Stable..``
-00000270: 6073 680a 7069 7020 696e 7374 616c 6c20  `sh.pip install 
-00000280: 2d55 2077 6f6d 2e70 790a 6060 600a 0a23  -U wom.py.```..#
-00000290: 2323 2044 6576 656c 6f70 6d65 6e74 0a0a  ## Development..
-000002a0: 6060 6073 680a 7069 7020 696e 7374 616c  ```sh.pip instal
-000002b0: 6c20 2d55 2067 6974 2b68 7474 7073 3a2f  l -U git+https:/
-000002c0: 2f67 6974 6875 622e 636f 6d2f 4a6f 6e78  /github.com/Jonx
-000002d0: 736c 6179 732f 776f 6d2e 7079 0a60 6060  slays/wom.py.```
-000002e0: 0a0a 466f 7220 6d6f 7265 2069 6e66 6f72  ..For more infor
-000002f0: 6d61 7469 6f6e 206f 6e20 7573 696e 6720  mation on using 
-00000300: 6070 6970 602c 2063 6865 636b 206f 7574  `pip`, check out
-00000310: 2074 6865 205b 7069 7020 646f 6375 6d65   the [pip docume
-00000320: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-00000330: 2f70 6970 2e70 7970 612e 696f 2f65 6e2f  /pip.pypa.io/en/
-00000340: 7374 6162 6c65 2f29 2e0a 0a23 2320 5072  stable/)...## Pr
-00000350: 6f62 6c65 6d73 0a0a 4966 2079 6f75 2772  oblems..If you'r
-00000360: 6520 6578 7065 7269 656e 6369 6e67 2061  e experiencing a
-00000370: 2070 726f 626c 656d 2077 6974 6820 7468   problem with th
-00000380: 6520 6c69 6272 6172 792c 2070 6c65 6173  e library, pleas
-00000390: 6520 6f70 656e 2061 6e20 6973 7375 650a  e open an issue.
-000003a0: 5b68 6572 655d 2868 7474 7073 3a2f 2f67  [here](https://g
-000003b0: 6974 6875 622e 636f 6d2f 4a6f 6e78 736c  ithub.com/Jonxsl
-000003c0: 6179 732f 776f 6d2e 7079 2f69 7373 7565  ays/wom.py/issue
-000003d0: 7329 2c20 6166 7465 7220 6669 7273 7420  s), after first 
-000003e0: 636f 6e66 6972 6d69 6e67 0a61 2073 696d  confirming.a sim
-000003f0: 696c 6172 2069 7373 7565 2077 6173 206e  ilar issue was n
-00000400: 6f74 2061 6c72 6561 6479 2063 7265 6174  ot already creat
-00000410: 6564 2e0a 0a23 2320 5768 6174 2069 7320  ed...## What is 
-00000420: 5769 7365 204f 6c64 204d 616e 0a0a 5769  Wise Old Man..Wi
-00000430: 7365 204f 6c64 204d 616e 2069 7320 616e  se Old Man is an
-00000440: 206f 7065 6e20 736f 7572 6365 204f 6c64   open source Old
-00000450: 7363 686f 6f6c 2052 756e 6573 6361 7065  school Runescape
-00000460: 2070 6c61 7965 7220 7072 6f67 7265 7373   player progress
-00000470: 2074 7261 636b 6572 2e0a 0a49 6620 796f   tracker...If yo
-00000480: 7527 7265 2069 6e74 6572 6573 7465 6420  u're interested 
-00000490: 696e 206c 6561 726e 696e 6720 6d6f 7265  in learning more
-000004a0: 2061 626f 7574 2074 6865 2057 6973 6520   about the Wise 
-000004b0: 4f6c 6420 4d61 6e20 7072 6f6a 6563 742c  Old Man project,
-000004c0: 2063 6f6e 7369 6465 7220 6368 6563 6b69   consider checki
-000004d0: 6e67 206f 7574 2061 6e79 206f 6620 7468  ng out any of th
-000004e0: 6573 6520 6c69 6e6b 733a 0a0a 2d20 5b57  ese links:..- [W
-000004f0: 6562 7369 7465 5d28 6874 7470 733a 2f2f  ebsite](https://
-00000500: 7769 7365 6f6c 646d 616e 2e6e 6574 2f29  wiseoldman.net/)
-00000510: 0a2d 205b 4150 4920 646f 6375 6d65 6e74  .- [API document
-00000520: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
-00000530: 6f63 732e 7769 7365 6f6c 646d 616e 2e6e  ocs.wiseoldman.n
-00000540: 6574 2f29 0a2d 205b 4769 7468 7562 2072  et/).- [Github r
-00000550: 6570 6f73 6974 6f72 795d 2868 7474 7073  epository](https
-00000560: 3a2f 2f77 6973 656f 6c64 6d61 6e2e 6e65  ://wiseoldman.ne
-00000570: 742f 6769 7468 7562 290a 2d20 5b44 6973  t/github).- [Dis
-00000580: 636f 7264 2063 6f6d 6d75 6e69 7479 5d28  cord community](
-00000590: 6874 7470 733a 2f2f 7769 7365 6f6c 646d  https://wiseoldm
-000005a0: 616e 2e6e 6574 2f64 6973 636f 7264 290a  an.net/discord).
-000005b0: 2d20 5b53 7570 706f 7274 2074 6865 2064  - [Support the d
-000005c0: 6576 656c 6f70 6572 7320 6f6e 2050 6174  evelopers on Pat
-000005d0: 7265 6f6e 5d28 6874 7470 733a 2f2f 7769  reon](https://wi
-000005e0: 7365 6f6c 646d 616e 2e6e 6574 2f70 6174  seoldman.net/pat
-000005f0: 7265 6f6e 290a 0a53 6f6d 6520 6f66 2074  reon)..Some of t
-00000600: 6865 2070 6f70 756c 6172 2066 6561 7475  he popular featu
-00000610: 7265 7320 696e 636c 7564 653a 0a0a 2d20  res include:..- 
-00000620: 4578 7065 7269 656e 6365 2074 7261 636b  Experience track
-00000630: 696e 670a 2d20 426f 7373 206b 696c 6c63  ing.- Boss killc
-00000640: 6f75 6e74 730a 2d20 506c 6179 6572 2061  ounts.- Player a
-00000650: 6368 6965 7665 6d65 6e74 730a 2d20 4772  chievements.- Gr
-00000660: 6f75 7020 636f 6d70 6574 6974 696f 6e73  oup competitions
-00000670: 0a2d 2047 6c6f 6261 6c20 6c65 6164 6572  .- Global leader
-00000680: 626f 6172 6473 0a2d 2041 2064 6973 636f  boards.- A disco
-00000690: 7264 2062 6f74 2066 6f72 2069 6e74 6572  rd bot for inter
-000006a0: 6163 7469 6e67 2077 6974 6820 7468 6520  acting with the 
-000006b0: 4150 490a 0a23 2320 436f 6e74 7269 6275  API..## Contribu
-000006c0: 7469 6e67 0a0a 776f 6d2e 7079 2069 7320  ting..wom.py is 
-000006d0: 6f70 656e 2074 6f20 636f 6e74 7269 6275  open to contribu
-000006e0: 7469 6f6e 732e 0a0a 436f 6d65 2062 6163  tions...Come bac
-000006f0: 6b20 736f 6f6e e284 a220 6f6e 6365 2049  k soon... once I
-00000700: 2776 6520 7772 6974 7465 6e20 7468 6520  've written the 
-00000710: 636f 6e74 7269 6275 7469 6e67 2067 7569  contributing gui
-00000720: 6465 2e0a 0a23 2320 4c69 6365 6e73 650a  de...## License.
-00000730: 0a77 6f6d 2e70 7920 6973 206c 6963 656e  .wom.py is licen
-00000740: 7365 6420 756e 6465 7220 7468 650a 5b4d  sed under the.[M
-00000750: 4954 204c 6963 656e 7365 5d28 6874 7470  IT License](http
-00000760: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4a  s://github.com/J
-00000770: 6f6e 7873 6c61 7973 2f77 6f6d 2e70 792f  onxslays/wom.py/
-00000780: 626c 6f62 2f6d 6173 7465 722f 4c49 4345  blob/master/LICE
-00000790: 4e53 4529 2e0a                           NSE)..
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0a20 2020 203c 6831 3e77 6f6d  er">.    <h1>wom
+00000020: 2e70 793c 2f68 313e 0a20 2020 203c 6120  .py</h1>.    <a 
+00000030: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000040: 7069 2e6f 7267 2f70 726f 6a65 6374 2f77  pi.org/project/w
+00000050: 6f6d 2e70 7922 3e3c 696d 6720 6865 6967  om.py"><img heig
+00000060: 6874 3d22 3230 2220 616c 743d 2253 7461  ht="20" alt="Sta
+00000070: 626c 6520 7665 7273 696f 6e22 2073 7263  ble version" src
+00000080: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000090: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+000000a0: 776f 6d2e 7079 3f6c 6162 656c 3d73 7461  wom.py?label=sta
+000000b0: 626c 6526 6c6f 676f 3d70 7970 6922 3e3c  ble&logo=pypi"><
+000000c0: 2f61 3e0a 2020 2020 3c61 2068 7265 663d  /a>.    <a href=
+000000d0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000000e0: 636f 6d2f 4a6f 6e78 736c 6179 732f 776f  com/Jonxslays/wo
+000000f0: 6d2e 7079 2f62 6c6f 622f 6d61 7374 6572  m.py/blob/master
+00000100: 2f4c 4943 454e 5345 223e 3c69 6d67 2068  /LICENSE"><img h
+00000110: 6569 6768 743d 2232 3022 2061 6c74 3d22  eight="20" alt="
+00000120: 4c69 6365 6e73 6522 2073 7263 3d22 6874  License" src="ht
+00000130: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000140: 732e 696f 2f70 7970 692f 6c2f 776f 6d2d  s.io/pypi/l/wom-
+00000150: 7079 3f6c 6162 656c 3d6c 6963 656e 7365  py?label=license
+00000160: 223e 3c2f 613e 0a20 2020 203c 6120 6872  "></a>.    <a hr
+00000170: 6566 3d22 6874 7470 733a 2f2f 7079 7468  ef="https://pyth
+00000180: 6f6e 2e6f 7267 223e 3c69 6d67 2068 6569  on.org"><img hei
+00000190: 6768 743d 2232 3022 2061 6c74 3d22 5079  ght="20" alt="Py
+000001a0: 7468 6f6e 2076 6572 7369 6f6e 7322 2073  thon versions" s
+000001b0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000001c0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+000001d0: 7079 7665 7273 696f 6e73 2f77 6f6d 2d70  pyversions/wom-p
+000001e0: 793f 6c61 6265 6c3d 7079 7468 6f6e 266c  y?label=python&l
+000001f0: 6f67 6f3d 7079 7468 6f6e 223e 3c2f 613e  ogo=python"></a>
+00000200: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000210: 7470 733a 2f2f 636f 6465 636c 696d 6174  tps://codeclimat
+00000220: 652e 636f 6d2f 6769 7468 7562 2f4a 6f6e  e.com/github/Jon
+00000230: 7873 6c61 7973 2f77 6f6d 2e70 792f 6d61  xslays/wom.py/ma
+00000240: 696e 7461 696e 6162 696c 6974 7922 3e3c  intainability"><
+00000250: 696d 6720 6865 6967 6874 3d22 3230 2220  img height="20" 
+00000260: 616c 743d 224d 6169 6e74 6169 6e61 6269  alt="Maintainabi
+00000270: 6c69 7479 2220 7372 633d 2268 7474 7073  lity" src="https
+00000280: 3a2f 2f61 7069 2e63 6f64 6563 6c69 6d61  ://api.codeclima
+00000290: 7465 2e63 6f6d 2f76 312f 6261 6467 6573  te.com/v1/badges
+000002a0: 2f33 3637 6662 3636 3765 6633 3732 3036  /367fb667ef37206
+000002b0: 3466 6535 612f 6d61 696e 7461 696e 6162  4fe5a/maintainab
+000002c0: 696c 6974 7922 202f 3e3c 2f61 3e0a 2020  ility" /></a>.  
+000002d0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000002e0: 3a2f 2f63 6f64 6563 6c69 6d61 7465 2e63  ://codeclimate.c
+000002f0: 6f6d 2f67 6974 6875 622f 4a6f 6e78 736c  om/github/Jonxsl
+00000300: 6179 732f 776f 6d2e 7079 2f74 6573 745f  ays/wom.py/test_
+00000310: 636f 7665 7261 6765 223e 3c69 6d67 2068  coverage"><img h
+00000320: 6569 6768 743d 2232 3022 2061 6c74 3d22  eight="20" alt="
+00000330: 436f 7665 7261 6765 2220 7372 633d 2268  Coverage" src="h
+00000340: 7474 7073 3a2f 2f61 7069 2e63 6f64 6563  ttps://api.codec
+00000350: 6c69 6d61 7465 2e63 6f6d 2f76 312f 6261  limate.com/v1/ba
+00000360: 6467 6573 2f33 3637 6662 3636 3765 6633  dges/367fb667ef3
+00000370: 3732 3036 3466 6535 612f 7465 7374 5f63  72064fe5a/test_c
+00000380: 6f76 6572 6167 6522 202f 3e3c 2f61 3e0a  overage" /></a>.
+00000390: 3c2f 6469 763e 0a0a 416e 2061 7379 6e63  </div>..An async
+000003a0: 6872 6f6e 6f75 7320 7772 6170 7065 7220  hronous wrapper 
+000003b0: 666f 7220 7468 6520 5b57 6973 6520 4f6c  for the [Wise Ol
+000003c0: 6420 4d61 6e20 4150 495d 2868 7474 7073  d Man API](https
+000003d0: 3a2f 2f64 6f63 732e 7769 7365 6f6c 646d  ://docs.wiseoldm
+000003e0: 616e 2e6e 6574 2f29 2e0a 0a54 6865 206c  an.net/)...The l
+000003f0: 6962 7261 7279 2061 696d 7320 746f 206d  ibrary aims to m
+00000400: 616b 6520 6974 2065 6173 7920 746f 2069  ake it easy to i
+00000410: 6e74 6572 6163 7420 7769 7468 2074 6865  nteract with the
+00000420: 2057 6973 6520 4f6c 6420 4d61 6e20 4150   Wise Old Man AP
+00000430: 4920 6279 0a70 726f 7669 6469 6e67 2073  I by.providing s
+00000440: 6572 7669 6365 206d 6574 686f 6473 206d  ervice methods m
+00000450: 6174 6368 696e 6720 616c 6c20 6176 6169  atching all avai
+00000460: 6c61 626c 6520 656e 6470 6f69 6e74 7320  lable endpoints 
+00000470: 616e 6420 6d6f 6465 6c20 636c 6173 7365  and model classe
+00000480: 730a 666f 7220 6461 7461 2063 6f6e 7369  s.for data consi
+00000490: 7374 656e 6379 2e0a 0a23 2320 446f 6375  stency...## Docu
+000004a0: 6d65 6e74 6174 696f 6e0a 0a2d 205b 5374  mentation..- [St
+000004b0: 6162 6c65 5d28 6874 7470 733a 2f2f 6a6f  able](https://jo
+000004c0: 6e78 736c 6179 732e 6769 7468 7562 2e69  nxslays.github.i
+000004d0: 6f2f 776f 6d2e 7079 2f29 0a2d 205b 4465  o/wom.py/).- [De
+000004e0: 7665 6c6f 706d 656e 745d 2868 7474 7073  velopment](https
+000004f0: 3a2f 2f6a 6f6e 7873 6c61 7973 2e67 6974  ://jonxslays.git
+00000500: 6875 622e 696f 2f77 6f6d 2e70 792f 6465  hub.io/wom.py/de
+00000510: 762f 290a 0a23 2320 496e 7374 616c 6c61  v/)..## Installa
+00000520: 7469 6f6e 0a0a 2a2a 5079 7468 6f6e 2076  tion..**Python v
+00000530: 6572 7369 6f6e 2033 2e38 206f 7220 6772  ersion 3.8 or gr
+00000540: 6561 7465 7220 6973 2072 6571 7569 7265  eater is require
+00000550: 6420 746f 2075 7365 2077 6f6d 2e70 792e  d to use wom.py.
+00000560: 2a2a 0a0a 2323 2320 5374 6162 6c65 0a0a  **..### Stable..
+00000570: 6060 6073 680a 7069 7020 696e 7374 616c  ```sh.pip instal
+00000580: 6c20 2d55 2077 6f6d 2e70 790a 6060 600a  l -U wom.py.```.
+00000590: 0a23 2323 2044 6576 656c 6f70 6d65 6e74  .### Development
+000005a0: 0a0a 6060 6073 680a 7069 7020 696e 7374  ..```sh.pip inst
+000005b0: 616c 6c20 2d55 2067 6974 2b68 7474 7073  all -U git+https
+000005c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a6f  ://github.com/Jo
+000005d0: 6e78 736c 6179 732f 776f 6d2e 7079 0a60  nxslays/wom.py.`
+000005e0: 6060 0a0a 466f 7220 6d6f 7265 2069 6e66  ``..For more inf
+000005f0: 6f72 6d61 7469 6f6e 206f 6e20 7573 696e  ormation on usin
+00000600: 6720 6070 6970 602c 2063 6865 636b 206f  g `pip`, check o
+00000610: 7574 2074 6865 205b 7069 7020 646f 6375  ut the [pip docu
+00000620: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+00000630: 3a2f 2f70 6970 2e70 7970 612e 696f 2f65  ://pip.pypa.io/e
+00000640: 6e2f 7374 6162 6c65 2f29 2e0a 0a23 2320  n/stable/)...## 
+00000650: 5072 6f62 6c65 6d73 0a0a 4966 2079 6f75  Problems..If you
+00000660: 2772 6520 6578 7065 7269 656e 6369 6e67  're experiencing
+00000670: 2061 2070 726f 626c 656d 2077 6974 6820   a problem with 
+00000680: 7468 6520 6c69 6272 6172 792c 2070 6c65  the library, ple
+00000690: 6173 6520 6f70 656e 2061 6e20 6973 7375  ase open an issu
+000006a0: 650a 5b68 6572 655d 2868 7474 7073 3a2f  e.[here](https:/
+000006b0: 2f67 6974 6875 622e 636f 6d2f 4a6f 6e78  /github.com/Jonx
+000006c0: 736c 6179 732f 776f 6d2e 7079 2f69 7373  slays/wom.py/iss
+000006d0: 7565 7329 2c20 6166 7465 7220 6669 7273  ues), after firs
+000006e0: 7420 636f 6e66 6972 6d69 6e67 0a61 2073  t confirming.a s
+000006f0: 696d 696c 6172 2069 7373 7565 2077 6173  imilar issue was
+00000700: 206e 6f74 2061 6c72 6561 6479 2063 7265   not already cre
+00000710: 6174 6564 2e0a 0a23 2320 5768 6174 2069  ated...## What i
+00000720: 7320 5769 7365 204f 6c64 204d 616e 0a0a  s Wise Old Man..
+00000730: 5769 7365 204f 6c64 204d 616e 2069 7320  Wise Old Man is 
+00000740: 616e 206f 7065 6e20 736f 7572 6365 204f  an open source O
+00000750: 6c64 7363 686f 6f6c 2052 756e 6573 6361  ldschool Runesca
+00000760: 7065 2070 6c61 7965 7220 7072 6f67 7265  pe player progre
+00000770: 7373 2074 7261 636b 6572 2e0a 0a49 6620  ss tracker...If 
+00000780: 796f 7527 7265 2069 6e74 6572 6573 7465  you're intereste
+00000790: 6420 696e 206c 6561 726e 696e 6720 6d6f  d in learning mo
+000007a0: 7265 2061 626f 7574 2074 6865 2057 6973  re about the Wis
+000007b0: 6520 4f6c 6420 4d61 6e20 7072 6f6a 6563  e Old Man projec
+000007c0: 742c 2063 6f6e 7369 6465 7220 6368 6563  t, consider chec
+000007d0: 6b69 6e67 206f 7574 2061 6e79 206f 6620  king out any of 
+000007e0: 7468 6573 6520 6c69 6e6b 733a 0a0a 2d20  these links:..- 
+000007f0: 5b57 6562 7369 7465 5d28 6874 7470 733a  [Website](https:
+00000800: 2f2f 7769 7365 6f6c 646d 616e 2e6e 6574  //wiseoldman.net
+00000810: 2f29 0a2d 205b 4150 4920 646f 6375 6d65  /).- [API docume
+00000820: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
+00000830: 2f64 6f63 732e 7769 7365 6f6c 646d 616e  /docs.wiseoldman
+00000840: 2e6e 6574 2f29 0a2d 205b 4769 7468 7562  .net/).- [Github
+00000850: 2072 6570 6f73 6974 6f72 795d 2868 7474   repository](htt
+00000860: 7073 3a2f 2f77 6973 656f 6c64 6d61 6e2e  ps://wiseoldman.
+00000870: 6e65 742f 6769 7468 7562 290a 2d20 5b44  net/github).- [D
+00000880: 6973 636f 7264 2063 6f6d 6d75 6e69 7479  iscord community
+00000890: 5d28 6874 7470 733a 2f2f 7769 7365 6f6c  ](https://wiseol
+000008a0: 646d 616e 2e6e 6574 2f64 6973 636f 7264  dman.net/discord
+000008b0: 290a 2d20 5b53 7570 706f 7274 2074 6865  ).- [Support the
+000008c0: 2064 6576 656c 6f70 6572 7320 6f6e 2050   developers on P
+000008d0: 6174 7265 6f6e 5d28 6874 7470 733a 2f2f  atreon](https://
+000008e0: 7769 7365 6f6c 646d 616e 2e6e 6574 2f70  wiseoldman.net/p
+000008f0: 6174 7265 6f6e 290a 0a53 6f6d 6520 6f66  atreon)..Some of
+00000900: 2074 6865 2070 6f70 756c 6172 2066 6561   the popular fea
+00000910: 7475 7265 7320 696e 636c 7564 653a 0a0a  tures include:..
+00000920: 2d20 4578 7065 7269 656e 6365 2074 7261  - Experience tra
+00000930: 636b 696e 670a 2d20 426f 7373 206b 696c  cking.- Boss kil
+00000940: 6c63 6f75 6e74 730a 2d20 506c 6179 6572  lcounts.- Player
+00000950: 2061 6368 6965 7665 6d65 6e74 730a 2d20   achievements.- 
+00000960: 4772 6f75 7020 636f 6d70 6574 6974 696f  Group competitio
+00000970: 6e73 0a2d 2047 6c6f 6261 6c20 6c65 6164  ns.- Global lead
+00000980: 6572 626f 6172 6473 0a2d 2041 2064 6973  erboards.- A dis
+00000990: 636f 7264 2062 6f74 2066 6f72 2069 6e74  cord bot for int
+000009a0: 6572 6163 7469 6e67 2077 6974 6820 7468  eracting with th
+000009b0: 6520 4150 490a 0a23 2320 436f 6e74 7269  e API..## Contri
+000009c0: 6275 7469 6e67 0a0a 776f 6d2e 7079 2069  buting..wom.py i
+000009d0: 7320 6f70 656e 2074 6f20 636f 6e74 7269  s open to contri
+000009e0: 6275 7469 6f6e 732e 0a0a 436f 6d65 2062  butions...Come b
+000009f0: 6163 6b20 736f 6f6e e284 a220 6f6e 6365  ack soon... once
+00000a00: 2049 2776 6520 7772 6974 7465 6e20 7468   I've written th
+00000a10: 6520 636f 6e74 7269 6275 7469 6e67 2067  e contributing g
+00000a20: 7569 6465 2e0a 0a23 2320 4c69 6365 6e73  uide...## Licens
+00000a30: 650a 0a77 6f6d 2e70 7920 6973 206c 6963  e..wom.py is lic
+00000a40: 656e 7365 6420 756e 6465 7220 7468 650a  ensed under the.
+00000a50: 5b4d 4954 204c 6963 656e 7365 5d28 6874  [MIT License](ht
+00000a60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000a70: 2f4a 6f6e 7873 6c61 7973 2f77 6f6d 2e70  /Jonxslays/wom.p
+00000a80: 792f 626c 6f62 2f6d 6173 7465 722f 4c49  y/blob/master/LI
+00000a90: 4345 4e53 4529 2e0a                      CENSE)..
```

### Comparing `wom_py-0.3.3/pyproject.toml` & `wom_py-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wom.py"
-version = "0.3.3"
+version = "0.4.0"
 description = "An asynchronous wrapper for the Wise Old Man API."
 authors = ["Jonxslays"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/wom.py"
 repository = "https://github.com/Jonxslays/wom.py"
 documentation = "https://jonxslays.github.io/wom.py"
```

### Comparing `wom_py-0.3.3/wom/__init__.py` & `wom_py-0.4.0/wom/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,43 @@
     Know what you're looking for? Hit the search bar ^!
 """
 
 from __future__ import annotations
 
 from typing import Final
 
+__packagename__: Final[str] = "wom.py"
+__version__: Final[str] = "0.4.0"
+__author__: Final[str] = "Jonxslays"
+__copyright__: Final[str] = "2023-present Jonxslays"
+__description__: Final[str] = "An asynchronous wrapper for the Wise Old Man API."
+__url__: Final[str] = "https://github.com/Jonxslays/wom.py"
+__docs__: Final[str] = "https://jonxslays.github.io/wom.py"
+__repository__: Final[str] = __url__
+__license__: Final[str] = "MIT"
+__git_sha__: Final[str] = "[47bafd3]"
+
+from . import client
+from . import constants
+from . import enums
+from . import errors
+from . import models
+from . import result
+from . import routes
+from . import serializer
+from . import services
+from .client import *
+from .enums import *
+from .errors import *
+from .models import *
+from .result import *
+from .routes import *
+from .serializer import *
+from .services import *
+
 __all__ = (
     "client",
     "constants",
     "enums",
     "errors",
     "models",
     "result",
@@ -70,14 +99,15 @@
     "CompiledRoute",
     "ComputedGains",
     "ComputedMetric",
     "ComputedMetricLeader",
     "ComputedMetrics",
     "DeltaLeaderboardEntry",
     "DeltaService",
+    "DeniedNameChangeReviewContext",
     "EfficiencyService",
     "Err",
     "Gains",
     "GroupDetail",
     "GroupHiscoresActivityItem",
     "GroupHiscoresBossItem",
     "GroupHiscoresComputedMetricItem",
@@ -91,17 +121,17 @@
     "GroupStatistics",
     "HttpErrorResponse",
     "HttpService",
     "HttpSuccessResponse",
     "Membership",
     "Metric",
     "MetricLeaders",
-    "NameChangeData",
-    "NameChangeDetail",
     "NameChange",
+    "NameChangeReviewContext",
+    "NameChangeReviewReason",
     "NameChangeService",
     "NameChangeStatus",
     "Ok",
     "Participation",
     "Period",
     "PlayerAchievementProgress",
     "PlayerBuild",
@@ -121,43 +151,15 @@
     "Result",
     "Route",
     "Serializer",
     "Skill",
     "SkillGains",
     "SkillLeader",
     "Skills",
+    "SkippedNameChangeReviewContext",
     "SnapshotData",
     "Snapshot",
     "Team",
     "Top5ProgressResult",
     "UnwrapError",
     "WomError",
 )
-
-__packagename__: Final[str] = "wom.py"
-__version__: Final[str] = "0.3.3"
-__author__: Final[str] = "Jonxslays"
-__copyright__: Final[str] = "2023-present Jonxslays"
-__description__: Final[str] = "An asynchronous wrapper for the Wise Old Man API."
-__url__: Final[str] = "https://github.com/Jonxslays/wom.py"
-__docs__: Final[str] = "https://jonxslays.github.io/wom.py"
-__repository__: Final[str] = __url__
-__license__: Final[str] = "MIT"
-__git_sha__: Final[str] = "[57608ca]"
-
-from . import client
-from . import constants
-from . import enums
-from . import errors
-from . import models
-from . import result
-from . import routes
-from . import serializer
-from . import services
-from .client import *
-from .enums import *
-from .errors import *
-from .models import *
-from .result import *
-from .routes import *
-from .serializer import *
-from .services import *
```

### Comparing `wom_py-0.3.3/wom/__main__.py` & `wom_py-0.4.0/wom/__main__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/_cli.py` & `wom_py-0.4.0/wom/_cli.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/client.py` & `wom_py-0.4.0/wom/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,18 +107,18 @@
         "_players",
         "_records",
         "_serializer",
     )
 
     def __init__(
         self,
-        api_key: str | None = None,
+        api_key: t.Optional[str] = None,
         *,
-        user_agent: str | None = None,
-        api_base_url: str | None = None,
+        user_agent: t.Optional[str] = None,
+        api_base_url: t.Optional[str] = None,
     ) -> None:
         self._serializer = serializer.Serializer()
         self._http = services.HttpService(api_key, user_agent, api_base_url)
         self.__init_core_services()
 
     @property
     def competitions(self) -> services.CompetitionService:
@@ -219,14 +219,19 @@
 
     def set_user_agent(self, user_agent: str) -> None:
         """Sets the user agent used by the http service.
 
         Args:
             user_agent: The new user agent to use.
 
+        !!! note
+
+            To remove a previously set user agent, call this method
+            with an empty string as the user agent.
+
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
```

### Comparing `wom_py-0.3.3/wom/constants.py` & `wom_py-0.4.0/wom/constants.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/enums.py` & `wom_py-0.4.0/wom/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         Returns:
             The generated enum.
         """
         return cls(value)
 
     @classmethod
-    def from_str_maybe(cls: t.Type[T], value: str) -> T | None:
+    def from_str_maybe(cls: t.Type[T], value: str) -> t.Optional[T]:
         """Attempt to generate this enum from the given value.
 
         Args:
             value: The value to generate from.
 
         Returns:
             The generated enum or `None` if the value was not a valid
@@ -80,19 +80,14 @@
     !!! tip
 
         Will always be one of [`Activities`][wom.Activities],
         [`Bosses`][wom.Bosses], [`ComputedMetrics`][wom.ComputedMetrics],
         or [`Skills`][wom.Skills].
     """
 
-    # TODO: Do we even need this method??????????
-    # @classmethod
-    # def _filter_on_value(cls: t.Type[T], value: str) -> set[T]:
-    #     return set(filter(lambda x: x.value == value, cls))  # type: ignore
-
     @classmethod
     def from_str(cls: t.Type[T], value: str) -> T:
         if cls is not Metric:
             return cls(value)
 
         children = {Skills, Activities, Bosses, ComputedMetrics}
 
@@ -101,15 +96,15 @@
                 return child(value)  # type: ignore
             except ValueError:
                 continue
 
         raise RuntimeError(f"No {cls} variant for {value!r}.")
 
     @classmethod
-    def from_str_maybe(cls: t.Type[T], value: str) -> T | None:
+    def from_str_maybe(cls: t.Type[T], value: str) -> t.Optional[T]:
         if cls is not Metric:
             return super(Metric, cls).from_str_maybe(value)  # pyright: ignore
 
         children = {Skills, Activities, Bosses, ComputedMetrics}
 
         for child in children:
             try:
```

### Comparing `wom_py-0.3.3/wom/errors.py` & `wom_py-0.4.0/wom/errors.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/models/__init__.py` & `wom_py-0.4.0/wom/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     "CompetitionStatus",
     "CompetitionType",
     "CompetitionWithParticipations",
     "ComputedGains",
     "ComputedMetric",
     "ComputedMetricLeader",
     "DeltaLeaderboardEntry",
+    "DeniedNameChangeReviewContext",
     "Gains",
     "GroupDetail",
     "GroupHiscoresActivityItem",
     "GroupHiscoresBossItem",
     "GroupHiscoresComputedMetricItem",
     "GroupHiscoresEntry",
     "GroupHiscoresSkillItem",
@@ -69,17 +70,17 @@
     "Group",
     "GroupRole",
     "GroupStatistics",
     "HttpErrorResponse",
     "HttpSuccessResponse",
     "Membership",
     "MetricLeaders",
-    "NameChangeData",
-    "NameChangeDetail",
     "NameChange",
+    "NameChangeReviewContext",
+    "NameChangeReviewReason",
     "NameChangeStatus",
     "Participation",
     "PlayerAchievementProgress",
     "PlayerBuild",
     "PlayerCompetitionStanding",
     "PlayerMembership",
     "Player",
@@ -90,14 +91,15 @@
     "PlayerStatus",
     "PlayerType",
     "Record",
     "RecordLeaderboardEntry",
     "Skill",
     "SkillGains",
     "SkillLeader",
+    "SkippedNameChangeReviewContext",
     "SnapshotData",
     "Snapshot",
     "Team",
     "Top5ProgressResult",
 )
 
 from .base import *
```

### Comparing `wom_py-0.3.3/wom/models/base.py` & `wom_py-0.4.0/wom/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,14 @@
 import attrs
 
 
 @attrs.define
 class BaseModel:
     """The base model all library models inherit from."""
 
-    def to_dict(self) -> dict[str, t.Any]:
+    def to_dict(self) -> t.Dict[str, t.Any]:
         """Converts this class into a dictionary.
 
         Returns:
             The requested dictionary.
         """
         return attrs.asdict(self)
```

### Comparing `wom_py-0.3.3/wom/models/competitions/__init__.py` & `wom_py-0.4.0/wom/models/competitions/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/models/competitions/enums.py` & `wom_py-0.4.0/wom/models/competitions/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/models/competitions/models.py` & `wom_py-0.4.0/wom/models/competitions/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Competition related models."""
 
 from __future__ import annotations
 
+import typing as t
 from datetime import datetime
 
 import attrs
 
 from wom import enums
 
 from ..base import BaseModel
@@ -82,30 +83,30 @@
 
     starts_at: datetime
     """The date the competition started at."""
 
     ends_at: datetime
     """The date the competition ended at."""
 
-    group_id: int | None
+    group_id: t.Optional[int]
     """The optional group id associated with the competition."""
 
     score: int
     """The competition's score."""
 
     created_at: datetime
     """The date the competition was created."""
 
     updated_at: datetime
     """The date the competition was updated."""
 
     participant_count: int
     """The number of players participating."""
 
-    group: Group | None
+    group: t.Optional[Group]
     """The [`Group`][wom.Group] associated with the competition, if
     there is one.
     """
 
 
 @attrs.define(init=False)
 class Participation(BaseModel):
@@ -113,15 +114,15 @@
 
     player_id: int
     """The ID of the player associated with this participation."""
 
     competition_id: int
     """The ID of the competition associated with this participation."""
 
-    team_name: str | None
+    team_name: t.Optional[str]
     """The optional team name associated with this participation."""
 
     created_at: datetime
     """The date this participation was created."""
 
     updated_at: datetime
     """The date this participation was updated."""
@@ -190,15 +191,15 @@
 @attrs.define(init=False)
 class CompetitionDetail(BaseModel):
     """Represents competition details."""
 
     competition: Competition
     """The [`Competition`][wom.Competition] that is being detailed."""
 
-    participations: list[CompetitionParticipationDetail]
+    participations: t.List[CompetitionParticipationDetail]
     """A list of [`CompetitionParticipationDetail`]
     [wom.CompetitionParticipationDetail] participations for this
     competition.
     """
 
 
 @attrs.define(init=False)
@@ -215,15 +216,15 @@
 @attrs.define(init=False)
 class Top5ProgressResult(BaseModel):
     """A top 5 progress result for a competition."""
 
     player: Player
     """The [`Player`][wom.Player] who made top 5 progress."""
 
-    history: list[CompetitionHistoryDataPoint]
+    history: t.List[CompetitionHistoryDataPoint]
     """A list of [CompetitionHistoryDataPoints]
     [wom.CompetitionHistoryDataPoint] making up the history
     of this top 5 progress result.
     """
 
 
 @attrs.define
@@ -238,38 +239,38 @@
 
     !!! tip
 
         This is a model class that you will create in order to send
         data to some endpoints.
     """
 
-    def __init__(self, name: str, participants: list[str]) -> None:
+    def __init__(self, name: str, participants: t.List[str]) -> None:
         self.name = name
         self.participants = participants
 
     name: str
     """The name of the team."""
 
-    participants: list[str]
+    participants: t.List[str]
     """A list of participant usernames on the team."""
 
 
 @attrs.define(init=False)
 class CompetitionWithParticipations(BaseModel):
     """Represents a competition with participations."""
 
     competition: Competition
     """The [`Competition`][wom.Competition] itself."""
 
-    participations: list[CompetitionParticipation]
+    participations: t.List[CompetitionParticipation]
     """A list containing the [`CompetitionParticipations`]
     [wom.CompetitionParticipation].
     """
 
-    verification_code: str | None
+    verification_code: t.Optional[str]
     """The verification code for the competition.
 
     !!! note
 
         Only returned when a competition is created and will be
         `None` otherwise.
     """
```

### Comparing `wom_py-0.3.3/wom/models/deltas/__init__.py` & `wom_py-0.4.0/wom/models/deltas/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/models/deltas/models.py` & `wom_py-0.4.0/wom/models/deltas/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/models/groups/__init__.py` & `wom_py-0.4.0/wom/models/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/models/groups/enums.py` & `wom_py-0.4.0/wom/models/groups/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/models/groups/models.py` & `wom_py-0.4.0/wom/models/groups/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
+import typing as t
 from datetime import datetime
 
 import attrs
 
 from wom import enums
 
 from ..base import BaseModel
@@ -62,18 +63,18 @@
 
     name: str
     """The groups name."""
 
     clan_chat: str
     """The clan chat for this group."""
 
-    description: str | None
+    description: t.Optional[str]
     """The groups optional description."""
 
-    homeworld: int | None
+    homeworld: t.Optional[int]
     """The groups optional homeworld."""
 
     verified: bool
     """Whether or not this group is verified."""
 
     score: int
     """The groups score."""
@@ -91,18 +92,18 @@
 @attrs.define(init=False)
 class GroupDetail(BaseModel):
     """Represents details about a group."""
 
     group: Group
     """The [`Group`][wom.Group] itself."""
 
-    memberships: list[GroupMembership]
+    memberships: t.List[GroupMembership]
     """A list of [`GroupMemberships`][wom.GroupMembership]."""
 
-    verification_code: str | None
+    verification_code: t.Optional[str]
     """The optional verification code for the group.
 
     !!! note
 
         This will only be present on group creation.
     """
 
@@ -113,15 +114,15 @@
 
     player_id: int
     """The unique ID of the player in this membership."""
 
     group_id: int
     """The group ID this membership belongs to."""
 
-    role: GroupRole | None
+    role: t.Optional[GroupRole]
     """The optional [`GroupRole`][wom.GroupRole] for this membership."""
 
     created_at: datetime
     """The date this membership was created."""
 
     updated_at: datetime
     """The date this membership was updated."""
@@ -161,39 +162,39 @@
 
     !!! tip
 
         This is a model class that you will create in order to send
         data to some endpoints.
     """
 
-    def __init__(self, username: str, role: GroupRole | None = None) -> None:
+    def __init__(self, username: str, role: t.Optional[GroupRole] = None) -> None:
         self.username = username
         self.role = role
 
     username: str
     """The group members username."""
 
-    role: GroupRole | None
+    role: t.Optional[GroupRole]
     """The optional [`GroupRole`][wom.GroupRole] for the member.
     """
 
 
 @attrs.define(init=False)
 class GroupHiscoresEntry(BaseModel):
     """Represents a group hiscores entry."""
 
     player: Player
     """The [`Player`][wom.Player] responsible for the entry."""
 
-    data: (
-        GroupHiscoresActivityItem
-        | GroupHiscoresBossItem
-        | GroupHiscoresSkillItem
-        | GroupHiscoresComputedMetricItem
-    )
+    data: t.Union[
+        GroupHiscoresActivityItem,
+        GroupHiscoresBossItem,
+        GroupHiscoresSkillItem,
+        GroupHiscoresComputedMetricItem,
+    ]
     """The data for this hiscores entry."""
 
 
 @attrs.define(init=False)
 class GroupHiscoresSkillItem(BaseModel):
     """Represents a group hiscores item for skills."""
 
@@ -313,30 +314,30 @@
     """The player leading in this metric."""
 
 
 @attrs.define(init=False)
 class MetricLeaders(BaseModel):
     """The leaders for each metric in a group."""
 
-    skills: dict[enums.Skills, SkillLeader]
+    skills: t.Dict[enums.Skills, SkillLeader]
     """A mapping of [`Skills`][wom.Skills] keys to [`SkillLeader`]
     [wom.SkillLeader] values.
     """
 
-    bosses: dict[enums.Bosses, BossLeader]
+    bosses: t.Dict[enums.Bosses, BossLeader]
     """A mapping of [`Bosses`][wom.Bosses] keys to [`BossLeader`]
     [wom.BossLeader] values.
     """
 
-    activities: dict[enums.Activities, ActivityLeader]
+    activities: t.Dict[enums.Activities, ActivityLeader]
     """A mapping of [`Activities`][wom.Activities] keys to [`ActivityLeader`]
     [wom.ActivityLeader] values.
     """
 
-    computed: dict[enums.ComputedMetrics, ComputedMetricLeader]
+    computed: t.Dict[enums.ComputedMetrics, ComputedMetricLeader]
     """A mapping of [`ComputedMetrics`][wom.ComputedMetrics] keys to
     [`ComputedMetricLeader`][wom.ComputedMetricLeader] values.
     """
 
 
 @attrs.define(init=False)
 class GroupStatistics(BaseModel):
```

### Comparing `wom_py-0.3.3/wom/models/http.py` & `wom_py-0.4.0/wom/models/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/models/names/__init__.py` & `wom_py-0.4.0/wom/models/names/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 # SOFTWARE.
 
 """The name change models and enums."""
 
 from __future__ import annotations
 
 __all__ = (
+    "DeniedNameChangeReviewContext",
     "NameChange",
-    "NameChangeData",
-    "NameChangeDetail",
+    "NameChangeReviewContext",
+    "NameChangeReviewReason",
     "NameChangeStatus",
+    "SkippedNameChangeReviewContext",
 )
 
 from .enums import *
 from .models import *
```

### Comparing `wom_py-0.3.3/wom/models/names/enums.py` & `wom_py-0.4.0/wom/models/names/enums.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,16 +19,26 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
 from wom.enums import BaseEnum
 
-__all__ = ("NameChangeStatus",)
+__all__ = ("NameChangeReviewReason", "NameChangeStatus")
 
 
 class NameChangeStatus(BaseEnum):
     """The available name change statuses."""
 
     Pending = "pending"
     Approved = "approved"
     Denied = "denied"
+
+
+class NameChangeReviewReason(BaseEnum):
+    ManualReview = "manual_review"
+    OldStatsNotFound = "old_stats_cannot_be_found"
+    NewNameNotFound = "new_name_not_on_the_hiscores"
+    NegativeGains = "negative_gains"
+    TransitionTooLong = "transition_period_too_long"
+    ExcessiveGains = "excessive_gains"
+    TotalLevelTooLow = "total_level_too_low"
```

### Comparing `wom_py-0.3.3/wom/models/players/__init__.py` & `wom_py-0.4.0/wom/models/players/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/models/players/enums.py` & `wom_py-0.4.0/wom/models/players/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/models/players/models.py` & `wom_py-0.4.0/wom/models/players/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
+import typing as t
 from datetime import datetime
 
 import attrs
 
 from wom import enums
 
 from ..base import BaseModel
@@ -124,30 +125,30 @@
     """The value of the computed metric."""
 
 
 @attrs.define(init=False)
 class SnapshotData(BaseModel):
     """The data associated with this snapshot."""
 
-    skills: dict[enums.Skills, Skill]
+    skills: t.Dict[enums.Skills, Skill]
     """A mapping of [`Skills`][wom.Skills] keys to [`Skill`][wom.Skill] values
     from this snapshot.
     """
 
-    bosses: dict[enums.Bosses, Boss]
+    bosses: t.Dict[enums.Bosses, Boss]
     """A mapping of [`Bosses`][wom.Bosses] keys to [`Boss`][wom.Boss] values
     from this snapshot.
     """
 
-    activities: dict[enums.Activities, Activity]
+    activities: t.Dict[enums.Activities, Activity]
     """A mapping of [`Activities`][wom.Activities] keys to [`Activity`]
     [wom.Activity] values from this snapshot.
     """
 
-    computed: dict[enums.ComputedMetrics, ComputedMetric]
+    computed: t.Dict[enums.ComputedMetrics, ComputedMetric]
     """A mapping of [`ComputedMetrics`][wom.ComputedMetrics] keys to
     [`ComputedMetric`][wom.ComputedMetric] values from this snapshot.
     """
 
 
 @attrs.define(init=False)
 class Snapshot(BaseModel):
@@ -155,15 +156,15 @@
 
     id: int
     """The unique ID of the snapshot."""
 
     player_id: int
     """The unique ID of the player for this snapshot."""
 
-    imported_at: datetime | None
+    imported_at: t.Optional[datetime]
     """The date the snapshot was imported, if it was."""
 
     data: SnapshotData
     """The [`SnapshotData`][wom.SnapshotData] for the snapshot."""
 
     created_at: datetime
     """The date the snapshot was created."""
@@ -184,15 +185,15 @@
 
     type: PlayerType
     """The [`PlayerType`][wom.PlayerType] for this player."""
 
     build: PlayerBuild
     """The [`PlayerBuild`][wom.PlayerBuild] for this player."""
 
-    country: Country | None
+    country: t.Optional[Country]
     """The players [`Country`][wom.Country] country of origin, if they
     have one set.
     """
 
     status: PlayerStatus
     """The players status, i.e. flagged, archived, etc."""
 
@@ -213,32 +214,32 @@
 
     registered_at: datetime
     """The date the player was registered with WOM."""
 
     updated_at: datetime
     """The date the player was last updated with WOM."""
 
-    last_changed_at: datetime | None
+    last_changed_at: t.Optional[datetime]
     """The date of the players last change (xp gain, boss kc, etc)."""
 
-    last_imported_at: datetime | None
+    last_imported_at: t.Optional[datetime]
     """The date of the last player history import."""
 
 
 @attrs.define(init=False)
 class PlayerDetail(BaseModel):
     """Represents details about a player."""
 
     player: Player
     """The [Player][wom.Player]."""
 
     combat_level: int
     """The players combat level."""
 
-    latest_snapshot: Snapshot | None
+    latest_snapshot: t.Optional[Snapshot]
     """The latest snapshot for the player, if there is one."""
 
 
 @attrs.define(init=False)
 class AssertPlayerType(BaseModel):
     """Represents a player type that has been asserted."""
 
@@ -269,15 +270,15 @@
 
     threshold: int
     """The threshold for this achievement."""
 
     created_at: datetime
     """The date the achievement was achieved."""
 
-    accuracy: int | None
+    accuracy: t.Optional[int]
     """The margin of error for the achievements creation date.
 
     !!! note
 
         Can be `None` if the achievement hasn't been recalculated since
         the addition of this field (~ Feb 2023). It can also be -1 for
         achievements with unknown dates.
@@ -301,20 +302,20 @@
     """The [`AchievementMeasure`][wom.AchievementMeasure] that
     the player obtained.
     """
 
     threshold: int
     """The threshold for this achievement."""
 
-    created_at: datetime | None
+    created_at: t.Optional[datetime]
     """The date the achievement was achieved, or `None` if it has not
     been achieved.
     """
 
-    accuracy: int | None
+    accuracy: t.Optional[int]
     """The margin of error for the achievements creation date.
 
     !!! note
 
         Can be `None` if the achievement hasn't been recalculated since
         the addition of this field (~ Feb 2023). It can also be -1 for
         achievements with unknown dates.
@@ -424,30 +425,30 @@
     """The value [`Gains`][wom.Gains]."""
 
 
 @attrs.define(init=False)
 class PlayerGainsData(BaseModel):
     """Contains all the player gains data."""
 
-    skills: dict[enums.Skills, SkillGains]
+    skills: t.Dict[enums.Skills, SkillGains]
     """A mapping of [`Skills`][wom.Skills] keys to [`SkillGains`]
     [wom.SkillGains] values.
     """
 
-    bosses: dict[enums.Bosses, BossGains]
+    bosses: t.Dict[enums.Bosses, BossGains]
     """A mapping of [`Bosses`][wom.Bosses] keys to [`BossGains`]
     [wom.BossGains] values.
     """
 
-    activities: dict[enums.Activities, ActivityGains]
+    activities: t.Dict[enums.Activities, ActivityGains]
     """A mapping of [`Activities`][wom.Activities] keys to [`ActivityGains`]
     [wom.ActivityGains] values.
     """
 
-    computed: dict[enums.ComputedMetrics, ComputedGains]
+    computed: t.Dict[enums.ComputedMetrics, ComputedGains]
     """A mapping of [`ComputedMetrics`][wom.ComputedMetrics] keys to
     [`ComputedGains`] [wom.ComputedGains] values.
     """
 
 
 @attrs.define(init=False)
 class PlayerGains(BaseModel):
```

### Comparing `wom_py-0.3.3/wom/models/records/__init__.py` & `wom_py-0.4.0/wom/models/records/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/models/records/models.py` & `wom_py-0.4.0/wom/models/records/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/result.py` & `wom_py-0.4.0/wom/result.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/routes.py` & `wom_py-0.4.0/wom/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     """
 
     __slots__ = ("_route", "_uri", "_params")
 
     def __init__(self, route: Route, uri: str) -> None:
         self._uri = uri
         self._route = route
-        self._params: dict[str, str | int] = {}
+        self._params: t.Dict[str, t.Union[str, int]] = {}
 
     @property
     def route(self) -> Route:
         """The route itself."""
         return self._route
 
     @property
@@ -60,19 +60,19 @@
 
     @property
     def method(self) -> str:
         """The routes method, i.e. GET, POST..."""
         return self.route.method
 
     @property
-    def params(self) -> dict[str, str | int]:
+    def params(self) -> t.Dict[str, t.Union[str, int]]:
         """The query params for the route."""
         return self._params
 
-    def with_params(self, params: dict[str, t.Any]) -> CompiledRoute:
+    def with_params(self, params: t.Dict[str, t.Any]) -> CompiledRoute:
         """Adds additional query params to this compiled route.
 
         Args:
             params: The query params to compile.
 
         Returns:
             The compiled route for chained calls.
@@ -88,15 +88,15 @@
     """A route that has not been compiled yet."""
 
     method: str
     """The request method to use."""
     uri: str
     """The request uri."""
 
-    def compile(self, *args: str | int) -> CompiledRoute:
+    def compile(self, *args: t.Union[str, int]) -> CompiledRoute:
         """Turn this route into a compiled route.
 
         Args:
             *args: The arguments to insert into the uri.
 
         Returns:
             The compiled route.
@@ -120,15 +120,14 @@
 PLAYER_COMPETITION_STANDINGS: t.Final[Route] = Route("GET", "/players/{}/competitions/standings")
 PLAYER_GROUP_MEMBERSHIPS: t.Final[Route] = Route("GET", "/players/{}/groups")
 PLAYER_GAINS: t.Final[Route] = Route("GET", "/players/{}/gained")
 PLAYER_RECORDS: t.Final[Route] = Route("GET", "/players/{}/records")
 PLAYER_SNAPSHOTS: t.Final[Route] = Route("GET", "/players/{}/snapshots")
 SEARCH_NAME_CHANGES: t.Final[Route] = Route("GET", "/names")
 SUBMIT_NAME_CHANGE: t.Final[Route] = Route("POST", "/names")
-NAME_CHANGE_DETAILS: t.Final[Route] = Route("GET", "/names/{}")
 PLAYER_NAME_CHANGES: t.Final[Route] = Route("GET", "/players/{}/names")
 GLOBAL_RECORD_LEADERS: t.Final[Route] = Route("GET", "/records/leaderboard")
 GLOBAL_EFFICIENCY_LEADERS: t.Final[Route] = Route("GET", "/efficiency/leaderboard")
 GLOBAL_DELTA_LEADERS: t.Final[Route] = Route("GET", "/deltas/leaderboard")
 SEARCH_GROUPS: t.Final[Route] = Route("GET", "/groups")
 GROUP_DETAILS: t.Final[Route] = Route("GET", "/groups/{}")
 CREATE_GROUP: t.Final[Route] = Route("POST", "/groups")
```

### Comparing `wom_py-0.3.3/wom/serializer.py` & `wom_py-0.4.0/wom/serializer.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 from wom import enums
 from wom import models
 
 __all__ = ("Serializer",)
 
 T = t.TypeVar("T")
-TransformT = t.Callable[[t.Any], t.Any] | None
+DictT = t.Dict[str, t.Any]
+TransformT = t.Optional[t.Callable[[t.Any], t.Any]]
 AchievementT = t.TypeVar("AchievementT", models.Achievement, models.AchievementProgress)
 HasMetricsT = t.TypeVar(
     "HasMetricsT",
     models.Skill,
     models.Boss,
     models.Activity,
     models.ComputedMetric,
@@ -57,82 +58,89 @@
     """Deserializes JSON data into wom.py model classes."""
 
     __slots__ = ()
 
     def _dt_from_iso(self, timestamp: str) -> datetime:
         return datetime.fromisoformat(timestamp.rstrip("Z"))
 
-    def _dt_from_iso_maybe(self, timestamp: str | None) -> datetime | None:
+    def _dt_from_iso_maybe(self, timestamp: t.Optional[str]) -> datetime | None:
         return self._dt_from_iso(timestamp) if timestamp else None
 
     def _to_camel_case(self, attr: str) -> str:
         first, *rest = attr.split("_")
         return "".join((first.lower(), *map(str.title, rest)))
 
     def __map(
-        self, serializer: t.Callable[[dict[str, t.Any]], HasMetricsT], data: list[dict[str, t.Any]]
-    ) -> dict[t.Any, HasMetricsT]:
+        self, serializer: t.Callable[[DictT], HasMetricsT], data: list[DictT]
+    ) -> t.Dict[t.Any, HasMetricsT]:
         return {x.metric: x for x in (serializer(y) for y in data)}
 
     def _set_attrs(
         self,
         model: t.Any,
-        data: dict[str, t.Any],
+        data: DictT,
         *attrs: str,
         transform: TransformT = None,
         camel_case: bool = False,
+        maybe: bool = False,
     ) -> None:
+        if transform and maybe:
+            raise RuntimeError("Only one of 'maybe' and 'transform' may be used.")
+
         for attr in attrs:
             cased_attr = self._to_camel_case(attr) if camel_case else attr
 
             if transform:
-                setattr(model, attr, transform(data[cased_attr]))
+                setattr(
+                    model,
+                    attr,
+                    transform(data.get(cased_attr, None) if maybe else data[cased_attr]),
+                )
             else:
-                setattr(model, attr, data[cased_attr])
+                setattr(model, attr, data.get(cased_attr, None) if maybe else data[cased_attr])
 
     def _set_attrs_cased(
         self,
         model: t.Any,
-        data: dict[str, t.Any],
+        data: DictT,
         *attrs: str,
         transform: TransformT = None,
+        maybe: bool = False,
     ) -> None:
-        self._set_attrs(model, data, *attrs, transform=transform, camel_case=True)
+        self._set_attrs(model, data, *attrs, transform=transform, camel_case=True, maybe=maybe)
 
-    def _deserialize_base_achievement(
-        self, model: AchievementT, data: dict[str, t.Any]
-    ) -> AchievementT:
+    def _deserialize_base_achievement(self, model: AchievementT, data: DictT) -> AchievementT:
         model.metric = enums.Metric.from_str(data["metric"])
         model.measure = models.AchievementMeasure.from_str(data["measure"])
         self._set_attrs_cased(model, data, "name", "player_id", "threshold", "accuracy")
         return model
 
     def _determine_hiscores_entry_item(
-        self, data: dict[str, t.Any]
-    ) -> (
-        models.GroupHiscoresActivityItem
-        | models.GroupHiscoresBossItem
-        | models.GroupHiscoresSkillItem
-        | models.GroupHiscoresComputedMetricItem
-    ):
+        self, data: DictT
+    ) -> t.Union[
+        models.GroupHiscoresActivityItem,
+        models.GroupHiscoresBossItem,
+        models.GroupHiscoresSkillItem,
+        models.GroupHiscoresComputedMetricItem,
+    ]:
         if "experience" in data:
             return self.deserialize_group_hiscores_skill_item(data)
 
         if "kills" in data:
             return self.deserialize_group_hiscores_boss_item(data)
 
         if "score" in data:
             return self.deserialize_group_hiscores_activity_item(data)
 
         if "value" in data:
             return self.deserialize_group_hiscores_computed_item(data)
 
         raise ValueError(f"Unknown hiscores entry item: {data}")
 
-    def deserialize_player(self, data: dict[str, t.Any]) -> models.Player:
+    def deserialize_player(self, data: DictT) -> models.Player:
         """Deserializes the data into a player model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -157,30 +165,30 @@
         player.country = models.Country.from_str_maybe(data["country"])
         player.registered_at = self._dt_from_iso(data["registeredAt"])
         player.updated_at = self._dt_from_iso(data["updatedAt"])
         player.last_changed_at = self._dt_from_iso_maybe(data["lastChangedAt"])
         player.last_imported_at = self._dt_from_iso_maybe(data["lastImportedAt"])
         return player
 
-    def deserialize_player_details(self, data: dict[str, t.Any]) -> models.PlayerDetail:
+    def deserialize_player_details(self, data: DictT) -> models.PlayerDetail:
         """Deserializes the data into a player detail model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         details = models.PlayerDetail()
         details.combat_level = data["combatLevel"]
         details.player = self.deserialize_player(data)
         details.latest_snapshot = self.deserialize_snapshot(data["latestSnapshot"])
         return details
 
-    def deserialize_snapshot(self, data: dict[str, t.Any]) -> models.Snapshot:
+    def deserialize_snapshot(self, data: DictT) -> models.Snapshot:
         """Deserializes the data into a snapshot model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -188,15 +196,15 @@
         snapshot = models.Snapshot()
         snapshot.created_at = self._dt_from_iso(data["createdAt"])
         snapshot.imported_at = self._dt_from_iso_maybe(data.get("importedAt"))
         snapshot.data = self.deserialize_snapshot_data(data["data"])
         self._set_attrs_cased(snapshot, data, "id", "player_id")
         return snapshot
 
-    def deserialize_snapshot_data(self, data: dict[str, t.Any]) -> models.SnapshotData:
+    def deserialize_snapshot_data(self, data: DictT) -> models.SnapshotData:
         """Deserializes the data into a snapshot data model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -204,114 +212,112 @@
         model = models.SnapshotData()
         model.skills = self.__map(self.deserialize_skill, data["skills"].values())
         model.bosses = self.__map(self.deserialize_boss, data["bosses"].values())
         model.activities = self.__map(self.deserialize_activity, data["activities"].values())
         model.computed = self.__map(self.deserialize_computed_metric, data["computed"].values())
         return model
 
-    def deserialize_skill(self, data: dict[str, t.Any]) -> models.Skill:
+    def deserialize_skill(self, data: DictT) -> models.Skill:
         """Deserializes the data into a skill model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         skill = models.Skill()
         skill.metric = enums.Skills.from_str(data["metric"])
         self._set_attrs(skill, data, "ehp", "rank", "level", "experience")
         return skill
 
-    def deserialize_boss(self, data: dict[str, t.Any]) -> models.Boss:
+    def deserialize_boss(self, data: DictT) -> models.Boss:
         """Deserializes the data into a boss model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         boss = models.Boss()
         boss.metric = enums.Bosses.from_str(data["metric"])
         self._set_attrs(boss, data, "ehb", "rank", "kills")
         return boss
 
-    def deserialize_activity(self, data: dict[str, t.Any]) -> models.Activity:
+    def deserialize_activity(self, data: DictT) -> models.Activity:
         """Deserializes the data into an activity model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         activity = models.Activity()
         activity.metric = enums.Activities.from_str(data["metric"])
         self._set_attrs(activity, data, "rank", "score")
         return activity
 
-    def deserialize_computed_metric(self, data: dict[str, t.Any]) -> models.ComputedMetric:
+    def deserialize_computed_metric(self, data: DictT) -> models.ComputedMetric:
         """Deserializes the data into a computed metric model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         computed = models.ComputedMetric()
         computed.metric = enums.ComputedMetrics.from_str(data["metric"])
         self._set_attrs(computed, data, "rank", "value")
         return computed
 
-    def deserialize_asserted_player_type(self, data: dict[str, t.Any]) -> models.AssertPlayerType:
+    def deserialize_asserted_player_type(self, data: DictT) -> models.AssertPlayerType:
         """Deserializes the data into an assert player type model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         asserted = models.AssertPlayerType()
         asserted.player = self.deserialize_player(data["player"])
         asserted.changed = data["changed"]
         return asserted
 
-    def deserialize_achievement_progress(
-        self, data: dict[str, t.Any]
-    ) -> models.AchievementProgress:
+    def deserialize_achievement_progress(self, data: DictT) -> models.AchievementProgress:
         """Deserializes the data into an achievement progress model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         achievement = self._deserialize_base_achievement(models.AchievementProgress(), data)
         achievement.created_at = self._dt_from_iso_maybe(data["createdAt"])
         return achievement
 
-    def deserialize_achievement(self, data: dict[str, t.Any]) -> models.Achievement:
+    def deserialize_achievement(self, data: DictT) -> models.Achievement:
         """Deserializes the data into an achievement model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         achievement = self._deserialize_base_achievement(models.Achievement(), data)
         achievement.created_at = self._dt_from_iso(data["createdAt"])
         return achievement
 
     def deserialize_player_achievement_progress(
-        self, data: dict[str, t.Any]
+        self, data: DictT
     ) -> models.PlayerAchievementProgress:
         """Deserializes the data into a player achievement progress
         model.
 
         Args:
             data: The JSON payload.
 
@@ -322,28 +328,28 @@
         progress.achievement = self.deserialize_achievement_progress(data)
         self._set_attrs_cased(
             progress, data, "current_value", "absolute_progress", "relative_progress"
         )
 
         return progress
 
-    def deserialize_gains(self, data: dict[str, t.Any]) -> models.Gains:
+    def deserialize_gains(self, data: DictT) -> models.Gains:
         """Deserializes the data into a gains model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         gains = models.Gains()
         self._set_attrs(gains, data, "gained", "start", "end")
         return gains
 
-    def deserialize_skill_gains(self, data: dict[str, t.Any]) -> models.SkillGains:
+    def deserialize_skill_gains(self, data: DictT) -> models.SkillGains:
         """Deserializes the data into a skill gains model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -352,57 +358,57 @@
         gains.metric = enums.Skills.from_str(data["metric"])
         self._set_attrs(
             gains, data, "experience", "ehp", "rank", "level", transform=self.deserialize_gains
         )
 
         return gains
 
-    def deserialize_boss_gains(self, data: dict[str, t.Any]) -> models.BossGains:
+    def deserialize_boss_gains(self, data: DictT) -> models.BossGains:
         """Deserializes the data into a boss gains model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         gains = models.BossGains()
         gains.metric = enums.Bosses.from_str(data["metric"])
         self._set_attrs(gains, data, "ehb", "rank", "kills", transform=self.deserialize_gains)
         return gains
 
-    def deserialize_activity_gains(self, data: dict[str, t.Any]) -> models.ActivityGains:
+    def deserialize_activity_gains(self, data: DictT) -> models.ActivityGains:
         """Deserializes the data into an activity gains model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         gains = models.ActivityGains()
         gains.metric = enums.Activities.from_str(data["metric"])
         self._set_attrs(gains, data, "rank", "score", transform=self.deserialize_gains)
         return gains
 
-    def deserialize_computed_gains(self, data: dict[str, t.Any]) -> models.ComputedGains:
+    def deserialize_computed_gains(self, data: DictT) -> models.ComputedGains:
         """Deserializes the data into a computed gains model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         gains = models.ComputedGains()
         gains.metric = enums.ComputedMetrics.from_str(data["metric"])
         self._set_attrs(gains, data, "rank", "value", transform=self.deserialize_gains)
         return gains
 
-    def deserialize_player_gains_data(self, data: dict[str, t.Any]) -> models.PlayerGainsData:
+    def deserialize_player_gains_data(self, data: DictT) -> models.PlayerGainsData:
         """Deserializes the data into a player gains data model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -410,103 +416,111 @@
         gains = models.PlayerGainsData()
         gains.skills = self.__map(self.deserialize_skill_gains, data["skills"].values())
         gains.bosses = self.__map(self.deserialize_boss_gains, data["bosses"].values())
         gains.computed = self.__map(self.deserialize_computed_gains, data["computed"].values())
         gains.activities = self.__map(self.deserialize_activity_gains, data["activities"].values())
         return gains
 
-    def deserialize_player_gains(self, data: dict[str, t.Any]) -> models.PlayerGains:
+    def deserialize_player_gains(self, data: DictT) -> models.PlayerGains:
         """Deserializes the data into a player gains model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         gains = models.PlayerGains()
         gains.data = self.deserialize_player_gains_data(data["data"])
         self._set_attrs_cased(gains, data, "starts_at", "ends_at", transform=self._dt_from_iso)
 
         return gains
 
-    def deserialize_name_change(self, data: dict[str, t.Any]) -> models.NameChange:
-        """Deserializes the data into a name change model.
+    def deserialize_name_change_review_context(
+        self, data: DictT
+    ) -> models.NameChangeReviewContext:
+        """Deserializes the data into a name change review context.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
-        change = models.NameChange()
-        change.status = models.NameChangeStatus.from_str(data["status"])
-        change.updated_at = self._dt_from_iso(data["updatedAt"])
-        change.created_at = self._dt_from_iso(data["createdAt"])
-        change.resolved_at = self._dt_from_iso_maybe(data["createdAt"])
-        self._set_attrs_cased(change, data, "id", "player_id", "old_name", "new_name")
-        return change
-
-    def deserialize_name_change_data(self, data: dict[str, t.Any]) -> models.NameChangeData:
-        """Deserializes the data into a name change data model.
-
-        Args:
-            data: The JSON payload.
+        ctx: models.NameChangeReviewContext
+        reason = models.NameChangeReviewReason.from_str(data["reason"])
 
-        Returns:
-            The requested model.
-        """
-        change_data = models.NameChangeData()
-        change_data.old_stats = self.deserialize_snapshot(data["oldStats"])
-        # NOTE: Hack to handle case where name change details new stats
-        # don't have an ID if the new username is not tracked by WOM
-        change_data.new_stats = None
-        new_stats = data.get("newStats")
-
-        if new_stats:
-            if "id" not in new_stats:
-                new_stats["id"] = -1
-
-            change_data.new_stats = self.deserialize_snapshot(new_stats)
+        skipped_reasons = (
+            models.NameChangeReviewReason.TransitionTooLong,
+            models.NameChangeReviewReason.ExcessiveGains,
+            models.NameChangeReviewReason.TotalLevelTooLow,
+        )
 
-        self._set_attrs_cased(
-            change_data,
-            data,
-            "is_new_on_hiscores",
-            "is_old_on_hiscores",
-            "has_negative_gains",
-            "is_new_tracked",
-            "time_diff",
-            "hours_diff",
-            "ehp_diff",
-            "ehb_diff",
+        denied_reasons = (
+            models.NameChangeReviewReason.ManualReview,
+            models.NameChangeReviewReason.OldStatsNotFound,
+            models.NameChangeReviewReason.NewNameNotFound,
+            models.NameChangeReviewReason.NegativeGains,
         )
 
-        return change_data
+        if reason in skipped_reasons:
+            ctx = models.SkippedNameChangeReviewContext()
+            ctx.reason = reason  # type: ignore[assignment]
+            self._set_attrs_cased(
+                ctx,
+                data,
+                "max_hours_diff",
+                "hours_diff",
+                "ehp_diff",
+                "ehb_diff",
+                "min_total_level",
+                "total_level",
+                maybe=True,
+            )
+        elif reason in denied_reasons:
+            ctx = models.DeniedNameChangeReviewContext()
+            ctx.reason = reason  # type: ignore[assignment]
+            ctx.negative_gains = None
+
+            if reason is models.NameChangeReviewReason.NegativeGains:
+                negative_gains: t.Dict[enums.Metric, int] = {}
+
+                for metric, value in data["negativeGains"].items():
+                    negative_gains[enums.Metric.from_str(metric)] = value
+
+                ctx.negative_gains = negative_gains
+        else:
+            raise RuntimeError("Unreachable code reached! Serializer::name_change_review_context")
+
+        return ctx
 
-    def deserialize_name_change_detail(self, data: dict[str, t.Any]) -> models.NameChangeDetail:
-        """Deserializes the data into a name change detail model.
+    def deserialize_name_change(self, data: DictT) -> models.NameChange:
+        """Deserializes the data into a name change model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
-        change_detail = models.NameChangeDetail()
-        change_detail.name_change = self.deserialize_name_change(data["nameChange"])
+        change = models.NameChange()
+        change.status = models.NameChangeStatus.from_str(data["status"])
+        change.updated_at = self._dt_from_iso(data["updatedAt"])
+        change.created_at = self._dt_from_iso(data["createdAt"])
+        change.resolved_at = self._dt_from_iso_maybe(data["createdAt"])
+        self._set_attrs_cased(change, data, "id", "player_id", "old_name", "new_name")
 
-        # Data is only present on pending name changes
-        change_detail.data = (
-            self.deserialize_name_change_data(d) if (d := data.get("data")) else None
-        )
+        if review_context := data.get("reviewContext", None):
+            change.review_context = self.deserialize_name_change_review_context(review_context)
+        else:
+            change.review_context = review_context
 
-        return change_detail
+        return change
 
-    def deserialize_record(self, data: dict[str, t.Any]) -> models.Record:
+    def deserialize_record(self, data: DictT) -> models.Record:
         """Deserializes the data into a record model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -514,33 +528,29 @@
         record = models.Record()
         record.period = enums.Period.from_str(data["period"])
         record.metric = enums.Metric.from_str(data["metric"])
         record.updated_at = self._dt_from_iso(data["updatedAt"])
         self._set_attrs_cased(record, data, "id", "player_id", "value")
         return record
 
-    def deserialize_record_leaderboard_entry(
-        self, data: dict[str, t.Any]
-    ) -> models.RecordLeaderboardEntry:
+    def deserialize_record_leaderboard_entry(self, data: DictT) -> models.RecordLeaderboardEntry:
         """Deserializes the data into a record leaderboard entry model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         record = models.RecordLeaderboardEntry()
         record.record = self.deserialize_record(data)
         record.player = self.deserialize_player(data["player"])
         return record
 
-    def deserialize_delta_leaderboard_entry(
-        self, data: dict[str, t.Any]
-    ) -> models.DeltaLeaderboardEntry:
+    def deserialize_delta_leaderboard_entry(self, data: DictT) -> models.DeltaLeaderboardEntry:
         """Deserializes the data into a delta leaderboard entry  model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -549,15 +559,15 @@
         delta.gained = data["gained"]
         delta.player_id = data["playerId"]
         delta.end_date = self._dt_from_iso(data["endDate"])
         delta.start_date = self._dt_from_iso(data["startDate"])
         delta.player = self.deserialize_player(data["player"])
         return delta
 
-    def deserialize_group(self, data: dict[str, t.Any]) -> models.Group:
+    def deserialize_group(self, data: DictT) -> models.Group:
         """Deserializes the data into a group model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -576,15 +586,15 @@
             "verified",
             "score",
             "member_count",
         )
 
         return group
 
-    def deserialize_membership(self, data: dict[str, t.Any]) -> models.Membership:
+    def deserialize_membership(self, data: DictT) -> models.Membership:
         """Deserializes the data into a membership model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -592,29 +602,29 @@
         membership = models.Membership()
         membership.role = models.GroupRole.from_str_maybe(data["role"])
         membership.created_at = self._dt_from_iso(data["createdAt"])
         membership.updated_at = self._dt_from_iso(data["updatedAt"])
         self._set_attrs_cased(membership, data, "player_id", "group_id")
         return membership
 
-    def deserialize_group_membership(self, data: dict[str, t.Any]) -> models.GroupMembership:
+    def deserialize_group_membership(self, data: DictT) -> models.GroupMembership:
         """Deserializes the data into a group membership model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         group = models.GroupMembership()
         group.player = self.deserialize_player(data["player"])
         group.membership = self.deserialize_membership(data)
         return group
 
-    def deserialize_group_details(self, data: dict[str, t.Any]) -> models.GroupDetail:
+    def deserialize_group_details(self, data: DictT) -> models.GroupDetail:
         """Deserializes the data into a group detail model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -622,92 +632,86 @@
         details = models.GroupDetail()
         details.verification_code = None
         details.group = self.deserialize_group(data)
         details.memberships = [self.deserialize_group_membership(m) for m in data["memberships"]]
         return details
 
     def deserialize_group_hiscores_activity_item(
-        self, data: dict[str, t.Any]
+        self, data: DictT
     ) -> models.GroupHiscoresActivityItem:
         """Deserializes the data into a group hiscores activity item
         model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         item = models.GroupHiscoresActivityItem()
         self._set_attrs(item, data, "rank", "score")
         return item
 
-    def deserialize_group_hiscores_boss_item(
-        self, data: dict[str, t.Any]
-    ) -> models.GroupHiscoresBossItem:
+    def deserialize_group_hiscores_boss_item(self, data: DictT) -> models.GroupHiscoresBossItem:
         """Deserializes the data into a group hiscores boss item model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         item = models.GroupHiscoresBossItem()
         self._set_attrs(item, data, "rank", "kills")
         return item
 
-    def deserialize_group_hiscores_skill_item(
-        self, data: dict[str, t.Any]
-    ) -> models.GroupHiscoresSkillItem:
+    def deserialize_group_hiscores_skill_item(self, data: DictT) -> models.GroupHiscoresSkillItem:
         """Deserializes the data into a group hiscores skill item model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         item = models.GroupHiscoresSkillItem()
         self._set_attrs(item, data, "rank", "level", "experience")
         return item
 
     def deserialize_group_hiscores_computed_item(
-        self, data: dict[str, t.Any]
+        self, data: DictT
     ) -> models.GroupHiscoresComputedMetricItem:
         """Deserializes the data into a group hiscores computed metric
         item model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         item = models.GroupHiscoresComputedMetricItem()
         self._set_attrs(item, data, "rank", "value")
         return item
 
-    def deserialize_group_hiscores_entry(
-        self, data: dict[str, t.Any]
-    ) -> models.GroupHiscoresEntry:
+    def deserialize_group_hiscores_entry(self, data: DictT) -> models.GroupHiscoresEntry:
         """Deserializes the data into a group hiscores entry model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         hiscores = models.GroupHiscoresEntry()
         hiscores.player = self.deserialize_player(data["player"])
         hiscores.data = self._determine_hiscores_entry_item(data["data"])
         return hiscores
 
-    def deserialize_group_statistics(self, data: dict[str, t.Any]) -> models.GroupStatistics:
+    def deserialize_group_statistics(self, data: DictT) -> models.GroupStatistics:
         """Deserializes the data into a group statistics model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -715,15 +719,15 @@
         statistics = models.GroupStatistics()
         statistics.maxed_200ms_count = data["maxed200msCount"]
         statistics.average_stats = self.deserialize_snapshot(data["averageStats"])
         statistics.metric_leaders = self.deserialize_metric_leaders(data["metricLeaders"])
         self._set_attrs_cased(statistics, data, "maxed_total_count", "maxed_combat_count")
         return statistics
 
-    def deserialize_competition(self, data: dict[str, t.Any]) -> models.Competition:
+    def deserialize_competition(self, data: DictT) -> models.Competition:
         """Deserializes the data into a competition model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -745,78 +749,74 @@
 
         self._set_attrs_cased(
             competition, data, "id", "title", "group_id", "score", "participant_count"
         )
 
         return competition
 
-    def deserialize_participation(self, data: dict[str, t.Any]) -> models.Participation:
+    def deserialize_participation(self, data: DictT) -> models.Participation:
         """Deserializes the data into a participation model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         participation = models.Participation()
         participation.created_at = self._dt_from_iso(data["createdAt"])
         participation.updated_at = self._dt_from_iso(data["updatedAt"])
         self._set_attrs_cased(participation, data, "player_id", "competition_id", "team_name")
         return participation
 
-    def deserialize_player_participation(
-        self, data: dict[str, t.Any]
-    ) -> models.PlayerParticipation:
+    def deserialize_player_participation(self, data: DictT) -> models.PlayerParticipation:
         """Deserializes the data into a player participation model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         player_participation = models.PlayerParticipation()
         player_participation.competition = self.deserialize_competition(data["competition"])
         player_participation.data = self.deserialize_participation(data)
         return player_participation
 
     def deserialize_competition_participation(
-        self, data: dict[str, t.Any]
+        self, data: DictT
     ) -> models.CompetitionParticipation:
         """Deserializes the data into a competition participation model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         competition_participation = models.CompetitionParticipation()
         competition_participation.player = self.deserialize_player(data["player"])
         competition_participation.data = self.deserialize_participation(data)
         return competition_participation
 
-    def deserialize_competition_progress(
-        self, data: dict[str, t.Any]
-    ) -> models.CompetitionProgress:
+    def deserialize_competition_progress(self, data: DictT) -> models.CompetitionProgress:
         """Deserializes the data into a competition progress model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         progress = models.CompetitionProgress()
         self._set_attrs(progress, data, "start", "end", "gained")
         return progress
 
     def deserialize_player_competition_standing(
-        self, data: dict[str, t.Any]
+        self, data: DictT
     ) -> models.PlayerCompetitionStanding:
         """Deserializes the data into a player competition standing
         model.
 
         Args:
             data: The JSON payload.
 
@@ -825,29 +825,29 @@
         """
         standing = models.PlayerCompetitionStanding()
         standing.rank = data["rank"]
         standing.participation = self.deserialize_player_participation(data)
         standing.progress = self.deserialize_competition_progress(data["progress"])
         return standing
 
-    def deserialize_player_membership(self, data: dict[str, t.Any]) -> models.PlayerMembership:
+    def deserialize_player_membership(self, data: DictT) -> models.PlayerMembership:
         """Deserializes the data into a player membership model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         player_membership = models.PlayerMembership()
         player_membership.group = self.deserialize_group(data["group"])
         player_membership.membership = self.deserialize_membership(data)
         return player_membership
 
-    def deserialize_competition_details(self, data: dict[str, t.Any]) -> models.CompetitionDetail:
+    def deserialize_competition_details(self, data: DictT) -> models.CompetitionDetail:
         """Deserializes the data into a competition detail model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -857,15 +857,15 @@
         details.participations = [
             self.deserialize_competition_participation_detail(d) for d in data["participations"]
         ]
 
         return details
 
     def deserialize_competition_participation_detail(
-        self, data: dict[str, t.Any]
+        self, data: DictT
     ) -> models.CompetitionParticipationDetail:
         """Deserializes the data into a competition participation
         detail model.
 
         Args:
             data: The JSON payload.
 
@@ -874,15 +874,15 @@
         """
         participation_details = models.CompetitionParticipationDetail()
         participation_details.participation = self.deserialize_competition_participation(data)
         participation_details.progress = self.deserialize_competition_progress(data["progress"])
         return participation_details
 
     def deserialize_competition_history_data_point(
-        self, data: dict[str, t.Any]
+        self, data: DictT
     ) -> models.CompetitionHistoryDataPoint:
         """Deserializes the data into a competition history data point
         model.
 
         Args:
             data: The JSON payload.
 
@@ -890,17 +890,15 @@
             The requested model.
         """
         datapoint = models.CompetitionHistoryDataPoint()
         datapoint.date = self._dt_from_iso(data["date"])
         datapoint.value = data["value"]
         return datapoint
 
-    def deserialize_top5_progress_result(
-        self, data: dict[str, t.Any]
-    ) -> models.Top5ProgressResult:
+    def deserialize_top5_progress_result(self, data: DictT) -> models.Top5ProgressResult:
         """Deserializes the data into a top 5 progress result model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
@@ -910,15 +908,15 @@
         progress.history = [
             self.deserialize_competition_history_data_point(h) for h in data["history"]
         ]
 
         return progress
 
     def deserialize_competition_with_participation(
-        self, data: dict[str, t.Any]
+        self, data: DictT
     ) -> models.CompetitionWithParticipations:
         """Deserializes the data into a competition with participations
         model.
 
         Args:
             data: The JSON payload.
 
@@ -930,75 +928,75 @@
         model.competition = self.deserialize_competition(data)
         model.participations = [
             self.deserialize_competition_participation(p) for p in data["participations"]
         ]
 
         return model
 
-    def deserialize_skill_leader(self, data: dict[str, t.Any]) -> models.SkillLeader:
+    def deserialize_skill_leader(self, data: DictT) -> models.SkillLeader:
         """Deserializes the data into a skill leader model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         leader = models.SkillLeader()
         leader.metric = enums.Skills.from_str(data["metric"])
         leader.player = self.deserialize_player(data["player"])
         self._set_attrs(leader, data, "experience", "rank", "level")
         return leader
 
-    def deserialize_boss_leader(self, data: dict[str, t.Any]) -> models.BossLeader:
+    def deserialize_boss_leader(self, data: DictT) -> models.BossLeader:
         """Deserializes the data into a boss leader model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         leader = models.BossLeader()
         leader.metric = enums.Bosses.from_str(data["metric"])
         leader.player = self.deserialize_player(data["player"])
         self._set_attrs(leader, data, "kills", "rank")
         return leader
 
-    def deserialize_activity_leader(self, data: dict[str, t.Any]) -> models.ActivityLeader:
+    def deserialize_activity_leader(self, data: DictT) -> models.ActivityLeader:
         """Deserializes the data into an activity leader model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         leader = models.ActivityLeader()
         leader.metric = enums.Activities.from_str(data["metric"])
         leader.player = self.deserialize_player(data["player"])
         self._set_attrs(leader, data, "score", "rank")
         return leader
 
-    def deserialize_computed_leader(self, data: dict[str, t.Any]) -> models.ComputedMetricLeader:
+    def deserialize_computed_leader(self, data: DictT) -> models.ComputedMetricLeader:
         """Deserializes the data into a computed metric leader model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         leader = models.ComputedMetricLeader()
         leader.metric = enums.ComputedMetrics.from_str(data["metric"])
         leader.player = self.deserialize_player(data["player"])
         self._set_attrs(leader, data, "value", "rank")
         return leader
 
-    def deserialize_metric_leaders(self, data: dict[str, t.Any]) -> models.MetricLeaders:
+    def deserialize_metric_leaders(self, data: DictT) -> models.MetricLeaders:
         """Deserializes the data into a metric leaders model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
```

### Comparing `wom_py-0.3.3/wom/services/__init__.py` & `wom_py-0.4.0/wom/services/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.3/wom/services/base.py` & `wom_py-0.4.0/wom/services/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,12 +43,12 @@
     """
 
     __slots__ = ("_dict", "_list", "_http", "_serializer")
 
     def __init__(self, http_service: HttpService, serializer: serializer.Serializer) -> None:
         self._http = http_service
         self._serializer = serializer
-        self._dict = dict[str, t.Any]
-        self._list = list[dict[str, t.Any]]
+        self._dict = t.Dict[str, t.Any]
+        self._list = t.List[t.Dict[str, t.Any]]
 
-    def _generate_map(self, **kwargs: t.Any) -> dict[str, t.Any]:
+    def _generate_map(self, **kwargs: t.Any) -> t.Dict[str, t.Any]:
         return {k: v for k, v in kwargs.items() if v is not None}
```

### Comparing `wom_py-0.3.3/wom/services/competitions.py` & `wom_py-0.4.0/wom/services/competitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,21 +41,21 @@
     """Handles endpoints related to competitions."""
 
     __slots__ = ()
 
     async def search_competitions(
         self,
         *,
-        title: str | None = None,
-        type: models.CompetitionType | None = None,
-        status: models.CompetitionStatus | None = None,
-        metric: enums.Metric | None = None,
-        limit: int | None = None,
-        offset: int | None = None,
-    ) -> ResultT[list[models.Competition]]:
+        title: t.Optional[str] = None,
+        type: t.Optional[models.CompetitionType] = None,
+        status: t.Optional[models.CompetitionStatus] = None,
+        metric: t.Optional[enums.Metric] = None,
+        limit: t.Optional[int] = None,
+        offset: t.Optional[int] = None,
+    ) -> ResultT[t.List[models.Competition]]:
         """Searches for competitions with the given criteria.
 
         Keyword Args:
             title: The optional title of the competition. Defaults to
                 `None`.
 
             type: The optional [`CompetitionType`][wom.CompetitionType]
@@ -109,15 +109,15 @@
 
         if isinstance(data, models.HttpErrorResponse):
             return result.Err(data)
 
         return result.Ok([self._serializer.deserialize_competition(c) for c in data])
 
     async def get_details(
-        self, id: int, *, metric: enums.Metric | None = None
+        self, id: int, *, metric: t.Optional[enums.Metric] = None
     ) -> ResultT[models.CompetitionDetail]:
         """Gets details for the given competition.
 
         Args:
             id: The ID of the competition.
 
         Keyword Args:
@@ -150,16 +150,16 @@
 
         if isinstance(data, models.HttpErrorResponse):
             return result.Err(data)
 
         return result.Ok(self._serializer.deserialize_competition_details(data))
 
     async def get_top_participant_history(
-        self, id: int, *, metric: enums.Metric | None = None
-    ) -> ResultT[list[models.Top5ProgressResult]]:
+        self, id: int, *, metric: t.Optional[enums.Metric] = None
+    ) -> ResultT[t.List[models.Top5ProgressResult]]:
         """Gets details for the players with the top 5 progress in the
         competition.
 
         Args:
             id: The ID of the competition.
 
         Keyword Args:
@@ -197,18 +197,18 @@
     async def create_competition(
         self,
         title: str,
         metric: enums.Metric,
         starts_at: datetime,
         ends_at: datetime,
         *,
-        group_id: int | None = None,
-        group_verification_code: str | None = None,
-        teams: list[models.Team] | None = None,
-        participants: list[str] | None = None,
+        group_id: t.Optional[int] = None,
+        group_verification_code: t.Optional[str] = None,
+        teams: t.Optional[t.List[models.Team]] = None,
+        participants: t.Optional[t.List[str]] = None,
     ) -> ResultT[models.CompetitionWithParticipations]:
         """Creates a new competition.
 
         Args:
             title: The title of the competition.
 
             metric: The [`Metric`][wom.Metric] the competition should
@@ -297,20 +297,20 @@
         return result.Ok(competition)
 
     async def edit_competition(
         self,
         id: int,
         verification_code: str,
         *,
-        title: str | None = None,
-        metric: enums.Metric | None = None,
-        starts_at: datetime | None = None,
-        ends_at: datetime | None = None,
-        teams: list[models.Team] | None = None,
-        participants: list[str] | None = None,
+        title: t.Optional[str] = None,
+        metric: t.Optional[enums.Metric] = None,
+        starts_at: t.Optional[datetime] = None,
+        ends_at: t.Optional[datetime] = None,
+        teams: t.Optional[t.List[models.Team]] = None,
+        participants: t.Optional[t.List[str]] = None,
     ) -> ResultT[models.CompetitionWithParticipations]:
         """Edits an existing competition.
 
         Args:
             id: The ID of the competition.
 
             verification_code: The verification code for the
@@ -593,15 +593,15 @@
     ) -> ResultT[models.HttpSuccessResponse]:
         """Attempts to update all outdated competition participants.
 
         !!! info
 
             Participants are outdated when either:
 
-            - Competition is ending or started with 6h of now and
+            - Competition is ending or started within 6h of now and
                 the player hasn't been updated in over 1h.
 
             - Player hasn't been updated in over 24h.
 
         !!! warning
 
             This method adds every outdated participant to an
```

### Comparing `wom_py-0.3.3/wom/services/deltas.py` & `wom_py-0.4.0/wom/services/efficiency.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,80 +26,79 @@
 from wom import enums
 from wom import models
 from wom import result
 from wom import routes
 
 from . import BaseService
 
-__all__ = ("DeltaService",)
+__all__ = ("EfficiencyService",)
 
 ValueT = t.TypeVar("ValueT")
 ResultT = result.Result[ValueT, models.HttpErrorResponse]
 
 
-class DeltaService(BaseService):
-    """Handles endpoints related to deltas."""
+class EfficiencyService(BaseService):
+    """Handles endpoints related to efficiency."""
 
     __slots__ = ()
 
-    async def get_global_leaderboards(
+    async def get_global_leaderboard(
         self,
-        metric: enums.Metric,
-        period: enums.Period,
+        metric: enums.ComputedMetrics = enums.ComputedMetrics.Ehp,
         *,
-        player_type: models.PlayerType | None = None,
-        player_build: models.PlayerBuild | None = None,
-        country: models.Country | None = None,
-    ) -> ResultT[list[models.DeltaLeaderboardEntry]]:
-        """Gets the top global delta leaderboard for a specific
-        metric and period.
+        player_type: t.Optional[models.PlayerType] = None,
+        player_build: t.Optional[models.PlayerBuild] = None,
+        country: t.Optional[models.Country] = None,
+        both: bool = False,
+    ) -> ResultT[t.List[models.Player]]:
+        """Gets the top global efficiency leaderboard.
 
         Args:
-            metric: The metric to filter on.
-
-            period: The period of time to filter on.
+            metric: The computed metric to filter on. Defaults to [`Ehp`]
+                [wom.ComputedMetrics].
 
         Keyword Args:
             player_type: The optional player type to filter on. Defaults
                 to `None`.
 
             player_build: The optional player build to filter on.
                 Defaults to `None`.
 
             country: The optional country to filter on. Defaults to
                 `None`.
 
+            both: If `True`, request both ehp and ehb computed metric
+                leaderboards. This will override the `metric`, if it was
+                provided. Defaults to `False`.
+
         Returns:
-            A [`Result`][wom.Result] containing a list of  delta
-                leaderboard entries.
+            A [`Result`][wom.Result] containing a list of the top
+                players.
 
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
             await client.start()
 
-            result = await client.deltas.get_global_leaderboards(
-                wom.Skills.Attack,
-                wom.Period.Day,
-                country=wom.Country.Gb,
+            result = await client.efficiency.get_global_leaderboard(
+                player_type=wom.PlayerType.Ironman,
             )
             ```
         """
         params = self._generate_map(
-            metric=metric.value,
-            period=period.value,
+            metric=metric.value if not both else "+".join(m.value for m in enums.ComputedMetrics),
             playerType=player_type.value if player_type else None,
             playerBuild=player_build.value if player_build else None,
             country=country.value if country else None,
         )
 
-        route = routes.GLOBAL_DELTA_LEADERS.compile().with_params(params)
+        route = routes.GLOBAL_EFFICIENCY_LEADERS.compile().with_params(params)
         data = await self._http.fetch(route, self._list)
 
         if isinstance(data, models.HttpErrorResponse):
             return result.Err(data)
 
-        return result.Ok([self._serializer.deserialize_delta_leaderboard_entry(d) for d in data])
+        return result.Ok([self._serializer.deserialize_player(p) for p in data])
```

### Comparing `wom_py-0.3.3/wom/services/efficiency.py` & `wom_py-0.4.0/wom/services/deltas.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,79 +26,80 @@
 from wom import enums
 from wom import models
 from wom import result
 from wom import routes
 
 from . import BaseService
 
-__all__ = ("EfficiencyService",)
+__all__ = ("DeltaService",)
 
 ValueT = t.TypeVar("ValueT")
 ResultT = result.Result[ValueT, models.HttpErrorResponse]
 
 
-class EfficiencyService(BaseService):
-    """Handles endpoints related to efficiency."""
+class DeltaService(BaseService):
+    """Handles endpoints related to deltas."""
 
     __slots__ = ()
 
-    async def get_global_leaderboard(
+    async def get_global_leaderboards(
         self,
-        metric: enums.ComputedMetrics = enums.ComputedMetrics.Ehp,
+        metric: enums.Metric,
+        period: enums.Period,
         *,
-        player_type: models.PlayerType | None = None,
-        player_build: models.PlayerBuild | None = None,
-        country: models.Country | None = None,
-        both: bool = False,
-    ) -> ResultT[list[models.Player]]:
-        """Gets the top global efficiency leaderboard.
+        player_type: t.Optional[models.PlayerType] = None,
+        player_build: t.Optional[models.PlayerBuild] = None,
+        country: t.Optional[models.Country] = None,
+    ) -> ResultT[t.List[models.DeltaLeaderboardEntry]]:
+        """Gets the top global delta leaderboard for a specific
+        metric and period.
 
         Args:
-            metric: The computed metric to filter on. Defaults to [`Ehp`]
-                [wom.ComputedMetrics].
+            metric: The metric to filter on.
+
+            period: The period of time to filter on.
 
         Keyword Args:
             player_type: The optional player type to filter on. Defaults
                 to `None`.
 
             player_build: The optional player build to filter on.
                 Defaults to `None`.
 
             country: The optional country to filter on. Defaults to
                 `None`.
 
-            both: If `True`, request both ehp and ehb computed metric
-                leaderboards. This will override the `metric`, if it was
-                provided. Defaults to `False`.
-
         Returns:
-            A [`Result`][wom.Result] containing a list of the top
-                players.
+            A [`Result`][wom.Result] containing a list of  delta
+                leaderboard entries.
 
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
             await client.start()
 
-            result = await client.efficiency.get_global_leaderboard(
-                player_type=wom.PlayerType.Ironman,
+            result = await client.deltas.get_global_leaderboards(
+                wom.Skills.Attack,
+                wom.Period.Day,
+                country=wom.Country.Gb,
             )
             ```
         """
         params = self._generate_map(
-            metric=metric.value if not both else "+".join(m.value for m in enums.ComputedMetrics),
+            metric=metric.value,
+            period=period.value,
             playerType=player_type.value if player_type else None,
             playerBuild=player_build.value if player_build else None,
             country=country.value if country else None,
         )
 
-        route = routes.GLOBAL_EFFICIENCY_LEADERS.compile().with_params(params)
+        route = routes.GLOBAL_DELTA_LEADERS.compile().with_params(params)
         data = await self._http.fetch(route, self._list)
 
         if isinstance(data, models.HttpErrorResponse):
             return result.Err(data)
 
-        return result.Ok([self._serializer.deserialize_player(p) for p in data])
+        return result.Ok([self._serializer.deserialize_delta_leaderboard_entry(d) for d in data])
```

### Comparing `wom_py-0.3.3/wom/services/groups.py` & `wom_py-0.4.0/wom/services/groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,20 +41,23 @@
 class GroupService(BaseService):
     """Handles endpoints related to groups."""
 
     __slots__ = ()
 
     def _prepare_member_fragments(
         self, members: t.Iterable[models.GroupMemberFragment]
-    ) -> tuple[dict[str, t.Any], ...]:
+    ) -> tuple[t.Dict[str, t.Any], ...]:
         return tuple({k: str(v) for k, v in m.to_dict().items() if v} for m in members)
 
     async def search_groups(
-        self, name: str | None = None, limit: int | None = None, offset: int | None = None
-    ) -> ResultT[list[models.Group]]:
+        self,
+        name: t.Optional[str] = None,
+        limit: t.Optional[int] = None,
+        offset: t.Optional[int] = None,
+    ) -> ResultT[t.List[models.Group]]:
         """Searches for groups that at least partially match the given
         name.
 
         Args:
             name: The group name to search for.
             limit: The pagination limit.
             offset: The pagination offset.
@@ -113,17 +116,17 @@
 
         return result.Ok(self._serializer.deserialize_group_details(data))
 
     async def create_group(
         self,
         name: str,
         *members: models.GroupMemberFragment,
-        clan_chat: str | None = None,
-        description: str | None = None,
-        homeworld: int | None = None,
+        clan_chat: t.Optional[str] = None,
+        description: t.Optional[str] = None,
+        homeworld: t.Optional[int] = None,
     ) -> ResultT[models.GroupDetail]:
         """Creates a new group.
 
         Args:
             name: The name for the group.
 
             *members: The optional members to add to the group.
@@ -178,19 +181,19 @@
         return result.Ok(group)
 
     async def edit_group(
         self,
         id: int,
         verification_code: str,
         *,
-        name: str | None = None,
-        members: t.Iterable[models.GroupMemberFragment] | None = None,
-        clan_chat: str | None = None,
-        description: str | None = None,
-        homeworld: int | None = None,
+        name: t.Optional[str] = None,
+        members: t.Optional[t.Iterable[models.GroupMemberFragment]] = None,
+        clan_chat: t.Optional[str] = None,
+        description: t.Optional[str] = None,
+        homeworld: t.Optional[int] = None,
     ) -> ResultT[models.GroupDetail]:
         """Edits an existing group.
 
         Args:
             id: The ID of the group.
 
             verification_code: The group verification code.
@@ -485,16 +488,16 @@
 
         if "players are being updated" in data.message:
             return result.Ok(models.HttpSuccessResponse(data.status, data.message))
 
         return result.Err(data)
 
     async def get_competitions(
-        self, id: int, *, limit: int | None = None, offset: int | None = None
-    ) -> ResultT[list[models.Competition]]:
+        self, id: int, *, limit: t.Optional[int] = None, offset: t.Optional[int] = None
+    ) -> ResultT[t.List[models.Competition]]:
         """Gets competitions for a given group.
 
         Args:
             id: The ID of the group.
 
         Keyword Args:
             limit: The optional pagination limit. Defaults to `None`.
@@ -527,20 +530,20 @@
         return result.Ok([self._serializer.deserialize_competition(c) for c in data])
 
     async def get_gains(
         self,
         id: int,
         metric: enums.Metric,
         *,
-        period: enums.Period | None = None,
-        start_date: datetime | None = None,
-        end_date: datetime | None = None,
-        limit: int | None = None,
-        offset: int | None = None,
-    ) -> ResultT[list[models.DeltaLeaderboardEntry]]:
+        period: t.Optional[enums.Period] = None,
+        start_date: t.Optional[datetime] = None,
+        end_date: t.Optional[datetime] = None,
+        limit: t.Optional[int] = None,
+        offset: t.Optional[int] = None,
+    ) -> ResultT[t.List[models.DeltaLeaderboardEntry]]:
         """Gets the gains for a group over a particular time frame.
 
         Args:
             id: The ID of the group.
 
             metric: The metric to filter on.
 
@@ -598,17 +601,17 @@
 
         return result.Ok([self._serializer.deserialize_delta_leaderboard_entry(d) for d in data])
 
     async def get_achievements(
         self,
         id: int,
         *,
-        limit: int | None = None,
-        offset: int | None = None,
-    ) -> ResultT[list[models.Achievement]]:
+        limit: t.Optional[int] = None,
+        offset: t.Optional[int] = None,
+    ) -> ResultT[t.List[models.Achievement]]:
         """Gets the achievements for the group.
 
         Args:
             id: The ID of the group.
 
         Keyword Args:
             limit: The optional pagination limit. Defaults to `None`.
@@ -642,17 +645,17 @@
 
     async def get_records(
         self,
         id: int,
         metric: enums.Metric,
         period: enums.Period,
         *,
-        limit: int | None = None,
-        offset: int | None = None,
-    ) -> ResultT[list[models.RecordLeaderboardEntry]]:
+        limit: t.Optional[int] = None,
+        offset: t.Optional[int] = None,
+    ) -> ResultT[t.List[models.RecordLeaderboardEntry]]:
         """Gets the records held by players in the group.
 
         Args:
             id: The ID of the group.
 
             metric: The metric to filter on.
 
@@ -697,17 +700,17 @@
         return result.Ok([self._serializer.deserialize_record_leaderboard_entry(a) for a in data])
 
     async def get_hiscores(
         self,
         id: int,
         metric: enums.Metric,
         *,
-        limit: int | None = None,
-        offset: int | None = None,
-    ) -> ResultT[list[models.GroupHiscoresEntry]]:
+        limit: t.Optional[int] = None,
+        offset: t.Optional[int] = None,
+    ) -> ResultT[t.List[models.GroupHiscoresEntry]]:
         """Gets the hiscores for the group.
 
         Args:
             id: The ID of the group.
 
             metric: The metric to filter on.
 
@@ -740,16 +743,16 @@
 
         if isinstance(data, models.HttpErrorResponse):
             return result.Err(data)
 
         return result.Ok([self._serializer.deserialize_group_hiscores_entry(h) for h in data])
 
     async def get_name_changes(
-        self, id: int, *, limit: int | None = None, offset: int | None = None
-    ) -> ResultT[list[models.NameChange]]:
+        self, id: int, *, limit: t.Optional[int] = None, offset: t.Optional[int] = None
+    ) -> ResultT[t.List[models.NameChange]]:
         """Gets the past name changes for the group.
 
         Args:
             id: The ID of the group.
 
         Keyword Args:
             limit: The optional pagination limit. Defaults to `None`.
```

### Comparing `wom_py-0.3.3/wom/services/http.py` & `wom_py-0.4.0/wom/services/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,17 +47,17 @@
         api_base_url: The optional api base url to use.
     """
 
     __slots__ = ("_base_url", "_headers", "_method_mapping", "_session")
 
     def __init__(
         self,
-        api_key: str | None,
-        user_agent: str | None,
-        api_base_url: str | None,
+        api_key: t.Optional[str],
+        user_agent: t.Optional[str],
+        api_base_url: t.Optional[str],
     ) -> None:
         self._headers = {
             "x-user-agent": (
                 f"{constants.USER_AGENT_BASE} {user_agent}"
                 if user_agent
                 else constants.DEFAULT_USER_AGENT
             )
@@ -149,15 +149,15 @@
             await self._session.close()
 
     async def fetch(
         self,
         route: routes.CompiledRoute,
         _: t.Type[T],
         *,
-        payload: dict[str, t.Any] | None = None,
+        payload: t.Optional[t.Dict[str, t.Any]] = None,
     ) -> T | models.HttpErrorResponse:
         """Fetches the given route.
 
         Args:
             route: The route to make the request to.
 
             _: The type expected to be returned.
```

### Comparing `wom_py-0.3.3/wom/services/names.py` & `wom_py-0.4.0/wom/services/names.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,20 +38,20 @@
 class NameChangeService(BaseService):
     """Handles endpoints related to name changes."""
 
     __slots__ = ()
 
     async def search_name_changes(
         self,
-        username: str | None = None,
+        username: t.Optional[str] = None,
         *,
-        status: models.NameChangeStatus | None = None,
-        limit: int | None = None,
-        offset: int | None = None,
-    ) -> ResultT[list[models.NameChange]]:
+        status: t.Optional[models.NameChangeStatus] = None,
+        limit: t.Optional[int] = None,
+        offset: t.Optional[int] = None,
+    ) -> ResultT[t.List[models.NameChange]]:
         """Searches for name changes.
 
         Args:
             username: The optional username to search for.
 
         Keyword Args:
             status: The optional name change status to filter on.
@@ -118,36 +118,7 @@
         route = routes.SUBMIT_NAME_CHANGE.compile()
         data = await self._http.fetch(route, self._dict, payload=payload)
 
         if isinstance(data, models.HttpErrorResponse):
             return result.Err(data)
 
         return result.Ok(self._serializer.deserialize_name_change(data))
-
-    async def get_name_change_details(self, id: int) -> ResultT[models.NameChangeDetail]:
-        """Gets the details for an existing name change.
-
-        Args:
-            id: The ID of the name change.
-
-        Returns:
-            A [`Result`][wom.Result] containing the name change details.
-
-        ??? example
-
-            ```py
-            import wom
-
-            client = wom.Client(...)
-
-            await client.start()
-
-            result = await client.names.get_name_change_details(123)
-            ```
-        """
-        route = routes.NAME_CHANGE_DETAILS.compile(id)
-        data = await self._http.fetch(route, self._dict)
-
-        if isinstance(data, models.HttpErrorResponse):
-            return result.Err(data)
-
-        return result.Ok(self._serializer.deserialize_name_change_detail(data))
```

### Comparing `wom_py-0.3.3/wom/services/players.py` & `wom_py-0.4.0/wom/services/players.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 
 class PlayerService(BaseService):
     """Handles endpoints related to players."""
 
     __slots__ = ()
 
     async def search_players(
-        self, username: str, *, limit: int | None = None, offset: int | None = None
-    ) -> ResultT[list[models.Player]]:
+        self, username: str, *, limit: t.Optional[int] = None, offset: t.Optional[int] = None
+    ) -> ResultT[t.List[models.Player]]:
         """Searches for a player by partial username.
 
         Args:
             username: The username to search for.
 
         Keyword Args:
             limit: The maximum number of paginated items to receive.
@@ -196,15 +196,15 @@
         data = await self._http.fetch(route, self._dict)
 
         if isinstance(data, models.HttpErrorResponse):
             return result.Err(data)
 
         return result.Ok(self._serializer.deserialize_player_details(data))
 
-    async def get_achievements(self, username: str) -> ResultT[list[models.Achievement]]:
+    async def get_achievements(self, username: str) -> ResultT[t.List[models.Achievement]]:
         """Gets the achievements for a given player.
 
         Args:
             username: The username to get the achievements for.
 
         Returns:
             A [`Result`][wom.Result] containing the list of player
@@ -228,15 +228,15 @@
         if isinstance(data, models.HttpErrorResponse):
             return result.Err(data)
 
         return result.Ok([self._serializer.deserialize_achievement(a) for a in data])
 
     async def get_achievement_progress(
         self, username: str
-    ) -> ResultT[list[models.PlayerAchievementProgress]]:
+    ) -> ResultT[t.List[models.PlayerAchievementProgress]]:
         """Gets the progress towards achievements for a given player.
 
         Args:
             username: The username to get the achievement progress for.
 
         Returns:
             A [`Result`][wom.Result] containing the list of player
@@ -264,18 +264,18 @@
             [self._serializer.deserialize_player_achievement_progress(p) for p in data]
         )
 
     async def get_competition_participations(
         self,
         username: str,
         *,
-        limit: int | None = None,
-        offset: int | None = None,
-        status: models.CompetitionStatus | None = None,
-    ) -> ResultT[list[models.PlayerParticipation]]:
+        limit: t.Optional[int] = None,
+        offset: t.Optional[int] = None,
+        status: t.Optional[models.CompetitionStatus] = None,
+    ) -> ResultT[t.List[models.PlayerParticipation]]:
         """Gets the competition participations for a given player.
 
         Args:
             username: The username to get the participations for.
 
         Keyword Args:
             limit: The maximum number of paginated items to receive.
@@ -316,15 +316,15 @@
 
         return result.Ok([self._serializer.deserialize_player_participation(p) for p in data])
 
     async def get_competition_standings(
         self,
         username: str,
         status: models.CompetitionStatus,
-    ) -> ResultT[list[models.PlayerCompetitionStanding]]:
+    ) -> ResultT[t.List[models.PlayerCompetitionStanding]]:
         """Gets the competition standings for a given player.
 
         Args:
             username: The username to get the standings for.
 
             status: The competition status to get standings for.
 
@@ -354,16 +354,16 @@
             return result.Err(data)
 
         return result.Ok(
             [self._serializer.deserialize_player_competition_standing(s) for s in data]
         )
 
     async def get_group_memberships(
-        self, username: str, *, limit: int | None = None, offset: int | None = None
-    ) -> ResultT[list[models.PlayerMembership]]:
+        self, username: str, *, limit: t.Optional[int] = None, offset: t.Optional[int] = None
+    ) -> ResultT[t.List[models.PlayerMembership]]:
         """Gets the group memberships for the given player.
 
         Args:
             username: The username to get the memberships for.
 
         Keyword Args:
             limit: The maximum number of paginated items to receive.
@@ -399,17 +399,17 @@
 
         return result.Ok([self._serializer.deserialize_player_membership(m) for m in data])
 
     async def get_gains(
         self,
         username: str,
         *,
-        period: enums.Period | None = None,
-        start_date: datetime | None = None,
-        end_date: datetime | None = None,
+        period: t.Optional[enums.Period] = None,
+        start_date: t.Optional[datetime] = None,
+        end_date: t.Optional[datetime] = None,
     ) -> ResultT[models.PlayerGains]:
         """Gets the gains made by this player over the given time span.
 
         Args:
             username: The username to get the gains for.
 
         Keyword Args:
@@ -458,17 +458,17 @@
 
         return result.Ok(self._serializer.deserialize_player_gains(data))
 
     async def get_records(
         self,
         username: str,
         *,
-        period: enums.Period | None = None,
-        metric: enums.Metric | None = None,
-    ) -> ResultT[list[models.Record]]:
+        period: t.Optional[enums.Period] = None,
+        metric: t.Optional[enums.Metric] = None,
+    ) -> ResultT[t.List[models.Record]]:
         """Gets the records held by this player.
 
         Args:
             username: The username to get the gains for.
 
         Keyword Args:
             period: The optional period of time to get gains for.
@@ -507,18 +507,18 @@
 
         return result.Ok([self._serializer.deserialize_record(r) for r in data])
 
     async def get_snapshots(
         self,
         username: str,
         *,
-        period: enums.Period | None = None,
-        start_date: datetime | None = None,
-        end_date: datetime | None = None,
-    ) -> ResultT[list[models.Snapshot]]:
+        period: t.Optional[enums.Period] = None,
+        start_date: t.Optional[datetime] = None,
+        end_date: t.Optional[datetime] = None,
+    ) -> ResultT[t.List[models.Snapshot]]:
         """Gets the snapshots for the player.
 
         Args:
             username: The username to get the snapshots for.
 
         Keyword Args:
             period: The optional period of time to get snapshots for.
@@ -562,15 +562,15 @@
         data = await self._http.fetch(route, self._list)
 
         if isinstance(data, models.HttpErrorResponse):
             return result.Err(data)
 
         return result.Ok([self._serializer.deserialize_snapshot(s) for s in data])
 
-    async def get_name_changes(self, username: str) -> ResultT[list[models.NameChange]]:
+    async def get_name_changes(self, username: str) -> ResultT[t.List[models.NameChange]]:
         """Gets the name changes for the player.
 
         Args:
             username: The username to get the name changes for.
 
         Returns:
             A [`Result`][wom.Result] containing the list of name changes.
```

### Comparing `wom_py-0.3.3/wom/services/records.py` & `wom_py-0.4.0/wom/services/records.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,18 +42,18 @@
     __slots__ = ()
 
     async def get_global_record_leaderboards(
         self,
         metric: enums.Metric,
         period: enums.Period,
         *,
-        player_type: models.PlayerType | None = None,
-        player_build: models.PlayerBuild | None = None,
-        country: models.Country | None = None,
-    ) -> ResultT[list[models.RecordLeaderboardEntry]]:
+        player_type: t.Optional[models.PlayerType] = None,
+        player_build: t.Optional[models.PlayerBuild] = None,
+        country: t.Optional[models.Country] = None,
+    ) -> ResultT[t.List[models.RecordLeaderboardEntry]]:
         """Gets the global record leaderboards.
 
         Args:
             metric: The metric to filter on.
 
             period: The period of time to filter on.
```

### Comparing `wom_py-0.3.3/PKG-INFO` & `wom_py-0.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 776f 6d2d  : 2.1.Name: wom-
-00000020: 7079 0a56 6572 7369 6f6e 3a20 302e 332e  py.Version: 0.3.
-00000030: 330a 5375 6d6d 6172 793a 2041 6e20 6173  3.Summary: An as
+00000020: 7079 0a56 6572 7369 6f6e 3a20 302e 342e  py.Version: 0.4.
+00000030: 300a 5375 6d6d 6172 793a 2041 6e20 6173  0.Summary: An as
 00000040: 796e 6368 726f 6e6f 7573 2077 7261 7070  ynchronous wrapp
 00000050: 6572 2066 6f72 2074 6865 2057 6973 6520  er for the Wise 
 00000060: 4f6c 6420 4d61 6e20 4150 492e 0a48 6f6d  Old Man API..Hom
 00000070: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
 00000080: 6769 7468 7562 2e63 6f6d 2f4a 6f6e 7873  github.com/Jonxs
 00000090: 6c61 7973 2f77 6f6d 2e70 790a 4c69 6365  lays/wom.py.Lice
 000000a0: 6e73 653a 204d 4954 0a41 7574 686f 723a  nse: MIT.Author:
@@ -76,129 +76,177 @@
 000004b0: 7468 7562 2e69 6f2f 776f 6d2e 7079 0a50  thub.io/wom.py.P
 000004c0: 726f 6a65 6374 2d55 524c 3a20 5265 706f  roject-URL: Repo
 000004d0: 7369 746f 7279 2c20 6874 7470 733a 2f2f  sitory, https://
 000004e0: 6769 7468 7562 2e63 6f6d 2f4a 6f6e 7873  github.com/Jonxs
 000004f0: 6c61 7973 2f77 6f6d 2e70 790a 4465 7363  lays/wom.py.Desc
 00000500: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
 00000510: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-00000520: 6f77 6e0a 0a23 2077 6f6d 2e70 790a 0a41  own..# wom.py..A
-00000530: 6e20 6173 796e 6368 726f 6e6f 7573 2077  n asynchronous w
-00000540: 7261 7070 6572 2066 6f72 2074 6865 205b  rapper for the [
-00000550: 5769 7365 204f 6c64 204d 616e 2041 5049  Wise Old Man API
-00000560: 5d28 6874 7470 733a 2f2f 646f 6373 2e77  ](https://docs.w
-00000570: 6973 656f 6c64 6d61 6e2e 6e65 742f 292e  iseoldman.net/).
-00000580: 0a0a 5468 6520 6c69 6272 6172 7920 6169  ..The library ai
-00000590: 6d73 2074 6f20 6d61 6b65 2069 7420 6561  ms to make it ea
-000005a0: 7379 2074 6f20 696e 7465 7261 6374 2077  sy to interact w
-000005b0: 6974 6820 7468 6520 5769 7365 204f 6c64  ith the Wise Old
-000005c0: 204d 616e 2041 5049 2062 790a 7072 6f76   Man API by.prov
-000005d0: 6964 696e 6720 7365 7276 6963 6520 6d65  iding service me
-000005e0: 7468 6f64 7320 666f 7220 616c 6c20 6176  thods for all av
-000005f0: 6169 6c61 626c 6520 656e 6470 6f69 6e74  ailable endpoint
-00000600: 7320 616e 6420 6d6f 6465 6c20 636c 6173  s and model clas
-00000610: 7365 730a 666f 7220 6461 7461 2063 6f6e  ses.for data con
-00000620: 7369 7374 656e 6379 2e0a 0a50 7974 686f  sistency...Pytho
-00000630: 6e20 7665 7273 696f 6e20 332e 3820 6f72  n version 3.8 or
-00000640: 2067 7265 6174 6572 2069 7320 7265 7175   greater is requ
-00000650: 6972 6564 2074 6f20 7573 6520 776f 6d2e  ired to use wom.
-00000660: 7079 2e0a 0a23 2320 4469 7363 6c61 696d  py...## Disclaim
-00000670: 6572 0a0a 5468 6520 6c69 6272 6172 7920  er..The library 
-00000680: 6973 2073 7469 6c6c 2069 6e20 4265 7461  is still in Beta
-00000690: 2c20 616e 6420 6173 2073 7563 6820 6665  , and as such fe
-000006a0: 6174 7572 6573 206f 7220 7075 626c 6963  atures or public
-000006b0: 2069 6e74 6572 6661 6365 730a 6d61 7920   interfaces.may 
-000006c0: 6368 616e 6765 2061 7420 616e 7920 7469  change at any ti
-000006d0: 6d65 2e20 5468 616e 6b73 2066 6f72 2063  me. Thanks for c
-000006e0: 6865 636b 696e 6720 6f75 7420 7468 6520  hecking out the 
-000006f0: 7072 6f6a 6563 7421 0a0a 2323 2044 6f63  project!..## Doc
-00000700: 756d 656e 7461 7469 6f6e 0a0a 2d20 5b53  umentation..- [S
-00000710: 7461 626c 655d 2868 7474 7073 3a2f 2f6a  table](https://j
-00000720: 6f6e 7873 6c61 7973 2e67 6974 6875 622e  onxslays.github.
-00000730: 696f 2f77 6f6d 2e70 792f 290a 2d20 5b44  io/wom.py/).- [D
-00000740: 6576 656c 6f70 6d65 6e74 5d28 6874 7470  evelopment](http
-00000750: 733a 2f2f 6a6f 6e78 736c 6179 732e 6769  s://jonxslays.gi
-00000760: 7468 7562 2e69 6f2f 776f 6d2e 7079 2f64  thub.io/wom.py/d
-00000770: 6576 2f29 0a0a 2323 2049 6e73 7461 6c6c  ev/)..## Install
-00000780: 6174 696f 6e0a 0a23 2323 2053 7461 626c  ation..### Stabl
-00000790: 650a 0a60 6060 7368 0a70 6970 2069 6e73  e..```sh.pip ins
-000007a0: 7461 6c6c 202d 5520 776f 6d2e 7079 0a60  tall -U wom.py.`
-000007b0: 6060 0a0a 2323 2320 4465 7665 6c6f 706d  ``..### Developm
-000007c0: 656e 740a 0a60 6060 7368 0a70 6970 2069  ent..```sh.pip i
-000007d0: 6e73 7461 6c6c 202d 5520 6769 742b 6874  nstall -U git+ht
-000007e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000007f0: 2f4a 6f6e 7873 6c61 7973 2f77 6f6d 2e70  /Jonxslays/wom.p
-00000800: 790a 6060 600a 0a46 6f72 206d 6f72 6520  y.```..For more 
-00000810: 696e 666f 726d 6174 696f 6e20 6f6e 2075  information on u
-00000820: 7369 6e67 2060 7069 7060 2c20 6368 6563  sing `pip`, chec
-00000830: 6b20 6f75 7420 7468 6520 5b70 6970 2064  k out the [pip d
-00000840: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-00000850: 7470 733a 2f2f 7069 702e 7079 7061 2e69  tps://pip.pypa.i
-00000860: 6f2f 656e 2f73 7461 626c 652f 292e 0a0a  o/en/stable/)...
-00000870: 2323 2050 726f 626c 656d 730a 0a49 6620  ## Problems..If 
-00000880: 796f 7527 7265 2065 7870 6572 6965 6e63  you're experienc
-00000890: 696e 6720 6120 7072 6f62 6c65 6d20 7769  ing a problem wi
-000008a0: 7468 2074 6865 206c 6962 7261 7279 2c20  th the library, 
-000008b0: 706c 6561 7365 206f 7065 6e20 616e 2069  please open an i
-000008c0: 7373 7565 0a5b 6865 7265 5d28 6874 7470  ssue.[here](http
-000008d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4a  s://github.com/J
-000008e0: 6f6e 7873 6c61 7973 2f77 6f6d 2e70 792f  onxslays/wom.py/
-000008f0: 6973 7375 6573 292c 2061 6674 6572 2066  issues), after f
-00000900: 6972 7374 2063 6f6e 6669 726d 696e 670a  irst confirming.
-00000910: 6120 7369 6d69 6c61 7220 6973 7375 6520  a similar issue 
-00000920: 7761 7320 6e6f 7420 616c 7265 6164 7920  was not already 
-00000930: 6372 6561 7465 642e 0a0a 2323 2057 6861  created...## Wha
-00000940: 7420 6973 2057 6973 6520 4f6c 6420 4d61  t is Wise Old Ma
-00000950: 6e0a 0a57 6973 6520 4f6c 6420 4d61 6e20  n..Wise Old Man 
-00000960: 6973 2061 6e20 6f70 656e 2073 6f75 7263  is an open sourc
-00000970: 6520 4f6c 6473 6368 6f6f 6c20 5275 6e65  e Oldschool Rune
-00000980: 7363 6170 6520 706c 6179 6572 2070 726f  scape player pro
-00000990: 6772 6573 7320 7472 6163 6b65 722e 0a0a  gress tracker...
-000009a0: 4966 2079 6f75 2772 6520 696e 7465 7265  If you're intere
-000009b0: 7374 6564 2069 6e20 6c65 6172 6e69 6e67  sted in learning
-000009c0: 206d 6f72 6520 6162 6f75 7420 7468 6520   more about the 
-000009d0: 5769 7365 204f 6c64 204d 616e 2070 726f  Wise Old Man pro
-000009e0: 6a65 6374 2c20 636f 6e73 6964 6572 2063  ject, consider c
-000009f0: 6865 636b 696e 6720 6f75 7420 616e 7920  hecking out any 
-00000a00: 6f66 2074 6865 7365 206c 696e 6b73 3a0a  of these links:.
-00000a10: 0a2d 205b 5765 6273 6974 655d 2868 7474  .- [Website](htt
-00000a20: 7073 3a2f 2f77 6973 656f 6c64 6d61 6e2e  ps://wiseoldman.
-00000a30: 6e65 742f 290a 2d20 5b41 5049 2064 6f63  net/).- [API doc
-00000a40: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-00000a50: 733a 2f2f 646f 6373 2e77 6973 656f 6c64  s://docs.wiseold
-00000a60: 6d61 6e2e 6e65 742f 290a 2d20 5b47 6974  man.net/).- [Git
-00000a70: 6875 6220 7265 706f 7369 746f 7279 5d28  hub repository](
-00000a80: 6874 7470 733a 2f2f 7769 7365 6f6c 646d  https://wiseoldm
-00000a90: 616e 2e6e 6574 2f67 6974 6875 6229 0a2d  an.net/github).-
-00000aa0: 205b 4469 7363 6f72 6420 636f 6d6d 756e   [Discord commun
-00000ab0: 6974 795d 2868 7474 7073 3a2f 2f77 6973  ity](https://wis
-00000ac0: 656f 6c64 6d61 6e2e 6e65 742f 6469 7363  eoldman.net/disc
-00000ad0: 6f72 6429 0a2d 205b 5375 7070 6f72 7420  ord).- [Support 
-00000ae0: 7468 6520 6465 7665 6c6f 7065 7273 206f  the developers o
-00000af0: 6e20 5061 7472 656f 6e5d 2868 7474 7073  n Patreon](https
-00000b00: 3a2f 2f77 6973 656f 6c64 6d61 6e2e 6e65  ://wiseoldman.ne
-00000b10: 742f 7061 7472 656f 6e29 0a0a 536f 6d65  t/patreon)..Some
-00000b20: 206f 6620 7468 6520 706f 7075 6c61 7220   of the popular 
-00000b30: 6665 6174 7572 6573 2069 6e63 6c75 6465  features include
-00000b40: 3a0a 0a2d 2045 7870 6572 6965 6e63 6520  :..- Experience 
-00000b50: 7472 6163 6b69 6e67 0a2d 2042 6f73 7320  tracking.- Boss 
-00000b60: 6b69 6c6c 636f 756e 7473 0a2d 2050 6c61  killcounts.- Pla
-00000b70: 7965 7220 6163 6869 6576 656d 656e 7473  yer achievements
-00000b80: 0a2d 2047 726f 7570 2063 6f6d 7065 7469  .- Group competi
-00000b90: 7469 6f6e 730a 2d20 476c 6f62 616c 206c  tions.- Global l
-00000ba0: 6561 6465 7262 6f61 7264 730a 2d20 4120  eaderboards.- A 
-00000bb0: 6469 7363 6f72 6420 626f 7420 666f 7220  discord bot for 
-00000bc0: 696e 7465 7261 6374 696e 6720 7769 7468  interacting with
-00000bd0: 2074 6865 2041 5049 0a0a 2323 2043 6f6e   the API..## Con
-00000be0: 7472 6962 7574 696e 670a 0a77 6f6d 2e70  tributing..wom.p
-00000bf0: 7920 6973 206f 7065 6e20 746f 2063 6f6e  y is open to con
-00000c00: 7472 6962 7574 696f 6e73 2e0a 0a43 6f6d  tributions...Com
-00000c10: 6520 6261 636b 2073 6f6f 6ee2 84a2 206f  e back soon... o
-00000c20: 6e63 6520 4927 7665 2077 7269 7474 656e  nce I've written
-00000c30: 2074 6865 2063 6f6e 7472 6962 7574 696e   the contributin
-00000c40: 6720 6775 6964 652e 0a0a 2323 204c 6963  g guide...## Lic
-00000c50: 656e 7365 0a0a 776f 6d2e 7079 2069 7320  ense..wom.py is 
-00000c60: 6c69 6365 6e73 6564 2075 6e64 6572 2074  licensed under t
-00000c70: 6865 0a5b 4d49 5420 4c69 6365 6e73 655d  he.[MIT License]
-00000c80: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000c90: 636f 6d2f 4a6f 6e78 736c 6179 732f 776f  com/Jonxslays/wo
-00000ca0: 6d2e 7079 2f62 6c6f 622f 6d61 7374 6572  m.py/blob/master
-00000cb0: 2f4c 4943 454e 5345 292e 0a0a            /LICENSE)...
+00000520: 6f77 6e0a 0a3c 6469 7620 616c 6967 6e3d  own..<div align=
+00000530: 2263 656e 7465 7222 3e0a 2020 2020 3c68  "center">.    <h
+00000540: 313e 776f 6d2e 7079 3c2f 6831 3e0a 2020  1>wom.py</h1>.  
+00000550: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000560: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000570: 6563 742f 776f 6d2e 7079 223e 3c69 6d67  ect/wom.py"><img
+00000580: 2068 6569 6768 743d 2232 3022 2061 6c74   height="20" alt
+00000590: 3d22 5374 6162 6c65 2076 6572 7369 6f6e  ="Stable version
+000005a0: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+000005b0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000005c0: 7069 2f76 2f77 6f6d 2e70 793f 6c61 6265  pi/v/wom.py?labe
+000005d0: 6c3d 7374 6162 6c65 266c 6f67 6f3d 7079  l=stable&logo=py
+000005e0: 7069 223e 3c2f 613e 0a20 2020 203c 6120  pi"></a>.    <a 
+000005f0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000600: 7468 7562 2e63 6f6d 2f4a 6f6e 7873 6c61  thub.com/Jonxsla
+00000610: 7973 2f77 6f6d 2e70 792f 626c 6f62 2f6d  ys/wom.py/blob/m
+00000620: 6173 7465 722f 4c49 4345 4e53 4522 3e3c  aster/LICENSE"><
+00000630: 696d 6720 6865 6967 6874 3d22 3230 2220  img height="20" 
+00000640: 616c 743d 224c 6963 656e 7365 2220 7372  alt="License" sr
+00000650: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000660: 6869 656c 6473 2e69 6f2f 7079 7069 2f6c  hields.io/pypi/l
+00000670: 2f77 6f6d 2d70 793f 6c61 6265 6c3d 6c69  /wom-py?label=li
+00000680: 6365 6e73 6522 3e3c 2f61 3e0a 2020 2020  cense"></a>.    
+00000690: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000006a0: 2f70 7974 686f 6e2e 6f72 6722 3e3c 696d  /python.org"><im
+000006b0: 6720 6865 6967 6874 3d22 3230 2220 616c  g height="20" al
+000006c0: 743d 2250 7974 686f 6e20 7665 7273 696f  t="Python versio
+000006d0: 6e73 2220 7372 633d 2268 7474 7073 3a2f  ns" src="https:/
+000006e0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000006f0: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
+00000700: 776f 6d2d 7079 3f6c 6162 656c 3d70 7974  wom-py?label=pyt
+00000710: 686f 6e26 6c6f 676f 3d70 7974 686f 6e22  hon&logo=python"
+00000720: 3e3c 2f61 3e0a 2020 2020 3c61 2068 7265  ></a>.    <a hre
+00000730: 663d 2268 7474 7073 3a2f 2f63 6f64 6563  f="https://codec
+00000740: 6c69 6d61 7465 2e63 6f6d 2f67 6974 6875  limate.com/githu
+00000750: 622f 4a6f 6e78 736c 6179 732f 776f 6d2e  b/Jonxslays/wom.
+00000760: 7079 2f6d 6169 6e74 6169 6e61 6269 6c69  py/maintainabili
+00000770: 7479 223e 3c69 6d67 2068 6569 6768 743d  ty"><img height=
+00000780: 2232 3022 2061 6c74 3d22 4d61 696e 7461  "20" alt="Mainta
+00000790: 696e 6162 696c 6974 7922 2073 7263 3d22  inability" src="
+000007a0: 6874 7470 733a 2f2f 6170 692e 636f 6465  https://api.code
+000007b0: 636c 696d 6174 652e 636f 6d2f 7631 2f62  climate.com/v1/b
+000007c0: 6164 6765 732f 3336 3766 6236 3637 6566  adges/367fb667ef
+000007d0: 3337 3230 3634 6665 3561 2f6d 6169 6e74  372064fe5a/maint
+000007e0: 6169 6e61 6269 6c69 7479 2220 2f3e 3c2f  ainability" /></
+000007f0: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000800: 6874 7470 733a 2f2f 636f 6465 636c 696d  https://codeclim
+00000810: 6174 652e 636f 6d2f 6769 7468 7562 2f4a  ate.com/github/J
+00000820: 6f6e 7873 6c61 7973 2f77 6f6d 2e70 792f  onxslays/wom.py/
+00000830: 7465 7374 5f63 6f76 6572 6167 6522 3e3c  test_coverage"><
+00000840: 696d 6720 6865 6967 6874 3d22 3230 2220  img height="20" 
+00000850: 616c 743d 2243 6f76 6572 6167 6522 2073  alt="Coverage" s
+00000860: 7263 3d22 6874 7470 733a 2f2f 6170 692e  rc="https://api.
+00000870: 636f 6465 636c 696d 6174 652e 636f 6d2f  codeclimate.com/
+00000880: 7631 2f62 6164 6765 732f 3336 3766 6236  v1/badges/367fb6
+00000890: 3637 6566 3337 3230 3634 6665 3561 2f74  67ef372064fe5a/t
+000008a0: 6573 745f 636f 7665 7261 6765 2220 2f3e  est_coverage" />
+000008b0: 3c2f 613e 0a3c 2f64 6976 3e0a 0a41 6e20  </a>.</div>..An 
+000008c0: 6173 796e 6368 726f 6e6f 7573 2077 7261  asynchronous wra
+000008d0: 7070 6572 2066 6f72 2074 6865 205b 5769  pper for the [Wi
+000008e0: 7365 204f 6c64 204d 616e 2041 5049 5d28  se Old Man API](
+000008f0: 6874 7470 733a 2f2f 646f 6373 2e77 6973  https://docs.wis
+00000900: 656f 6c64 6d61 6e2e 6e65 742f 292e 0a0a  eoldman.net/)...
+00000910: 5468 6520 6c69 6272 6172 7920 6169 6d73  The library aims
+00000920: 2074 6f20 6d61 6b65 2069 7420 6561 7379   to make it easy
+00000930: 2074 6f20 696e 7465 7261 6374 2077 6974   to interact wit
+00000940: 6820 7468 6520 5769 7365 204f 6c64 204d  h the Wise Old M
+00000950: 616e 2041 5049 2062 790a 7072 6f76 6964  an API by.provid
+00000960: 696e 6720 7365 7276 6963 6520 6d65 7468  ing service meth
+00000970: 6f64 7320 6d61 7463 6869 6e67 2061 6c6c  ods matching all
+00000980: 2061 7661 696c 6162 6c65 2065 6e64 706f   available endpo
+00000990: 696e 7473 2061 6e64 206d 6f64 656c 2063  ints and model c
+000009a0: 6c61 7373 6573 0a66 6f72 2064 6174 6120  lasses.for data 
+000009b0: 636f 6e73 6973 7465 6e63 792e 0a0a 2323  consistency...##
+000009c0: 2044 6f63 756d 656e 7461 7469 6f6e 0a0a   Documentation..
+000009d0: 2d20 5b53 7461 626c 655d 2868 7474 7073  - [Stable](https
+000009e0: 3a2f 2f6a 6f6e 7873 6c61 7973 2e67 6974  ://jonxslays.git
+000009f0: 6875 622e 696f 2f77 6f6d 2e70 792f 290a  hub.io/wom.py/).
+00000a00: 2d20 5b44 6576 656c 6f70 6d65 6e74 5d28  - [Development](
+00000a10: 6874 7470 733a 2f2f 6a6f 6e78 736c 6179  https://jonxslay
+00000a20: 732e 6769 7468 7562 2e69 6f2f 776f 6d2e  s.github.io/wom.
+00000a30: 7079 2f64 6576 2f29 0a0a 2323 2049 6e73  py/dev/)..## Ins
+00000a40: 7461 6c6c 6174 696f 6e0a 0a2a 2a50 7974  tallation..**Pyt
+00000a50: 686f 6e20 7665 7273 696f 6e20 332e 3820  hon version 3.8 
+00000a60: 6f72 2067 7265 6174 6572 2069 7320 7265  or greater is re
+00000a70: 7175 6972 6564 2074 6f20 7573 6520 776f  quired to use wo
+00000a80: 6d2e 7079 2e2a 2a0a 0a23 2323 2053 7461  m.py.**..### Sta
+00000a90: 626c 650a 0a60 6060 7368 0a70 6970 2069  ble..```sh.pip i
+00000aa0: 6e73 7461 6c6c 202d 5520 776f 6d2e 7079  nstall -U wom.py
+00000ab0: 0a60 6060 0a0a 2323 2320 4465 7665 6c6f  .```..### Develo
+00000ac0: 706d 656e 740a 0a60 6060 7368 0a70 6970  pment..```sh.pip
+00000ad0: 2069 6e73 7461 6c6c 202d 5520 6769 742b   install -U git+
+00000ae0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000af0: 6f6d 2f4a 6f6e 7873 6c61 7973 2f77 6f6d  om/Jonxslays/wom
+00000b00: 2e70 790a 6060 600a 0a46 6f72 206d 6f72  .py.```..For mor
+00000b10: 6520 696e 666f 726d 6174 696f 6e20 6f6e  e information on
+00000b20: 2075 7369 6e67 2060 7069 7060 2c20 6368   using `pip`, ch
+00000b30: 6563 6b20 6f75 7420 7468 6520 5b70 6970  eck out the [pip
+00000b40: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
+00000b50: 6874 7470 733a 2f2f 7069 702e 7079 7061  https://pip.pypa
+00000b60: 2e69 6f2f 656e 2f73 7461 626c 652f 292e  .io/en/stable/).
+00000b70: 0a0a 2323 2050 726f 626c 656d 730a 0a49  ..## Problems..I
+00000b80: 6620 796f 7527 7265 2065 7870 6572 6965  f you're experie
+00000b90: 6e63 696e 6720 6120 7072 6f62 6c65 6d20  ncing a problem 
+00000ba0: 7769 7468 2074 6865 206c 6962 7261 7279  with the library
+00000bb0: 2c20 706c 6561 7365 206f 7065 6e20 616e  , please open an
+00000bc0: 2069 7373 7565 0a5b 6865 7265 5d28 6874   issue.[here](ht
+00000bd0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000be0: 2f4a 6f6e 7873 6c61 7973 2f77 6f6d 2e70  /Jonxslays/wom.p
+00000bf0: 792f 6973 7375 6573 292c 2061 6674 6572  y/issues), after
+00000c00: 2066 6972 7374 2063 6f6e 6669 726d 696e   first confirmin
+00000c10: 670a 6120 7369 6d69 6c61 7220 6973 7375  g.a similar issu
+00000c20: 6520 7761 7320 6e6f 7420 616c 7265 6164  e was not alread
+00000c30: 7920 6372 6561 7465 642e 0a0a 2323 2057  y created...## W
+00000c40: 6861 7420 6973 2057 6973 6520 4f6c 6420  hat is Wise Old 
+00000c50: 4d61 6e0a 0a57 6973 6520 4f6c 6420 4d61  Man..Wise Old Ma
+00000c60: 6e20 6973 2061 6e20 6f70 656e 2073 6f75  n is an open sou
+00000c70: 7263 6520 4f6c 6473 6368 6f6f 6c20 5275  rce Oldschool Ru
+00000c80: 6e65 7363 6170 6520 706c 6179 6572 2070  nescape player p
+00000c90: 726f 6772 6573 7320 7472 6163 6b65 722e  rogress tracker.
+00000ca0: 0a0a 4966 2079 6f75 2772 6520 696e 7465  ..If you're inte
+00000cb0: 7265 7374 6564 2069 6e20 6c65 6172 6e69  rested in learni
+00000cc0: 6e67 206d 6f72 6520 6162 6f75 7420 7468  ng more about th
+00000cd0: 6520 5769 7365 204f 6c64 204d 616e 2070  e Wise Old Man p
+00000ce0: 726f 6a65 6374 2c20 636f 6e73 6964 6572  roject, consider
+00000cf0: 2063 6865 636b 696e 6720 6f75 7420 616e   checking out an
+00000d00: 7920 6f66 2074 6865 7365 206c 696e 6b73  y of these links
+00000d10: 3a0a 0a2d 205b 5765 6273 6974 655d 2868  :..- [Website](h
+00000d20: 7474 7073 3a2f 2f77 6973 656f 6c64 6d61  ttps://wiseoldma
+00000d30: 6e2e 6e65 742f 290a 2d20 5b41 5049 2064  n.net/).- [API d
+00000d40: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+00000d50: 7470 733a 2f2f 646f 6373 2e77 6973 656f  tps://docs.wiseo
+00000d60: 6c64 6d61 6e2e 6e65 742f 290a 2d20 5b47  ldman.net/).- [G
+00000d70: 6974 6875 6220 7265 706f 7369 746f 7279  ithub repository
+00000d80: 5d28 6874 7470 733a 2f2f 7769 7365 6f6c  ](https://wiseol
+00000d90: 646d 616e 2e6e 6574 2f67 6974 6875 6229  dman.net/github)
+00000da0: 0a2d 205b 4469 7363 6f72 6420 636f 6d6d  .- [Discord comm
+00000db0: 756e 6974 795d 2868 7474 7073 3a2f 2f77  unity](https://w
+00000dc0: 6973 656f 6c64 6d61 6e2e 6e65 742f 6469  iseoldman.net/di
+00000dd0: 7363 6f72 6429 0a2d 205b 5375 7070 6f72  scord).- [Suppor
+00000de0: 7420 7468 6520 6465 7665 6c6f 7065 7273  t the developers
+00000df0: 206f 6e20 5061 7472 656f 6e5d 2868 7474   on Patreon](htt
+00000e00: 7073 3a2f 2f77 6973 656f 6c64 6d61 6e2e  ps://wiseoldman.
+00000e10: 6e65 742f 7061 7472 656f 6e29 0a0a 536f  net/patreon)..So
+00000e20: 6d65 206f 6620 7468 6520 706f 7075 6c61  me of the popula
+00000e30: 7220 6665 6174 7572 6573 2069 6e63 6c75  r features inclu
+00000e40: 6465 3a0a 0a2d 2045 7870 6572 6965 6e63  de:..- Experienc
+00000e50: 6520 7472 6163 6b69 6e67 0a2d 2042 6f73  e tracking.- Bos
+00000e60: 7320 6b69 6c6c 636f 756e 7473 0a2d 2050  s killcounts.- P
+00000e70: 6c61 7965 7220 6163 6869 6576 656d 656e  layer achievemen
+00000e80: 7473 0a2d 2047 726f 7570 2063 6f6d 7065  ts.- Group compe
+00000e90: 7469 7469 6f6e 730a 2d20 476c 6f62 616c  titions.- Global
+00000ea0: 206c 6561 6465 7262 6f61 7264 730a 2d20   leaderboards.- 
+00000eb0: 4120 6469 7363 6f72 6420 626f 7420 666f  A discord bot fo
+00000ec0: 7220 696e 7465 7261 6374 696e 6720 7769  r interacting wi
+00000ed0: 7468 2074 6865 2041 5049 0a0a 2323 2043  th the API..## C
+00000ee0: 6f6e 7472 6962 7574 696e 670a 0a77 6f6d  ontributing..wom
+00000ef0: 2e70 7920 6973 206f 7065 6e20 746f 2063  .py is open to c
+00000f00: 6f6e 7472 6962 7574 696f 6e73 2e0a 0a43  ontributions...C
+00000f10: 6f6d 6520 6261 636b 2073 6f6f 6ee2 84a2  ome back soon...
+00000f20: 206f 6e63 6520 4927 7665 2077 7269 7474   once I've writt
+00000f30: 656e 2074 6865 2063 6f6e 7472 6962 7574  en the contribut
+00000f40: 696e 6720 6775 6964 652e 0a0a 2323 204c  ing guide...## L
+00000f50: 6963 656e 7365 0a0a 776f 6d2e 7079 2069  icense..wom.py i
+00000f60: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
+00000f70: 2074 6865 0a5b 4d49 5420 4c69 6365 6e73   the.[MIT Licens
+00000f80: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00000f90: 622e 636f 6d2f 4a6f 6e78 736c 6179 732f  b.com/Jonxslays/
+00000fa0: 776f 6d2e 7079 2f62 6c6f 622f 6d61 7374  wom.py/blob/mast
+00000fb0: 6572 2f4c 4943 454e 5345 292e 0a0a       er/LICENSE)...
```

