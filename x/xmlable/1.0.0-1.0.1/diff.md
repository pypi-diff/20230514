# Comparing `tmp/xmlable-1.0.0.tar.gz` & `tmp/xmlable-1.0.1.tar.gz`

## Comparing `xmlable-1.0.0.tar` & `xmlable-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 xmlable-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/basic_config/config.xsd
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/basic_config/config_xml_example.xml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/basic_config/config_xml_template.xml
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/basic_config/main.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/complex/config.xsd
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/complex/config_xml_example.xml
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/complex/config_xml_template.xml
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/complex/main.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/invalid/main.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/maps/config.xsd
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/maps/config_xml_example.xml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/maps/config_xml_template.xml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/maps/main.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/namespaces/config.xsd
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/namespaces/config_xml_example.xml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/namespaces/config_xml_template.xml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/namespaces/main.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/userdefined/config.xsd
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/userdefined/config_xml_example.xml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/userdefined/config_xml_template.xml
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 xmlable-1.0.0/examples/userdefined/main.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 xmlable-1.0.0/src/xmlable/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 xmlable-1.0.0/src/xmlable/_errors.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 xmlable-1.0.0/src/xmlable/_io.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 xmlable-1.0.0/src/xmlable/_lxml_helpers.py
--rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 xmlable-1.0.0/src/xmlable/_manual.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 xmlable-1.0.0/src/xmlable/_user.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 xmlable-1.0.0/src/xmlable/_utils.py
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 xmlable-1.0.0/src/xmlable/_xmlify.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 xmlable-1.0.0/src/xmlable/_xobject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xmlable-1.0.0/src/xmlable/py.typed
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 xmlable-1.0.0/tests/test_basic.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 xmlable-1.0.0/tests/utils.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 xmlable-1.0.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 xmlable-1.0.0/LICENSE
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 xmlable-1.0.0/README.md
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 xmlable-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 xmlable-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 xmlable-1.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/basic_config/config.xsd
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/basic_config/config_xml_example.xml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/basic_config/config_xml_template.xml
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/basic_config/main.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/complex/config.xsd
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/complex/config_xml_example.xml
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/complex/config_xml_template.xml
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/complex/main.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/invalid/main.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/maps/config.xsd
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/maps/config_xml_example.xml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/maps/config_xml_template.xml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/maps/main.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/namespaces/config.xsd
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/namespaces/config_xml_example.xml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/namespaces/config_xml_template.xml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/namespaces/main.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/userdefined/config.xsd
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/userdefined/config_xml_example.xml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/userdefined/config_xml_template.xml
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 xmlable-1.0.1/examples/userdefined/main.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_errors.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_io.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_lxml_helpers.py
+-rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_manual.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_user.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_utils.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_xmlify.py
+-rw-r--r--   0        0        0    23007 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/_xobject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xmlable-1.0.1/src/xmlable/py.typed
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 xmlable-1.0.1/tests/test_basic.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 xmlable-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 xmlable-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 xmlable-1.0.1/README.md
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 xmlable-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 xmlable-1.0.1/PKG-INFO
```

### Comparing `xmlable-1.0.0/.github/workflows/ci.yml` & `xmlable-1.0.1/.github/workflows/ci.yml`

 * *Files 22% similar despite different names*

```diff
@@ -18,14 +18,17 @@
       - uses: actions/setup-python@v4
         with:
           python-version: "3.11"
       - name: Install Hatch
         run: pipx install hatch
       - name: Test
         run: hatch run check:test
+      - name: typecheck
+        continue-on-error: true
+        run: hatch run check:typecheck
       - name: lint
         run: hatch run check:lint
       - name: Build
         run: hatch build
       - name: Publish
         if: github.ref == 'refs/heads/master'
         run: hatch publish --user "__token__" --auth ${{ secrets.XMLABLE_TOKEN }}
```

### Comparing `xmlable-1.0.0/examples/basic_config/config.xsd` & `xmlable-1.0.1/examples/basic_config/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/examples/basic_config/main.py` & `xmlable-1.0.1/examples/basic_config/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/examples/complex/config.xsd` & `xmlable-1.0.1/examples/complex/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/examples/complex/config_xml_example.xml` & `xmlable-1.0.1/examples/complex/config_xml_example.xml`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/examples/complex/config_xml_template.xml` & `xmlable-1.0.1/examples/complex/config_xml_template.xml`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/examples/complex/main.py` & `xmlable-1.0.1/examples/complex/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/examples/maps/config.xsd` & `xmlable-1.0.1/examples/maps/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/examples/maps/config_xml_example.xml` & `xmlable-1.0.1/examples/maps/config_xml_example.xml`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/examples/maps/config_xml_template.xml` & `xmlable-1.0.1/examples/maps/config_xml_template.xml`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/examples/maps/main.py` & `xmlable-1.0.1/examples/maps/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/examples/namespaces/config.xsd` & `xmlable-1.0.1/examples/namespaces/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/examples/namespaces/main.py` & `xmlable-1.0.1/examples/namespaces/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/examples/userdefined/config.xsd` & `xmlable-1.0.1/examples/userdefined/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/examples/userdefined/main.py` & `xmlable-1.0.1/examples/userdefined/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/src/xmlable/_errors.py` & `xmlable-1.0.1/src/xmlable/_errors.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/src/xmlable/_io.py` & `xmlable-1.0.1/src/xmlable/_io.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/src/xmlable/_lxml_helpers.py` & `xmlable-1.0.1/src/xmlable/_lxml_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,8 +26,8 @@
     return with_children(parent, [child])
 
 
 def children(obj: ObjectifiedElement) -> Iterable[ObjectifiedElement]:
     def not_comment(child_obj: ObjectifiedElement):
         return child_obj.tag != "comment"
 
