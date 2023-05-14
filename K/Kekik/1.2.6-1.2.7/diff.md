# Comparing `tmp/Kekik-1.2.6.tar.gz` & `tmp/Kekik-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kekik-1.2.6.tar", last modified: Sat May 13 11:09:43 2023, max compression
+gzip compressed data, was "Kekik-1.2.7.tar", last modified: Sun May 14 06:33:03 2023, max compression
```

## Comparing `Kekik-1.2.6.tar` & `Kekik-1.2.7.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:09:43.714169 Kekik-1.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:09:43.714169 Kekik-1.2.6/Kekik/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/BIST.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/Nesne.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/csv2dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/dict2csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/dict2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/dosya2set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/dosya_indir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/hwid_kontrol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:09:43.714169 Kekik-1.2.6/Kekik/kisi_ver/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/kisi_ver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   189486 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/kisi_ver/biyografiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    88066 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/kisi_ver/isimler.py
--rw-r--r--   0 runner    (1001) docker     (123)    78485 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/kisi_ver/soyisimler.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/link_islemleri.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/list2html.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/liste_fetis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/mail_gonder.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/okunabilir_byte.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/proxy_ver.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/qr_ver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/ses_fetis.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/slugify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/txt_fetis.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-13 11:09:25.000000 Kekik-1.2.6/Kekik/zaman_donustur.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:09:43.714169 Kekik-1.2.6/Kekik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-13 11:09:43.000000 Kekik-1.2.6/Kekik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-13 11:09:43.000000 Kekik-1.2.6/Kekik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 11:09:43.000000 Kekik-1.2.6/Kekik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-13 11:09:43.000000 Kekik-1.2.6/Kekik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-13 11:09:43.000000 Kekik-1.2.6/Kekik.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-13 11:09:25.000000 Kekik-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-13 11:09:25.000000 Kekik-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-13 11:09:43.714169 Kekik-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-05-13 11:09:25.000000 Kekik-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 11:09:43.714169 Kekik-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-13 11:09:25.000000 Kekik-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:33:03.297975 Kekik-1.2.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:33:03.293975 Kekik-1.2.7/Kekik/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/BIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/Nesne.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/csv2dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/dict2csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/dict2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/dosya2set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/dosya_indir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/hwid_kontrol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:33:03.297975 Kekik-1.2.7/Kekik/kisi_ver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/kisi_ver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189486 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/kisi_ver/biyografiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88066 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/kisi_ver/isimler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78485 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/kisi_ver/soyisimler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/link_islemleri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/list2html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/liste_fetis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/mail_gonder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/okunabilir_byte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/proxy_ver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/qr_ver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/ses_fetis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/slugify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/txt_fetis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/unicode_tr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-14 06:32:42.000000 Kekik-1.2.7/Kekik/zaman_donustur.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:33:03.297975 Kekik-1.2.7/Kekik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-05-14 06:33:03.000000 Kekik-1.2.7/Kekik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-14 06:33:03.000000 Kekik-1.2.7/Kekik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 06:33:03.000000 Kekik-1.2.7/Kekik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-14 06:33:03.000000 Kekik-1.2.7/Kekik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 06:33:03.000000 Kekik-1.2.7/Kekik.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 06:32:42.000000 Kekik-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 06:32:42.000000 Kekik-1.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-05-14 06:33:03.297975 Kekik-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-05-14 06:32:42.000000 Kekik-1.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 06:33:03.297975 Kekik-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-14 06:32:42.000000 Kekik-1.2.7/setup.py
```

### Comparing `Kekik-1.2.6/Kekik/BIST.py` & `Kekik-1.2.7/Kekik/BIST.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/Nesne.py` & `Kekik-1.2.7/Kekik/Nesne.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/__init__.py` & `Kekik-1.2.7/Kekik/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
 ####
 from Kekik.slugify         import slugify
