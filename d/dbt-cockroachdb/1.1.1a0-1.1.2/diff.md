# Comparing `tmp/dbt_cockroachdb-1.1.1a0-py3-none-any.whl.zip` & `tmp/dbt_cockroachdb-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 9762 bytes, number of entries: 17
+Zip file size: 9740 bytes, number of entries: 17
 -rw-rw-r--  2.0 unx      445 b- defN 23-May-08 19:22 dbt/adapters/cockroachdb/__init__.py
 -rw-rw-r--  2.0 unx       18 b- defN 23-May-08 19:22 dbt/adapters/cockroachdb/__version__.py
 -rw-rw-r--  2.0 unx     6562 b- defN 23-May-14 09:52 dbt/adapters/cockroachdb/connections.py
 -rw-rw-r--  2.0 unx      544 b- defN 23-May-11 10:31 dbt/adapters/cockroachdb/impl.py
 -rw-rw-r--  2.0 unx       52 b- defN 23-May-08 19:22 dbt/include/cockroachdb/__init__.py
 -rw-rw-r--  2.0 unx       80 b- defN 23-May-08 19:22 dbt/include/cockroachdb/dbt_project.yml
 -rw-rw-r--  2.0 unx      283 b- defN 23-May-14 09:55 dbt/include/cockroachdb/profile_template.yml
 -rw-rw-r--  2.0 unx     5545 b- defN 23-May-08 19:22 dbt/include/cockroachdb/macros/adapters.sql
 -rw-rw-r--  2.0 unx     1186 b- defN 23-May-08 19:22 dbt/include/cockroachdb/macros/catalog.sql
 -rw-rw-r--  2.0 unx      333 b- defN 23-May-11 08:09 dbt/include/cockroachdb/macros/adapters/columns.sql
 -rw-rw-r--  2.0 unx      279 b- defN 23-May-11 08:11 dbt/include/cockroachdb/macros/adapters/freshness.sql
 -rw-rw-r--  2.0 unx      380 b- defN 23-May-11 08:11 dbt/include/cockroachdb/macros/adapters/metadata.sql
--rw-rw-r--  2.0 unx        0 b- defN 23-May-14 11:16 dbt_cockroachdb-1.1.1a0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      950 b- defN 23-May-14 11:16 dbt_cockroachdb-1.1.1a0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-14 11:16 dbt_cockroachdb-1.1.1a0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 23-May-14 11:16 dbt_cockroachdb-1.1.1a0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1608 b- defN 23-May-14 11:16 dbt_cockroachdb-1.1.1a0.dist-info/RECORD
-17 files, 18361 bytes uncompressed, 7020 bytes compressed:  61.8%
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-14 11:20 dbt_cockroachdb-1.1.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      947 b- defN 23-May-14 11:20 dbt_cockroachdb-1.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-14 11:20 dbt_cockroachdb-1.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 23-May-14 11:20 dbt_cockroachdb-1.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1598 b- defN 23-May-14 11:20 dbt_cockroachdb-1.1.2.dist-info/RECORD
+17 files, 18348 bytes uncompressed, 7018 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: dbt/include/cockroachdb/macros/adapters/freshness.sql
 Comment: 
 
 Filename: dbt/include/cockroachdb/macros/adapters/metadata.sql
 Comment: 
 
-Filename: dbt_cockroachdb-1.1.1a0.dist-info/LICENSE
+Filename: dbt_cockroachdb-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: dbt_cockroachdb-1.1.1a0.dist-info/METADATA
+Filename: dbt_cockroachdb-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: dbt_cockroachdb-1.1.1a0.dist-info/WHEEL
+Filename: dbt_cockroachdb-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: dbt_cockroachdb-1.1.1a0.dist-info/top_level.txt
+Filename: dbt_cockroachdb-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dbt_cockroachdb-1.1.1a0.dist-info/RECORD
+Filename: dbt_cockroachdb-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dbt_cockroachdb-1.1.1a0.dist-info/METADATA` & `dbt_cockroachdb-1.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-cockroachdb
-Version: 1.1.1a0
+Version: 1.1.2
 Summary: The cockroachdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/salaluf
 Author: Shoham Alaluf
 Author-email: author@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,12 +15,12 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 License-File: LICENSE
-Requires-Dist: dbt-core (==1.1.1a)
+Requires-Dist: dbt-core (==1.1.2)
 Requires-Dist: psycopg-binary (~=3.1)
 
 The cockroachdb adapter plugin for dbt (data build tool)
```

## Comparing `dbt_cockroachdb-1.1.1a0.dist-info/RECORD` & `dbt_cockroachdb-1.1.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 dbt/include/cockroachdb/dbt_project.yml,sha256=gYWdyJBRJWnOWoxFb5esAHm5CwRq7TOQqyCMLdtSKTA,80
 dbt/include/cockroachdb/profile_template.yml,sha256=BCkgGMyiqaaFGFq28hrLsQJHr-5AhOJaKxOuy9o3pNM,283
 dbt/include/cockroachdb/macros/adapters.sql,sha256=Bas5ux2QSIVYrIBAkEK6DOBDUaxR2JslYBg50a-JZlE,5545
 dbt/include/cockroachdb/macros/catalog.sql,sha256=_0sLilGHmBPYeUephDqTlTS9sQwF3_-O3uBLpAtVWg8,1186
 dbt/include/cockroachdb/macros/adapters/columns.sql,sha256=L6uKF3ze9XJvFp9wC3S9eNleOK2Q-ptQAsBiWdmAb40,333
 dbt/include/cockroachdb/macros/adapters/freshness.sql,sha256=K2gj5X3dhDB5oaJMo_CVH0RTmG_mo4aSynIgINaTAPY,279
 dbt/include/cockroachdb/macros/adapters/metadata.sql,sha256=GelhtMryAiWskUPI80PCagXcEZVVM4zZV4Tqa17Cpbg,380
-dbt_cockroachdb-1.1.1a0.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dbt_cockroachdb-1.1.1a0.dist-info/METADATA,sha256=lPNdTCDu0GZ221haLANmP-tiJdZ9MKg10SO-idawGM0,950
-dbt_cockroachdb-1.1.1a0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dbt_cockroachdb-1.1.1a0.dist-info/top_level.txt,sha256=B2YH4he17ajilEWOGCKHbRcEJlCuZKwCcgFcLPntLsE,4
-dbt_cockroachdb-1.1.1a0.dist-info/RECORD,,
+dbt_cockroachdb-1.1.2.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+dbt_cockroachdb-1.1.2.dist-info/METADATA,sha256=6Uwzg1HQEH_x6EdftSeWIVF5_rvS64dMGVGCBcnaWlg,947
+dbt_cockroachdb-1.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dbt_cockroachdb-1.1.2.dist-info/top_level.txt,sha256=B2YH4he17ajilEWOGCKHbRcEJlCuZKwCcgFcLPntLsE,4
+dbt_cockroachdb-1.1.2.dist-info/RECORD,,
```

