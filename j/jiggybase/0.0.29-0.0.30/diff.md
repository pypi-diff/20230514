# Comparing `tmp/jiggybase-0.0.29.tar.gz` & `tmp/jiggybase-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.29.tar", last modified: Tue May  9 14:31:02 2023, max compression
+gzip compressed data, was "jiggybase-0.0.30.tar", last modified: Sun May 14 15:03:50 2023, max compression
```

## Comparing `jiggybase-0.0.29.tar` & `jiggybase-0.0.30.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-09 14:31:02.157775 jiggybase-0.0.29/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.29/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     6715 2023-05-09 14:31:02.157354 jiggybase-0.0.29/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     6181 2023-05-05 04:06:19.000000 jiggybase-0.0.29/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-09 14:31:02.148782 jiggybase-0.0.29/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.29/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.29/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     8541 2023-05-09 14:30:44.000000 jiggybase-0.0.29/jiggybase/collection.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-09 14:31:02.151010 jiggybase-0.0.29/jiggybase/examples/
--rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.29/jiggybase/examples/jiggybase_upload.py
--rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.29/jiggybase/examples/upload_email_example.py
--rw-r--r--   0 wsk        (501) staff       (20)     5535 2023-05-07 14:55:55.000000 jiggybase-0.0.29/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.29/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-09 14:31:02.156534 jiggybase-0.0.29/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.29/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.29/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.29/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.29/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.29/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.29/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.29/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.29/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.29/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     3166 2023-05-07 04:31:10.000000 jiggybase-0.0.29/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.29/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.29/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.29/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.29/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.29/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-09 14:31:02.150433 jiggybase-0.0.29/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     6715 2023-05-09 14:31:02.000000 jiggybase-0.0.29/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      852 2023-05-09 14:31:02.000000 jiggybase-0.0.29/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-09 14:31:02.000000 jiggybase-0.0.29/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-09 14:31:02.000000 jiggybase-0.0.29/jiggybase.egg-info/entry_points.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-09 14:31:02.000000 jiggybase-0.0.29/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-09 14:31:02.000000 jiggybase-0.0.29/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-09 14:30:24.000000 jiggybase-0.0.29/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-09 14:31:02.157866 jiggybase-0.0.29/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-09 14:31:02.156880 jiggybase-0.0.29/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.29/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-14 15:03:50.658132 jiggybase-0.0.30/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.30/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     6809 2023-05-14 15:03:50.657686 jiggybase-0.0.30/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6275 2023-05-14 14:54:25.000000 jiggybase-0.0.30/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-14 15:03:50.647848 jiggybase-0.0.30/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.30/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2403 2023-05-14 15:03:38.000000 jiggybase-0.0.30/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     8541 2023-05-09 14:30:44.000000 jiggybase-0.0.30/jiggybase/collection.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-14 15:03:50.650662 jiggybase-0.0.30/jiggybase/examples/
+-rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.30/jiggybase/examples/jiggybase_upload.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.30/jiggybase/examples/upload_email_example.py
+-rw-r--r--   0 wsk        (501) staff       (20)     5535 2023-05-07 14:55:55.000000 jiggybase-0.0.30/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.30/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-14 15:03:50.656682 jiggybase-0.0.30/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.30/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.30/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.30/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.30/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.30/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.30/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.30/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.30/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.30/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3165 2023-05-12 19:13:14.000000 jiggybase-0.0.30/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.30/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.30/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.30/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.30/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.30/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-14 15:03:50.649999 jiggybase-0.0.30/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     6809 2023-05-14 15:03:50.000000 jiggybase-0.0.30/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      852 2023-05-14 15:03:50.000000 jiggybase-0.0.30/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-14 15:03:50.000000 jiggybase-0.0.30/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-14 15:03:50.000000 jiggybase-0.0.30/jiggybase.egg-info/entry_points.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-14 15:03:50.000000 jiggybase-0.0.30/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-14 15:03:50.000000 jiggybase-0.0.30/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-14 14:57:47.000000 jiggybase-0.0.30/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-14 15:03:50.658270 jiggybase-0.0.30/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-14 15:03:50.657128 jiggybase-0.0.30/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.30/test/test.py
```

### Comparing `jiggybase-0.0.29/LICENSE` & `jiggybase-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/PKG-INFO` & `jiggybase-0.0.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.29
+Version: 0.0.30
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -58,14 +58,15 @@
 These are the top level methods of th `JiggyBase` client, primarily used for getting the user's organizations or all collections across all organizations.
 
 - `orgs()` - Returns a list of `Org` objects the user is a member of.
 - `get_org(name_or_id: str)` - Returns the `Org` object matching the given name or ID.
 - `api_keys()` - Returns a list of the user's `ApiKey` objects.
 - `authenticated_user()` - Returns the authenticated user's `User` object.
 - `collections()` - Returns a list of all `Collection` objects in all organizations the user is a member of.
+- `collection_names()` - Returns a list of unique `Collection` names within the organization.
 - `collection(name: str)` - Returns the `Collection` object matching the given name.
 
 ### Organization
 
 Organizations in JiggyBase are a mechanism for separating different customers within the JiggyBase service.   Users can be a member of mutiple unrelated organizations.  A new user who subscribes to a JiggyBase service tier has their own oganization that they control as administrator of the organization.  Users can also be invited to an organization by existing members of the organization.
 
 For an `Org` object (e.g., `my_org = jb.get_org("<org_name>")`), you have access to the following methods:
