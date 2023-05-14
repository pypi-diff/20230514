# Comparing `tmp/express-integrations-monday-1.0.8.tar.gz` & `tmp/express-integrations-monday-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\express-integrations-monday-1.0.8.tar", last modified: Sat Sep  3 05:12:41 2022, max compression
+gzip compressed data, was "dist\express-integrations-monday-1.0.9.tar", last modified: Mon Oct 24 14:59:11 2022, max compression
```

## Comparing `express-integrations-monday-1.0.8.tar` & `express-integrations-monday-1.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-09-03 05:12:41.294176 express-integrations-monday-1.0.8/
--rw-rw-rw-   0        0        0    11551 2022-06-19 15:15:09.000000 express-integrations-monday-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     1102 2022-09-03 05:12:41.294676 express-integrations-monday-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      453 2022-06-19 15:12:23.000000 express-integrations-monday-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-09-03 05:12:41.275160 express-integrations-monday-1.0.8/express_integrations_monday.egg-info/
--rw-rw-rw-   0        0        0     1102 2022-09-03 05:12:41.000000 express-integrations-monday-1.0.8/express_integrations_monday.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2022-09-03 05:12:41.000000 express-integrations-monday-1.0.8/express_integrations_monday.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-03 05:12:41.000000 express-integrations-monday-1.0.8/express_integrations_monday.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-24 16:55:20.000000 express-integrations-monday-1.0.8/express_integrations_monday.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       32 2022-09-03 05:12:41.000000 express-integrations-monday-1.0.8/express_integrations_monday.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-09-03 05:12:41.000000 express-integrations-monday-1.0.8/express_integrations_monday.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-09-03 05:12:41.280665 express-integrations-monday-1.0.8/monday/
--rw-rw-rw-   0        0        0      164 2022-08-24 14:13:01.000000 express-integrations-monday-1.0.8/monday/__init__.py
--rw-rw-rw-   0        0        0      103 2022-09-03 05:12:33.000000 express-integrations-monday-1.0.8/monday/__version__.py
--rw-rw-rw-   0        0        0     1358 2022-09-02 12:51:05.000000 express-integrations-monday-1.0.8/monday/client.py
--rw-rw-rw-   0        0        0       42 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.8/monday/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-09-03 05:12:41.281665 express-integrations-monday-1.0.8/monday/graphqlclient/
--rw-rw-rw-   0        0        0     2623 2022-09-03 04:07:49.000000 express-integrations-monday-1.0.8/monday/graphqlclient/client.py
--rw-rw-rw-   0        0        0    15693 2022-09-02 14:22:44.000000 express-integrations-monday-1.0.8/monday/query_joins.py
-drwxrwxrwx   0        0        0        0 2022-09-03 05:12:41.293175 express-integrations-monday-1.0.8/monday/resources/
--rw-rw-rw-   0        0        0      720 2022-08-24 17:25:12.000000 express-integrations-monday-1.0.8/monday/resources/__init__.py
--rw-rw-rw-   0        0        0      778 2022-09-02 12:51:05.000000 express-integrations-monday-1.0.8/monday/resources/account.py
--rw-rw-rw-   0        0        0      697 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.8/monday/resources/base.py
--rw-rw-rw-   0        0        0     1738 2022-08-24 20:53:04.000000 express-integrations-monday-1.0.8/monday/resources/boards.py
--rw-rw-rw-   0        0        0      295 2022-06-19 14:49:04.000000 express-integrations-monday-1.0.8/monday/resources/complexity.py
--rw-rw-rw-   0        0        0     1318 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.8/monday/resources/groups.py
--rw-rw-rw-   0        0        0     2087 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.8/monday/resources/items.py
--rw-rw-rw-   0        0        0      538 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.8/monday/resources/notification.py
--rw-rw-rw-   0        0        0      315 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.8/monday/resources/tags.py
--rw-rw-rw-   0        0        0      732 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.8/monday/resources/updates.py
--rw-rw-rw-   0        0        0      434 2022-08-24 17:25:12.000000 express-integrations-monday-1.0.8/monday/resources/users.py
--rw-rw-rw-   0        0        0      567 2022-06-19 14:49:04.000000 express-integrations-monday-1.0.8/monday/resources/webhooks.py
--rw-rw-rw-   0        0        0     1454 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.8/monday/resources/workspaces.py
--rw-rw-rw-   0        0        0       90 2022-06-19 15:21:31.000000 express-integrations-monday-1.0.8/monday/utils.py
--rw-rw-rw-   0        0        0       86 2022-09-03 05:12:41.295677 express-integrations-monday-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1039 2022-09-03 05:12:33.000000 express-integrations-monday-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-24 14:59:11.422280 express-integrations-monday-1.0.9/
+-rw-rw-rw-   0        0        0    11551 2022-06-19 15:15:09.000000 express-integrations-monday-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1102 2022-10-24 14:59:11.422780 express-integrations-monday-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2022-06-19 15:12:23.000000 express-integrations-monday-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-10-24 14:59:11.402264 express-integrations-monday-1.0.9/express_integrations_monday.egg-info/
+-rw-rw-rw-   0        0        0     1102 2022-10-24 14:59:11.000000 express-integrations-monday-1.0.9/express_integrations_monday.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2022-10-24 14:59:11.000000 express-integrations-monday-1.0.9/express_integrations_monday.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-24 14:59:11.000000 express-integrations-monday-1.0.9/express_integrations_monday.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-24 16:55:20.000000 express-integrations-monday-1.0.9/express_integrations_monday.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       32 2022-10-24 14:59:11.000000 express-integrations-monday-1.0.9/express_integrations_monday.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-10-24 14:59:11.000000 express-integrations-monday-1.0.9/express_integrations_monday.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-10-24 14:59:11.407268 express-integrations-monday-1.0.9/monday/
+-rw-rw-rw-   0        0        0      164 2022-08-24 14:13:01.000000 express-integrations-monday-1.0.9/monday/__init__.py
+-rw-rw-rw-   0        0        0      103 2022-10-24 14:53:59.000000 express-integrations-monday-1.0.9/monday/__version__.py
+-rw-rw-rw-   0        0        0     1358 2022-09-02 12:51:05.000000 express-integrations-monday-1.0.9/monday/client.py
+-rw-rw-rw-   0        0        0       42 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.9/monday/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-10-24 14:59:11.408269 express-integrations-monday-1.0.9/monday/graphqlclient/
+-rw-rw-rw-   0        0        0     2623 2022-09-03 04:07:49.000000 express-integrations-monday-1.0.9/monday/graphqlclient/client.py
+-rw-rw-rw-   0        0        0    15691 2022-10-24 14:00:00.000000 express-integrations-monday-1.0.9/monday/query_joins.py
+drwxrwxrwx   0        0        0        0 2022-10-24 14:59:11.421779 express-integrations-monday-1.0.9/monday/resources/
+-rw-rw-rw-   0        0        0      720 2022-08-24 17:25:12.000000 express-integrations-monday-1.0.9/monday/resources/__init__.py
+-rw-rw-rw-   0        0        0      778 2022-09-02 12:51:05.000000 express-integrations-monday-1.0.9/monday/resources/account.py
+-rw-rw-rw-   0        0        0      697 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.9/monday/resources/base.py
+-rw-rw-rw-   0        0        0     1738 2022-08-24 20:53:04.000000 express-integrations-monday-1.0.9/monday/resources/boards.py
+-rw-rw-rw-   0        0        0      295 2022-06-19 14:49:04.000000 express-integrations-monday-1.0.9/monday/resources/complexity.py
+-rw-rw-rw-   0        0        0     1318 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.9/monday/resources/groups.py
+-rw-rw-rw-   0        0        0     2087 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.9/monday/resources/items.py
+-rw-rw-rw-   0        0        0      538 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.9/monday/resources/notification.py
+-rw-rw-rw-   0        0        0      315 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.9/monday/resources/tags.py
+-rw-rw-rw-   0        0        0      732 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.9/monday/resources/updates.py
+-rw-rw-rw-   0        0        0      434 2022-08-24 17:25:12.000000 express-integrations-monday-1.0.9/monday/resources/users.py
+-rw-rw-rw-   0        0        0      567 2022-06-19 14:49:04.000000 express-integrations-monday-1.0.9/monday/resources/webhooks.py
+-rw-rw-rw-   0        0        0     1454 2022-05-05 13:45:06.000000 express-integrations-monday-1.0.9/monday/resources/workspaces.py
+-rw-rw-rw-   0        0        0       90 2022-06-19 15:21:31.000000 express-integrations-monday-1.0.9/monday/utils.py
+-rw-rw-rw-   0        0        0       86 2022-10-24 14:59:11.423781 express-integrations-monday-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1039 2022-09-03 05:12:33.000000 express-integrations-monday-1.0.9/setup.py
```

### Comparing `express-integrations-monday-1.0.8/LICENSE` & `express-integrations-monday-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/PKG-INFO` & `express-integrations-monday-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-integrations-monday
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python client library for Monday.com
 Home-page: https://github.com/expressintegrations/monday
 Author: Express Integrations
 Author-email: jasper@expressintegrations.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `express-integrations-monday-1.0.8/express_integrations_monday.egg-info/PKG-INFO` & `express-integrations-monday-1.0.9/express_integrations_monday.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-integrations-monday
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python client library for Monday.com
 Home-page: https://github.com/expressintegrations/monday
 Author: Express Integrations
 Author-email: jasper@expressintegrations.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `express-integrations-monday-1.0.8/express_integrations_monday.egg-info/SOURCES.txt` & `express-integrations-monday-1.0.9/express_integrations_monday.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/monday/client.py` & `express-integrations-monday-1.0.9/monday/client.py`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/monday/graphqlclient/client.py` & `express-integrations-monday-1.0.9/monday/graphqlclient/client.py`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/monday/query_joins.py` & `express-integrations-monday-1.0.9/monday/query_joins.py`

 * *Files 0% similar despite different names*

```diff
@@ -755,15 +755,15 @@
     return query
 
 
 def create_webhook_query(board_id, url, event, column_id: Optional[str]):
     column_config = f', config: "{{\\"columnId\\": \\"{column_id}\\"}}"' if column_id else ''
     query = '''
     mutation {
-        create_webhook (board_id:%s, url: "%s", event: %s%s) {
+        create_webhook (board_id:%s, url: %s, event: %s%s) {
             id
             board_id
         }
     }
     ''' % (board_id, url, event, column_config)
     return query
```

### Comparing `express-integrations-monday-1.0.8/monday/resources/__init__.py` & `express-integrations-monday-1.0.9/monday/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/monday/resources/account.py` & `express-integrations-monday-1.0.9/monday/resources/account.py`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/monday/resources/base.py` & `express-integrations-monday-1.0.9/monday/resources/base.py`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/monday/resources/boards.py` & `express-integrations-monday-1.0.9/monday/resources/boards.py`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/monday/resources/groups.py` & `express-integrations-monday-1.0.9/monday/resources/groups.py`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/monday/resources/items.py` & `express-integrations-monday-1.0.9/monday/resources/items.py`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/monday/resources/notification.py` & `express-integrations-monday-1.0.9/monday/resources/notification.py`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/monday/resources/updates.py` & `express-integrations-monday-1.0.9/monday/resources/updates.py`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/monday/resources/webhooks.py` & `express-integrations-monday-1.0.9/monday/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/monday/resources/workspaces.py` & `express-integrations-monday-1.0.9/monday/resources/workspaces.py`

 * *Files identical despite different names*

### Comparing `express-integrations-monday-1.0.8/setup.py` & `express-integrations-monday-1.0.9/setup.py`

 * *Files identical despite different names*

