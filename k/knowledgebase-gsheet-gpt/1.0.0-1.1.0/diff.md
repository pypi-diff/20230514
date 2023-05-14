# Comparing `tmp/knowledgebase-gsheet-gpt-1.0.0.tar.gz` & `tmp/knowledgebase-gsheet-gpt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledgebase-gsheet-gpt-1.0.0.tar", last modified: Sat May 13 03:07:02 2023, max compression
+gzip compressed data, was "knowledgebase-gsheet-gpt-1.1.0.tar", last modified: Sun May 14 09:23:12 2023, max compression
```

## Comparing `knowledgebase-gsheet-gpt-1.0.0.tar` & `knowledgebase-gsheet-gpt-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-13 03:07:02.703986 knowledgebase-gsheet-gpt-1.0.0/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1656 2023-05-13 03:07:02.703874 knowledgebase-gsheet-gpt-1.0.0/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1474 2023-05-13 03:07:02.000000 knowledgebase-gsheet-gpt-1.0.0/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-13 03:07:02.703687 knowledgebase-gsheet-gpt-1.0.0/knowledgebase_gsheet_gpt.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1656 2023-05-13 03:07:02.000000 knowledgebase-gsheet-gpt-1.0.0/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-13 03:07:02.000000 knowledgebase-gsheet-gpt-1.0.0/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-13 03:07:02.000000 knowledgebase-gsheet-gpt-1.0.0/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-13 03:07:02.000000 knowledgebase-gsheet-gpt-1.0.0/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       98 2023-05-13 03:07:02.000000 knowledgebase-gsheet-gpt-1.0.0/knowledgebase_gsheet_gpt.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-13 03:07:02.000000 knowledgebase-gsheet-gpt-1.0.0/knowledgebase_gsheet_gpt.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     4364 2023-05-13 03:07:02.000000 knowledgebase-gsheet-gpt-1.0.0/knowledgebase_gsheet_gpt.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-13 03:07:02.704023 knowledgebase-gsheet-gpt-1.0.0/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-13 03:07:02.000000 knowledgebase-gsheet-gpt-1.0.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 09:23:12.041819 knowledgebase-gsheet-gpt-1.1.0/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-14 09:23:12.041684 knowledgebase-gsheet-gpt-1.1.0/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1476 2023-05-14 09:23:11.000000 knowledgebase-gsheet-gpt-1.1.0/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 09:23:12.041429 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-14 09:23:12.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-14 09:23:12.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-14 09:23:12.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-14 09:23:12.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)      108 2023-05-14 09:23:12.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-14 09:23:12.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     4722 2023-05-14 09:23:11.000000 knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-14 09:23:12.041858 knowledgebase-gsheet-gpt-1.1.0/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-14 09:23:11.000000 knowledgebase-gsheet-gpt-1.1.0/setup.py
```

### Comparing `knowledgebase-gsheet-gpt-1.0.0/PKG-INFO` & `knowledgebase-gsheet-gpt-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.0.0
+Version: 1.1.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
@@ -24,17 +24,17 @@
 ```
 
 ## 使用方法
 1. 首先，確保您已擁有 Google API 憑證 (JSON 檔案)。若尚未擁有，請參考 [Google API 官方文件](https://developers.google.com/identity/protocols/oauth2/service-account#creatinganaccount) 以建立一個。
 2. 運行以下命令行，將 `user` 替換為您的電子郵件地址，將 `key_file` 替換為您 Google API 憑證的路徑，將 `sheet_ids` 替換為您要下載的 Google 試算表 ID（以逗號分隔），並將 `prompt` 替換為您的問題：
 
 ```
-python3 -m knowledgebase_gsheet_gpt --user 用戶電子郵件 --key-file Google服務帳戶密鑰JSON文件路徑 --sheet-ids 試算表ID --prompt 提示問題
+python3 -m knowledgebase_gsheet_gpt --user 用戶電子郵件 --prompt 提示問題 --sheet-ids 試算表ID --key-file Google服務帳戶密鑰JSON文件路徑 
 ```
 
 例如：
 ```