```

### Comparing `jiggybase-0.0.29/README.md` & `jiggybase-0.0.30/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 These are the top level methods of th `JiggyBase` client, primarily used for getting the user's organizations or all collections across all organizations.
 
 - `orgs()` - Returns a list of `Org` objects the user is a member of.
 - `get_org(name_or_id: str)` - Returns the `Org` object matching the given name or ID.
 - `api_keys()` - Returns a list of the user's `ApiKey` objects.
 - `authenticated_user()` - Returns the authenticated user's `User` object.
 - `collections()` - Returns a list of all `Collection` objects in all organizations the user is a member of.
+- `collection_names()` - Returns a list of unique `Collection` names within the organization.
 - `collection(name: str)` - Returns the `Collection` object matching the given name.
 
 ### Organization
 
 Organizations in JiggyBase are a mechanism for separating different customers within the JiggyBase service.   Users can be a member of mutiple unrelated organizations.  A new user who subscribes to a JiggyBase service tier has their own oganization that they control as administrator of the organization.  Users can also be invited to an organization by existing members of the organization.
 
 For an `Org` object (e.g., `my_org = jb.get_org("<org_name>")`), you have access to the following methods:
```

### Comparing `jiggybase-0.0.29/jiggybase/client.py` & `jiggybase-0.0.30/jiggybase/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,13 +56,23 @@
         """
         collections = []
         for org in self.orgs():
             for collection in org.collections():
                 collections.append(collection)
         return collections
 
+    def collection_names(self) -> List[Collection]:
+        """
+        return the unique collection name for all collections in all Orgs that the user is a member of
+        """
+        names = []
+        for org in self.orgs():
+            for collection in org.collections():
+                names.append(collection.name)
+        return names
+            
     def collection(self, name : str) -> Collection:
         for org in self.orgs():
             for collection in org.collections():
                 if collection.name == name:
                     return collection
         raise ValueError(f'Collection "{name}" not found')
```

### Comparing `jiggybase-0.0.29/jiggybase/collection.py` & `jiggybase-0.0.30/jiggybase/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/examples/jiggybase_upload.py` & `jiggybase-0.0.30/jiggybase/examples/jiggybase_upload.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/examples/upload_email_example.py` & `jiggybase-0.0.30/jiggybase/examples/upload_email_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/jiggybase_session.py` & `jiggybase-0.0.30/jiggybase/jiggybase_session.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/login.py` & `jiggybase-0.0.30/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/models/auth.py` & `jiggybase-0.0.30/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/models/chat.py` & `jiggybase-0.0.30/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/models/chunk.py` & `jiggybase-0.0.30/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/models/collection.py` & `jiggybase-0.0.30/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/models/metadata.py` & `jiggybase-0.0.30/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/models/org.py` & `jiggybase-0.0.30/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/models/plugin.py` & `jiggybase-0.0.30/jiggybase/models/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         estr += f"text={text})"
         return estr
 
     
 class DocumentChunkWithScore(DocumentChunk):
     score: float
 
-
 class Document(BaseModel):
     id: Optional[str]
     text: str
     metadata: Optional[DocumentMetadata] = None
     mimetype: Optional[str] = None
     token_count: Optional[int] = None
```

### Comparing `jiggybase-0.0.29/jiggybase/models/plugin_config.py` & `jiggybase-0.0.30/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/models/prompt.py` & `jiggybase-0.0.30/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/models/providers.py` & `jiggybase-0.0.30/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/models/user.py` & `jiggybase-0.0.30/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase/org.py` & `jiggybase-0.0.30/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.30/jiggybase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.29
+Version: 0.0.30
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -58,14 +58,15 @@
 These are the top level methods of th `JiggyBase` client, primarily used for getting the user's organizations or all collections across all organizations.
 
 - `orgs()` - Returns a list of `Org` objects the user is a member of.
 - `get_org(name_or_id: str)` - Returns the `Org` object matching the given name or ID.
 - `api_keys()` - Returns a list of the user's `ApiKey` objects.
 - `authenticated_user()` - Returns the authenticated user's `User` object.
 - `collections()` - Returns a list of all `Collection` objects in all organizations the user is a member of.
+- `collection_names()` - Returns a list of unique `Collection` names within the organization.
 - `collection(name: str)` - Returns the `Collection` object matching the given name.
 
 ### Organization
 
 Organizations in JiggyBase are a mechanism for separating different customers within the JiggyBase service.   Users can be a member of mutiple unrelated organizations.  A new user who subscribes to a JiggyBase service tier has their own oganization that they control as administrator of the organization.  Users can also be invited to an organization by existing members of the organization.
 
 For an `Org` object (e.g., `my_org = jb.get_org("<org_name>")`), you have access to the following methods:
```

### Comparing `jiggybase-0.0.29/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.30/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.29/pyproject.toml` & `jiggybase-0.0.30/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.29"
+version = "0.0.30"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.0.29/test/test.py` & `jiggybase-0.0.30/test/test.py`

 * *Files identical despite different names*

