# Comparing `tmp/diannpy-0.1.0.tar.gz` & `tmp/diannpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diannpy-0.1.0.tar", max compression
+gzip compressed data, was "diannpy-0.1.1.tar", max compression
```

## Comparing `diannpy-0.1.0.tar` & `diannpy-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2022-06-07 15:13:08.252228 diannpy-0.1.0/diannpy/__init__.py
--rw-r--r--   0        0        0     6471 2022-09-20 10:11:22.718555 diannpy-0.1.0/diannpy/handlers.py
--rw-r--r--   0        0        0    31670 2022-09-19 11:44:49.281951 diannpy-0.1.0/diannpy/operation.py
--rw-r--r--   0        0        0      705 2022-09-20 10:10:53.809489 diannpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1055 2022-09-20 10:11:31.887990 diannpy-0.1.0/setup.py
--rw-r--r--   0        0        0     1000 2022-09-20 10:11:31.887990 diannpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-06-07 15:13:08.252228 diannpy-0.1.1/diannpy/__init__.py
+-rw-r--r--   0        0        0     6471 2022-09-20 10:11:22.718555 diannpy-0.1.1/diannpy/handlers.py
+-rw-r--r--   0        0        0    35216 2023-05-14 14:53:37.885939 diannpy-0.1.1/diannpy/operation.py
+-rw-r--r--   0        0        0      649 2023-05-14 12:38:09.298447 diannpy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1014 1970-01-01 00:00:00.000000 diannpy-0.1.1/setup.py
+-rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 diannpy-0.1.1/PKG-INFO
```

### Comparing `diannpy-0.1.0/diannpy/handlers.py` & `diannpy-0.1.1/diannpy/handlers.py`

 * *Files identical despite different names*

### Comparing `diannpy-0.1.0/diannpy/operation.py` & `diannpy-0.1.1/diannpy/operation.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sklearn.neighbors
 import time
 from goatools.anno.gaf_reader import GafReader
 from goatools.obo_parser import GODag
 
 
 from sklearn.decomposition import PCA
-from sklearn.preprocessing import StandardScaler, normalize, RobustScaler
+from sklearn.preprocessing import RobustScaler
 
 sys.modules['sklearn.neighbors.base'] = sklearn.neighbors._base
 matplotlib.use('agg')
 
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_pdf import PdfPages
 
@@ -133,16 +133,32 @@
         self.data = pd.DataFrame()
 
     def set_data(self, data):
         self.data = data
 
 
 class Diann:
-    def __init__(self, folder_path, temp_folder_path=".", fasta_lib_path="", goa_file="", go_obo=""):
+    def __init__(self, folder_path, temp_folder_path=".", fasta_lib_path="", goa_file="", go_obo="", protein_coverage=False, modification_map=False):
+        """
+        Main object of diannpy
+
+        :type go_obo: str
+        obo file used in conjunction with goa file to add GO definition to output
+        :type goa_file: str
+        goa file used in conjunction with obo file to add GO definition to output
+        :type fasta_lib_path: str
+        fasta library file location used for ptm mapping (default would obtain fasta from uniprot)
+        :type temp_folder_path: str
+        folder location of temporary file for the package (default at the current location)
+        :type folder_path: str
+        folder location of DIANN output
+
+        """
         self.temp_folder_path = temp_folder_path
+        # Creating temporary folder if it does not exist
         os.makedirs(self.temp_folder_path, exist_ok=True)
         self.progress_file = open(os.path.join(self.temp_folder_path, "progress.txt"), "wt")
         self.folder_path = folder_path
         self.fasta_lib_path = fasta_lib_path
         self.goa_file = goa_file
         self.go_obo = go_obo
         self.annotation = {}
@@ -172,28 +188,35 @@
         print("Drawing profile")
         self.draw_profile(self.joined_pg, os.path.join(self.temp_folder_path, "profile.pg.pdf"))
         self.draw_total_intensity(self.joined_pr, os.path.join(self.temp_folder_path, "total.intensity.pr.pdf"))
         self.draw_detected_genes(self.joined_pr, os.path.join(self.temp_folder_path, "gene.detected.pr.pdf"))
         self.draw_cv(self.joined_pr, os.path.join(self.temp_folder_path, "cv.pr.pdf"),
                      ["Condition", "Protein.Group", "Modified.Sequence"])
         self.draw_cv(self.joined_pg, os.path.join(self.temp_folder_path, "cv.pg.pdf"), ["Condition", "Protein.Group"])
