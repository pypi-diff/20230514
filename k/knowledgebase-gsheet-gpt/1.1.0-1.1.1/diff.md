# Comparing `tmp/knowledgebase-gsheet-gpt-1.1.0.tar.gz` & `tmp/knowledgebase-gsheet-gpt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledgebase-gsheet-gpt-1.1.0.tar", last modified: Sun May 14 09:23:12 2023, max compression
+gzip compressed data, was "knowledgebase-gsheet-gpt-1.1.1.tar", last modified: Sun May 14 09:34:57 2023, max compression
```

## Comparing `knowledgebase-gsheet-gpt-1.1.0.tar` & `knowledgebase-gsheet-gpt-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 09:23:12.041819 knowledgebase-gsheet-gpt-1.1.0/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-14 09:23:12.041684 knowledgebase-gsheet-gpt-1.1.0/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1476 2023-05-14 09:23:11.000000 knowledgebase-gsheet-gpt-1.1.0/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 09:23:12.041429 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-14 09:23:12.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-14 09:23:12.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-14 09:23:12.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-14 09:23:12.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)      108 2023-05-14 09:23:12.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-14 09:23:12.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     4722 2023-05-14 09:23:11.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-14 09:23:12.041858 knowledgebase-gsheet-gpt-1.1.0/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-14 09:23:11.000000 knowledgebase-gsheet-gpt-1.1.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 09:34:57.300608 knowledgebase-gsheet-gpt-1.1.1/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-14 09:34:57.300493 knowledgebase-gsheet-gpt-1.1.1/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1476 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 09:34:57.300310 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       98 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     4762 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-14 09:34:57.300642 knowledgebase-gsheet-gpt-1.1.1/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/setup.py
```

### Comparing `knowledgebase-gsheet-gpt-1.1.0/PKG-INFO` & `knowledgebase-gsheet-gpt-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.1.0
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
```

### Comparing `knowledgebase-gsheet-gpt-1.1.0/README.md` & `knowledgebase-gsheet-gpt-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/PKG-INFO` & `knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.1.0
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
```

### Comparing `knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.py` & `knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,21 @@
                              key_file=DEFAULT_KEY_FILE):
     os.environ["TOKENIZERS_PARALLELISM"] = "true"
 
     user = user.lower().replace('@', '_').replace('.', '_')
     data_folder = f'./data/users/{user}'
 
     # Google Sheet Downloader
-    google_sheet_downloader.download_google_sheets(
-        key_file,
-        sheet_ids,
-        os.path.join(data_folder, 'google_sheet_downloader'),
-        False
-    )
+    if sheet_ids:
+        google_sheet_downloader.download_google_sheets(
+            key_file,
+            sheet_ids,
+            os.path.join(data_folder, 'google_sheet_downloader'),
+            False
+        )
 
     # CSV Embeddings Creator
     csv_embeddings_creator.create_embeddings(
         os.path.join(data_folder, 'google_sheet_downloader'),
         os.path.join(data_folder, 'csv_embeddings_creator', 'txt'),
         os.path.join(data_folder, 'csv_embeddings_creator', 'embeddings'),
         False
@@ -83,15 +84,15 @@
     for i in range(top_n):
         knowledge_prompt += f"{ranked_result['ranking'][i]['content']}"
         knowledge_prompt += '\n\n'
 
     knowledge_prompt += before_question_prompt
     knowledge_prompt += f"{prompt}\n"
 
-    # print('knowledgebase_gsheet_gpt.py, knowledge_prompt:\n', knowledge_prompt)
+    print('knowledgebase_gsheet_gpt.py, knowledge_prompt:\n', knowledge_prompt)
     response_queue = openai_chat_thread.openai_chat_thread_taiwan(prompt=knowledge_prompt, model=model)
     return response_queue
 
 
 def main():
     arg = parse_arguments()
     response_stream = knowledgebase_gsheet_gpt(arg.user,
```

### Comparing `knowledgebase-gsheet-gpt-1.1.0/setup.py` & `knowledgebase-gsheet-gpt-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="knowledgebase-gsheet-gpt",
-    version="1.1.0",
+    version="1.1.1",
     packages=find_packages(),
     py_modules=['knowledgebase_gsheet_gpt'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'knowledgebase_gsheet_gpt = knowledgebase_gsheet_gpt:main',
         ],
```

