# Comparing `tmp/checkify-0.5.tar.gz` & `tmp/checkify-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkify-0.5.tar", last modified: Sat May 13 14:43:23 2023, max compression
+gzip compressed data, was "checkify-0.6.tar", last modified: Sun May 14 06:24:53 2023, max compression
```

## Comparing `checkify-0.5.tar` & `checkify-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 14:43:23.709805 checkify-0.5/
--rw-rw-rw-   0        0        0     1101 2023-05-13 13:47:43.000000 checkify-0.5/LICENSE
--rw-rw-rw-   0        0        0     1143 2023-05-13 14:43:23.707800 checkify-0.5/PKG-INFO
--rw-rw-rw-   0        0        0      587 2023-05-13 14:30:49.000000 checkify-0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 14:43:23.671795 checkify-0.5/checkify/
--rw-rw-rw-   0        0        0        0 2023-05-13 13:57:56.000000 checkify-0.5/checkify/__init__.py
--rw-rw-rw-   0        0        0      792 2023-05-13 14:43:08.000000 checkify-0.5/checkify/code_checker.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:43:23.704794 checkify-0.5/checkify.egg-info/
--rw-rw-rw-   0        0        0     1143 2023-05-13 14:43:23.000000 checkify-0.5/checkify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-13 14:43:23.000000 checkify-0.5/checkify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 14:43:23.000000 checkify-0.5/checkify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-13 14:43:23.000000 checkify-0.5/checkify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-13 14:43:23.000000 checkify-0.5/checkify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 14:43:23.709805 checkify-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-05-13 14:43:16.000000 checkify-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:24:52.789443 checkify-0.6/
+-rw-rw-rw-   0        0        0     1101 2023-05-13 13:47:43.000000 checkify-0.6/LICENSE
+-rw-rw-rw-   0        0        0     2559 2023-05-14 06:24:52.709449 checkify-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1871 2023-05-14 06:23:23.000000 checkify-0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 06:24:52.171447 checkify-0.6/checkify/
+-rw-rw-rw-   0        0        0        0 2023-05-13 13:57:56.000000 checkify-0.6/checkify/__init__.py
+-rw-rw-rw-   0        0        0     1055 2023-05-14 06:20:26.000000 checkify-0.6/checkify/code_checker.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:24:52.699450 checkify-0.6/checkify.egg-info/
+-rw-rw-rw-   0        0        0     2559 2023-05-14 06:24:50.000000 checkify-0.6/checkify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-14 06:24:51.000000 checkify-0.6/checkify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 06:24:50.000000 checkify-0.6/checkify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-14 06:24:50.000000 checkify-0.6/checkify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 06:24:50.000000 checkify-0.6/checkify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 06:24:52.790445 checkify-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1183 2023-05-14 06:24:12.000000 checkify-0.6/setup.py
```

### Comparing `checkify-0.5/LICENSE` & `checkify-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `checkify-0.5/checkify/code_checker.py` & `checkify-0.6/checkify/code_checker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-import os
 import openai
-from dotenv import load_dotenv
 
-# Load the environment variables from the .env file
-load_dotenv()
+def check_code(code):
+    # Ask the user for their OpenAI API key
+    api_key = input("Please enter your OpenAI API key: ")
 
-# Get the API key from the environment variable
-api_key = os.getenv('OPENAI_API_KEY')
+    try:
+        # Set up the GPT API credentials
+        openai.api_key = api_key
 
-def check_code(code):
-    # Set up the GPT API credentials
-    openai.api_key = api_key
+        # Call the GPT API to check the code and get the response
+        response = openai.Completion.create(
+            engine='davinci',
+            prompt=code,
+            max_tokens=100,
+            n=1,
+            stop=None,
+            temperature=0.8,
+            top_p=1,
+            frequency_penalty=0,
+            presence_penalty=0,
+            log_level='info'
+        )
+
+        # Extract and return the generated explanation
+        explanation = response.choices[0].text.strip()
+        return explanation
+
+    except openai.error.AuthenticationError:
+        print("Invalid API key. Authentication failed.")
+        return None
 
-    # Call the GPT API to check the code and get the response
-    response = openai.Completion.create(
-        engine='davinci',
-        prompt=code,
-        max_tokens=100,
-        n=1,
-        stop=None,
-        temperature=0.8,
-        top_p=1,
-        frequency_penalty=0,
-        presence_penalty=0,
-        log_level='info'
-    )
-
-    # Extract and return the generated explanation
-    explanation = response.choices[0].text.strip()
-    return explanation
+    except openai.error.OpenAIError as e:
+        print("An error occurred while communicating with the OpenAI API:", str(e))
+        return None
```

### Comparing `checkify-0.5/setup.py` & `checkify-0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='checkify',
-    version='0.5',
+    version='0.6',
     packages=['checkify'],
     install_requires=[
         'openai'
     ],
     author="Tripathi Aditya Prakash",                     # Full name of the author
-    description="Python package that utilizes the GPT API to check for errors in code and explain the code.",
+    description="Python package that utilizes the power of the GPT API to provide comprehensive code analysis and assistance. It helps you identify errors in code, explains the code logic, and offers valuable suggestions for improvement.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/aditya0072001/checkify',
         classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

