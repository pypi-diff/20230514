# Comparing `tmp/embedders-0.0.8-py2.py3-none-any.whl.zip` & `tmp/embedders-0.0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 20411 bytes, number of entries: 17
--rw-r--r--  2.0 unx     5753 b- defN 22-May-06 12:23 embedders/__init__.py
+Zip file size: 20538 bytes, number of entries: 17
+-rw-r--r--  2.0 unx     5782 b- defN 22-May-16 08:25 embedders/__init__.py
 -rw-r--r--  2.0 unx      399 b- defN 22-May-05 14:04 embedders/util.py
 -rw-r--r--  2.0 unx      151 b- defN 22-May-05 14:04 embedders/classification/__init__.py
--rw-r--r--  2.0 unx     1034 b- defN 22-May-05 14:04 embedders/classification/contextual.py
+-rw-r--r--  2.0 unx     1168 b- defN 22-May-16 08:38 embedders/classification/contextual.py
 -rw-r--r--  2.0 unx     3285 b- defN 22-May-05 14:04 embedders/classification/count_based.py
 -rw-r--r--  2.0 unx     2176 b- defN 22-May-05 14:04 embedders/classification/reduce.py
 -rw-r--r--  2.0 unx      634 b- defN 22-May-05 14:04 embedders/extraction/__init__.py
--rw-r--r--  2.0 unx     5570 b- defN 22-May-05 14:04 embedders/extraction/contextual.py
+-rw-r--r--  2.0 unx     5786 b- defN 22-May-16 08:32 embedders/extraction/contextual.py
 -rw-r--r--  2.0 unx     1784 b- defN 22-May-05 14:04 embedders/extraction/count_based.py
 -rw-r--r--  2.0 unx     2711 b- defN 22-May-05 14:04 embedders/extraction/reduce.py
 -rw-r--r--  2.0 unx        0 b- defN 22-May-05 14:04 embedders/samples/__init__.py
 -rw-r--r--  2.0 unx     6158 b- defN 22-May-05 14:04 embedders/samples/clickbait.py
--rw-r--r--  2.0 unx    11340 b- defN 22-May-06 12:24 embedders-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     8849 b- defN 22-May-06 12:24 embedders-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-May-06 12:24 embedders-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 22-May-06 12:24 embedders-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1451 b- defN 22-May-06 12:24 embedders-0.0.8.dist-info/RECORD
-17 files, 51415 bytes uncompressed, 18009 bytes compressed:  65.0%
+-rw-r--r--  2.0 unx    11340 b- defN 22-May-16 08:38 embedders-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8811 b- defN 22-May-16 08:38 embedders-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 22-May-16 08:38 embedders-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 22-May-16 08:38 embedders-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1451 b- defN 22-May-16 08:38 embedders-0.0.9.dist-info/RECORD
+17 files, 51756 bytes uncompressed, 18136 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: embedders/samples/__init__.py
 Comment: 
 
 Filename: embedders/samples/clickbait.py
 Comment: 
 
-Filename: embedders-0.0.8.dist-info/LICENSE
+Filename: embedders-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: embedders-0.0.8.dist-info/METADATA
+Filename: embedders-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: embedders-0.0.8.dist-info/WHEEL
+Filename: embedders-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: embedders-0.0.8.dist-info/top_level.txt
+Filename: embedders-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: embedders-0.0.8.dist-info/RECORD
+Filename: embedders-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## embedders/__init__.py

```diff
@@ -53,15 +53,15 @@
         if as_generator:
             return self._encode(documents, fit_model)
         else:
             embeddings = []
             if show_progress:
                 num_batches = util.num_batches(documents, self.batch_size)
                 print("Initializing model, might take some time...")
-                for embedding_batch in tqdm(self._encode(documents, fit_model), total=num_batches):
+                for embedding_batch in tqdm(self._encode(documents, fit_model), total=num_batches, desc="Encoding batches ..."):
                     embeddings.extend(embedding_batch)
             else:
                 for embedding_batch in self._encode(documents, fit_model):
                     embeddings.extend(embedding_batch)
             return embeddings
 
     def fit_transform(
```

## embedders/classification/contextual.py

```diff
@@ -1,25 +1,29 @@
 from typing import List, Union, Generator
 from sentence_transformers import SentenceTransformer
 from embedders import util
 from embedders.classification import SentenceEmbedder
 from spacy.tokens.doc import Doc
+import torch
 
 
 class TransformerSentenceEmbedder(SentenceEmbedder):
     """Embeds documents using large, pre-trained transformers from https://huggingface.co
 
     Args:
         config_string (str): Name of the model listed on https://huggingface.co/models
         batch_size (int, optional): Defines the number of conversions after which the embedder yields. Defaults to 128.
     """
 
     def __init__(self, config_string: str, batch_size: int = 128):
 
         super().__init__(batch_size)
-        self.model = SentenceTransformer(config_string)
+        self.device = torch.device(
+            'cuda' if torch.cuda.is_available() else 'cpu'
+        )
+        self.model = SentenceTransformer(config_string).to(self.device)
 
     def _encode(
         self, documents: List[Union[str, Doc]], fit_model: bool
     ) -> Generator[List[List[float]], None, None]:
         for documents_batch in util.batch(documents, self.batch_size):
             yield self.model.encode(documents_batch, show_progress_bar=False).tolist()
```

