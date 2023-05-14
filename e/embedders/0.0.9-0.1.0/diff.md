# Comparing `tmp/embedders-0.0.9-py2.py3-none-any.whl.zip` & `tmp/embedders-0.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 20538 bytes, number of entries: 17
--rw-r--r--  2.0 unx     5782 b- defN 22-May-16 08:25 embedders/__init__.py
--rw-r--r--  2.0 unx      399 b- defN 22-May-05 14:04 embedders/util.py
--rw-r--r--  2.0 unx      151 b- defN 22-May-05 14:04 embedders/classification/__init__.py
--rw-r--r--  2.0 unx     1168 b- defN 22-May-16 08:38 embedders/classification/contextual.py
--rw-r--r--  2.0 unx     3285 b- defN 22-May-05 14:04 embedders/classification/count_based.py
--rw-r--r--  2.0 unx     2176 b- defN 22-May-05 14:04 embedders/classification/reduce.py
--rw-r--r--  2.0 unx      634 b- defN 22-May-05 14:04 embedders/extraction/__init__.py
--rw-r--r--  2.0 unx     5786 b- defN 22-May-16 08:32 embedders/extraction/contextual.py
--rw-r--r--  2.0 unx     1784 b- defN 22-May-05 14:04 embedders/extraction/count_based.py
--rw-r--r--  2.0 unx     2711 b- defN 22-May-05 14:04 embedders/extraction/reduce.py
--rw-r--r--  2.0 unx        0 b- defN 22-May-05 14:04 embedders/samples/__init__.py
--rw-r--r--  2.0 unx     6158 b- defN 22-May-05 14:04 embedders/samples/clickbait.py
--rw-r--r--  2.0 unx    11340 b- defN 22-May-16 08:38 embedders-0.0.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     8811 b- defN 22-May-16 08:38 embedders-0.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-May-16 08:38 embedders-0.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 22-May-16 08:38 embedders-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1451 b- defN 22-May-16 08:38 embedders-0.0.9.dist-info/RECORD
-17 files, 51756 bytes uncompressed, 18136 bytes compressed:  65.0%
+Zip file size: 23223 bytes, number of entries: 18
+-rw-r--r--  2.0 unx     6934 b- defN 22-Oct-30 14:35 embedders/__init__.py
+-rw-r--r--  2.0 unx      143 b- defN 22-Sep-07 08:19 embedders/enums.py
+-rw-r--r--  2.0 unx      399 b- defN 22-Jul-22 10:51 embedders/util.py
+-rw-r--r--  2.0 unx      178 b- defN 22-Sep-07 08:19 embedders/classification/__init__.py
+-rw-r--r--  2.0 unx     2853 b- defN 23-May-14 10:24 embedders/classification/contextual.py
+-rw-r--r--  2.0 unx     3285 b- defN 22-Jul-22 10:51 embedders/classification/count_based.py
+-rw-r--r--  2.0 unx     2170 b- defN 22-Jul-22 10:51 embedders/classification/reduce.py
+-rw-r--r--  2.0 unx      670 b- defN 22-Sep-07 08:19 embedders/extraction/__init__.py
+-rw-r--r--  2.0 unx    14751 b- defN 22-Oct-22 16:42 embedders/extraction/contextual.py
+-rw-r--r--  2.0 unx     1784 b- defN 22-Jul-22 10:51 embedders/extraction/count_based.py
+-rw-r--r--  2.0 unx     2705 b- defN 22-Jul-22 10:51 embedders/extraction/reduce.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jul-22 10:51 embedders/samples/__init__.py
+-rw-r--r--  2.0 unx     6158 b- defN 22-Jul-22 10:51 embedders/samples/clickbait.py
+-rw-r--r--  2.0 unx    11340 b- defN 23-May-14 10:25 embedders-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7012 b- defN 23-May-14 10:25 embedders-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-14 10:25 embedders-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-14 10:25 embedders-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1526 b- defN 23-May-14 10:25 embedders-0.1.0.dist-info/RECORD
+18 files, 62028 bytes uncompressed, 20709 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: embedders/__init__.py
 Comment: 
 
+Filename: embedders/enums.py
+Comment: 
+
 Filename: embedders/util.py
 Comment: 
 
 Filename: embedders/classification/__init__.py
 Comment: 
 
 Filename: embedders/classification/contextual.py
@@ -30,23 +33,23 @@
 
 Filename: embedders/samples/__init__.py
 Comment: 
 
 Filename: embedders/samples/clickbait.py
 Comment: 
 
