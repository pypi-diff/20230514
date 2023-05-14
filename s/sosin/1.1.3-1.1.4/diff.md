# Comparing `tmp/sosin-1.1.3.tar.gz` & `tmp/sosin-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.1.3.tar", last modified: Fri May 12 12:18:15 2023, max compression
+gzip compressed data, was "sosin-1.1.4.tar", last modified: Sun May 14 03:15:01 2023, max compression
```

## Comparing `sosin-1.1.3.tar` & `sosin-1.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 12:18:15.474296 sosin-1.1.3/
--rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     1268 2023-05-12 12:18:15.473296 sosin-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-12 12:18:15.475294 sosin-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      985 2023-05-12 12:17:53.000000 sosin-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:18:15.435506 sosin-1.1.3/sosin/
--rw-rw-rw-   0        0        0       23 2023-05-12 11:29:34.000000 sosin-1.1.3/sosin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:18:15.458873 sosin-1.1.3/sosin/databases/
--rw-rw-rw-   0        0        0     4934 2023-04-24 10:38:48.000000 sosin-1.1.3/sosin/databases/fs.py
--rw-rw-rw-   0        0        0     9763 2023-05-12 11:29:34.000000 sosin-1.1.3/sosin/databases/rdb.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:18:15.460872 sosin-1.1.3/sosin/rpa/
--rw-rw-rw-   0        0        0    10828 2023-04-22 13:06:11.000000 sosin-1.1.3/sosin/rpa/email_mgr.py
--rw-rw-rw-   0        0        0     3698 2023-05-10 06:56:55.000000 sosin-1.1.3/sosin/rpa/sms_mgr.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:18:15.467295 sosin-1.1.3/sosin/utils/
--rw-rw-rw-   0        0        0     1797 2023-05-12 11:29:34.000000 sosin-1.1.3/sosin/utils/currency.py
--rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.1.3/sosin/utils/log.py
--rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.1.3/sosin/utils/progress.py
--rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.1.3/sosin/utils/secret.py
--rw-rw-rw-   0        0        0      885 2023-05-10 06:56:55.000000 sosin-1.1.3/sosin/utils/zip.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:18:15.472296 sosin-1.1.3/sosin/web/
--rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.1.3/sosin/web/content.py
--rw-rw-rw-   0        0        0     5505 2023-05-12 11:29:29.000000 sosin-1.1.3/sosin/web/session.py
--rw-rw-rw-   0        0        0     1051 2023-05-12 11:29:34.000000 sosin-1.1.3/sosin/web/translate.py
--rw-rw-rw-   0        0        0     4394 2023-05-12 12:17:53.000000 sosin-1.1.3/sosin/web/virtual.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:18:15.456873 sosin-1.1.3/sosin.egg-info/
--rw-rw-rw-   0        0        0     1268 2023-05-12 12:18:15.000000 sosin-1.1.3/sosin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-05-12 12:18:15.000000 sosin-1.1.3/sosin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 12:18:15.000000 sosin-1.1.3/sosin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-12 12:18:15.000000 sosin-1.1.3/sosin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-12 12:18:15.000000 sosin-1.1.3/sosin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.485884 sosin-1.1.4/
+-rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1268 2023-05-14 03:15:01.483875 sosin-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-14 03:15:01.485884 sosin-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-05-14 01:57:48.000000 sosin-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.397470 sosin-1.1.4/sosin/
+-rw-rw-rw-   0        0        0      295 2023-05-14 01:57:48.000000 sosin-1.1.4/sosin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.453484 sosin-1.1.4/sosin/databases/
+-rw-rw-rw-   0        0        0     4934 2023-04-24 10:38:48.000000 sosin-1.1.4/sosin/databases/fs.py
+-rw-rw-rw-   0        0        0     9763 2023-05-14 01:57:45.000000 sosin-1.1.4/sosin/databases/rdb.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.456697 sosin-1.1.4/sosin/rpa/
+-rw-rw-rw-   0        0        0    10926 2023-05-14 01:57:48.000000 sosin-1.1.4/sosin/rpa/email_mgr.py
+-rw-rw-rw-   0        0        0     3698 2023-05-10 06:56:55.000000 sosin-1.1.4/sosin/rpa/sms_mgr.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.464838 sosin-1.1.4/sosin/utils/
+-rw-rw-rw-   0        0        0     1797 2023-05-14 01:57:45.000000 sosin-1.1.4/sosin/utils/currency.py
+-rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.1.4/sosin/utils/log.py
+-rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.1.4/sosin/utils/progress.py
+-rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.1.4/sosin/utils/secret.py
+-rw-rw-rw-   0        0        0      885 2023-05-10 06:56:55.000000 sosin-1.1.4/sosin/utils/zip.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.482365 sosin-1.1.4/sosin/web/
+-rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.1.4/sosin/web/content.py
+-rw-rw-rw-   0        0        0     5506 2023-05-14 01:57:26.000000 sosin-1.1.4/sosin/web/session.py
+-rw-rw-rw-   0        0        0     1051 2023-05-14 01:57:45.000000 sosin-1.1.4/sosin/web/translate.py
+-rw-rw-rw-   0        0        0     4394 2023-05-14 01:57:45.000000 sosin-1.1.4/sosin/web/virtual.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.450315 sosin-1.1.4/sosin.egg-info/
+-rw-rw-rw-   0        0        0     1268 2023-05-14 03:15:01.000000 sosin-1.1.4/sosin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-05-14 03:15:01.000000 sosin-1.1.4/sosin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 03:15:01.000000 sosin-1.1.4/sosin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-14 03:15:01.000000 sosin-1.1.4/sosin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-14 03:15:01.000000 sosin-1.1.4/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.1.3/LICENSE` & `sosin-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sosin-1.1.3/PKG-INFO` & `sosin-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sosin-1.1.3/README.md` & `sosin-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sosin-1.1.3/setup.py` & `sosin-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 setuptools.setup(
     name                                = "sosin",
-    version                             = "1.1.3",
+    version                             = "1.1.4",
     license                             = 'MIT',
     author                              = "Jason Choi",
     author_email                        = "svstar94@gmail.com",
     description                         = "Python utils for general works",
     long_description                    = open('README.md').read(),
     url                                 = "https://github.com/devsosin/sosin",
     install_requires                    = ['requests', 'requests-toolbelt'],
     packages                            = ['sosin', 'sosin.databases', 'sosin.rpa', 'sosin.utils', 'sosin.web'],
     python_requires                     = '>=3.9',
     classifiers                         = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
-    ],
+    ]
 )
