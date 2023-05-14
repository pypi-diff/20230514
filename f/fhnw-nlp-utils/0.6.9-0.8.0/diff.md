# Comparing `tmp/fhnw_nlp_utils-0.6.9-py3-none-any.whl.zip` & `tmp/fhnw_nlp_utils-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 23956 bytes, number of entries: 18
+Zip file size: 24269 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-18 07:56 fhnw/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-18 07:56 fhnw/nlp/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-18 08:10 fhnw/nlp/utils/__init__.py
 -rw-r--r--  2.0 unx      144 b- defN 21-Sep-18 08:10 fhnw/nlp/utils/colab.py
--rw-r--r--  2.0 unx     2249 b- defN 23-May-07 16:48 fhnw/nlp/utils/defaults.py
--rw-r--r--  2.0 unx     6890 b- defN 23-May-07 16:47 fhnw/nlp/utils/normalize.py
+-rw-r--r--  2.0 unx     2254 b- defN 23-May-08 04:31 fhnw/nlp/utils/defaults.py
+-rw-r--r--  2.0 unx     6987 b- defN 23-May-08 04:39 fhnw/nlp/utils/normalize.py
 -rw-r--r--  2.0 unx    37887 b- defN 23-Mar-12 20:31 fhnw/nlp/utils/params.py
 -rw-r--r--  2.0 unx     9537 b- defN 22-Dec-12 20:18 fhnw/nlp/utils/ploting.py
--rw-r--r--  2.0 unx     2262 b- defN 22-Aug-25 17:41 fhnw/nlp/utils/preprocess.py
+-rw-r--r--  2.0 unx     2262 b- defN 23-May-08 04:38 fhnw/nlp/utils/preprocess.py
 -rw-r--r--  2.0 unx    10048 b- defN 21-Nov-14 18:34 fhnw/nlp/utils/processing.py
 -rw-r--r--  2.0 unx     6838 b- defN 21-Nov-03 20:09 fhnw/nlp/utils/storage.py
--rw-r--r--  2.0 unx     3346 b- defN 22-Oct-05 05:11 fhnw/nlp/utils/system.py
+-rw-r--r--  2.0 unx     4124 b- defN 23-May-10 05:18 fhnw/nlp/utils/system.py
 -rw-r--r--  2.0 unx     3212 b- defN 22-Aug-10 15:41 fhnw/nlp/utils/text.py
 -rw-r--r--  2.0 unx     7656 b- defN 23-Apr-19 05:05 fhnw/nlp/utils/transformers.py
--rw-r--r--  2.0 unx     1298 b- defN 23-May-07 16:49 fhnw_nlp_utils-0.6.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-07 16:49 fhnw_nlp_utils-0.6.9.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-07 16:49 fhnw_nlp_utils-0.6.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1459 b- defN 23-May-07 16:49 fhnw_nlp_utils-0.6.9.dist-info/RECORD
-18 files, 92923 bytes uncompressed, 21566 bytes compressed:  76.8%
+-rw-r--r--  2.0 unx     1298 b- defN 23-May-14 17:40 fhnw_nlp_utils-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-14 17:40 fhnw_nlp_utils-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-14 17:40 fhnw_nlp_utils-0.8.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1459 b- defN 23-May-14 17:40 fhnw_nlp_utils-0.8.0.dist-info/RECORD
+18 files, 93803 bytes uncompressed, 21879 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: fhnw/nlp/utils/text.py
 Comment: 
 
 Filename: fhnw/nlp/utils/transformers.py
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.9.dist-info/METADATA
+Filename: fhnw_nlp_utils-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.9.dist-info/WHEEL
+Filename: fhnw_nlp_utils-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.9.dist-info/top_level.txt
+Filename: fhnw_nlp_utils-0.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fhnw_nlp_utils-0.6.9.dist-info/RECORD
+Filename: fhnw_nlp_utils-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fhnw/nlp/utils/defaults.py

```diff
@@ -29,15 +29,15 @@
                 try:
                     nltk.data.find('tokenizers/punkt')
                 except LookupError:
                     nltk.download('punkt')
 
                 __nlp_utils_defaults.stemmer = SnowballStemmer("german")
                 
-    return __nlp_utils_defaults.stemmer
+    return __nlp_utils_defaults.stemmer.stem
 
 
 def default_tokenizer():
     """Initialization of default tokenizer
     
     Returns
     -------
```