-Filename: embedders-0.0.9.dist-info/LICENSE
+Filename: embedders-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: embedders-0.0.9.dist-info/METADATA
+Filename: embedders-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: embedders-0.0.9.dist-info/WHEEL
+Filename: embedders-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: embedders-0.0.9.dist-info/top_level.txt
+Filename: embedders-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: embedders-0.0.9.dist-info/RECORD
+Filename: embedders-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## embedders/__init__.py

```diff
@@ -1,16 +1,20 @@
-from abc import ABC, abstractmethod
-from typing import List, Generator, Optional, Union
+from abc import ABCMeta, abstractmethod
+from typing import Dict, List, Generator, Optional, Union
 from spacy.tokens.doc import Doc
 from sklearn.decomposition import PCA
 from tqdm import tqdm
 from embedders import util
+from joblib import dump, load
 
 
-class Transformer(ABC):
+class Transformer(metaclass=ABCMeta):
+    def __init__(self):
+        self._warnings = {}
+
     @abstractmethod
     def fit_transform(
         self, documents: List[Union[str, Doc]], as_generator: bool
     ) -> Union[List, Generator]:
         """Trains the given algorithm to embed textual documents into semantic vector-spacy representations.
 
         Args:
@@ -33,35 +37,51 @@
             as_generator (bool): Embeddings are calculated batch-wise. If this is set to False, the results will be summarized in one list, else a generator will yield the values.
 
         Returns:
             Union[List, Generator]: List with all embeddings or generator that yields the embeddings.
         """
         pass
 
-
-class Embedder(Transformer):
     @abstractmethod
-    def __init__(self):
+    def get_warnings(self) -> Dict:
+        """Collects all warnings reported during the embedding creation or PCA.
+
+        Returns:
+            List: List with all warnings
+        """
         pass
 
+
+class Embedder(Transformer, metaclass=ABCMeta):
+    def __init__(self):
+        super().__init__()
+
     @abstractmethod
     def _encode(self, documents: List[Union[str, Doc]], fit_model: bool) -> Generator:
         pass
 
     def _encode_batch(
-        self, documents: List[Union[str, Doc]], as_generator: bool, fit_model: bool, show_progress: Optional[bool] = True
+        self,
+        documents: List[Union[str, Doc]],
+        as_generator: bool,
+        fit_model: bool,
+        show_progress: Optional[bool] = True,
     ) -> Union[List, Generator]:
         if as_generator:
             return self._encode(documents, fit_model)
         else:
             embeddings = []
             if show_progress:
                 num_batches = util.num_batches(documents, self.batch_size)
                 print("Initializing model, might take some time...")
-                for embedding_batch in tqdm(self._encode(documents, fit_model), total=num_batches, desc="Encoding batches ..."):
+                for embedding_batch in tqdm(
+                    self._encode(documents, fit_model),
+                    total=num_batches,
+                    desc="Encoding batches ...",
+                ):
                     embeddings.extend(embedding_batch)
             else:
                 for embedding_batch in self._encode(documents, fit_model):
                     embeddings.extend(embedding_batch)
             return embeddings
 
     def fit_transform(
@@ -70,16 +90,19 @@
         return self._encode_batch(documents, as_generator, True)
 
     def transform(
         self, documents: List[Union[str, Doc]], as_generator: bool = False
     ) -> Union[List, Generator]:
         return self._encode_batch(documents, as_generator, False)
 
+    def get_warnings(self) -> Dict:
+        return self._warnings
+
 
-class PCAReducer(Transformer):
+class PCAReducer(Transformer, metaclass=ABCMeta):
     """Wraps embedder into a principial component analysis to reduce the dimensionality.
 
     Args:
         embedder (Embedder): Algorithm to embed the documents.
         n_components (int, optional): Number of principal components to keep. Defaults to 8.
         autocorrect_n_components (bool, optional): If there are less data samples than specified components, this will automatically reduce the number of principial components. Defaults to True.
     """
@@ -87,19 +110,36 @@
     def __init__(
         self,
         embedder: Embedder,
         n_components: int = 8,
         autocorrect_n_components: bool = True,
         **kwargs
     ):
+        super().__init__()
         self.embedder = embedder
         self.reducer = PCA(n_components=n_components, **kwargs)
         self.batch_size = self.embedder.batch_size
         self.autocorrect_n_components = autocorrect_n_components
 
+    def store_pca_weights(self, file_name: str):
+        """Stores the PCA weights to a file.
+
+        Args:
+            file_name (str): Path to the file without any file endings.
+        """
+        dump(self.reducer, f'{file_name}.joblib') 
+
+    def load_pca_weights(self, file_name: str):
+        """Loads the PCA weights from a file.
+
+        Args:
+            file_name (str): Path to the file without any file endings.
+        """
+        self.reducer = load(f'{file_name}.joblib')
+
     @abstractmethod
     def _reduce(
         self,
         documents: List[Union[str, Doc]],
         fit_model: bool,
         fit_after_n_batches: int,
     ):
@@ -143,8 +183,11 @@
             documents,
             as_generator,
             True,
             fit_after_n_batches,
         )
 
     def transform(self, documents, as_generator=False) -> Union[List, Generator]:
-        return self._reduce_batch(documents, as_generator, False, False, 0)
+        return self._reduce_batch(documents, as_generator, False, 0)
+
+    def get_warnings(self) -> Dict:
+        return {**self._warnings, **self.embedder.get_warnings()}
```

