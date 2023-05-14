# Comparing `tmp/callingcardstools-0.1.3.tar.gz` & `tmp/callingcardstools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callingcardstools-0.1.3.tar", max compression
+gzip compressed data, was "callingcardstools-0.1.4.tar", max compression
```

## Comparing `callingcardstools-0.1.3.tar` & `callingcardstools-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.1.3/LICENSE
--rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.1.3/README.md
--rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.1.3/callingcardstools/Alignment/AlignmentTagger.py
--rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.1.3/callingcardstools/Alignment/SummaryParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.1.3/callingcardstools/Alignment/__init__.py
--rw-r--r--   0        0        0     8592 2023-04-30 11:24:56.126405 callingcardstools-0.1.3/callingcardstools/Alignment/mammals/ReadRecords.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.3/callingcardstools/Alignment/mammals/__init__.py
--rw-r--r--   0        0        0     7744 2023-04-30 11:27:18.725988 callingcardstools-0.1.3/callingcardstools/Alignment/mammals/process_alignments.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.3/callingcardstools/Alignment/yeast/__init__.py
--rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.1.3/callingcardstools/Alignment/yeast/legacy_makeccf.py
--rw-r--r--   0        0        0    11493 2023-05-06 17:03:46.674557 callingcardstools-0.1.3/callingcardstools/Alignment/yeast/process_alignments.py
--rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.1.3/callingcardstools/BarcodeParser/BarcodeParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.3/callingcardstools/BarcodeParser/__init__.py
--rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.1.3/callingcardstools/BarcodeParser/barcode_table_to_json.py
--rw-r--r--   0        0        0    16874 2023-05-02 18:36:19.660388 callingcardstools-0.1.3/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
--rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.1.3/callingcardstools/BarcodeParser/yeast/__init__.py
--rw-r--r--   0        0        0     4084 2023-05-06 12:15:15.710439 callingcardstools-0.1.3/callingcardstools/QC/StatusFlags.py
--rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.1.3/callingcardstools/QC/__init__.py
--rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.1.3/callingcardstools/QC/create_status_coder.py
--rw-r--r--   0        0        0     7357 2023-05-06 11:17:03.212706 callingcardstools-0.1.3/callingcardstools/QC/parse_id_to_barcode.py
--rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.1.3/callingcardstools/Reads/ReadParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.1.3/callingcardstools/Reads/__init__.py
--rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.1.3/callingcardstools/Reads/legacy_split_fastq.py
--rw-r--r--   0        0        0    11222 2023-05-03 02:30:53.474496 callingcardstools-0.1.3/callingcardstools/Reads/split_fastq.py
--rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.1.3/callingcardstools/Resources/PackageResources.py
--rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.1.3/callingcardstools/Resources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.3/callingcardstools/Resources/human/__init__.py
--rw-r--r--   0        0        0      695 2023-04-30 11:24:56.134406 callingcardstools-0.1.3/callingcardstools/Resources/human/barcode_details.json
--rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.1.3/callingcardstools/Resources/human/chr_map.csv
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.3/callingcardstools/Resources/mouse/__init__.py
--rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.1.3/callingcardstools/Resources/mouse/barcode_details.json
--rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.1.3/callingcardstools/Resources/yeast/README.md
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.3/callingcardstools/Resources/yeast/__init__.py
--rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.1.3/callingcardstools/Resources/yeast/barcode_details.json
--rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.1.3/callingcardstools/Resources/yeast/yeast.db
--rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.1.3/callingcardstools/__init__.py
--rw-r--r--   0        0        0     5674 2023-05-02 19:43:08.730006 callingcardstools-0.1.3/callingcardstools/__main__.py
--rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.1.3/callingcardstools/utils.py
--rw-r--r--   0        0        0     2016 2023-05-06 17:20:44.170147 callingcardstools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 callingcardstools-0.1.3/setup.py
--rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 callingcardstools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.1.4/README.md
+-rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.1.4/callingcardstools/Alignment/AlignmentTagger.py
+-rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.1.4/callingcardstools/Alignment/SummaryParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.1.4/callingcardstools/Alignment/__init__.py
+-rw-r--r--   0        0        0     8592 2023-04-30 11:24:56.126405 callingcardstools-0.1.4/callingcardstools/Alignment/mammals/ReadRecords.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.4/callingcardstools/Alignment/mammals/__init__.py
+-rw-r--r--   0        0        0     7744 2023-04-30 11:27:18.725988 callingcardstools-0.1.4/callingcardstools/Alignment/mammals/process_alignments.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.4/callingcardstools/Alignment/yeast/__init__.py
+-rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.1.4/callingcardstools/Alignment/yeast/legacy_makeccf.py
+-rw-r--r--   0        0        0    11493 2023-05-06 17:03:46.674557 callingcardstools-0.1.4/callingcardstools/Alignment/yeast/process_alignments.py
+-rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.1.4/callingcardstools/BarcodeParser/BarcodeParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.4/callingcardstools/BarcodeParser/__init__.py
+-rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.1.4/callingcardstools/BarcodeParser/barcode_table_to_json.py
+-rw-r--r--   0        0        0    16935 2023-05-14 12:37:55.905065 callingcardstools-0.1.4/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
+-rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.1.4/callingcardstools/BarcodeParser/yeast/__init__.py
+-rw-r--r--   0        0        0     4084 2023-05-06 12:15:15.710439 callingcardstools-0.1.4/callingcardstools/QC/StatusFlags.py
+-rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.1.4/callingcardstools/QC/__init__.py
+-rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.1.4/callingcardstools/QC/create_status_coder.py
+-rw-r--r--   0        0        0     7357 2023-05-06 11:17:03.212706 callingcardstools-0.1.4/callingcardstools/QC/parse_id_to_barcode.py
+-rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.1.4/callingcardstools/Reads/ReadParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.1.4/callingcardstools/Reads/__init__.py
+-rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.1.4/callingcardstools/Reads/legacy_split_fastq.py
+-rw-r--r--   0        0        0    11471 2023-05-14 12:33:07.536131 callingcardstools-0.1.4/callingcardstools/Reads/split_fastq.py
+-rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.1.4/callingcardstools/Resources/PackageResources.py
+-rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/human/__init__.py
+-rw-r--r--   0        0        0      695 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/human/barcode_details.json
+-rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/human/chr_map.csv
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/mouse/__init__.py
+-rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/mouse/barcode_details.json
+-rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/yeast/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/yeast/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.1.4/callingcardstools/Resources/yeast/barcode_details.json
+-rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.1.4/callingcardstools/Resources/yeast/yeast.db
+-rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.1.4/callingcardstools/__init__.py
+-rw-r--r--   0        0        0     5674 2023-05-14 12:31:35.835834 callingcardstools-0.1.4/callingcardstools/__main__.py
+-rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.1.4/callingcardstools/utils.py
+-rw-r--r--   0        0        0     2016 2023-05-14 12:39:49.417968 callingcardstools-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 callingcardstools-0.1.4/setup.py
+-rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 callingcardstools-0.1.4/PKG-INFO
```

### Comparing `callingcardstools-0.1.3/LICENSE` & `callingcardstools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/README.md` & `callingcardstools-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Alignment/AlignmentTagger.py` & `callingcardstools-0.1.4/callingcardstools/Alignment/AlignmentTagger.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Alignment/SummaryParser.py` & `callingcardstools-0.1.4/callingcardstools/Alignment/SummaryParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Alignment/mammals/ReadRecords.py` & `callingcardstools-0.1.4/callingcardstools/Alignment/mammals/ReadRecords.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Alignment/mammals/process_alignments.py` & `callingcardstools-0.1.4/callingcardstools/Alignment/mammals/process_alignments.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Alignment/yeast/legacy_makeccf.py` & `callingcardstools-0.1.4/callingcardstools/Alignment/yeast/legacy_makeccf.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Alignment/yeast/process_alignments.py` & `callingcardstools-0.1.4/callingcardstools/Alignment/yeast/process_alignments.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/BarcodeParser/BarcodeParser.py` & `callingcardstools-0.1.4/callingcardstools/BarcodeParser/BarcodeParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/BarcodeParser/barcode_table_to_json.py` & `callingcardstools-0.1.4/callingcardstools/BarcodeParser/barcode_table_to_json.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py` & `callingcardstools-0.1.4/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,18 +336,19 @@
         """
         # check that the output_dirpath is a valid directory
         if not os.path.join(output_dirpath):
             raise ValueError("output_dirpath must be a valid directory")
         # if raw is true, then pickle the object
         if raw:
             pickle_path = os.path.join(
-                output_dirpath, filename + suffix + ".pickle")
+                output_dirpath, filename + '_' + suffix + ".pickle")
             logger.info("pickling barcode_qc object to %s{pick_path}")
             with open(pickle_path, "wb") as pickle_file:
                 pickle.dump(self, pickle_file)
+                
         # if component_dict is passed
         if component_dict:
             # input checks
             if not isinstance(component_dict, dict):
                 raise TypeError("component_dict must be a dictionary")
             if not {'tf', 'r1_primer', 'r2_transposon'} == \
                     set(list(component_dict.keys())):
@@ -362,26 +363,28 @@
                     raise TypeError("component_dict values must be lists")
             if len({len(x) for x in component_dict.values()}) != 1:
                 raise ValueError("component_dict values must be lists of "
                                  "the same length")
             # extract summaries from the metrics
             r1_primer_summary, r2_transposon_summary = \
                 self._summarize_by_tf(component_dict)
+            
             # write r1_primer_summary to file
             r1_primer_basename = \
-                filename + "_r1_primer_summary" + suffix + ".csv"
+                filename + "_r1_primer_summary" + '_' + suffix + ".csv"
             r1_primer_summary_path = os.path.join(
                 output_dirpath, r1_primer_basename)
             r1_primer_summary_df = pd.DataFrame(r1_primer_summary)
             logger.info("writing r1_primer_summary "
                         "to %s{r1_primer_summary_path}")
             r1_primer_summary_df.to_csv(r1_primer_summary_path, index=False)
+            
             # write r2_transposon summary to file
             r2_transposon_summary_basename = \
-                filename + "_r2_transposon_summary" + suffix + ".csv"
+                filename + "_r2_transposon_summary" + '_' + suffix + ".csv"
             r2_transposon_summary_path = os.path.join(
                 output_dirpath, r2_transposon_summary_basename)
             r2_transposon_summary_df = pd.DataFrame(r2_transposon_summary)
             logger.info("writing r2_transposon_summary "
                         "to %s{r2_transposon_summary_path}")
             r2_transposon_summary_df.to_csv(
                 r2_transposon_summary_path, index=False)
```

### Comparing `callingcardstools-0.1.3/callingcardstools/QC/StatusFlags.py` & `callingcardstools-0.1.4/callingcardstools/QC/StatusFlags.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/QC/create_status_coder.py` & `callingcardstools-0.1.4/callingcardstools/QC/create_status_coder.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/QC/parse_id_to_barcode.py` & `callingcardstools-0.1.4/callingcardstools/QC/parse_id_to_barcode.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Reads/ReadParser.py` & `callingcardstools-0.1.4/callingcardstools/Reads/ReadParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Reads/legacy_split_fastq.py` & `callingcardstools-0.1.4/callingcardstools/Reads/legacy_split_fastq.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Reads/split_fastq.py` & `callingcardstools-0.1.4/callingcardstools/Reads/split_fastq.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,39 +60,40 @@
                         help='barcode filename (full path)',
                         required=True)
     parser.add_argument('-s',
                         '--split_key',
                         help="Either a name of a key in " +
                         "barcode_details['components'], or just a string. "
                         "This will be used to create the passing "
-                        "output fastq filenames",
+                        "output fastq filenames. Defaults to 'tf' which is "
+                        "appropriate for yeast data",
                         default="tf")
     parser.add_argument('-n',
                         '--split_suffix',
                         help='append this after the tf name and before _R1.fq '
-                        'in the output fastq files',
+                        'in the output fastq files. Defaults to "split"',
                         default="split")
+    parser.add_argument('-o',
+                        '--output_dirpath',
+                        help='a path to a directory where the output files '
+                        'will be output. Defaults to the current directory',
+                        default=".")
     parser.add_argument('-v',
                         '--verbose_qc',
                         help='set this flag to output a file which contains '
                         'the barcode components for each read ID in the '
                         'fastq files associated with its barcode components',
                         action='store_true')
     parser.add_argument('-p',
                         '--pickle_qc',
                         help='set this flag to output a pickle file which '
                         'containing the BarcodeQcCounter object. This is '
                         'useful when splitting the fastq files prior to '
                         'demultiplexing',
                         action='store_true')
-    parser.add_argument('-o',
-                        '--output_dirpath',
-                        help='a path to a directory where the output files '
-                        'will be output',
-                        default=".")
 
     return subparser
 
 
 def split_fastq(args: argparse.Namespace):
 
     # Check inputs
@@ -160,15 +161,15 @@
         id_bc_map.write(
             "\t".join(['id'] + list(rp.components) + additional_components))
         id_bc_map.write("\n")
 
     logging.info('parsing fastq files...')
     # iterate over reads, split reads whose barcode components
     # match expectation into the appropriate file, and reads which don't
-    # fulfill barcode expecations into undetermined.fq
+    # fulfill barcode expectations into undetermined.fq
     while True:
         try:
             rp.next()
         except StopIteration:
             break
         read_dict = rp.parse()
         # if the verbose_qc is on, record the line in the id_bc_map file
@@ -248,16 +249,19 @@
                          rp.barcode_dict['r2']['transposon']['index'][0])
     for k, v in rp.barcode_dict['components']['tf']['map'].items():
         r1_primer_seq = k[r1_primer_start:r1_primer_end]
         r2_transposon_seq = k[r2_transposon_start:r2_transposon_end]
         component_dict['tf'].append(v)
         component_dict['r1_primer'].append(r1_primer_seq)
         component_dict['r2_transposon'].append(r2_transposon_seq)
+        
     # summarize the barcode metrics
     if args.pickle_qc:
         bc_counter.write(raw=args.pickle_qc,
-                         output_dirpath=args.output_dirpath)
+                         output_dirpath=args.output_dirpath,
+                         suffix=args.split_suffix)
     else:
         bc_counter.write(component_dict=component_dict,
-                         output_dirpath=args.output_dirpath)
+                         output_dirpath=args.output_dirpath,
+                         suffix=args.split_suffix)
 
     logging.info('Done parsing the fastqs!')
```

### Comparing `callingcardstools-0.1.3/callingcardstools/Resources/PackageResources.py` & `callingcardstools-0.1.4/callingcardstools/Resources/PackageResources.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Resources/human/barcode_details.json` & `callingcardstools-0.1.4/callingcardstools/Resources/human/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Resources/human/chr_map.csv` & `callingcardstools-0.1.4/callingcardstools/Resources/human/chr_map.csv`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Resources/mouse/barcode_details.json` & `callingcardstools-0.1.4/callingcardstools/Resources/mouse/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Resources/yeast/README.md` & `callingcardstools-0.1.4/callingcardstools/Resources/yeast/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Resources/yeast/barcode_details.json` & `callingcardstools-0.1.4/callingcardstools/Resources/yeast/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/Resources/yeast/yeast.db` & `callingcardstools-0.1.4/callingcardstools/Resources/yeast/yeast.db`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/callingcardstools/__main__.py` & `callingcardstools-0.1.4/callingcardstools/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         'allows finer exploration of the barcode and alignment metrics',
     }
 
     # common options -- these can be applied to all scripts via the 'parent'---
     # argument -- see subparsers.add_parser for parse_bam below ---------------
     common_args = argparse.ArgumentParser(
         prog="callingcardstools", add_help=False)
-    common_args_group = common_args.add_argument_group('general')
+    common_args_group = common_args.add_argument_group('General')
     common_args_group.add_argument(
         "-l",
         "--log_level",
         choices=("critical", "error", "warning", "info", "debug"),
         default="warning")
 
     # Create a top level parser -----------------------------------------------
```

### Comparing `callingcardstools-0.1.3/callingcardstools/utils.py` & `callingcardstools-0.1.4/callingcardstools/utils.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.3/pyproject.toml` & `callingcardstools-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "callingCardsTools"
-version = "0.1.3"
+version = "0.1.4"
 description = "A collection of objects and functions to work with calling cards sequencing tools"
 authors = ["chase mateusiak <chase.mateusiak@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://cmatkhan.github.io/callingCardsTools/"
 repository = "https://github.com/cmatKhan/callingCardsTools"
 documentation = "https://cmatkhan.github.io/callingCardsTools/"
```

### Comparing `callingcardstools-0.1.3/setup.py` & `callingcardstools-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'scipy>=1.8.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['callingcardstools = callingcardstools:__main__.main']}
 
 setup_kwargs = {
     'name': 'callingcardstools',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'A collection of objects and functions to work with calling cards sequencing tools',
     'long_description': "# Installation \n\n```\npip install callingcardstools\n```\n\nTo start using the command line tools, see the help message with:\n\n```\ncallingcardstools --help\n```\n\n# Development Installation\n\n1. install [poetry](https://python-poetry.org/)\n  - I prefer to set the default location of the virtual environment to the \n  project directory. You can set that as a global configuration for your \n  poetry installation like so: `poetry config virtualenvs.in-project true`\n\n2. git clone the repo\n\n3. cd into the repo and issue the command `poetry install`\n\n4. shell into the virtual environment with `poetry shell`\n\n5. build the package with `poetry build`\n\n6. install the callingcardstools packge into your virtual environment \n  `pip install dist/callingcardstools-...`\n  - Note: you could figure out how to use the pip install `-e` flag to \n  have an interactive development environment. I don't think that is compatible \n  with only the `pyproject.toml` file, but if you look it up, you'll find good \n  stackoverflow instructions on how to put a dummy `setup.py` file in to make \n  this possible\n\n7. Building the Dockerimage:\n\nCurrently the Dockerimage is built from a stable version on github\n\nNote that unless I set it up, you won't be able to push to my dockerhub repo. \nI think that is possible to do, though. If you wish to push to your own dockerhub, \nreplace the cmatkhan to your username.\n\n```bash\ndocker build -t cmatkhan/callingcardstools - < Dockerfile\n```\n\nwhere cmatkhan/callingcardstools is the tag. This will default to the version \n`latest`\n\nTo push:\n\n```bash\ndocker push cmatkhan/callingcardstools\n```",
     'author': 'chase mateusiak',
     'author_email': 'chase.mateusiak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://cmatkhan.github.io/callingCardsTools/',
```

### Comparing `callingcardstools-0.1.3/PKG-INFO` & `callingcardstools-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: callingcardstools
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of objects and functions to work with calling cards sequencing tools
 Home-page: https://cmatkhan.github.io/callingCardsTools/
 License: MIT
 Author: chase mateusiak
 Author-email: chase.mateusiak@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

