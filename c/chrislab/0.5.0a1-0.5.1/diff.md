# Comparing `tmp/chrislab-0.5.0a1.tar.gz` & `tmp/chrislab-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrislab-0.5.0a1.tar", last modified: Fri May 12 08:16:33 2023, max compression
+gzip compressed data, was "chrislab-0.5.1.tar", last modified: Sun May 14 13:42:44 2023, max compression
```

## Comparing `chrislab-0.5.0a1.tar` & `chrislab-0.5.1.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.886947 chrislab-0.5.0a1/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      832 2023-05-12 08:16:33.886947 chrislab-0.5.0a1/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1148 2023-05-12 08:16:33.886947 chrislab-0.5.0a1/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.882947 chrislab-0.5.0a1/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.882947 chrislab-0.5.0a1/src/chrislab/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.882947 chrislab-0.5.0a1/src/chrislab/common/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/common/__init__.py
--rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/common/downloader.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14529 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/common/tokenizer_korbert.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    13164 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/common/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.886947 chrislab-0.5.0a1/src/chrislab/language/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/language/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1316 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/language/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/language/converter.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/language/evaluater.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    39567 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/language/finetuner.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/language/modeling.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/language/predictor.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.886947 chrislab-0.5.0a1/src/chrislab/ratsnlp/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/ratsnlp/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10788 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/chrislab/ratsnlp/cli.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.882947 chrislab-0.5.0a1/src/chrislab.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      832 2023-05-12 08:16:33.000000 chrislab-0.5.0a1/src/chrislab.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     1722 2023-05-12 08:16:33.000000 chrislab-0.5.0a1/src/chrislab.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-12 08:16:33.000000 chrislab-0.5.0a1/src/chrislab.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      108 2023-05-12 08:16:33.000000 chrislab-0.5.0a1/src/chrislab.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      249 2023-05-12 08:16:33.000000 chrislab-0.5.0a1/src/chrislab.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-05-12 08:16:33.000000 chrislab-0.5.0a1/src/chrislab.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-12 08:16:33.000000 chrislab-0.5.0a1/src/chrislab.egg-info/zip-safe
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.886947 chrislab-0.5.0a1/src/ratsnlp/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.886947 chrislab-0.5.0a1/src/ratsnlp/nlpbook/
--rw-rw-r--   0 chris     (1000) chris     (1000)       70 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6249 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/arguments.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.886947 chrislab-0.5.0a1/src/ratsnlp/nlpbook/classification/
--rw-rw-r--   0 chris     (1000) chris     (1000)       59 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/classification/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5626 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/classification/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1715 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/classification/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/data_utils.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      663 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/deploy.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.886947 chrislab-0.5.0a1/src/ratsnlp/nlpbook/generation/
--rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/generation/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/generation/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5379 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/generation/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/generation/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1301 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/generation/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      653 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/metrics.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.886947 chrislab-0.5.0a1/src/ratsnlp/nlpbook/ner/
--rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/ner/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12004 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/ner/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1802 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/ner/task.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.886947 chrislab-0.5.0a1/src/ratsnlp/nlpbook/paircls/
--rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/paircls/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2675 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/paircls/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/paircls/deploy.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:16:33.886947 chrislab-0.5.0a1/src/ratsnlp/nlpbook/qa/
--rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/qa/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/qa/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17108 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/qa/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/qa/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2088 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/qa/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1253 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/trainer.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8691 2023-05-12 07:41:54.000000 chrislab-0.5.0a1/src/ratsnlp/nlpbook/utils.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.617095 chrislab-0.5.1/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-05-12 08:42:23.000000 chrislab-0.5.1/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-05-14 13:42:44.617095 chrislab-0.5.1/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-05-12 08:42:23.000000 chrislab-0.5.1/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-05-12 08:42:23.000000 chrislab-0.5.1/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1203 2023-05-14 13:42:44.617095 chrislab-0.5.1/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.613095 chrislab-0.5.1/src/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.613095 chrislab-0.5.1/src/chrislab/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.613095 chrislab-0.5.1/src/chrislab/common/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/common/__init__.py
+-rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/common/downloader.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14529 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/common/tokenizer_korbert.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    13164 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/common/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.613095 chrislab-0.5.1/src/chrislab/language/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1316 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/converter.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/evaluater.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    39567 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/finetuner.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/modeling.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/predictor.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.613095 chrislab-0.5.1/src/chrislab.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1442 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      164 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/entry_points.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      249 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/zip-safe
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.613095 chrislab-0.5.1/src/nlpbook/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       70 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6033 2023-05-14 13:30:52.000000 chrislab-0.5.1/src/nlpbook/arguments.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.617095 chrislab-0.5.1/src/nlpbook/cls/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       59 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/cls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5289 2023-05-14 13:16:43.000000 chrislab-0.5.1/src/nlpbook/cls/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5726 2023-05-14 13:15:00.000000 chrislab-0.5.1/src/nlpbook/cls/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1740 2023-05-14 13:20:25.000000 chrislab-0.5.1/src/nlpbook/cls/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/data_utils.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      663 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/deploy.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.617095 chrislab-0.5.1/src/nlpbook/generation/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/generation/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/generation/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5371 2023-05-14 13:19:21.000000 chrislab-0.5.1/src/nlpbook/generation/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/generation/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1293 2023-05-14 13:21:01.000000 chrislab-0.5.1/src/nlpbook/generation/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      653 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/metrics.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.617095 chrislab-0.5.1/src/nlpbook/ner/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/ner/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7513 2023-05-14 13:16:43.000000 chrislab-0.5.1/src/nlpbook/ner/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11914 2023-05-14 13:20:25.000000 chrislab-0.5.1/src/nlpbook/ner/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8099 2023-05-14 13:20:25.000000 chrislab-0.5.1/src/nlpbook/ner/task.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.617095 chrislab-0.5.1/src/nlpbook/paircls/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/paircls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2656 2023-05-14 13:15:23.000000 chrislab-0.5.1/src/nlpbook/paircls/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/paircls/deploy.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.617095 chrislab-0.5.1/src/nlpbook/qa/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/qa/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/qa/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    17104 2023-05-14 13:20:44.000000 chrislab-0.5.1/src/nlpbook/qa/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/qa/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2072 2023-05-14 13:20:34.000000 chrislab-0.5.1/src/nlpbook/qa/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1468 2023-05-14 13:19:09.000000 chrislab-0.5.1/src/nlpbook/trainer.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8696 2023-05-12 08:57:23.000000 chrislab-0.5.1/src/nlpbook/utils.py
```

### Comparing `chrislab-0.5.0a1/LICENSE` & `chrislab-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/PKG-INFO` & `chrislab-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.0a1
+Version: 0.5.1
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.0a1/setup.cfg` & `chrislab-0.5.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrislab
-version = 0.5.0a1
+version = 0.5.1
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrislab
 description = An advanced tool for doing experimental study.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
