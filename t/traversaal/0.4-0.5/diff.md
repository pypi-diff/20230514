# Comparing `tmp/traversaal-0.4.tar.gz` & `tmp/traversaal-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traversaal-0.4.tar", last modified: Sun May 14 07:00:30 2023, max compression
+gzip compressed data, was "traversaal-0.5.tar", last modified: Sun May 14 07:08:24 2023, max compression
```

## Comparing `traversaal-0.4.tar` & `traversaal-0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 07:00:30.117926 traversaal-0.4/
--rw-r--r--   0 aimzlicious   (501) staff       (20)     1761 2023-05-14 07:00:30.117792 traversaal-0.4/PKG-INFO
--rw-r--r--   0 aimzlicious   (501) staff       (20)     1522 2023-05-14 06:42:38.000000 traversaal-0.4/README.md
--rw-r--r--   0 aimzlicious   (501) staff       (20)       38 2023-05-14 07:00:30.117965 traversaal-0.4/setup.cfg
--rw-r--r--   0 aimzlicious   (501) staff       (20)      641 2023-05-14 06:54:06.000000 traversaal-0.4/setup.py
-drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 07:00:30.117623 traversaal-0.4/traversaal.egg-info/
--rw-r--r--   0 aimzlicious   (501) staff       (20)     1761 2023-05-14 07:00:30.000000 traversaal-0.4/traversaal.egg-info/PKG-INFO
--rw-r--r--   0 aimzlicious   (501) staff       (20)      187 2023-05-14 07:00:30.000000 traversaal-0.4/traversaal.egg-info/SOURCES.txt
--rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 07:00:30.000000 traversaal-0.4/traversaal.egg-info/dependency_links.txt
--rw-r--r--   0 aimzlicious   (501) staff       (20)       25 2023-05-14 07:00:30.000000 traversaal-0.4/traversaal.egg-info/requires.txt
--rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 07:00:30.000000 traversaal-0.4/traversaal.egg-info/top_level.txt
+drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 07:08:24.284086 traversaal-0.5/
+-rw-r--r--   0 aimzlicious   (501) staff       (20)     1740 2023-05-14 07:08:24.283952 traversaal-0.5/PKG-INFO
+-rw-r--r--   0 aimzlicious   (501) staff       (20)     1501 2023-05-14 07:07:42.000000 traversaal-0.5/README.md
+-rw-r--r--   0 aimzlicious   (501) staff       (20)       38 2023-05-14 07:08:24.284127 traversaal-0.5/setup.cfg
+-rw-r--r--   0 aimzlicious   (501) staff       (20)      641 2023-05-14 07:08:17.000000 traversaal-0.5/setup.py
+drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 07:08:24.283777 traversaal-0.5/traversaal.egg-info/
+-rw-r--r--   0 aimzlicious   (501) staff       (20)     1740 2023-05-14 07:08:24.000000 traversaal-0.5/traversaal.egg-info/PKG-INFO
+-rw-r--r--   0 aimzlicious   (501) staff       (20)      187 2023-05-14 07:08:24.000000 traversaal-0.5/traversaal.egg-info/SOURCES.txt
+-rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 07:08:24.000000 traversaal-0.5/traversaal.egg-info/dependency_links.txt
+-rw-r--r--   0 aimzlicious   (501) staff       (20)       25 2023-05-14 07:08:24.000000 traversaal-0.5/traversaal.egg-info/requires.txt
+-rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 07:08:24.000000 traversaal-0.5/traversaal.egg-info/top_level.txt
```

### Comparing `traversaal-0.4/PKG-INFO` & `traversaal-0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traversaal
-Version: 0.4
+Version: 0.5
 Summary: A semantic search package for hotel data
 Home-page: https://github.com/hamzafarooq
 Author: Traversaal
 Author-email: hello@traversaal.com
 Description-Content-Type: text/markdown
 
 ## Traversaal
@@ -27,26 +27,26 @@
 
 import pandas as pd
 import traversaal
 
 model_name = 'bert-base-uncased'
 search = traversaal.SemanticSearch(model_name)
 
-# Load your hotel data into a DataFrame
 df = pd.read_csv('hotels.csv')
-
-# Define the search query
 query = 'great location and service'
 
