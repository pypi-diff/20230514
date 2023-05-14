# Comparing `tmp/dnadb-0.3.0.tar.gz` & `tmp/dnadb-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.3.0.tar", last modified: Sat May 13 03:03:23 2023, max compression
+gzip compressed data, was "dnadb-0.4.0.tar", last modified: Sun May 14 15:59:48 2023, max compression
```

## Comparing `dnadb-0.3.0.tar` & `dnadb-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-13 03:03:23.858793 dnadb-0.3.0/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.3.0/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-13 03:03:23.854793 dnadb-0.3.0/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.3.0/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-12 20:49:48.000000 dnadb-0.3.0/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-13 03:03:23.858793 dnadb-0.3.0/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-13 03:03:23.854793 dnadb-0.3.0/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-13 03:03:23.854793 dnadb-0.3.0/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-12 20:50:07.000000 dnadb-0.3.0/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-13 03:03:23.854793 dnadb-0.3.0/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.3.0/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-03-29 23:23:08.000000 dnadb-0.3.0/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.3.0/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-13 03:03:23.854793 dnadb-0.3.0/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5492 2023-04-14 13:32:31.000000 dnadb-0.3.0/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.3.0/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     2234 2023-05-10 12:52:14.000000 dnadb-0.3.0/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4815 2023-05-11 20:35:23.000000 dnadb-0.3.0/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     5208 2023-05-11 01:32:34.000000 dnadb-0.3.0/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     5969 2023-05-11 01:44:43.000000 dnadb-0.3.0/src/dnadb/fastq.py
--rw-r--r--   0 dwl2x     (1000) users      (100)        0 2023-05-09 22:29:41.000000 dnadb-0.3.0/src/dnadb/otu.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    19471 2023-05-13 03:02:48.000000 dnadb-0.3.0/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.3.0/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-13 03:03:23.854793 dnadb-0.3.0/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-13 03:03:23.000000 dnadb-0.3.0/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      519 2023-05-13 03:03:23.000000 dnadb-0.3.0/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-13 03:03:23.000000 dnadb-0.3.0/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-13 03:03:23.000000 dnadb-0.3.0/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-13 03:03:23.000000 dnadb-0.3.0/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-14 15:59:48.755522 dnadb-0.4.0/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.4.0/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-14 15:59:48.755522 dnadb-0.4.0/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.4.0/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-14 15:58:37.000000 dnadb-0.4.0/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-14 15:59:48.755522 dnadb-0.4.0/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-14 15:59:48.751522 dnadb-0.4.0/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-14 15:59:48.755522 dnadb-0.4.0/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-14 15:58:48.000000 dnadb-0.4.0/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-14 15:59:48.755522 dnadb-0.4.0/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.4.0/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.4.0/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.4.0/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-14 15:59:48.755522 dnadb-0.4.0/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 15:33:28.000000 dnadb-0.4.0/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.4.0/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     2234 2023-05-10 12:52:14.000000 dnadb-0.4.0/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     4815 2023-05-11 20:35:23.000000 dnadb-0.4.0/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5208 2023-05-11 01:32:34.000000 dnadb-0.4.0/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5969 2023-05-11 01:44:43.000000 dnadb-0.4.0/src/dnadb/fastq.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)        0 2023-05-09 22:29:41.000000 dnadb-0.4.0/src/dnadb/otu.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    19344 2023-05-14 14:55:16.000000 dnadb-0.4.0/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.4.0/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-14 15:59:48.755522 dnadb-0.4.0/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-14 15:59:48.000000 dnadb-0.4.0/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      519 2023-05-14 15:59:48.000000 dnadb-0.4.0/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-14 15:59:48.000000 dnadb-0.4.0/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-14 15:59:48.000000 dnadb-0.4.0/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-14 15:59:48.000000 dnadb-0.4.0/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.3.0/LICENSE` & `dnadb-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.3.0/PKG-INFO` & `dnadb-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.3.0
+Version: 0.4.0
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.3.0/pyproject.toml` & `dnadb-0.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.3.0/src/dnadb/datasets/dataset.py` & `dnadb-0.4.0/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.3.0/src/dnadb/datasets/greengenes.py` & `dnadb-0.4.0/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.3.0/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.4.0/src/dnadb/datasets/silva/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from dataclasses import replace
 import enum
 from functools import cached_property
 from pathlib import Path
 from typing import List, Optional, Union
 
 
 from . import taxonomy_map as taxmap
@@ -48,32 +49,32 @@
         super().__init__(path=path, version=version, force_download=force_download)
         if not (self.path / self.fasta_file).exists() or force_download:
             self.__build_dna_fasta()
         if not (self.path / self.taxonomy_file).exists() or force_download:
             self.__build_taxonomy_map()
 
     def __build_dna_fasta(self):