## embedders/extraction/contextual.py

```diff
@@ -42,15 +42,16 @@
                 vocabulary.append([tok.text for tok in doc])
             if fit_model:
                 self.model = word2vec.Word2Vec(vocabulary, min_count=1)
 
         for documents_batch in util.batch(documents, self.batch_size):
             documents_batch_embedded = []
             for doc in documents_batch:
-                documents_batch_embedded.append([lookup_w2v(tok.text) for tok in doc])
+                documents_batch_embedded.append(
+                    [lookup_w2v(tok.text) for tok in doc])
             yield documents_batch_embedded
 
 
 class TransformerTokenEmbedder(TokenEmbedder):
     """Embeds documents using large, pre-trained transformers from https://huggingface.co
 
     Args:
@@ -64,16 +65,23 @@
         self,
         config_string: str,
         language_code: str,
         precomputed_docs: bool = False,
         batch_size: int = 128,
     ):
         super().__init__(language_code, precomputed_docs, batch_size)
-        self.transformer_tokenizer = AutoTokenizer.from_pretrained(config_string)
-        self.model = AutoModel.from_pretrained(config_string, output_hidden_states=True)
+        self.device = torch.device(
+            'cuda' if torch.cuda.is_available() else 'cpu'
+        )
+        self.transformer_tokenizer = AutoTokenizer.from_pretrained(
+            config_string
+        )
+        self.model = AutoModel.from_pretrained(
+            config_string, output_hidden_states=True
+        ).to(self.device)
 
     def _encode(
         self, documents: Union[List[str], List[Doc]], fit_model: bool
     ) -> Generator[List[List[List[float]]], None, None]:
         for documents_batch in util.batch(documents, self.batch_size):
             documents_batch_embedded = []
             for doc in documents_batch:
@@ -102,15 +110,16 @@
         for key, values in embeddings.items():
             embeddings[key] = np.array(values).mean(0).tolist()
         return list(embeddings.values())
 
     def _get_char_level_embeddings(
         self, document: str
     ) -> List[List[Tuple[int, int, List[List[float]]]]]:
-        encoded = self.transformer_tokenizer.encode_plus(document, return_tensors="pt")
+        encoded = self.transformer_tokenizer.encode_plus(
+            document, return_tensors="pt")
         tokens = encoded.encodings[0]
         num_tokens = len(
             set(tokens.words[1:-1])
         )  # 1 and -1 are [CLS] tokens, and other tokens can be ##subwords
         with torch.no_grad():
             output = self.model(**encoded)
 
@@ -120,14 +129,15 @@
         layers = [-4, -3, -2, -1]
         output = torch.stack([states[i] for i in layers]).sum(0).squeeze()
 
         token_embeddings = []
 
         for token_idx in range(num_tokens):
             index_begin, index_end = tokens.word_to_chars(token_idx)
-            token_ids_word = np.where(np.array(encoded.word_ids()) == token_idx)
+            token_ids_word = np.where(
+                np.array(encoded.word_ids()) == token_idx)
             # Only select the tokens that constitute the requested word
             word_tokens_output = output[token_ids_word]
             token_embeddings.append(
                 [index_begin, index_end, word_tokens_output.tolist()]
             )
         return token_embeddings
```

## Comparing `embedders-0.0.8.dist-info/LICENSE` & `embedders-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `embedders-0.0.8.dist-info/METADATA` & `embedders-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedders
-Version: 0.0.8
+Version: 0.0.9
 Summary: High-level API for creating sentence and token embeddings
 Home-page: https://github.com/code-kern-ai/embedders
 Author: Johannes Hötter
 Author-email: johannes.hoetter@kern.ai
 License: UNKNOWN
 Keywords: kern,machine learning,representation learning,python
 Platform: UNKNOWN
@@ -50,15 +50,14 @@
 Requires-Dist: spacy-legacy (==3.0.9)
 Requires-Dist: spacy-loggers (==1.0.2)
 Requires-Dist: srsly (==2.4.3)
 Requires-Dist: thinc (==8.0.15)
 Requires-Dist: threadpoolctl (==3.1.0)
 Requires-Dist: tokenizers (==0.12.1)
 Requires-Dist: torch (==1.11.0)