-# Perform the semantic search
-results = search.search(df, query)
+embedding_df, results = search.search(df, query)
+
+print("Embedding DataFrame:")
+print(embedding_df.head())
 
-# Print the top results
+print("\nSearch Results:")
 print(results.head())
 
+
 For more detailed usage examples and API documentation, please refer to the GitHub repository.
 
 Contributing
 Contributions to Traversaal are welcome! If you encounter any issues, have suggestions, or would like to contribute enhancements or new features, please feel free to submit a pull request on the GitHub repository.
 
 License
 Traversaal is licensed under the MIT License. See the LICENSE file for more details.
```

### Comparing `traversaal-0.4/README.md` & `traversaal-0.5/traversaal.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: traversaal
+Version: 0.5
+Summary: A semantic search package for hotel data
+Home-page: https://github.com/hamzafarooq
+Author: Traversaal
+Author-email: hello@traversaal.com
+Description-Content-Type: text/markdown
+
 ## Traversaal
 
 Traversaal is a Python package that provides a simple semantic search functionality for hotel data. It leverages large language models such as BERT to encode hotel descriptions and reviews, allowing users to perform semantic search queries and retrieve relevant results based on the provided search query.
 
 ## Features
 
 - Efficient semantic search for hotel data based on descriptions and reviews.
@@ -18,26 +27,26 @@
 
 import pandas as pd
 import traversaal
 
 model_name = 'bert-base-uncased'
 search = traversaal.SemanticSearch(model_name)
 
-# Load your hotel data into a DataFrame
 df = pd.read_csv('hotels.csv')
-
-# Define the search query
 query = 'great location and service'
 
-# Perform the semantic search
-results = search.search(df, query)
+embedding_df, results = search.search(df, query)
 
-# Print the top results
+print("Embedding DataFrame:")
+print(embedding_df.head())
+
+print("\nSearch Results:")
 print(results.head())
 
+
 For more detailed usage examples and API documentation, please refer to the GitHub repository.
 
 Contributing
 Contributions to Traversaal are welcome! If you encounter any issues, have suggestions, or would like to contribute enhancements or new features, please feel free to submit a pull request on the GitHub repository.
 
 License
 Traversaal is licensed under the MIT License. See the LICENSE file for more details.
```

### Comparing `traversaal-0.4/setup.py` & `traversaal-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name="traversaal",
-    version="0.4",
+    version="0.5",
     description="A semantic search package for hotel data",
     author="Traversaal",
     author_email="hello@traversaal.com",
     url="https://github.com/hamzafarooq",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `traversaal-0.4/traversaal.egg-info/PKG-INFO` & `traversaal-0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: traversaal
-Version: 0.4
-Summary: A semantic search package for hotel data
-Home-page: https://github.com/hamzafarooq
-Author: Traversaal
-Author-email: hello@traversaal.com
-Description-Content-Type: text/markdown
-
 ## Traversaal
 
 Traversaal is a Python package that provides a simple semantic search functionality for hotel data. It leverages large language models such as BERT to encode hotel descriptions and reviews, allowing users to perform semantic search queries and retrieve relevant results based on the provided search query.
 
 ## Features
 
 - Efficient semantic search for hotel data based on descriptions and reviews.
@@ -27,26 +18,26 @@
 
 import pandas as pd
 import traversaal
 
 model_name = 'bert-base-uncased'
 search = traversaal.SemanticSearch(model_name)
 
-# Load your hotel data into a DataFrame
 df = pd.read_csv('hotels.csv')
-
-# Define the search query
 query = 'great location and service'
 
-# Perform the semantic search
-results = search.search(df, query)
+embedding_df, results = search.search(df, query)
 
-# Print the top results
+print("Embedding DataFrame:")
+print(embedding_df.head())
+
+print("\nSearch Results:")
 print(results.head())
 
+
 For more detailed usage examples and API documentation, please refer to the GitHub repository.
 
 Contributing
 Contributions to Traversaal are welcome! If you encounter any issues, have suggestions, or would like to contribute enhancements or new features, please feel free to submit a pull request on the GitHub repository.
 
 License
 Traversaal is licensed under the MIT License. See the LICENSE file for more details.
```

