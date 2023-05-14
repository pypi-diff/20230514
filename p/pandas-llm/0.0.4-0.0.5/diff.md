# Comparing `tmp/pandas_llm-0.0.4.tar.gz` & `tmp/pandas_llm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_llm-0.0.4.tar", last modified: Sat May 13 14:56:54 2023, max compression
+gzip compressed data, was "pandas_llm-0.0.5.tar", last modified: Sun May 14 18:10:17 2023, max compression
```

## Comparing `pandas_llm-0.0.4.tar` & `pandas_llm-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-05-13 14:56:54.140380 pandas_llm-0.0.4/
--rw-r--r--   0 alessioricco   (501) staff       (20)     1068 2023-05-11 12:07:22.000000 pandas_llm-0.0.4/LICENSE
--rw-r--r--   0 alessioricco   (501) staff       (20)     2542 2023-05-13 14:56:54.140472 pandas_llm-0.0.4/PKG-INFO
--rw-r--r--   0 alessioricco   (501) staff       (20)     1725 2023-05-13 14:31:01.000000 pandas_llm-0.0.4/README.md
-drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-05-13 14:56:54.139183 pandas_llm-0.0.4/pandas_llm/
--rw-r--r--   0 alessioricco   (501) staff       (20)       32 2023-05-11 15:03:14.000000 pandas_llm-0.0.4/pandas_llm/__init__.py
--rw-r--r--   0 alessioricco   (501) staff       (20)     2600 2023-05-13 14:31:01.000000 pandas_llm-0.0.4/pandas_llm/example-chatbot.py
--rw-r--r--   0 alessioricco   (501) staff       (20)      888 2023-05-13 14:31:01.000000 pandas_llm-0.0.4/pandas_llm/example.py
--rw-r--r--   0 alessioricco   (501) staff       (20)    11178 2023-05-13 14:31:01.000000 pandas_llm-0.0.4/pandas_llm/pandas_llm.py
--rw-r--r--   0 alessioricco   (501) staff       (20)     1967 2023-05-11 12:28:50.000000 pandas_llm-0.0.4/pandas_llm/sandbox.py
-drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-05-13 14:56:54.140238 pandas_llm-0.0.4/pandas_llm.egg-info/
--rw-r--r--   0 alessioricco   (501) staff       (20)     2542 2023-05-13 14:56:54.000000 pandas_llm-0.0.4/pandas_llm.egg-info/PKG-INFO
--rw-r--r--   0 alessioricco   (501) staff       (20)      327 2023-05-13 14:56:54.000000 pandas_llm-0.0.4/pandas_llm.egg-info/SOURCES.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)        1 2023-05-13 14:56:54.000000 pandas_llm-0.0.4/pandas_llm.egg-info/dependency_links.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)      187 2023-05-13 14:56:54.000000 pandas_llm-0.0.4/pandas_llm.egg-info/requires.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)       11 2023-05-13 14:56:54.000000 pandas_llm-0.0.4/pandas_llm.egg-info/top_level.txt
--rw-r--r--   0 alessioricco   (501) staff       (20)       79 2023-05-13 14:56:54.140800 pandas_llm-0.0.4/setup.cfg
--rw-r--r--   0 alessioricco   (501) staff       (20)     2035 2023-05-13 14:31:01.000000 pandas_llm-0.0.4/setup.py
+drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-05-14 18:10:17.194713 pandas_llm-0.0.5/
+-rw-r--r--   0 alessioricco   (501) staff       (20)     1068 2023-05-11 12:07:22.000000 pandas_llm-0.0.5/LICENSE
+-rw-r--r--   0 alessioricco   (501) staff       (20)     2657 2023-05-14 18:10:17.194800 pandas_llm-0.0.5/PKG-INFO
+-rw-r--r--   0 alessioricco   (501) staff       (20)     1840 2023-05-14 18:08:55.000000 pandas_llm-0.0.5/README.md
+drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-05-14 18:10:17.193613 pandas_llm-0.0.5/pandas_llm/
+-rw-r--r--   0 alessioricco   (501) staff       (20)    13119 2023-05-14 18:01:48.000000 pandas_llm-0.0.5/pandas_llm/__init__.py
+-rw-r--r--   0 alessioricco   (501) staff       (20)     2599 2023-05-14 18:07:43.000000 pandas_llm-0.0.5/pandas_llm/example-chatbot.py
+-rw-r--r--   0 alessioricco   (501) staff       (20)     1000 2023-05-14 18:06:35.000000 pandas_llm-0.0.5/pandas_llm/example.py
+drwxr-xr-x   0 alessioricco   (501) staff       (20)        0 2023-05-14 18:10:17.194573 pandas_llm-0.0.5/pandas_llm.egg-info/
+-rw-r--r--   0 alessioricco   (501) staff       (20)     2657 2023-05-14 18:10:17.000000 pandas_llm-0.0.5/pandas_llm.egg-info/PKG-INFO
+-rw-r--r--   0 alessioricco   (501) staff       (20)      280 2023-05-14 18:10:17.000000 pandas_llm-0.0.5/pandas_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)        1 2023-05-14 18:10:17.000000 pandas_llm-0.0.5/pandas_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)      187 2023-05-14 18:10:17.000000 pandas_llm-0.0.5/pandas_llm.egg-info/requires.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)       11 2023-05-14 18:10:17.000000 pandas_llm-0.0.5/pandas_llm.egg-info/top_level.txt
+-rw-r--r--   0 alessioricco   (501) staff       (20)       79 2023-05-14 18:10:17.195256 pandas_llm-0.0.5/setup.cfg
+-rw-r--r--   0 alessioricco   (501) staff       (20)     2035 2023-05-14 18:09:53.000000 pandas_llm-0.0.5/setup.py
```

### Comparing `pandas_llm-0.0.4/LICENSE` & `pandas_llm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_llm-0.0.4/PKG-INFO` & `pandas_llm-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pandas_llm
-Version: 0.0.4
+Version: 0.0.5
 Summary: Conversational Pandas Dataframes
 Home-page: https://github.com/DashyDashOrg/pandas-llm