@@ -48,13 +48,14 @@
 
 [options.package_data]
 * = README.md
 
 [options.entry_points]
 console_scripts = 
 	chrislab.language = chrislab.language.cli:app
-	chrislab.ratsnlp = chrislab.ratsnlp.cli:app
+	ratsnlp.nlpbook.cls = ratsnlp.nlpbook.cls.cli:app
+	ratsnlp.nlpbook.ner = ratsnlp.nlpbook.ner.cli:app
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `chrislab-0.5.0a1/src/chrislab/common/downloader.py` & `chrislab-0.5.1/src/chrislab/common/downloader.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/chrislab/common/tokenizer_korbert.py` & `chrislab-0.5.1/src/chrislab/common/tokenizer_korbert.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/chrislab/common/util.py` & `chrislab-0.5.1/src/chrislab/common/util.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/chrislab/language/cli.py` & `chrislab-0.5.1/src/chrislab/language/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/chrislab/language/converter.py` & `chrislab-0.5.1/src/chrislab/language/converter.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/chrislab/language/evaluater.py` & `chrislab-0.5.1/src/chrislab/language/evaluater.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/chrislab/language/finetuner.py` & `chrislab-0.5.1/src/chrislab/language/finetuner.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/chrislab/language/modeling.py` & `chrislab-0.5.1/src/chrislab/language/modeling.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/chrislab/language/predictor.py` & `chrislab-0.5.1/src/chrislab/language/predictor.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/chrislab/ratsnlp/cli.py` & `chrislab-0.5.1/src/nlpbook/cls/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,103 +2,27 @@
 
 import torch
 from Korpora import Korpora
 from torch.utils.data import DataLoader, RandomSampler
 from torch.utils.data import SequentialSampler
 from typer import Typer
 
+import nlpbook
 from chrisbase.io import JobTimer, out_hr
-from ratsnlp import nlpbook
-from ratsnlp.nlpbook.deploy import get_web_service_app
-from ratsnlp.nlpbook.arguments import NLUTrainerArguments, NLUServerArguments
-from ratsnlp.nlpbook.classification.corpus import NsmcCorpus, ClassificationDataset
-from ratsnlp.nlpbook.classification.task import ClassificationTask
-from ratsnlp.nlpbook.ner.corpus import NERCorpus, NERDataset
-from ratsnlp.nlpbook.ner.task import NERTask
-from transformers import BertConfig, BertForSequenceClassification, BertForTokenClassification
+from nlpbook.arguments import NLUTrainerArguments, NLUServerArguments
+from nlpbook.cls.corpus import NsmcCorpus, ClassificationDataset
+from nlpbook.cls.task import ClassificationTask
+from nlpbook.deploy import get_web_service_app
+from transformers import BertConfig, BertForSequenceClassification
 from transformers import BertTokenizer
 
 app = Typer()
 
 
 @app.command()
-def train_ner(config: Path | str):
-    config = Path(config)
-    assert config.exists(), f"No config file: {config}"
-    args = NLUTrainerArguments.from_json(config.read_text())
-    args.print_dataframe()
-
-    with JobTimer(f"chrialab.ratsnlp train_ner {config}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
-        nlpbook.set_seed(args)
-        nlpbook.set_logger()
-        out_hr(c='-')
-
-        nlpbook.download_downstream_dataset(args)
-        out_hr(c='-')
-
-        tokenizer = BertTokenizer.from_pretrained(
-            args.pretrained_model_path,
-            do_lower_case=False,
-        )
-        print(f"tokenizer={tokenizer}")
-        print(f"tokenized={tokenizer.tokenize('안녕하세요. 반갑습니다.')}")
-        out_hr(c='-')
-
-        corpus = NERCorpus(args)
-        train_dataset = NERDataset(
-            args=args,
-            corpus=corpus,
-            tokenizer=tokenizer,
-            mode="train",
-        )
-        train_dataloader = DataLoader(
-            train_dataset,
-            batch_size=args.batch_size,
-            sampler=RandomSampler(train_dataset, replacement=False),
-            collate_fn=nlpbook.data_collator,
-            drop_last=False,
-            num_workers=args.cpu_workers,
-        )
-        out_hr(c='-')
-
-        val_dataset = NERDataset(
-            args=args,
-            corpus=corpus,
-            tokenizer=tokenizer,
-            mode="val",
-        )
-        val_dataloader = DataLoader(
-            val_dataset,
-            batch_size=args.batch_size,
-            sampler=SequentialSampler(val_dataset),
-            collate_fn=nlpbook.data_collator,
-            drop_last=False,
-            num_workers=args.cpu_workers,
-        )
-        out_hr(c='-')
-
-        pretrained_model_config = BertConfig.from_pretrained(
-            args.pretrained_model_path,
-            num_labels=corpus.num_labels,
-        )
-        model = BertForTokenClassification.from_pretrained(
-            args.pretrained_model_path,
-            config=pretrained_model_config,
-        )
-        out_hr(c='-')
-
-        torch.set_float32_matmul_precision('high')
-        nlpbook.get_trainer(args).fit(
-            NERTask(model, args),
-            train_dataloaders=train_dataloader,
-            val_dataloaders=val_dataloader,
-        )
-
-
-@app.command()
 def train_cls(config: Path | str):
     config = Path(config)
     assert config.exists(), f"No config file: {config}"
     args = NLUTrainerArguments.from_json(config.read_text())
     args.print_dataframe()
 
     with JobTimer(f"chrialab.ratsnlp train_cls {config}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
@@ -168,98 +92,33 @@
             ClassificationTask(model, args),
             train_dataloaders=train_dataloader,
             val_dataloaders=val_dataloader,
         )
 
 
 @app.command()
-def serve_ner(config: Path | str):
-    config = Path(config)
-    assert config.exists(), f"No config file: {config}"
-    args = NLUServerArguments.from_json(config.read_text())
-    args.print_dataframe()
-
-    with JobTimer(f"chrialab.ratsnlp serve {config}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
-        downstream_model_path = args.downstream_model_home / args.downstream_model_file
-        assert downstream_model_path.exists(), f"No downstream model file: {downstream_model_path}"
-        downstream_model_ckpt = torch.load(downstream_model_path, map_location=torch.device("cpu"))
-        pretrained_model_config = BertConfig.from_pretrained(
-            args.pretrained_model_path,
-            num_labels=downstream_model_ckpt['state_dict']['model.classifier.bias'].shape.numel(),
-        )
-        model = BertForTokenClassification(pretrained_model_config)
-        model.load_state_dict({k.replace("model.", ""): v for k, v in downstream_model_ckpt['state_dict'].items()})
-        model.eval()
-
-        tokenizer = BertTokenizer.from_pretrained(
-            args.pretrained_model_path,
-            do_lower_case=False,
-        )
-
-        downstream_label_path: Path = args.downstream_model_home / "label_map.txt"
-        assert downstream_label_path.exists(), f"No downstream label file: {downstream_label_path}"
-        labels = downstream_label_path.read_text().splitlines(keepends=False)
-        id_to_label = {idx: label for idx, label in enumerate(labels)}
-
-        def inference_fn(sentence):
-            from transformers.modeling_outputs import TokenClassifierOutput
-            from torch import Tensor
-            inputs = tokenizer(
-                [sentence],
-                max_length=args.max_seq_length,
-                padding="max_length",
-                truncation=True,
-            )
-            with torch.no_grad():
-                outputs: TokenClassifierOutput = model(**{k: torch.tensor(v) for k, v in inputs.items()})
-                all_probs: Tensor = outputs.logits[0].softmax(dim=1)
-                top_probs, top_preds = torch.topk(all_probs, dim=1, k=1)
-                tokens = tokenizer.convert_ids_to_tokens(inputs["input_ids"][0])
-                top_labels = [id_to_label[pred[0].item()] for pred in top_preds]
-                result = []
-                for token, label, top_prob in zip(tokens, top_labels, top_probs):
-                    if token in tokenizer.all_special_tokens:
-                        continue
-                    result.append({
-                        "token": token,
-                        "label": label,
-                        "prob": f"{round(top_prob[0].item(), 4):.4f}",
-                    })
-            return {
-                'sentence': sentence,
-                'result': result,
-            }
-
-        service = get_web_service_app(inference_fn, template_file="serve_ner.html", ngrok_home=args.env.working_path)
-        service.run()
-
-
-@app.command()
 def serve_cls(config: Path | str):
     config = Path(config)
     assert config.exists(), f"No config file: {config}"
     args = NLUServerArguments.from_json(config.read_text())
     args.print_dataframe()
 
-    with JobTimer(f"chrialab.ratsnlp serve {config}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
+    with JobTimer(f"chrialab.ratsnlp serve_cls {config}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         downstream_model_path = args.downstream_model_home / args.downstream_model_file
         assert downstream_model_path.exists(), f"No downstream model file: {downstream_model_path}"
         downstream_model_ckpt = torch.load(downstream_model_path, map_location=torch.device("cpu"))
         pretrained_model_config = BertConfig.from_pretrained(
             args.pretrained_model_path,
             num_labels=downstream_model_ckpt['state_dict']['model.classifier.bias'].shape.numel(),
         )
         model = BertForSequenceClassification(pretrained_model_config)
         model.load_state_dict({k.replace("model.", ""): v for k, v in downstream_model_ckpt['state_dict'].items()})
         model.eval()
 
-        tokenizer = BertTokenizer.from_pretrained(
-            args.pretrained_model_path,
-            do_lower_case=False,
-        )
+        tokenizer = BertTokenizer.from_pretrained(args.pretrained_model_path, do_lower_case=False)
 
         def inference_fn(sentence):
             inputs = tokenizer(
                 [sentence],
                 max_length=args.max_seq_length,
                 padding="max_length",
                 truncation=True,
```

