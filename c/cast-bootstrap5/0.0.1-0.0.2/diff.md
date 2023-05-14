# Comparing `tmp/cast-bootstrap5-0.0.1.tar.gz` & `tmp/cast_bootstrap5-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cast-bootstrap5-0.0.1.tar", last modified: Sun May 14 17:39:25 2023, max compression
+gzip compressed data, was "cast_bootstrap5-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cast-bootstrap5-0.0.1.tar` & `cast_bootstrap5-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     3076 2023-05-14 06:09:02.904474 cast-bootstrap5-0.0.1/.gitignore
--rw-r--r--   0        0        0     1505 2023-05-14 05:53:16.406076 cast-bootstrap5-0.0.1/LICENSE
--rw-r--r--   0        0        0     1214 2023-05-14 17:37:07.008152 cast-bootstrap5-0.0.1/README.md
--rw-r--r--   0        0        0       62 2023-05-14 12:14:44.849935 cast-bootstrap5-0.0.1/cast_bootstrap5/__init__.py
--rw-r--r--   0        0        0      104 2023-05-14 06:02:59.592444 cast-bootstrap5-0.0.1/cast_bootstrap5/apps.py
--rw-r--r--   0        0        0   194901 2023-05-14 06:06:30.960655 cast-bootstrap5-0.0.1/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css
--rw-r--r--   0        0        0     6287 2023-05-14 12:11:23.910525 cast-bootstrap5-0.0.1/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/cast.css
--rw-r--r--   0        0        0    80420 2023-05-14 06:06:51.255917 cast-bootstrap5-0.0.1/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js
--rw-r--r--   0        0        0    42819 1985-10-26 08:15:00.000000 cast-bootstrap5-0.0.1/cast_bootstrap5/static/cast_bootstrap5/js/htmx.min.js
--rw-r--r--   0        0        0    87462 1991-10-18 12:00:00.000000 cast-bootstrap5-0.0.1/cast_bootstrap5/static/cast_bootstrap5/js/jquery/jquery-3.7.0.min.js
--rw-r--r--   0        0        0      196 2023-05-14 05:59:16.067158 cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/400.html
--rw-r--r--   0        0        0      184 2023-05-14 05:59:16.067612 cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/403.html
--rw-r--r--   0        0        0      200 2023-05-14 05:59:16.068027 cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/403_csrf.html
--rw-r--r--   0        0        0      198 2023-05-14 05:59:16.068410 cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/404.html
--rw-r--r--   0        0        0      319 2023-05-14 05:59:16.068832 cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/500.html
--rw-r--r--   0        0        0      748 2023-05-14 05:59:16.069442 cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/_list_of_posts_and_paging_controls.html
--rw-r--r--   0        0        0     2803 2023-05-14 10:14:30.106436 cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/base.html
--rw-r--r--   0        0        0     2984 2023-05-14 06:54:16.139088 cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/blog_list_of_posts.html
--rw-r--r--   0        0        0      213 2023-05-14 05:59:16.070689 cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/episode.html
--rw-r--r--   0        0        0     2367 2023-05-14 05:59:16.071108 cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/pagination.html
--rw-r--r--   0        0        0     2092 2023-05-14 05:59:16.071518 cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/post.html
--rw-r--r--   0        0        0      573 2023-05-14 05:59:16.071911 cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/post_body.html
--rw-r--r--   0        0        0     1473 2023-05-14 09:11:33.661861 cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/gallery.html
--rw-r--r--   0        0        0     2146 2023-05-14 07:08:10.337131 cast-bootstrap5-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 cast-bootstrap5-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3076 2023-05-14 06:09:02.904474 cast_bootstrap5-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1505 2023-05-14 05:53:16.406076 cast_bootstrap5-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1214 2023-05-14 17:37:07.008152 cast_bootstrap5-0.0.2/README.md
+-rw-r--r--   0        0        0       63 2023-05-14 18:58:37.729184 cast_bootstrap5-0.0.2/cast_bootstrap5/__init__.py
+-rw-r--r--   0        0        0      104 2023-05-14 06:02:59.592444 cast_bootstrap5-0.0.2/cast_bootstrap5/apps.py
+-rw-r--r--   0        0        0   194901 2023-05-14 06:06:30.960655 cast_bootstrap5-0.0.2/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css
+-rw-r--r--   0        0        0     6287 2023-05-14 12:11:23.910525 cast_bootstrap5-0.0.2/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/cast.css
+-rw-r--r--   0        0        0    80420 2023-05-14 06:06:51.255917 cast_bootstrap5-0.0.2/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   333078 2023-05-14 18:57:34.863906 cast_bootstrap5-0.0.2/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0    42819 1985-10-26 08:15:00.000000 cast_bootstrap5-0.0.2/cast_bootstrap5/static/cast_bootstrap5/js/htmx.min.js
+-rw-r--r--   0        0        0    87462 1991-10-18 12:00:00.000000 cast_bootstrap5-0.0.2/cast_bootstrap5/static/cast_bootstrap5/js/jquery/jquery-3.7.0.min.js
+-rw-r--r--   0        0        0      196 2023-05-14 05:59:16.067158 cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/400.html
+-rw-r--r--   0        0        0      184 2023-05-14 05:59:16.067612 cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/403.html
+-rw-r--r--   0        0        0      200 2023-05-14 05:59:16.068027 cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/403_csrf.html
+-rw-r--r--   0        0        0      198 2023-05-14 05:59:16.068410 cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/404.html
+-rw-r--r--   0        0        0      319 2023-05-14 05:59:16.068832 cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/500.html
+-rw-r--r--   0        0        0      748 2023-05-14 05:59:16.069442 cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/_list_of_posts_and_paging_controls.html
+-rw-r--r--   0        0        0     2803 2023-05-14 10:14:30.106436 cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/base.html
+-rw-r--r--   0        0        0     2984 2023-05-14 06:54:16.139088 cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/blog_list_of_posts.html
+-rw-r--r--   0        0        0      213 2023-05-14 05:59:16.070689 cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/episode.html
+-rw-r--r--   0        0        0     2367 2023-05-14 05:59:16.071108 cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/pagination.html
+-rw-r--r--   0        0        0     2092 2023-05-14 05:59:16.071518 cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/post.html
+-rw-r--r--   0        0        0      573 2023-05-14 05:59:16.071911 cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/post_body.html
+-rw-r--r--   0        0        0     1473 2023-05-14 09:11:33.661861 cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/gallery.html
+-rw-r--r--   0        0        0     2146 2023-05-14 07:08:10.337131 cast_bootstrap5-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 cast_bootstrap5-0.0.2/PKG-INFO
```

### Comparing `cast-bootstrap5-0.0.1/.gitignore` & `cast_bootstrap5-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/LICENSE` & `cast_bootstrap5-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/README.md` & `cast_bootstrap5-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css` & `cast_bootstrap5-0.0.2/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/cast.css` & `cast_bootstrap5-0.0.2/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/cast.css`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js` & `cast_bootstrap5-0.0.2/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/cast_bootstrap5/static/cast_bootstrap5/js/htmx.min.js` & `cast_bootstrap5-0.0.2/cast_bootstrap5/static/cast_bootstrap5/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/cast_bootstrap5/static/cast_bootstrap5/js/jquery/jquery-3.7.0.min.js` & `cast_bootstrap5-0.0.2/cast_bootstrap5/static/cast_bootstrap5/js/jquery/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/_list_of_posts_and_paging_controls.html` & `cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/_list_of_posts_and_paging_controls.html`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/base.html` & `cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/base.html`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/blog_list_of_posts.html` & `cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/blog_list_of_posts.html`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/pagination.html` & `cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/pagination.html`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/post.html` & `cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/post.html`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/bootstrap5/post_body.html` & `cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/bootstrap5/post_body.html`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/cast_bootstrap5/templates/cast/gallery.html` & `cast_bootstrap5-0.0.2/cast_bootstrap5/templates/cast/gallery.html`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/pyproject.toml` & `cast_bootstrap5-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cast-bootstrap5-0.0.1/PKG-INFO` & `cast_bootstrap5-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cast-bootstrap5
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bootstrap5 theme for django-cast
 Keywords: blog,podcast,video,audio
 Author-email: Jochen Wersdörfer <jochen-castbootstrap5@wersdoerfer.de>
 Requires-Python: >=3.9
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
```

