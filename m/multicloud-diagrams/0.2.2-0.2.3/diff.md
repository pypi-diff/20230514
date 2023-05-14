# Comparing `tmp/multicloud_diagrams-0.2.2.tar.gz` & `tmp/multicloud_diagrams-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicloud_diagrams-0.2.2.tar", max compression
+gzip compressed data, was "multicloud_diagrams-0.2.3.tar", max compression
```

## Comparing `multicloud_diagrams-0.2.2.tar` & `multicloud_diagrams-0.2.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.2.2/LICENSE
--rw-r--r--   0        0        0     2292 2023-05-14 20:59:03.162735 multicloud_diagrams-0.2.2/README.md
--rw-r--r--   0        0        0    17035 2023-05-14 17:33:30.479330 multicloud_diagrams-0.2.2/multicloud_diagrams/__init__.py
--rw-r--r--   0        0        0      509 2023-05-14 20:59:57.294501 multicloud_diagrams-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2810 1970-01-01 00:00:00.000000 multicloud_diagrams-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2404 2023-05-14 21:05:56.433884 multicloud_diagrams-0.2.3/README.md
+-rw-r--r--   0        0        0    17035 2023-05-14 17:33:30.479330 multicloud_diagrams-0.2.3/multicloud_diagrams/__init__.py
+-rw-r--r--   0        0        0      509 2023-05-14 21:06:33.597095 multicloud_diagrams-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 multicloud_diagrams-0.2.3/PKG-INFO
```

### Comparing `multicloud_diagrams-0.2.2/LICENSE` & `multicloud_diagrams-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.2.2/README.md` & `multicloud_diagrams-0.2.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -36,19 +36,19 @@
 
 #### AWS DynamoDB Details
 
 - Source [aws_dynamo.py](samples/samples/aws_dynamo.py)
 
 - Output compiled [drawio diagram](samples/output/output.prod.dynamo.drawio):
 
-![output.prod.dynamo.png](samples/output/png/output.prod.dynamo.png)
+![output.prod.dynamo.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.dynamo.png)
 
 #### AWS IAM Graph
 
 - Source [aws_dynamo.py](samples/samples/aws_dynamo.py)
 - Output compiled [drawio diagram](samples/output/output.prod.iam-roles.drawio)
 
-![output.prod.iam-roles.png](samples/output/png/output.prod.iam-roles.png)
+![output.prod.iam-roles.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.iam-roles.png)
 
 ### FYI:
 
 OpenSource Guide, [How to contribute to opensource](https://opensource.guide/)
```

### Comparing `multicloud_diagrams-0.2.2/multicloud_diagrams/__init__.py` & `multicloud_diagrams-0.2.3/multicloud_diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.2.2/PKG-INFO` & `multicloud_diagrams-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicloud-diagrams
-Version: 0.2.2
+Version: 0.2.3
 Summary: Library to generate DRAW.IO compatible diagrams to represent Cloud infrastructure. AWS Cloud supported.
 License: MIT
 Author: Roman Tsypuk
 Author-email: tsypuk.conf@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -50,19 +50,19 @@
 
 #### AWS DynamoDB Details
 
 - Source [aws_dynamo.py](samples/samples/aws_dynamo.py)
 
 - Output compiled [drawio diagram](samples/output/output.prod.dynamo.drawio):
 
-![output.prod.dynamo.png](samples/output/png/output.prod.dynamo.png)
+![output.prod.dynamo.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.dynamo.png)
 
 #### AWS IAM Graph
 
 - Source [aws_dynamo.py](samples/samples/aws_dynamo.py)
 - Output compiled [drawio diagram](samples/output/output.prod.iam-roles.drawio)
 
-![output.prod.iam-roles.png](samples/output/png/output.prod.iam-roles.png)
+![output.prod.iam-roles.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.iam-roles.png)
 
 ### FYI:
 
 OpenSource Guide, [How to contribute to opensource](https://opensource.guide/)
```