### Comparing `chrislab-0.5.0a1/src/chrislab.egg-info/PKG-INFO` & `chrislab-0.5.1/src/chrislab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.0a1
+Version: 0.5.1
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.0a1/src/chrislab.egg-info/SOURCES.txt` & `chrislab-0.5.1/src/chrislab.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -17,36 +17,35 @@
 src/chrislab/language/__init__.py
 src/chrislab/language/cli.py
 src/chrislab/language/converter.py
 src/chrislab/language/evaluater.py
 src/chrislab/language/finetuner.py
 src/chrislab/language/modeling.py
 src/chrislab/language/predictor.py
-src/chrislab/ratsnlp/__init__.py
-src/chrislab/ratsnlp/cli.py
-src/ratsnlp/__init__.py
-src/ratsnlp/nlpbook/__init__.py
-src/ratsnlp/nlpbook/arguments.py
-src/ratsnlp/nlpbook/data_utils.py
-src/ratsnlp/nlpbook/deploy.py
-src/ratsnlp/nlpbook/metrics.py
-src/ratsnlp/nlpbook/trainer.py
-src/ratsnlp/nlpbook/utils.py
-src/ratsnlp/nlpbook/classification/__init__.py
-src/ratsnlp/nlpbook/classification/corpus.py
-src/ratsnlp/nlpbook/classification/task.py
-src/ratsnlp/nlpbook/generation/__init__.py
-src/ratsnlp/nlpbook/generation/arguments.py
-src/ratsnlp/nlpbook/generation/corpus.py
-src/ratsnlp/nlpbook/generation/deploy.py
-src/ratsnlp/nlpbook/generation/task.py
-src/ratsnlp/nlpbook/ner/__init__.py
-src/ratsnlp/nlpbook/ner/corpus.py
-src/ratsnlp/nlpbook/ner/task.py
-src/ratsnlp/nlpbook/paircls/__init__.py
-src/ratsnlp/nlpbook/paircls/corpus.py
-src/ratsnlp/nlpbook/paircls/deploy.py
-src/ratsnlp/nlpbook/qa/__init__.py
-src/ratsnlp/nlpbook/qa/arguments.py
-src/ratsnlp/nlpbook/qa/corpus.py
-src/ratsnlp/nlpbook/qa/deploy.py
-src/ratsnlp/nlpbook/qa/task.py
+src/nlpbook/__init__.py
+src/nlpbook/arguments.py
+src/nlpbook/data_utils.py
+src/nlpbook/deploy.py
+src/nlpbook/metrics.py
+src/nlpbook/trainer.py
+src/nlpbook/utils.py
+src/nlpbook/cls/__init__.py
+src/nlpbook/cls/cli.py
+src/nlpbook/cls/corpus.py
+src/nlpbook/cls/task.py
+src/nlpbook/generation/__init__.py
+src/nlpbook/generation/arguments.py
+src/nlpbook/generation/corpus.py
+src/nlpbook/generation/deploy.py
+src/nlpbook/generation/task.py
+src/nlpbook/ner/__init__.py
+src/nlpbook/ner/cli.py
+src/nlpbook/ner/corpus.py
+src/nlpbook/ner/task.py
+src/nlpbook/paircls/__init__.py
+src/nlpbook/paircls/corpus.py
+src/nlpbook/paircls/deploy.py
+src/nlpbook/qa/__init__.py
+src/nlpbook/qa/arguments.py
+src/nlpbook/qa/corpus.py
+src/nlpbook/qa/deploy.py
+src/nlpbook/qa/task.py
```

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/arguments.py` & `chrislab-0.5.1/src/nlpbook/arguments.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from chrisbase.io import ProjectEnv
 from chrisbase.io import files, make_parent_dir, out_hr, out_table
 from chrisbase.util import to_dataframe
 
 
 @dataclass
 class NLUArguments(DataClassJsonMixin):
+    postfix = None
+
     def env_data(self) -> ProjectEnv:
         if isinstance(self.env, ProjectEnv):
             return self.env
         else:
             return ProjectEnv.from_dict(self.env)
 
     def env_dict(self) -> dict:
@@ -26,18 +28,26 @@
             return self.env.to_dict()
         else:
             return self.env
 
     def __post_init__(self):
         self.env = self.env_data()
         self.downstream_model_home = Path(self.downstream_model_home)
+        if not self.working_config_file:
+            self.working_config_file = self.downstream_model_home \
+                .with_stem(self.downstream_model_home.stem + (f"={self.postfix}" if self.postfix else "")) \
+                .with_suffix('.json').name
 
     env: ProjectEnv | dict = field(
         metadata={"help": "current project environment"}
     )
+    working_config_file: str | None = field(
+        default=None,
+        metadata={"help": "filename of current config"}
+    )
     pretrained_model_path: Path | str | None = field(
         default="beomi/kcbert-base",
         metadata={"help": "name/path of pretrained model"}
     )
     downstream_model_home: Path | str | None = field(
         default=None,
         metadata={"help": "root directory of output model and working config"}
@@ -46,17 +56,33 @@
         default=None,
         metadata={"help": "filename or filename format of output model"}
     )
     downstream_task_name: str | None = field(
         default=None,
         metadata={"help": "name of downstream task"}
     )
-    working_config_file: str | None = field(
+    downstream_data_home: Path | str | None = field(
         default=None,
-        metadata={"help": "filename of current config"}
+        metadata={"help": "root of downstream data"}
+    )
+    downstream_data_name: str | None = field(
+        default=None,
+        metadata={"help": "name of downstream data"}
+    )
+    downstream_data_file: str | None = field(
+        default=None,
+        metadata={"help": "filename of downstream data"}
+    )
+    overwrite_cache: bool = field(
+        default=False,
+        metadata={"help": "overwrite the cached training and evaluation sets"}
+    )
+    force_download: bool = field(
+        default=False,
+        metadata={"help": "force to download downstream data and pretrained models"}
     )
     max_seq_length: int = field(
         default=128,
         metadata={"help": "The maximum total input sequence length after tokenization. "
                           "Sequences longer than this will be truncated, sequences shorter will be padded."}
     )
 
@@ -77,99 +103,81 @@
         out_hr(c='-')
         out_table(self.as_dataframe())
         out_hr(c='-')
         return self
 
 
 @dataclass
-class NLUTrainerArguments(NLUArguments):
+class NLUServerArguments(NLUArguments):
+    postfix = "serve"
+
+    def __post_init__(self):
+        super().__post_init__()
+        if self.downstream_model_home.exists() and self.downstream_model_home.is_dir() and not self.downstream_model_file:
+            ckpt_files = files(self.downstream_model_home / "*.ckpt")
+            ckpt_files = sorted([x for x in ckpt_files if "temp" not in str(x) and "tmp" not in str(x)], key=str)
+            assert len(ckpt_files) > 0, f"No checkpoint file in {self.downstream_model_home}"
+            self.downstream_model_file = ckpt_files[-1].name
+
+
+@dataclass
+class NLUTesterArguments(NLUServerArguments):
+    postfix = "test"
+
     def __post_init__(self):
         super().__post_init__()
-        self.downstream_data_home = Path(self.downstream_data_home)
-        if not self.working_config_file:
-            self.working_config_file = self.downstream_model_home \
-                .with_stem(self.downstream_model_home.stem + "=train") \
-                .with_suffix('.json').name
-        if not self.save_top_k:
-            self.save_top_k = self.epochs
 
-    downstream_data_home: Path | str | None = field(
-        default="/content/Korpora",
-        metadata={"help": "root of downstream data"}
-    )
-    downstream_data_name: str | None = field(
-        default=None,
-        metadata={"help": "name of downstream data"}
-    )
-    save_top_k: int = field(
-        default=None,
-        metadata={"help": "save top k model checkpoints"}
-    )
-    monitor: str = field(
-        default="min val_loss",
-        metadata={"help": "monitor condition (save top k)"}
-    )
-    seed: int | None = field(
-        default=None,
-        metadata={"help": "random seed"}
-    )
-    overwrite_cache: bool = field(
-        default=False,
-        metadata={"help": "overwrite the cached training and evaluation sets"}
-    )
-    force_download: bool = field(
-        default=False,
-        metadata={"help": "force to download downstream data and pretrained models"}
-    )
-    test_mode: bool = field(
-        default=False,
-        metadata={"help": "test mode enables `fast_dev_run`"}
-    )
-    learning_rate: float = field(
-        default=5e-5,
-        metadata={"help": "learning rate"}
-    )
-    epochs: int = field(
-        default=1,
-        metadata={"help": "max epochs"}
-    )
     batch_size: int = field(
         default=32,
         metadata={"help": "batch size. if 0, let lightening find the best batch size"}
     )
     cpu_workers: int = field(
         default=os.cpu_count(),
         metadata={"help": "number of CPU workers"}
     )
     accelerator: str | Accelerator = field(
         default="auto",
         metadata={"help": 'accelerator types ("cpu", "gpu", "tpu", "ipu", "hpu", "mps", "auto")'}
     )
     precision: str | int = field(
-        default="32-true",
+        default=32,
         metadata={"help": "floating-point precision type"}
     )
     strategy: str | Strategy = field(
-        default="auto",
+        default="single_device",
         metadata={"help": 'training strategies'}
     )
     devices: List[int] | str | int = field(
-        default="auto",
+        default=1,
         metadata={"help": 'devices to use'}
     )
 
 
 @dataclass
-class NLUServerArguments(NLUArguments):
+class NLUTrainerArguments(NLUTesterArguments):
+    postfix = "train"
+
     def __post_init__(self):
         super().__post_init__()
-        assert self.downstream_model_home.exists(), f"downstream_model_home does not exist: {self.downstream_model_home}"
-        assert self.downstream_model_home.is_dir(), f"downstream_model_home is not a directory: {self.downstream_model_home}"
-        if not self.working_config_file:
-            self.working_config_file = self.downstream_model_home \
-                .with_stem(self.downstream_model_home.stem + "=serve") \
-                .with_suffix('.json').name
-        if not self.downstream_model_file:
-            ckpt_files = files(self.downstream_model_home / "*.ckpt")
-            ckpt_files = sorted([x for x in ckpt_files if "temp" not in str(x) and "tmp" not in str(x)], key=str)
-            assert len(ckpt_files) > 0, f"No checkpoint file in {self.downstream_model_home}"
-            self.downstream_model_file = ckpt_files[-1].name
+        if not self.save_top_k:
+            self.save_top_k = self.epochs
+
+    learning_rate: float = field(
+        default=5e-5,
+        metadata={"help": "learning rate"}
+    )
+    epochs: int = field(
+        default=1,
+        metadata={"help": "max epochs"}
+    )
+    save_top_k: int = field(
+        default=None,
+        metadata={"help": "save top k model checkpoints"}
+    )
+    monitor: str = field(
+        default="min val_loss",
+        metadata={"help": "monitor condition (save top k)"}
+    )
+    seed: int | None = field(
+        default=None,
+        metadata={"help": "random seed"}
+    )
```

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/classification/corpus.py` & `chrislab-0.5.1/src/nlpbook/cls/corpus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import csv
 import logging
 import os
 import time
 from dataclasses import dataclass
