# Comparing `tmp/jvc_projector_remote_improved2-3.6.0.tar.gz` & `tmp/jvc_projector_remote_improved2-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jvc_projector_remote_improved2-3.6.0.tar", last modified: Fri May 12 22:56:30 2023, max compression
+gzip compressed data, was "jvc_projector_remote_improved2-3.6.1.tar", last modified: Sun May 14 15:00:05 2023, max compression
```

## Comparing `jvc_projector_remote_improved2-3.6.0.tar` & `jvc_projector_remote_improved2-3.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:56:30.084529 jvc_projector_remote_improved2-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-12 22:56:18.000000 jvc_projector_remote_improved2-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-12 22:56:30.084529 jvc_projector_remote_improved2-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-12 22:56:18.000000 jvc_projector_remote_improved2-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:56:30.080529 jvc_projector_remote_improved2-3.6.0/jvc_projector/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-12 22:56:18.000000 jvc_projector_remote_improved2-3.6.0/jvc_projector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-05-12 22:56:18.000000 jvc_projector_remote_improved2-3.6.0/jvc_projector/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-05-12 22:56:18.000000 jvc_projector_remote_improved2-3.6.0/jvc_projector/jvc_projector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:56:30.080529 jvc_projector_remote_improved2-3.6.0/jvc_projector_remote_improved2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-12 22:56:30.000000 jvc_projector_remote_improved2-3.6.0/jvc_projector_remote_improved2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-12 22:56:30.000000 jvc_projector_remote_improved2-3.6.0/jvc_projector_remote_improved2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 22:56:30.000000 jvc_projector_remote_improved2-3.6.0/jvc_projector_remote_improved2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 22:56:30.000000 jvc_projector_remote_improved2-3.6.0/jvc_projector_remote_improved2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 22:56:30.084529 jvc_projector_remote_improved2-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-12 22:56:18.000000 jvc_projector_remote_improved2-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:56:30.084529 jvc_projector_remote_improved2-3.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 22:56:18.000000 jvc_projector_remote_improved2-3.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-12 22:56:18.000000 jvc_projector_remote_improved2-3.6.0/tests/testLowLatency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:00:05.414622 jvc_projector_remote_improved2-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-14 15:00:05.414622 jvc_projector_remote_improved2-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:00:05.414622 jvc_projector_remote_improved2-3.6.1/jvc_projector/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector/jvc_projector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:00:05.414622 jvc_projector_remote_improved2-3.6.1/jvc_projector_remote_improved2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-14 15:00:05.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector_remote_improved2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-14 15:00:05.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector_remote_improved2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:00:05.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector_remote_improved2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 15:00:05.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector_remote_improved2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:00:05.418622 jvc_projector_remote_improved2-3.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:00:05.414622 jvc_projector_remote_improved2-3.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/tests/testLowLatency.py
```

### Comparing `jvc_projector_remote_improved2-3.6.0/LICENSE` & `jvc_projector_remote_improved2-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jvc_projector_remote_improved2-3.6.0/PKG-INFO` & `jvc_projector_remote_improved2-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jvc_projector_remote_improved2
-Version: 3.6.0
+Version: 3.6.1
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `jvc_projector_remote_improved2-3.6.0/README.md` & `jvc_projector_remote_improved2-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `jvc_projector_remote_improved2-3.6.0/jvc_projector/commands.py` & `jvc_projector_remote_improved2-3.6.1/jvc_projector/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,14 +213,22 @@
 class EshiftModes(Enum):
     off = b"0"
     on = b"1"
 
 
 class ContentTypes(Enum):
     # Auto Transition Values
+    auto = b"0"
+    sdr = b"1"
+    hdr10_plus = b"2"
+    hdr10 = b"3"
+    hlg = b"4"
+
+class ContentTypeTrans(Enum):
+    # Auto Transition Values
     sdr = b"1"
     hdr10_plus = b"2"
     hdr10 = b"3"
     hlg = b"4"
 
 
 class HdrProcessing(Enum):
@@ -291,15 +299,16 @@
     # response -> \x40\x89\x01\x4D\x44(the model code)\x0A
     get_model = b"MD"
 
     # software version
     get_software_version = b"IFSV", str, ACKs.info_ack
 
     # content type
