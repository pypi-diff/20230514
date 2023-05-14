# Comparing `tmp/multicloud_diagrams-0.2.0.tar.gz` & `tmp/multicloud_diagrams-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicloud_diagrams-0.2.0.tar", max compression
+gzip compressed data, was "multicloud_diagrams-0.2.1.tar", max compression
```

## Comparing `multicloud_diagrams-0.2.0.tar` & `multicloud_diagrams-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.2.0/LICENSE
--rw-r--r--   0        0        0        0 2023-05-14 15:51:16.576166 multicloud_diagrams-0.2.0/README.md
--rw-r--r--   0        0        0    17035 2023-05-14 17:22:53.723977 multicloud_diagrams-0.2.0/multicloud_diagrams/__init__.py
--rw-r--r--   0        0        0      509 2023-05-14 17:23:23.355314 multicloud_diagrams-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 multicloud_diagrams-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.2.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-14 15:51:16.576166 multicloud_diagrams-0.2.1/README.md
+-rw-r--r--   0        0        0    17035 2023-05-14 17:33:30.479330 multicloud_diagrams-0.2.1/multicloud_diagrams/__init__.py
+-rw-r--r--   0        0        0      509 2023-05-14 18:13:39.252207 multicloud_diagrams-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 multicloud_diagrams-0.2.1/PKG-INFO
```

### Comparing `multicloud_diagrams-0.2.0/LICENSE` & `multicloud_diagrams-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.2.0/multicloud_diagrams/__init__.py` & `multicloud_diagrams-0.2.1/multicloud_diagrams/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             # Position Vertex based on X,Y cords
             if f'vertex:{table_name}:row:{index}' in self.prev_coords:
                 if 'x' in self.prev_coords[f'vertex:{table_name}:row:{index}']:
                     mx_geometry.set('x', self.prev_coords[f'vertex:{table_name}:row:{index}']['x'])
                 if 'y' in self.prev_coords[f'vertex:{table_name}:row:{index}']:
                     mx_geometry.set('y', self.prev_coords[f'vertex:{table_name}:row:{index}']['y'])
 
-    def add_vertex(self, id: str, node_name: str, ARN: str, metadata='', node_type=''):
+    def add_vertex(self, id: str, node_name: str, arn: str, metadata='', node_type=''):
 
         # check that there is no such vertex already
         exist = False
         for mx_cell in self.root:
             # print(mxCell.attrib['id'])
             if mx_cell.attrib['id'] == f'vertex:{node_type}:{id}':
                 logging.warning(f'Already exists: vertex:{node_type}:{id} name:{node_name}')
@@ -164,15 +164,15 @@
 
             stringified_metadata = self.stringify_dict(metadata)
 
             mx_cell = et.SubElement(self.root,
                                     'mxCell',
                                     id=f'vertex:{node_type}:{id}',
                                     # id = f'vertex:{ARN}',
-                                    value=f'<b>Name</b>: {node_name}<BR><b>ARN</b>: {ARN} {stringified_metadata}',
+                                    value=f'<b>Name</b>: {node_name}<BR><b>ARN</b>: {arn} {stringified_metadata}',
                                     style=("verticalLabelPosition=bottom;"
                                            "html=1;"
                                            "verticalAlign=top;"
                                            "aspect=fixed;align=left;"
                                            "pointerEvents=1;"
                                            f"{shape_parameters['style']}"
                                            ""),
```

### Comparing `multicloud_diagrams-0.2.0/PKG-INFO` & `multicloud_diagrams-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicloud-diagrams
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library to generate DRAW.IO compatible diagrams to represent Cloud infrastructure. AWS Cloud supported.
 License: MIT
 Author: Roman Tsypuk
 Author-email: tsypuk.conf@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