-        print("Converting FASTA to DNA...")
-        fasta_path = Path((self.path / self.fasta_file).stem) # remove .gz extension
+        print("Converting RNA to DNA...")
+        fasta_path = Path(self.path / self.fasta_file).with_suffix("") # remove .gz extension
         fasta_path.parent.mkdir(exist_ok=True)
 
         def map_to_dna(entry: fasta.FastaEntry) -> fasta.FastaEntry:
-            entry.sequence = to_dna(entry.sequence)
-            return entry
+            return replace(entry, sequence=to_dna(entry.sequence))
         entry_iterator = fasta.entries(self.path / self.__rna_fasta_file)
         entry_iterator = map(map_to_dna, entry_iterator)
         with open(fasta_path, 'w') as file:
             fasta.write(file, entry_iterator)
 
         print("Compressing FASTA...")
         compress(fasta_path)
 
     def __build_taxonomy_map(self):
         print("Building taxonomy map...")
-        taxonomy_file_path = Path((self.path / self.taxonomy_file).stem) # remove .gz extension
+        # remove .gz extension
+        taxonomy_file_path = Path(self.path / self.taxonomy_file).with_suffix("")
         taxonomy_file_path.parent.mkdir(exist_ok=True)
 
         input_taxonomy = open_file(self.path / self.__taxonomy_file, 'r')
         input_taxonomy_tree = open_file(self.path / self.__taxonomy_tree_file, 'r')
         input_taxonomy_map = open_file(self.path / self.__taxonomy_map_file, 'r')
         ouput_taxonomy = open(taxonomy_file_path, 'w')
```

### Comparing `dnadb-0.3.0/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.4.0/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.3.0/src/dnadb/db.py` & `dnadb-0.4.0/src/dnadb/db.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.3.0/src/dnadb/dna.py` & `dnadb-0.4.0/src/dnadb/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.3.0/src/dnadb/fasta.py` & `dnadb-0.4.0/src/dnadb/fasta.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.3.0/src/dnadb/fastq.py` & `dnadb-0.4.0/src/dnadb/fastq.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.3.0/src/dnadb/taxonomy.py` & `dnadb-0.4.0/src/dnadb/taxonomy.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
     Split taxonomy label into a tuple
     """
     # print(f'Split: {tuple(re.findall(r"\w__([^;]+)", taxonomy))}')
     return tuple(re.findall(r"\w__([^;]+)", taxonomy))
 
 
-def join_taxonomy(taxonomy: Union[Tuple[str], List[str]]) -> str:
+def join_taxonomy(taxonomy: Union[Tuple[str, ...], List[str]]) -> str:
     """
     Merge a taxonomy tuple into a string format
     """
     depth = len(taxonomy)
     assert depth >= 1 and depth <= len(RANKS), "Invalid taxonomy"
     taxonomy = tuple(taxonomy) + ("",) * (len(RANKS) - depth)
     return "; ".join([f"{RANK_PREFIXES[i]}__{taxon}" for i, taxon in enumerate(taxonomy)])
@@ -299,32 +299,42 @@
 
     def __init__(self, depth: int):
         self.depth = depth
         self.taxons = tuple(TaxonomyHierarchy.TaxonDict() for _ in range(depth))
         self.__taxon_to_id_map: Optional[Tuple[Dict[Taxon, int], ...]] = None
         self.__id_to_taxon_map: Optional[Tuple[Dict[int, Taxon], ...]] = None
 
+    def add_entries(self, entries: Iterable[TaxonomyEntry]):
+        """
+        Add taxonomy entries to the hierarchy.
+
+        Args:
+            entries (Iterable[TaxonomyEntry]): The taxonomy entries to add.
+        """
+        for entry in entries:
+            self.add_entry(entry)
+
     def add_entry(self, entry: TaxonomyEntry):
         """
         Add a taxonomy entry to the hierarchy.
 
         Args:
             entry (TaxonomyEntry): The taxonomy entry to add.
         """
         self.add_taxonomy(entry.label)
 
-    def add_entries(self, entries: Iterable[TaxonomyEntry]):
+    def add_taxonomies(self, taxonomies: Iterable[str]):
         """
-        Add taxonomy entries to the hierarchy.
+        Add taxonomy labels to the hierarchy.
 
         Args:
-            entries (Iterable[TaxonomyEntry]): The taxonomy entries to add.
+            taxonomies (Iterable[str]): The taxonomy labels to add (e.g. "k__Bacteria; ...").
         """
-        for entry in entries:
-            self.add_entry(entry)
+        for taxonomy in taxonomies:
+            self.add_taxonomy(taxonomy)
 
     def add_taxonomy(self, taxonomy: str):
         """
         Add a taxonomy to the hierarchy.
 
         Args:
             taxonomy (str): The taxonomy label to add (e.g. "k__Bacteria; ...").
