# Comparing `tmp/tap_totango-0.1.0.tar.gz` & `tmp/tap_totango-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_totango-0.1.0.tar", max compression
+gzip compressed data, was "tap_totango-0.2.0.tar", max compression
```

## Comparing `tap_totango-0.1.0.tar` & `tap_totango-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     2944 2023-05-13 19:27:45.024895 tap_totango-0.1.0/README.md
--rw-r--r--   0        0        0     1133 2023-05-13 22:35:33.883534 tap_totango-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-13 00:04:24.083057 tap_totango-0.1.0/tap_totango/__init__.py
--rw-r--r--   0        0        0     4583 2023-05-13 16:21:54.720246 tap_totango-0.1.0/tap_totango/client.py
--rw-r--r--   0        0        0      431 2023-05-13 22:00:37.289103 tap_totango-0.1.0/tap_totango/schemas/accounts.json
--rw-r--r--   0        0        0     1878 2023-05-13 16:35:50.832342 tap_totango-0.1.0/tap_totango/schemas/events.json
--rw-r--r--   0        0        0     3382 2023-05-13 22:05:49.923900 tap_totango-0.1.0/tap_totango/streams.py
--rw-r--r--   0        0        0     4360 2023-05-13 22:01:11.100997 tap_totango-0.1.0/tap_totango/tap.py
--rw-r--r--   0        0        0     3685 1970-01-01 00:00:00.000000 tap_totango-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2944 2023-05-13 19:27:45.024895 tap_totango-0.2.0/README.md
+-rw-r--r--   0        0        0     1133 2023-05-14 01:50:14.081654 tap_totango-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-13 00:04:24.083057 tap_totango-0.2.0/tap_totango/__init__.py
+-rw-r--r--   0        0        0     4583 2023-05-13 16:21:54.720246 tap_totango-0.2.0/tap_totango/client.py
+-rw-r--r--   0        0        0      431 2023-05-13 22:00:37.289103 tap_totango-0.2.0/tap_totango/schemas/accounts.json
+-rw-r--r--   0        0        0     1878 2023-05-13 16:35:50.832342 tap_totango-0.2.0/tap_totango/schemas/events.json
+-rw-r--r--   0        0        0      918 2023-05-14 01:35:34.115672 tap_totango-0.2.0/tap_totango/schemas/users.json
+-rw-r--r--   0        0        0     4764 2023-05-14 01:28:57.199660 tap_totango-0.2.0/tap_totango/streams.py
+-rw-r--r--   0        0        0     6528 2023-05-14 01:22:13.452744 tap_totango-0.2.0/tap_totango/tap.py
+-rw-r--r--   0        0        0     3685 1970-01-01 00:00:00.000000 tap_totango-0.2.0/PKG-INFO
```

### Comparing `tap_totango-0.1.0/README.md` & `tap_totango-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tap_totango-0.1.0/pyproject.toml` & `tap_totango-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-totango"
-version = "0.1.0"
+version = "0.2.0"
 description = "`tap-totango` is a Singer tap for totango, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Edson Nogueira"]
 keywords = [
     "ELT",
     "totango",
 ]
```

### Comparing `tap_totango-0.1.0/tap_totango/client.py` & `tap_totango-0.2.0/tap_totango/client.py`

 * *Files identical despite different names*

### Comparing `tap_totango-0.1.0/tap_totango/schemas/events.json` & `tap_totango-0.2.0/tap_totango/schemas/events.json`

 * *Files identical despite different names*

### Comparing `tap_totango-0.1.0/tap_totango/streams.py` & `tap_totango-0.2.0/tap_totango/streams.py`

 * *Files 18% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     name = "accounts"
     rest_method = "POST"
 
     path = "/api/v1/search/accounts"
 
     records_jsonpath = "$.response.accounts.hits[*]"
-    primary_keys = ["id"]
+    primary_keys = ["name"]
     replication_key = None
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     schema_filepath = SCHEMAS_DIR / "accounts.json"  # noqa: ERA001
 
     def prepare_request_payload(
         self,
         context: dict | None,  # noqa: ARG002
@@ -101,7 +101,51 @@
             "offset": params["accounts_offset"],
             "count": params["accounts_count"],
             "sort_by": params["accounts_sort_by"],
             "sort_order": params["accounts_sort_order"],
         }
         data = {"query": json.dumps(query)}
         return data
+
+
+class UsersStream(totangoStream):
+    """Define custom stream."""
+
+    name = "users"
+    rest_method = "POST"
+
+    path = "/api/v1/search/users"
+
+    records_jsonpath = "$.response.users.hits[*]"
+    primary_keys = ["name"]
+    replication_key = None
+    # Optionally, you may also use `schema_filepath` in place of `schema`:
+    schema_filepath = SCHEMAS_DIR / "users.json"  # noqa: ERA001
+
+    def prepare_request_payload(
+        self,
+        context: dict | None,  # noqa: ARG002
+        next_page_token: t.Any | None,  # noqa: ARG002
+    ) -> dict | None:
+        """Prepare the data payload for the REST API request.
+
+        By default, no payload will be sent (return None).
+
+        Args:
+            context: The stream context.
+            next_page_token: The next page index or value.
+
+        Returns:
+            A dictionary with the JSON body for a POST requests.
+        """
+        # TODO: Delete this method if no payload is required. (Most REST APIs.)
+        params = self.config
+        query = {
+            "terms": params["users_terms"],
+            "fields": params["users_fields"],
+            "offset": params["users_offset"],
+            "count": params["users_count"],
+            "sort_by": params["users_sort_by"],
+            "sort_order": params["users_sort_order"],
+        }
+        data = {"query": json.dumps(query)}
+        return data
```

