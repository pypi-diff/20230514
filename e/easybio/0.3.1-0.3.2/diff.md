# Comparing `tmp/easybio-0.3.1.tar.gz` & `tmp/easybio-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybio-0.3.1.tar", last modified: Wed Apr 26 08:00:24 2023, max compression
+gzip compressed data, was "easybio-0.3.2.tar", last modified: Sun May 14 12:49:39 2023, max compression
```

## Comparing `easybio-0.3.1.tar` & `easybio-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-04-26 08:00:24.486647 easybio-0.3.1/
--rw-rw-r--   0 lei       (1003) lei       (1004)      536 2023-04-26 08:00:24.482647 easybio-0.3.1/PKG-INFO
--rwxrwxr-x   0 lei       (1003) lei       (1004)       30 2023-04-21 05:50:43.000000 easybio-0.3.1/README.md
-drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-04-26 08:00:24.482647 easybio-0.3.1/easyBio/
-drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-04-26 08:00:24.482647 easybio-0.3.1/easyBio/Utils/
--rw-rw-r--   0 lei       (1003) lei       (1004)      337 2023-04-25 14:52:14.000000 easybio-0.3.1/easyBio/Utils/__init__.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     8089 2023-04-22 12:59:53.000000 easybio-0.3.1/easyBio/Utils/download.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     3640 2023-04-25 14:49:11.000000 easybio-0.3.1/easyBio/Utils/downloadUtils.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     7183 2023-04-26 07:57:47.000000 easybio-0.3.1/easyBio/Utils/easyBioUtils.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     2045 2023-04-21 18:02:00.000000 easybio-0.3.1/easyBio/Utils/netUtils.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     1044 2023-04-25 14:49:13.000000 easybio-0.3.1/easyBio/Utils/toolsUtils.py
--rw-rw-r--   0 lei       (1003) lei       (1004)      234 2023-04-25 14:49:00.000000 easybio-0.3.1/easyBio/__init__.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     3809 2023-04-24 05:43:51.000000 easybio-0.3.1/easyBio/changeSRAName.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     1093 2023-04-22 13:14:40.000000 easybio-0.3.1/easyBio/downloadSRA.py
--rw-rw-r--   0 lei       (1003) lei       (1004)      128 2023-04-21 17:04:20.000000 easybio-0.3.1/easyBio/easyBio.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     2914 2023-04-25 14:54:28.000000 easybio-0.3.1/easyBio/pipline.py
--rw-rw-r--   0 lei       (1003) lei       (1004)      816 2023-04-24 09:50:20.000000 easybio-0.3.1/easyBio/run_cellranger.py
--rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-04-21 05:39:47.000000 easybio-0.3.1/easyBio/run_test.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     1490 2023-04-25 14:48:41.000000 easybio-0.3.1/easyBio/splitSRA.py
-drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-04-26 08:00:24.482647 easybio-0.3.1/easybio.egg-info/
--rw-rw-r--   0 lei       (1003) lei       (1004)      536 2023-04-26 08:00:24.000000 easybio-0.3.1/easybio.egg-info/PKG-INFO
--rw-rw-r--   0 lei       (1003) lei       (1004)      575 2023-04-26 08:00:24.000000 easybio-0.3.1/easybio.egg-info/SOURCES.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-04-26 08:00:24.000000 easybio-0.3.1/easybio.egg-info/dependency_links.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)      261 2023-04-26 08:00:24.000000 easybio-0.3.1/easybio.egg-info/entry_points.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-04-22 17:45:52.000000 easybio-0.3.1/easybio.egg-info/not-zip-safe
--rw-rw-r--   0 lei       (1003) lei       (1004)       29 2023-04-26 08:00:24.000000 easybio-0.3.1/easybio.egg-info/requires.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)        8 2023-04-26 08:00:24.000000 easybio-0.3.1/easybio.egg-info/top_level.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-04-26 08:00:24.486647 easybio-0.3.1/setup.cfg
--rw-rw-r--   0 lei       (1003) lei       (1004)     1393 2023-04-26 08:00:06.000000 easybio-0.3.1/setup.py
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-05-14 12:49:39.547809 easybio-0.3.2/
+-rw-rw-r--   0 lei       (1003) lei       (1004)      538 2023-05-14 12:49:39.547809 easybio-0.3.2/PKG-INFO
+-rwxrwxr-x   0 lei       (1003) lei       (1004)       30 2023-04-21 05:50:43.000000 easybio-0.3.2/README.md
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-05-14 12:49:39.547809 easybio-0.3.2/easyBio/
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-05-14 12:49:39.547809 easybio-0.3.2/easyBio/Utils/
+-rw-rw-r--   0 lei       (1003) lei       (1004)      381 2023-04-29 18:26:15.000000 easybio-0.3.2/easyBio/Utils/__init__.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     8161 2023-04-26 10:50:07.000000 easybio-0.3.2/easyBio/Utils/download.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2972 2023-05-14 12:48:32.000000 easybio-0.3.2/easyBio/Utils/downloadUtils.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     8191 2023-04-30 05:57:48.000000 easybio-0.3.2/easyBio/Utils/easyBioUtils.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2117 2023-04-26 10:50:17.000000 easybio-0.3.2/easyBio/Utils/netUtils.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1116 2023-05-11 06:52:34.000000 easybio-0.3.2/easyBio/Utils/toolsUtils.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)      296 2023-05-11 07:10:43.000000 easybio-0.3.2/easyBio/__init__.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     5260 2023-04-27 04:43:16.000000 easybio-0.3.2/easyBio/changeSRAName.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1165 2023-05-14 12:19:48.000000 easybio-0.3.2/easyBio/downloadSRA.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)      200 2023-04-26 10:50:00.000000 easybio-0.3.2/easyBio/easyBio.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     3216 2023-05-14 09:54:01.000000 easybio-0.3.2/easyBio/pipline.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)      904 2023-04-28 15:36:48.000000 easybio-0.3.2/easyBio/run_cellranger.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)      110 2023-04-26 10:48:58.000000 easybio-0.3.2/easyBio/run_test.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     3239 2023-05-04 03:51:00.000000 easybio-0.3.2/easyBio/runvelocyto.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1479 2023-04-29 17:22:45.000000 easybio-0.3.2/easyBio/splitSRA.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1006 2023-04-29 17:25:20.000000 easybio-0.3.2/easyBio/test.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2841 2023-04-30 05:59:02.000000 easybio-0.3.2/easyBio/velocyto2.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2954 2023-04-26 10:42:04.000000 easybio-0.3.2/easyBio/velocyto3.py
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-05-14 12:49:39.547809 easybio-0.3.2/easybio.egg-info/
+-rw-rw-r--   0 lei       (1003) lei       (1004)      538 2023-05-14 12:49:39.000000 easybio-0.3.2/easybio.egg-info/PKG-INFO
+-rw-rw-r--   0 lei       (1003) lei       (1004)      656 2023-05-14 12:49:39.000000 easybio-0.3.2/easybio.egg-info/SOURCES.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-05-14 12:49:39.000000 easybio-0.3.2/easybio.egg-info/dependency_links.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)      302 2023-05-14 12:49:39.000000 easybio-0.3.2/easybio.egg-info/entry_points.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-04-22 17:45:52.000000 easybio-0.3.2/easybio.egg-info/not-zip-safe
+-rw-rw-r--   0 lei       (1003) lei       (1004)       20 2023-05-14 12:49:39.000000 easybio-0.3.2/easybio.egg-info/requires.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        8 2023-05-14 12:49:39.000000 easybio-0.3.2/easybio.egg-info/top_level.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-05-14 12:49:39.547809 easybio-0.3.2/setup.cfg
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1427 2023-05-14 12:49:31.000000 easybio-0.3.2/setup.py
```

### Comparing `easybio-0.3.1/PKG-INFO` & `easybio-0.3.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybio
-Version: 0.3.1
+Version: 0.3.2
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
@@ -12,7 +12,9 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 
 # easyBio_conda
 easyBio_conda