@@ -344,121 +354,102 @@
         for rank, name in enumerate(taxonomy):
             if not self.has_taxon(name, rank):
                 self.__taxon_to_id_map = None
                 self.__id_to_taxon_map = None
                 self.taxons[rank].insert(Taxon(name, rank, parent))
             parent = self.taxons[rank][name]
 
-    def has_taxon(self, taxon: str, rank: int) -> bool:
-        """
-        Check if the given taxon is present within the hierarchy.
-
-        Args:
-            taxon (str): The taxon name to check.
-            rank (int): The rank of the taxon.
-
-        Returns:
-            bool: The taxon is present within the hierarchy.
-        """
-        return (rank < self.depth) and taxon.casefold() in self.taxons[rank]
-
-    def has_taxons(self, taxons: Tuple[str], strict: bool = False) -> bool:
-        """
-        Check if the hierarchy has a list of taxons.
-
-        Note: When strict == False, a valid hierarchy is assumed.
-        """
-        if not strict:
-            return self.has_taxon(taxons[-1], len(taxons) - 1)
-        return all(taxon.casefold() in self.taxons[rank] for rank, taxon in enumerate(taxons))
-
-    @overload
-    def has_taxonomy(self, taxonomy: TaxonomyEntry, strict: bool = False) -> bool:
+    def has_entry(self, taxonomy: TaxonomyEntry, strict: bool = False) -> bool:
         """
         Check if the hierarchy has the given taxonomy.
 
         Args:
             taxonomy (str): The taxonomy label to check (e.g. "k__Bacteria; ...").
             strict (bool, optional): Ensure every taxon exists. Defaults to False.
 
         Returns:
             bool: The hierarchy contains the taxonomy.
         """
-        ...
+        return self.has_taxonomy(taxonomy.label, strict)
 
-    @overload
     def has_taxonomy(self, taxonomy: str, strict: bool = False) -> bool:
         """
         Check if the hierarchy has the given taxonomy.
 
         Args:
             taxonomy (TaxonomyEntry): The taxonomy to check.
             strict (bool, optional): Ensure every taxon exists. Defaults to False.
 
         Returns:
             bool: The hierarchy contains the taxonomy.
         """
-        ...
-
-    def has_taxonomy(self, taxonomy: Union[str, TaxonomyEntry], strict: bool = False) -> bool:
         if isinstance(taxonomy, TaxonomyEntry):
             taxonomy = taxonomy.label
         taxons = split_taxonomy(taxonomy)
         return self.has_taxons(taxons, strict)
 
-    @overload
-    def reduce_taxonomy(self, taxonomy: str, strict: bool = False) -> str:
+    def has_taxon(self, taxon: str, rank: int) -> bool:
         """
-        Reduce the taxonomy to a valid known taxonomy label in the hierarchy.
+        Check if the given taxon is present within the hierarchy.
 
         Args:
-            taxonomy (str): The taxonomy label to reduce (e.g. "k__Bacteria; ...").
-            strict (bool, optional): Ensure every taxon exists. Defaults to False.
+            taxon (str): The taxon name to check.
+            rank (int): The rank of the taxon.
 
         Returns:
-            str: The reduced taxonomy label.
+            bool: The taxon is present within the hierarchy.
         """
-        ...
+        return (rank < self.depth) and taxon.casefold() in self.taxons[rank]
 
-    @overload
-    def reduce_taxonomy(self, taxonomy: TaxonomyEntry, strict: bool = False) -> TaxonomyEntry:
+    def has_taxons(self, taxons: Tuple[str, ...], strict: bool = False) -> bool:
+        """
+        Check if the hierarchy has a list of taxons.
+
+        Note: When strict == False, a valid hierarchy is assumed.
+        """
+        if not strict:
+            return self.has_taxon(taxons[-1], len(taxons) - 1)
+        return all(taxon.casefold() in self.taxons[rank] for rank, taxon in enumerate(taxons))
+
+    def reduce_entry(self, taxonomy: TaxonomyEntry, strict: bool = False) -> TaxonomyEntry:
         """
         Reduce the taxonomy to a valid known taxonomy label in the hierarchy.
 
         Args:
             taxonomy (TaxonomyEntry): The taxonomy entry to reduce.
             strict (bool, optional): Ensure every taxon exists. Defaults to False.
 
         Returns:
             TaxonomyEntry: A new TaxonomyEntry instance containing the reduced taxonomy label.
         """