### Comparing `tap_totango-0.1.0/tap_totango/tap.py` & `tap_totango-0.2.0/tap_totango/tap.py`

 * *Files 20% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             required=True,
             default=0,
             description="Page number (0 is the 1st-page).",
         ),
         th.Property(
             "account_id",
             th.StringType,
-            description="Filter the results for a specific account.",
+            description="Filter the events stream results for a specific account.",
         ),
         th.Property(
             "accounts_terms",
             th.ArrayType(
                 th.ObjectType(
                     th.Property("type", th.StringType, required=True),
                     additional_properties=True,
@@ -106,20 +106,72 @@
         ),
         th.Property(
             "accounts_sort_order",
             th.StringType(allowed_values=["ASC", "DESC"]),
             default="ASC",
             description="Order to sort the accounts stream results set by.",
         ),
+        th.Property(
+            "users_terms",
+            th.ArrayType(
+                th.ObjectType(
+                    th.Property("type", th.StringType, required=True),
+                    additional_properties=True,
+                )
+            ),
+            required=True,
+            default=[],
+            description="An array containing filter conditions to use for the users stream search.",
+        ),
+        th.Property(
+            "users_fields",
+            th.ArrayType(
+                th.ObjectType(
+                    th.Property("type", th.StringType, required=True),
+                    additional_properties=True,
+                )
+            ),
+            required=True,
+            default=[],
+            description="List of fields to return as results. Note that the account name and account-id are always returned as well.",
+        ),
+        th.Property(
+            "users_count",
+            th.IntegerType,
+            default=1000,
+            description="The maximum number of users to return in the events result set. The max. value for count is 1000.",
+        ),
+        th.Property(
+            "users_offset",
+            th.IntegerType,
+            default=0,
+            description='Record number (0 states "start at record 0"). The record size can be defined using the count parameter (and limited to 1000). Tip: To page through results, ask for 1000 records (count: 1000). If you receive 1000 records, assume there’s more, in which case you want to pull the next 1000 records (offset: 1000…then 2000…etc.). Repeat paging until the number of records returned is less than 1000.',
+        ),
+        th.Property(
+            "users_sort_by",
+            th.StringType,
+            default="display_name",
+            description="Field name to sort the users stream results set by.",
+        ),
+        th.Property(
+            "users_sort_order",
+            th.StringType(allowed_values=["ASC", "DESC"]),
+            default="ASC",
+            description="Order to sort the users stream results set by.",
+        ),
     ).to_dict()
 
     def discover_streams(self) -> list[streams.totangoStream]:
         """Return a list of discovered streams.
 
         Returns:
             A list of discovered streams.
         """
-        return [streams.EventsStream(self), streams.AccountsStream(self)]
+        return [
+            streams.EventsStream(self),
+            streams.AccountsStream(self),
+            streams.UsersStream(self),
+        ]
 
 
 if __name__ == "__main__":
     Taptotango.cli()
```

### Comparing `tap_totango-0.1.0/PKG-INFO` & `tap_totango-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-totango
-Version: 0.1.0
+Version: 0.2.0
 Summary: `tap-totango` is a Singer tap for totango, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,totango
 Author: Edson Nogueira
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