## embedders/classification/__init__.py

```diff
@@ -1,6 +1,7 @@
 from embedders import Embedder
 
 
 class SentenceEmbedder(Embedder):
     def __init__(self, batch_size: int = 128):
+        super().__init__()
         self.batch_size = batch_size
```

## embedders/classification/contextual.py

```diff
@@ -1,29 +1,67 @@
 from typing import List, Union, Generator
 from sentence_transformers import SentenceTransformer
 from embedders import util
 from embedders.classification import SentenceEmbedder
 from spacy.tokens.doc import Doc
 import torch
+import openai
+from openai import error as openai_error
+import cohere
 
 
-class TransformerSentenceEmbedder(SentenceEmbedder):
+class HuggingFaceSentenceEmbedder(SentenceEmbedder):
     """Embeds documents using large, pre-trained transformers from https://huggingface.co
 
     Args:
         config_string (str): Name of the model listed on https://huggingface.co/models
         batch_size (int, optional): Defines the number of conversions after which the embedder yields. Defaults to 128.
     """
 
     def __init__(self, config_string: str, batch_size: int = 128):
-
         super().__init__(batch_size)
-        self.device = torch.device(
-            'cuda' if torch.cuda.is_available() else 'cpu'
-        )
+        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.model = SentenceTransformer(config_string).to(self.device)
 
     def _encode(
         self, documents: List[Union[str, Doc]], fit_model: bool
     ) -> Generator[List[List[float]], None, None]:
         for documents_batch in util.batch(documents, self.batch_size):
             yield self.model.encode(documents_batch, show_progress_bar=False).tolist()
+
+
+class OpenAISentenceEmbedder(SentenceEmbedder):
+    def __init__(self, openai_api_key: str, model_name: str, batch_size: int = 128):
+        super().__init__(batch_size)
+        self.model_name = model_name
+        self.openai_api_key = openai_api_key
+        openai.api_key = self.openai_api_key
+
+    def _encode(
+        self, documents: List[Union[str, Doc]], fit_model: bool
+    ) -> Generator[List[List[float]], None, None]:
+        for documents_batch in util.batch(documents, self.batch_size):
+            documents_batch = [doc.replace("\n", " ") for doc in documents_batch]
+            try:
+                response = openai.Embedding.create(
+                    input=documents_batch, model=self.model_name
+                )
+                embeddings = [entry["embedding"] for entry in response["data"]]
+                yield embeddings
+            except openai_error.AuthenticationError:
+                raise Exception(
+                    "OpenAI API key is invalid. Please provide a valid API key in the constructor of OpenAISentenceEmbedder."
+                )
+
+
+class CohereSentenceEmbedder(SentenceEmbedder):
+    def __init__(self, cohere_api_key: str, batch_size: int = 128):
+        super().__init__(batch_size)
+        self.cohere_api_key = cohere_api_key
+        self.model = cohere.Client(self.cohere_api_key)
+
+    def _encode(
+        self, documents: List[Union[str, Doc]], fit_model: bool
+    ) -> Generator[List[List[float]], None, None]:
+        for documents_batch in util.batch(documents, self.batch_size):
+            embeddings = self.model.embed(documents_batch).embeddings
+            yield embeddings
```

## embedders/classification/reduce.py

