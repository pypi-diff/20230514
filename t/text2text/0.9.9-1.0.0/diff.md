# Comparing `tmp/text2text-0.9.9.tar.gz` & `tmp/text2text-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-0.9.9.tar", last modified: Sat Feb  4 23:57:45 2023, max compression
+gzip compressed data, was "text2text-1.0.0.tar", last modified: Sat May 13 23:07:45 2023, max compression
```

## Comparing `text2text-0.9.9.tar` & `text2text-1.0.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-04 23:57:45.235654 text2text-0.9.9/
--rwxr-xr-x   0 root         (0) root         (0)     1334 2023-02-04 23:05:59.000000 text2text-0.9.9/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    59271 2023-02-04 23:57:45.235654 text2text-0.9.9/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    58469 2023-02-04 23:05:59.000000 text2text-0.9.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-04 23:57:45.235654 text2text-0.9.9/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1213 2023-02-04 23:57:28.000000 text2text-0.9.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-04 23:57:45.232654 text2text-0.9.9/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      633 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-02-04 23:55:27.000000 text2text-0.9.9/text2text/answerer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-04 23:57:45.233654 text2text-0.9.9/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-02-04 23:29:29.000000 text2text-0.9.9/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-04 23:57:45.234654 text2text-0.9.9/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-02-04 23:38:10.000000 text2text-0.9.9/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/searcher.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-02-04 23:26:08.000000 text2text-0.9.9/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-02-04 23:05:59.000000 text2text-0.9.9/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-02-04 23:31:55.000000 text2text-0.9.9/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-04 23:57:45.233654 text2text-0.9.9/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    59271 2023-02-04 23:57:45.000000 text2text-0.9.9/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2023-02-04 23:57:45.000000 text2text-0.9.9/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-04 23:57:45.000000 text2text-0.9.9/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      127 2023-02-04 23:57:45.000000 text2text-0.9.9/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-02-04 23:57:45.000000 text2text-0.9.9/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 23:07:45.611461 text2text-1.0.0/
+-rwxr-xr-x   0 root         (0) root         (0)     1334 2023-05-13 22:14:45.000000 text2text-1.0.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    60334 2023-05-13 23:07:45.611461 text2text-1.0.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    59520 2023-05-13 23:04:11.000000 text2text-1.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-13 23:07:45.611461 text2text-1.0.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1225 2023-05-13 23:04:31.000000 text2text-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 23:07:45.607460 text2text-1.0.0/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-05-13 22:39:09.000000 text2text-1.0.0/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     9928 2023-05-13 22:49:09.000000 text2text-1.0.0/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 23:07:45.609460 text2text-1.0.0/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-05-13 22:47:11.000000 text2text-1.0.0/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 23:07:45.610461 text2text-1.0.0/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-05-13 22:15:54.000000 text2text-1.0.0/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/searcher.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-05-13 22:19:58.000000 text2text-1.0.0/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-13 22:14:45.000000 text2text-1.0.0/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 23:07:45.608461 text2text-1.0.0/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    60334 2023-05-13 23:07:45.000000 text2text-1.0.0/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-05-13 23:07:45.000000 text2text-1.0.0/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-13 23:07:45.000000 text2text-1.0.0/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      127 2023-05-13 23:07:45.000000 text2text-1.0.0/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-13 23:07:45.000000 text2text-1.0.0/text2text.egg-info/top_level.txt
```

### Comparing `text2text-0.9.9/LICENSE.txt` & `text2text-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/PKG-INFO` & `text2text-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 0.9.9
+Version: 1.0.0
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
-Keywords: multilingual crosslingual bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
+Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Text2Text: Crosslingual NLP/G toolkit
@@ -36,14 +36,15 @@
   * [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance)
   * [Translation](https://github.com/artitw/text2text#translation)
   * [Question Answering](https://github.com/artitw/text2text#question-answering)
   * [Question Generation](https://github.com/artitw/text2text#question-generation)
   * [Summarization](https://github.com/artitw/text2text#summarization)
   * [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation)
   * [Dialog Responder](https://github.com/artitw/text2text#dialog-responder)
+  * [Assistant](https://github.com/artitw/text2text#assistant)
   * [Finetuning](https://github.com/artitw/text2text#training--finetuning)
   * [Identification](https://github.com/artitw/text2text#identification)
   * [Web Server](https://github.com/artitw/text2text#serving)
 * [Questions?](https://github.com/artitw/text2text#questions)
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
 * [Code of Conduct](https://github.com/artitw/text2text#code-of-conduct)
@@ -65,15 +66,15 @@
   * See [Colab Demo](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR) and [Examples](#examples) below
 
 ## Class Diagram
 ```
       Indexer    Measurer   Counter -- Tfidfer
            \          \     /             \
         Searcher     Tokenizer           Bm25er
-             \_______    |
+             \_______    |      ________________ Assistant
               _______Transformer______________
              /           |                    \
         Answerer     Translator              Abstractor
            /         /    |     \              /       \
   Responder  Vectorizer  Fitter  Variator  Questioner  Summarizer
                   /
           Identifier
@@ -92,14 +93,15 @@
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
 [Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
 [Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
 [Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
 [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Explain Text2Text in one sentence"]).assist()` | `['Text to text translation uses a deep learning model to generate a text in another language from a given source text.']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
 ## Languages Available
@@ -740,14 +742,23 @@
 dialog = ' EOS '.join(dialog)
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
+### Assistant
+Not chatGPT level but it works
+```
+res = t2t.Handler(["Outline steps for contributing to open source code"]).assist()
+# 1) Find an open source project that you are interested in. You can do this by searching the internet for the project name or using a search engine to find the project page on GitHub.
+# 2) Verify that you have the necessary permissions to make changes to the code. If the project uses basic permissions, you can use git to check out the code. If the code uses more advanced permissions, you can find a way to use those permissions.
+# 3) Perform a code review to ensure that your contributions are properly credits and, if necessary, include a reasoning of your changes.
+```
+
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
 result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"], 
             src_lang="en",
             tgt_lang="zh",
             num_epochs=10,
```

### Comparing `text2text-0.9.9/README.md` & `text2text-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
   * [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance)
   * [Translation](https://github.com/artitw/text2text#translation)
   * [Question Answering](https://github.com/artitw/text2text#question-answering)
   * [Question Generation](https://github.com/artitw/text2text#question-generation)
   * [Summarization](https://github.com/artitw/text2text#summarization)
   * [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation)
   * [Dialog Responder](https://github.com/artitw/text2text#dialog-responder)
+  * [Assistant](https://github.com/artitw/text2text#assistant)
   * [Finetuning](https://github.com/artitw/text2text#training--finetuning)
   * [Identification](https://github.com/artitw/text2text#identification)
   * [Web Server](https://github.com/artitw/text2text#serving)
 * [Questions?](https://github.com/artitw/text2text#questions)
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
 * [Code of Conduct](https://github.com/artitw/text2text#code-of-conduct)
@@ -51,15 +52,15 @@
   * See [Colab Demo](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR) and [Examples](#examples) below
 
 ## Class Diagram
 ```
       Indexer    Measurer   Counter -- Tfidfer
            \          \     /             \
         Searcher     Tokenizer           Bm25er
-             \_______    |
+             \_______    |      ________________ Assistant
               _______Transformer______________
              /           |                    \
         Answerer     Translator              Abstractor
            /         /    |     \              /       \
   Responder  Vectorizer  Fitter  Variator  Questioner  Summarizer
                   /
           Identifier
@@ -78,14 +79,15 @@
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
 [Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
 [Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
 [Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
 [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Explain Text2Text in one sentence"]).assist()` | `['Text to text translation uses a deep learning model to generate a text in another language from a given source text.']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
 ## Languages Available
@@ -726,14 +728,23 @@
 dialog = ' EOS '.join(dialog)
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
+### Assistant
+Not chatGPT level but it works
+```
+res = t2t.Handler(["Outline steps for contributing to open source code"]).assist()
+# 1) Find an open source project that you are interested in. You can do this by searching the internet for the project name or using a search engine to find the project page on GitHub.
+# 2) Verify that you have the necessary permissions to make changes to the code. If the project uses basic permissions, you can use git to check out the code. If the code uses more advanced permissions, you can find a way to use those permissions.
+# 3) Perform a code review to ensure that your contributions are properly credits and, if necessary, include a reasoning of your changes.
+```
+
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
 result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"], 
             src_lang="en",
             tgt_lang="zh",
             num_epochs=10,
```

### Comparing `text2text-0.9.9/setup.py` & `text2text-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="0.9.9",
+  version="1.0.0",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
   classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
   ],
-  keywords='multilingual crosslingual bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot',
+  keywords='multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot',
   install_requires=[
     'accelerate',
     'bitsandbytes',
     'faiss-cpu',
     'flask',
     'googledrivedownloader',
     'numpy',
```

### Comparing `text2text-0.9.9/text2text/__init__.py` & `text2text-1.0.0/text2text/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .transformer import Transformer
+from .assistant import Assistant
 from .tokenizer import Tokenizer
 from .measurer import Measurer
 from .translator import Translator
 from .vectorizer import Vectorizer
 from .fitter import Fitter
 from .counter import Counter
 from .tfidfer import Tfidfer
```

### Comparing `text2text-0.9.9/text2text/abstractor.py` & `text2text-1.0.0/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/answerer.py` & `text2text-1.0.0/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/biunilm/loader_utils.py` & `text2text-1.0.0/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/biunilm/seq2seq_loader.py` & `text2text-1.0.0/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/bm25er.py` & `text2text-1.0.0/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/counter.py` & `text2text-1.0.0/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/fitter.py` & `text2text-1.0.0/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/handler.py` & `text2text-1.0.0/text2text/handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 class Handler(object):
   """
   Text Handler unified API for text transformers
   """
 
   EXPOSED_TRANSFORMERS = {
     "answer": t2t.Answerer,
+    "assist": t2t.Assistant,
     "bm25": t2t.Bm25er,
     "count": t2t.Counter,
     "identify":t2t.Identifier,
     "index": t2t.Indexer,
     "fit": t2t.Fitter,
     "measure": t2t.Measurer,
     "question": t2t.Questioner,
```

### Comparing `text2text-0.9.9/text2text/identifier.py` & `text2text-1.0.0/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/indexer.py` & `text2text-1.0.0/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/measurer.py` & `text2text-1.0.0/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.0.0/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.0.0/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.0.0/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.0.0/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.0.0/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/questioner.py` & `text2text-1.0.0/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/responder.py` & `text2text-1.0.0/text2text/responder.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/searcher.py` & `text2text-1.0.0/text2text/searcher.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/server.py` & `text2text-1.0.0/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/summarizer.py` & `text2text-1.0.0/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/tfidfer.py` & `text2text-1.0.0/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/tokenizer.py` & `text2text-1.0.0/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/transformer.py` & `text2text-1.0.0/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/translator.py` & `text2text-1.0.0/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text/vectorizer.py` & `text2text-1.0.0/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-0.9.9/text2text.egg-info/PKG-INFO` & `text2text-1.0.0/text2text.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 0.9.9
+Version: 1.0.0
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
-Keywords: multilingual crosslingual bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
+Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Text2Text: Crosslingual NLP/G toolkit
@@ -36,14 +36,15 @@
   * [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance)
   * [Translation](https://github.com/artitw/text2text#translation)
   * [Question Answering](https://github.com/artitw/text2text#question-answering)
   * [Question Generation](https://github.com/artitw/text2text#question-generation)
   * [Summarization](https://github.com/artitw/text2text#summarization)
   * [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation)
   * [Dialog Responder](https://github.com/artitw/text2text#dialog-responder)
+  * [Assistant](https://github.com/artitw/text2text#assistant)
   * [Finetuning](https://github.com/artitw/text2text#training--finetuning)
   * [Identification](https://github.com/artitw/text2text#identification)
   * [Web Server](https://github.com/artitw/text2text#serving)
 * [Questions?](https://github.com/artitw/text2text#questions)
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
 * [Code of Conduct](https://github.com/artitw/text2text#code-of-conduct)
@@ -65,15 +66,15 @@
   * See [Colab Demo](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR) and [Examples](#examples) below
 
 ## Class Diagram
 ```
       Indexer    Measurer   Counter -- Tfidfer
            \          \     /             \
         Searcher     Tokenizer           Bm25er
-             \_______    |
+             \_______    |      ________________ Assistant
               _______Transformer______________
              /           |                    \
         Answerer     Translator              Abstractor
            /         /    |     \              /       \
   Responder  Vectorizer  Fitter  Variator  Questioner  Summarizer
                   /
           Identifier
@@ -92,14 +93,15 @@
 [Indexer](https://github.com/artitw/text2text#index) | `i = h.index()` | Index object for similarity retrieval
 [Search](https://github.com/artitw/text2text#search) | `h.search(queries=["Hello"])` | `array([[0.09]])`
 [Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
 [Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
 [Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
 [Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler(["Explain Text2Text in one sentence"]).assist()` | `['Text to text translation uses a deep learning model to generate a text in another language from a given source text.']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
 ## Languages Available
@@ -740,14 +742,23 @@
 dialog = ' EOS '.join(dialog)
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
 t2t.Handler([input_state]).respond()
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
+### Assistant
+Not chatGPT level but it works
+```
+res = t2t.Handler(["Outline steps for contributing to open source code"]).assist()
+# 1) Find an open source project that you are interested in. You can do this by searching the internet for the project name or using a search engine to find the project page on GitHub.
+# 2) Verify that you have the necessary permissions to make changes to the code. If the project uses basic permissions, you can use git to check out the code. If the code uses more advanced permissions, you can find a way to use those permissions.
+# 3) Perform a code review to ensure that your contributions are properly credits and, if necessary, include a reasoning of your changes.
+```
+
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
 result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"], 
             src_lang="en",
             tgt_lang="zh",
             num_epochs=10,
```

### Comparing `text2text-0.9.9/text2text.egg-info/SOURCES.txt` & `text2text-1.0.0/text2text.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.txt
 README.md
 setup.py
 text2text/__init__.py
 text2text/abstractor.py
 text2text/answerer.py
+text2text/assistant.py
 text2text/bm25er.py
 text2text/counter.py
 text2text/fitter.py
 text2text/handler.py
 text2text/identifier.py
 text2text/indexer.py
 text2text/measurer.py
```