+from pathlib import Path
 from typing import List, Optional
 
 import torch
 from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 
-from ratsnlp.nlpbook import NLUTrainerArguments
+from nlpbook.arguments import NLUTrainerArguments
 from transformers import PreTrainedTokenizer
 
 logger = logging.getLogger("ratsnlp")
 
 
 @dataclass
 class ClassificationExample:
@@ -115,15 +116,15 @@
         if not mode in ["train", "val", "test"]:
             raise KeyError(f"mode({mode}) is not a valid split name")
         # Load data features from cache or dataset file
         cached_features_file = os.path.join(
             args.downstream_data_home,
             args.downstream_data_name,
             "cached_{}_{}_{}_{}_{}".format(
-                mode,
+                Path(args.downstream_data_file).stem,
                 tokenizer.__class__.__name__,
                 str(args.max_seq_length),
                 args.downstream_data_name,
                 args.downstream_task_name,
             ),
         )
 
@@ -138,17 +139,18 @@
                 logger.info(
                     f"Loading features from cached file {cached_features_file} [took %.3f s]", time.time() - start
                 )
             else:
                 corpus_path = os.path.join(
                     args.downstream_data_home,
                     args.downstream_data_name,
+                    args.downstream_data_file,
                 )
                 logger.info(f"Creating features from dataset file at {corpus_path}")