```diff
@@ -17,15 +17,15 @@
         fit_after_n_batches: int,
     ) -> Generator[List[List[Union[float, int]]], None, None]:
         if fit_model:
             embeddings_training = []
             num_batches = util.num_batches(documents, self.embedder.batch_size)
             fit_after_n_batches = min(num_batches, fit_after_n_batches) - 1
             for batch_idx, batch in enumerate(
-                list(self.embedder.fit_transform(documents, as_generator=True))
+                self.embedder.fit_transform(documents, as_generator=True)
             ):
                 if batch_idx <= fit_after_n_batches:
                     embeddings_training.append(batch)
 
                 if batch_idx == fit_after_n_batches:
                     embeddings_training_flattened = []
                     for batch_training in embeddings_training:
```

## embedders/extraction/__init__.py

```diff
@@ -1,20 +1,23 @@
 import spacy
 from embedders import Embedder
 from spacy.tokens.doc import Doc
 from typing import Union
 
+
 class TokenEmbedder(Embedder):
-    def __init__(self, language_code: str, precomputed_docs:bool=False, batch_size:int=128):
+    def __init__(
+        self, language_code: str, precomputed_docs: bool = False, batch_size: int = 128
+    ):
+        super().__init__()
         self.preloaded = precomputed_docs
         if precomputed_docs:
             self.nlp = spacy.blank(language_code)
         else:
             self.nlp = spacy.load(language_code)
         self.batch_size = batch_size
 
     def _get_tokenized_document(self, document: Union[str, Doc]):
         if self.preloaded:
             return document
         else:
             return self.nlp(document)
-
```

## embedders/extraction/contextual.py

