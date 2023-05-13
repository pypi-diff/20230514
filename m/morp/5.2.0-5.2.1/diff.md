# Comparing `tmp/morp-5.2.0.tar.gz` & `tmp/morp-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morp-5.2.0.tar", last modified: Tue Apr 25 19:02:12 2023, max compression
+gzip compressed data, was "morp-5.2.1.tar", last modified: Sat May 13 22:41:32 2023, max compression
```

## Comparing `morp-5.2.0.tar` & `morp-5.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-25 19:02:12.666091 morp-5.2.0/
--rw-r--r--   0 jaymon     (501) staff       (20)     1079 2017-07-29 01:05:20.000000 morp-5.2.0/LICENSE.txt
--rw-r--r--   0 jaymon     (501) staff       (20)     3744 2023-04-25 19:02:12.665965 morp-5.2.0/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)     3021 2023-03-03 20:29:34.000000 morp-5.2.0/README.md
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-25 19:02:12.663828 morp-5.2.0/morp/
--rw-r--r--   0 jaymon     (501) staff       (20)      347 2023-04-25 19:01:46.000000 morp-5.2.0/morp/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)     6756 2023-02-05 20:04:47.000000 morp-5.2.0/morp/__main__.py
--rw-r--r--   0 jaymon     (501) staff       (20)       97 2023-02-07 07:17:53.000000 morp-5.2.0/morp/compat.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4714 2023-03-31 06:52:48.000000 morp-5.2.0/morp/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     1022 2023-03-03 09:33:58.000000 morp-5.2.0/morp/exception.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-25 19:02:12.665793 morp-5.2.0/morp/interface/
--rw-r--r--   0 jaymon     (501) staff       (20)     2944 2023-02-07 07:11:11.000000 morp-5.2.0/morp/interface/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11735 2023-03-03 09:01:56.000000 morp-5.2.0/morp/interface/base.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4869 2023-03-03 20:33:14.000000 morp-5.2.0/morp/interface/dropfile.py
--rw-r--r--   0 jaymon     (501) staff       (20)    13537 2023-04-25 19:00:40.000000 morp-5.2.0/morp/interface/sqs.py
--rw-r--r--   0 jaymon     (501) staff       (20)    10350 2023-03-07 19:10:15.000000 morp-5.2.0/morp/message.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-25 19:02:12.664745 morp-5.2.0/morp.egg-info/
--rw-r--r--   0 jaymon     (501) staff       (20)     3744 2023-04-25 19:02:12.000000 morp-5.2.0/morp.egg-info/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      397 2023-04-25 19:02:12.000000 morp-5.2.0/morp.egg-info/SOURCES.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-04-25 19:02:12.000000 morp-5.2.0/morp.egg-info/dependency_links.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       47 2023-04-25 19:02:12.000000 morp-5.2.0/morp.egg-info/entry_points.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-04-25 19:02:12.000000 morp-5.2.0/morp.egg-info/requires.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-04-25 19:02:12.000000 morp-5.2.0/morp.egg-info/top_level.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-04-25 19:02:12.666135 morp-5.2.0/setup.cfg
--rw-r--r--   0 jaymon     (501) staff       (20)     1815 2023-02-05 21:01:52.000000 morp-5.2.0/setup.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-13 22:41:32.211141 morp-5.2.1/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1079 2017-07-29 01:05:20.000000 morp-5.2.1/LICENSE.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)     3744 2023-05-13 22:41:32.211027 morp-5.2.1/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)     3021 2023-03-03 20:29:34.000000 morp-5.2.1/README.md
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-13 22:41:32.209605 morp-5.2.1/morp/
+-rw-r--r--   0 jaymon     (501) staff       (20)      347 2023-05-13 22:41:10.000000 morp-5.2.1/morp/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     6756 2023-02-05 20:04:47.000000 morp-5.2.1/morp/__main__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)       97 2023-02-07 07:17:53.000000 morp-5.2.1/morp/compat.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4714 2023-03-31 06:52:48.000000 morp-5.2.1/morp/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     1022 2023-03-03 09:33:58.000000 morp-5.2.1/morp/exception.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-13 22:41:32.210851 morp-5.2.1/morp/interface/
+-rw-r--r--   0 jaymon     (501) staff       (20)     2944 2023-02-07 07:11:11.000000 morp-5.2.1/morp/interface/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11735 2023-03-03 09:01:56.000000 morp-5.2.1/morp/interface/base.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5069 2023-05-13 22:39:43.000000 morp-5.2.1/morp/interface/dropfile.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    13543 2023-05-13 22:35:50.000000 morp-5.2.1/morp/interface/sqs.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    10354 2023-05-13 22:20:12.000000 morp-5.2.1/morp/message.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-13 22:41:32.210381 morp-5.2.1/morp.egg-info/
+-rw-r--r--   0 jaymon     (501) staff       (20)     3744 2023-05-13 22:41:32.000000 morp-5.2.1/morp.egg-info/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      397 2023-05-13 22:41:32.000000 morp-5.2.1/morp.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-05-13 22:41:32.000000 morp-5.2.1/morp.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       47 2023-05-13 22:41:32.000000 morp-5.2.1/morp.egg-info/entry_points.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-05-13 22:41:32.000000 morp-5.2.1/morp.egg-info/requires.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-05-13 22:41:32.000000 morp-5.2.1/morp.egg-info/top_level.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-05-13 22:41:32.211175 morp-5.2.1/setup.cfg
+-rw-r--r--   0 jaymon     (501) staff       (20)     1815 2023-02-05 21:01:52.000000 morp-5.2.1/setup.py
```

### Comparing `morp-5.2.0/LICENSE.txt` & `morp-5.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morp-5.2.0/PKG-INFO` & `morp-5.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morp
-Version: 5.2.0
+Version: 5.2.1
 Summary: Send and receive messages without thinking about it
 Home-page: http://github.com/Jaymon/morp
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Keywords: Amazon AWS SQS messages message-passing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `morp-5.2.0/README.md` & `morp-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `morp-5.2.0/morp/__main__.py` & `morp-5.2.1/morp/__main__.py`

 * *Files identical despite different names*

### Comparing `morp-5.2.0/morp/config.py` & `morp-5.2.1/morp/config.py`

 * *Files identical despite different names*

### Comparing `morp-5.2.0/morp/exception.py` & `morp-5.2.1/morp/exception.py`

 * *Files identical despite different names*

### Comparing `morp-5.2.0/morp/interface/__init__.py` & `morp-5.2.1/morp/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `morp-5.2.0/morp/interface/base.py` & `morp-5.2.1/morp/interface/base.py`

 * *Files identical despite different names*