-                examples = self.corpus.get_examples(corpus_path, mode)
+                examples = self.corpus.get_examples(corpus_path)
                 self.features = convert_examples_to_features_fn(
                     examples,
                     tokenizer,
                     args,
                     label_list=self.corpus.get_labels(),
                 )
                 start = time.time()
```

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/classification/task.py` & `chrislab-0.5.1/src/nlpbook/cls/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pytorch_lightning import LightningModule
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
 
-from ratsnlp.nlpbook import NLUTrainerArguments
-from ratsnlp.nlpbook.metrics import accuracy
+from nlpbook.arguments import NLUTrainerArguments
+from nlpbook.metrics import accuracy
 from transformers import PreTrainedModel
+from transformers.modeling_outputs import SequenceClassifierOutput
 
 
 class ClassificationTask(LightningModule):
 
     def __init__(self,
                  model: PreTrainedModel,
                  args: NLUTrainerArguments,
@@ -22,25 +23,23 @@
         scheduler = ExponentialLR(optimizer, gamma=0.9)
         return {
             'optimizer': optimizer,
             'scheduler': scheduler,
         }
 
     def training_step(self, inputs, batch_idx):
-        # outputs: SequenceClassifierOutput
-        outputs = self.model(**inputs)
+        outputs: SequenceClassifierOutput = self.model(**inputs)
         preds = outputs.logits.argmax(dim=-1)
         labels = inputs["labels"]
         acc = accuracy(preds, labels)
         self.log("loss", outputs.loss, prog_bar=False, logger=True, on_step=True, on_epoch=False)
         self.log("acc", acc, prog_bar=True, logger=True, on_step=True, on_epoch=False)
         return outputs.loss
 
     def validation_step(self, inputs, batch_idx):
-        # outputs: SequenceClassifierOutput
-        outputs = self.model(**inputs)
+        outputs: SequenceClassifierOutput = self.model(**inputs)
         preds = outputs.logits.argmax(dim=-1)
         labels = inputs["labels"]
         acc = accuracy(preds, labels)
         self.log("val_loss", outputs.loss, prog_bar=True, logger=True, on_step=False, on_epoch=True)
         self.log("val_acc", acc, prog_bar=True, logger=True, on_step=False, on_epoch=True)
         return outputs.loss
```

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/data_utils.py` & `chrislab-0.5.1/src/nlpbook/data_utils.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/deploy.py` & `chrislab-0.5.1/src/nlpbook/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/generation/arguments.py` & `chrislab-0.5.1/src/nlpbook/generation/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/generation/corpus.py` & `chrislab-0.5.1/src/nlpbook/generation/corpus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import os
 import csv