```diff
@@ -1,143 +1,349 @@
-from typing import List, Tuple, Union, Generator
+from typing import List, Tuple, Union, Iterator
 import torch
+import math
 import numpy as np
+import re
 from transformers import AutoTokenizer, AutoModel
 from collections import defaultdict
-from gensim.models import word2vec
 from embedders import util
 from spacy.tokens.doc import Doc
 
 
+from embedders.enums import WarningType
 from embedders.extraction import TokenEmbedder
 
 
-class SkipGramTokenEmbedder(TokenEmbedder):
-    """Embeds documents using a word2vec approach from gensim.
-
-    Args:
-        language_code (str): Name of the spaCy language model
-        precomputed_docs (bool, optional): If you have a large text corpus, it might make sense to precompute the data and input tokenized spaCy documents. Defaults to False.
-        batch_size (int, optional): Defines the number of conversions after which the embedder yields. Defaults to 128.
-    """
-
-    def __init__(
-        self, language_code: str, precomputed_docs: bool = False, batch_size: int = 128
-    ):
-        super().__init__(language_code, precomputed_docs, batch_size)
-        self.model = None
-
-    def _encode(
-        self, documents: Union[List[str], List[Doc]], fit_model: bool
-    ) -> Generator[List[List[List[float]]], None, None]:
-        def lookup_w2v(text: str) -> List[float]:
-            try:
-                return self.model.wv[text].tolist()
-            except KeyError:
-                return [0.0 for _ in range(self.model.vector_size)]
-
-        if not self.preloaded:
-            documents = [self.nlp(doc) for doc in documents]
-            vocabulary = []
-            for doc in documents:
-                vocabulary.append([tok.text for tok in doc])
-            if fit_model:
-                self.model = word2vec.Word2Vec(vocabulary, min_count=1)
-
-        for documents_batch in util.batch(documents, self.batch_size):
-            documents_batch_embedded = []
-            for doc in documents_batch:
-                documents_batch_embedded.append(
-                    [lookup_w2v(tok.text) for tok in doc])
-            yield documents_batch_embedded
-
-
 class TransformerTokenEmbedder(TokenEmbedder):
     """Embeds documents using large, pre-trained transformers from https://huggingface.co
 
     Args:
         config_string (str): Name of the model listed on https://huggingface.co/models
         language_code (str): Name of the spaCy language model
         precomputed_docs (bool, optional): If you have a large text corpus, it might make sense to precompute the data and input tokenized spaCy documents. Defaults to False.
         batch_size (int, optional): Defines the number of conversions after which the embedder yields. Defaults to 128.
     """
 
+    _NL_TOKEN = "[NL]"
+
     def __init__(
         self,
         config_string: str,
         language_code: str,
         precomputed_docs: bool = False,
         batch_size: int = 128,
     ):
         super().__init__(language_code, precomputed_docs, batch_size)
-        self.device = torch.device(
-            'cuda' if torch.cuda.is_available() else 'cpu'
-        )
-        self.transformer_tokenizer = AutoTokenizer.from_pretrained(
-            config_string
+        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
+        self.transformer_tokenizer = AutoTokenizer.from_pretrained(config_string)
+        self.transformer_tokenizer.add_special_tokens(
+            {"additional_special_tokens": [self._NL_TOKEN]}
         )
+
         self.model = AutoModel.from_pretrained(
             config_string, output_hidden_states=True
         ).to(self.device)
+        self.model.resize_token_embeddings(len(self.transformer_tokenizer))
 
     def _encode(
         self, documents: Union[List[str], List[Doc]], fit_model: bool
-    ) -> Generator[List[List[List[float]]], None, None]:
-        for documents_batch in util.batch(documents, self.batch_size):
+    ) -> Iterator[List[List[List[float]]]]:
+        for batch_number, documents_batch in enumerate(
+            util.batch(documents, self.batch_size)
+        ):
+            """
+            Computation of embeddings for each spacy token of each document. For the
+            embedding creation transformer models are used. Embeddings are calculated
+            for the transformer tokens of the document, then these token embeddings are
+            matched to the spacy tokens.
+
+            Args:
+                documents: list of strings or spacy documents
+                fit_model: not used, required by base class
+            Return:
+                Token embeddings for each document
+            """
+
             documents_batch_embedded = []
-            for doc in documents_batch:
-                char_level_embs = self._get_char_level_embeddings(str(doc))
-                doc = self._get_tokenized_document(doc)
-                document_embedded = self._get_token_embedding_from_char_embedding(
-                    char_level_embs, doc
+            for document_number, document in enumerate(documents_batch):
+                doc = self._get_tokenized_document(document)
+
+                # no spacy token.
+                # set special token as text, so that an embedding
+                # is created that can be processed by the PCA.
+                if len(doc) == 0:
+                    doc = self.nlp(self._NL_TOKEN)
+
+                # spacy creates tokens which only contain whitespace characters.
+                # the transformer tokenizer ignores these tokens.
+                # in order to avoid problems while matching the tokens the text is
+                # preprocessed.
+                text, prep_offsets = self._preprocess_doc_text(doc)
+
+                # transformer models have a maximum number of tokens which can be
+                # processed at the same time.
+                # in this case the text is splitted in mutliple subparts
+                number_est_tokens = self._estimate_token_number(text)
+                idx_document = batch_number * self.batch_size + document_number
+                if self.model.config.max_position_embeddings < number_est_tokens:
+                    if WarningType.DOCUMENT_IS_SPLITTED.value in self._warnings:
+                        self._warnings[WarningType.DOCUMENT_IS_SPLITTED.value].append(
+                            idx_document
+                        )
+                    else:
+                        self._warnings[WarningType.DOCUMENT_IS_SPLITTED.value] = [
+                            idx_document
+                        ]
+
+                    transformer_embs = []
+                    for doc_part, index_offset in self._split_document(
+                        text, number_est_tokens
+                    ):
+                        transformer_embs.extend(
+                            self._get_transformer_embeddings(
+                                doc_part, idx_document, index_offset
+                            )
+                        )
+                else:
+                    transformer_embs = self._get_transformer_embeddings(
+                        text, idx_document
+                    )
+
+                document_embedded = self._match_transformer_embeddings_to_spacy_tokens(
+                    transformer_embs, doc, prep_offsets
                 )
+
+                if len(document_embedded) != len(doc):
+                    idx_document = batch_number * self.batch_size + document_number
+                    if WarningType.TOKEN_MISMATCHING.value in self._warnings:
+                        self._warnings[WarningType.TOKEN_MISMATCHING.value].append(
+                            idx_document
+                        )
+                    else:
+                        self._warnings[WarningType.TOKEN_MISMATCHING.value] = [
+                            idx_document
+                        ]
+
                 documents_batch_embedded.append(document_embedded)
             yield documents_batch_embedded
 
-    def _get_token_embedding_from_char_embedding(
+    def _preprocess_doc_text(self, doc: Doc) -> Tuple[str, np.ndarray]:
+        """Replaces the text of tokens which only consist of whitespace characters
+        with the special token [NL] (new line).
+        The special token and the whitespace string can consist of different number of
+        chars. To match the tokens later these differences are saved as offsets.
+
+        Args:
+            doc: spacy document
+        Returns:
+            Preprocessed text in which whitespace tokens are
+            replaced by a special token, an array containing the indices of replaced
+            strings and the resulting offset
+        """
+
+        prep_text = ""
+        idx_already_preprocessed = 0
+        # pairs of the line number of the preprocessed text and the offset relative to
+        # the original document, here, offset is the difference btw the preprocessed and
+        # the original text.
+        prep_offsets = [(0, 0)]
+
+        for tkn in doc:
+            if not re.sub(r"[\s]+", "", tkn.text):
+                # indices of current token which will be replaced by the special token
+                idx_start, idx_end = tkn.idx, tkn.idx + len(tkn)
+                # append already processed text and the special token
+                prep_text += doc.text[idx_already_preprocessed:idx_start]
+                prep_text += self._NL_TOKEN
+
+                additional_offset = len(tkn) - len(self._NL_TOKEN)
+                prep_offsets.append(
+                    (
+                        len(prep_text),  # index to apply offset
+                        additional_offset,  # offset to be applied
+                    )
+                )
+                idx_already_preprocessed = idx_end
+
+        # add remaining text
+        prep_text += doc.text[idx_already_preprocessed:]
+
+        return prep_text, np.array(prep_offsets)
+
+    def _match_transformer_embeddings_to_spacy_tokens(
         self,
-        char_level_embeddings: List[List[Tuple[int, int, List[List[float]]]]],
+        transformer_embeddings: List[List[Tuple[int, int, List[List[float]]]]],
         document_tokenized: Doc,
+        prep_offsets: np.ndarray = None,
     ) -> List[List[float]]:
+        """
+        Transformer and spacy tokens differ. Usual the transformer tokenizer splits
+        splits the text into smaller subparts in comparison to the spacy tokenizer.
+        To create embeddings for the spacy tokens the transformer embeddings must be
+        matched. This is done by comparing the char spans of the tokens and matching the
+        tokens which overlap.
+
+        Args:
+            transformer_embeddings: List of start and end indices for each transformer
+                token and the corresponding embedding
+            document_tokenized: spacy tokens
+            prep_offsets: Indices and offsets to match the preprocessed text to the
+                original document
+        Returns:
+            Embeddings for each spacy token in the tokenized document.
+        """
+
         embeddings = defaultdict(list)
 
-        for index_start, index_end, char_embeddings in char_level_embeddings:
+        for index_start, index_end, transformer_emb in transformer_embeddings:
+
+            if prep_offsets is not None:
+                index_start = self._add_offset(index_start, prep_offsets)
+                index_end = self._add_offset(index_end, prep_offsets)
+
             span = document_tokenized.char_span(
                 index_start, index_end, alignment_mode="expand"
             )
             if span is not None:
-                token = span[0]
-                embeddings[token.i].extend(char_embeddings)
+                # if a transformer token include multiple spacy tokens, the spacy
+                # tokens get the same transformer embedding.
+                for token in span:
+                    embeddings[token.i].extend(transformer_emb)
         for key, values in embeddings.items():
             embeddings[key] = np.array(values).mean(0).tolist()
         return list(embeddings.values())
 
-    def _get_char_level_embeddings(
-        self, document: str
+    def _add_offset(self, idx: int, offsets: np.ndarray) -> int:
+        """
+        Adds offset to index according to the offsets array.
+
+        Args:
+            idx: index to transform
+            offsets: indices and the corresponding offsets
+        Returns:
+            Index customized according to the offset
+        """
+        return idx + np.sum(offsets[np.where(offsets[:, 0] <= idx)][:, 1])
+
+    def _get_transformer_embeddings(
+        self,
+        document: str,
+        idx_document: int,
+        idx_offset: int = 0,
     ) -> List[List[Tuple[int, int, List[List[float]]]]]:
-        encoded = self.transformer_tokenizer.encode_plus(
-            document, return_tensors="pt")
+        """
+        Calculates embeddings for the given document using a transformer model.
+        First, the corresponding transformer tokens are computed. The next steps
+        computes the embeddings. With each embedding the indices of the according
+        chars are returned. idx_offset is used to return the correct indices if the
+        document has been split.
+
+        Args:
+            document: plain document text
+            idx_offset: offset if the document has been splitted
+        Returns:
+           Start and end index for each transformer token and the calculated
+           embedding
+        """
+        encoded = self.transformer_tokenizer(document, return_tensors="pt").to(
+            self.device
+        )
         tokens = encoded.encodings[0]
-        num_tokens = len(
-            set(tokens.words[1:-1])
-        )  # 1 and -1 are [CLS] tokens, and other tokens can be ##subwords
+
+        # fallback if the number of tokens is still too big
+        if len(tokens) > self.model.config.max_position_embeddings:
+            if WarningType.DOCUMENT_IS_SPLITTED.value in self._warnings:
+                self._warnings[WarningType.DOCUMENT_IS_SPLITTED.value].append(
+                    idx_document
+                )
+            else:
+                self._warnings[WarningType.DOCUMENT_IS_SPLITTED.value] = [idx_document]
+
+            token_embs = []
+            for doc_part, additional_idx_offset in self._split_document(
+                document, len(tokens)
+            ):
+                token_embs.extend(
+                    self._get_transformer_embeddings(
+                        doc_part, idx_document, idx_offset + additional_idx_offset
+                    )
+                )
+            return token_embs
+
         with torch.no_grad():
             output = self.model(**encoded)
 
         # Get all hidden states
         states = output.hidden_states
         # Stack and sum last four layers
         layers = [-4, -3, -2, -1]
         output = torch.stack([states[i] for i in layers]).sum(0).squeeze()
 
         token_embeddings = []
-
-        for token_idx in range(num_tokens):
-            index_begin, index_end = tokens.word_to_chars(token_idx)
-            token_ids_word = np.where(
-                np.array(encoded.word_ids()) == token_idx)
+        # 1 and -1 are [CLS] tokens, and other tokens can be ##subwords
+        for word_idx in set(tokens.word_ids[1:-1]):
+            index_begin, index_end = tokens.word_to_chars(word_idx)
+            token_ids_word = np.where(np.array(encoded.word_ids()) == word_idx)
             # Only select the tokens that constitute the requested word
             word_tokens_output = output[token_ids_word]
             token_embeddings.append(
-                [index_begin, index_end, word_tokens_output.tolist()]
+                [
+                    index_begin + idx_offset,
+                    index_end + idx_offset,
+                    word_tokens_output.tolist(),
+                ]
             )
         return token_embeddings
+
+    def _estimate_token_number(self, document: str) -> int:
+        """
+        Estimates the number of tokens which are generated by the transformer model.
+        It is based on the rule of thumb that per token 3 subtokens are created by
+        the transformer tokenizer. Tokens are created by splitting at every
+        special and whitespace character.
+        Special Characters are handled seperately according to the assumption that each
+        special character is treated as a token by the transformer tokenizer.
+
+        Args:
+            document: plain text document
+        Returns:
+            Estimation for the number of transformer tokens included in the document
+        """
+        avg_subtokens_per_token = 3
+        number_word_tokens = len(re.findall(r"\[NL\]|\w+", document))
+        number_special_characters = len(re.sub(r"[\w\s]+", "", document))
+        return avg_subtokens_per_token * number_word_tokens + number_special_characters
+
+    def _split_document(
+        self, document: str, estimated_tokens: int
+    ) -> Iterator[Tuple[str, int]]:
+        """
+        Splits the documens into subparts, according to the model's max length and the
+        number of estimated tokens.
+
+        Args:
+            document: plain text document
+            estimated_tokens: estimation for the token number
+        Returns:
+            Yields subpart of the document, splitted depending on max model length and
+            estimated number of tokens
+        """
+        # the regular expression matches the special token [NL], any word consiting of
+        # numbers and chars and single characters which are no whitespace or word
+        # character
+        token_spans = [
+            token.span() for token in re.finditer(r"\[NL\]|\w+|[^\w\s]+?", document)
+        ]
+        split_into = (
+            round(estimated_tokens / self.model.config.max_position_embeddings) + 1
+        )
+        len_part = math.ceil(len(token_spans) / split_into)
+
+        prev_split_idx = 0
+        for i in range(split_into):
+            current_split_idx = min(
+                len(document),
+                token_spans[min((i + 1) * len_part, len(token_spans) - 1)][1],
+            )
+            yield document[prev_split_idx:current_split_idx], prev_split_idx
+            prev_split_idx = current_split_idx
```

