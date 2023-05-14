# Comparing `tmp/john-0.1.5a0.tar.gz` & `tmp/john-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "john-0.1.5a0.tar", max compression
+gzip compressed data, was "john-0.1.6.tar", max compression
```

## Comparing `john-0.1.5a0.tar` & `john-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1108 2023-04-24 10:27:11.710010 john-0.1.5a0/LICENSE
--rw-r--r--   0        0        0      268 2023-04-24 10:27:11.710010 john-0.1.5a0/README.md
--rw-r--r--   0        0        0       85 2023-04-24 13:37:39.992745 john-0.1.5a0/john/__init__.py
--rw-r--r--   0        0        0      106 2023-04-24 10:27:11.710010 john-0.1.5a0/john/factory.py
--rw-r--r--   0        0        0     2090 2023-05-03 15:54:44.915729 john-0.1.5a0/john/tdd.py
--rw-r--r--   0        0        0     7943 2023-05-03 15:55:42.420797 john-0.1.5a0/john/test_case.py
--rw-r--r--   0        0        0      681 2023-05-03 17:03:16.264584 john-0.1.5a0/pyproject.toml
--rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 john-0.1.5a0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 john-0.1.6/LICENSE
+-rw-r--r--   0        0        0      268 2023-05-03 17:25:05.122292 john-0.1.6/README.md
+-rw-r--r--   0        0        0       85 2023-05-03 17:25:05.122292 john-0.1.6/john/__init__.py
+-rw-r--r--   0        0        0      106 2023-05-03 17:25:05.122292 john-0.1.6/john/factory.py
+-rw-r--r--   0        0        0     2171 2023-05-03 17:25:05.123292 john-0.1.6/john/tdd.py
+-rw-r--r--   0        0        0     7980 2023-05-14 14:02:57.779903 john-0.1.6/john/test_case.py
+-rw-r--r--   0        0        0      679 2023-05-14 14:13:19.093613 john-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 john-0.1.6/PKG-INFO
```

### Comparing `john-0.1.5a0/LICENSE` & `john-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `john-0.1.5a0/john/tdd.py` & `john-0.1.6/john/tdd.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from john import TestCase
-from crelm import Factory
-import importlib
-import os.path
-
-class TddState:
-    def __init__(self, module_name:str):
-        self._module_name = module_name
-
-        self.reset()
-
-    def reset(self):
-        self.tube = None
-        self.sut = None
-        self.externs = []
-
-    def _ensure_tube(self) -> None:
-        if not self.tube:
-            self.sut = None
-
-            test_case_module = importlib.import_module(self._module_name)
-            test_case_filename = test_case_module.__file__
-            test_case_name = os.path.splitext(
-                os.path.basename(test_case_filename))[0]
-
-            c_filename = f'{test_case_name}.c'
-            h_filename = f'{test_case_name}.h'
-
-            self.tube = Factory().create_Tube(test_case_name) \
-                .set_source_folder_relative(test_case_filename) \
-                .add_source_file(c_filename) \
-                .add_header_file(h_filename) \
-                .add_externs(self.externs)
-            
-            return self.tube
-
-    def ensure_sut(self):
-        if not self.sut:
-            self.sut = self._ensure_tube().squeeze()
-
-        return self.sut
-
-class Tdd(TestCase):
-
-    @staticmethod
-    def go():
-        Tdd.Runner.run()
-
-    @classmethod
-    def setUpClass(clazz) -> None:
-        clazz._state = TddState(clazz.__module__)
-        return super().setUpClass()
-
-    @classmethod
-    def tearDownClass(clazz) -> None:
-        clazz._state = None
-        return super().tearDownClass()
-
-    def setUpMocks(self):
-        pass
-
-    def setUp(self):
-        super().setUp()
-        self.setUpMocks()
-
-    @property
-    def _state(self):
-        return self.__class__._state
-
-    @property
-    def sut(self):
-        return self._state.ensure_sut()
-    
-    def register_mock(self, sig:str) -> None:
-        if not self._state.sut:
-            self._state.externs.append(sig)
-
-    def attach_mock(self, func):
-        def_extern_decorator = self._state.tube._ffi.def_extern()
-        def_extern_decorator(func)
-        return getattr(self._state.tube._lib, func.__name__)
+from john import TestCase
+from crelm import Factory
+import importlib
+import os.path
+
+class TddState:
+    def __init__(self, module_name:str):
+        self._module_name = module_name
+
+        self.reset()
+
+    def reset(self):
+        self.tube = None
+        self.sut = None
+        self.externs = []
+
+    def _ensure_tube(self) -> None:
+        if not self.tube:
+            self.sut = None
+
+            test_case_module = importlib.import_module(self._module_name)
+            test_case_filename = test_case_module.__file__
+            test_case_name = os.path.splitext(
+                os.path.basename(test_case_filename))[0]
+
+            c_filename = f'{test_case_name}.c'
+            h_filename = f'{test_case_name}.h'
+
+            self.tube = Factory().create_Tube(test_case_name) \
+                .set_source_folder_relative(test_case_filename) \
+                .add_source_file(c_filename) \
+                .add_header_file(h_filename) \
+                .add_externs(self.externs)
+            
+            return self.tube
+
+    def ensure_sut(self):
+        if not self.sut:
+            self.sut = self._ensure_tube().squeeze()
+
+        return self.sut
+
+class Tdd(TestCase):
+
+    @staticmethod
+    def go():
+        Tdd.Runner.run()
+
+    @classmethod
+    def setUpClass(clazz) -> None:
+        clazz._state = TddState(clazz.__module__)
+        return super().setUpClass()
+
+    @classmethod
+    def tearDownClass(clazz) -> None:
+        clazz._state = None
+        return super().tearDownClass()
+
+    def setUpMocks(self):
+        pass
+
+    def setUp(self):
+        super().setUp()
+        self.setUpMocks()
+
+    @property
+    def _state(self):
+        return self.__class__._state
+
+    @property
+    def sut(self):
+        return self._state.ensure_sut()
+    
+    def register_mock(self, sig:str) -> None:
+        if not self._state.sut:
+            self._state.externs.append(sig)
+
+    def attach_mock(self, func):
+        def_extern_decorator = self._state.tube._ffi.def_extern()
+        def_extern_decorator(func)
+        return getattr(self._state.tube._lib, func.__name__)
```

