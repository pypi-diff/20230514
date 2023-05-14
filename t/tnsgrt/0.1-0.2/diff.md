# Comparing `tmp/tnsgrt-0.1.tar.gz` & `tmp/tnsgrt-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tnsgrt-0.1.tar", last modified: Fri May 12 00:59:11 2023, max compression
+gzip compressed data, was "tnsgrt-0.2.tar", last modified: Sun May 14 01:06:50 2023, max compression
```

## Comparing `tnsgrt-0.1.tar` & `tnsgrt-0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 00:59:11.693037 tnsgrt-0.1/
--rw-rw-rw-   0        0        0     1098 2023-05-12 00:36:53.000000 tnsgrt-0.1/LICENSE
--rw-rw-rw-   0        0        0     2011 2023-05-12 00:59:11.687961 tnsgrt-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      113 2023-05-12 00:52:21.000000 tnsgrt-0.1/README.md
--rw-rw-rw-   0        0        0      822 2023-05-12 00:58:53.000000 tnsgrt-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 00:59:11.693037 tnsgrt-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 00:59:11.666924 tnsgrt-0.1/tests/
--rw-rw-rw-   0        0        0     2173 2023-05-11 05:29:13.000000 tnsgrt-0.1/tests/test_snelson.py
--rw-rw-rw-   0        0        0     6465 2023-05-11 05:29:13.000000 tnsgrt-0.1/tests/test_stiffness.py
--rw-rw-rw-   0        0        0    35237 2023-05-11 05:29:13.000000 tnsgrt-0.1/tests/test_structure.py
--rw-rw-rw-   0        0        0     1727 2023-05-11 05:29:13.000000 tnsgrt-0.1/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 00:59:11.687961 tnsgrt-0.1/tnsgrt.egg-info/
--rw-rw-rw-   0        0        0     2011 2023-05-12 00:59:11.000000 tnsgrt-0.1/tnsgrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-05-12 00:59:11.000000 tnsgrt-0.1/tnsgrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 00:59:11.000000 tnsgrt-0.1/tnsgrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-12 00:59:11.000000 tnsgrt-0.1/tnsgrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 00:59:11.000000 tnsgrt-0.1/tnsgrt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 01:06:50.183207 tnsgrt-0.2/
+-rw-rw-rw-   0        0        0     1098 2023-05-12 00:36:53.000000 tnsgrt-0.2/LICENSE
+-rw-rw-rw-   0        0        0     2062 2023-05-14 01:06:50.183207 tnsgrt-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2023-05-12 05:06:43.000000 tnsgrt-0.2/README.md
+-rw-rw-rw-   0        0        0      822 2023-05-14 01:05:41.000000 tnsgrt-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 01:06:50.183207 tnsgrt-0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 01:06:50.183207 tnsgrt-0.2/tests/
+-rw-rw-rw-   0        0        0     1056 2023-05-12 04:29:28.000000 tnsgrt-0.2/tests/test_michell.py
+-rw-rw-rw-   0        0        0     2173 2023-05-11 05:29:13.000000 tnsgrt-0.2/tests/test_snelson.py
+-rw-rw-rw-   0        0        0     6465 2023-05-13 13:55:14.000000 tnsgrt-0.2/tests/test_stiffness.py
+-rw-rw-rw-   0        0        0    39014 2023-05-14 00:03:27.000000 tnsgrt-0.2/tests/test_structure.py
+-rw-rw-rw-   0        0        0     1727 2023-05-11 05:29:13.000000 tnsgrt-0.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-14 01:06:50.183207 tnsgrt-0.2/tnsgrt.egg-info/
+-rw-rw-rw-   0        0        0     2062 2023-05-14 01:06:50.000000 tnsgrt-0.2/tnsgrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-14 01:06:50.000000 tnsgrt-0.2/tnsgrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 01:06:50.000000 tnsgrt-0.2/tnsgrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-14 01:06:50.000000 tnsgrt-0.2/tnsgrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 01:06:50.000000 tnsgrt-0.2/tnsgrt.egg-info/top_level.txt
```

### Comparing `tnsgrt-0.1/LICENSE` & `tnsgrt-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.1/PKG-INFO` & `tnsgrt-0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tnsgrt
-Version: 0.1
+Version: 0.2
 Summary: Python library with support for analysis and design of Tensegrity structures
 Author-email: "Mauricio C. de Oliveira" <mcdeoliveira@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Mauricio de Oliveira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,8 +42,8 @@
 Install with pip by typing:
 
     pip install tnsgrt
 
 
 ## Documentation
 