-Download-URL: https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.4
+Download-URL: https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.5
 Author: DashyDash
 Author-email: alessio@dashydash.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/DashyDashOrg/pandas-llm/issues
 Keywords: pypi,pandas-llm,pandas,llm,ai,openai,chatgpt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -38,14 +38,18 @@
 
 ## Usage
 Here's a quick example of how to use pandas-llm:
 
 ```python
 import os
 import pandas as pd
+
+# import sys
+# from pathlib import Path
+# sys.path.append(str(Path(__file__).resolve().parent.parent))
 from pandas_llm import PandasLLM
 
 # Data
 # Please note that these names, ages, and donations are randomly generated 
 # and do not correspond to real individuals or their donations.
 data = [('John Doe', 25, 50), 
         ('Jane Smith', 38, 70),
@@ -55,15 +59,15 @@
         ('Emily Wilson', 30, 60),
         ('Daniel Taylor', 35, 75),
         ('Sophia Moore', 40, 85),
         ('David Thomas', 50, 65),
         ('Olivia Jackson', 29, 55)]
 df = pd.DataFrame(data, columns=['name', 'age', 'donation'])
 
-conv_df = PandasLLM(data=df, openai_api_key = os.environ.get("OPENAI_API_KEY"))
+conv_df = PandasLLM(data=df, llm_api_key = os.environ.get("OPENAI_API_KEY"), verbose=True)
 result = conv_df.prompt("What is the average donation of people older than 30 who donated more than $50?")
 
 print(f"Result ({type(result)}):\n {result}")
 # Result (<class 'numpy.float64'>):
 #  75.0
 ```