+
+
```

### Comparing `easybio-0.3.1/easyBio/Utils/download.py` & `easybio-0.3.2/easyBio/Utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+# Author: Lei
+# Date: 2023-04-20
+# Description:
 import os
 import requests
 import threadpool
 import math
 from time import time
 import urllib.parse
```

### Comparing `easybio-0.3.1/easyBio/Utils/downloadUtils.py` & `easybio-0.3.2/easyBio/Utils/downloadUtils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+# Author: Lei
+# Date: 2023-04-20
+# Description:
 import math
 import os
 from .netUtils import requestGet
 from .download import Download
 
 
 def getbioproject(gsenumber):
@@ -49,15 +53,15 @@
 
     Returns:
     None
     """
     print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
     threads = min(50, math.ceil(threads / 2))
     bioproject = getbioproject(gsenumber)
-    pjurl = f"https://www.ebi.ac.uk/ena/portal/api/filereport?result=read_run&accession={bioproject}&offset=0&limit=1000&format=json&fields=study_accession,secondary_study_accession,sample_accession,secondary_sample_accession,experiment_accession,run_accession,submission_accession,tax_id,scientific_name,instrument_platform,instrument_model,library_name,nominal_length,library_layout,library_strategy,library_source,library_selection,read_count,base_count,center_name,first_public,last_updated,experiment_title,study_title,study_alias,experiment_alias,run_alias,fastq_bytes,fastq_md5,fastq_ftp,fastq_aspera,fastq_galaxy,submitted_bytes,submitted_md5,submitted_ftp,submitted_aspera,submitted_galaxy,submitted_format,sra_bytes,sra_md5,sra_ftp,sra_aspera,sra_galaxy,cram_index_ftp,cram_index_aspera,cram_index_galaxy,sample_alias,broker_name,sample_title,nominal_sdev,first_created"
+    pjurl = f"https://www.ebi.ac.uk/ena/portal/api/filereport?result=read_run&accession={bioproject}&limit=1000&format=json&fields=run_accession"
     pjre = requestGet(pjurl)
     results = pjre.json()
     filedirs = f"{dirs}/{gsenumber}/raw/sra"
     os.makedirs(filedirs, exist_ok=True)
 
     if idDownloadAll(results, filedirs):
         print("\033[32mAll files have been successfully downloaded. Exiting or entering the fastq-dump program...\033[0m")
@@ -68,12 +72,8 @@
         print("\033[33mrun_accession: {}\033[0m".format(run_accession))
         # sra_md5 = study["sra_md5"]
         sra_ftp = f"https://sra-pub-run-odp.s3.amazonaws.com/sra/{run_accession}/{run_accession}"
         download = Download(sra_ftp, dirs=filedirs, fileName=f"{run_accession}.sra",
                             threadNum=threads, limitTime=60000)
         download.start()
     
-    return False
-
-
-
-
+    return False
```

### Comparing `easybio-0.3.1/easyBio/Utils/easyBioUtils.py` & `easybio-0.3.2/easyBio/Utils/easyBioUtils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+# Author: Lei
+# Date: 2023-04-20
+# Description:
 from concurrent.futures import ThreadPoolExecutor
 import os
 import shutil
 import subprocess
 import concurrent
 
 from .toolsUtils import get_num_threads
@@ -75,31 +79,46 @@
     for sample in samples:
         cmd = f"""cellranger count --id={sample} \
 --transcriptome={db} \
 --fastqs={fq_dir} \
 --sample={sample} \
 --expect-cells={expectcellnum} \
 --nosecondary"""
+
+#         cmd = f"""cellranger count --id={sample} \
+# --transcriptome={db} \
+# --fastqs={fq_dir} \
+# --sample={sample} \
+# --expect-cells={expectcellnum}"""
         print("\033[1;33m Running command for sample {}:\033[0m".format(sample))
         print("\033[1;31m{}\033[0m".format(cmd))
         subprocess.run(cmd, shell=True)