-    return filter(not_comment, obj.getchildren())
+    return filter(not_comment, obj.getchildren())  # type: ignore[arg-type, operator]
```

### Comparing `xmlable-1.0.0/src/xmlable/_manual.py` & `xmlable-1.0.1/src/xmlable/_manual.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/src/xmlable/_user.py` & `xmlable-1.0.1/src/xmlable/_user.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/src/xmlable/_utils.py` & `xmlable-1.0.1/src/xmlable/_utils.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/src/xmlable/_xmlify.py` & `xmlable-1.0.1/src/xmlable/_xmlify.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/src/xmlable/_xobject.py` & `xmlable-1.0.1/src/xmlable/_xobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,21 +457,21 @@
     INV: only generic types for v are {tuple, list, dict, set}
     """
     t = type(v)
     if t in {int, float, str, bool, NoneType}:
         return t
     elif t == dict and len(v) > 0:
         t0, t1 = next(iter(v.items()))
-        return dict[resolve_type(t0), resolve_type(t1)]
+        return dict[resolve_type(t0), resolve_type(t1)]  # type: ignore[misc, index, no-any-return]
     elif t == list and len(v) > 0:
-        return list[resolve_type(v[0])]
+        return list[resolve_type(v[0])]  # type: ignore[misc, index, no-any-return]
     elif t == set and len(v) > 0:
-        return set[resolve_type(next(iter(v)))]
+        return set[resolve_type(next(iter(v)))]  # type: ignore[misc, index, no-any-return]
     elif t == tuple and len(v) > 0:
-        return tuple[*(resolve_type(vi) for vi in v)]
+        return tuple[*(resolve_type(vi) for vi in v)]  # type: ignore[misc, no-any-return]
     else:
         # INV: non-generic type
         return t
 
 
 @dataclass
 class UnionObj(XObject):
@@ -518,15 +518,15 @@
                 for t, xobj in self.xobjects.items()
             ],
         )
 
     def xml_out(self, name: str, val: Any, ctx: XErrorCtx) -> _Element:
         t = resolve_type(val)
 
-        if (val_xobj := self.xobjects.get(t)) is not None:
+        if t is not None and (val_xobj := self.xobjects.get(t)) is not None:
             variant_name = self.elem_gen(t)
             return with_child(
                 Element(name),
                 val_xobj.xml_out(variant_name, val, ctx.next(variant_name)),
             )
         else:
             types = " | ".join(str(t) for t in self.xobjects.keys())
```

### Comparing `xmlable-1.0.0/tests/test_basic.py` & `xmlable-1.0.1/tests/test_basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,31 @@
 from dataclasses import dataclass
+from lxml import etree, objectify
+from typing import Any
+
 from xmlable import *
-from utils import validate
+
+
+def validate(obj: Any):
+    schema_name: str = "basic"
+    obj_cls = type(obj)
+
+    """ Checks both a valid xml conforms """
+    xsd = obj_cls.xsd(schema_name)
+    xsd_schema = etree.XMLSchema(xsd)
+
+    xml = obj.xml_value(schema_name)
+    xml_str = etree.tostring(xml)
+    xml_object = objectify.fromstring(xml_str)
+
+    # validation check
+    xsd_schema.assertValid(xml)
+    assert obj == obj_cls.parse(
+        xml_object
+    ), "Parsed object does not match source"
 
 
 def test_scalar_classes():
     @xmlify
     @dataclass
     class Test0:
         pass
```

### Comparing `xmlable-1.0.0/LICENSE` & `xmlable-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlable-1.0.0/pyproject.toml` & `xmlable-1.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xmlable"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Oliver Killane", email="oliverkillane.business@gmail.com" },
 ]
 description = "A tool for generating xsd and xml config from python data classes"
 readme = "README.md"
 license = { file = "LICENSE"}
 keywords = ["xml", "xmlschema", "xsd", "lxml"]
@@ -23,15 +23,15 @@
     "lxml-stubs==0.4.0",
     "termcolor==2.3.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/OliverKillane/xmlable"
 "Bug Tracker" = "https://github.com/OliverKillane/xmlable/issues"
-
+"Source" = "https://github.com/OliverKillane/xmlable"
 
 [project.optional-dependencies]
 dev = [
     "black==23.3.0",
     "mypy==1.2.0",
     "pytest==7.3.1",
 ]
@@ -77,7 +77,8 @@
 
 [tool.hatch.envs.check]
 features = ["dev"]
 
 [tool.hatch.envs.check.scripts]
 test = "pytest"
 lint = "black ."
+typecheck = "mypy --check-untyped-defs"
```

### Comparing `xmlable-1.0.0/PKG-INFO` & `xmlable-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: xmlable
-Version: 1.0.0
+Version: 1.0.1
 Summary: A tool for generating xsd and xml config from python data classes
 Project-URL: Homepage, https://github.com/OliverKillane/xmlable
 Project-URL: Bug Tracker, https://github.com/OliverKillane/xmlable/issues
+Project-URL: Source, https://github.com/OliverKillane/xmlable
 Author-email: Oliver Killane <oliverkillane.business@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Oliver Killane
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -39,40 +40,40 @@
 Requires-Dist: black==23.3.0; extra == 'dev'
 Requires-Dist: mypy==1.2.0; extra == 'dev'
 Requires-Dist: pytest==7.3.1; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # XMLable
 
-## What is this?
-
-An easy xml/xsd config generator and parser for python dataclasses!
+## An easy xml/xsd generator and parser for python dataclasses!
 
 ```python
 @xmlify
 @dataclass
 class Config:
     date: str
     number_of_cores: int
     codes: list[int]
     show_logs: bool
 
 
-write_xsd(Config, "config.xsd")
-write_xml(Config, "config_xml_template.xml")
-write_xml_value(
-    Config(
-        date="31/02/2023",  # no validation yet :(
-        number_of_cores=48,
-        codes=[101, 345, 42, 67],
-        show_logs=False,
-    ),
-    "config_xml_example.xml",
+write_file("config.xsd", Config.xsd())
+write_file("config_xml_template.xml", Config.xml())
+
+original = Config(
+    date="31/02/2023",  # no validation yet :(
+    number_of_cores=48,
+    codes=[101, 345, 42, 67],
+    show_logs=False,
 )
-config: Config = parse_file(Config, "config_xml_example.xml")
+write_file("config_xml_example.xml", original.xml_value())
+
+read_config: Config = parse_file(Config, "config_xml_example.xml")
+
+assert read_config == original
 ```
 
 See more in [examples](examples/)
 
 ## Capabilities
 
 ### Types
@@ -96,15 +97,15 @@
     a: dict[tuple[int, str], list[tuple[dict[int, float | str], set[bool]]]]
 
 c1 = Complex(
     a={(3, "hello"): [({3: 0.4}, {True, False}), ({2: "str"}, {False})]}
 )
 ```
 
-#### Custom Classes
+### Custom Classes
 
 The xmlify interface can be implemented by adding methods described in [xmlify](src/xmlable/_xmlify.py)
 Once the class `is_xmlified` it can be used just as if generated by `@xmlify`
 
 ```python
 from xmlable._xobject import XObject
 from xmlable._user import IXmlify
@@ -133,19 +134,17 @@
 
     def xsd_dependencies() -> set[type]:
         return {MyClass}
 ```
 
 See the [user define example](examples/userdefined) for implementation.
 
--
-
-### Limitations
+## Limitations
 
-#### Unions of Generic Types
+### Unions of Generic Types
 
 Generating xsd works, parsing works, however generating an xml template can fail
 if they type is not determinable at runtime.
 
 - Values do not have type arguments carried with them
 - Many types are indistinguishable in python
 
@@ -175,25 +174,21 @@
 pip install .[dev] # install optional dev dependencies (mypy, black and pytest)
 
 black . # to reformat
 mypy    # type check
 pytest  # to run tests
 ```
 
-## To Improve
+[Hatch](https://hatch.pypa.io/) is used for build.
 
-### Better Namespaces
+## To Improve
 
-Lxml qualifies namespaces for element names, but not for other attributes.
-As xsd types need to be qualified, and lxml will not, there are several options:
+### Fuzzing
 
-1. Always use no prefix as the xmlSchema, and add as an invariant to all code. [problematic as user may want to change prefix]
-2. Create our own namespace resolution algo to traverse tree, determine what prefixes to use for what namespaces [complex and decide when to overwrite a custom xmlified object's chosen prefixes - an author may hardcode]
-3. Use string for type, but add to element's namespace map so lxml can resolve properly. But if the user overwrites with their own prefix, both will be present for this element. [On balance best approach]
+(As a fun weekend project) generate arbitrary python data types with values, and dataclasses.
+Then `@xmlify` all and validate as in the current tests
 
-I chose option [3.] on balance, for example:
+### Etree vs Objectify
 
-```python
-Element('{http://www.w3.org/2001/XMLSchema}element', type="xs:integer", nsmap={'xs' : 'http://www.w3.org/2001/XMLSchema'})
-```
+Currently using objectify for parsing and etree for construction, I want to move parsing to use `etree`
 
-Hence if we use a schema using `xsd`, it will declare the `xs` namespace at this interface (hence type string is valid), but continue to use `xsd` for everything else.
+- previously used objectify for quick prototype.
```

