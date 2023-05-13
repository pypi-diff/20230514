# Comparing `tmp/pyGenieScript-0.0.0b8.tar.gz` & `tmp/pyGenieScript-0.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGenieScript-0.0.0b8.tar", last modified: Thu Apr  6 21:27:58 2023, max compression
+gzip compressed data, was "pyGenieScript-0.0.0b9.tar", last modified: Wed Apr 12 01:30:35 2023, max compression
```

## Comparing `pyGenieScript-0.0.0b8.tar` & `pyGenieScript-0.0.0b9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:27:58.699025 pyGenieScript-0.0.0b8/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-06 21:27:44.000000 pyGenieScript-0.0.0b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-06 21:27:58.699025 pyGenieScript-0.0.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-06 21:27:44.000000 pyGenieScript-0.0.0b8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:27:58.699025 pyGenieScript-0.0.0b8/pyGenieScript/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-06 21:27:44.000000 pyGenieScript-0.0.0b8/pyGenieScript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18031 2023-04-06 21:27:44.000000 pyGenieScript-0.0.0b8/pyGenieScript/geniescript.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-06 21:27:44.000000 pyGenieScript-0.0.0b8/pyGenieScript/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:27:58.699025 pyGenieScript-0.0.0b8/pyGenieScript/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-06 21:27:44.000000 pyGenieScript-0.0.0b8/pyGenieScript/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-06 21:27:44.000000 pyGenieScript-0.0.0b8/pyGenieScript/tests/test_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:27:58.699025 pyGenieScript-0.0.0b8/pyGenieScript.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-06 21:27:58.000000 pyGenieScript-0.0.0b8/pyGenieScript.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-06 21:27:58.000000 pyGenieScript-0.0.0b8/pyGenieScript.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 21:27:58.000000 pyGenieScript-0.0.0b8/pyGenieScript.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-06 21:27:58.000000 pyGenieScript-0.0.0b8/pyGenieScript.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-06 21:27:58.000000 pyGenieScript-0.0.0b8/pyGenieScript.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-06 21:27:44.000000 pyGenieScript-0.0.0b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 21:27:58.699025 pyGenieScript-0.0.0b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-06 21:27:44.000000 pyGenieScript-0.0.0b8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:30:35.600906 pyGenieScript-0.0.0b9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-12 01:30:16.000000 pyGenieScript-0.0.0b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-12 01:30:35.600906 pyGenieScript-0.0.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-12 01:30:16.000000 pyGenieScript-0.0.0b9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:30:35.600906 pyGenieScript-0.0.0b9/pyGenieScript/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-12 01:30:16.000000 pyGenieScript-0.0.0b9/pyGenieScript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-12 01:30:16.000000 pyGenieScript-0.0.0b9/pyGenieScript/geniescript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-12 01:30:16.000000 pyGenieScript-0.0.0b9/pyGenieScript/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:30:35.600906 pyGenieScript-0.0.0b9/pyGenieScript/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-12 01:30:16.000000 pyGenieScript-0.0.0b9/pyGenieScript/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-12 01:30:16.000000 pyGenieScript-0.0.0b9/pyGenieScript/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:30:35.600906 pyGenieScript-0.0.0b9/pyGenieScript.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-12 01:30:35.000000 pyGenieScript-0.0.0b9/pyGenieScript.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-12 01:30:35.000000 pyGenieScript-0.0.0b9/pyGenieScript.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:30:35.000000 pyGenieScript-0.0.0b9/pyGenieScript.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 01:30:35.000000 pyGenieScript-0.0.0b9/pyGenieScript.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 01:30:35.000000 pyGenieScript-0.0.0b9/pyGenieScript.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-12 01:30:16.000000 pyGenieScript-0.0.0b9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 01:30:35.600906 pyGenieScript-0.0.0b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-12 01:30:16.000000 pyGenieScript-0.0.0b9/setup.py
```

### Comparing `pyGenieScript-0.0.0b8/LICENSE` & `pyGenieScript-0.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyGenieScript-0.0.0b8/PKG-INFO` & `pyGenieScript-0.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGenieScript
-Version: 0.0.0b8
+Version: 0.0.0b9
 Summary: A packaged GenieScript in Python
 Author: Stanford University Open Virtual Assistant Lab
 Author-email: Shicheng Liu <shicheng@cs.stanford.edu>
 Project-URL: Homepage, https://github.com/stanford-oval/pyGenieScript.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyGenieScript-0.0.0b8/README.md` & `pyGenieScript-0.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `pyGenieScript-0.0.0b8/pyGenieScript/__init__.py` & `pyGenieScript-0.0.0b9/pyGenieScript/__init__.py`

 * *Files identical despite different names*

