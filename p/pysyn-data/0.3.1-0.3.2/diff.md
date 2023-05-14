# Comparing `tmp/pysyn_data-0.3.1.tar.gz` & `tmp/pysyn_data-0.3.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysyn_data-0.3.1.tar", last modified: Sun May 14 18:54:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