-        self.protein_coverage()
-        self.modification_map()
+        if protein_coverage:
+            self.protein_coverage()
+        if modification_map:
+            self.modification_map()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.progress_file.close()
 
     def write_progress(self, message):
         self.progress_file.write(str(time.time()) + "\t" + message + "\n")
         self.progress_file.flush()
 
     def join_df(self, df_dict):
+        """
+        Transpose data file from wide form to long form with the categorical column being the `Sample` name column and `Intensity` as the value
+        :param df_dict:
+        :return:
+        """
         combined_pr = []
         order = []
         condition_order = []
         for k in df_dict:
             if k in self.annotation:
                 folder = k
                 df = pd.melt(df_dict[k],
@@ -227,42 +250,59 @@
         else:
             df = pd.concat(combined_pr, ignore_index=True)
         df["Sample"] = pd.Categorical(df["Sample"].values, categories=order)
         df["Condition"] = pd.Categorical(df["Condition"].values, categories=condition_order)
         return df
 
     def parse_log(self):
+        """
+        go through diann log output and return a dictionary composing  of the folder location of the log file as key and
+        a list of sample column from annotation.txt file from within that folder
+
+        this function also help setting internal sample and condition annotation dictionary of the object
+
+        :return: dict[str, list]
+        """
         file_location = {}
         self.write_progress("Began parsing log file")
         for l in glob(os.path.join(self.folder_path, "**", "*"), recursive=True):
             if l.endswith("Reports.log.txt"):
                 folder, _ = os.path.split(l)
                 file_location[folder] = []
                 annotation_path = os.path.join(folder, "annotation.txt")
+
                 if os.path.exists(annotation_path):
+                    # Get sample names from annotation.txt file
                     self.annotation[folder] = {}
                     df = pd.read_csv(annotation_path, sep="\t")
                     for i, r in df.iterrows():
                         self.annotation[folder][r["Sample"]] = r["Condition"]
                     file_location[folder] = list(df["Sample"].values)
 
                 else:
+                    # Opening log file and using `Loading run` line as flag for parsing sample name
                     with open(l, "rt") as log_stuff:
                         for line in log_stuff:
                             line = line.strip()
                             if "Loading run" in line:
                                 match = re.search("Loading run (.+)", line)
                                 if match:
                                     file = match.group(1)
                                     if file not in file_location[folder]:
                                         file_location[folder].append(file)
         self.write_progress("Completed parsing log file")
         return file_location
 
     def process_pr(self, folder_path, file_list):
+        """
+
+        :param folder_path: folder_path of DIANN output
+        :param file_list: list of input sample
+        :return: pd.DataFrame
+        """
         self.write_progress("Began processing pr_matrix file")
         pr_file = os.path.join(folder_path, "Reports.pr_matrix.tsv")
         df = pd.read_csv(pr_file, sep="\t")
         initial_check_pr(df, file_list)
         self.write_progress("Completed processing pr_matrix file")
         return df
 
@@ -348,15 +388,15 @@
         df = pd.read_csv(report_path, sep="\t")
         for i, r in df.iterrows():
             sample = self.raw_file_location[folder][i]
             df.at[i, "Condition"] = self.annotation[folder][sample]
         mean_data = []
         for label, group_data in df.groupby("Condition"):
             mean_data.append(
-                [label, np.mean(group_data['Proteins.Identified']), sem(group_data["Proteins.Identified"])])
+                [label[0], np.mean(group_data['Proteins.Identified']), sem(group_data["Proteins.Identified"])])
         df_mean = pd.DataFrame(mean_data, columns=["Condition", "Count", "Error"])
         result = ggplot() + \
                  geom_col(df_mean, aes(x="Condition", y="Count", fill="Condition")) + \
                  geom_point(df, aes(x="Condition", y="Proteins.Identified"), fill="black", position="jitter") + \
                  geom_errorbar(
                      df_mean, aes(x="Condition", ymin="Count-Error", ymax="Count+Error")) + \
                  scale_fill_brewer(type="qual", palette="Pastel1") + theme_minimal()