-See
+See on [read the docs](https://tnsgrt.readthedocs.io).
```

### Comparing `tnsgrt-0.1/pyproject.toml` & `tnsgrt-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tnsgrt"
-version = "0.1"
+version = "0.2"
 authors = [
     { name = "Mauricio C. de Oliveira", email = "mcdeoliveira@duck.com" }
 ]
 description = "Python library with support for analysis and design of Tensegrity structures"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["Tensegrity", "structures", "trusses"]
```

### Comparing `tnsgrt-0.1/tests/test_snelson.py` & `tnsgrt-0.2/tests/test_snelson.py`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.1/tests/test_stiffness.py` & `tnsgrt-0.2/tests/test_stiffness.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,26 +13,26 @@
     def test_stiffness(self):
         s = Prism(3)
         S, F, v = s.stiffness()
         d = S.eigs()[0]
         # 6 rigid body nodes
         self.assertEqual(np.count_nonzero(d < 1e-3), 6)
         # 6 rigid body nodes + 1 soft node
-        self.assertEqual(np.count_nonzero(d < 1e7), 7)
+        self.assertEqual(np.count_nonzero(d < 1e6), 7)
 
     def test_rigid_body_1(self):
         s = Prism(3)
         # calculate stiffness
         S, F, v = s.stiffness(apply_rigid_body_constraint=True)
         # calculate eigenvalues
         d = S.eigs(k=6)[0]
         # no rigid body nodes
         self.assertEqual(np.count_nonzero(d < 1e-3), 0)
         # 1 soft node
-        self.assertEqual(np.count_nonzero(d < 1e7), 1)
+        self.assertEqual(np.count_nonzero(d < 1e6), 1)
 
     def test_eigenmodes(self):
         s = Prism(3)
         # calculate stiffness
         S, F, v = s.stiffness(apply_rigid_body_constraint=True)
         # eigenmodes
         d = S.modes(k=6)[0]
```

### Comparing `tnsgrt-0.1/tests/test_structure.py` & `tnsgrt-0.2/tests/test_structure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import unittest
 
 import numpy as np
+import pandas as pd
 import scipy
 
+from tnsgrt import utils
 from tnsgrt.stiffness import NodeConstraint, Stiffness
 from tnsgrt.structure import Structure
 
 
 class TestStructure(unittest.TestCase):
 
     def test_constructor(self):
@@ -82,14 +84,15 @@
         np.testing.assert_array_equal(s.members, members)
         np.testing.assert_array_equal(s.member_tags['bar'], np.arange(2, 3, dtype=np.uint64))
         np.testing.assert_array_equal(s.member_tags['string'], np.arange(0, 2, dtype=np.uint64))
         self.assertEqual(s.get_number_of_nodes(), 3)
         self.assertEqual(s.get_number_of_members(), 3)
         self.assertEqual(len(s.member_properties), 3)
 
+        member_defaults = Structure.member_defaults.copy()
         Structure.member_defaults['vertical'] = {'linewidth': 1001, 'volume': 2}
         s = Structure(nodes, members,
                       member_tags={
                           'bar': np.arange(1, 3, dtype=np.uint64),
                           'string': np.arange(0, 1, dtype=np.uint64),
                           'vertical': np.arange(2, 3, dtype=np.uint64)
                       },
@@ -122,14 +125,81 @@
         np.testing.assert_array_equal(s.get_members_by_tags(['bar', 'vertical']), [2])
         self.assertEqual(len(s.member_properties), 3)
         self.assertEqual(s.member_properties.loc[1, 'linewidth'], 2)
         self.assertEqual(s.member_properties.loc[2, 'linewidth'], 1001)
         self.assertEqual(s.get_member_properties([1, 2], ['volume', 'mass']).to_dict('index'),
                          {1: {'volume': 0., 'mass': 1.}, 2: {'volume': 2., 'mass': 1.}})
         self.assertEqual(s.get_member_properties(2, ['volume', 'mass']).to_dict(), {'volume': 2., 'mass': 1.})
+        Structure.member_defaults = member_defaults
+
+    def test_get_set_member_properties(self):
+
+        nodes = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
+        members = np.array([[0, 1, 2], [1, 2, 0]])
+        s = Structure(nodes, members,
+                      member_tags={
+                          'bar': np.arange(1, 3, dtype=np.uint64),
+                          'string': np.arange(0, 1, dtype=np.uint64),
+                          'vertical': np.arange(2, 3, dtype=np.uint64)
+                      },
+                      node_tags={
+                          'bottom': np.array([0, 1], dtype=np.uint64),
+                          'top': np.array([2], dtype=np.uint64)
+                      })
+
+        properties = s.get_member_properties([1, 2], 'volume')
+        self.assertIsInstance(properties, pd.Series)
+        self.assertEqual(len(properties), 2)
+        np.testing.assert_array_equal(properties.values, [0, 0])
+
+        properties = s.get_member_properties(slice(None), 'volume')
+        self.assertIsInstance(properties, pd.Series)
+        self.assertEqual(len(properties), 3)
+
+        properties = s.get_member_properties([1, 2], 'facecolor')
+        self.assertIsInstance(properties, pd.Series)
+        self.assertEqual(len(properties), 2)
+
+        properties = s.get_member_properties(slice(None), 'facecolor')
+        self.assertIsInstance(properties, pd.Series)
+        self.assertEqual(len(properties), 3)
+
+        properties = s.get_member_properties([1, 2], ['volume', 'facecolor'])
+        self.assertIsInstance(properties, pd.DataFrame)
+        self.assertEqual(len(properties), 2)
+
+        properties = s.get_member_properties(slice(None), ['volume', 'facecolor'])
+        self.assertIsInstance(properties, pd.DataFrame)
+        self.assertEqual(len(properties), 3)
+
+        s.set_member_properties(2, 'volume', 3)
+        np.testing.assert_array_equal(s.member_properties['volume'].values, [0, 0, 3])
+
+        s.set_member_properties([1, 2], 'volume', [1, 2])
+        np.testing.assert_array_equal(s.member_properties['volume'].values, [0, 1, 2])
+
+        s.set_member_properties([1, 2], 'volume', 3)
+        np.testing.assert_array_equal(s.member_properties['volume'].values, [0, 3, 3])
+
+        s.set_member_properties([1, 2], 'volume', 1, wrap=True)
+        np.testing.assert_array_equal(s.member_properties['volume'].values, [0, 1, 1])
+
+        s.set_member_properties(2, 'facecolor', utils.Colors.BROWN.value, wrap=True)
+        self.assertEqual(s.member_properties['facecolor'].tolist(),
+                         [utils.Colors.ORANGE.value, utils.Colors.BLUE.value, utils.Colors.BROWN.value])
+
+        s.set_member_properties([1, 2], 'facecolor', utils.Colors.GREEN.value, wrap=True)
+        self.assertEqual(s.member_properties['facecolor'].tolist(),
+                         [utils.Colors.ORANGE.value, utils.Colors.GREEN.value, utils.Colors.GREEN.value])
+
+        s.set_member_properties([1, 2], 'facecolor', [utils.Colors.BLUE.value, utils.Colors.ORANGE.value],
+                                wrap=True, scalar=False)
+        self.assertEqual(s.member_properties['facecolor'].tolist(),
+                         [utils.Colors.ORANGE.value, utils.Colors.BLUE.value, utils.Colors.ORANGE.value])
+
 
     def test_add_members_and_add_nodes(self):
 
         nodes1 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
         members1 = np.array([[0, 1, 2], [1, 2, 0]])
         s = Structure(nodes1, members1,
                       member_tags={
@@ -159,14 +229,15 @@
         np.testing.assert_array_equal(s.nodes, [[1, 0, 0, 1, 0], [0, 1, 0, 1, 1], [0, 0, 1, 0, 1]])
         np.testing.assert_array_equal(s.member_properties.index, np.arange(4))
 
     def test_copy(self):
 
         nodes = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
         members = np.array([[0, 1, 2], [1, 2, 0]])
+        member_defaults = Structure.member_defaults.copy()
         Structure.member_defaults['vertical'] = {'linewidth': 1001, 'volume': 2}
         s = Structure(nodes, members,
                       member_tags={
                           'bar': np.arange(1, 3, dtype=np.uint64),
                           'string': np.arange(0, 1, dtype=np.uint64),
                           'vertical': np.arange(2, 3, dtype=np.uint64)
                       },
@@ -233,14 +304,16 @@
         self.assertEqual(len(copy.member_properties), 3)
         self.assertEqual(copy.member_properties.loc[1, 'linewidth'], 2)
         self.assertEqual(copy.member_properties.loc[2, 'linewidth'], 1001)
         self.assertEqual(copy.get_member_properties([1, 2], ['volume', 'mass']).to_dict('index'),
                          {1: {'volume': 0., 'mass': 1.}, 2: {'volume': 2., 'mass': 1.}})
         self.assertEqual(copy.get_member_properties(2, ['volume', 'mass']).to_dict(), {'volume': 2., 'mass': 1.})
 
+        Structure.member_defaults = member_defaults
+
     def test_merge(self):
 
         nodes1 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
         members1 = np.array([[0, 1, 2], [1, 2, 0]])
         s1 = Structure(nodes1, members1,
                        member_tags={
                            'bar': np.arange(1, 3, dtype=np.uint64),
@@ -603,22 +676,25 @@
         # forces
         force = np.hstack((np.kron(np.array([-np.sqrt(2), -1, np.sqrt(11)]), np.ones((3,))), [np.sqrt(3)]))
         np.testing.assert_allclose(s1.member_properties['force'], force)
 
         lambda_ = np.hstack((np.kron(np.array([-1, -1, 4]), np.ones((3,))), [4]))
         np.testing.assert_allclose(s1.member_properties['lambda_'], lambda_)
 
+        mass = np.hstack((157./200. * np.ones((6,)), 157./200./4 * np.ones((4,))))
         np.testing.assert_allclose(s1.member_properties['mass'] / s1.get_member_length() / np.pi,
-                                   157./200. * np.ones((10,)))
+                                   mass)
 
+        volume = np.hstack((np.ones((6,)), 1/4 * np.ones((4,))))
         np.testing.assert_allclose(10000 * s1.member_properties['volume'] / s1.get_member_length() / np.pi,
-                                   np.ones((10,)))
+                                   volume)
 
         np.testing.assert_allclose(s1.member_properties['stiffness'],
-                                   np.pi * s1.member_properties['modulus'] * s1.member_properties['radius']**2
+                                   np.pi * s1.member_properties['modulus'] * (s1.member_properties['radius']**2 -
+                                                                              s1.member_properties['inner_radius']**2)
                                    / s1.get_member_length())
 
         np.testing.assert_allclose(s1.member_properties['rest_length'],
                                    s1.get_member_length() * (1 - s1.member_properties['lambda_'].values
                                                              / s1.member_properties['stiffness']))
 
     def test_node_tags(self):
```

### Comparing `tnsgrt-0.1/tests/test_utils.py` & `tnsgrt-0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.1/tnsgrt.egg-info/PKG-INFO` & `tnsgrt-0.2/tnsgrt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tnsgrt
-Version: 0.1
+Version: 0.2
 Summary: Python library with support for analysis and design of Tensegrity structures
 Author-email: "Mauricio C. de Oliveira" <mcdeoliveira@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Mauricio de Oliveira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,8 +42,8 @@
 Install with pip by typing:
 
     pip install tnsgrt
 
 
 ## Documentation
 
-See
+See on [read the docs](https://tnsgrt.readthedocs.io).
```

