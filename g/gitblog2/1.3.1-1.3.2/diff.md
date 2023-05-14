# Comparing `tmp/gitblog2-1.3.1.tar.gz` & `tmp/gitblog2-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitblog2-1.3.1.tar", max compression
+gzip compressed data, was "gitblog2-1.3.2.tar", max compression
```

## Comparing `gitblog2-1.3.1.tar` & `gitblog2-1.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1065 2023-02-18 16:19:17.029548 gitblog2-1.3.1/LICENSE
--rw-r--r--   0        0        0     5253 2023-05-07 19:52:22.954797 gitblog2-1.3.1/README.md
--rw-r--r--   0        0        0      261 2023-04-08 12:33:53.131324 gitblog2-1.3.1/build.py
--rw-r--r--   0        0        0       25 2023-02-18 16:19:17.029548 gitblog2-1.3.1/gitblog2/__init__.py
--rwxr-xr-x   0        0        0     1508 2023-04-10 20:54:33.366345 gitblog2-1.3.1/gitblog2/cli.py
--rw-r--r--   0        0        0    18286 2023-04-23 19:26:07.469167 gitblog2-1.3.1/gitblog2/lib.py
--rw-r--r--   0        0        0      362 2023-04-22 16:58:21.192330 gitblog2-1.3.1/gitblog2/media/favicon.svg
--rw-r--r--   0        0        0     8722 2023-04-23 20:17:32.494835 gitblog2-1.3.1/gitblog2/media/icons.svg
--rw-r--r--   0        0        0    11956 2023-04-23 20:36:33.972886 gitblog2-1.3.1/gitblog2/style.css
--rw-r--r--   0        0        0     1699 2023-05-07 18:44:44.958647 gitblog2-1.3.1/gitblog2/templates/article.html.j2
--rw-r--r--   0        0        0      216 2023-04-23 15:52:04.561501 gitblog2-1.3.1/gitblog2/templates/article_datetimes.html.j2
--rw-r--r--   0        0        0      607 2023-05-06 20:03:16.183715 gitblog2-1.3.1/gitblog2/templates/footer.html.j2
--rw-r--r--   0        0        0      317 2023-04-25 07:58:25.050819 gitblog2-1.3.1/gitblog2/templates/head_common.html.j2
--rw-r--r--   0        0        0      985 2023-05-06 19:13:55.628052 gitblog2-1.3.1/gitblog2/templates/index.html.j2
--rw-r--r--   0        0        0      586 2023-05-07 20:03:28.710948 gitblog2-1.3.1/gitblog2/templates/navbar.html.j2
--rw-r--r--   0        0        0      605 2023-05-07 20:07:58.402620 gitblog2-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 gitblog2-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-18 16:19:17.029548 gitblog2-1.3.2/LICENSE
+-rw-r--r--   0        0        0     5253 2023-05-07 19:52:22.954797 gitblog2-1.3.2/README.md
+-rw-r--r--   0        0        0      261 2023-04-08 12:33:53.131324 gitblog2-1.3.2/build.py
+-rw-r--r--   0        0        0       25 2023-02-18 16:19:17.029548 gitblog2-1.3.2/gitblog2/__init__.py
+-rwxr-xr-x   0        0        0     1508 2023-04-10 20:54:33.366345 gitblog2-1.3.2/gitblog2/cli.py
+-rw-r--r--   0        0        0    18286 2023-04-23 19:26:07.469167 gitblog2-1.3.2/gitblog2/lib.py
+-rw-r--r--   0        0        0      362 2023-04-22 16:58:21.192330 gitblog2-1.3.2/gitblog2/media/favicon.svg
+-rw-r--r--   0        0        0     8722 2023-04-23 20:17:32.494835 gitblog2-1.3.2/gitblog2/media/icons.svg
+-rw-r--r--   0        0        0     6077 2023-05-07 20:08:41.909301 gitblog2-1.3.2/gitblog2/style.css
+-rw-r--r--   0        0        0     1699 2023-05-07 18:44:44.958647 gitblog2-1.3.2/gitblog2/templates/article.html.j2
+-rw-r--r--   0        0        0      216 2023-04-23 15:52:04.561501 gitblog2-1.3.2/gitblog2/templates/article_datetimes.html.j2
+-rw-r--r--   0        0        0      607 2023-05-06 20:03:16.183715 gitblog2-1.3.2/gitblog2/templates/footer.html.j2
+-rw-r--r--   0        0        0      317 2023-04-25 07:58:25.050819 gitblog2-1.3.2/gitblog2/templates/head_common.html.j2
+-rw-r--r--   0        0        0      985 2023-05-06 19:13:55.628052 gitblog2-1.3.2/gitblog2/templates/index.html.j2
+-rw-r--r--   0        0        0      450 2023-05-07 20:12:22.720620 gitblog2-1.3.2/gitblog2/templates/navbar.html.j2
+-rw-r--r--   0        0        0      605 2023-05-07 20:12:54.672173 gitblog2-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 gitblog2-1.3.2/PKG-INFO
```

### Comparing `gitblog2-1.3.1/LICENSE` & `gitblog2-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gitblog2-1.3.1/README.md` & `gitblog2-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `gitblog2-1.3.1/gitblog2/cli.py` & `gitblog2-1.3.2/gitblog2/cli.py`

 * *Files identical despite different names*

### Comparing `gitblog2-1.3.1/gitblog2/lib.py` & `gitblog2-1.3.2/gitblog2/lib.py`

 * *Files identical despite different names*

### Comparing `gitblog2-1.3.1/gitblog2/media/icons.svg` & `gitblog2-1.3.2/gitblog2/media/icons.svg`

 * *Files identical despite different names*

### Comparing `gitblog2-1.3.1/gitblog2/templates/article.html.j2` & `gitblog2-1.3.2/gitblog2/templates/article.html.j2`

 * *Files identical despite different names*

### Comparing `gitblog2-1.3.1/gitblog2/templates/footer.html.j2` & `gitblog2-1.3.2/gitblog2/templates/footer.html.j2`

 * *Files identical despite different names*

### Comparing `gitblog2-1.3.1/gitblog2/templates/index.html.j2` & `gitblog2-1.3.2/gitblog2/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `gitblog2-1.3.1/pyproject.toml` & `gitblog2-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitblog2"
-version = "1.3.1"
+version = "1.3.2"
 description = "Git + Markdown = blog"
 authors = ["Henri Hannetel <henri.hannetel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "gitblog2"}]
 include = ["gitblog2/*"]
```

### Comparing `gitblog2-1.3.1/PKG-INFO` & `gitblog2-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitblog2
-Version: 1.3.1
+Version: 1.3.2
 Summary: Git + Markdown = blog
 License: MIT
 Author: Henri Hannetel
 Author-email: henri.hannetel@pm.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