+
+        # result = subprocess.run(
+        #     cmd, shell=True, capture_output=True, text=True)
+        # output = result.stdout  # 获取输出结果
+        # # 对输出结果进行运算
+        # output_lines = output.splitlines()
+        # pre = " ".join(output_lines[-20:-18])  # 获取最后20行中的前2行，并将它们连接为一个字符串
+        # print(f"{sample} {pre}")
+
+        
         if matricespath != "":
             mv_cmd = ["mv", f"{sample}", f"{matricespath}"]
             subprocess.run(mv_cmd, check=True)
 
-
 # 多线程跑cellranger使用，目前看效果不大（比单线程快不了太多）
-def run_cellranger(sample, db, fq_dir, expectcellnum, matricespath):
+def run_cellranger(sample, core, db, fq_dir, expectcellnum, matricespath):
     ## --localmem = 128 \
     cmd = f"""cellranger count --id={sample} \
+--localcores={core} \
 --transcriptome={db} \
 --fastqs={fq_dir} \
 --sample={sample} \
---expect-cells={expectcellnum} \
---nosecondary"""
+--expect-cells={expectcellnum}"""
     print("\033[1;33m Running command for sample {}:\033[0m".format(sample))
     print("\033[1;31m{}\033[0m".format(cmd))
     subprocess.run(cmd, shell=True)
     if matricespath != "":
         mv_cmd = ["mv", f"{sample}", f"{matricespath}"]
         subprocess.run(mv_cmd, check=True)
         
@@ -130,20 +149,26 @@
             sample_id = filename.split("_")[0]
             # 剔除掉已存在的处理好的文件夹
             if matricespath != "":
                 sample_dir = os.path.join(matricespath, sample_id)
                 if not os.path.isdir(sample_dir):
                     samples.add(sample_id)
     print(samples)
-
-    num_threads = int(get_num_threads() / 10)
-
+    
+    folder_count = len(samples)
+    
+    for i in range(1, min(folder_count + 1, 21)):
+        if folder_count % i == 0:
+            max_workers = i
+    
+    num_threads = max_workers
+    core = 100 // num_threads
     # 调用函数
     with ThreadPoolExecutor(max_workers=num_threads) as executor:
-        futures = {executor.submit(run_cellranger, sample, db, fq_dir,
+        futures = {executor.submit(run_cellranger, sample, core, db, fq_dir,
                                 expectcellnum, matricespath): sample for sample in samples}
         for future in concurrent.futures.as_completed(futures):
             sample = futures[future]
             try:
                 future.result()
                 print(f"Sample {sample} completed successfully.")
             except Exception as e:
@@ -169,24 +194,27 @@
 
     for folder in os.listdir(matrices_base):
         src_folder = os.path.join(matrices_base, folder)
 
         if os.path.isdir(src_folder):
             src_file = os.path.join(src_folder, 'outs', 'web_summary.html')
             src_matrix_folder = os.path.join(
-                src_folder, 'outs', 'raw_feature_bc_matrix')
+                src_folder, 'outs', 'filtered_feature_bc_matrix')
             matrixh5flie = os.path.join(
                 src_folder, 'outs', 'filtered_feature_bc_matrix.h5')
 
             if os.path.exists(src_file):
                 dst_file = os.path.join(summary_base, folder + '.html')
-                shutil.copy2(src_file, dst_file)
+                if not os.path.exists(dst_file):
+                    shutil.copy2(src_file, dst_file)
                 
             if os.path.exists(src_matrix_folder):
                 dst_matrix_folder = os.path.join(matrix_base, folder)
-                shutil.copytree(src_matrix_folder, dst_matrix_folder)
+                if not os.path.exists(dst_matrix_folder):
+                    shutil.copytree(src_matrix_folder, dst_matrix_folder)
             
             if os.path.exists(matrixh5flie):
                 dst_matrixh5_folder = os.path.join(matrixh5_base, folder)
-                shutil.copy2(matrixh5flie, dst_matrixh5_folder)
+                if not os.path.exists(dst_matrixh5_folder):
+                    shutil.copy2(matrixh5flie, dst_matrixh5_folder)
     
     print("\033[1;32m All output results have been organized.\033[0m")
```

### Comparing `easybio-0.3.1/easyBio/Utils/netUtils.py` & `easybio-0.3.2/easyBio/Utils/netUtils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+# Author: Lei
+# Date: 2023-04-20
+# Description:
 import time
 import requests
 
 
 def defineSession():
     """
     This function defines and returns a new `requests.Session` object.
