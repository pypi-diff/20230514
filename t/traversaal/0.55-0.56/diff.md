# Comparing `tmp/traversaal-0.55.tar.gz` & `tmp/traversaal-0.56-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traversaal-0.55.tar", last modified: Sun May 14 07:28:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

