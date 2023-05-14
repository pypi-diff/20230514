# Comparing `tmp/osintbuddy-0.0.2rc23.post1.tar.gz` & `tmp/osintbuddy-0.0.2rc24.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osintbuddy-0.0.2rc23.post1.tar", last modified: Sat May 13 23:58:11 2023, max compression
+gzip compressed data, was "osintbuddy-0.0.2rc24.post1.tar", last modified: Sun May 14 00:47:50 2023, max compression
```

## Comparing `osintbuddy-0.0.2rc23.post1.tar` & `osintbuddy-0.0.2rc24.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      274 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      447 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      314 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1807 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.pypirc
--rw-r--r--   0        0        0        5 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      316 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/Dockerfile
--rw-r--r--   0        0        0       11 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/LICENSE
--rw-r--r--   0        0        0      809 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/README.md
--rw-r--r--   0        0        0       47 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/docs/developer.md
--rw-r--r--   0        0        0      471 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/docs/pyproject.md
--rw-r--r--   0        0        0      208 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/docs/workflows.md
--rw-r--r--   0        0        0     6666 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/pyproject.toml
--rw-r--r--   0        0        0      293 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/README.md
--rw-r--r--   0        0        0      374 2023-05-13 23:58:11.451463 osintbuddy-0.0.2rc23.post1/src/osintbuddy/__init__.py
--rw-r--r--   0        0        0      151 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/errors.py
--rw-r--r--   0        0        0      527 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/examples/ip-plugin.py
--rw-r--r--   0        0        0      206 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/manager.py
--rw-r--r--   0        0        0      358 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/node/__init__.py
--rw-r--r--   0        0        0     1302 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/node/base.py
--rw-r--r--   0        0        0     2989 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/node/displays.py
--rw-r--r--   0        0        0     4099 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/node/inputs.py
--rw-r--r--   0        0        0     6429 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/plugins.py
--rw-r--r--   0        0        0     1301 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/utils.py
--rw-r--r--   0        0        0      964 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/tests/conftest.py
--rw-r--r--   0        0        0      664 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/tests/test_methods.py
--rw-r--r--   0        0        0     2661 1970-01-01 00:00:00.000000 osintbuddy-0.0.2rc23.post1/PKG-INFO
+-rw-r--r--   0        0        0      274 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      447 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      314 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1807 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/.pypirc
+-rw-r--r--   0        0        0        5 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      316 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/Dockerfile
+-rw-r--r--   0        0        0       11 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/LICENSE
+-rw-r--r--   0        0        0      809 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/README.md
+-rw-r--r--   0        0        0       47 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/docs/developer.md
+-rw-r--r--   0        0        0      471 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      208 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6666 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/src/README.md
+-rw-r--r--   0        0        0      374 2023-05-14 00:47:49.988958 osintbuddy-0.0.2rc24.post1/src/osintbuddy/__init__.py
+-rw-r--r--   0        0        0      151 2023-05-14 00:47:44.896869 osintbuddy-0.0.2rc24.post1/src/osintbuddy/errors.py
+-rw-r--r--   0        0        0      527 2023-05-14 00:47:44.900869 osintbuddy-0.0.2rc24.post1/src/osintbuddy/examples/ip-plugin.py
+-rw-r--r--   0        0        0      206 2023-05-14 00:47:44.900869 osintbuddy-0.0.2rc24.post1/src/osintbuddy/manager.py
+-rw-r--r--   0        0        0      358 2023-05-14 00:47:44.900869 osintbuddy-0.0.2rc24.post1/src/osintbuddy/node/__init__.py
+-rw-r--r--   0        0        0     1302 2023-05-14 00:47:44.900869 osintbuddy-0.0.2rc24.post1/src/osintbuddy/node/base.py
+-rw-r--r--   0        0        0     2989 2023-05-14 00:47:44.900869 osintbuddy-0.0.2rc24.post1/src/osintbuddy/node/displays.py
+-rw-r--r--   0        0        0     4099 2023-05-14 00:47:44.900869 osintbuddy-0.0.2rc24.post1/src/osintbuddy/node/inputs.py
+-rw-r--r--   0        0        0     6329 2023-05-14 00:47:44.900869 osintbuddy-0.0.2rc24.post1/src/osintbuddy/plugins.py
+-rw-r--r--   0        0        0     1301 2023-05-14 00:47:44.900869 osintbuddy-0.0.2rc24.post1/src/osintbuddy/utils.py
+-rw-r--r--   0        0        0      964 2023-05-14 00:47:44.900869 osintbuddy-0.0.2rc24.post1/tests/conftest.py
+-rw-r--r--   0        0        0      664 2023-05-14 00:47:44.900869 osintbuddy-0.0.2rc24.post1/tests/test_methods.py
+-rw-r--r--   0        0        0     2661 1970-01-01 00:00:00.000000 osintbuddy-0.0.2rc24.post1/PKG-INFO
```

### Comparing `osintbuddy-0.0.2rc23.post1/.gitignore` & `osintbuddy-0.0.2rc24.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc23.post1/.pre-commit-config.yaml` & `osintbuddy-0.0.2rc24.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc23.post1/README.md` & `osintbuddy-0.0.2rc24.post1/README.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc23.post1/docs/pylint.md` & `osintbuddy-0.0.2rc24.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc23.post1/pyproject.toml` & `osintbuddy-0.0.2rc24.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc23.post1/src/osintbuddy/examples/ip-plugin.py` & `osintbuddy-0.0.2rc24.post1/src/osintbuddy/examples/ip-plugin.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc23.post1/src/osintbuddy/node/base.py` & `osintbuddy-0.0.2rc24.post1/src/osintbuddy/node/base.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc23.post1/src/osintbuddy/node/displays.py` & `osintbuddy-0.0.2rc24.post1/src/osintbuddy/node/displays.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc23.post1/src/osintbuddy/node/inputs.py` & `osintbuddy-0.0.2rc24.post1/src/osintbuddy/node/inputs.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc23.post1/src/osintbuddy/plugins.py` & `osintbuddy-0.0.2rc24.post1/src/osintbuddy/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,48 +118,48 @@
         }
         self.transform_labels = [
             {'label': func.label, 'icon': func.icon} for func in transforms
             if hasattr(func, 'icon') and hasattr(func, 'label')
         ]
 
     def __call__(self):