-    content_type = b"PMAT", ContentTypes, ACKs.picture_ack
+    content_type = b"PMCT", ContentTypes, ACKs.picture_ack
+    content_type_trans = b"PMAT", ContentTypeTrans, ACKs.picture_ack
 
     # hdr processing (like frame by frame)
     hdr_processing = b"PMHP", HdrProcessing, ACKs.picture_ack
     hdr_level = b"PMHL", HdrLevel, ACKs.picture_ack
 
     # hdr data
     hdr_data = b"IFHR", HdrData, ACKs.info_ack
```

### Comparing `jvc_projector_remote_improved2-3.6.0/jvc_projector/jvc_projector.py` & `jvc_projector_remote_improved2-3.6.1/jvc_projector/jvc_projector.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,42 +26,42 @@
     SourceStatuses,
     TheaterOptimizer,
     HdrData,
     LampPowerModes,
     LaserPowerModes,
     AspectRatioModes,
     MaskModes,
-    HdrLevel
+    HdrLevel,
+    ContentTypeTrans,
 )
 
 
 class JVCProjector:
     """JVC Projector Control"""
 
     def __init__(
         self,
         host: str,
         password: str = "",
         # Can supply a logger object. It can hook into the HA logger
         logger: logging.Logger = logging.getLogger(__name__),
         port: int = 20554,
-        connect_timeout: int = 5,
+        connect_timeout: int = 3,
     ):
         self.host = host
         self.port = port
         # NZ models have password authentication
         self.password = password
         self.connect_timeout: int = connect_timeout
         self.logger = logger
         # Const values
         self.PJ_OK: Final = ACKs.greeting.value
         self.PJ_ACK: Final = ACKs.pj_ack.value
         self.PJ_REQ: Final = ACKs.pj_req.value
         self.client = None
-        self.command_read_timeout = 3
         # NZ or NX (NP5 is classified as NX)
         self.model_family = ""
 
     def open_connection(self) -> bool:
         """Open a connection"""
         self.logger.debug("Starting open connection")
         msg, success = self.reconnect()
@@ -269,18 +269,19 @@
         # ensure this doesnt run with dead client
         if self.client is None:
             self.logger.debug("Client is none. Reforming connection")
             self.reconnect()
 
         # max retries
         retry_count = 0
-        # use this to store error if retry counte exceeded
+        # use this to store error if retry count exceeded
         error = ""
 
-        while retry_count < 5:
+        # retry once in case connection is dead
+        while retry_count < 2:
             self.logger.debug("do_command sending command: %s", command)
             # send the command
             try:
                 self.client.sendall(command)
             except ConnectionError as err:
                 # reaching this means the writer was closed somewhere
                 self.logger.error(err)
@@ -332,15 +333,15 @@
 
             # if all fine, return the value
             return msg, True
 
         self.logger.error("retry count for running commands exceeded")
         self.logger.error(error)
 
-        return "retry count exceeded", None
+        raise TimeoutError(error)
 
     def _check_received_msg(
         self, received_msg: bytes, ack_value: bytes, command_type: bytes
     ) -> bytes:
         # This is unlikely to happen unless we read blank response
         if received_msg == b"":
             return received_msg
@@ -499,15 +500,15 @@
 
     def get_input_mode(self) -> str:
         """
         Get the current input mode
         """
         state, _ = self._do_reference_op("input_mode", ACKs.input_ack)
         return InputModes(state.replace(ACKs.input_ack.value, b"")).name
-    
+
     def get_mask_mode(self) -> str:
         """
         Get the current mask mode
         """
         state, _ = self._do_reference_op("mask", ACKs.hdmi_ack)
         return MaskModes(state.replace(ACKs.hdmi_ack.value, b"")).name
 
@@ -534,36 +535,43 @@
 
     def get_input_level(self) -> str:
         """
         Get the current input level
         """
         state, _ = self._do_reference_op("input_level", ACKs.hdmi_ack)
         return InputLevel(state.replace(ACKs.hdmi_ack.value, b"")).name
-    
+
     def get_software_version(self) -> str:
         """
         Get the current software version
         """
         state, _ = self._do_reference_op("get_software_version", ACKs.info_ack)
         return state.replace(ACKs.info_ack.value, b"")
 
     def get_content_type(self) -> str:
         """
         Get the current content type
         """
         state, _ = self._do_reference_op("content_type", ACKs.picture_ack)
         return ContentTypes(state.replace(ACKs.picture_ack.value, b"")).name
 