```

### Comparing `pandas_llm-0.0.4/README.md` & `pandas_llm-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 ## Usage
 Here's a quick example of how to use pandas-llm:
 
 ```python
 import os
 import pandas as pd
+
+# import sys
+# from pathlib import Path
+# sys.path.append(str(Path(__file__).resolve().parent.parent))
 from pandas_llm import PandasLLM
 
 # Data
 # Please note that these names, ages, and donations are randomly generated 
 # and do not correspond to real individuals or their donations.
 data = [('John Doe', 25, 50), 
         ('Jane Smith', 38, 70),
@@ -34,15 +38,15 @@
         ('Emily Wilson', 30, 60),
         ('Daniel Taylor', 35, 75),
         ('Sophia Moore', 40, 85),
         ('David Thomas', 50, 65),
         ('Olivia Jackson', 29, 55)]
 df = pd.DataFrame(data, columns=['name', 'age', 'donation'])
 
-conv_df = PandasLLM(data=df, openai_api_key = os.environ.get("OPENAI_API_KEY"))
+conv_df = PandasLLM(data=df, llm_api_key = os.environ.get("OPENAI_API_KEY"), verbose=True)
 result = conv_df.prompt("What is the average donation of people older than 30 who donated more than $50?")
 
 print(f"Result ({type(result)}):\n {result}")
 # Result (<class 'numpy.float64'>):
 #  75.0
 ```
```

### Comparing `pandas_llm-0.0.4/pandas_llm/example-chatbot.py` & `pandas_llm-0.0.5/pandas_llm/example-chatbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     print()
     banner = """
     Welcome to the Donation Data CLI.
     The donation dataset has three columns (name, age, donation)
     Please note that these names, ages, and donations are randomly generated and do not correspond to real individuals or their donations.
     
     You can ask questions like:
-    - show me the name of donors
+    - show me the list of names
     - What is the average age of people who donated?
     - What is the average donation amount?
     - What is the average donation of people older than 30?
     - What is the average donation of people older than 30 who donated more than $50?
     """
     print(banner)
```

### Comparing `pandas_llm-0.0.4/pandas_llm/example.py` & `pandas_llm-0.0.5/pandas_llm/example.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import os
 import pandas as pd
+
+import sys
+from pathlib import Path
+sys.path.append(str(Path(__file__).resolve().parent.parent))
 from pandas_llm import PandasLLM
 
 # Data
 # Please note that these names, ages, and donations are randomly generated 
 # and do not correspond to real individuals or their donations.
 data = [('John Doe', 25, 50), 
         ('Jane Smith', 38, 70),
@@ -13,13 +17,13 @@
         ('Emily Wilson', 30, 60),
         ('Daniel Taylor', 35, 75),
         ('Sophia Moore', 40, 85),
         ('David Thomas', 50, 65),
         ('Olivia Jackson', 29, 55)]
 df = pd.DataFrame(data, columns=['name', 'age', 'donation'])
 
-conv_df = PandasLLM(data=df, llm_api_key = os.environ.get("OPENAI_API_KEY"))
+conv_df = PandasLLM(data=df, llm_api_key = os.environ.get("OPENAI_API_KEY"), verbose=True)
 result = conv_df.prompt("What is the average donation of people older than 30 who donated more than $50?")
 
 print(f"Result ({type(result)}):\n {result}")
 # Result (<class 'numpy.float64'>):
 #  75.0
```

### Comparing `pandas_llm-0.0.4/pandas_llm/pandas_llm.py` & `pandas_llm-0.0.5/pandas_llm/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,69 @@
 import pandas as pd
 import datetime
 import numpy as np
 import openai
 import os
-from sandbox import Sandbox
 import re
 import json
 
