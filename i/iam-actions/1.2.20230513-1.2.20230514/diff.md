# Comparing `tmp/iam_actions-1.2.20230513.tar.gz` & `tmp/iam_actions-1.2.20230514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230513.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230514.tar", max compression
```

## Comparing `iam_actions-1.2.20230513.tar` & `iam_actions-1.2.20230514.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-13 02:24:08.003716 iam_actions-1.2.20230513/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-13 02:24:08.003716 iam_actions-1.2.20230513/README.md
--rw-r--r--   0        0        0      228 2023-05-13 02:24:08.003716 iam_actions-1.2.20230513/iam_actions/__init__.py
--rw-r--r--   0        0        0  4253134 2023-05-13 02:25:58.575315 iam_actions-1.2.20230513/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-13 02:24:08.003716 iam_actions-1.2.20230513/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-13 02:24:08.003716 iam_actions-1.2.20230513/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-13 02:24:08.003716 iam_actions-1.2.20230513/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-13 02:24:08.003716 iam_actions-1.2.20230513/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-13 02:24:08.003716 iam_actions-1.2.20230513/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-13 02:24:08.003716 iam_actions-1.2.20230513/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-13 02:24:08.003716 iam_actions-1.2.20230513/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-13 02:24:08.003716 iam_actions-1.2.20230513/iam_actions/generate/services.py
--rw-r--r--   0        0        0   546948 2023-05-13 02:25:58.575315 iam_actions-1.2.20230513/iam_actions/policies.json
--rw-r--r--   0        0        0   193815 2023-05-13 02:25:58.575315 iam_actions-1.2.20230513/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   530553 2023-05-13 02:25:58.575315 iam_actions-1.2.20230513/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-13 02:25:59.331311 iam_actions-1.2.20230513/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230513/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230513/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-14 02:28:24.701946 iam_actions-1.2.20230514/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-14 02:28:24.701946 iam_actions-1.2.20230514/README.md
+-rw-r--r--   0        0        0      228 2023-05-14 02:28:24.701946 iam_actions-1.2.20230514/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4253134 2023-05-14 02:30:10.442568 iam_actions-1.2.20230514/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-14 02:28:24.701946 iam_actions-1.2.20230514/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-14 02:28:24.701946 iam_actions-1.2.20230514/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-14 02:28:24.701946 iam_actions-1.2.20230514/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-14 02:28:24.701946 iam_actions-1.2.20230514/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-14 02:28:24.701946 iam_actions-1.2.20230514/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-14 02:28:24.701946 iam_actions-1.2.20230514/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-14 02:28:24.701946 iam_actions-1.2.20230514/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-14 02:28:24.701946 iam_actions-1.2.20230514/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   546948 2023-05-14 02:30:10.442568 iam_actions-1.2.20230514/iam_actions/policies.json
+-rw-r--r--   0        0        0   193815 2023-05-14 02:30:10.442568 iam_actions-1.2.20230514/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   530553 2023-05-14 02:30:10.442568 iam_actions-1.2.20230514/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-14 02:30:11.178571 iam_actions-1.2.20230514/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230514/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230514/PKG-INFO
```

### Comparing `iam_actions-1.2.20230513/LICENSE` & `iam_actions-1.2.20230514/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230513/README.md` & `iam_actions-1.2.20230514/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230513/iam_actions/actions.json` & `iam_actions-1.2.20230514/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -17067,305 +17067,305 @@
             "condition_keys": [],
             "description": "Grants permission to validate an address to be used for 911 calls made with Amazon Chime Voice Connectors",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms": {
