# Comparing `tmp/cdk-sops-secrets-1.2.94.tar.gz` & `tmp/cdk-sops-secrets-1.2.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-sops-secrets-1.2.94.tar", last modified: Sat May 13 01:10:28 2023, max compression
+gzip compressed data, was "cdk-sops-secrets-1.2.95.tar", last modified: Sun May 14 01:14:49 2023, max compression
```

## Comparing `cdk-sops-secrets-1.2.94.tar` & `cdk-sops-secrets-1.2.95.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:10:28.256811 cdk-sops-secrets-1.2.94/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-13 01:10:17.000000 cdk-sops-secrets-1.2.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-13 01:10:17.000000 cdk-sops-secrets-1.2.94/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-13 01:10:28.252811 cdk-sops-secrets-1.2.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-05-13 01:10:17.000000 cdk-sops-secrets-1.2.94/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-13 01:10:17.000000 cdk-sops-secrets-1.2.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 01:10:28.256811 cdk-sops-secrets-1.2.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-13 01:10:17.000000 cdk-sops-secrets-1.2.94/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:10:28.244810 cdk-sops-secrets-1.2.94/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:10:28.248811 cdk-sops-secrets-1.2.94/src/cdk_sops_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)    76168 2023-05-13 01:10:17.000000 cdk-sops-secrets-1.2.94/src/cdk_sops_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:10:28.248811 cdk-sops-secrets-1.2.94/src/cdk_sops_secrets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-13 01:10:17.000000 cdk-sops-secrets-1.2.94/src/cdk_sops_secrets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  7060079 2023-05-13 01:10:17.000000 cdk-sops-secrets-1.2.94/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.2.94.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 01:10:17.000000 cdk-sops-secrets-1.2.94/src/cdk_sops_secrets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:10:28.248811 cdk-sops-secrets-1.2.94/src/cdk_sops_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-13 01:10:28.000000 cdk-sops-secrets-1.2.94/src/cdk_sops_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-13 01:10:28.000000 cdk-sops-secrets-1.2.94/src/cdk_sops_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 01:10:28.000000 cdk-sops-secrets-1.2.94/src/cdk_sops_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-13 01:10:28.000000 cdk-sops-secrets-1.2.94/src/cdk_sops_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 01:10:28.000000 cdk-sops-secrets-1.2.94/src/cdk_sops_secrets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:14:49.756324 cdk-sops-secrets-1.2.95/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-14 01:14:33.000000 cdk-sops-secrets-1.2.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 01:14:33.000000 cdk-sops-secrets-1.2.95/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-14 01:14:49.756324 cdk-sops-secrets-1.2.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-05-14 01:14:33.000000 cdk-sops-secrets-1.2.95/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-14 01:14:33.000000 cdk-sops-secrets-1.2.95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:14:49.756324 cdk-sops-secrets-1.2.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-14 01:14:33.000000 cdk-sops-secrets-1.2.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:14:49.744323 cdk-sops-secrets-1.2.95/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:14:49.744323 cdk-sops-secrets-1.2.95/src/cdk_sops_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)    76168 2023-05-14 01:14:33.000000 cdk-sops-secrets-1.2.95/src/cdk_sops_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:14:49.748324 cdk-sops-secrets-1.2.95/src/cdk_sops_secrets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-14 01:14:33.000000 cdk-sops-secrets-1.2.95/src/cdk_sops_secrets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7060086 2023-05-14 01:14:33.000000 cdk-sops-secrets-1.2.95/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.2.95.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:14:33.000000 cdk-sops-secrets-1.2.95/src/cdk_sops_secrets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:14:49.748324 cdk-sops-secrets-1.2.95/src/cdk_sops_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-14 01:14:49.000000 cdk-sops-secrets-1.2.95/src/cdk_sops_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-14 01:14:49.000000 cdk-sops-secrets-1.2.95/src/cdk_sops_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:14:49.000000 cdk-sops-secrets-1.2.95/src/cdk_sops_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-14 01:14:49.000000 cdk-sops-secrets-1.2.95/src/cdk_sops_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 01:14:49.000000 cdk-sops-secrets-1.2.95/src/cdk_sops_secrets.egg-info/top_level.txt
```

### Comparing `cdk-sops-secrets-1.2.94/LICENSE` & `cdk-sops-secrets-1.2.95/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.2.94/PKG-INFO` & `cdk-sops-secrets-1.2.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.2.94
+Version: 1.2.95
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<dev@markussiebert.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/markussiebert/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-sops-secrets-1.2.94/README.md` & `cdk-sops-secrets-1.2.95/README.md`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.2.94/setup.py` & `cdk-sops-secrets-1.2.95/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-sops-secrets",
-    "version": "1.2.94",
+    "version": "1.2.95",
     "description": "CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.",
     "license": "Apache-2.0",
     "url": "https://constructs.dev/packages/cdk-sops-secrets",
     "long_description_content_type": "text/markdown",
     "author": "Markus Siebert<dev@markussiebert.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_sops_secrets",
         "cdk_sops_secrets._jsii"
     ],
     "package_data": {
         "cdk_sops_secrets._jsii": [
-            "cdk-sops-secrets@1.2.94.jsii.tgz"
+            "cdk-sops-secrets@1.2.95.jsii.tgz"
         ],
         "cdk_sops_secrets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-sops-secrets-1.2.94/src/cdk_sops_secrets/__init__.py` & `cdk-sops-secrets-1.2.95/src/cdk_sops_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.2.94/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.2.94.jsii.tgz` & `cdk-sops-secrets-1.2.95/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.2.95.jsii.tgz`

 * *Files 19% similar despite different names*

#### Comparing `cdk-sops-secrets@1.2.94.jsii.tgz-content` & `cdk-sops-secrets@1.2.95.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'je/klbq2/lMWHW0IdoiLOppkYTvcGu59LNtLqPJqGSg='", "'version'": "'1.2.95'"}*