-python3 -m knowledgebase_gsheet_gpt --user example@example.com --key-file google_key_file.json --sheet-ids 1abcdefg,2hijklmn --prompt "請問屁股癢癢的怎麼辦?"
+python3 -m knowledgebase_gsheet_gpt --user example@example.com --prompt "請問屁股癢癢的怎麼辦?" --sheet-ids 1abcdefg,2hijklmn --key-file google_key_file.json 
 ```
 
 3. 您將會看到 GPT 模型生成的串流回答。
```

### Comparing `knowledgebase-gsheet-gpt-1.0.0/README.md` & `knowledgebase-gsheet-gpt-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 ```
 
 ## 使用方法
 1. 首先，確保您已擁有 Google API 憑證 (JSON 檔案)。若尚未擁有，請參考 [Google API 官方文件](https://developers.google.com/identity/protocols/oauth2/service-account#creatinganaccount) 以建立一個。
 2. 運行以下命令行，將 `user` 替換為您的電子郵件地址，將 `key_file` 替換為您 Google API 憑證的路徑，將 `sheet_ids` 替換為您要下載的 Google 試算表 ID（以逗號分隔），並將 `prompt` 替換為您的問題：
 
 ```
-python3 -m knowledgebase_gsheet_gpt --user 用戶電子郵件 --key-file Google服務帳戶密鑰JSON文件路徑 --sheet-ids 試算表ID --prompt 提示問題
+python3 -m knowledgebase_gsheet_gpt --user 用戶電子郵件 --prompt 提示問題 --sheet-ids 試算表ID --key-file Google服務帳戶密鑰JSON文件路徑 
 ```
 
 例如：
 ```
-python3 -m knowledgebase_gsheet_gpt --user example@example.com --key-file google_key_file.json --sheet-ids 1abcdefg,2hijklmn --prompt "請問屁股癢癢的怎麼辦?"
+python3 -m knowledgebase_gsheet_gpt --user example@example.com --prompt "請問屁股癢癢的怎麼辦?" --sheet-ids 1abcdefg,2hijklmn --key-file google_key_file.json 
 ```
 
 3. 您將會看到 GPT 模型生成的串流回答。
```

### Comparing `knowledgebase-gsheet-gpt-1.0.0/knowledgebase_gsheet_gpt.egg-info/PKG-INFO` & `knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.0.0
+Version: 1.1.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
@@ -24,17 +24,17 @@
 ```
 
 ## 使用方法
 1. 首先，確保您已擁有 Google API 憑證 (JSON 檔案)。若尚未擁有，請參考 [Google API 官方文件](https://developers.google.com/identity/protocols/oauth2/service-account#creatinganaccount) 以建立一個。
 2. 運行以下命令行，將 `user` 替換為您的電子郵件地址，將 `key_file` 替換為您 Google API 憑證的路徑，將 `sheet_ids` 替換為您要下載的 Google 試算表 ID（以逗號分隔），並將 `prompt` 替換為您的問題：
 
 ```
-python3 -m knowledgebase_gsheet_gpt --user 用戶電子郵件 --key-file Google服務帳戶密鑰JSON文件路徑 --sheet-ids 試算表ID --prompt 提示問題
+python3 -m knowledgebase_gsheet_gpt --user 用戶電子郵件 --prompt 提示問題 --sheet-ids 試算表ID --key-file Google服務帳戶密鑰JSON文件路徑 
 ```
 
 例如：
 ```
-python3 -m knowledgebase_gsheet_gpt --user example@example.com --key-file google_key_file.json --sheet-ids 1abcdefg,2hijklmn --prompt "請問屁股癢癢的怎麼辦?"
+python3 -m knowledgebase_gsheet_gpt --user example@example.com --prompt "請問屁股癢癢的怎麼辦?" --sheet-ids 1abcdefg,2hijklmn --key-file google_key_file.json 
 ```
 
 3. 您將會看到 GPT 模型生成的串流回答。
```

### Comparing `knowledgebase-gsheet-gpt-1.0.0/knowledgebase_gsheet_gpt.py` & `knowledgebase-gsheet-gpt-1.1.0/knowledgebase_gsheet_gpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,38 +4,47 @@
 import os
 
 import csv_embeddings_creator
 import google_sheet_downloader
 import openai_chat_thread
 import similarity_ranker
 
+DEFAULT_BEFORE_QUESTION_PROMPT = '\n-- the user question\n'
 DEFAULT_BEFORE_KNOWLEDGE_PROMPT = '\n-- reference following knowledge base content to answer the user question (answer as long as possible)\n'
+DEFAULT_MODEL = "gpt-4"
+DEFAULT_TOP_N = 3
+DEFAULT_KEY_FILE = "./keys/google_service_account_key.json"
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description='Knowledgebase GSheet GPT')
     parser.add_argument('--user', type=str, required=True, help='User email')
