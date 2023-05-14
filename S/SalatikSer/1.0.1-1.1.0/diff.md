# Comparing `tmp/SalatikSer-1.0.1.tar.gz` & `tmp/SalatikSer-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SalatikSer-1.0.1.tar", last modified: Sun May 14 11:15:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