```diff
@@ -2771,15 +2771,15 @@
             }
         }
     },
     "description": "CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.",
     "docs": {
         "stability": "experimental"
     },
-    "fingerprint": "BXpIa0s25KeE/klolyokCSYCUXJhNRBDH0wdnU3pSxI=",
+    "fingerprint": "je/klbq2/lMWHW0IdoiLOppkYTvcGu59LNtLqPJqGSg=",
     "homepage": "https://constructs.dev/packages/cdk-sops-secrets",
     "jsiiVersion": "1.81.0 (build 80988b0)",
     "keywords": [
         "cdk",
         "gitops",
         "kms",
         "mozilla/sops",
@@ -3672,9 +3672,9 @@
                     "name": "ASSET"
                 }
             ],
             "name": "UploadType",
             "symbolId": "src/index:UploadType"
         }
     },
-    "version": "1.2.94"
+    "version": "1.2.95"
 }
```

##### package/lib/index.js

###### js-beautify {}

```diff
@@ -130,15 +130,15 @@
         this.versionId = cr.getAttString('VersionId');
     }
 }
 exports.SopsSync = SopsSync;
 _a = JSII_RTTI_SYMBOL_1;
 SopsSync[_a] = {
     fqn: "cdk-sops-secrets.SopsSync",
-    version: "1.2.94"
+    version: "1.2.95"
 };
 class SopsSyncProvider extends aws_lambda_1.SingletonFunction {
     constructor(scope, id) {
         super(scope, id ?? 'SopsSyncProvider', {
             code: aws_lambda_1.Code.fromAsset(scope.node.tryGetContext('sops_sync_provider_asset_path') ||
                 path.join(__dirname, '../assets/cdk-sops-lambda.zip')),
             runtime: aws_lambda_1.Runtime.GO_1_X,
@@ -157,15 +157,15 @@
         this.sopsAgeKeys.push(key);
     }
 }
 exports.SopsSyncProvider = SopsSyncProvider;
 _b = JSII_RTTI_SYMBOL_1;
 SopsSyncProvider[_b] = {
     fqn: "cdk-sops-secrets.SopsSyncProvider",
-    version: "1.2.94"
+    version: "1.2.95"
 };
 /**
  * A drop in replacement for the normal Secret, that is populated with the encrypted
  * content of the given sops file.
  */
 class SopsSecret extends constructs_1.Construct {
     constructor(scope, id, props) {
@@ -222,10 +222,10 @@
         return this.secretValueFromJson('');
     }
 }
 exports.SopsSecret = SopsSecret;
 _c = JSII_RTTI_SYMBOL_1;
 SopsSecret[_c] = {
     fqn: "cdk-sops-secrets.SopsSecret",
-    version: "1.2.94"
+    version: "1.2.95"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiaW5kZXguanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvaW5kZXgudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSx5QkFBeUI7QUFDekIsNkJBQTZCO0FBQzdCLG1DQUFtQztBQUNuQyw2Q0FVcUI7QUFPckIsaURBQWdEO0FBQ2hELHVEQUEwRTtBQUMxRSw2REFBa0Q7QUFDbEQsdUVBT3dDO0FBQ3hDLDJDQUF1QztBQUV2QyxJQUFZLFVBU1g7QUFURCxXQUFZLFVBQVU7SUFDcEI7O09BRUc7SUFDSCwrQkFBaUIsQ0FBQTtJQUNqQjs7T0FFRztJQUNILDZCQUFlLENBQUE7QUFDakIsQ0FBQyxFQVRXLFVBQVUsR0FBVixrQkFBVSxLQUFWLGtCQUFVLFFBU3JCO0FBK0VEOztHQUVHO0FBQ0gsTUFBYSxRQUFTLFNBQVEsc0JBQVM7SUEwQnJDLFlBQVksS0FBZ0IsRUFBRSxFQUFVLEVBQUUsS0FBb0I7UUFDNUQsS0FBSyxDQUFDLEtBQUssRUFBRSxFQUFFLENBQUMsQ0FBQztRQUVqQixJQUFJLENBQUMsWUFBWSxHQUFHLEtBQUssQ0FBQyxhQUFhLElBQUksSUFBSSxDQUFDO1FBQ2hELElBQUksQ0FBQyxPQUFPLEdBQUcsS0FBSyxDQUFDLE9BQU8sSUFBSSxJQUFJLENBQUM7UUFDckMsSUFBSSxDQUFDLGlCQUFpQixHQUFHLEtBQUssQ0FBQyxlQUFlLElBQUksSUFBSSxDQUFDO1FBRXZELE1BQU0sY0FBYyxHQUNsQixLQUFLLENBQUMsY0FBYyxJQUFJLEtBQUssQ0FBQyxZQUFZLENBQUMsS0FBSyxDQUFDLEdBQUcsQ0FBQyxDQUFDLEdBQUcsRUFBRSxDQUFDO1FBQzlELFFBQVEsY0FBYyxFQUFFO1lBQ3RCLEtBQUssTUFBTSxDQUFDLENBQUM7Z0JBQ1gsSUFBSSxDQUFDLGNBQWMsR0FBRyxNQUFNLENBQUM7Z0JBQzdCLE1BQU07YUFDUDtZQUNELEtBQUssTUFBTSxDQUFDLENBQUM7Z0JBQ1gsSUFBSSxDQUFDLGNBQWMsR0FBRyxN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LENBQUM7SUFDSixDQUFDO0lBQ00sbUJBQW1CLENBQ3hCLFNBQTBCO1FBRTFCLE9BQU8sSUFBSSxDQUFDLE1BQU0sQ0FBQyxtQkFBbUIsQ0FBQyxTQUFTLENBQUMsQ0FBQztJQUNwRCxDQUFDO0lBQ00scUJBQXFCO1FBQzFCLE9BQU8sSUFBSSxDQUFDLE1BQU0sQ0FBQyxxQkFBcUIsRUFBRSxDQUFDO0lBQzdDLENBQUM7SUFDTSxNQUFNLENBQUMsTUFBK0I7UUFDM0MsT0FBTyxJQUFJLENBQUMsTUFBTSxDQUFDLE1BQU0sQ0FBQyxNQUFNLENBQUMsQ0FBQztJQUNwQyxDQUFDO0lBQ00sa0JBQWtCLENBQUMsTUFBcUI7UUFDN0MsT0FBTyxJQUFJLENBQUMsTUFBTSxDQUFDLGtCQUFrQixDQUFDLE1BQU0sQ0FBQyxDQUFDO0lBQ2hELENBQUM7SUFFTSxtQkFBbUIsQ0FBQyxTQUFpQjtRQUMxQyxPQUFPLHlCQUFXLENBQUMsY0FBYyxDQUFDLElBQUksQ0FBQyxTQUFTLEVBQUU7WUFDaEQsU0FBUztZQUNULFNBQVMsRUFBRSxJQUFJLENBQUMsSUFBSSxDQUFDLFNBQVM7U0FDL0IsQ0FBQyxDQUFDO0lBQ0wsQ0FBQztJQUVELElBQVcsV0FBVztRQUNwQixPQUFPLElBQUksQ0FBQyxtQkFBbUIsQ0FBQyxFQUFFLENBQUMsQ0FBQztJQUN0QyxDQUFDOztBQS9FSCxnQ0FnRkMiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgKiBhcyBmcyBmcm9tICdmcyc7XG5pbXBvcnQgKiBhcyBwYXRoIGZyb20gJ3BhdGgnO1xuLy9pbXBvcnQgKiBhcyBjcnlwdG8gZnJvbSAnY3J5cHRvJztcbmltcG9ydCB7XG4gIEFubm90YXRpb25zLFxuICBDdXN0b21SZXNvdXJjZSxcbiAgRHVyYXRpb24sXG4gIEZpbGVTeXN0ZW0sXG4gIExhenksXG4gIFJlbW92YWxQb2xpY3ksXG4gIFJlc291cmNlRW52aXJvbm1lbnQsXG4gIFNlY3JldFZhbHVlLFxuICBTdGFjayxcbn0gZnJvbSAnYXdzLWNkay1saWInO1xuaW1wb3J0IHtcbiAgSUdyYW50YWJsZSxcbiAgR3JhbnQsXG4gIFBvbGljeVN0YXRlbWVudCxcbiAgQWRkVG9SZXNvdXJjZVBvbGljeVJlc3VsdCxcbn0gZnJvbSAnYXdzLWNkay1saWIvYXdzLWlhbSc7XG5pbXBvcnQgeyBJS2V5LCBLZXkgfSBmcm9tICdhd3MtY2RrLWxpYi9hd3Mta21zJztcbmltcG9ydCB7IENvZGUsIFJ1bnRpbWUsIFNpbmdsZXRvbkZ1bmN0aW9uIH0gZnJvbSAnYXdzLWNkay1saWIvYXdzLWxhbWJkYSc7XG5pbXBvcnQgeyBBc3NldCB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1zMy1hc3NldHMnO1xuaW1wb3J0IHtcbiAgSVNlY3JldCxcbiAgSVNlY3JldEF0dGFjaG1lbnRUYXJnZXQsXG4gIFJvdGF0aW9uU2NoZWR1bGUsXG4gIFJvdGF0aW9uU2NoZWR1bGVPcHRpb25zLFxuICBTZWNyZXQsXG4gIFNlY3JldFByb3BzLFxufSBmcm9tICdhd3MtY2RrLWxpYi9hd3Mtc2VjcmV0c21hbmFnZXInO1xuaW1wb3J0IHsgQ29uc3RydWN0IH0gZnJvbSAnY29uc3RydWN0cyc7XG5cbmV4cG9ydCBlbnVtIFVwbG9hZFR5cGUge1xuICAvKipcbiAgICogUGFzcyB0aGUgc2VjcmV0IGRhdGEgaW5saW5lIChiYXNlNjQgZW5jb2RlZCBhbmQgY29tcHJlc3NlZClcbiAgICovXG4gIElOTElORSA9ICdJTkxJTkUnLFxuICAvKipcbiAgICogVXBsYW9kIHRoZSBzZWNlcnQgZGF0YSBhcyBhc3NldFxuICAgKi9cbiAgQVNTRVQgPSAnQVNTRVQnLFxufVxuXG4vKipcbiAqIENvbmZpZ3VyYXRpb24gb3B0aW9ucyBmb3IgdGhlIFNvcHNTeW5jXG4gKi9cbmV4cG9ydCBpbnRlcmZhY2UgU29wc1N5bmNPcHRpb25zIHtcbiAgLyoqXG4gICAqIFRoZSBjdXN0b20gcmVzb3VyY2UgcHJvdmlkZXIgdG8gdXNlLiBJZiB5b3UgZG9uJ3Qgc3BlY2lmeSBhbnksIGEgbmV3XG4gICAqIHByb3ZpZGVyIHdpbGwgYmUgY3JlYXRlZCAtIG9yIGlmIGFscmVhZHkgZXhpc3RzIHdpdGhpbiB0aGlzIHN0YWNrIC0gcmV1c2VkLlxuICAgKlxuICAgKiBAZGVmYXVsdCAtIEEgbmV3IHNpbmdsZXRvbiBwcm92aWRlciB3aWxsIGJlIGNyZWF0ZWRcbiAgICovXG4gIHJlYWRvbmx5IHNvcHNQcm92aWRlcj86IFNvcHNTeW5jUHJvdmlkZXI7XG5cbiAgLyoqXG4gICAqIFRoZSBmaWxlcGF0aCB0byB0aGUgc29wcyBmaWxlXG4gICAqL1xuICByZWFkb25seSBzb3BzRmlsZVBhdGg6IHN0cmluZztcblxuICAvKipcbiAgICogSG93IHNob3VsZCB0aGUgc2VjcmV0IGJlIHBhc3NlZCB0byB0aGUgQ3VzdG9tUmVzb3VyY2U/XG4gICAqIEBkZWZhdWx0IElOTElORVxuICAgKi9cbiAgcmVhZG9ubHkgdXBsb2FkVHlwZT86IFVwbG9hZFR5cGU7XG5cbiAgLyoqXG4gICAqIFRoZSBmb3JtYXQgb2YgdGhlIHNvcHMgZmlsZS5cbiAgICpcbiAgICogQGRlZmF1bHQgLSBUaGUgZmlsZWZvcm1hdCB3aWxsIGJlIGRlcml2ZWQgZnJvbSB0aGUgZmlsZSBlbmRpbmdcbiAgICovXG4gIHJlYWRvbmx5IHNvcHNGaWxlRm9ybWF0PzogdW5kZWZpbmVkIHwgJ2pzb24nIHwgJ3lhbWwnO1xuXG4gIC8qKlxuICAgKiBUaGUga21zS2V5IHVzZWQgdG8gZW5jcnlwdCB0aGUgc29wcyBmaWxlLiBFbmNyeXB0IHBlcm1pc3Npb25zXG4gICAqIHdpbGwgYmUgZ3JhbnRlZCB0byB0aGUgY3VzdG9tIHJlc291cmNlIHByb3ZpZGVyLlxuICAgKlxuICAgKiBAZGVmYXVsdCAtIFRoZSBrZXkgd2lsbCBiZSBkZXJpdmVkIGZyb20gdGhlIHNvcHMgZmlsZVxuICAgKi9cbiAgcmVhZG9ubHkgc29wc0ttc0tleT86IElLZXlbXTtcblxuICAvKipcbiAgICogVGhlIGFnZSBrZXkgdGhhdCBzaG91bGQgYmUgdXNlZCBmb3IgZW5jcnlwdGlvbi5cbiAgICovXG4gIHJlYWRvbmx5IHNvcHNBZ2VLZXk/OiBTZWNyZXRWYWx1ZTtcblxuICAvKipcbiAgICogU2hvdWxkIHRoZSBlbmNyeXB0ZWQgc29wcyB2YWx1ZSBzaG91bGQgYmUgY29udmVydGVkIHRvIEpTT04/XG4gICAqIE9ubHkgSlNPTiBjYW4gYmUgaGFuZGxlZCBieSBjbG91ZCBmb3JtYXRpb25zIGR5bmFtaWMgcmVmZXJlbmNlcy5cbiAgICpcbiAgICogQGRlZmF1bHQgdHJ1ZVxuICAgKi9cbiAgcmVhZG9ubHkgY29udmVydFRvSlNPTj86IGJvb2xlYW47XG5cbiAgLyoqXG4gICAqIFNob3VsZCB0aGUgc3RydWN0dXJlIGJlIGZsYXR0ZW5lZD8gVGhlIHJlc3VsdCB3aWxsIGJlIGEgZmxhdCBzdHJ1Y3R1cmUgYW5kIGFsbFxuICAgKiBvYmplY3Qga2V5cyB3aWxsIGJlIHJlcGxhY2VkIHdpdGggdGhlIGZ1bGwganNvbnBhdGggYXMga2V5LlxuICAgKiBUaGlzIGlzIHVzZWZ1bGwgZm9yIGR5bmFtaWMgcmVmZXJlbmNlcywgYXMgdGhvc2UgZG9uJ3Qgc3VwcG9ydCBuZXN0ZWQgb2JqZWN0cy5cbiAgICpcbiAgICogQGRlZmF1bHQgdHJ1ZVxuICAgKi9cbiAgcmVhZG9ubHkgZmxhdHRlbj86IGJvb2xlYW47XG5cbiAgLyoqXG4gICAqIFNoYWxsIGFsbCB2YWx1ZXMgYmUgZmxhdHRlbmVkPyBUaGlzIGlzIHVzZWZ1bGwgZm9yIGR5bmFtaWMgcmVmZXJlbmNlcywgYXMgdGhlcmVcbiAgICogYXJlIGxvb2t1cCBlcnJvcnMgZm9yIGNlcnRhaW4gZmxvYXQgdHlwZXNcbiAgICovXG4gIHJlYWRvbmx5IHN0cmluZ2lmeVZhbHVlcz86IGJvb2xlYW47XG59XG5cbi8qKlxuICogVGhlIGNvbmZpZ3VyYXRpb24gb3B0aW9ucyBleHRlbmRlZCBieSB0aGUgdGFyZ2V0IFNlY3JldFxuICovXG5leHBvcnQgaW50ZXJmYWNlIFNvcHNTeW5jUHJvcHMgZXh0ZW5kcyBTb3BzU3luY09wdGlvbnMge1xuICAvKipcbiAgICogVGhlIHNlY3JldCB0aGF0IHdpbGwgYmUgcG9wdWxhdGVkIHdpdGggdGhlIGVuY3J5cHRlZCBzb3BzIGZpbGUgY29udGVudC5cbiAgICovXG4gIHJlYWRvbmx5IHNlY3JldDogSVNlY3JldDtcbn1cblxuLyoqXG4gKiBUaGUgY3VzdG9tIHJlc291cmNlLCB0aGF0IGlzIHN5bmNpbmcgdGhlIGNvbnRlbnQgZnJvbSBhIHNvcHMgZmlsZSB0byBhIHNlY3JldC5cbiAqL1xuZXhwb3J0IGNsYXNzIFNvcHNTeW5jIGV4dGVuZHMgQ29uc3RydWN0IHtcbiAgLyoqXG4gICAqIFRoZSBjdXJyZW50IHZlcnNpb25JZCBvZiB0aGUgc2VjcmV0IHBvcHVsYXRlZCB2aWEgdGhpcyByZXNvdXJjZVxuICAgKi9cbiAgcmVhZG9ubHkgdmVyc2lvbklkOiBzdHJpbmc7XG5cbiAgLyoqXG4gICAqIFRoZSBmb3JtYXQgb2YgdGhlIGlucHV0IGZpbGVcbiAgICovXG4gIHJlYWRvbmx5IHNvcHNGaWxlRm9ybWF0OiAnanNvbicgfCAneWFtbCc7XG5cbiAgLyoqXG4gICAqIFdhcyB0aGUgZm9ybWF0IGNvbnZlcnRlZCB0byBqc29uP1xuICAgKi9cbiAgcmVhZG9ubHkgY29udmVyVG9KU09OOiBib29sZWFuO1xuXG4gIC8qKlxuICAgKiBXYXMgdGhlIHN0cnVjdHVyZSBmbGF0dGVuZWQ/XG4gICAqL1xuICByZWFkb25seSBmbGF0dGVuOiBib29sZWFuO1xuXG4gIC8qKlxuICAgKiBXZXJlIHRoZSB2YWx1ZXMgc3RyaW5naWZpZWQ/XG4gICAqL1xuICByZWFkb25seSBzdHJpbmdpZmllZFZhbHVlczogYm9vbGVhbjtcblxuICBjb25zdHJ1Y3RvcihzY29wZTogQ29uc3RydWN0LCBpZDogc3RyaW5nLCBwcm9wczogU29wc1N5bmNQcm9wcykge1xuICAgIHN1cGVyKHNjb3BlLCBpZCk7XG5cbiAgICB0aGlzLmNvbnZlclRvSlNPTiA9IHByb3BzLmNvbnZlcnRUb0pTT04gPz8gdHJ1ZTtcbiAgICB0aGlzLmZsYXR0ZW4gPSBwcm9wcy5mbGF0dGVuID8/IHRydWU7XG4gICAgdGhpcy5zdHJpbmdpZmllZFZhbHVlcyA9IHByb3BzLnN0cmluZ2lmeVZhbHVlcyA/PyB0cnVlO1xuXG4gICAgY29uc3Qgc29wc0ZpbGVGb3JtYXQgPVxuICAgICAgcHJvcHMuc29wc0ZpbGVGb3JtYXQgPz8gcHJvcHMuc29wc0ZpbGVQYXRoLnNwbGl0KCcuJykucG9wKCk7XG4gICAgc3dpdGNoIChzb3BzRmlsZUZvcm1hdCkge1xuICAgICAgY2FzZSAnanNvbic6IHtcbiAgICAgICAgdGhpcy5zb3BzRmlsZUZvcm1hdCA9ICdqc29uJztcbiAgICAgICAgYnJlYWs7XG4gICAgICB9XG4gICAgICBjYXNlICd5YW1sJzoge1xuICAgICAgICB0aGlzLnNvcHNGaWxlRm9ybWF0ID0gJ3lhbWwnO1xuICAgICAgICBicmVhaztcbiAgICAgIH1cbiAgICAgIGNhc2UgJ3ltbCc6IHtcbiAgICAgICAgdGhpcy5zb3BzRmlsZUZvcm1hdCA9ICd5YW1sJztcbiAgICAgICAgYnJlYWs7XG4gICAgICB9XG4gICAgICBkZWZhdWx0OiB7XG4gICAgICAgIHRocm93IG5ldyBFcnJvcihgVW5zdXBwb3J0ZWQgc29wc0ZpbGVGb3JtYXQgJHtzb3BzRmlsZUZvcm1hdH1gKTtcbiAgICAgIH1cbiAgICB9XG5cbiAgICBjb25zdCBwcm92aWRlciA9IHByb3BzLnNvcHNQcm92aWRlciA/PyBuZXcgU29wc1N5bmNQcm92aWRlcihzY29wZSk7XG5cbiAgICBpZiAoIWZzLmV4aXN0c1N5bmMocHJvcHMuc29wc0ZpbGVQYXRoKSkge1xuICAgICAgdGhyb3cgbmV3IEVycm9yKGBGaWxlICR7cHJvcHMuc29wc0ZpbGVQYXRofSBkb2VzIG5vdCBleGlzdCFgKTtcbiAgICB9XG5cbiAgICAvKipcbiAgICAgKiBIYW5kbGUgdXBsb2FkVHlwZSBJTkxJTkUgb3IgQVNTRVRcbiAgICAgKi9cbiAgICBjb25zdCB1cGxvYWRUeXBlID0gcHJvcHMudXBsb2FkVHlwZSA/PyBVcGxvYWRUeXBlLklOTElORTtcbiAgICBsZXQgc29wc0Fzc2V0OiBBc3NldCB8IHVuZGVmaW5lZCA9IHVuZGVmaW5lZDtcbiAgICBsZXQgc29wc0lubGluZTogeyBDb250ZW50OiBzdHJpbmc7IEhhc2g6IHN0cmluZyB9IHwgdW5kZWZpbmVkID0gdW5kZWZpbmVkO1xuICAgIGxldCBzb3BzUzNGaWxlOiB7IEJ1Y2tldDogc3RyaW5nOyBLZXk6IHN0cmluZyB9IHwgdW5kZWZpbmVkID0gdW5kZWZpbmVkO1xuXG4gICAgc3dpdGNoICh1cGxvYWRUeXBlKSB7XG4gICAgICBjYXNlIFVwbG9hZFR5cGUuSU5MSU5FOiB7XG4gICAgICAgIHNvcHNJbmxpbmUgPSB7XG4gICAgICAgICAgQ29udGVudDogZnMucmVhZEZpbGVTeW5jKHByb3BzLnNvcHNGaWxlUGF0aCkudG9TdHJpbmcoJ2Jhc2U2NCcpLFxuICAgICAgICAgIC8vIFdlIGNhbGN1bGF0ZSB0aGUgaGFzaCB0aGUgc2FtZSB3YXkgYXMgaXQgd291bGQgYmUgZG9uZSBieSBuZXcgQXNzZXQoLi4pIC0gc28gd2UgY2FuIGVuc3VyZSBzdGFibGUgdmVyc2lvbiBuYW1lcyBldmVuIGlmIHN3aXRjaGluZyBmcm9tIElOTElORSB0byBBU1NFVCBhbmQgdmljZXZlcnNhLlxuICAgICAgICAgIEhhc2g6IEZpbGVTeXN0ZW0uZmluZ2VycHJpbnQocHJvcHMuc29wc0ZpbGVQYXRoKSxcbiAgICAgICAgfTtcbiAgICAgICAgYnJlYWs7XG4gICAgICB9XG4gICAgICBjYXNlIFVwbG9hZFR5cGUuQVNTRVQ6IHtcbiAgICAgICAgc29wc0Fzc2V0ID0gbmV3IEFzc2V0KHRoaXMsICdBc3NldCcsIHtcbiAgICAgICAgICBwYXRoOiBwcm9wcy5zb3BzRmlsZVBhdGgsXG4gICAgICAgIH0pO1xuICAgICAgICBzb3BzUzNGaWxlID0ge1xuICAgICAgICAgIEJ1Y2tldDogc29wc0Fzc2V0LmJ1Y2tldC5idWNrZXROYW1lLFxuICAgICAgICAgIEtleTogc29wc0Fzc2V0LnMzT2JqZWN0S2V5LFxuICAgICAgICB9O1xuICAgICAgICBicmVhaztcbiAgICAgIH1cbiAgICB9XG5cbiAgICBpZiAocHJvdmlkZXIucm9sZSAhPT0gdW5kZWZpbmVkKSB7XG4gICAgICBpZiAocHJvcHMuc29wc0ttc0tleSAhPT0gdW5kZWZpbmVkKSB7XG4gICAgICAgIHByb3BzLnNvcHNLbXNLZXkuZm9yRWFjaCgoa2V5KSA9PiBrZXkuZ3JhbnREZWNyeXB0KHByb3ZpZGVyLnJvbGUhKSk7XG4gICAgICB9XG4gICAgICBjb25zdCBmaWxlQ29udGVudCA9IGZzLnJlYWRGaWxlU3luYyhwcm9wcy5zb3BzRmlsZVBhdGgpO1xuICAgICAgY29uc3QgcmVnZXggPSAvYXJuOmF3czprbXM6W2EtejAtOS1dKzpbXFxkXSs6a2V5XFwvW2EtejAtOS1dKy9nbTtcbiAgICAgIGNvbnN0IHJlc3VsdHMgPSByZWdleC5leGVjKGZpbGVDb250ZW50LnRvU3RyaW5nKCkpO1xuICAgICAgaWYgKHJlc3VsdHMgIT09IHVuZGVmaW5lZCkge1xuICAgICAgICByZXN1bHRzPy5mb3JFYWNoKChyZXN1bHQsIGluZGV4KSA9PlxuICAgICAgICAgIEtleS5mcm9tS2V5QXJuKHRoaXMsIGBTb3BzS2V5JHtpbmRleH1gLCByZXN1bHQpLmdyYW50RGVjcnlwdChcbiAgICAgICAgICAgIHByb3ZpZGVyLnJvbGUhLFxuICAgICAgICAgICksXG4gICAgICAgICk7XG4gICAgICB9XG4gICAgICBwcm9wcy5zZWNyZXQuZ3JhbnRXcml0ZShwcm92aWRlcik7XG4gICAgICBpZiAoc29wc0Fzc2V0ICE9PSB1bmRlZmluZWQpIHtcbiAgICAgICAgc29wc0Fzc2V0LmJ1Y2tldC5ncmFudFJlYWQocHJvdmlkZXIpO1xuICAgICAgfVxuICAgICAgLyoqXG4gICAgICAgKiBmaXhlcyAjMjM0XG4gICAgICAgKiBJZiB0aGUga21zIGtleSBmb3Igc2VjcmV0cyBlbmNyeXB0aW9uIGlzIGFuIElLZXlcbiAgICAgICAqIHRoZXJlIHdpbGwgYmUgbm8gcGVybWlzc2lvbnMgb3RoZXJ3aXNlXG4gICAgICAgKi9cbiAgICAgIGlmIChcbiAgICAgICAgcHJvcHMuc2VjcmV0LmVuY3J5cHRpb25LZXkgIT09IHVuZGVmaW5lZCAmJlxuICAgICAgICAhKHByb3BzLnNlY3JldC5lbmNyeXB0aW9uS2V5IGluc3RhbmNlb2YgS2V5KVxuICAgICAgKSB7XG4gICAgICAgIHByb3BzLnNlY3JldC5lbmNyeXB0aW9uS2V5LmdyYW50RW5jcnlwdERlY3J5cHQocHJvdmlkZXIpO1xuICAgICAgfVxuICAgIH0gZWxzZSB7XG4gICAgICBBbm5vdGF0aW9ucy5vZih0aGlzKS5hZGRXYXJuaW5nKFxuICAgICAgICBgUGxlYXNlIGVuc3VyZSBwcm9wcGVyIHBlcm1pc3Npb25zIGZvciB0aGUgcGFzc2VkIGxhbWJkYSBmdW5jdGlvbjpcXG4gIC0gd3JpdGUgQWNjZXNzIHRvIHRoZSBzZWNyZXRcXG4gIC0gZW5jcnlwdCB3aXRoIHRoZSBzb3BzS21zS2V5JHtcbiAgICAgICAgICB1cGxvYWRUeXBlID09PSBVcGxvYWRUeXBlLkFTU0VUXG4gICAgICAgICAgICA/ICdcXG4gIC0gZG93bmxvYWQgZnJvbSBhc3NldCBidWNrZXQnXG4gICAgICAgICAgICA6ICcnXG4gICAgICAgIH1gLFxuICAgICAgKTtcbiAgICB9XG4gICAgaWYgKHByb3BzLnNvcHNBZ2VLZXkgIT09IHVuZGVmaW5lZCkge1xuICAgICAgcHJvdmlkZXIuYWRkQWdlS2V5KHByb3BzLnNvcHNBZ2VLZXkpO1xuICAgIH1cblxuICAgIGNvbnN0IGNyID0gbmV3IEN1c3RvbVJlc291cmNlKHRoaXMsICdSZXNvdXJjZScsIHtcbiAgICAgIHNlcnZpY2VUb2tlbjogcHJvdmlkZXIuZnVuY3Rpb25Bcm4sXG4gICAgICByZXNvdXJjZVR5cGU6ICdDdXN0b206OlNvcHNTeW5jJyxcbiAgICAgIHByb3BlcnRpZXM6IHtcbiAgICAgICAgU2VjcmV0QVJOOiBwcm9wcy5zZWNyZXQuc2VjcmV0QXJuLFxuICAgICAgICBTb3BzUzNGaWxlOiBzb3BzUzNGaWxlLFxuICAgICAgICBTb3BzSW5saW5lOiBzb3BzSW5saW5lLFxuICAgICAgICBDb252ZXJ0VG9KU09OOiB0aGlzLmNvbnZlclRvSlNPTixcbiAgICAgICAgRmxhdHRlbjogdGhpcy5mbGF0dGVuLFxuICAgICAgICBGb3JtYXQ6IHRoaXMuc29wc0ZpbGVGb3JtYXQsXG4gICAgICAgIFN0cmluZ2lmaWVkVmFsdWVzOiB0aGlzLnN0cmluZ2lmaWVkVmFsdWVzLFxuICAgICAgfSxcbiAgICB9KTtcbiAgICB0aGlzLnZlcnNpb25JZCA9IGNyLmdldEF0dFN0cmluZygnVmVyc2lvbklkJyk7XG4gIH1cbn1cblxuZXhwb3J0IGNsYXNzIFNvcHNTeW5jUHJvdmlkZXIgZXh0ZW5kcyBTaW5nbGV0b25GdW5jdGlvbiBpbXBsZW1lbnRzIElHcmFudGFibGUge1xuICBwcml2YXRlIHNvcHNBZ2VLZXlzOiBTZWNyZXRWYWx1ZVtdO1xuXG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkPzogc3RyaW5nKSB7XG4gICAgc3VwZXIoc2NvcGUsIGlkID8/ICdTb3BzU3luY1Byb3ZpZGVyJywge1xuICAgICAgY29kZTogQ29kZS5mcm9tQXNzZXQoXG4gICAgICAgIHNjb3BlLm5vZGUudHJ5R2V0Q29udGV4dCgnc29wc19zeW5jX3Byb3ZpZGVyX2Fzc2V0X3BhdGgnKSB8fFxuICAgICAgICAgIHBhdGguam9pbihfX2Rpcm5hbWUsICcuLi9hc3NldHMvY2RrLXNvcHMtbGFtYmRhLnppcCcpLFxuICAgICAgKSxcbiAgICAgIHJ1bnRpbWU6IFJ1bnRpbWUuR09fMV9YLFxuICAgICAgaGFuZGxlcjogJ2Nkay1zb3BzLXNlY3JldHMnLFxuICAgICAgdXVpZDogJ1NvcHNTeW5jUHJvdmlkZXInLFxuICAgICAgdGltZW91dDogRHVyYXRpb24uc2Vjb25kcyg2MCksXG4gICAgICBlbnZpcm9ubWVudDoge1xuICAgICAgICBTT1BTX0FHRV9LRVk6IExhenkuc3RyaW5nKHtcbiAgICAgICAgICBwcm9kdWNlOiAoKSA9PlxuICAgICAgICAgICAgKHRoaXMuc29wc0FnZUtleXMubWFwKChzZWNyZXQpID0+IHNlY3JldC50b1N0cmluZygpKSA/PyBbXSkuam9pbihcbiAgICAgICAgICAgICAgJ1xcbicsXG4gICAgICAgICAgICApLFxuICAgICAgICB9KSxcbiAgICAgIH0sXG4gICAgfSk7XG4gICAgdGhpcy5zb3BzQWdlS2V5cyA9IFtdO1xuICB9XG5cbiAgcHVibGljIGFkZEFnZUtleShrZXk6IFNlY3JldFZhbHVlKSB7XG4gICAgdGhpcy5zb3BzQWdlS2V5cy5wdXNoKGtleSk7XG4gIH1cbn1cblxuLyoqXG4gKiBUaGUgY29uZmlndXJhdGlvbiBvcHRpb25zIG9mIHRoZSBTb3BzU2VjcmV0XG4gKi9cbmV4cG9ydCBpbnRlcmZhY2UgU29wc1NlY3JldFByb3BzIGV4dGVuZHMgU2VjcmV0UHJvcHMsIFNvcHNTeW5jT3B0aW9ucyB7fVxuXG4vKipcbiAqIEEgZHJvcCBpbiByZXBsYWNlbWVudCBmb3IgdGhlIG5vcm1hbCBTZWNyZXQsIHRoYXQgaXMgcG9wdWxhdGVkIHdpdGggdGhlIGVuY3J5cHRlZFxuICogY29udGVudCBvZiB0aGUgZ2l2ZW4gc29wcyBmaWxlLlxuICovXG5leHBvcnQgY2xhc3MgU29wc1NlY3JldCBleHRlbmRzIENvbnN0cnVjdCBpbXBsZW1lbnRzIElTZWNyZXQge1xuICBwcml2YXRlIHJlYWRvbmx5IHNlY3JldDogU2VjcmV0O1xuICByZWFkb25seSBlbmNyeXB0aW9uS2V5PzogSUtleSB8IHVuZGVmaW5lZDtcbiAgcmVhZG9ubHkgc2VjcmV0QXJuOiBzdHJpbmc7XG4gIHJlYWRvbmx5IHNlY3JldEZ1bGxBcm4/OiBzdHJpbmcgfCB1bmRlZmluZWQ7XG4gIHJlYWRvbmx5IHNlY3JldE5hbWU6IHN0cmluZztcbiAgcmVhZG9ubHkgc3RhY2s6IFN0YWNrO1xuICByZWFkb25seSBlbnY6IFJlc291cmNlRW52aXJvbm1lbnQ7XG5cbiAgcmVhZG9ubHkgc3luYzogU29wc1N5bmM7XG4gIHB1YmxpYyBjb25zdHJ1Y3RvcihzY29wZTogQ29uc3RydWN0LCBpZDogc3RyaW5nLCBwcm9wczogU29wc1NlY3JldFByb3BzKSB7XG4gICAgc3VwZXIoc2NvcGUsIGlkKTtcbiAgICB0aGlzLnNlY3JldCA9IG5ldyBTZWNyZXQodGhpcywgJ1Jlc291cmNlJywgcHJvcHMgYXMgU2VjcmV0UHJvcHMpO1xuXG4gICAgLy8gRnVsbGZpbGwgc2VjcmV0IEludGVyZmFjZVxuICAgIHRoaXMuZW5jcnlwdGlvbktleSA9IHRoaXMuc2VjcmV0LmVuY3J5cHRpb25LZXk7XG4gICAgdGhpcy5zZWNyZXRBcm4gPSB0aGlzLnNlY3JldC5zZWNyZXRBcm47XG4gICAgdGhpcy5zZWNyZXROYW1lID0gdGhpcy5zZWNyZXQuc2VjcmV0TmFtZTtcbiAgICB0aGlzLnN0YWNrID0gU3RhY2sub2Yoc2NvcGUpO1xuICAgIHRoaXMuZW52ID0ge1xuICAgICAgYWNjb3VudDogdGhpcy5zdGFjay5hY2NvdW50LFxuICAgICAgcmVnaW9uOiB0aGlzLnN0YWNrLnJlZ2lvbixcbiAgICB9O1xuXG4gICAgdGhpcy5zeW5jID0gbmV3IFNvcHNTeW5jKHRoaXMsICdTb3BzU3luYycsIHtcbiAgICAgIHNlY3JldDogdGhpcy5zZWNyZXQsXG4gICAgICAuLi4ocHJvcHMgYXMgU29wc1N5bmNPcHRpb25zKSxcbiAgICB9KTtcbiAgfVxuXG4gIC8qKlxuICAgKiBSZXR1cm5zIHRoZSBjdXJyZW50IHZlcnNpb25JZCB0aGF0IHdhcyBjcmVhdGVkIHZpYSB0aGUgU29wc1N5bmNcbiAgICovXG4gIHB1YmxpYyBjdXJyZW50VmVyc2lvbklkKCk6IHN0cmluZyB7XG4gICAgcmV0dXJuIHRoaXMuc3luYy52ZXJzaW9uSWQ7XG4gIH1cblxuICBwdWJsaWMgZ3JhbnRSZWFkKGdyYW50ZWU6IElHcmFudGFibGUsIHZlcnNpb25TdGFnZXM/OiBzdHJpbmdbXSk6IEdyYW50IHtcbiAgICByZXR1cm4gdGhpcy5zZWNyZXQuZ3JhbnRSZWFkKGdyYW50ZWUsIHZlcnNpb25TdGFnZXMpO1xuICB9XG4gIHB1YmxpYyBncmFudFdyaXRlKF9ncmFudGVlOiBJR3JhbnRhYmxlKTogR3JhbnQge1xuICAgIHRocm93IG5ldyBFcnJvcihcbiAgICAgIGBNZXRob2QgZ3JhbnRXcml0ZSguLi4pIG5vdCBhbGxvd2VkIGFzIHRoaXMgc2VjcmV0IGlzIG1hbmFnZWQgYnkgU29wc1N5bmNgLFxuICAgICk7XG4gIH1cbiAgcHVibGljIGFkZFJvdGF0aW9uU2NoZWR1bGUoXG4gICAgaWQ6IHN0cmluZyxcbiAgICBvcHRpb25zOiBSb3RhdGlvblNjaGVkdWxlT3B0aW9ucyxcbiAgKTogUm90YXRpb25TY2hlZHVsZSB7XG4gICAgdGhyb3cgbmV3IEVycm9yKFxuICAgICAgYE1ldGhvZCBhZGRUb3RhdGlvblNjaGVkdWxlKCcke2lkfScsICR7SlNPTi5zdHJpbmdpZnkoXG4gICAgICAgIG9wdGlvbnMsXG4gICAgICApfSkgbm90IGFsbG93ZWQgYXMgdGhpcyBzZWNyZXQgaXMgbWFuYWdlZCBieSBTb3BzU3luY2AsXG4gICAgKTtcbiAgfVxuICBwdWJsaWMgYWRkVG9SZXNvdXJjZVBvbGljeShcbiAgICBzdGF0ZW1lbnQ6IFBvbGljeVN0YXRlbWVudCxcbiAgKTogQWRkVG9SZXNvdXJjZVBvbGljeVJlc3VsdCB7XG4gICAgcmV0dXJuIHRoaXMuc2VjcmV0LmFkZFRvUmVzb3VyY2VQb2xpY3koc3RhdGVtZW50KTtcbiAgfVxuICBwdWJsaWMgZGVueUFjY291bnRSb290RGVsZXRlKCk6IHZvaWQge1xuICAgIHJldHVybiB0aGlzLnNlY3JldC5kZW55QWNjb3VudFJvb3REZWxldGUoKTtcbiAgfVxuICBwdWJsaWMgYXR0YWNoKHRhcmdldDogSVNlY3JldEF0dGFjaG1lbnRUYXJnZXQpOiBJU2VjcmV0IHtcbiAgICByZXR1cm4gdGhpcy5zZWNyZXQuYXR0YWNoKHRhcmdldCk7XG4gIH1cbiAgcHVibGljIGFwcGx5UmVtb3ZhbFBvbGljeShwb2xpY3k6IFJlbW92YWxQb2xpY3kpOiB2b2lkIHtcbiAgICByZXR1cm4gdGhpcy5zZWNyZXQuYXBwbHlSZW1vdmFsUG9saWN5KHBvbGljeSk7XG4gIH1cblxuICBwdWJsaWMgc2VjcmV0VmFsdWVGcm9tSnNvbihqc29uRmllbGQ6IHN0cmluZykge1xuICAgIHJldHVybiBTZWNyZXRWYWx1ZS5zZWNyZXRzTWFuYWdlcih0aGlzLnNlY3JldEFybiwge1xuICAgICAganNvbkZpZWxkLFxuICAgICAgdmVyc2lvbklkOiB0aGlzLnN5bmMudmVyc2lvbklkLFxuICAgIH0pO1xuICB9XG5cbiAgcHVibGljIGdldCBzZWNyZXRWYWx1ZSgpOiBTZWNyZXRWYWx1ZSB7XG4gICAgcmV0dXJuIHRoaXMuc2VjcmV0VmFsdWVGcm9tSnNvbignJyk7XG4gIH1cbn1cbiJdfQ==
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9716880341880341%*

 * *Differences: {"'devDependencies'": "{'projen': '^0.71.55'}", "'version'": "'1.2.95'"}*

```diff
@@ -24,15 +24,15 @@
         "jest-junit": "^15",
         "jsii": "1.x",
         "jsii-diff": "^1.81.0",
         "jsii-docgen": "^6.3.27",
         "jsii-pacmak": "^1.81.0",
         "npm-check-updates": "^16",
         "prettier": "^2.8.8",
-        "projen": "^0.71.53",
+        "projen": "^0.71.55",
         "standard-version": "^9",
         "ts-jest": "^27",
         "ts-node": "^10.9.1",
         "typescript": "^4.9.5"
     },
     "homepage": "https://constructs.dev/packages/cdk-sops-secrets",
     "jest": {
@@ -148,9 +148,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "experimental",
     "types": "lib/index.d.ts",
-    "version": "1.2.94"
+    "version": "1.2.95"
 }
```

### Comparing `cdk-sops-secrets-1.2.94/src/cdk_sops_secrets.egg-info/PKG-INFO` & `cdk-sops-secrets-1.2.95/src/cdk_sops_secrets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.2.94
+Version: 1.2.95
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<dev@markussiebert.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/markussiebert/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