-        return self.node_blueprint()
+        return self.blueprint()
 
     @staticmethod
     def _map_node_elements(element, kwargs):
         label = to_snake_case(element['label'])
         for passed_label in kwargs:
             if passed_label == label:
                 if type(kwargs[label]) is str:
                     element['value'] = kwargs[label]
                 elif type(kwargs[label]) is dict:
                     for t in kwargs[label]:
                         element[t] = kwargs[label][t]
         return element
 
     @classmethod
-    def node_blueprint(cls, **kwargs):
+    def blueprint(cls, **kwargs):
         """
         Generate and return a dictionary representing the plugins node.
         Includes label, name, color, icon, and a list of all elements
         for the node/plugin.
         """
         node = defaultdict(None)
         node['label'] = cls.label
         node['name'] = cls.name
         node['color'] = cls.color
         node['icon'] = cls.icon
         node['elements'] = []
         for element in cls.node:
             if type(element) is list:
+                e = []
                 for elm in element:
-                    node['elements'].append(cls._map_node_elements(elm.json(), kwargs))
+                    e.append(cls._map_node_elements(elm.json(), kwargs))
+                node['elements'].append(e)
             else:
-                print('element: ', element.json(), to_snake_case(element.json()['label']))
-                print('kwargs: ', kwargs, '\n\n')
                 e = cls._map_node_elements(element.json(), kwargs)
                 node['elements'].append(e)
         return node
 
     def _get_transform(self, transform_type: str, node, **kwargs) -> Any:
         """ Return output from a function accepting node data.
             The function will be called with a single argument, the node data
```

### Comparing `osintbuddy-0.0.2rc23.post1/src/osintbuddy/utils.py` & `osintbuddy-0.0.2rc24.post1/src/osintbuddy/utils.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc23.post1/tests/conftest.py` & `osintbuddy-0.0.2rc24.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc23.post1/tests/test_methods.py` & `osintbuddy-0.0.2rc24.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc23.post1/PKG-INFO` & `osintbuddy-0.0.2rc24.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osintbuddy
-Version: 0.0.2rc23.post1
+Version: 0.0.2rc24.post1
 Summary: OSINTBuddy - mine, merge, and map data for novel insights
 Author-email: jerlendds <jerlendsdev@proton.me>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

