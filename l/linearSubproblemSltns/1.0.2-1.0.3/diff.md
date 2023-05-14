# Comparing `tmp/linearsubproblemsltns-1.0.2.tar.gz` & `tmp/linearsubproblemsltns-1.0.3.tar.gz`

## Comparing `linearsubproblemsltns-1.0.2.tar` & `linearsubproblemsltns-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/__init__.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/rand_py.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp1_lib.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp2E_lib.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp2_lib.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp3_lib.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp4_lib.py
--rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp5_lib.py
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp6_lib.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/LICENSE
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/README.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/__init__.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/rand_py.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp1_lib.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp2E_lib.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp2_lib.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp3_lib.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp4_lib.py
+-rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp5_lib.py
+-rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp6_lib.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/README.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.3/PKG-INFO
```

### Comparing `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/rand_py.py` & `linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/rand_py.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp1_lib.py` & `linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp1_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp2E_lib.py` & `linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp2E_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp2_lib.py` & `linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp2_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp3_lib.py` & `linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp3_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp4_lib.py` & `linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp4_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp5_lib.py` & `linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp5_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp6_lib.py` & `linearsubproblemsltns-1.0.3/src/linearSubproblemSltns/sp6_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.2/LICENSE` & `linearsubproblemsltns-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.2/README.md` & `linearsubproblemsltns-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Summary:
 - This is a research project led by Alexander Elias and Dr. John Wen at RPI.
 - Summation of research: https://arxiv.org/pdf/2211.05737.pdf
 - Included here is the Python version of the MATLAB-based canonical subproblems for inverse kinematics on robots.
 - Additional MATLAB, C++, Rust, and Python files are located at https://github.com/rpiRobotics/linear-subproblem-solutions/.
+- See the project on PyPi: https://pypi.org/project/linearsubproblemsltns/
 ---
 # Python Branch Guide:
 ## Dependencies:
 - NumPy: https://numpy.org/install/
 - SciPy: https://scipy.org/install/
 - Python (version compatible w/ installed NumPy)
 ---
 ## To Use Example Code:
 - Clone the above repo
 - To see timing information and a simple demo, run each sp#.py file
-- Otherwise, just include yhe pip module in your applications as needed
+- Otherwise, just include the pip module in your applications as needed using pip install linearSubproblemSltns
 ---
 ## Advice:
 - NumPy vs MATLAB can be confusing at first, see [this article](https://numpy.org/doc/stable/user/numpy-for-matlab-users.html) for some clarity.
 - See the below note on precision/formatting.
 - NumPy makes it extremely easy to export/import entire matrices as csv/excel files.  Make use of this if you can.
 ---
 ## Precision and Formatting
@@ -42,8 +43,8 @@
 | ------------- | ---------------  | ------------------   |
 | Sp1           | 78716.896 ns     | 73754.058 ns         |
 | Sp2           | 325238.43 ns     | 318135.293 ns        |
 | Sp2E          | 409206.773 ns    | 400298.479 ns        |
 | Sp3           | 127781.537 ns    | 122444.399 ns        |
 | Sp4           | 104747.862 ns    | 99615.851 ns         |
 | Sp5           | 1353110.805 ns   | 1341531.159 ns       |
-| Sp6           | 614233.523 ns    | 596708.225 ns        |
+| Sp6           | 614233.523 ns    | 596708.225 ns        |
```

### Comparing `linearsubproblemsltns-1.0.2/pyproject.toml` & `linearsubproblemsltns-1.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling", "scipy", "numpy"]
 build-backend = "hatchling.build"
 [project]
 name = "linearSubproblemSltns"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name ="Alexander Elias", email ="eliasa3@rpi.edu" }, { name="Ashton Ropp", email="ashr8011@gmail.com" },
 ]
 description = "This is a new tool for multi-joint robotic arm calculations developed at RPI."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `linearsubproblemsltns-1.0.2/PKG-INFO` & `linearsubproblemsltns-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linearSubproblemSltns
-Version: 1.0.2
+Version: 1.0.3
 Summary: This is a new tool for multi-joint robotic arm calculations developed at RPI.
 Project-URL: Homepage, https://github.com/rpiRobotics/linear-subproblem-solutions
 Project-URL: Bug Tracker, https://github.com/rpiRobotics/linear-subproblem-solutions/issues
 Project-URL: Paper, https://arxiv.org/pdf/2211.05737.pdf
 Author-email: Alexander Elias <eliasa3@rpi.edu>, Ashton Ropp <ashr8011@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
@@ -16,25 +16,26 @@
 Description-Content-Type: text/markdown
 
 # Summary:
 - This is a research project led by Alexander Elias and Dr. John Wen at RPI.
 - Summation of research: https://arxiv.org/pdf/2211.05737.pdf
 - Included here is the Python version of the MATLAB-based canonical subproblems for inverse kinematics on robots.
 - Additional MATLAB, C++, Rust, and Python files are located at https://github.com/rpiRobotics/linear-subproblem-solutions/.
+- See the project on PyPi: https://pypi.org/project/linearsubproblemsltns/
 ---
 # Python Branch Guide:
 ## Dependencies:
 - NumPy: https://numpy.org/install/
 - SciPy: https://scipy.org/install/
 - Python (version compatible w/ installed NumPy)
 ---
 ## To Use Example Code:
 - Clone the above repo
 - To see timing information and a simple demo, run each sp#.py file
-- Otherwise, just include yhe pip module in your applications as needed
+- Otherwise, just include the pip module in your applications as needed using pip install linearSubproblemSltns
 ---
 ## Advice:
 - NumPy vs MATLAB can be confusing at first, see [this article](https://numpy.org/doc/stable/user/numpy-for-matlab-users.html) for some clarity.
 - See the below note on precision/formatting.
 - NumPy makes it extremely easy to export/import entire matrices as csv/excel files.  Make use of this if you can.
 ---
 ## Precision and Formatting
@@ -59,8 +60,8 @@
 | ------------- | ---------------  | ------------------   |
 | Sp1           | 78716.896 ns     | 73754.058 ns         |
 | Sp2           | 325238.43 ns     | 318135.293 ns        |
 | Sp2E          | 409206.773 ns    | 400298.479 ns        |
 | Sp3           | 127781.537 ns    | 122444.399 ns        |
 | Sp4           | 104747.862 ns    | 99615.851 ns         |
 | Sp5           | 1353110.805 ns   | 1341531.159 ns       |
-| Sp6           | 614233.523 ns    | 596708.225 ns        |
+| Sp6           | 614233.523 ns    | 596708.225 ns        |
```