-import time
-import torch
 import logging
-from filelock import FileLock
+import os
+import time
 from dataclasses import dataclass
 from typing import List, Optional
+
+import torch
+from filelock import FileLock
 from torch.utils.data.dataset import Dataset
-from transformers import PreTrainedTokenizerFast
-from ratsnlp.nlpbook.generation.arguments import GenerationTrainArguments
 
+from nlpbook.generation.arguments import GenerationTrainArguments
+from transformers import PreTrainedTokenizerFast
 
 logger = logging.getLogger("ratsnlp")
 
 
 @dataclass
 class GenerationExample:
     text: str
@@ -54,15 +55,14 @@
 
 
 def _convert_examples_to_generation_features(
         examples: List[GenerationExample],
         tokenizer: PreTrainedTokenizerFast,
         args: GenerationTrainArguments,
 ):
-
     logger.info(
         "tokenize sentences, it could take a lot of time..."
     )
     start = time.time()
     batch_encoding = tokenizer(
         [example.text for example in examples],
         max_length=args.max_seq_length,
```

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/generation/deploy.py` & `chrislab-0.5.1/src/nlpbook/generation/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/generation/task.py` & `chrislab-0.5.1/src/nlpbook/generation/task.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pytorch_lightning import LightningModule
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
 
-from ratsnlp.nlpbook.generation.arguments import GenerationTrainArguments
+from nlpbook.generation.arguments import GenerationTrainArguments
 from transformers import PreTrainedModel
 
 
 class GenerationTask(LightningModule):
 
     def __init__(self,
                  model: PreTrainedModel,
```

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/metrics.py` & `chrislab-0.5.1/src/nlpbook/metrics.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/ner/corpus.py` & `chrislab-0.5.1/src/nlpbook/ner/corpus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 import os
 import re
 import time
 from dataclasses import dataclass
+from pathlib import Path
 from typing import List, Optional
 
 import torch
 from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 
-from ratsnlp.nlpbook import NLUTrainerArguments
+from nlpbook.arguments import NLUTrainerArguments, NLUTesterArguments
 from transformers import BertTokenizer
 from transformers.tokenization_utils_base import PaddingStrategy, TruncationStrategy
 
 logger = logging.getLogger("ratsnlp")
 
 # 자체 제작 NER 코퍼스 기준의 레이블 시퀀스를 만들기 위한 ID 체계
 # 나 는 삼성 에 입사 했다
@@ -39,23 +40,22 @@
     label_ids: Optional[List[int]] = None
 
 
 class NERCorpus:
 
     def __init__(
             self,
-            args: NLUTrainerArguments
+            args: NLUTrainerArguments | NLUTesterArguments,
     ):
         self.args = args
 
-    def get_examples(self, data_root_path, mode):
-        data_fpath = os.path.join(data_root_path, f"{mode}.txt")
-        logger.info(f"loading {mode} data... LOOKING AT {data_fpath}")
+    def get_examples(self, data_path):
+        logger.info(f"loading data from {data_path}...")
         examples = []
-        for line in open(data_fpath, "r", encoding="utf-8").readlines():
+        for line in open(data_path, "r", encoding="utf-8").readlines():
             text, label = line.split("\u241E")
             examples.append(NERExample(text=text, label=label))
         return examples
 
     def get_labels(self):
         label_map_path = os.path.join(
             self.args.downstream_model_home,
@@ -247,32 +247,29 @@
     return features
 
 
 class NERDataset(Dataset):
 
     def __init__(
             self,
-            args: NLUTrainerArguments,
+            args: NLUTrainerArguments | NLUTesterArguments,
             tokenizer: BertTokenizer,
             corpus: NERCorpus,
-            mode: Optional[str] = "train",
             convert_examples_to_features_fn=_convert_examples_to_ner_features,
     ):
         if corpus is not None:
             self.corpus = corpus
         else:
             raise KeyError("corpus is not valid")
-        if not mode in ["train", "val", "test"]:
-            raise KeyError(f"mode({mode}) is not a valid split name")
         # Load data features from cache or dataset file
         cached_features_file = os.path.join(
             args.downstream_data_home,
             args.downstream_data_name,
             "cached_{}_{}_{}_{}_{}".format(
-                mode,
+                Path(args.downstream_data_file).stem,
                 tokenizer.__class__.__name__,
                 str(args.max_seq_length),
                 args.downstream_data_name,
                 args.downstream_task_name,
             ),
         )
 
@@ -287,17 +284,18 @@
                 logger.info(
                     f"Loading features from cached file {cached_features_file} [took %.3f s]", time.time() - start
                 )
             else:
                 corpus_path = os.path.join(
                     args.downstream_data_home,
                     args.downstream_data_name,
+                    args.downstream_data_file,
                 )
                 logger.info(f"Creating features from dataset file at {corpus_path}")
-                examples = self.corpus.get_examples(corpus_path, mode)
+                examples = self.corpus.get_examples(corpus_path)
                 self.features = convert_examples_to_features_fn(
                     examples,
                     tokenizer,
                     args,
                     label_list=self.corpus.get_labels(),
                 )
                 start = time.time()
```

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/paircls/corpus.py` & `chrislab-0.5.1/src/nlpbook/paircls/corpus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import json
 import logging
-from ratsnlp.nlpbook.classification.corpus import ClassificationExample
+from nlpbook.cls.corpus import ClassificationExample
 
 
 logger = logging.getLogger("ratsnlp")
 
 
 class KlueNLICorpus:
```

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/paircls/deploy.py` & `chrislab-0.5.1/src/nlpbook/paircls/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/qa/arguments.py` & `chrislab-0.5.1/src/nlpbook/qa/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/qa/corpus.py` & `chrislab-0.5.1/src/nlpbook/qa/corpus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import os
-import time
 import json
-import torch
 import logging
-from tqdm import tqdm
-from functools import partial
-from filelock import FileLock
+import os
+import time
 from dataclasses import dataclass
-from typing import List, Optional
+from functools import partial
 from multiprocessing import Pool, cpu_count
-from transformers import PreTrainedTokenizer
+from typing import List, Optional
+
+import torch
+from filelock import FileLock
 from torch.utils.data.dataset import Dataset
-from ratsnlp.nlpbook.qa import QATrainArguments
+from tqdm import tqdm
 
+from nlpbook.qa import QATrainArguments
+from transformers import PreTrainedTokenizer
 
 logger = logging.getLogger("ratsnlp")
 
 
 @dataclass
 class QAExample:
     # 질문 : 임종석이 여의도 농민 폭력 시위를 주도한 혐의로 지명수배 된 날은?
@@ -108,15 +109,15 @@
 
 
 def _improve_answer_span(doc_tokens, input_start, input_end, tokenizer, orig_answer_text):
     """Returns tokenized answer spans that better match the annotated answer."""
     tok_answer_text = " ".join(tokenizer.tokenize(orig_answer_text))
     for new_start in range(input_start, input_end + 1):
         for new_end in range(input_end, new_start - 1, -1):
-            text_span = " ".join(doc_tokens[new_start : (new_end + 1)])
+            text_span = " ".join(doc_tokens[new_start: (new_end + 1)])
             if text_span == tok_answer_text:
                 return new_start, new_end
     return input_start, input_end
 
 
 def _squad_convert_example_to_features(example, max_seq_length, doc_stride, max_query_length):
     features = []
@@ -240,15 +241,15 @@
 
         encoded_dict["start"] = len(spans) * doc_stride
         encoded_dict["length"] = paragraph_len
 
         spans.append(encoded_dict)
 
         if "overflowing_tokens" not in encoded_dict or (
-            "overflowing_tokens" in encoded_dict and len(encoded_dict["overflowing_tokens"]) == 0
+                "overflowing_tokens" in encoded_dict and len(encoded_dict["overflowing_tokens"]) == 0
         ):
             break
         # tokenizer.encode_plus에서 return_overflowing_tokens=True로 켜면
         # truncate하고 남은 토큰들을 리턴한다, 이를 span_doc_tokens에 다시 넣어 재처리한다
         # 이렇게 하는 이유는 max_seq_length보다 보통 context_text가 길기 때문에
         # 동일한 question-context pair로부터 학습 인스턴스를 stride해 가며 여러 개를 복제
         span_doc_tokens = encoded_dict["overflowing_tokens"]
```

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/qa/deploy.py` & `chrislab-0.5.1/src/nlpbook/qa/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/qa/task.py` & `chrislab-0.5.1/src/nlpbook/qa/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pytorch_lightning import LightningModule
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
 
-from ratsnlp.nlpbook.metrics import accuracy
-from ratsnlp.nlpbook.qa import QATrainArguments
+from nlpbook.metrics import accuracy
+from nlpbook.qa import QATrainArguments
 from transformers import PreTrainedModel
 
 
 class QATask(LightningModule):
 
     def __init__(self,
                  model: PreTrainedModel,
```

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/trainer.py` & `chrislab-0.5.1/src/nlpbook/trainer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,40 @@
-import os
-
 import torch
-
 from pytorch_lightning import Trainer
 from pytorch_lightning.callbacks import ModelCheckpoint
-from ratsnlp.nlpbook.arguments import NLUTrainerArguments
+
+from chrisbase.io import make_dir
+from nlpbook.arguments import NLUTrainerArguments, NLUTesterArguments
 
 
-def get_trainer(args: NLUTrainerArguments, return_trainer_only=True):
-    ckpt_path = os.path.abspath(args.downstream_model_home)
-    os.makedirs(ckpt_path, exist_ok=True)
+def get_trainer(args: NLUTrainerArguments):
+    downstream_model_home = make_dir(args.downstream_model_home)
     checkpoint_callback = ModelCheckpoint(
-        dirpath=ckpt_path,
+        dirpath=downstream_model_home,
         filename=args.downstream_model_file,
         save_top_k=args.save_top_k,
         monitor=args.monitor.split()[1],
         mode=args.monitor.split()[0],
     )
     trainer = Trainer(
+        num_sanity_val_steps=0,
         max_epochs=args.epochs,
-        fast_dev_run=args.test_mode,
-        num_sanity_val_steps=None if args.test_mode else 0,
         callbacks=[checkpoint_callback],
-        default_root_dir=ckpt_path,
+        default_root_dir=downstream_model_home,
         deterministic=torch.cuda.is_available() and args.seed is not None,
         accelerator=args.accelerator if args.accelerator else None,
         precision=args.precision if args.precision else 32,
         strategy=args.strategy if not args.strategy else None,
         devices=args.devices if not args.devices else None,
     )
-    if return_trainer_only:
-        return trainer
-    else:
-        return checkpoint_callback, trainer
+    return trainer
+
+
+def get_tester(args: NLUTesterArguments):
+    trainer = Trainer(
+        fast_dev_run=True,
+        accelerator=args.accelerator if args.accelerator else None,
+        precision=args.precision if args.precision else 32,
+        strategy=args.strategy if not args.strategy else None,
+        devices=args.devices if not args.devices else None,
+    )
+    return trainer
```

### Comparing `chrislab-0.5.0a1/src/ratsnlp/nlpbook/utils.py` & `chrislab-0.5.1/src/nlpbook/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             "fname": "klue_nli_train.json",
         },
         "val": {
             "googledrive_file_id": "1UKIDAFOFuDSah7A66FZXSA8XUWUHhBAd",
             "fname": "klue_nli_dev.json",
         }
     },
-    "ner": {
+    "kmou-ner": {
         "train": {
             "googledrive_file_id": "1RP764owqs1kZeHcjFnCX7zXt2EcjGY1i",
             "fname": "train.txt",
         },
         "val": {
             "googledrive_file_id": "1bEPNWT5952rD3xjg0LfJBy3hLHry3yUL",
             "fname": "val.txt",
```

