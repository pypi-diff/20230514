# Comparing `tmp/jutility-0.0.1.tar.gz` & `tmp/jutility-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jake\Documents\Programming\jutility\dist\.tmp-qvp1b_s2\jutility-0.0.1.tar", last modified: Sat May 13 21:10:53 2023, max compression
+gzip compressed data, was "C:\Users\Jake\Documents\Programming\jutility\dist\.tmp-x6wipxzi\jutility-0.0.2.tar", last modified: Sat May 13 21:32:23 2023, max compression
```

## Comparing `jutility-0.0.1.tar` & `jutility-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 21:10:53.000000 jutility-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-05-13 21:09:33.000000 jutility-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      705 2023-05-13 21:10:53.000000 jutility-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      110 2023-05-13 21:08:21.000000 jutility-0.0.1/README.md
--rw-rw-rw-   0        0        0      673 2023-05-13 21:03:26.000000 jutility-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 21:10:53.000000 jutility-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-13 21:10:53.000000 jutility-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-13 21:10:53.000000 jutility-0.0.1/src/jutility/
--rw-rw-rw-   0        0        0        0 2023-05-13 20:59:58.000000 jutility-0.0.1/src/jutility/__init__.py
--rw-rw-rw-   0        0        0    16201 2023-05-13 21:09:33.000000 jutility-0.0.1/src/jutility/plotting.py
--rw-rw-rw-   0        0        0    10041 2023-05-09 15:30:12.000000 jutility-0.0.1/src/jutility/sweep.py
--rw-rw-rw-   0        0        0    13218 2023-05-11 19:23:07.000000 jutility-0.0.1/src/jutility/util.py
-drwxrwxrwx   0        0        0        0 2023-05-13 21:10:53.000000 jutility-0.0.1/src/jutility.egg-info/
--rw-rw-rw-   0        0        0      705 2023-05-13 21:10:53.000000 jutility-0.0.1/src/jutility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-13 21:10:53.000000 jutility-0.0.1/src/jutility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 21:10:53.000000 jutility-0.0.1/src/jutility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-13 21:10:53.000000 jutility-0.0.1/src/jutility.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-13 21:32:23.000000 jutility-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-05-13 21:09:33.000000 jutility-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1384 2023-05-13 21:32:23.000000 jutility-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      771 2023-05-13 21:23:26.000000 jutility-0.0.2/README.md
+-rw-rw-rw-   0        0        0      673 2023-05-13 21:32:08.000000 jutility-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-13 21:32:23.000000 jutility-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-13 21:32:23.000000 jutility-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-13 21:32:23.000000 jutility-0.0.2/src/jutility/
+-rw-rw-rw-   0        0        0        0 2023-05-13 20:59:58.000000 jutility-0.0.2/src/jutility/__init__.py
+-rw-rw-rw-   0        0        0    16215 2023-05-13 21:31:01.000000 jutility-0.0.2/src/jutility/plotting.py
+-rw-rw-rw-   0        0        0    10048 2023-05-13 21:30:51.000000 jutility-0.0.2/src/jutility/sweep.py
+-rw-rw-rw-   0        0        0    13218 2023-05-11 19:23:07.000000 jutility-0.0.2/src/jutility/util.py
+drwxrwxrwx   0        0        0        0 2023-05-13 21:32:23.000000 jutility-0.0.2/src/jutility.egg-info/
+-rw-rw-rw-   0        0        0     1384 2023-05-13 21:32:23.000000 jutility-0.0.2/src/jutility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-13 21:32:23.000000 jutility-0.0.2/src/jutility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-13 21:32:23.000000 jutility-0.0.2/src/jutility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-13 21:32:23.000000 jutility-0.0.2/src/jutility.egg-info/top_level.txt
```

### Comparing `jutility-0.0.1/LICENSE` & `jutility-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jutility-0.0.1/pyproject.toml` & `jutility-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "jutility"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jake Levi", email="jakelevi@hotmail.co.uk" },
 ]
 description = "Collection of Python utilities intended to be useful for machine learning research and experiments"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jutility-0.0.1/src/jutility/plotting.py` & `jutility-0.0.2/src/jutility/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import textwrap
 import math
 import matplotlib.pyplot as plt
 import matplotlib.lines
 import matplotlib.patches
 import numpy as np
 import PIL
-import util
+from jutility import util
 
 class Line:
     def __init__(self, x=None, y=None, **kwargs):
         if y is None:
             if x is None:
                 raise ValueError("Must specify x and/or y")
             y = x
```

### Comparing `jutility-0.0.1/src/jutility/sweep.py` & `jutility-0.0.2/src/jutility/sweep.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import numpy as np
-import util
-import plotting
+from jutility import util, plotting
 
 def get_range(val_lo, val_hi, val_num=10, log_space=False):
     if log_space:
         log_lo, log_hi = np.log([val_lo, val_hi])
         val_range = np.exp(np.linspace(log_lo, log_hi, val_num))
     else:
         val_range = np.linspace(val_lo, val_hi, val_num)
```

### Comparing `jutility-0.0.1/src/jutility/util.py` & `jutility-0.0.2/src/jutility/util.py`

 * *Files identical despite different names*