```

### Comparing `easybio-0.3.1/easyBio/Utils/toolsUtils.py` & `easybio-0.3.2/easyBio/Utils/toolsUtils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+# Author: Lei
+# Date: 2023-04-20
+# Description:
 import datetime
 import multiprocessing
 import os
 
 
 def del_files(dir_path):
     if os.path.isfile(dir_path):
```

### Comparing `easybio-0.3.1/easyBio/changeSRAName.py` & `easybio-0.3.2/easyBio/changeSRAName.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+# Author: Lei
+# Date: 2023-04-20
+# Description:
 import argparse
 from collections import defaultdict
 import os
 import re
 
 
 def renames1(folder_path):
@@ -75,18 +79,53 @@
 
             new_name = f"SRR{name}_S1_L00{lane_number}_{read_type}_001.fastq.gz"
             os.rename(os.path.join(folder_path, file),
                       os.path.join(folder_path, new_name))
             print(f'Renamed {file} to {new_name}')
 
 
+
+def rename_files2(files, folder_path, mapping, srr_counts):
+    name_add_mapping = {}
+    name_add_srr_mapping = {}
+    for file in files:
+        srr_match = re.match(r'(SRR\d+)_(\d)', file)
+        if srr_match:
+            srr, number = srr_match.groups()
+            name = mapping[srr]
+            read_type = ''
+            if srr_counts[srr] == 2:
+                read_type = 'R1' if number == '1' else 'R2'
+            elif srr_counts[srr] == 3:
+                read_type = 'I1' if number == '1' else (
+                    'R1' if number == '2' else 'R2')
+
+            if srr in name_add_srr_mapping:
+                lane_number = name_add_srr_mapping[srr]
+            else:
+                name_add_mapping[name] = name_add_mapping.get(name, 0) + 1
+                name_add_srr_mapping[srr] = name_add_mapping[name]
+                lane_number = name_add_srr_mapping[srr]
+
+            new_name = f"SRR{name}_S{lane_number}_L001_{read_type}_001.fastq.gz"
+            os.rename(os.path.join(folder_path, file),
+                      os.path.join(folder_path, new_name))
+            print(f'Renamed {file} to {new_name}')
+
+
 def renames2(list_file, folder_path):
     mapping = read_mapping_file(list_file)
     files, srr_counts = count_srr_occurrences(folder_path)
     rename_files(files, folder_path, mapping, srr_counts)
