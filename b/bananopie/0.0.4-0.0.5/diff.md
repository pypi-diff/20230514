# Comparing `tmp/bananopie-0.0.4.tar.gz` & `tmp/bananopie-0.0.5.win-amd64.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bananopie-0.0.4.tar", last modified: Mon Dec  5 00:57:47 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