-    parser.add_argument('--key-file', type=str, required=True, help='Google service account key JSON file path')
-    parser.add_argument('--sheet-ids', type=str, required=True, help='Comma separated Google sheet IDs to download')
     parser.add_argument('--prompt', type=str, required=True, help='Prompt sentence for finding similar embeddings.')
-    parser.add_argument('--before-question-prompt', type=str, default='\n-- the user question\n',
+    parser.add_argument('--sheet-ids', type=str, default="", help='Comma separated Google sheet IDs to download')
+    parser.add_argument('--before-question-prompt', type=str, default=DEFAULT_BEFORE_QUESTION_PROMPT,
                         help='Text before the user question in the final prompt')
     parser.add_argument('--before-knowledge-prompt', type=str,
                         default=DEFAULT_BEFORE_KNOWLEDGE_PROMPT,
                         help='Text before the knowledge base content in the final prompt')
-    parser.add_argument('--top-n', type=int, default=3,
+    parser.add_argument('--top-n', type=int, default=DEFAULT_TOP_N,
                         help='Number of top similar knowledge base texts to include in the final prompt')
-    parser.add_argument('--model', type=str, default='gpt-3.5-turbo',
+    parser.add_argument('--model', type=str, default=DEFAULT_MODEL,
                         help='gpt-3.5-turbo or gpt-4')
+    parser.add_argument('--key-file', type=str, default=DEFAULT_KEY_FILE,
+                        help='Google service account key JSON file path')
     return parser.parse_args()
 
 
-def knowledgebase_gsheet_gpt(user, key_file, sheet_ids, prompt, before_question_prompt='\n-- the user question\n',
+def knowledgebase_gsheet_gpt(user, prompt,
+                             sheet_ids="",
+                             before_question_prompt=DEFAULT_BEFORE_QUESTION_PROMPT,
                              before_knowledge_prompt=DEFAULT_BEFORE_KNOWLEDGE_PROMPT,
-                             top_n=3, model='gpt-3.5-turbo'):
+                             top_n=DEFAULT_TOP_N,
+                             model=DEFAULT_MODEL,
+                             key_file=DEFAULT_KEY_FILE):
     os.environ["TOKENIZERS_PARALLELISM"] = "true"
 
     user = user.lower().replace('@', '_').replace('.', '_')
     data_folder = f'./data/users/{user}'
 
     # Google Sheet Downloader
     google_sheet_downloader.download_google_sheets(
@@ -82,21 +91,21 @@
     response_queue = openai_chat_thread.openai_chat_thread_taiwan(prompt=knowledge_prompt, model=model)
     return response_queue
 
 
 def main():
     arg = parse_arguments()
     response_stream = knowledgebase_gsheet_gpt(arg.user,
-                                               arg.key_file,
-                                               arg.sheet_ids,
                                                arg.prompt,
+                                               arg.sheet_ids,
                                                arg.before_question_prompt,
                                                arg.before_knowledge_prompt,
                                                arg.top_n,
-                                               arg.model
+                                               arg.model,
+                                               arg.key_file
                                                )
     while True:
         response = response_stream.get()
         if response is None:
             break
         print(response, end="", flush=True)
```

### Comparing `knowledgebase-gsheet-gpt-1.0.0/setup.py` & `knowledgebase-gsheet-gpt-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="knowledgebase-gsheet-gpt",
-    version="1.0.0",
+    version="1.1.0",
     packages=find_packages(),
     py_modules=['knowledgebase_gsheet_gpt'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'knowledgebase_gsheet_gpt = knowledgebase_gsheet_gpt:main',
         ],
```