+    
+
+def renames3(list_file, folder_path):
+    mapping = read_mapping_file(list_file)
+    files, srr_counts = count_srr_occurrences(folder_path)
+    rename_files2(files, folder_path, mapping, srr_counts)
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Process list_file and folder_path")
     parser.add_argument("-l", "--list_file", help="matching list")
     parser.add_argument("-f", "--folder_path", default=os.getcwd(),
@@ -97,15 +136,16 @@
     list_file = args.list_file
     folder_path = args.folder_path
     
     print("\033[1;32m list_file:\033[0m \033[32m{}\033[0m".format(list_file))
     print("\033[1;32m folder_path:\033[0m \033[32m{}\033[0m".format(folder_path))
     
     if list_file:
-        renames2(list_file, folder_path)
+        # renames2(list_file, folder_path)
+        renames3(list_file, folder_path)
     else:
         renames1(folder_path)
     print("\033[1;32m Rename completed\033[0m")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `easybio-0.3.1/easyBio/downloadSRA.py` & `easybio-0.3.2/easyBio/downloadSRA.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+# Author: Lei
+# Date: 2023-04-20
+# Description:
 import argparse
 import os
 
 from .Utils import downLoadSRA
 from .Utils import get_num_threads
```

### Comparing `easybio-0.3.1/easyBio/pipline.py` & `easybio-0.3.2/easyBio/pipline.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,26 @@
+# -*- coding: utf-8 -*-
+# Author: Lei
+# Date: 2023-04-20
+# Description:
 import os
 
 from .Utils import tidySummary
 from .Utils import get_num_threads
 
-from .changeSRAName import renames1, renames2
-from .Utils import check_file_exists, cellrangerRun, splitSRAfun, downLoadSRA
+from .changeSRAName import renames1, renames2, renames3
+from .Utils import check_file_exists, cellrangerRun, splitSRAfun, downLoadSRA, cellrangerRun2
 import argparse
 
+
+# def writeLog(logname, logcontent):
+#     with open(f"{logFiles}/{logname}", 'w') as file:
+#         file.write(logcontent)
+
+
 def main():
     num_threads = get_num_threads()
 
     # Set up argument parser
     parser = argparse.ArgumentParser(
         description="Process GSE number, directory and threads")
     parser.add_argument("-g", "--gsenumber", help="GSE number")
@@ -34,14 +44,17 @@
     threads = args.threads
     kind = args.kind
     db_path = args.db_path
     expectcellnum = args.expectcellnum
     list_file = args.list_file
 
     rawdirs = f"{dirs}/{gsenumber}/raw"
+    # logdirs = f"{rawdirs}/log"
+
+    # os.makedirs(logdirs, exist_ok=True)
 
     # 下载 SRA 数据
     downLoadSRA(gsenumber, dirs, threads)
 
     print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
 
 
@@ -60,15 +73,15 @@
     if file_exists:
         print(f"fastq文件已进行改名")
     else:
         splitSRAfun(folder, fqfiles, threads, kind)
         
         print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
         if list_file:
-            renames2(list_file, fqfiles)
+            renames3(list_file, fqfiles)
         else:
             renames1(fqfiles)
         print("\033[1;32m Rename completed\033[0m")
 
     print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
     matricespath = f"{rawdirs}/matrices"
     os.makedirs(matricespath, exist_ok=True)
```

### Comparing `easybio-0.3.1/easyBio/run_cellranger.py` & `easybio-0.3.2/easyBio/run_cellranger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+# -*- coding: utf-8 -*-
+# Author: Lei
+# Date: 2023-04-20
+# Description:
 import argparse
 
-from .Utils import cellrangerRun
+from .Utils import cellrangerRun, cellrangerRun2
 
 
 def main():
     parser = argparse.ArgumentParser(
             description="A script that processes input arguments.")
     
     parser.add_argument("-db", "--db_path", required=True,
```

### Comparing `easybio-0.3.1/easyBio/splitSRA.py` & `easybio-0.3.2/easyBio/splitSRA.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import os
 from pathlib import Path
 
 from .Utils import splitSRAfun
-from .Utils import createDir, get_num_threads
+from .Utils import get_num_threads
 
 def main():
     num_threads = get_num_threads()
    # Parse command line arguments
     parser = argparse.ArgumentParser(
         description="Process .sra files with parallel-fastq-dump")
     parser.add_argument("-f", "--folder", default=".",
```

### Comparing `easybio-0.3.1/easybio.egg-info/PKG-INFO` & `easybio-0.3.2/easybio.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybio
-Version: 0.3.1
+Version: 0.3.2
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
@@ -12,7 +12,9 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 
 # easyBio_conda
 easyBio_conda
+
+
```

### Comparing `easybio-0.3.1/easybio.egg-info/SOURCES.txt` & `easybio-0.3.2/easybio.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 easyBio/__init__.py
 easyBio/changeSRAName.py
 easyBio/downloadSRA.py
 easyBio/easyBio.py
 easyBio/pipline.py
 easyBio/run_cellranger.py
 easyBio/run_test.py
+easyBio/runvelocyto.py
 easyBio/splitSRA.py
+easyBio/test.py
+easyBio/velocyto2.py
+easyBio/velocyto3.py
 easyBio/Utils/__init__.py
 easyBio/Utils/download.py
 easyBio/Utils/downloadUtils.py
 easyBio/Utils/easyBioUtils.py
 easyBio/Utils/netUtils.py
 easyBio/Utils/toolsUtils.py
 easybio.egg-info/PKG-INFO
```

### Comparing `easybio-0.3.1/setup.py` & `easybio-0.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
-VERSION = '0.3.1'
+VERSION = '0.3.2'
 
 setup(
     name='easybio',  # package name
     version=VERSION,  # package version
     author='Lei Cui',
     author_email='cuilei798@qq.com',
     maintainer='Lei Cui',
@@ -21,22 +21,22 @@
     entry_points={
         'console_scripts': [
             'easyBio=easyBio.easyBio:main',
             'easydownloadSRA=easyBio.downloadSRA:main',
             'easysplitSRA=easyBio.splitSRA:main',
             'easychangeSRAName=easyBio.changeSRAName:main',
             'easycellranger=easyBio.run_cellranger:main',
-            'easyscGEOpipline=easyBio.pipline:main',
+            'easyscGEOpipline=easyBio.pipline:main', 
+            'easyVelocyto=easyBio.runvelocyto:main',
         ]
     },
     install_requires=[
         # 'biopython',
         'threadpool',
-        'requests',
-        'argparse'
+        'requests'
         # Add more dependencies here
     ],
     package_data={
         'Utils': ['Utils/*']
     },
     classifiers=[
         'Operating System :: OS Independent',
```