```

### Comparing `sosin-1.1.3/sosin/databases/fs.py` & `sosin-1.1.4/sosin/databases/fs.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.3/sosin/databases/rdb.py` & `sosin-1.1.4/sosin/databases/rdb.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.3/sosin/rpa/email_mgr.py` & `sosin-1.1.4/sosin/rpa/email_mgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,17 @@
             IMAP_PORT = 993
             imap = imaplib.IMAP4_SSL(IMAP_SERVER, IMAP_PORT)
             imap.login(self.email_id, self.email_pw)
             self.protocol = imap
 
     def __del__(self) -> None:
         self.protocol.close()
-        self.protocol.logout()
+        # SMTP_SSL has no method logout
+        if type(self.protocol) != smtplib.SMTP_SSL:
+            self.protocol.logout()
 
     def get_email(self, header_subjects:list=[], header_since:str=None, header_from:str=None, 
                   label:str=None, encode_type='utf-8', save_path:str=None, remove_email=True
                     ) -> list[dict]:
         """
         메일 제목에 특정 문자열이 있거나 특정 발송인의 이메일 반환\n
         **필수값**\n
```

### Comparing `sosin-1.1.3/sosin/rpa/sms_mgr.py` & `sosin-1.1.4/sosin/rpa/sms_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.3/sosin/utils/currency.py` & `sosin-1.1.4/sosin/utils/currency.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.3/sosin/utils/progress.py` & `sosin-1.1.4/sosin/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.3/sosin/utils/zip.py` & `sosin-1.1.4/sosin/utils/zip.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.3/sosin/web/content.py` & `sosin-1.1.4/sosin/web/content.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.3/sosin/web/session.py` & `sosin-1.1.4/sosin/web/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,22 @@
     Session Manager
     """
 
     history:list[requests.Response] = []
 
     def __init__(self, cookie_path:str='./cookie', history_mode:bool=False) -> None:
         self._headers = { 'User-Agent': 'Mozilla/5.0' }
+        self._cookies = {}
         self._cookie_path = cookie_path
         self._mode = history_mode
         
         try:
             open(cookie_path, 'r')
             self._load_cookies()
-        except:
-            self._cookies = {}
+        except: pass
 
     def __del__(self):
         self._save_cookies()
     
     # ------------------------------------------------------------------------
     # Request Management
     def get(self, url:str, headers:dict={}, cookies:dict={}, **kwargs) -> requests.Response:
```

### Comparing `sosin-1.1.3/sosin/web/translate.py` & `sosin-1.1.4/sosin/web/translate.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.3/sosin/web/virtual.py` & `sosin-1.1.4/sosin/web/virtual.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.3/sosin.egg-info/PKG-INFO` & `sosin-1.1.4/sosin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

