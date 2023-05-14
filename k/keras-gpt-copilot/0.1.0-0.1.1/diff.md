# Comparing `tmp/keras-gpt-copilot-0.1.0.tar.gz` & `tmp/keras-gpt-copilot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-gpt-copilot-0.1.0.tar", last modified: Sun May 14 20:34:22 2023, max compression
+gzip compressed data, was "keras-gpt-copilot-0.1.1.tar", last modified: Sun May 14 21:16:25 2023, max compression
```

## Comparing `keras-gpt-copilot-0.1.0.tar` & `keras-gpt-copilot-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 20:34:22.031182 keras-gpt-copilot-0.1.0/
--rw-rw-rw-   0        0        0     1068 2023-04-26 21:45:39.000000 keras-gpt-copilot-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1182 2023-05-14 20:34:22.018184 keras-gpt-copilot-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    16847 2023-05-14 19:59:57.000000 keras-gpt-copilot-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 20:34:22.014386 keras-gpt-copilot-0.1.0/keras_gpt_copilot.egg-info/
--rw-rw-rw-   0        0        0     1182 2023-05-14 20:34:21.000000 keras-gpt-copilot-0.1.0/keras_gpt_copilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-05-14 20:34:21.000000 keras-gpt-copilot-0.1.0/keras_gpt_copilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 20:34:21.000000 keras-gpt-copilot-0.1.0/keras_gpt_copilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-05-14 20:34:21.000000 keras-gpt-copilot-0.1.0/keras_gpt_copilot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 20:34:21.000000 keras-gpt-copilot-0.1.0/keras_gpt_copilot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 20:34:22.032182 keras-gpt-copilot-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1381 2023-05-14 20:33:21.000000 keras-gpt-copilot-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 21:16:25.060067 keras-gpt-copilot-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-05-14 21:16:24.931141 keras-gpt-copilot-0.1.1/KerasGPTCopilot/
+drwxrwxrwx   0        0        0        0 2023-05-14 21:16:24.992104 keras-gpt-copilot-0.1.1/KerasGPTCopilot/core/
+-rw-rw-rw-   0        0        0    13226 2023-05-14 19:14:45.000000 keras-gpt-copilot-0.1.1/KerasGPTCopilot/core/ModelAdvisor.py
+-rw-rw-rw-   0        0        0       38 2023-05-12 17:32:21.000000 keras-gpt-copilot-0.1.1/KerasGPTCopilot/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 21:16:25.002098 keras-gpt-copilot-0.1.1/KerasGPTCopilot/extras/
+-rw-rw-rw-   0        0        0        0 2023-04-20 19:05:36.000000 keras-gpt-copilot-0.1.1/KerasGPTCopilot/extras/__init__.py
+-rw-rw-rw-   0        0        0     1441 2023-05-14 19:15:26.000000 keras-gpt-copilot-0.1.1/KerasGPTCopilot/extras/util.py
+-rw-rw-rw-   0        0        0     1068 2023-04-26 21:45:39.000000 keras-gpt-copilot-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-05-14 21:10:57.000000 keras-gpt-copilot-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1182 2023-05-14 21:16:25.047078 keras-gpt-copilot-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    16847 2023-05-14 19:59:57.000000 keras-gpt-copilot-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 21:16:25.043074 keras-gpt-copilot-0.1.1/keras_gpt_copilot.egg-info/
+-rw-rw-rw-   0        0        0     1182 2023-05-14 21:16:24.000000 keras-gpt-copilot-0.1.1/keras_gpt_copilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-05-14 21:16:24.000000 keras-gpt-copilot-0.1.1/keras_gpt_copilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 21:16:24.000000 keras-gpt-copilot-0.1.1/keras_gpt_copilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-05-14 21:16:24.000000 keras-gpt-copilot-0.1.1/keras_gpt_copilot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 21:16:24.000000 keras-gpt-copilot-0.1.1/keras_gpt_copilot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 21:16:25.065065 keras-gpt-copilot-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-05-14 21:14:44.000000 keras-gpt-copilot-0.1.1/setup.py
```

### Comparing `keras-gpt-copilot-0.1.0/LICENSE` & `keras-gpt-copilot-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-gpt-copilot-0.1.0/PKG-INFO` & `keras-gpt-copilot-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-gpt-copilot
-Version: 0.1.0
+Version: 0.1.1
 Summary: Integrate an LLM copilot within your Keras model development workflow
 Home-page: https://github.com/fabprezja/keras-gpt-copilot
 Author: Fabi Prezja
 Author-email: faprezja@fairn.fi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `keras-gpt-copilot-0.1.0/README.md` & `keras-gpt-copilot-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `keras-gpt-copilot-0.1.0/keras_gpt_copilot.egg-info/PKG-INFO` & `keras-gpt-copilot-0.1.1/keras_gpt_copilot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-gpt-copilot
-Version: 0.1.0
+Version: 0.1.1
 Summary: Integrate an LLM copilot within your Keras model development workflow
 Home-page: https://github.com/fabprezja/keras-gpt-copilot
 Author: Fabi Prezja
 Author-email: faprezja@fairn.fi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `keras-gpt-copilot-0.1.0/setup.py` & `keras-gpt-copilot-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="keras-gpt-copilot",
-    version="0.1.0",
+    version="0.1.1",
     description="Integrate an LLM copilot within your Keras model development workflow",
     long_description="Keras GPT Copilot is the first Python package designed to integrate an LLM copilot within the model development workflow, offering iterative feedback options for enhancing the performance of your Keras deep learning models. Utilizing the power of OpenAI's GPT models, Keras GPT Copilot can use any of the compatible models (GPT4 is recommended). However, the prompt-only mode allows for compatibility with other large language models.",
     author="Fabi Prezja",
     author_email="faprezja@fairn.fi",
     url="https://github.com/fabprezja/keras-gpt-copilot",
     packages=find_packages(),
     install_requires=[
@@ -22,8 +22,9 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     python_requires=">=3.7",
+    include_package_data=True,  # Add this line
 )
```