### Comparing `pyGenieScript-0.0.0b8/pyGenieScript/geniescript.py` & `pyGenieScript-0.0.0b9/pyGenieScript/geniescript.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
         
         if 'genie_installed_ver_hash' in locals():
             print("Installed genie-toolkit version: {}".format(genie_installed_ver_hash))
         else:
             print("Installed genie-toolkit version: N/A")
         
         print("Specified genie-toolkit version: {}\nwill reinstall genie-toolkit".format(genie_desired_ver_hash))
-        print("You can disregard any npm errors above as long as the new installation is succesful")
+        print("You can disregard any npm errors above as long as the new installation is successful")
         return True
     
     def __retrieve_port_number(self, process):
         while True:
             output = process.stdout.readline()
             if output == '' and process.poll() is not None:
                 break
```

### Comparing `pyGenieScript-0.0.0b8/pyGenieScript/tests/__init__.py` & `pyGenieScript-0.0.0b9/pyGenieScript/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyGenieScript-0.0.0b8/pyGenieScript/tests/test_setup.py` & `pyGenieScript-0.0.0b9/pyGenieScript/tests/test_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pyGenieScript.geniescript
 
 def test_genienlp():
     if "installgenienlp" in os.environ:
         subprocess.check_call([sys.executable, "-m", "pip", "install", 'genienlp==0.7.0a4'])
     
     if (not shutil.which('genienlp')):
-        # genienlp is not succesfully installed
+        # genienlp is not successfully installed
         raise ValueError("genienlp is not correctly installed")
     assert(True)
 
 def test_setup():
     genie = pyGenieScript.geniescript.Genie()
     genie.initialize('yelp', 'yelp')
     response = genie.query("show me a chinese restaurant")
```

### Comparing `pyGenieScript-0.0.0b8/pyGenieScript.egg-info/PKG-INFO` & `pyGenieScript-0.0.0b9/pyGenieScript.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGenieScript
-Version: 0.0.0b8
+Version: 0.0.0b9
 Summary: A packaged GenieScript in Python
 Author: Stanford University Open Virtual Assistant Lab
 Author-email: Shicheng Liu <shicheng@cs.stanford.edu>
 Project-URL: Homepage, https://github.com/stanford-oval/pyGenieScript.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyGenieScript-0.0.0b8/pyproject.toml` & `pyGenieScript-0.0.0b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "npm"]
 
 [project]
 name = "pyGenieScript"
-version = "0.0.0b8"
+version = "0.0.0b9"
 authors = [
   { name="Shicheng Liu", email="shicheng@cs.stanford.edu" },
 ]
 description = "A packaged GenieScript in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyGenieScript-0.0.0b8/setup.py` & `pyGenieScript-0.0.0b9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,14 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install as _install
 from setuptools.command.sdist import sdist as _sdist
      
 setup(
     name='pyGenieScript',
     author="Stanford University Open Virtual Assistant Lab",
-    version='0.0.0-b8',
+    version='0.0.0-b9',
     packages=find_packages(),
     package_data={'pyGenieScript': ['package.json']},
     include_package_data=True,
     install_requires=[
     ],
 )
```