## embedders/extraction/reduce.py

```diff
@@ -27,15 +27,15 @@
         self, documents, fit_model, fit_after_n_batches
     ) -> Generator[List[List[List[Union[float, int]]]], None, None]:
         if fit_model:
             embeddings_training = []
             num_batches = util.num_batches(documents, self.embedder.batch_size)
             fit_after_n_batches = min(num_batches, fit_after_n_batches) - 1
             for batch_idx, batch in enumerate(
-                list(self.embedder.fit_transform(documents, as_generator=True))
+                self.embedder.fit_transform(documents, as_generator=True)
             ):
                 if batch_idx <= fit_after_n_batches:
                     embeddings_training.append(batch)
 
                 if batch_idx == fit_after_n_batches:
                     embeddings_training_flattened = []
                     for batch_training in embeddings_training:
```

## Comparing `embedders-0.0.9.dist-info/LICENSE` & `embedders-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `embedders-0.0.9.dist-info/RECORD` & `embedders-0.1.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-embedders/__init__.py,sha256=zmWDBOmBdHpg3-3wr4wdSdE6ZL1S35TGd7gZap6aC6g,5782
+embedders/__init__.py,sha256=k16jAhhQlZWXuJKGP2mIvhOWI7zxhk_B97i4cNlCYIc,6934
+embedders/enums.py,sha256=uGhAUUum4w6fNKZa8gqXBlnPTnKbZhFsbIEFdDdXzcc,143
 embedders/util.py,sha256=XnpCyf5U0z7EWmgOQJ46v1diI6JXsYGYFBI2c_-nycc,399