-        "UpdateCollaboration": {
+        "BatchGetSchema": {
             "access_level": "Undocumented",
-            "action": "UpdateCollaboration",
+            "action": "BatchGetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAnalysisRule": {
+        "CreateMembership": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAnalysisRule",
+            "action": "CreateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTable": {
+        "GetConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTable",
+            "action": "GetConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMembers": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListMembers",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProtectedQuery": {
+        "ListCollaborations": {
             "access_level": "Undocumented",
-            "action": "GetProtectedQuery",
+            "action": "ListCollaborations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMembership": {
+        "GetConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "UpdateMembership",
+            "action": "GetConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMember": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteMember",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemas": {
+        "DeleteMembership": {
             "access_level": "Undocumented",
-            "action": "ListSchemas",
+            "action": "DeleteMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborations": {
+        "UpdateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "ListCollaborations",
+            "action": "UpdateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchema": {
+        "DeleteCollaboration": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchema",
+            "action": "DeleteCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCollaboration": {
+        "ListMembers": {
             "access_level": "Undocumented",
-            "action": "DeleteCollaboration",
+            "action": "ListMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTableAssociations": {
+        "DeleteConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTableAssociations",
+            "action": "DeleteConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCollaboration": {
+        "DeleteConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "CreateCollaboration",
+            "action": "DeleteConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaAnalysisRule": {
+        "UpdateMembership": {
             "access_level": "Undocumented",
-            "action": "GetSchemaAnalysisRule",
+            "action": "UpdateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMemberships": {
+        "GetConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "ListMemberships",
+            "action": "GetConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProtectedQuery": {
+        "UpdateCollaboration": {
             "access_level": "Undocumented",
-            "action": "UpdateProtectedQuery",
+            "action": "UpdateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTables": {
+        "StartProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTables",
+            "action": "StartProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMembership": {
+        "DeleteConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "GetMembership",
+            "action": "DeleteConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMembership": {
+        "UpdateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "DeleteMembership",
+            "action": "UpdateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaboration": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "GetCollaboration",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAssociation": {
+        "ListProtectedQueries": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAssociation",
+            "action": "ListProtectedQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAssociation": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAssociation",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAssociation": {
+        "GetMembership": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAssociation",
+            "action": "GetMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAnalysisRule": {
+        "CreateCollaboration": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAnalysisRule",
+            "action": "CreateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAnalysisRule": {
+        "DeleteMember": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAnalysisRule",
+            "action": "DeleteMember",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAnalysisRule": {
+        "ListConfiguredTableAssociations": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAnalysisRule",
+            "action": "ListConfiguredTableAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "CreateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "CreateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProtectedQueries": {
+        "ListMemberships": {
             "access_level": "Undocumented",
-            "action": "ListProtectedQueries",
+            "action": "ListMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateConfiguredTableAssociation": {
             "access_level": "Undocumented",
             "action": "CreateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMembership": {
+        "GetCollaboration": {
             "access_level": "Undocumented",
-            "action": "CreateMembership",
+            "action": "GetCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProtectedQuery": {
+        "ListSchemas": {
             "access_level": "Undocumented",
-            "action": "StartProtectedQuery",
+            "action": "ListSchemas",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTable": {
+        "ListConfiguredTables": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTable",
+            "action": "ListConfiguredTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTable": {
+        "GetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTable",
+            "action": "GetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTable": {
+        "UpdateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTable",
+            "action": "UpdateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloud9": {
@@ -24711,81 +24711,81 @@
             "orphan": false,
             "resources": [
                 "association"
             ]
         }
     },
     "codeguru-security": {
-        "ListScans": {
+        "GetFindings": {
             "access_level": "Undocumented",
-            "action": "ListScans",
+            "action": "GetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountConfiguration": {
+        "CreateScan": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountConfiguration",
+            "action": "CreateScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUploadUrl": {
+        "UpdateAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateUploadUrl",
+            "action": "UpdateAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetScan": {
+        "ListFindings": {
             "access_level": "Undocumented",
-            "action": "GetScan",
+            "action": "ListFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateScan": {
+        "BatchGetFindings": {
             "access_level": "Undocumented",
-            "action": "CreateScan",
+            "action": "BatchGetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindings": {
+        "ListScans": {
             "access_level": "Undocumented",
-            "action": "ListFindings",
+            "action": "ListScans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFindings": {
+        "DeleteScansByCategory": {
             "access_level": "Undocumented",
-            "action": "GetFindings",
+            "action": "DeleteScansByCategory",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteScansByCategory": {
+        "GetScan": {
             "access_level": "Undocumented",
-            "action": "DeleteScansByCategory",
+            "action": "GetScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetFindings": {
+        "CreateUploadUrl": {
             "access_level": "Undocumented",
-            "action": "BatchGetFindings",
+            "action": "CreateUploadUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codepipeline": {
@@ -32692,41 +32692,41 @@
             "condition_keys": [],
             "description": "Grants permission to validates if the s3 bucket exists with appropriate permissions for CUR delivery",
             "orphan": false,
             "resources": []
         }
     },
     "customer-verification": {
-        "UpdateCustomerVerificationDetails": {
+        "CreateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "UpdateCustomerVerificationDetails",
+            "action": "CreateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomerVerificationEligibility": {
+        "GetCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "GetCustomerVerificationEligibility",
+            "action": "GetCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCustomerVerificationDetails": {
+        "GetCustomerVerificationEligibility": {
             "access_level": "Undocumented",
-            "action": "CreateCustomerVerificationDetails",
+            "action": "GetCustomerVerificationEligibility",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomerVerificationDetails": {
+        "UpdateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "GetCustomerVerificationDetails",
+            "action": "UpdateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "databrew": {
@@ -34242,275 +34242,275 @@
             "access_level": "Undocumented",
             "action": "GetProjectCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProject": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "GetProject",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "GetProjectConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "GetProjectConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserProjects": {
+        "GetProject": {
             "access_level": "Undocumented",
-            "action": "ListUserProjects",
+            "action": "GetProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProjectConfiguration": {
+        "ListUserProjects": {
             "access_level": "Undocumented",
-            "action": "GetProjectConfiguration",
+            "action": "ListUserProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "datazonecontrol": {
-        "DeleteDataSource": {
+        "CreateAccountAssociationInvitation": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "CreateAccountAssociationInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourcesByEnvironment": {
+        "GetDomain": {
             "access_level": "Undocumented",
-            "action": "ListDataSourcesByEnvironment",
+            "action": "GetDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "DissociateAccount": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "DissociateAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReviewAccountAssociationInvitation": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "ReviewAccountAssociationInvitation",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPortalLoginAuthCode": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetUserPortalLoginAuthCode",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSourceByEnvironment": {
+        "ListDomains": {
             "access_level": "Undocumented",
-            "action": "GetDataSourceByEnvironment",
+            "action": "ListDomains",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironment": {
+        "ListAssociatedEnvironments": {
             "access_level": "Undocumented",
-            "action": "ListEnvironment",
+            "action": "ListAssociatedEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAssociationInvitation": {
+        "ListAllAssociatedAccountsForEnvironment": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAssociationInvitation",
+            "action": "ListAllAssociatedAccountsForEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssociatedEnvironments": {
+        "GetMetadataCollector": {
             "access_level": "Undocumented",
-            "action": "ListAssociatedEnvironments",
+            "action": "GetMetadataCollector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllAssociatedAccountsForEnvironment": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListAllAssociatedAccountsForEnvironment",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListDataSourcesByEnvironment": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListDataSourcesByEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetadataCollector": {
+        "UpdateAccountAssociationDescription": {
             "access_level": "Undocumented",
-            "action": "GetMetadataCollector",
+            "action": "UpdateAccountAssociationDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "ListMetadataCollectorRuns": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "ListMetadataCollectorRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountAssociationDescription": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountAssociationDescription",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataCollectors": {
+        "GetDataSourceByEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListMetadataCollectors",
+            "action": "GetDataSourceByEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironment": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "DeleteEnvironment": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DissociateAccount": {
+        "GetUserPortalLoginAuthCode": {
             "access_level": "Undocumented",
-            "action": "DissociateAccount",
+            "action": "GetUserPortalLoginAuthCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssociatedDomain": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "GetAssociatedDomain",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataCollectorRuns": {
+        "ListEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListMetadataCollectorRuns",
+            "action": "ListEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironment": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironment",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAssociationInvitations": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListAccountAssociationInvitations",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDomains": {
+        "ListAccountAssociationInvitations": {
             "access_level": "Undocumented",
-            "action": "ListDomains",
+            "action": "ListAccountAssociationInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomain": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "GetDomain",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "GetAssociatedDomain": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "GetAssociatedDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "ReviewAccountAssociationInvitation": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "ReviewAccountAssociationInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListMetadataCollectors": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListMetadataCollectors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "dax": {
@@ -62174,33 +62174,33 @@
             "condition_keys": [],
             "description": "Grants permission to verify the email for FreeRTOS extended maintenance plan (EMP)",
             "orphan": false,
             "resources": []
         }
     },
     "freetier": {
-        "GetFreeTierUsage": {
+        "GetFreeTierAlertPreference": {
             "access_level": "Undocumented",
-            "action": "GetFreeTierUsage",
+            "action": "GetFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFreeTierAlertPreference": {
+        "GetFreeTierUsage": {
             "access_level": "Undocumented",
-            "action": "PutFreeTierAlertPreference",
+            "action": "GetFreeTierUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFreeTierAlertPreference": {
+        "PutFreeTierAlertPreference": {
             "access_level": "Undocumented",
-            "action": "GetFreeTierAlertPreference",
+            "action": "PutFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "fsx": {
@@ -70648,1369 +70648,1369 @@
             "condition_keys": [],
             "description": "Grants permission to update an Amazon Honeycode team for your AWS Account",
             "orphan": false,
             "resources": []
         }
     },
     "iam": {
-        "CreateVirtualMFADevice": {
+        "AddRoleToInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "CreateVirtualMFADevice",
+            "action": "AddRoleToInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstanceProfile": {
+        "ListRoles": {
             "access_level": "Undocumented",
-            "action": "CreateInstanceProfile",
+            "action": "ListRoles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "CreateAccountAlias": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "CreateAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSTSRegionalEndpointStatus": {
+        "UntagRole": {
             "access_level": "Undocumented",
-            "action": "SetSTSRegionalEndpointStatus",
+            "action": "UntagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagOpenIDConnectProvider": {
+        "ListServerCertificates": {
             "access_level": "Undocumented",
-            "action": "UntagOpenIDConnectProvider",
+            "action": "ListServerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfiles": {
+        "ListAttachedUserPolicies": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfiles",
+            "action": "ListAttachedUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateOrganizationsAccessReport": {
+        "GetInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "GenerateOrganizationsAccessReport",
+            "action": "GetInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagMFADevice": {
+        "UpdateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "UntagMFADevice",
+            "action": "UpdateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeactivateMFADevice": {
+        "DetachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "DeactivateMFADevice",
+            "action": "DetachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagServerCertificate": {
+        "SimulateCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "TagServerCertificate",
+            "action": "SimulateCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRoleDescription": {
+        "GenerateCredentialReport": {
             "access_level": "Undocumented",
-            "action": "UpdateRoleDescription",
+            "action": "GenerateCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagRole": {
+        "DeleteSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "UntagRole",
+            "action": "DeleteSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCloudFrontPublicKey": {
+        "DeletePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "UpdateCloudFrontPublicKey",
+            "action": "DeletePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserPolicies": {
+        "UpdateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListUserPolicies",
+            "action": "UpdateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountAlias": {
+        "DeleteVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountAlias",
+            "action": "DeleteVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachUserPolicy": {
+        "GetSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DetachUserPolicy",
+            "action": "GetSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSigningCertificates": {
+        "DeleteAccountAlias": {
             "access_level": "Undocumented",
-            "action": "ListSigningCertificates",
+            "action": "DeleteAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountSummary": {
+        "ListAttachedRolePolicies": {
             "access_level": "Undocumented",
-            "action": "GetAccountSummary",
+            "action": "ListAttachedRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviderTags": {
+        "ListAccountAliases": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviderTags",
+            "action": "ListAccountAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRole": {
+        "ListOpenIDConnectProviders": {
             "access_level": "Undocumented",
-            "action": "GetRole",
+            "action": "ListOpenIDConnectProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAssumeRolePolicy": {
+        "TagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateAssumeRolePolicy",
+            "action": "TagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServerCertificate": {
+        "DeleteOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetServerCertificate",
+            "action": "DeleteOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulatePrincipalPolicy": {
+        "GetUserPolicy": {
             "access_level": "Undocumented",
-            "action": "SimulatePrincipalPolicy",
+            "action": "GetUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRole": {
+        "DeleteServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "UpdateRole",
+            "action": "DeleteServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagMFADevice": {
+        "ListServiceSpecificCredentials": {
             "access_level": "Undocumented",
-            "action": "TagMFADevice",
+            "action": "ListServiceSpecificCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "CreatePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "CreatePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccessKey": {
+        "DetachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateAccessKey",
+            "action": "DetachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "UpdateAccessKey": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "UpdateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePermissionsBoundary": {
+        "ListSAMLProviders": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePermissionsBoundary",
+            "action": "ListSAMLProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPolicy": {
+        "GetCredentialReport": {
             "access_level": "Undocumented",
-            "action": "PutUserPolicy",
+            "action": "GetCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOpenIDConnectProvider": {
+        "GetServiceLinkedRoleDeletionStatus": {
             "access_level": "Undocumented",
-            "action": "GetOpenIDConnectProvider",
+            "action": "GetServiceLinkedRoleDeletionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyVersion": {
+        "DeleteLoginProfile": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyVersion",
+            "action": "DeleteLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyVersion": {
+        "GetRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetPolicyVersion",
+            "action": "GetRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "GetServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "GetServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCredentialReport": {
+        "ListUserTags": {
             "access_level": "Undocumented",
-            "action": "GenerateCredentialReport",
+            "action": "ListUserTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRole": {
+        "GetAccountName": {
             "access_level": "Undocumented",
-            "action": "DeleteRole",
+            "action": "GetAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagUser": {
+        "RemoveRoleFromInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UntagUser",
+            "action": "RemoveRoleFromInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupPolicies": {
+        "CreateAccessKey": {
             "access_level": "Undocumented",
-            "action": "ListGroupPolicies",
+            "action": "CreateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachRolePolicy": {
+        "UpdateAssumeRolePolicy": {
             "access_level": "Undocumented",
-            "action": "AttachRolePolicy",
+            "action": "UpdateAssumeRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadCloudFrontPublicKey": {
+        "CreateInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UploadCloudFrontPublicKey",
+            "action": "CreateInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulateCustomPolicy": {
+        "PutUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "SimulateCustomPolicy",
+            "action": "PutUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountEmailAddress": {
+        "CreateGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountEmailAddress",
+            "action": "CreateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagUser": {
+        "GetContextKeysForPrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "TagUser",
+            "action": "GetContextKeysForPrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagPolicy": {
+        "ListInstanceProfiles": {
             "access_level": "Undocumented",
-            "action": "UntagPolicy",
+            "action": "ListInstanceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachUserPolicy": {
+        "PassRole": {
             "access_level": "Undocumented",
-            "action": "AttachUserPolicy",
+            "action": "PassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfileTags": {
+        "ListVirtualMFADevices": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfileTags",
+            "action": "ListVirtualMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableMFADevice": {
+        "DeleteRolePolicy": {
             "access_level": "Undocumented",
-            "action": "EnableMFADevice",
+            "action": "DeleteRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountName": {
+        "TagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetAccountName",
+            "action": "TagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviders": {
+        "UploadCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviders",
+            "action": "UploadCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountName": {
+        "UploadSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountName",
+            "action": "UploadSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviderTags": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviderTags",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSSHPublicKey": {
+        "DeleteSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "UploadSSHPublicKey",
+            "action": "DeleteSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVirtualMFADevice": {
+        "UntagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteVirtualMFADevice",
+            "action": "UntagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagSAMLProvider": {
+        "UpdateRole": {
             "access_level": "Undocumented",
-            "action": "UntagSAMLProvider",
+            "action": "UpdateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSSHPublicKeys": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "ListSSHPublicKeys",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSSHPublicKey": {
+        "ListAttachedGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "UpdateSSHPublicKey",
+            "action": "ListAttachedGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupPolicy": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "GetGroupPolicy",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedUserPolicies": {
+        "DeleteCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListAttachedUserPolicies",
+            "action": "DeleteCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserToGroup": {
+        "GetPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "AddUserToGroup",
+            "action": "GetPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCloudFrontPublicKeys": {
+        "DeleteRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ListCloudFrontPublicKeys",
+            "action": "DeleteRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePolicy": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePolicy",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstanceProfile": {
+        "TagUser": {
             "access_level": "Undocumented",
-            "action": "DeleteInstanceProfile",
+            "action": "TagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfilesForRole": {
+        "DeleteAccessKey": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfilesForRole",
+            "action": "DeleteAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRolePolicies": {
+        "GetCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListRolePolicies",
+            "action": "GetCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChangePassword": {
+        "ListGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "ChangePassword",
+            "action": "ListGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSigningCertificate": {
+        "RemoveClientIDFromOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateSigningCertificate",
+            "action": "RemoveClientIDFromOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceLinkedRole": {
+        "UntagPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateServiceLinkedRole",
+            "action": "UntagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSAMLProvider": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "CreateSAMLProvider",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOpenIDConnectProvider": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteOpenIDConnectProvider",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForPrincipalPolicy": {
+        "UpdateAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForPrincipalPolicy",
+            "action": "UpdateAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroupPolicy": {
+        "ListInstanceProfileTags": {
             "access_level": "Undocumented",
-            "action": "PutGroupPolicy",
+            "action": "ListInstanceProfileTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagRole": {
+        "UpdateAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "TagRole",
+            "action": "UpdateAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagInstanceProfile": {
+        "GetGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagInstanceProfile",
+            "action": "GetGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSigningCertificate": {
+        "GetServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteSigningCertificate",
+            "action": "GetServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachRolePolicy": {
+        "DeleteRole": {
             "access_level": "Undocumented",
-            "action": "DetachRolePolicy",
+            "action": "DeleteRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "ListPolicyVersions": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "ListPolicyVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPermissionsBoundary": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPermissionsBoundary",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPolicy": {
+        "UntagUser": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPolicy",
+            "action": "UntagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadServerCertificate": {
+        "ResetServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "UploadServerCertificate",
+            "action": "ResetServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "GetLoginProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "GetLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTags": {
+        "ListEntitiesForPolicy": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTags",
+            "action": "ListEntitiesForPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedGroupPolicies": {
+        "ListRolePolicies": {
             "access_level": "Undocumented",
-            "action": "ListAttachedGroupPolicies",
+            "action": "ListRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPolicy": {
+        "TagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "GetUserPolicy",
+            "action": "TagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceSpecificCredentials": {
+        "ListSSHPublicKeys": {
             "access_level": "Undocumented",
-            "action": "ListServiceSpecificCredentials",
+            "action": "ListSSHPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPoliciesGrantingServiceAccess": {
+        "GetOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "ListPoliciesGrantingServiceAccess",
+            "action": "GetOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccessKeyLastUsed": {
+        "DeleteUserPolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccessKeyLastUsed",
+            "action": "DeleteUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccessKey": {
+        "PutGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteAccessKey",
+            "action": "PutGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceLinkedRole": {
+        "SetSTSRegionalEndpointStatus": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceLinkedRole",
+            "action": "SetSTSRegionalEndpointStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSAMLProvider": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "GetSAMLProvider",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "GenerateOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "GenerateOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRole": {
+        "AttachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "CreateRole",
+            "action": "AttachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserFromGroup": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "RemoveUserFromGroup",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagInstanceProfile": {
+        "AttachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "TagInstanceProfile",
+            "action": "AttachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagServerCertificate": {
+        "ListInstanceProfilesForRole": {
             "access_level": "Undocumented",
-            "action": "UntagServerCertificate",
+            "action": "ListInstanceProfilesForRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachGroupPolicy": {
+        "ListPolicyTags": {
             "access_level": "Undocumented",
-            "action": "DetachGroupPolicy",
+            "action": "ListPolicyTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountPasswordPolicy": {
+        "ListUserPolicies": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountPasswordPolicy",
+            "action": "ListUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOrganizationsAccessReport": {
+        "UntagMFADevice": {
             "access_level": "Undocumented",
-            "action": "GetOrganizationsAccessReport",
+            "action": "UntagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateServiceLastAccessedDetails": {
+        "SetDefaultPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "GenerateServiceLastAccessedDetails",
+            "action": "SetDefaultPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLoginProfile": {
+        "TagRole": {
             "access_level": "Undocumented",
-            "action": "DeleteLoginProfile",
+            "action": "TagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSAMLProvider": {
+        "ListOpenIDConnectProviderTags": {
             "access_level": "Undocumented",
-            "action": "UpdateSAMLProvider",
+            "action": "ListOpenIDConnectProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSSHPublicKey": {
+        "UpdateRoleDescription": {
             "access_level": "Undocumented",
-            "action": "GetSSHPublicKey",
+            "action": "UpdateRoleDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveRoleFromInstanceProfile": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "RemoveRoleFromInstanceProfile",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountAuthorizationDetails": {
+        "DeleteSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "GetAccountAuthorizationDetails",
+            "action": "DeleteSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetails": {
+        "CreateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetails",
+            "action": "CreateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoles": {
+        "GenerateServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "ListRoles",
+            "action": "GenerateServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "TagMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "TagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetServiceSpecificCredential": {
+        "GetRole": {
             "access_level": "Undocumented",
-            "action": "ResetServiceSpecificCredential",
+            "action": "GetRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroupPolicy": {
+        "ListSTSRegionalEndpointsStatus": {
             "access_level": "Undocumented",
-            "action": "DeleteGroupPolicy",
+            "action": "ListSTSRegionalEndpointsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "ResyncMFADevice": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "ResyncMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVirtualMFADevices": {
+        "DeleteServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListVirtualMFADevices",
+            "action": "DeleteServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "DetachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "DetachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroup": {
+        "SetSecurityTokenServicePreferences": {
             "access_level": "Undocumented",
-            "action": "CreateGroup",
+            "action": "SetSecurityTokenServicePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSHPublicKey": {
+        "ListAccessKeys": {
             "access_level": "Undocumented",
-            "action": "DeleteSSHPublicKey",
+            "action": "ListAccessKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountPasswordPolicy": {
+        "UpdateAccountName": {
             "access_level": "Undocumented",
-            "action": "GetAccountPasswordPolicy",
+            "action": "UpdateAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviders": {
+        "UploadSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviders",
+            "action": "UploadSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAliases": {
+        "ListServerCertificateTags": {
             "access_level": "Undocumented",
-            "action": "ListAccountAliases",
+            "action": "ListServerCertificateTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLoginProfile": {
+        "UpdateSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "CreateLoginProfile",
+            "action": "UpdateSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroup": {
+        "UntagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateGroup",
+            "action": "UntagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPermissionsBoundary": {
+        "CreateServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "PutUserPermissionsBoundary",
+            "action": "CreateServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePolicy": {
+        "CreateOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "PutRolePolicy",
+            "action": "CreateOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOpenIDConnectProvider": {
+        "GetAccessKeyLastUsed": {
             "access_level": "Undocumented",
-            "action": "CreateOpenIDConnectProvider",
+            "action": "GetAccessKeyLastUsed",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForCustomPolicy": {
+        "UpdateServerCertificate": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForCustomPolicy",
+            "action": "UpdateServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEntitiesForPolicy": {
+        "DeleteUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ListEntitiesForPolicy",
+            "action": "DeleteUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResyncMFADevice": {
+        "TagPolicy": {
             "access_level": "Undocumented",
-            "action": "ResyncMFADevice",
+            "action": "TagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLoginProfile": {
+        "AttachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateLoginProfile",
+            "action": "AttachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSTSRegionalEndpointsStatus": {
+        "ListRoleTags": {
             "access_level": "Undocumented",
-            "action": "ListSTSRegionalEndpointsStatus",
+            "action": "ListRoleTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServerCertificate": {
+        "CreateRole": {
             "access_level": "Undocumented",
-            "action": "DeleteServerCertificate",
+            "action": "CreateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCloudFrontPublicKey": {
+        "UntagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetCloudFrontPublicKey",
+            "action": "UntagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagSAMLProvider": {
+        "UploadServerCertificate": {
             "access_level": "Undocumented",
-            "action": "TagSAMLProvider",
+            "action": "UploadServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADeviceTags": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "ListMFADeviceTags",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddClientIDToOpenIDConnectProvider": {
+        "UntagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "AddClientIDToOpenIDConnectProvider",
+            "action": "UntagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "GetOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "GetOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedRolePolicies": {
+        "ListMFADevices": {
             "access_level": "Undocumented",
-            "action": "ListAttachedRolePolicies",
+            "action": "ListMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePermissionsBoundary": {
+        "ChangePassword": {
             "access_level": "Undocumented",
-            "action": "PutRolePermissionsBoundary",
+            "action": "ChangePassword",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceSpecificCredential": {
+        "RemoveUserFromGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceSpecificCredential",
+            "action": "RemoveUserFromGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetAccountEmailAddress": {
             "access_level": "Undocumented",
             "action": "GetAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "UpdateCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "UpdateCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADevices": {
+        "SimulatePrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "ListMFADevices",
+            "action": "SimulatePrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServerCertificate": {
+        "TagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateServerCertificate",
+            "action": "TagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOpenIDConnectProviderThumbprint": {
+        "UpdateGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateOpenIDConnectProviderThumbprint",
+            "action": "UpdateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSigningCertificate": {
+        "AddClientIDToOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UploadSigningCertificate",
+            "action": "AddClientIDToOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountPasswordPolicy": {
+        "ListCloudFrontPublicKeys": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountPasswordPolicy",
+            "action": "ListCloudFrontPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSAMLProvider": {
+        "EnableMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteSAMLProvider",
+            "action": "EnableMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLinkedRoleDeletionStatus": {
+        "CreateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "GetServiceLinkedRoleDeletionStatus",
+            "action": "CreateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccessKey": {
+        "DeleteInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "CreateAccessKey",
+            "action": "DeleteInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccessKeys": {
+        "DeleteAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "ListAccessKeys",
+            "action": "DeleteAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveClientIDFromOpenIDConnectProvider": {
+        "PutRolePolicy": {
             "access_level": "Undocumented",
-            "action": "RemoveClientIDFromOpenIDConnectProvider",
+            "action": "PutRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserTags": {
+        "GetAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "ListUserTags",
+            "action": "GetAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAlias": {
+        "ListSAMLProviderTags": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAlias",
+            "action": "ListSAMLProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstanceProfile": {
+        "UpdateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "GetInstanceProfile",
+            "action": "UpdateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLoginProfile": {
+        "GetAccountSummary": {
             "access_level": "Undocumented",
-            "action": "GetLoginProfile",
+            "action": "GetAccountSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyVersion": {
+        "PutUserPolicy": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyVersion",
+            "action": "PutUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRolePolicy": {
+        "DeactivateMFADevice": {
             "access_level": "Undocumented",
-            "action": "GetRolePolicy",
+            "action": "DeactivateMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "DeleteServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "DeleteServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddRoleToInstanceProfile": {
+        "GetServiceLastAccessedDetailsWithEntities": {
             "access_level": "Undocumented",
-            "action": "AddRoleToInstanceProfile",
+            "action": "GetServiceLastAccessedDetailsWithEntities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPolicyVersion": {
+        "UpdateOpenIDConnectProviderThumbprint": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPolicyVersion",
+            "action": "UpdateOpenIDConnectProviderThumbprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificateTags": {
+        "GetSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificateTags",
+            "action": "GetSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagPolicy": {
+        "ListSigningCertificates": {
             "access_level": "Undocumented",
-            "action": "TagPolicy",
+            "action": "ListSigningCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachGroupPolicy": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "AttachGroupPolicy",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoleTags": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "ListRoleTags",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetailsWithEntities": {
+        "UpdateSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetailsWithEntities",
+            "action": "UpdateSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRole": {
+        "DeleteGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "PassRole",
+            "action": "DeleteGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyVersions": {
+        "GetContextKeysForCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "ListPolicyVersions",
+            "action": "GetContextKeysForCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificates": {
+        "CreateVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificates",
+            "action": "CreateVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredentialReport": {
+        "GetAccountAuthorizationDetails": {
             "access_level": "Undocumented",
-            "action": "GetCredentialReport",
+            "action": "GetAccountAuthorizationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityTokenServicePreferences": {
+        "ListMFADeviceTags": {
             "access_level": "Undocumented",
-            "action": "SetSecurityTokenServicePreferences",
+            "action": "ListMFADeviceTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceSpecificCredential": {
+        "PutRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "CreateServiceSpecificCredential",
+            "action": "PutRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagOpenIDConnectProvider": {
+        "ListPoliciesGrantingServiceAccess": {
             "access_level": "Undocumented",
-            "action": "TagOpenIDConnectProvider",
+            "action": "ListPoliciesGrantingServiceAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCloudFrontPublicKey": {
+        "AddUserToGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteCloudFrontPublicKey",
+            "action": "AddUserToGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServiceSpecificCredential": {
+        "CreateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "UpdateServiceSpecificCredential",
+            "action": "CreateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "identity-sync": {
@@ -73786,33 +73786,33 @@
             "orphan": false,
             "resources": [
                 "Monitor"
             ]
         }
     },
     "invoicing": {
-        "PutInvoiceEmailDeliveryPreferences": {
+        "GetInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "PutInvoiceEmailDeliveryPreferences",
+            "action": "GetInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoiceEmailDeliveryPreferences": {
+        "GetInvoicePDF": {
             "access_level": "Undocumented",
-            "action": "GetInvoiceEmailDeliveryPreferences",
+            "action": "GetInvoicePDF",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoicePDF": {
+        "PutInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "GetInvoicePDF",
+            "action": "PutInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListInvoiceSummaries": {
             "access_level": "Undocumented",
@@ -79600,889 +79600,889 @@
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         }
     },
     "iotwireless": {
-        "GetLogLevelsByResourceTypes": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetLogLevelsByResourceTypes",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDestination": {
+        "GetMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteDestination",
+            "action": "GetMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMulticastGroupWithFuotaTask": {
+        "SendDataToMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "AssociateMulticastGroupWithFuotaTask",
+            "action": "SendDataToMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevicesForWirelessDeviceImportTask": {
+        "UpdateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListDevicesForWirelessDeviceImportTask",
+            "action": "UpdateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroupSession": {
+        "UpdateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroupSession",
+            "action": "UpdateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDestination": {
+        "GetWirelessGatewayStatistics": {
             "access_level": "Undocumented",
-            "action": "CreateDestination",
+            "action": "GetWirelessGatewayStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceProfiles": {
+        "GetWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "ListDeviceProfiles",
+            "action": "GetWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessGateway": {
+        "DisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessGateway",
+            "action": "DisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromCertificate": {
+        "DeleteWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromCertificate",
+            "action": "DeleteWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestWirelessDevice": {
+        "GetFuotaTask": {
             "access_level": "Undocumented",
-            "action": "TestWirelessDevice",
+            "action": "GetFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithThing": {
+        "DisassociateAwsAccountFromPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithThing",
+            "action": "DisassociateAwsAccountFromPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroup": {
+        "DeleteQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroup",
+            "action": "DeleteQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithThing": {
+        "UpdateLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithThing",
+            "action": "UpdateLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithCertificate": {
+        "GetNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithCertificate",
+            "action": "GetNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTaskDefinition": {
+        "CancelMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTaskDefinition",
+            "action": "CancelMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLogLevelsByResourceTypes": {
+        "DeleteWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "UpdateLogLevelsByResourceTypes",
+            "action": "DeleteWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNetworkAnalyzerConfigurations": {
+        "ListDevicesForWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "ListNetworkAnalyzerConfigurations",
+            "action": "ListDevicesForWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDevice": {
+        "CreateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDevice",
+            "action": "CreateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionConfiguration": {
+        "DisassociateMulticastGroupFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetPositionConfiguration",
+            "action": "DisassociateMulticastGroupFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithMulticastGroup": {
+        "TestWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithMulticastGroup",
+            "action": "TestWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceProfile": {
+        "PutPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceProfile",
+            "action": "PutPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMulticastGroupFromFuotaTask": {
+        "UpdateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "DisassociateMulticastGroupFromFuotaTask",
+            "action": "UpdateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceProfiles": {
+        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ListServiceProfiles",
+            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMulticastGroupSession": {
+        "GetServiceEndpoint": {
             "access_level": "Undocumented",
-            "action": "CancelMulticastGroupSession",
+            "action": "GetServiceEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSingleWirelessDeviceImportTask": {
+        "GetResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartSingleWirelessDeviceImportTask",
+            "action": "GetResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerAccounts": {
+        "GetResourcePosition": {
             "access_level": "Undocumented",
-            "action": "ListPartnerAccounts",
+            "action": "GetResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterWirelessDevice": {
+        "UpdateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "DeregisterWirelessDevice",
+            "action": "UpdateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromThing": {
+        "CreateWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromThing",
+            "action": "CreateWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DisassociateWirelessDeviceFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DisassociateWirelessDeviceFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNetworkAnalyzerConfiguration": {
+        "DeleteWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "GetNetworkAnalyzerConfiguration",
+            "action": "DeleteWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTask": {
+        "GetLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTask",
+            "action": "GetLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGateway": {
+        "GetWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGateway",
+            "action": "GetWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDevices": {
+        "UpdateDestination": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDevices",
+            "action": "UpdateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromMulticastGroup": {
+        "GetDestination": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromMulticastGroup",
+            "action": "GetDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFuotaTasks": {
+        "StartNetworkAnalyzerStream": {
             "access_level": "Undocumented",
-            "action": "ListFuotaTasks",
+            "action": "StartNetworkAnalyzerStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetResourceLogLevel": {
+        "ListWirelessGateways": {
             "access_level": "Undocumented",
-            "action": "ResetResourceLogLevel",
+            "action": "ListWirelessGateways",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFuotaTask": {
+        "AssociateWirelessDeviceWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdateFuotaTask",
+            "action": "AssociateWirelessDeviceWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFuotaTask": {
+        "AssociateWirelessGatewayWithThing": {
             "access_level": "Undocumented",
-            "action": "GetFuotaTask",
+            "action": "AssociateWirelessGatewayWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNetworkAnalyzerConfiguration": {
+        "ListDeviceProfiles": {
             "access_level": "Undocumented",
-            "action": "DeleteNetworkAnalyzerConfiguration",
+            "action": "ListDeviceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNetworkAnalyzerConfiguration": {
+        "StartSingleWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "UpdateNetworkAnalyzerConfiguration",
+            "action": "StartSingleWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceImportTask": {
+        "ListMulticastGroupsByFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceImportTask",
+            "action": "ListMulticastGroupsByFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayCertificate": {
+        "GetEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayCertificate",
+            "action": "GetEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPosition": {
+        "ResetAllResourceLogLevels": {
             "access_level": "Undocumented",
-            "action": "GetPosition",
+            "action": "ResetAllResourceLogLevels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAwsAccountWithPartnerAccount": {
+        "GetWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "AssociateAwsAccountWithPartnerAccount",
+            "action": "GetWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourceLogLevel": {
+        "UpdateResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "PutResourceLogLevel",
+            "action": "UpdateResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventConfigurations": {
+        "GetPosition": {
             "access_level": "Undocumented",
-            "action": "ListEventConfigurations",
+            "action": "GetPosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDestination": {
+        "UpdatePosition": {
             "access_level": "Undocumented",
-            "action": "GetDestination",
+            "action": "UpdatePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTask": {
+        "GetServiceProfile": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTask",
+            "action": "GetServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartWirelessDeviceImportTask": {
+        "GetWirelessGatewayCertificate": {
             "access_level": "Undocumented",
-            "action": "StartWirelessDeviceImportTask",
+            "action": "GetWirelessGatewayCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceProfile": {
+        "DeleteDestination": {
             "access_level": "Undocumented",
-            "action": "GetServiceProfile",
+            "action": "DeleteDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceEventConfiguration": {
+        "PutResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceEventConfiguration",
+            "action": "PutResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceLogLevel": {
+        "ListWirelessDevices": {
             "access_level": "Undocumented",
-            "action": "GetResourceLogLevel",
+            "action": "ListWirelessDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceProfile": {
+        "CreateDestination": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceProfile",
+            "action": "CreateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDeviceImportTask": {
+        "CreateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDeviceImportTask",
+            "action": "CreateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceEndpoint": {
+        "ListEventConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetServiceEndpoint",
+            "action": "ListEventConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
+        "ListPartnerAccounts": {
             "access_level": "Undocumented",
-            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
+            "action": "ListPartnerAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayStatistics": {
+        "ListServiceProfiles": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayStatistics",
+            "action": "ListServiceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFuotaTask": {
+        "AssociateMulticastGroupWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DeleteFuotaTask",
+            "action": "AssociateMulticastGroupWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToMulticastGroup": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "SendDataToMulticastGroup",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDevice": {
+        "CreateWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDevice",
+            "action": "CreateWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionEstimate": {
+        "GetPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "GetPositionEstimate",
+            "action": "GetPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTaskDefinition": {
+        "ListWirelessGatewayTaskDefinitions": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTaskDefinition",
+            "action": "ListWirelessGatewayTaskDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventConfigurationByResourceTypes": {
+        "SendDataToWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateEventConfigurationByResourceTypes",
+            "action": "SendDataToWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromFuotaTask": {
+        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromFuotaTask",
+            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroupsByFuotaTask": {
+        "ListPositionConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroupsByFuotaTask",
+            "action": "ListPositionConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceEventConfiguration": {
+        "ListDestinations": {
             "access_level": "Undocumented",
-            "action": "GetResourceEventConfiguration",
+            "action": "ListDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMulticastGroupSession": {
+        "CreateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartMulticastGroupSession",
+            "action": "CreateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessDevice": {
+        "AssociateWirelessDeviceWithThing": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessDevice",
+            "action": "AssociateWirelessDeviceWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToWirelessDevice": {
+        "UpdateResourcePosition": {
             "access_level": "Undocumented",
-            "action": "SendDataToWirelessDevice",
+            "action": "UpdateResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartNetworkAnalyzerStream": {
+        "DisassociateWirelessDeviceFromThing": {
             "access_level": "Undocumented",
-            "action": "StartNetworkAnalyzerStream",
+            "action": "DisassociateWirelessDeviceFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourcePosition": {
+        "CreateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdateResourcePosition",
+            "action": "CreateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetAllResourceLogLevels": {
+        "StartMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "ResetAllResourceLogLevels",
+            "action": "StartMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFuotaTask": {
+        "AssociateAwsAccountWithPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "StartFuotaTask",
+            "action": "AssociateAwsAccountWithPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnerAccount": {
+        "GetPositionEstimate": {
             "access_level": "Undocumented",
-            "action": "GetPartnerAccount",
+            "action": "GetPositionEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceStatistics": {
+        "StartFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceStatistics",
+            "action": "StartFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroups": {
+        "UpdateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroups",
+            "action": "UpdateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMulticastGroup": {
+        "ListQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "CreateMulticastGroup",
+            "action": "ListQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayFirmwareInformation": {
+        "DisassociateWirelessGatewayFromCertificate": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayFirmwareInformation",
+            "action": "DisassociateWirelessGatewayFromCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGateway": {
+        "DeleteDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGateway",
+            "action": "DeleteDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTask": {
+        "DeleteServiceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTask",
+            "action": "DeleteServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPositionConfiguration": {
+        "StartWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "PutPositionConfiguration",
+            "action": "StartWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDeviceImportTask": {
+        "DeleteMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDeviceImportTask",
+            "action": "DeleteMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
+        "ListNetworkAnalyzerConfigurations": {
             "access_level": "Undocumented",
-            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
+            "action": "ListNetworkAnalyzerConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueuedMessages": {
+        "GetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "ListQueuedMessages",
+            "action": "GetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceProfile": {
+        "AssociateWirelessGatewayWithCertificate": {
             "access_level": "Undocumented",
-            "action": "CreateServiceProfile",
+            "action": "AssociateWirelessGatewayWithCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFuotaTask": {
+        "GetMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "CreateFuotaTask",
+            "action": "GetMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNetworkAnalyzerConfiguration": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateNetworkAnalyzerConfiguration",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePosition": {
+        "DeleteWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetResourcePosition",
+            "action": "DeleteWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnerAccount": {
+        "CreateDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnerAccount",
+            "action": "CreateDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDevice": {
+        "ListMulticastGroups": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDevice",
+            "action": "ListMulticastGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDestination": {
+        "ListWirelessDeviceImportTasks": {
             "access_level": "Undocumented",
-            "action": "UpdateDestination",
+            "action": "ListWirelessDeviceImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithFuotaTask": {
+        "GetDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithFuotaTask",
+            "action": "GetDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventConfigurationByResourceTypes": {
+        "DisassociateWirelessGatewayFromThing": {
             "access_level": "Undocumented",
-            "action": "GetEventConfigurationByResourceTypes",
+            "action": "DisassociateWirelessGatewayFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromThing": {
+        "GetWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromThing",
+            "action": "GetWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGateways": {
+        "CreateServiceProfile": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGateways",
+            "action": "CreateServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceProfile": {
+        "GetWirelessGatewayFirmwareInformation": {
             "access_level": "Undocumented",
-            "action": "GetDeviceProfile",
+            "action": "GetWirelessGatewayFirmwareInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAwsAccountFromPartnerAccount": {
+        "DeregisterWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "DisassociateAwsAccountFromPartnerAccount",
+            "action": "DeregisterWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDeviceImportTasks": {
+        "UpdateEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDeviceImportTasks",
+            "action": "UpdateEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePosition": {
+        "UpdateWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "UpdatePosition",
+            "action": "UpdateWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGatewayTaskDefinitions": {
+        "DeleteFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGatewayTaskDefinitions",
+            "action": "DeleteFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMulticastGroup": {
+        "AssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateMulticastGroup",
+            "action": "AssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTaskDefinition": {
+        "DeleteNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTaskDefinition",
+            "action": "DeleteNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueuedMessages": {
+        "GetPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteQueuedMessages",
+            "action": "GetPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMulticastGroup": {
+        "GetWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "DeleteMulticastGroup",
+            "action": "GetWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPositionConfigurations": {
+        "ListFuotaTasks": {
             "access_level": "Undocumented",
-            "action": "ListPositionConfigurations",
+            "action": "ListFuotaTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGateway": {
+        "GetWirelessDeviceStatistics": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGateway",
+            "action": "GetWirelessDeviceStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDestinations": {
+        "ResetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "ListDestinations",
+            "action": "ResetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceProfile": {
+        "DeleteWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceProfile",
+            "action": "DeleteWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iq": {
@@ -83087,315 +83087,315 @@
             "resources": [
                 "index",
                 "thesaurus"
             ]
         }
     },
     "kendra-ranking": {
-        "ListRescoreExecutionPlans": {
+        "UpdateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "ListRescoreExecutionPlans",
+            "action": "UpdateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRescoreExecutionPlan": {
+        "CreateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "DescribeRescoreExecutionPlan",
+            "action": "CreateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "Rescore": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "Rescore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRescoreExecutionPlan": {
+        "ListRescoreExecutionPlans": {
             "access_level": "Undocumented",
-            "action": "UpdateRescoreExecutionPlan",
+            "action": "ListRescoreExecutionPlans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRescoreExecutionPlan": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateRescoreExecutionPlan",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteRescoreExecutionPlan": {
             "access_level": "Undocumented",
             "action": "DeleteRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Rescore": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "Rescore",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DescribeRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DescribeRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesis": {
-        "DescribeStreamConsumer": {
+        "DescribeStream": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamConsumer",
+            "action": "DescribeStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTagsFromStream": {
+        "UpdateShardCount": {
             "access_level": "Undocumented",
-            "action": "RemoveTagsFromStream",
+            "action": "UpdateShardCount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStreamMode": {
+        "DeregisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "UpdateStreamMode",
+            "action": "DeregisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStream": {
+        "DisableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "DeleteStream",
+            "action": "DisableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SplitShard": {
+        "RegisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "SplitShard",
+            "action": "RegisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartStreamEncryption": {
+        "RemoveTagsFromStream": {
             "access_level": "Undocumented",
-            "action": "StartStreamEncryption",
+            "action": "RemoveTagsFromStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecords": {
+        "PutRecord": {
             "access_level": "Undocumented",
-            "action": "PutRecords",
+            "action": "PutRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopStreamEncryption": {
+        "MergeShards": {
             "access_level": "Undocumented",
-            "action": "StopStreamEncryption",
+            "action": "MergeShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecord": {
+        "ListTagsForStream": {
             "access_level": "Undocumented",
-            "action": "PutRecord",
+            "action": "ListTagsForStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "EnableEnhancedMonitoring": {
             "access_level": "Undocumented",
             "action": "EnableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreamConsumers": {
+        "ListStreams": {
             "access_level": "Undocumented",
-            "action": "ListStreamConsumers",
+            "action": "ListStreams",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecords": {
+        "SplitShard": {
             "access_level": "Undocumented",
-            "action": "GetRecords",
+            "action": "SplitShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShardIterator": {
+        "GetRecords": {
             "access_level": "Undocumented",
-            "action": "GetShardIterator",
+            "action": "GetRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShards": {
+        "StartStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "ListShards",
+            "action": "StartStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamSummary": {
+        "ListShards": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamSummary",
+            "action": "ListShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateShardCount": {
+        "DescribeStreamSummary": {
             "access_level": "Undocumented",
-            "action": "UpdateShardCount",
+            "action": "DescribeStreamSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MergeShards": {
+        "DescribeLimits": {
             "access_level": "Undocumented",
-            "action": "MergeShards",
+            "action": "DescribeLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForStream": {
+        "CreateStream": {
             "access_level": "Undocumented",
-            "action": "ListTagsForStream",
+            "action": "CreateStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterStreamConsumer": {
+        "IncreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "DeregisterStreamConsumer",
+            "action": "IncreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisableEnhancedMonitoring": {
+        "SubscribeToShard": {
             "access_level": "Undocumented",
-            "action": "DisableEnhancedMonitoring",
+            "action": "SubscribeToShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateStream": {
+        "ListStreamConsumers": {
             "access_level": "Undocumented",
-            "action": "CreateStream",
+            "action": "ListStreamConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreams": {
+        "StopStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "ListStreams",
+            "action": "StopStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeLimits": {
+        "DecreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "DescribeLimits",
+            "action": "DecreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SubscribeToShard": {
+        "UpdateStreamMode": {
             "access_level": "Undocumented",
-            "action": "SubscribeToShard",
+            "action": "UpdateStreamMode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterStreamConsumer": {
+        "DescribeStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "RegisterStreamConsumer",
+            "action": "DescribeStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecreaseStreamRetentionPeriod": {
+        "DeleteStream": {
             "access_level": "Undocumented",
-            "action": "DecreaseStreamRetentionPeriod",
+            "action": "DeleteStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTagsToStream": {
+        "PutRecords": {
             "access_level": "Undocumented",
-            "action": "AddTagsToStream",
+            "action": "PutRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStream": {
+        "GetShardIterator": {
             "access_level": "Undocumented",
-            "action": "DescribeStream",
+            "action": "GetShardIterator",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IncreaseStreamRetentionPeriod": {
+        "AddTagsToStream": {
             "access_level": "Undocumented",
-            "action": "IncreaseStreamRetentionPeriod",
+            "action": "AddTagsToStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesisanalytics": {
@@ -85962,169 +85962,169 @@
             "orphan": false,
             "resources": [
                 "function"
             ]
         }
     },
     "launchwizard": {
-        "DescribeProvisioningEvents": {
+        "ListWorkloadDeploymentOptions": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisioningEvents",
+            "action": "ListWorkloadDeploymentOptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAdditionalNode": {
+        "UpdateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "CreateAdditionalNode",
+            "action": "UpdateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSettingsSet": {
+        "DeleteAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "CreateSettingsSet",
+            "action": "DeleteAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSettingsSet": {
+        "GetResourceCostEstimate": {
             "access_level": "Undocumented",
-            "action": "DeleteSettingsSet",
+            "action": "GetResourceCostEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIpAddress": {
+        "CreateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "GetIpAddress",
+            "action": "CreateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceCostEstimate": {
+        "ListProvisionedApps": {
             "access_level": "Undocumented",
-            "action": "GetResourceCostEstimate",
+            "action": "ListProvisionedApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInfrastructureSuggestion": {
+        "DescribeSettingsSet": {
             "access_level": "Undocumented",
-            "action": "GetInfrastructureSuggestion",
+            "action": "DescribeSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedApps": {
+        "GetIpAddress": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedApps",
+            "action": "GetIpAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSettingsSet": {
+        "ListWorkloads": {
             "access_level": "Undocumented",
-            "action": "DescribeSettingsSet",
+            "action": "ListWorkloads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentOptions": {
+        "ListSettingsSets": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentOptions",
+            "action": "ListSettingsSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAdditionalNode": {
+        "StartProvisioning": {
             "access_level": "Undocumented",
-            "action": "DeleteAdditionalNode",
+            "action": "StartProvisioning",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApp": {
+        "DescribeProvisionedApp": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "DescribeProvisionedApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdditionalNodes": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "ListAdditionalNodes",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSettingsSet": {
+        "DescribeAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "UpdateSettingsSet",
+            "action": "DescribeAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSettingsSets": {
+        "ListAdditionalNodes": {
             "access_level": "Undocumented",
-            "action": "ListSettingsSets",
+            "action": "ListAdditionalNodes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloads": {
+        "CreateAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "ListWorkloads",
+            "action": "CreateAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProvisioning": {
+        "GetWorkloadAssets": {
             "access_level": "Undocumented",
-            "action": "StartProvisioning",
+            "action": "GetWorkloadAssets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAdditionalNode": {
+        "GetInfrastructureSuggestion": {
             "access_level": "Undocumented",
-            "action": "DescribeAdditionalNode",
+            "action": "GetInfrastructureSuggestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAssets": {
+        "DescribeProvisioningEvents": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAssets",
+            "action": "DescribeProvisioningEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisionedApp": {
+        "DeleteSettingsSet": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisionedApp",
+            "action": "DeleteSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "lex": {
@@ -101618,25 +101618,25 @@
             "orphan": false,
             "resources": [
                 "studio-component"
             ]
         }
     },
     "notifications": {
-        "DisassociateChannel": {
+        "CreateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "DisassociateChannel",
+            "action": "CreateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNotificationConfiguration": {
+        "AssociateChannel": {
             "access_level": "Undocumented",
-            "action": "CreateNotificationConfiguration",
+            "action": "AssociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListNotificationConfigurations": {
             "access_level": "Undocumented",
@@ -101650,145 +101650,145 @@
             "access_level": "Undocumented",
             "action": "GetNotificationEvent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterNotificationHub": {
+        "DeleteEventRule": {
             "access_level": "Undocumented",
-            "action": "DeregisterNotificationHub",
+            "action": "DeleteEventRule",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetNotificationConfiguration": {
             "access_level": "Undocumented",
             "action": "GetNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEventRule": {
+        "ListNotificationEvents": {
             "access_level": "Undocumented",
-            "action": "CreateEventRule",
+            "action": "ListNotificationEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNotificationConfiguration": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "UpdateNotificationConfiguration",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationEvents": {
+        "RegisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "ListNotificationEvents",
+            "action": "RegisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateEventRule": {
             "access_level": "Undocumented",
             "action": "UpdateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationHubs": {
+        "DisassociateChannel": {
             "access_level": "Undocumented",
-            "action": "ListNotificationHubs",
+            "action": "DisassociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListEventRules": {
             "access_level": "Undocumented",
             "action": "ListEventRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateChannel": {
-            "access_level": "Undocumented",
-            "action": "AssociateChannel",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "ListChannels": {
+        "CreateEventRule": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "CreateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEventRule": {
+        "DeregisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "DeleteEventRule",
+            "action": "DeregisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventRule": {
+        "UpdateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetEventRule",
+            "action": "UpdateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterNotificationHub": {
+        "DeleteNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "RegisterNotificationHub",
+            "action": "DeleteNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNotificationConfiguration": {
+        "ListNotificationHubs": {
             "access_level": "Undocumented",
-            "action": "DeleteNotificationConfiguration",
+            "action": "ListNotificationHubs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetEventRule": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "notifications-contacts": {
@@ -101796,65 +101796,65 @@
             "access_level": "Undocumented",
             "action": "SendActivationCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEmailContact": {
+        "CreateEmailContact": {
             "access_level": "Undocumented",
-            "action": "DeleteEmailContact",
+            "action": "CreateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEmailContact": {
+        "GetEmailContact": {
             "access_level": "Undocumented",
-            "action": "CreateEmailContact",
+            "action": "GetEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ActivateEmailContact": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ActivateEmailContact",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEmailContacts": {
+        "ActivateEmailContact": {
             "access_level": "Undocumented",
-            "action": "ListEmailContacts",
+            "action": "ActivateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEmailContact": {
+        "DeleteEmailContact": {
             "access_level": "Undocumented",
-            "action": "GetEmailContact",
+            "action": "DeleteEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListEmailContacts": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListEmailContacts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Undocumented",
@@ -104175,129 +104175,129 @@
             "orphan": false,
             "resources": [
                 "policy"
             ]
         }
     },
     "osis": {
-        "CreatePipeline": {
+        "ListPipelines": {
             "access_level": "Undocumented",
-            "action": "CreatePipeline",
+            "action": "ListPipelines",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePipeline": {
+        "GetPipeline": {
             "access_level": "Undocumented",
-            "action": "ValidatePipeline",
+            "action": "GetPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePipeline": {
+        "Ingest": {
             "access_level": "Undocumented",
-            "action": "DeletePipeline",
+            "action": "Ingest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopPipeline": {
+        "ListPipelineBlueprints": {
             "access_level": "Undocumented",
-            "action": "StopPipeline",
+            "action": "ListPipelineBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelines": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListPipelines",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeletePipeline": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeletePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipeline": {
+        "StartPipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipeline",
+            "action": "StartPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePipeline": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdatePipeline",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineChangeProgress": {
+        "GetPipelineBlueprint": {
             "access_level": "Undocumented",
-            "action": "GetPipelineChangeProgress",
+            "action": "GetPipelineBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelineBlueprints": {
+        "GetPipelineChangeProgress": {
             "access_level": "Undocumented",
-            "action": "ListPipelineBlueprints",
+            "action": "GetPipelineChangeProgress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Ingest": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "Ingest",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPipeline": {
+        "CreatePipeline": {
             "access_level": "Undocumented",
-            "action": "StartPipeline",
+            "action": "CreatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdatePipeline": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ValidatePipeline": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ValidatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineBlueprint": {
+        "StopPipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipelineBlueprint",
+            "action": "StopPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "outposts": {
@@ -104895,65 +104895,65 @@
             "orphan": false,
             "resources": [
                 "device"
             ]
         }
     },
     "payments": {
-        "DeletePaymentInstrument": {
+        "CreatePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "DeletePaymentInstrument",
+            "action": "CreatePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentStatus": {
+        "UpdatePaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "GetPaymentStatus",
+            "action": "UpdatePaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePaymentPreferences": {
+        "ListPaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "UpdatePaymentPreferences",
+            "action": "ListPaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPaymentPreferences": {
+        "DeletePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "ListPaymentPreferences",
+            "action": "DeletePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentInstrument": {
+        "GetPaymentStatus": {
             "access_level": "Undocumented",
-            "action": "GetPaymentInstrument",
+            "action": "GetPaymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MakePayment": {
+        "GetPaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "MakePayment",
+            "action": "GetPaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePaymentInstrument": {
+        "MakePayment": {
             "access_level": "Undocumented",
-            "action": "CreatePaymentInstrument",
+            "action": "MakePayment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "personalize": {
@@ -110084,281 +110084,281 @@
             "orphan": false,
             "resources": [
                 "vpcconnection"
             ]
         }
     },
     "ram": {
-        "GetResourceShareAssociations": {
+        "DeletePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareAssociations",
+            "action": "DeletePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceTypes": {
+        "GetResourceShareInvitations": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "GetResourceShareInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptResourceShareInvitation": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "AcceptResourceShareInvitation",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPermissionVersion": {
+        "DeletePermission": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPermissionVersion",
+            "action": "DeletePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicies": {
+        "ReplacePermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicies",
+            "action": "ReplacePermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionVersions": {
+        "GetResourceShareAssociations": {
             "access_level": "Undocumented",
-            "action": "ListPermissionVersions",
+            "action": "GetResourceShareAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceShare": {
+        "ListPrincipals": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceShare",
+            "action": "ListPrincipals",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromotePermissionCreatedFromPolicy": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "PromotePermissionCreatedFromPolicy",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermissionVersion": {
+        "ListReplacePermissionAssociationsWork": {
             "access_level": "Undocumented",
-            "action": "CreatePermissionVersion",
+            "action": "ListReplacePermissionAssociationsWork",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResourceShare": {
+        "CreatePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "CreateResourceShare",
+            "action": "CreatePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceSharePermissions": {
+        "DeleteResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListResourceSharePermissions",
+            "action": "DeleteResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromoteResourceShareCreatedFromPolicy": {
+        "PromotePermissionCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "PromoteResourceShareCreatedFromPolicy",
+            "action": "PromotePermissionCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceShare": {
+        "UpdateResourceShare": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceShare",
+            "action": "UpdateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareInvitations": {
+        "ListPermissionVersions": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareInvitations",
+            "action": "ListPermissionVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShares": {
+        "ListPendingInvitationResources": {
             "access_level": "Undocumented",
-            "action": "GetResourceShares",
+            "action": "ListPendingInvitationResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissions": {
+        "DisassociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "ListPermissions",
+            "action": "DisassociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReplacePermissionAssociationsWork": {
+        "ListPermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "ListReplacePermissionAssociationsWork",
+            "action": "ListPermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResources": {
+        "ListResourceSharePermissions": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "ListResourceSharePermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceSharePermission": {
+        "GetResourcePolicies": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceSharePermission",
+            "action": "GetResourcePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermissionVersion": {
+        "AssociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "DeletePermissionVersion",
+            "action": "AssociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetResourceShares": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetResourceShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceSharePermission": {
+        "PromoteResourceShareCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceSharePermission",
+            "action": "PromoteResourceShareCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionAssociations": {
+        "GetPermission": {
             "access_level": "Undocumented",
-            "action": "ListPermissionAssociations",
+            "action": "GetPermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrincipals": {
+        "DisassociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListPrincipals",
+            "action": "DisassociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateResourceShare": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableSharingWithAwsOrganization": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "EnableSharingWithAwsOrganization",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermission": {
+        "RejectResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "CreatePermission",
+            "action": "RejectResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPendingInvitationResources": {
+        "EnableSharingWithAwsOrganization": {
             "access_level": "Undocumented",
-            "action": "ListPendingInvitationResources",
+            "action": "EnableSharingWithAwsOrganization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReplacePermissionAssociations": {
+        "SetDefaultPermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ReplacePermissionAssociations",
+            "action": "SetDefaultPermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectResourceShareInvitation": {
+        "AcceptResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "RejectResourceShareInvitation",
+            "action": "AcceptResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceShare": {
+        "CreatePermission": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceShare",
+            "action": "CreatePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourceShare": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "DeleteResourceShare",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPermission": {
+        "ListPermissions": {
             "access_level": "Undocumented",
-            "action": "GetPermission",
+            "action": "ListPermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermission": {
+        "AssociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "DeletePermission",
+            "action": "AssociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "rbin": {
@@ -127808,113 +127808,113 @@
             "orphan": false,
             "resources": [
                 "schema"
             ]
         }
     },
     "scn": {
-        "RemoveAdminPermissionsForUser": {
+        "UpdateInstance": {
             "access_level": "Undocumented",
-            "action": "RemoveAdminPermissionsForUser",
+            "action": "UpdateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstance": {
+        "RemoveAdminPermissionsForUser": {
             "access_level": "Undocumented",
-            "action": "CreateInstance",
+            "action": "RemoveAdminPermissionsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSSOApplication": {
+        "CreateInstance": {
             "access_level": "Undocumented",
-            "action": "CreateSSOApplication",
+            "action": "CreateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSOApplication": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteSSOApplication",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListInstances": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssignAdminPermissionsToUser": {
+        "ListAdminUsers": {
             "access_level": "Undocumented",
-            "action": "AssignAdminPermissionsToUser",
+            "action": "ListAdminUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdminUsers": {
+        "CreateSSOApplication": {
             "access_level": "Undocumented",
-            "action": "ListAdminUsers",
+            "action": "CreateSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstances": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListInstances",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateInstance": {
+        "DescribeInstance": {
             "access_level": "Undocumented",
-            "action": "UpdateInstance",
+            "action": "DescribeInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteInstance": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstance": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteInstance",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "AssignAdminPermissionsToUser": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "AssignAdminPermissionsToUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeInstance": {
+        "DeleteSSOApplication": {
             "access_level": "Undocumented",
-            "action": "DescribeInstance",
+            "action": "DeleteSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sdb": {
@@ -142676,273 +142676,273 @@
             "condition_keys": [],
             "description": "Grants permission to list accounts that might be useful in a new query",
             "orphan": false,
             "resources": []
         }
     },
     "tnb": {
-        "CreateSolFunctionPackage": {
+        "DeleteSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "CreateSolFunctionPackage",
+            "action": "DeleteSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkInstance": {
+        "PutSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkInstance",
+            "action": "PutSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackage": {
+        "InstantiateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackage",
+            "action": "InstantiateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolFunctionPackage": {
+        "ValidateSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "UpdateSolFunctionPackage",
+            "action": "ValidateSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionInstance": {
+        "GetSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionInstance",
+            "action": "GetSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageContent": {
+        "CreateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageContent",
+            "action": "CreateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageContent": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageContent",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolFunctionPackage": {
+        "GetSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "DeleteSolFunctionPackage",
+            "action": "GetSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkInstance": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkInstance",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolNetworkPackageContent": {
+        "GetSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "PutSolNetworkPackageContent",
+            "action": "GetSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InstantiateSolNetworkInstance": {
+        "ListSolFunctionInstances": {
             "access_level": "Undocumented",
-            "action": "InstantiateSolNetworkInstance",
+            "action": "ListSolFunctionInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkInstances": {
+        "CreateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkInstances",
+            "action": "CreateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolFunctionPackageContent": {
+        "ListSolNetworkPackages": {
             "access_level": "Undocumented",
-            "action": "ValidateSolFunctionPackageContent",
+            "action": "ListSolNetworkPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageDescriptor": {
+        "UpdateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageDescriptor",
+            "action": "UpdateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkPackage": {
+        "CreateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkPackage",
+            "action": "CreateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkInstance": {
+        "ListSolFunctionPackages": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkInstance",
+            "action": "ListSolFunctionPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkInstance": {
+        "DeleteSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkInstance",
+            "action": "DeleteSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListSolNetworkOperations": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListSolNetworkOperations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkOperations": {
+        "GetSolFunctionPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkOperations",
+            "action": "GetSolFunctionPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TerminateSolNetworkInstance": {
+        "GetSolFunctionInstance": {
             "access_level": "Undocumented",
-            "action": "TerminateSolNetworkInstance",
+            "action": "GetSolFunctionInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkPackage": {
+        "GetSolNetworkPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkPackage",
+            "action": "GetSolNetworkPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSolNetworkOperation": {
+        "GetSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "CancelSolNetworkOperation",
+            "action": "GetSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackage": {
+        "GetSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackage",
+            "action": "GetSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageDescriptor": {
+        "PutSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageDescriptor",
+            "action": "PutSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionInstances": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionInstances",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CancelSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CancelSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ValidateSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ValidateSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionPackages": {
+        "DeleteSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionPackages",
+            "action": "DeleteSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolNetworkPackageContent": {
+        "GetSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ValidateSolNetworkPackageContent",
+            "action": "GetSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkPackages": {
+        "UpdateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkPackages",
+            "action": "UpdateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkOperation": {
+        "UpdateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkOperation",
+            "action": "UpdateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolFunctionPackageContent": {
+        "ListSolNetworkInstances": {
             "access_level": "Undocumented",
-            "action": "PutSolFunctionPackageContent",
+            "action": "ListSolNetworkInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkPackage": {
+        "TerminateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkPackage",
+            "action": "TerminateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "transcribe": {
```

### Comparing `iam_actions-1.2.20230513/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230514/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230513/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230514/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230513/iam_actions/generate/generate.py` & `iam_actions-1.2.20230514/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230513/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230514/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230513/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230514/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230513/iam_actions/generate/services.py` & `iam_actions-1.2.20230514/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230513/iam_actions/policies.json` & `iam_actions-1.2.20230514/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230513/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230514/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230513/iam_actions/services.json` & `iam_actions-1.2.20230514/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230513/pyproject.toml` & `iam_actions-1.2.20230514/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230513"
+version = "1.2.20230514"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230513/setup.py` & `iam_actions-1.2.20230514/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230513',
+    'version': '1.2.20230514',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230513/PKG-INFO` & `iam_actions-1.2.20230514/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230513
+Version: 1.2.20230514
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

