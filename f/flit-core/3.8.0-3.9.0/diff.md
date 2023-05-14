# Comparing `tmp/flit_core-3.8.0.tar.gz` & `tmp/flit_core-3.9.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flit_core-3.8.0.tar", last modified: Sat Nov  5 13:07:59 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