### Comparing `morp-5.2.0/morp/interface/dropfile.py` & `morp-5.2.1/morp/interface/dropfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,16 +134,22 @@
             queue.delete()
 
     def _cleanup(self, fp, message, **kwargs):
         # clear the message so other get() requests will move on (this is the
         # one thing we can do with an exclusive lock to tell other processes
         # we have already looked at the file, I wish we could delete under an 
         # exclusive lock)
-        if kwargs.get("truncate", True):
-            fp.truncate()
+        try:
+            if kwargs.get("truncate", True):
+                fp.truncate()
 
-        fcntl.flock(fp, fcntl.LOCK_UN)
-        fp.close()
+            fcntl.flock(fp, fcntl.LOCK_UN)
+            fp.close()
+
+        except ValueError:
+            # .truncate - ValueError: truncate of closed file
+            # .flock - ValueError: I/O operation on closed file
+            pass
 
         if kwargs.get("delete", True):
             message.delete()
```

### Comparing `morp-5.2.0/morp/interface/sqs.py` & `morp-5.2.1/morp/interface/sqs.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import itertools
 import base64
 
 import boto3
 from botocore.exceptions import ClientError
 from botocore.credentials import RefreshableCredentials
 from botocore.session import get_session
+from datatypes import Datetime
 
 from ..compat import *
 from .base import Interface
 
 
 class Region(String):
     """Small wrapper that just makes sure the AWS region is valid"""
@@ -85,24 +86,22 @@
         # if an sts arn is given, get credential by assuming given role
         if arn := self.connection_config.options.get("arn", ""):
             sts_client = session.client(
                 service_name="sts",
                 region_name=region,
             )
 
+            session_ttl = self.connection_config.options.get("session_ttl", 3600)
             response = sts_client.assume_role(
                 RoleArn=arn,
                 RoleSessionName=self.connection_config.options.get(
                     "session_name",
                     "morp"
                 ),
-                DurationSeconds=self.connection_config.options.get(
-                    "session_ttl",
-                    3600
-                ),
+                DurationSeconds=session_ttl,
             ).get("Credentials")
 
             credentials = {
                 "access_key": response.get("AccessKeyId"),
                 "secret_key": response.get("SecretAccessKey"),
                 "token": response.get("SessionToken"),
                 "expiry_time": response.get("Expiration").isoformat(),
@@ -110,15 +109,15 @@
 
         else:
             session_credentials = session.get_credentials().__dict__
             credentials = {
                 "access_key": session_credentials.get("access_key"),
                 "secret_key": session_credentials.get("secret_key"),
                 "token": session_credentials.get("token"),
-                "expiry_time": Datetime(seconds=self.session_ttl).isoformat(),
+                "expiry_time": Datetime(seconds=session_ttl).isoformat(),
             }
 
         return credentials
 
 
 class SQS(Interface):
     """wraps amazon's SQS to make it work with our generic interface
```

### Comparing `morp-5.2.0/morp/message.py` & `morp-5.2.1/morp/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,21 +290,21 @@
     def target(self):
         """This method will be called from handle() and can handle any processing
         of the message, it should be defined in the child classes"""
         raise NotImplementedError()
 
     def ack(self):
         """Acknowledge this message has been processed"""
-        cls.interface.ack(cls.get_name(), self.to_interface())
+        self.interface.ack(self.get_name(), self.to_interface())
 
     def release(self, **kwargs):
         """Release this message back to the interface so another message instance
         can pick it up
         """
-        cls.interface.release(cls.get_name(), self.to_interface(), **kwargs)
+        self.interface.release(self.get_name(), self.to_interface(), **kwargs)
 
     def release_later(self, delay_seconds):
         """If you want to release the message and not have it be visible for some
         amount of time
 
         :param delay_seconds: int, how many seconds before the message can be
             processed again. The max value is interface specific
```

### Comparing `morp-5.2.0/morp.egg-info/PKG-INFO` & `morp-5.2.1/morp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morp
-Version: 5.2.0
+Version: 5.2.1
 Summary: Send and receive messages without thinking about it
 Home-page: http://github.com/Jaymon/morp
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Keywords: Amazon AWS SQS messages message-passing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `morp-5.2.0/setup.py` & `morp-5.2.1/setup.py`

 * *Files identical despite different names*