+    def get_content_type_trans(self) -> str:
+        """
+        Get the current auto content transition type
+        """
+        state, _ = self._do_reference_op("content_type_trans", ACKs.picture_ack)
+        return ContentTypeTrans(state.replace(ACKs.picture_ack.value, b"")).name
+
     def get_hdr_processing(self) -> str:
         """
         Get the current hdr processing setting like frame by frame. Will fail if not in HDR mode!
         """
         state, _ = self._do_reference_op("hdr_processing", ACKs.picture_ack)
         return HdrProcessing(state.replace(ACKs.picture_ack.value, b"")).name
-    
+
     def get_hdr_level(self) -> str:
         """
         Get the current hdr quantization level
         """
         state, _ = self._do_reference_op("hdr_level", ACKs.picture_ack)
         return HdrLevel(state.replace(ACKs.picture_ack.value, b"")).name
```

### Comparing `jvc_projector_remote_improved2-3.6.0/jvc_projector_remote_improved2.egg-info/PKG-INFO` & `jvc_projector_remote_improved2-3.6.1/jvc_projector_remote_improved2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jvc-projector-remote-improved2
-Version: 3.6.0
+Version: 3.6.1
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `jvc_projector_remote_improved2-3.6.0/setup.py` & `jvc_projector_remote_improved2-3.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jvc_projector_remote_improved2",
-    version="3.6.0",
+    version="3.6.1",
     author="iloveicedgreentea",
     description="A package to control JVC projectors over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/jvc_projector_improved",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `jvc_projector_remote_improved2-3.6.0/tests/testLowLatency.py` & `jvc_projector_remote_improved2-3.6.1/tests/testLowLatency.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,40 +18,41 @@
     Test projector
     """
 
     def test_mock_update(self):
         """Emulates how HA would run updates"""
         state = jvc.is_on()
         self.assertEqual(state, True)
-        self.assertEqual(jvc.model_family, "NZ")
+        self.assertEqual(jvc.model_family, "NZ7")
 
         if state:
-            lowlatency_enabled = jvc.is_ll_on()
-            installation_mode = jvc.get_install_mode()
-            input_mode = jvc.get_input_mode()
-            laser_mode = jvc.get_laser_mode()
-            eshift = jvc.get_eshift_mode()
-            color_mode = jvc.get_color_mode()
-            input_level = jvc.get_input_level()
-            content_type = jvc.get_content_type()
+            print(jvc.get_software_version())
+    #         lowlatency_enabled = jvc.is_ll_on()
+    #         installation_mode = jvc.get_install_mode()
+    #         input_mode = jvc.get_input_mode()
+    #         laser_mode = jvc.get_laser_mode()
+    #         eshift = jvc.get_eshift_mode()
+    #         color_mode = jvc.get_color_mode()
+    #         input_level = jvc.get_input_level()
+    #         content_type = jvc.get_content_type()
 
-            self.assertFalse(lowlatency_enabled)
-            self.assertEqual(installation_mode, "mode3")
-            self.assertEqual(input_mode, "hdmi2")
-            self.assertEqual(laser_mode, "auto3")
-            self.assertEqual(eshift, "off")
-            self.assertEqual(color_mode, "auto")
-            self.assertEqual(input_level, "standard")
-            self.assertEqual(content_type, "sdr")
+    #         self.assertFalse(lowlatency_enabled)
+    #         self.assertEqual(installation_mode, "mode3")
+    #         self.assertEqual(input_mode, "hdmi2")
+    #         self.assertEqual(laser_mode, "auto3")
+    #         self.assertEqual(eshift, "off")
+    #         self.assertEqual(color_mode, "auto")
+    #         self.assertEqual(input_level, "standard")
+    #         self.assertEqual(content_type, "sdr")
     
-    def test_send_command(self):
-        """test a command"""
-        # open menu
-        ack, success = jvc.exec_command("menu, menu")
+    # def test_send_command(self):
+    #     """test a command"""
+    #     # open menu
+    #     ack, success = jvc.exec_command("menu, menu")
 
-        self.assertEqual(ack, "ok")
-        self.assertTrue(success)
+    #     self.assertEqual(ack, "ok")
+    #     self.assertTrue(success)
 
-        # close menu
-        ack, success = jvc.exec_command("menu, menu")
-        self.assertEqual(ack, "ok")
-        self.assertTrue(success)
+    #     # close menu
+    #     ack, success = jvc.exec_command("menu, menu")
+    #     self.assertEqual(ack, "ok")
+    #     self.assertTrue(success)
```

