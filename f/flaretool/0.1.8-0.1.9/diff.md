# Comparing `tmp/flaretool-0.1.8.tar.gz` & `tmp/flaretool-0.1.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaretool-0.1.8.tar", last modified: Fri May 12 06:50:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