+# sandbox.py
+from RestrictedPython import compile_restricted
+from RestrictedPython.Guards import safe_builtins,guarded_iter_unpack_sequence
+from  RestrictedPython.Eval import default_guarded_getattr, default_guarded_getitem, default_guarded_getiter
+import pandas as pd
+
+class Sandbox:
+    def __init__(self):
+        self._allowed_imports = {}
+
+    def allow_import(self, module_name):
+        try:
+            module = __import__(module_name)
+            self._allowed_imports[module_name] = module
+        except ImportError:
+            pass
+
+    def execute(self, code, local_vars = {}):
+        allowed_builtins = safe_builtins
+        # Add __builtins__, __import__, and allowed imports to the globals
+        restricted_globals = {"__builtins__": allowed_builtins}
+        restricted_globals.update(self._allowed_imports)
+
+        builtin_mappings = {
+            "__import__": __import__,
+            "_getattr_": default_guarded_getattr,
+            "_getitem_": default_guarded_getitem,
+            "_getiter_": default_guarded_getiter,
+            "_iter_unpack_sequence_": guarded_iter_unpack_sequence,
+            "list": list,
+            "set": set,
+            "pd": pd,
+        }
+
+        series_methods = [
+            "sum", "mean", "any", "argmax", "argmin", "count", "cumsum", "cumprod", "diff",
+            "dropna", "fillna", "head", "idxmax", "idxmin", "last", "max", "min", "notna",
+            "prod", "quantile", "rename", "round", "tail", "to_frame", "to_list", "to_numpy",
+            "to_string","unique",  "sort_index", "sort_values", "aggregate"
+        ]
+
+
+        builtin_mappings.update({method: getattr(pd.Series, method) for method in series_methods})
+
+        restricted_globals["__builtins__"].update(builtin_mappings)
+
+        byte_code = compile_restricted(source=code, filename='<inline>', mode='exec')
+
+        # Execute the restricted code
+        exec(byte_code, restricted_globals, local_vars)
+
+        return local_vars
+
+
 class PandasLLM(pd.DataFrame):
     """
     PandasLLM is a subclass of the Pandas DataFrame class. It is designed to provide a
     wrapper around the OpenAI API. 
     """
 
     code_blocks = [r'```python(.*?)```',r'```(.*?)```']
```

### Comparing `pandas_llm-0.0.4/pandas_llm.egg-info/PKG-INFO` & `pandas_llm-0.0.5/pandas_llm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pandas-llm
-Version: 0.0.4
+Version: 0.0.5
 Summary: Conversational Pandas Dataframes
 Home-page: https://github.com/DashyDashOrg/pandas-llm
-Download-URL: https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.4
+Download-URL: https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.5
 Author: DashyDash
 Author-email: alessio@dashydash.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/DashyDashOrg/pandas-llm/issues
 Keywords: pypi,pandas-llm,pandas,llm,ai,openai,chatgpt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -38,14 +38,18 @@
 
 ## Usage
 Here's a quick example of how to use pandas-llm:
 
 ```python
 import os
 import pandas as pd
+
+# import sys
+# from pathlib import Path
+# sys.path.append(str(Path(__file__).resolve().parent.parent))
 from pandas_llm import PandasLLM
 
 # Data
 # Please note that these names, ages, and donations are randomly generated 
 # and do not correspond to real individuals or their donations.
 data = [('John Doe', 25, 50), 
         ('Jane Smith', 38, 70),
@@ -55,15 +59,15 @@
         ('Emily Wilson', 30, 60),
         ('Daniel Taylor', 35, 75),
         ('Sophia Moore', 40, 85),
         ('David Thomas', 50, 65),
         ('Olivia Jackson', 29, 55)]
 df = pd.DataFrame(data, columns=['name', 'age', 'donation'])
 
-conv_df = PandasLLM(data=df, openai_api_key = os.environ.get("OPENAI_API_KEY"))
+conv_df = PandasLLM(data=df, llm_api_key = os.environ.get("OPENAI_API_KEY"), verbose=True)
 result = conv_df.prompt("What is the average donation of people older than 30 who donated more than $50?")
 
 print(f"Result ({type(result)}):\n {result}")
 # Result (<class 'numpy.float64'>):
 #  75.0
 ```
```

### Comparing `pandas_llm-0.0.4/setup.py` & `pandas_llm-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pandas_llm',                           # should match the package folder
-    version='0.0.4',                                # important for updates
+    version='0.0.5',                                # important for updates
     license='MIT',                                  # should match your chosen license
     description='Conversational Pandas Dataframes',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='DashyDash',
     author_email='alessio@dashydash.com',
     url='https://github.com/DashyDashOrg/pandas-llm', 
@@ -47,9 +47,9 @@
         "RestrictedPython",
         "six",
         "tqdm",
         "tzdata",
         "urllib3",
         "yarl",
     ],   
-    download_url="https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.4",
+    download_url="https://github.com/DashyDashOrg/pandas-llm/releases/tag/v0.0.5",
 )
```