-embedders/classification/__init__.py,sha256=ewZiEukpAOgMLKU-JTdPhHrPVJFLQUKzZAco7cC1ihw,151
-embedders/classification/contextual.py,sha256=P1rpUfpt9A1HamoMRu7BLcQpdIF5C76Z7gFlVQ6gvW0,1168
+embedders/classification/__init__.py,sha256=A0qKkBCI9ENcyY3D2H2at8IOLEpK112uwN2iJEOoG7c,178
+embedders/classification/contextual.py,sha256=U_sNfHqugkQT9rsajj5QKzZ24iwDy82kML-aO2byLS4,2853
 embedders/classification/count_based.py,sha256=uaGTdwljsA1cXlYWhtFQhuAGUtct12j3qnXh-mfIq9k,3285
-embedders/classification/reduce.py,sha256=4v1dmFTg_337rRnormjwBShIjF-qO_8e2TGFvzsKYFw,2176
-embedders/extraction/__init__.py,sha256=q40GJDzPIov-Za_wu7uzuO6YMJQ14iEJT9T3PMkic4o,634
-embedders/extraction/contextual.py,sha256=hOSLX99x6t6V8jelfCPy_cm9y0hfpoNM8Ug1b1TPzNg,5786
+embedders/classification/reduce.py,sha256=hXXoK_vS-tzCmZmPFbfQ_pML2bGzqL2w-UrWhqn5gV4,2170
+embedders/extraction/__init__.py,sha256=D5YDQTnOTa7qO76CSXyqHCTtmIP559crWHXCBkTo5Co,670
+embedders/extraction/contextual.py,sha256=r0wviuKgssOqpx32iVzb5IRrTziR5TpDs-0a2TlyQWo,14751
 embedders/extraction/count_based.py,sha256=uwhg2r3D-My3faMv81OHCDkbQyjTWv3Uomft6BsxKik,1784