-        ...
+        return replace(taxonomy, label=self.reduce_taxonomy(taxonomy.label, strict))
 
-    def reduce_taxonomy(
-        self,
-        taxonomy: Union[str, TaxonomyEntry],
-        strict: bool = False
-    ) -> Union[str, TaxonomyEntry]:
-        taxonomy_label = taxonomy.label if isinstance(taxonomy, TaxonomyEntry) else taxonomy
-        taxons = split_taxonomy(taxonomy_label)
-        reduced_taxonomy = join_taxonomy(self.reduce_taxons(taxons, strict))
-        if isinstance(taxonomy, TaxonomyEntry):
-            return replace(taxonomy, label=reduced_taxonomy)
-        return reduced_taxonomy
+    def reduce_taxonomy(self, taxonomy: str, strict: bool = False) -> str:
+        """
+        Reduce the taxonomy to a valid known taxonomy label in the hierarchy.
+
+        Args:
+            taxonomy (str): The taxonomy label to reduce (e.g. "k__Bacteria; ...").
+            strict (bool, optional): Ensure every taxon exists. Defaults to False.
+
+        Returns:
+            str: The reduced taxonomy label.
+        """
+        return join_taxonomy(self.reduce_taxons(split_taxonomy(taxonomy), strict))
 
-    def reduce_taxons(self, taxons: Tuple[str], strict: bool = False) -> Tuple[str]:
+    def reduce_taxons(self, taxons: Tuple[str, ...], strict: bool = False) -> Tuple[str, ...]:
         """
         Reduce the taxonomy tuple to a valid known taxonomy in the hierarchy.
 
         Args:
-            taxons (Tuple[str]): The taxonomy tuple to reduce.
+            taxons (Tuple[str, ...]): The taxonomy tuple to reduce.
             strict (bool, optional): Ensure every taxon exists. Defaults to False.
 
         Returns:
-            Tuple[str]: The reduced taxonomy tuple.
+            Tuple[str, ...]: The reduced taxonomy tuple.
         """
         if strict:
             for rank, taxon in enumerate(taxons):
                 if taxon not in self.taxons[rank]:
                     return taxons[:rank]
             return taxons
         for i in range(len(taxons) - 1, -1, -1):
@@ -471,28 +462,28 @@
         Tokenize the taxonomy label into a a tuple of taxon integer IDs
 
         Args:
             taxonomy (str): The taxonomy label to tokenize (e.g. "k__Bacteria; ...").
             pad (bool): Pad the taxonomy with -1s to the depth of the hierarchy. Defaults to False.
 
         Returns:
-            Tuple[str]: The tokenized taxonomy.
+            Tuple[str, ...]: The tokenized taxonomy.
         """
         return self.tokenize_taxons(split_taxonomy(taxonomy), pad)
 
     def tokenize_taxons(self, taxons: Tuple[str, ...], pad: bool = False) -> npt.NDArray[np.int64]:
         """
         Tokenize the taxonomy tuple into a a tuple of taxon integer IDs
 
         Args:
-            taxons (Tuple[str]): The taxonomy tuple to tokenize.
+            taxons (Tuple[str, ...]): The taxonomy tuple to tokenize.
             pad (bool): Pad the taxonomy with -1s to the depth of the hierarchy. Defaults to False.
 
         Returns:
-            Tuple[str]: The tokenized taxonomy.
+            Tuple[str, ...]: The tokenized taxonomy.
         """
         result = np.empty(len(taxons), np.int64) if not pad else np.full(self.depth, -1, np.int64)
         for rank, taxon in enumerate(taxons):
             result[rank] = self.taxon_to_id_map[rank][self.taxons[rank][taxon]]
         return result
 
     def detokenize(self, taxon_tokens: npt.NDArray[np.int64]) -> str:
@@ -511,15 +502,15 @@
         """
         Detokenize the taxonomy tokens into a taxonomy tuple.
 
         Args:
             taxon_tokens (npt.NDArray[np.int64]): The taxonomy tokens.
 
         Returns:
-            Tuple[str]: The detokenized taxonomy tuple.
+            Tuple[str, ...]: The detokenized taxonomy tuple.
         """
         result = tuple()
         for rank, token in enumerate(taxon_tokens):
             if token < 0:
                 break
             result += (self.id_to_taxon_map[rank][token].name,)
         return result
```

### Comparing `dnadb-0.3.0/src/dnadb/utils.py` & `dnadb-0.4.0/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.3.0/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.4.0/src/dnadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.3.0
+Version: 0.4.0
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.3.0/src/dnadb.egg-info/SOURCES.txt` & `dnadb-0.4.0/src/dnadb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