## fhnw/nlp/utils/normalize.py

```diff
@@ -40,42 +40,46 @@
 
     Parameters
     ----------
     text : str, iterable
         The text either as string or iterable of tokens (in this case tokenization is not applied)
     stopwords : set
         A set of stopword to remove from the tokens
-    stemmer: nltk stemmer
-        The stemmer to use (e.g. SnowballStemmer)
+    stemmer: callable
+        The stemmer to use (callable e.g. SnowballStemmer)
     word_splitter: splitter
         The word splitter to use (callable e.g. compound_split to split compound words) or None to disable word splitting
         
     Returns
     -------
     list
         The tokenized and stemmed text
     """
+    from typing import Callable
     from fhnw.nlp.utils.processing import is_iterable
         
     if isinstance(text, str):
         from fhnw.nlp.utils.defaults import default_tokenizer
         word_tokens = default_tokenizer()(text)
     elif is_iterable(text):
         word_tokens = text
     else:
         raise TypeError("Only string or iterable (e.g. list) is supported. Received a "+ str(type(text)))
 
+    if not isinstance(stemmer, Callable):
+        stemmer = stemmer.stem 
+
     if word_splitter is not None:
         # with python 3.8
-        #return [stemmer.stem(lower) for word in word_tokens if word.lower() not in stopwords for split in word_splitter(word) if (lower := split.lower()) not in stopwords]
-        return [stemmer.stem(split.lower()) for word in word_tokens if word.lower() not in stopwords for split in word_splitter(word) if split.lower() not in stopwords]
+        #return [stemmer(lower) for word in word_tokens if word.lower() not in stopwords for split in word_splitter(word) if (lower := split.lower()) not in stopwords]
+        return [stemmer(split.lower()) for word in word_tokens if word.lower() not in stopwords for split in word_splitter(word) if split.lower() not in stopwords]
     else:
         # with python 3.8
-        #return [stemmer.stem(lower) for word in word_tokens if (lower := word.lower()) not in stopwords]
-        return [stemmer.stem(word.lower()) for word in word_tokens if word.lower() not in stopwords]
+        #return [stemmer(lower) for word in word_tokens if (lower := word.lower()) not in stopwords]
+        return [stemmer(word.lower()) for word in word_tokens if word.lower() not in stopwords]
 
 
 def tokenize_lemma(text, stopwords, lemmanizer, keep_ners=False):
     """Tokenizes, lowercases and lemmatizes a text and removes stopwords
 
     Parameters
     ----------
@@ -143,16 +147,16 @@
     ----------
     text : str, iterable
         The text either as string or iterable of tokens (in this case tokenization is not applied)
     stopwords : set
         A set of stopword to remove from the tokens
     word_splitter: callable
         The word splitter to use (callable e.g. compound_split to split compound words) or None to disable word splitting
-    stemmer: nltk stemmer
-        The stemmer to use (e.g. SnowballStemmer) or None to disable stemming
+    stemmer: callable
+        The stemmer to use (callable e.g. SnowballStemmer) or None to disable stemming
     lemmanizer: spacy nlp pipeline
         The lemmanizer to use (must be spacy nlp pipeline) or None to disable lemmantization
     lemma_with_ner: bool
         Defines if named entities (NERs) should be keept in one token
         
     Returns
     -------
```

## fhnw/nlp/utils/system.py

```diff
@@ -123,7 +123,37 @@
     except ImportError as e:
         pass
     except Exception as e:
     	print("Error in 'igpu':", e)
     	pass
     
     return s
+    
+    
+def set_log_level(level = 1):
+    """Sets the log level of python/tensorflow
+
+    Parameters
+    ----------
+    level : int
+        The log level (0 -> NOTSET, 1 -> WARNING, 2 -> ERROR, 3 -> CRITICAL
+    version : str
+        A specific version number
+    """
+    
+    import logging
+    import os
+
+    tf_level = logging.WARN
+    if level == 0:
+        tf_level =  logging.NOTSET
+    elif level == 1:
+        tf_level = logging.WARNING
+    elif level == 2:
+        tf_level = logging.ERROR
+    else:
+        tf_level = logging.CRITICAL
+    
+    # see https://stackoverflow.com/a/42121886
+    os.environ["TF_CPP_MIN_LOG_LEVEL"] = str(level)
+    # see https://docs.python.org/3/library/logging.html#logging-levels
+    logging.getLogger("tensorflow").setLevel(tf_level)
```