-embedders/extraction/reduce.py,sha256=czQkO2GtrzJbLd4RSnjr7V8AS9M89BumDw3QCxwGFKw,2711
+embedders/extraction/reduce.py,sha256=iezo-xOkYfeuuio4O_JSUEeBfJHG6Iw1MqUmpS5enwk,2705
 embedders/samples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 embedders/samples/clickbait.py,sha256=IiivTTmb3zIUaurod3L0ADruCQuXtHGXsU4fW4IrFQc,6158
-embedders-0.0.9.dist-info/LICENSE,sha256=JYWPdm7R90tTEXK6muMxOgQBHToBQaLT9rPehcITO4I,11340
-embedders-0.0.9.dist-info/METADATA,sha256=as9Qcitw3kooTsHazW-3b9rpCa3ggsuC0a7xFhNA7dw,8811
-embedders-0.0.9.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-embedders-0.0.9.dist-info/top_level.txt,sha256=iRhfbBg_ZWmtclxcpD-WZe5rD-rvHFHKGkJwcWZM_f0,10
-embedders-0.0.9.dist-info/RECORD,,
+embedders-0.1.0.dist-info/LICENSE,sha256=JYWPdm7R90tTEXK6muMxOgQBHToBQaLT9rPehcITO4I,11340
+embedders-0.1.0.dist-info/METADATA,sha256=cq2bMjYi3EtWIGq1Nk2GgRxOhLhAHeUyrdW6e3UsLwU,7012
+embedders-0.1.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+embedders-0.1.0.dist-info/top_level.txt,sha256=iRhfbBg_ZWmtclxcpD-WZe5rD-rvHFHKGkJwcWZM_f0,10
+embedders-0.1.0.dist-info/RECORD,,
```