@@ -369,19 +409,19 @@
         mean_data = []
         for label, group_data in data_pr.groupby("Sample"):
             plots.append(
                 ggplot(group_data, aes(x='Category', y='Count', fill='Category', label='Count')) \
                 + scale_fill_brewer(type="qual", palette="Pastel2") \
                 + geom_col() \
                 + geom_text() \
-                + theme_minimal() + theme(figure_size=(8, 6)) + ggtitle(label))
+                + theme_minimal() + theme(figure_size=(8, 6)) + ggtitle(label[0]))
         not_null = data_pr[data_pr["Category"] == "Not Null"]
         not_null["Condition"] = Series([self.annotation[folder][i] for i in not_null["Sample"]], index=not_null.index)
         for label, group_data in not_null.groupby("Condition"):
-            mean_data.append([label, np.mean(group_data['Count']), sem(group_data["Count"])])
+            mean_data.append([label[0], np.mean(group_data['Count']), sem(group_data["Count"])])
         df_mean = pd.DataFrame(mean_data, columns=["Condition", "Count", "Error"])
         plots = [
                     ggplot() +
                     geom_col(df_mean, aes(x="Condition", y="Count", fill="Condition")) +
                     geom_point(not_null, aes(x="Condition", y="Count"), fill="black", position="jitter") +
                     geom_errorbar(
                         df_mean, aes(x="Condition", ymin="Count-Error", ymax="Count+Error")) +
@@ -435,86 +475,120 @@
                 else:
                     current_seq += line
 
             seqs[current_id[:]] = current_seq[:]
         return seqs
 
     def get_seq(self, proteins):
-        for p in proteins["Protein.Group"].split(";"):
-            if p in self.fasta_lib:
-                if p in self.fasta_lib:
-                    yield p, self.fasta_lib[p], proteins["Genes"]
-                else:
-                    yield p, None, proteins["Genes"]
+        # from the protein.group column, get uniprot accession id list and return sequence stored in fasta library if available
+        # if not, return None
+        for protein in proteins["Protein.Group"].split(";"):
+            if protein in self.fasta_lib:
+                yield protein, self.fasta_lib[protein], proteins["Genes"]
+            else:
+                yield protein, None, proteins["Genes"]
+
 
     def protein_coverage(self):
+        # calculate coverage of each protein from DIANN peptide data
+        # coverage is defined as the percentage of the protein sequence that is covered by peptides
+        # coverage is calculated for each sample and peptide with no intensity is not counted
+        # peptide is mapped by checking if they match exactly with any sequence in the protein
+        # if the protein isoform is not found, the first isoform is used
+        # if the peptide is not found in the protein, it is not counted
+
         self.write_progress("Began analyzing protein coverage")
         cover_dict = {}
         gene_dict = {}
-        for i, r in self.joined_pr.iterrows():
-            if pd.notnull(r["Intensity"]):
-                for protein, seq, gene in self.get_seq(r):
+
+        # get peptide data with intensity
+        temp_df = self.joined_pr[self.joined_pr["Intensity"].notnull()]
+
+        # iterate through each peptide
+        for i, r in temp_df.iterrows():
+            # get protein sequence and gene name
+            for protein, seq, gene in self.get_seq(r):
+                if protein not in gene_dict:
                     gene_dict[protein] = gene
-                    if protein not in cover_dict:
-                        cover_dict[protein] = {}
-                    if r["Sample"] not in cover_dict[protein]:
-                        cover_dict[protein][r["Sample"]] = {}
-                    if seq:
-                        try:
+                if protein not in cover_dict:
+                    cover_dict[protein] = {}
+
+                if r["Sample"] not in cover_dict[protein]:
+                    cover_dict[protein][r["Sample"]] = {}
+
+                if seq:
+                    # try to map peptide to protein sequence if it could not be mapped, try the first isoform
+                    try:
+                        ind = seq.index(r["Stripped.Sequence"])
+                    except ValueError:
+                        if protein+"-1" in self.fasta_lib:
+                            seq = self.fasta_lib[protein+"-1"]
                             ind = seq.index(r["Stripped.Sequence"])
-                        except ValueError:
-                            if protein+"-1" in self.fasta_lib:
-                                seq = self.fasta_lib[protein+"-1"]
-                                ind = seq.index(r["Stripped.Sequence"])
-                            else:
-                                ind = -1
-                        if ind > -1:
-                            for n in range(len(r["Stripped.Sequence"])):
-                                pos = ind + n
-                                if pos not in cover_dict[protein][r["Sample"]]:
-                                    cover_dict[protein][r["Sample"]][pos] = 0
-                                cover_dict[protein][r["Sample"]][pos] = cover_dict[protein][r["Sample"]][pos] + 1
+                        else:
+                            ind = -1
+                    if ind > -1:
+                        # if peptide is found, count the position of each residue of the peptide in the protein
+                        # if the position is not in the dictionary, add it
+                        # if the position is in the dictionary, add 1 to the count
+                        for n in range(len(r["Stripped.Sequence"])):
+                            pos = ind + n
+                            if pos not in cover_dict[protein][r["Sample"]]:
+                                cover_dict[protein][r["Sample"]][pos] = 0
+                            cover_dict[protein][r["Sample"]][pos] = cover_dict[protein][r["Sample"]][pos] + 1
         result = []
+
+        # calculate coverage for each protein
         for p in cover_dict:
             if p in self.fasta_lib:
                 for s in cover_dict[p]:
                     covered_pos = list(cover_dict[p][s].keys())
                     seq_len = len(self.fasta_lib[p])
                     result.append([p, len(covered_pos), seq_len, len(covered_pos) / seq_len, gene_dict[p], s])
 
         df = pd.DataFrame(result,
                           columns=["Protein", "Length Covered", "Length", "Covered Proportion", "Gene names", "Sample"])
         self.coverage = df
         self.coverage.to_csv(os.path.join(self.temp_folder_path, "coverage.txt"), sep="\t", index=False)
         self.write_progress("Completed analyzing protein coverage")
 
     def modification_map(self):
+        # map modification sites of each protein from DIANN peptide data
+        # modification sites are defined as the position of the modified residue in the protein sequence
+
         self.write_progress("Began mapping modification sites")
         mod_dict = {}
         result = []
-        for i, r in self.joined_pr.iterrows():
-            if pd.notnull(r["Intensity"]):
-                for protein, seq, gene in self.get_seq(r):
-
-                    if protein not in mod_dict:
-                        mod_dict[protein] = {}
-                    if r["Sample"] not in mod_dict[protein]:
-                        mod_dict[protein][r["Sample"]] = {}
 
-                    if seq:
-                        try:
+        # get peptide data with intensity
+        temp_df = self.joined_pr[self.joined_pr["Intensity"].notnull()]
+
+        for i, r in temp_df.iterrows():
+            for protein, seq, gene in self.get_seq(r):
+
+                if protein not in mod_dict:
+                    mod_dict[protein] = {}
+                if r["Sample"] not in mod_dict[protein]:
+                    mod_dict[protein][r["Sample"]] = {}
+
+                if seq:
+                    try:
+                        ind = seq.index(r["Stripped.Sequence"])
+                    except ValueError:
+                        if protein+"-1" in self.fasta_lib:
+                            seq = self.fasta_lib[protein+"-1"]
                             ind = seq.index(r["Stripped.Sequence"])
-                        except ValueError:
-                            if protein+"-1" in self.fasta_lib:
-                                seq = self.fasta_lib[protein+"-1"]
-                                ind = seq.index(r["Stripped.Sequence"])
-                            else:
-                                ind = -1
-                        modded_pep = Sequence(r["Modified.Sequence"])
+                        else:
+                            ind = -1
+
+                    # parse modified sequence to get the position of the modified residue
+                    modded_pep = Sequence(r["Modified.Sequence"])
+                    # if the peptide is found in the protein, map the modification site
+                    if ind > -1:
                         for n, a in enumerate(modded_pep):
+                            # if the residue is modified, get the name of the modification and the position of the residue
                             if len(a.mods) > 0:
                                 for m in a.mods:
                                     name = self.unimod_mapper.id_to_name(str(m).replace("UniMod:", ""))
                                     pos = ind + n
                                     result.append([protein, pos, name[0], gene, r["Sample"], r["Intensity"]])
 
         df = pd.DataFrame(result, columns=["Protein", "Position", "Modification", "Gene names", "Sample", "Intensity"])
@@ -544,15 +618,17 @@
     def draw_cv_density(self, df: pd.DataFrame, filename):
         self.write_progress("Began creating CV plot")
         plots = []
         custom_legend = {}
         with PdfPages(filename) as pdf_pages:
 
             for label, group_data in df.groupby(["Condition"]):
+                label = label[0]
                 fig, ax = plt.subplots()
+                print(label, np.round(group_data["CV"].median(), 2))
                 title = label + " ({})".format(np.round(group_data["CV"].median(), 2))
                 custom_legend[label] = title
                 sns.kdeplot(data=group_data, x="CV", linewidth=5, ax=ax).set(title=title)
                 plots.append(fig)
             fig, ax = plt.subplots()
             sns.kdeplot(data=df.assign(Label=df["Condition"].map(custom_legend)), hue="Label", x="CV", linewidth=5,
                         ax=ax)
```

### Comparing `diannpy-0.1.0/setup.py` & `diannpy-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,39 +5,37 @@
 ['diannpy']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['goatools>=1.2.3,<2.0.0',
+ 'matplotlib>=3.5.3,<4.0.0',
  'missingpy>=0.2.0,<0.3.0',
- 'pandas>=1.4.4,<2.0.0',
+ 'pandas==2.0.0',
  'pandera>=0.12.0,<0.13.0',
- 'plotnine>=0.9.0,<0.10.0',
- 'redis>=4.3.3,<5.0.0',
- 'requests>=2.28.0,<3.0.0',
- 'rpy2>=3.5.4,<4.0.0',
- 'rq>=1.10.1,<2.0.0',
- 'scikit-learn>=1.1.1,<2.0.0',
+ 'plotnine>=0.12.1,<0.13.0',
+ 'requests>=2.30.0,<3.0.0',
+ 'scikit-learn==1.1.2',
  'seaborn>=0.12.0,<0.13.0',
  'sequal>=1.0.1,<2.0.0',
- 'tornado>=6.1,<7.0',
+ 'tornado>=6.3.1,<7.0.0',
  'unimod-mapper>=0.6.6,<0.7.0',
- 'uniprotparser>=1.0.8,<2.0.0']
+ 'uniprotparser>=1.1.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'diannpy',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': "a package to provide additional report from DIANN's output of proteomics experiment",
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Toan Phung',
     'author_email': 'toan.phungkhoiquoctoan@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `diannpy-0.1.0/PKG-INFO` & `diannpy-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: diannpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: a package to provide additional report from DIANN's output of proteomics experiment
 Author: Toan Phung
 Author-email: toan.phungkhoiquoctoan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: goatools (>=1.2.3,<2.0.0)
+Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
 Requires-Dist: missingpy (>=0.2.0,<0.3.0)
-Requires-Dist: pandas (>=1.4.4,<2.0.0)
+Requires-Dist: pandas (==2.0.0)
 Requires-Dist: pandera (>=0.12.0,<0.13.0)
-Requires-Dist: plotnine (>=0.9.0,<0.10.0)
-Requires-Dist: redis (>=4.3.3,<5.0.0)
-Requires-Dist: requests (>=2.28.0,<3.0.0)
-Requires-Dist: rpy2 (>=3.5.4,<4.0.0)
-Requires-Dist: rq (>=1.10.1,<2.0.0)
-Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
+Requires-Dist: plotnine (>=0.12.1,<0.13.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: scikit-learn (==1.1.2)
 Requires-Dist: seaborn (>=0.12.0,<0.13.0)
 Requires-Dist: sequal (>=1.0.1,<2.0.0)
-Requires-Dist: tornado (>=6.1,<7.0)
+Requires-Dist: tornado (>=6.3.1,<7.0.0)
 Requires-Dist: unimod-mapper (>=0.6.6,<0.7.0)
-Requires-Dist: uniprotparser (>=1.0.8,<2.0.0)
+Requires-Dist: uniprotparser (>=1.1.0,<2.0.0)
```