-Requires-Dist: torchvision (==0.12.0)
 Requires-Dist: tqdm (==4.64.0)
 Requires-Dist: transformers (==4.18.0)
 Requires-Dist: typer (==0.4.1)
 Requires-Dist: typing-extensions (==4.2.0)
 Requires-Dist: urllib3 (==1.26.9)
 Requires-Dist: wasabi (==0.9.1)
 
@@ -156,15 +155,15 @@
 | embedders.extraction.reduce     | PCATokenEmbedder    | Wraps embedder into a principial component analysis to reduce the dimensionality |
 
 ## Pre-trained embedders
 With growing availability of large, pre-trained models such as provided by [🤗 Hugging Face](https://huggingface.co/), embedding complex sentences in a wide variety of languages and domains becomes much more applicable. If you want to make use of transformer models, you can just use the configuration string of the respective model, which will automatically pull the correct model for the [🤗 Hugging Face Hub](https://huggingface.co/models).
 
 ## Roadmap
 - [x] Add extensive documentation to existing embedders
-- [ ] Add sample projects
+- [x] Add sample projects
 - [ ] Add test cases
 - [ ] Add further text feature-based sentence and word embedders
 - [ ] Add pre-trained word2vec embeddings
 
 If you want to have something added, feel free to open an [issue](https://github.com/code-kern-ai/embedders/issues).
 
 ## Contributing
```

## Comparing `embedders-0.0.8.dist-info/RECORD` & `embedders-0.0.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-embedders/__init__.py,sha256=ydr4wjI2wAcmPoVd2GTzMcnEJJQPWdnEJPMLvb5ZSog,5753
+embedders/__init__.py,sha256=zmWDBOmBdHpg3-3wr4wdSdE6ZL1S35TGd7gZap6aC6g,5782
 embedders/util.py,sha256=XnpCyf5U0z7EWmgOQJ46v1diI6JXsYGYFBI2c_-nycc,399
 embedders/classification/__init__.py,sha256=ewZiEukpAOgMLKU-JTdPhHrPVJFLQUKzZAco7cC1ihw,151
-embedders/classification/contextual.py,sha256=-GZNMr_GViWT0hjfON7y-NikzWShiduOgDY_lybiQLM,1034
+embedders/classification/contextual.py,sha256=P1rpUfpt9A1HamoMRu7BLcQpdIF5C76Z7gFlVQ6gvW0,1168
 embedders/classification/count_based.py,sha256=uaGTdwljsA1cXlYWhtFQhuAGUtct12j3qnXh-mfIq9k,3285
 embedders/classification/reduce.py,sha256=4v1dmFTg_337rRnormjwBShIjF-qO_8e2TGFvzsKYFw,2176
 embedders/extraction/__init__.py,sha256=q40GJDzPIov-Za_wu7uzuO6YMJQ14iEJT9T3PMkic4o,634
-embedders/extraction/contextual.py,sha256=TMocO04_oghJmCZWNbdRZibub1lUUkMcq0_ztuuz8Y8,5570
+embedders/extraction/contextual.py,sha256=hOSLX99x6t6V8jelfCPy_cm9y0hfpoNM8Ug1b1TPzNg,5786
 embedders/extraction/count_based.py,sha256=uwhg2r3D-My3faMv81OHCDkbQyjTWv3Uomft6BsxKik,1784
 embedders/extraction/reduce.py,sha256=czQkO2GtrzJbLd4RSnjr7V8AS9M89BumDw3QCxwGFKw,2711
 embedders/samples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 embedders/samples/clickbait.py,sha256=IiivTTmb3zIUaurod3L0ADruCQuXtHGXsU4fW4IrFQc,6158
-embedders-0.0.8.dist-info/LICENSE,sha256=JYWPdm7R90tTEXK6muMxOgQBHToBQaLT9rPehcITO4I,11340
-embedders-0.0.8.dist-info/METADATA,sha256=1n92boVW03VWHw272F7tInSPBlXd7gbk7imYwaIzIAA,8849
-embedders-0.0.8.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-embedders-0.0.8.dist-info/top_level.txt,sha256=iRhfbBg_ZWmtclxcpD-WZe5rD-rvHFHKGkJwcWZM_f0,10
-embedders-0.0.8.dist-info/RECORD,,
+embedders-0.0.9.dist-info/LICENSE,sha256=JYWPdm7R90tTEXK6muMxOgQBHToBQaLT9rPehcITO4I,11340
+embedders-0.0.9.dist-info/METADATA,sha256=as9Qcitw3kooTsHazW-3b9rpCa3ggsuC0a7xFhNA7dw,8811
+embedders-0.0.9.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+embedders-0.0.9.dist-info/top_level.txt,sha256=iRhfbBg_ZWmtclxcpD-WZe5rD-rvHFHKGkJwcWZM_f0,10
+embedders-0.0.9.dist-info/RECORD,,
```