### Comparing `john-0.1.5a0/john/test_case.py` & `john-0.1.6/john/test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,21 +98,21 @@
             '*.c', '*.h', '*.so', '*.i', '*.o')]
         return unittest.TestCase.setUp(self)
 
     def writeFile(self, filename: str, text: str) -> str:
         return self._helper.write_file(self.testName, filename=filename, text=text)
 
 class AssertMixin:
-    def assertZero(self, actual, msg=None):
+    def assertZero(self, actual, msg='Should be zero but is not'):
         assert 0 == actual, msg
 
-    def assertNotZero(self, actual, msg=None):
+    def assertNotZero(self, actual, msg='Is zero but should not be'):
         assert 0 != actual, msg
 
-# foss: based on https://stackconfig = overflow.com/questions/4319825/python-unittest-opposite-of-assertraises
+# foss: based on https://stackoverflow.com/questions/4319825/python-unittest-opposite-of-assertraises
 is_micropython = sys.implementation.name == "micropython"
 
 if is_micropython:
     from unittest import AssertRaisesContext
 
     class AssertDoesNotRaiseContext(AssertRaisesContext):
         def __exit__(self, exc_type, exc_value, tb):
```

### Comparing `john-0.1.5a0/pyproject.toml` & `john-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "john"
-version = "0.1.5a0"
+version = "0.1.6"
 description = "Jeneral Outlying Helper Nuggetoids"
 authors = [
   "WideOpenTech <fossie@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `john-0.1.5a0/PKG-INFO` & `john-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: john
-Version: 0.1.5a0
+Version: 0.1.6
 Summary: Jeneral Outlying Helper Nuggetoids
 Home-page: https://github.com/wideopensource/john
 Author: WideOpenTech
 Author-email: fossie@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