+from Kekik.unicode_tr      import unicode_tr
 from Kekik.link_islemleri  import link_ayikla, youtube_link_mi
 from Kekik.okunabilir_byte import okunabilir_byte
 from Kekik.zaman_donustur  import sure2saniye, zaman_donustur
 from Kekik.dict2json       import dict2json
 from Kekik.qr_ver          import qr_ver
 from Kekik.dosya_indir     import dosya_indir
 from Kekik.hwid_kontrol    import benim_hwid, hwid_kontrol
```

### Comparing `Kekik-1.2.6/Kekik/cli.py` & `Kekik-1.2.7/Kekik/cli.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/dict2csv.py` & `Kekik-1.2.7/Kekik/dict2csv.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/dict2json.py` & `Kekik-1.2.7/Kekik/dict2json.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/dosya_indir.py` & `Kekik-1.2.7/Kekik/dosya_indir.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/hwid_kontrol.py` & `Kekik-1.2.7/Kekik/hwid_kontrol.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/kisi_ver/__init__.py` & `Kekik-1.2.7/Kekik/kisi_ver/__init__.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/kisi_ver/biyografiler.py` & `Kekik-1.2.7/Kekik/kisi_ver/biyografiler.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/kisi_ver/isimler.py` & `Kekik-1.2.7/Kekik/kisi_ver/isimler.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/kisi_ver/soyisimler.py` & `Kekik-1.2.7/Kekik/kisi_ver/soyisimler.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/link_islemleri.py` & `Kekik-1.2.7/Kekik/link_islemleri.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/list2html.py` & `Kekik-1.2.7/Kekik/list2html.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/mail_gonder.py` & `Kekik-1.2.7/Kekik/mail_gonder.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/okunabilir_byte.py` & `Kekik-1.2.7/Kekik/okunabilir_byte.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/proxy_ver.py` & `Kekik-1.2.7/Kekik/proxy_ver.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/qr_ver.py` & `Kekik-1.2.7/Kekik/qr_ver.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/ses_fetis.py` & `Kekik-1.2.7/Kekik/ses_fetis.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/slugify.py` & `Kekik-1.2.7/Kekik/slugify.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/txt_fetis.py` & `Kekik-1.2.7/Kekik/txt_fetis.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik/zaman_donustur.py` & `Kekik-1.2.7/Kekik/zaman_donustur.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/Kekik.egg-info/PKG-INFO` & `Kekik-1.2.7/Kekik.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kekik
-Version: 1.2.6
+Version: 1.2.7
 Summary: İşlerimizi kolaylaştıracak fonksiyonların el altında durduğu kütüphane..
 Home-page: https://github.com/keyiflerolsun/Kekik
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: Kekik,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,18 +24,20 @@
 ![License](https://img.shields.io/pypi/l/Kekik?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/Kekik?logo=windowsterminal&logoColor=white)
 
 ![PyPI](https://img.shields.io/pypi/v/Kekik?logo=pypi&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/Kekik?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/Kekik?logo=pypi&logoColor=white)
 
+[![PyPI Yükle](https://github.com/keyiflerolsun/Kekik/actions/workflows/pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/Kekik/actions/workflows/pypiYukle.yml)
+
 *İşlerimizi kolaylaştıracak fonksiyonların el altında durduğu kütüphane..*
 
-[![ForTheBadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
+[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
 # Yüklemek
 pip install Kekik
 
@@ -50,14 +52,23 @@
 from Kekik import slugify
 
 print(slugify("Ömer Faruk Sancak"))
 
 # » omer-faruk-sancak
 ```
 
+### **[unicode_tr](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/unicode_tr.py)**
+```python
+from Kekik import unicode_tr
+
+print(unicode_tr(u"izmir istanbul").title())
+
+# » İzmir İstanbul
+```
+
 ### **[link_ayikla](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/link_islemleri.py)**
 ```python
 from Kekik import link_ayikla
 
 print(link_ayikla("Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent ornare nec turpis at mollis. Aenean iaculis metus libero, a rhoncus justo suscipit quis. Suspendisse sodales ante eros. Curabitur sagittis massa lacus, vel placerat turpis aliquet ac. Nulla porta cursus consequat. Etiam tristique vestibulum maximus. Vestibulum scelerisque vehicula ex, non feugiat eros placerat a. Cras eleifend cursus felis. Nullam pulvinar dictum purus, eu lobortis sapien posuere accumsan. Integer suscipit nisi diam, nec gravida eros malesuada a. Sed vestibulum sollicitudin ex ut volutpat. Phasellus non magna sed neque blandit vestibulum vitae nec ante. https://google.com Proin fringilla ligula nec metus sagittis venenatis."))
 
 # ['https://google.com']
@@ -226,15 +237,15 @@
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ## 🌐 Telif Hakkı ve Lisans
 
-* *Copyright (C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
+* *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/Kekik/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
 
 *Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
 
 ##
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Kekik Version: 1.2.6 Summary: Ä°Ålerimizi
+Metadata-Version: 2.1 Name: Kekik Version: 1.2.7 Summary: Ä°Ålerimizi
 kolaylaÅtÄ±racak fonksiyonlarÄ±n el altÄ±nda durduÄu kÃ¼tÃ¼phane.. Home-page:
 https://github.com/keyiflerolsun/Kekik Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 Kekik,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -13,30 +13,35 @@
 Kekik&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/âï¸-Kahve
 Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/pyversions/
 Kekik?logo=python&logoColor=white) ![License](https://img.shields.io/pypi/l/
 Kekik?logo=gnu&logoColor=white) ![Status](https://img.shields.io/pypi/status/
 Kekik?logo=windowsterminal&logoColor=white) ![PyPI](https://img.shields.io/
 pypi/v/Kekik?logo=pypi&logoColor=white) ![PyPI - Downloads](https://
 img.shields.io/pypi/dm/Kekik?logo=pypi&logoColor=white) ![PyPI - Wheel](https:/
-/img.shields.io/pypi/wheel/Kekik?logo=pypi&logoColor=white) *Ä°Ålerimizi
-kolaylaÅtÄ±racak fonksiyonlarÄ±n el altÄ±nda durduÄu kÃ¼tÃ¼phane..* [!
-[ForTheBadge made-with-python](http://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](http://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install Kekik #
-GÃ¼ncellemek pip install -U Kekik ``` ## [https://i.imgur.com/ETZ1ABF.png]
-KullanÄ±m ### **[slugify](https://github.com/keyiflerolsun/Kekik/blob/main/
-Kekik/slugify.py)** ```python from Kekik import slugify print(slugify("Ãmer
-Faruk Sancak")) # Â» omer-faruk-sancak ``` ### **[link_ayikla](https://
-github.com/keyiflerolsun/Kekik/blob/main/Kekik/link_islemleri.py)** ```python
-from Kekik import link_ayikla print(link_ayikla("Lorem ipsum dolor sit amet,
-consectetur adipiscing elit. Praesent ornare nec turpis at mollis. Aenean
-iaculis metus libero, a rhoncus justo suscipit quis. Suspendisse sodales ante
-eros. Curabitur sagittis massa lacus, vel placerat turpis aliquet ac. Nulla
-porta cursus consequat. Etiam tristique vestibulum maximus. Vestibulum
+/img.shields.io/pypi/wheel/Kekik?logo=pypi&logoColor=white) [![PyPI YÃ¼kle]
+(https://github.com/keyiflerolsun/Kekik/actions/workflows/pypiYukle.yml/
+badge.svg)](https://github.com/keyiflerolsun/Kekik/actions/workflows/
+pypiYukle.yml) *Ä°Ålerimizi kolaylaÅtÄ±racak fonksiyonlarÄ±n el altÄ±nda
+durduÄu kÃ¼tÃ¼phane..* [![ForTheBadge made-with-python](https://
+ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash #
+YÃ¼klemek pip install Kekik # GÃ¼ncellemek pip install -U Kekik ``` ## [https:/
+/i.imgur.com/ETZ1ABF.png] KullanÄ±m ### **[slugify](https://github.com/
+keyiflerolsun/Kekik/blob/main/Kekik/slugify.py)** ```python from Kekik import
+slugify print(slugify("Ãmer Faruk Sancak")) # Â» omer-faruk-sancak ``` ### **
+[unicode_tr](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/
+unicode_tr.py)** ```python from Kekik import unicode_tr print(unicode_tr
+(u"izmir istanbul").title()) # Â» Ä°zmir Ä°stanbul ``` ### **[link_ayikla]
+(https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/link_islemleri.py)**
+```python from Kekik import link_ayikla print(link_ayikla("Lorem ipsum dolor
+sit amet, consectetur adipiscing elit. Praesent ornare nec turpis at mollis.
+Aenean iaculis metus libero, a rhoncus justo suscipit quis. Suspendisse sodales
+ante eros. Curabitur sagittis massa lacus, vel placerat turpis aliquet ac.
+Nulla porta cursus consequat. Etiam tristique vestibulum maximus. Vestibulum
 scelerisque vehicula ex, non feugiat eros placerat a. Cras eleifend cursus
 felis. Nullam pulvinar dictum purus, eu lobortis sapien posuere accumsan.
 Integer suscipit nisi diam, nec gravida eros malesuada a. Sed vestibulum
 sollicitudin ex ut volutpat. Phasellus non magna sed neque blandit vestibulum
 vitae nec ante. https://google.com Proin fringilla ligula nec metus sagittis
 venenatis.")) # ['https://google.com'] ``` ### **[youtube_link_mi](https://
 github.com/keyiflerolsun/Kekik/blob/main/Kekik/link_islemleri.py)** ```python
@@ -123,14 +128,14 @@
 blob/main/Kekik/txt_fetis.py)** ### **[satirlar_ekle](https://github.com/
 keyiflerolsun/Kekik/blob/main/Kekik/txt_fetis.py)** ### **[satir_sil](https://
 github.com/keyiflerolsun/Kekik/blob/main/Kekik/txt_fetis.py)** ### **
 [list2html](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/
 list2html.py)** ### **[mail_gonder](https://github.com/keyiflerolsun/Kekik/
 blob/main/Kekik/mail_gonder.py)** ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla]
 (https://KekikAkademi.org/Kahve)** ## ð Telif HakkÄ± ve Lisans * *Copyright
-(C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
+(C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
 GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/
 keyiflerolsun/Kekik/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
 lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
 isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
 (https://t.me/KekikKahve) ## > **[@KekikAkademi](https://t.me/KekikAkademi)**
 *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `Kekik-1.2.6/Kekik.egg-info/SOURCES.txt` & `Kekik-1.2.7/Kekik.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 Kekik/mail_gonder.py
 Kekik/okunabilir_byte.py
 Kekik/proxy_ver.py
 Kekik/qr_ver.py
 Kekik/ses_fetis.py
 Kekik/slugify.py
 Kekik/txt_fetis.py
+Kekik/unicode_tr.py
 Kekik/zaman_donustur.py
 Kekik.egg-info/PKG-INFO
 Kekik.egg-info/SOURCES.txt
 Kekik.egg-info/dependency_links.txt
 Kekik.egg-info/requires.txt
 Kekik.egg-info/top_level.txt
 Kekik/kisi_ver/__init__.py
```

### Comparing `Kekik-1.2.6/LICENSE` & `Kekik-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Kekik-1.2.6/PKG-INFO` & `Kekik-1.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kekik
-Version: 1.2.6
+Version: 1.2.7
 Summary: İşlerimizi kolaylaştıracak fonksiyonların el altında durduğu kütüphane..
 Home-page: https://github.com/keyiflerolsun/Kekik
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: Kekik,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,18 +24,20 @@
 ![License](https://img.shields.io/pypi/l/Kekik?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/Kekik?logo=windowsterminal&logoColor=white)
 
 ![PyPI](https://img.shields.io/pypi/v/Kekik?logo=pypi&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/Kekik?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/Kekik?logo=pypi&logoColor=white)
 
+[![PyPI Yükle](https://github.com/keyiflerolsun/Kekik/actions/workflows/pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/Kekik/actions/workflows/pypiYukle.yml)
+
 *İşlerimizi kolaylaştıracak fonksiyonların el altında durduğu kütüphane..*
 
-[![ForTheBadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
+[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
 # Yüklemek
 pip install Kekik
 
@@ -50,14 +52,23 @@
 from Kekik import slugify
 
 print(slugify("Ömer Faruk Sancak"))
 
 # » omer-faruk-sancak
 ```
 
+### **[unicode_tr](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/unicode_tr.py)**
+```python
+from Kekik import unicode_tr
+
+print(unicode_tr(u"izmir istanbul").title())
+
+# » İzmir İstanbul
+```
+
 ### **[link_ayikla](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/link_islemleri.py)**
 ```python
 from Kekik import link_ayikla
 
 print(link_ayikla("Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent ornare nec turpis at mollis. Aenean iaculis metus libero, a rhoncus justo suscipit quis. Suspendisse sodales ante eros. Curabitur sagittis massa lacus, vel placerat turpis aliquet ac. Nulla porta cursus consequat. Etiam tristique vestibulum maximus. Vestibulum scelerisque vehicula ex, non feugiat eros placerat a. Cras eleifend cursus felis. Nullam pulvinar dictum purus, eu lobortis sapien posuere accumsan. Integer suscipit nisi diam, nec gravida eros malesuada a. Sed vestibulum sollicitudin ex ut volutpat. Phasellus non magna sed neque blandit vestibulum vitae nec ante. https://google.com Proin fringilla ligula nec metus sagittis venenatis."))
 
 # ['https://google.com']
@@ -226,15 +237,15 @@
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ## 🌐 Telif Hakkı ve Lisans
 
-* *Copyright (C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
+* *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/Kekik/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
 
 *Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
 
 ##
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Kekik Version: 1.2.6 Summary: Ä°Ålerimizi
+Metadata-Version: 2.1 Name: Kekik Version: 1.2.7 Summary: Ä°Ålerimizi
 kolaylaÅtÄ±racak fonksiyonlarÄ±n el altÄ±nda durduÄu kÃ¼tÃ¼phane.. Home-page:
 https://github.com/keyiflerolsun/Kekik Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 Kekik,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -13,30 +13,35 @@
 Kekik&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/âï¸-Kahve
 Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/pyversions/
 Kekik?logo=python&logoColor=white) ![License](https://img.shields.io/pypi/l/
 Kekik?logo=gnu&logoColor=white) ![Status](https://img.shields.io/pypi/status/
 Kekik?logo=windowsterminal&logoColor=white) ![PyPI](https://img.shields.io/
 pypi/v/Kekik?logo=pypi&logoColor=white) ![PyPI - Downloads](https://
 img.shields.io/pypi/dm/Kekik?logo=pypi&logoColor=white) ![PyPI - Wheel](https:/
-/img.shields.io/pypi/wheel/Kekik?logo=pypi&logoColor=white) *Ä°Ålerimizi
-kolaylaÅtÄ±racak fonksiyonlarÄ±n el altÄ±nda durduÄu kÃ¼tÃ¼phane..* [!
-[ForTheBadge made-with-python](http://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](http://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install Kekik #
-GÃ¼ncellemek pip install -U Kekik ``` ## [https://i.imgur.com/ETZ1ABF.png]
-KullanÄ±m ### **[slugify](https://github.com/keyiflerolsun/Kekik/blob/main/
-Kekik/slugify.py)** ```python from Kekik import slugify print(slugify("Ãmer
-Faruk Sancak")) # Â» omer-faruk-sancak ``` ### **[link_ayikla](https://
-github.com/keyiflerolsun/Kekik/blob/main/Kekik/link_islemleri.py)** ```python
-from Kekik import link_ayikla print(link_ayikla("Lorem ipsum dolor sit amet,
-consectetur adipiscing elit. Praesent ornare nec turpis at mollis. Aenean
-iaculis metus libero, a rhoncus justo suscipit quis. Suspendisse sodales ante
-eros. Curabitur sagittis massa lacus, vel placerat turpis aliquet ac. Nulla
-porta cursus consequat. Etiam tristique vestibulum maximus. Vestibulum
+/img.shields.io/pypi/wheel/Kekik?logo=pypi&logoColor=white) [![PyPI YÃ¼kle]
+(https://github.com/keyiflerolsun/Kekik/actions/workflows/pypiYukle.yml/
+badge.svg)](https://github.com/keyiflerolsun/Kekik/actions/workflows/
+pypiYukle.yml) *Ä°Ålerimizi kolaylaÅtÄ±racak fonksiyonlarÄ±n el altÄ±nda
+durduÄu kÃ¼tÃ¼phane..* [![ForTheBadge made-with-python](https://
+ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash #
+YÃ¼klemek pip install Kekik # GÃ¼ncellemek pip install -U Kekik ``` ## [https:/
+/i.imgur.com/ETZ1ABF.png] KullanÄ±m ### **[slugify](https://github.com/
+keyiflerolsun/Kekik/blob/main/Kekik/slugify.py)** ```python from Kekik import
+slugify print(slugify("Ãmer Faruk Sancak")) # Â» omer-faruk-sancak ``` ### **
+[unicode_tr](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/
+unicode_tr.py)** ```python from Kekik import unicode_tr print(unicode_tr
+(u"izmir istanbul").title()) # Â» Ä°zmir Ä°stanbul ``` ### **[link_ayikla]
+(https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/link_islemleri.py)**
+```python from Kekik import link_ayikla print(link_ayikla("Lorem ipsum dolor
+sit amet, consectetur adipiscing elit. Praesent ornare nec turpis at mollis.
+Aenean iaculis metus libero, a rhoncus justo suscipit quis. Suspendisse sodales
+ante eros. Curabitur sagittis massa lacus, vel placerat turpis aliquet ac.
+Nulla porta cursus consequat. Etiam tristique vestibulum maximus. Vestibulum
 scelerisque vehicula ex, non feugiat eros placerat a. Cras eleifend cursus
 felis. Nullam pulvinar dictum purus, eu lobortis sapien posuere accumsan.
 Integer suscipit nisi diam, nec gravida eros malesuada a. Sed vestibulum
 sollicitudin ex ut volutpat. Phasellus non magna sed neque blandit vestibulum
 vitae nec ante. https://google.com Proin fringilla ligula nec metus sagittis
 venenatis.")) # ['https://google.com'] ``` ### **[youtube_link_mi](https://
 github.com/keyiflerolsun/Kekik/blob/main/Kekik/link_islemleri.py)** ```python
@@ -123,14 +128,14 @@
 blob/main/Kekik/txt_fetis.py)** ### **[satirlar_ekle](https://github.com/
 keyiflerolsun/Kekik/blob/main/Kekik/txt_fetis.py)** ### **[satir_sil](https://
 github.com/keyiflerolsun/Kekik/blob/main/Kekik/txt_fetis.py)** ### **
 [list2html](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/
 list2html.py)** ### **[mail_gonder](https://github.com/keyiflerolsun/Kekik/
 blob/main/Kekik/mail_gonder.py)** ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla]
 (https://KekikAkademi.org/Kahve)** ## ð Telif HakkÄ± ve Lisans * *Copyright
-(C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
+(C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
 GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/
 keyiflerolsun/Kekik/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
 lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
 isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
 (https://t.me/KekikKahve) ## > **[@KekikAkademi](https://t.me/KekikAkademi)**
 *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `Kekik-1.2.6/README.md` & `Kekik-1.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 ![License](https://img.shields.io/pypi/l/Kekik?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/Kekik?logo=windowsterminal&logoColor=white)
 
 ![PyPI](https://img.shields.io/pypi/v/Kekik?logo=pypi&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/Kekik?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/Kekik?logo=pypi&logoColor=white)
 
+[![PyPI Yükle](https://github.com/keyiflerolsun/Kekik/actions/workflows/pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/Kekik/actions/workflows/pypiYukle.yml)
+
 *İşlerimizi kolaylaştıracak fonksiyonların el altında durduğu kütüphane..*
 
-[![ForTheBadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
+[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
 # Yüklemek
 pip install Kekik
 
@@ -34,14 +36,23 @@
 from Kekik import slugify
 
 print(slugify("Ömer Faruk Sancak"))
 
 # » omer-faruk-sancak
 ```
 
+### **[unicode_tr](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/unicode_tr.py)**
+```python
+from Kekik import unicode_tr
+
+print(unicode_tr(u"izmir istanbul").title())
+
+# » İzmir İstanbul
+```
+
 ### **[link_ayikla](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/link_islemleri.py)**
 ```python
 from Kekik import link_ayikla
 
 print(link_ayikla("Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent ornare nec turpis at mollis. Aenean iaculis metus libero, a rhoncus justo suscipit quis. Suspendisse sodales ante eros. Curabitur sagittis massa lacus, vel placerat turpis aliquet ac. Nulla porta cursus consequat. Etiam tristique vestibulum maximus. Vestibulum scelerisque vehicula ex, non feugiat eros placerat a. Cras eleifend cursus felis. Nullam pulvinar dictum purus, eu lobortis sapien posuere accumsan. Integer suscipit nisi diam, nec gravida eros malesuada a. Sed vestibulum sollicitudin ex ut volutpat. Phasellus non magna sed neque blandit vestibulum vitae nec ante. https://google.com Proin fringilla ligula nec metus sagittis venenatis."))
 
 # ['https://google.com']
@@ -210,15 +221,15 @@
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ## 🌐 Telif Hakkı ve Lisans
 
-* *Copyright (C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
+* *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/Kekik/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
 
 *Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
 
 ##
```

#### html2text {}

```diff
@@ -5,30 +5,35 @@
 Kekik&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/âï¸-Kahve
 Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/pyversions/
 Kekik?logo=python&logoColor=white) ![License](https://img.shields.io/pypi/l/
 Kekik?logo=gnu&logoColor=white) ![Status](https://img.shields.io/pypi/status/
 Kekik?logo=windowsterminal&logoColor=white) ![PyPI](https://img.shields.io/
 pypi/v/Kekik?logo=pypi&logoColor=white) ![PyPI - Downloads](https://
 img.shields.io/pypi/dm/Kekik?logo=pypi&logoColor=white) ![PyPI - Wheel](https:/
-/img.shields.io/pypi/wheel/Kekik?logo=pypi&logoColor=white) *Ä°Ålerimizi
-kolaylaÅtÄ±racak fonksiyonlarÄ±n el altÄ±nda durduÄu kÃ¼tÃ¼phane..* [!
-[ForTheBadge made-with-python](http://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](http://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install Kekik #
-GÃ¼ncellemek pip install -U Kekik ``` ## [https://i.imgur.com/ETZ1ABF.png]
-KullanÄ±m ### **[slugify](https://github.com/keyiflerolsun/Kekik/blob/main/
-Kekik/slugify.py)** ```python from Kekik import slugify print(slugify("Ãmer
-Faruk Sancak")) # Â» omer-faruk-sancak ``` ### **[link_ayikla](https://
-github.com/keyiflerolsun/Kekik/blob/main/Kekik/link_islemleri.py)** ```python
-from Kekik import link_ayikla print(link_ayikla("Lorem ipsum dolor sit amet,
-consectetur adipiscing elit. Praesent ornare nec turpis at mollis. Aenean
-iaculis metus libero, a rhoncus justo suscipit quis. Suspendisse sodales ante
-eros. Curabitur sagittis massa lacus, vel placerat turpis aliquet ac. Nulla
-porta cursus consequat. Etiam tristique vestibulum maximus. Vestibulum
+/img.shields.io/pypi/wheel/Kekik?logo=pypi&logoColor=white) [![PyPI YÃ¼kle]
+(https://github.com/keyiflerolsun/Kekik/actions/workflows/pypiYukle.yml/
+badge.svg)](https://github.com/keyiflerolsun/Kekik/actions/workflows/
+pypiYukle.yml) *Ä°Ålerimizi kolaylaÅtÄ±racak fonksiyonlarÄ±n el altÄ±nda
+durduÄu kÃ¼tÃ¼phane..* [![ForTheBadge made-with-python](https://
+ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash #
+YÃ¼klemek pip install Kekik # GÃ¼ncellemek pip install -U Kekik ``` ## [https:/
+/i.imgur.com/ETZ1ABF.png] KullanÄ±m ### **[slugify](https://github.com/
+keyiflerolsun/Kekik/blob/main/Kekik/slugify.py)** ```python from Kekik import
+slugify print(slugify("Ãmer Faruk Sancak")) # Â» omer-faruk-sancak ``` ### **
+[unicode_tr](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/
+unicode_tr.py)** ```python from Kekik import unicode_tr print(unicode_tr
+(u"izmir istanbul").title()) # Â» Ä°zmir Ä°stanbul ``` ### **[link_ayikla]
+(https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/link_islemleri.py)**
+```python from Kekik import link_ayikla print(link_ayikla("Lorem ipsum dolor
+sit amet, consectetur adipiscing elit. Praesent ornare nec turpis at mollis.
+Aenean iaculis metus libero, a rhoncus justo suscipit quis. Suspendisse sodales
+ante eros. Curabitur sagittis massa lacus, vel placerat turpis aliquet ac.
+Nulla porta cursus consequat. Etiam tristique vestibulum maximus. Vestibulum
 scelerisque vehicula ex, non feugiat eros placerat a. Cras eleifend cursus
 felis. Nullam pulvinar dictum purus, eu lobortis sapien posuere accumsan.
 Integer suscipit nisi diam, nec gravida eros malesuada a. Sed vestibulum
 sollicitudin ex ut volutpat. Phasellus non magna sed neque blandit vestibulum
 vitae nec ante. https://google.com Proin fringilla ligula nec metus sagittis
 venenatis.")) # ['https://google.com'] ``` ### **[youtube_link_mi](https://
 github.com/keyiflerolsun/Kekik/blob/main/Kekik/link_islemleri.py)** ```python
@@ -115,14 +120,14 @@
 blob/main/Kekik/txt_fetis.py)** ### **[satirlar_ekle](https://github.com/
 keyiflerolsun/Kekik/blob/main/Kekik/txt_fetis.py)** ### **[satir_sil](https://
 github.com/keyiflerolsun/Kekik/blob/main/Kekik/txt_fetis.py)** ### **
 [list2html](https://github.com/keyiflerolsun/Kekik/blob/main/Kekik/
 list2html.py)** ### **[mail_gonder](https://github.com/keyiflerolsun/Kekik/
 blob/main/Kekik/mail_gonder.py)** ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla]
 (https://KekikAkademi.org/Kahve)** ## ð Telif HakkÄ± ve Lisans * *Copyright
-(C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
+(C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU
 GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/
 keyiflerolsun/Kekik/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
 lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
 isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
 (https://t.me/KekikKahve) ## > **[@KekikAkademi](https://t.me/KekikAkademi)**
 *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `Kekik-1.2.6/setup.py` & `Kekik-1.2.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 setup(
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
     packages     = ["Kekik"],
 
     name         = "Kekik",
-    version      = "1.2.6",
+    version      = "1.2.7",
     url          = "https://github.com/keyiflerolsun/Kekik",
     description  = "İşlerimizi kolaylaştıracak fonksiyonların el altında durduğu kütüphane..",
     keywords     = ["Kekik", "KekikAkademi", "keyiflerolsun"],
 
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True,
```