## Comparing `fhnw_nlp_utils-0.6.9.dist-info/METADATA` & `fhnw_nlp_utils-0.8.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhnw-nlp-utils
-Version: 0.6.9
+Version: 0.8.0
 Summary: Utilities for NLP courses taught at FHNW.
 Home-page: http://github.com/markif/fhnw-nlp-utils
 Author: Fabian
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
```

## Comparing `fhnw_nlp_utils-0.6.9.dist-info/RECORD` & `fhnw_nlp_utils-0.8.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 fhnw/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fhnw/nlp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fhnw/nlp/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fhnw/nlp/utils/colab.py,sha256=5XiWtCz9R_MTtGC76BJgCNhdJPp2eGNYinv5C5NAK4A,144
-fhnw/nlp/utils/defaults.py,sha256=pMTKPCXYmZqHTIKW6hhPJ9Q-pW8xLjHPGcUaZZPe5zk,2249
-fhnw/nlp/utils/normalize.py,sha256=UeYJUCv31ezsTmgazw_v1Edn_sqI_YE_cFZ9EjiDKR8,6890
+fhnw/nlp/utils/defaults.py,sha256=H6IpvtUWZ2GLFyQkFBGO-gcbYhTzzLdZd772ecg5_nk,2254
+fhnw/nlp/utils/normalize.py,sha256=ymAlh3WJm2ptVeCiSd58DsmKca-JtgMRHGfa6QR76cw,6987
 fhnw/nlp/utils/params.py,sha256=xavHoG_CMmygKGp3lwHqPbZUpfnrjdLjZPII2fiZPjE,37887
 fhnw/nlp/utils/ploting.py,sha256=8ya50BauVgWfRh7X7V9urU5SCvd7RSF7INhCgKHdzzc,9537
 fhnw/nlp/utils/preprocess.py,sha256=FDy6HAYS3OjKue9kVigh7Cg84gc3rju5Zu0WuOLVoq0,2262
 fhnw/nlp/utils/processing.py,sha256=73R2Vy4tMzXpbjSbck7xZFDigaA3cjuLxbe-ZXxs_uc,10048
 fhnw/nlp/utils/storage.py,sha256=F3C19qp9x2cGHnE0mdLVQxLLqBzgtFUCWZSGtzmk_yw,6838
-fhnw/nlp/utils/system.py,sha256=yRphzlhw34C8qyl-sgUSbz56_Ckr8G-tsRJkko-pv-U,3346
+fhnw/nlp/utils/system.py,sha256=K89rjO5-55g0nYHWlyj0KHAIGo4TWV6__xiH9C6Ouxk,4124
 fhnw/nlp/utils/text.py,sha256=ElaWYdl_7YkHc_IHJyEUZPvKgcADTcbEBEL1FO5emME,3212
 fhnw/nlp/utils/transformers.py,sha256=Jge66cuppFN3llTo38FSKvjuuqbHtAZXnfgeGj6qWe4,7656
-fhnw_nlp_utils-0.6.9.dist-info/METADATA,sha256=bY5ZL3-bW7Wid-R3h8ymxxg33HsFCKnR2brwk_9tB0Q,1298
-fhnw_nlp_utils-0.6.9.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
-fhnw_nlp_utils-0.6.9.dist-info/top_level.txt,sha256=G3JGQX_1iq_fMxU1-sbRHKR8vesyWdKRcLPkdbd66MA,5
-fhnw_nlp_utils-0.6.9.dist-info/RECORD,,
+fhnw_nlp_utils-0.8.0.dist-info/METADATA,sha256=Jp-UTzdnkLNJa72Umv5UMQcNz0QaS6B3qjN_88s-Hoc,1298
+fhnw_nlp_utils-0.8.0.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
+fhnw_nlp_utils-0.8.0.dist-info/top_level.txt,sha256=G3JGQX_1iq_fMxU1-sbRHKR8vesyWdKRcLPkdbd66MA,5
+fhnw_nlp_utils-0.8.0.dist-info/RECORD,,
```

