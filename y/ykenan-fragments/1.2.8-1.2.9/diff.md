# Comparing `tmp/ykenan_fragments-1.2.8.tar.gz` & `tmp/ykenan_fragments-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_fragments-1.2.8.tar", last modified: Fri May 12 02:30:31 2023, max compression
+gzip compressed data, was "ykenan_fragments-1.2.9.tar", last modified: Fri May 12 05:26:20 2023, max compression
```

## Comparing `ykenan_fragments-1.2.8.tar` & `ykenan_fragments-1.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 02:30:31.559351 ykenan_fragments-1.2.8/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.2.8/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0      971 2023-05-12 02:30:31.559351 ykenan_fragments-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.8/README.md
--rw-rw-rw-   0        0        0      775 2023-05-12 02:21:10.000000 ykenan_fragments-1.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       52 2023-05-12 02:21:10.000000 ykenan_fragments-1.2.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 02:30:31.559351 ykenan_fragments-1.2.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 02:30:31.497350 ykenan_fragments-1.2.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-12 02:30:31.531352 ykenan_fragments-1.2.8/src/ykenan_fragments/
--rw-rw-rw-   0        0        0     2012 2023-05-12 02:02:30.000000 ykenan_fragments-1.2.8/src/ykenan_fragments/__init__.py
--rw-rw-rw-   0        0        0     5383 2023-05-12 02:02:30.000000 ykenan_fragments-1.2.8/src/ykenan_fragments/genome_transformation.py
--rw-rw-rw-   0        0        0    15901 2023-05-12 02:02:30.000000 ykenan_fragments-1.2.8/src/ykenan_fragments/get_fragments.py
--rw-rw-rw-   0        0        0    14835 2023-05-12 02:02:30.000000 ykenan_fragments-1.2.8/src/ykenan_fragments/get_sort_fragments.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:30:31.558353 ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/
--rw-rw-rw-   0        0        0      971 2023-05-12 02:30:31.000000 ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-05-12 02:30:31.000000 ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 02:30:31.000000 ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-12 02:30:31.000000 ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-12 02:30:31.000000 ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 05:26:20.518996 ykenan_fragments-1.2.9/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      971 2023-05-12 05:26:20.505997 ykenan_fragments-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.9/README.md
+-rw-rw-rw-   0        0        0      775 2023-05-12 05:13:08.000000 ykenan_fragments-1.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       52 2023-05-12 02:21:10.000000 ykenan_fragments-1.2.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 05:26:20.519998 ykenan_fragments-1.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 05:26:20.448996 ykenan_fragments-1.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 05:26:20.483997 ykenan_fragments-1.2.9/src/ykenan_fragments/
+-rw-rw-rw-   0        0        0     2012 2023-05-12 02:02:30.000000 ykenan_fragments-1.2.9/src/ykenan_fragments/__init__.py
+-rw-rw-rw-   0        0        0     5383 2023-05-12 02:02:30.000000 ykenan_fragments-1.2.9/src/ykenan_fragments/genome_transformation.py
+-rw-rw-rw-   0        0        0    16533 2023-05-12 05:13:08.000000 ykenan_fragments-1.2.9/src/ykenan_fragments/get_fragments.py
+-rw-rw-rw-   0        0        0    14835 2023-05-12 02:02:30.000000 ykenan_fragments-1.2.9/src/ykenan_fragments/get_sort_fragments.py
+drwxrwxrwx   0        0        0        0 2023-05-12 05:26:20.504996 ykenan_fragments-1.2.9/src/ykenan_fragments.egg-info/
+-rw-rw-rw-   0        0        0      971 2023-05-12 05:26:20.000000 ykenan_fragments-1.2.9/src/ykenan_fragments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-05-12 05:26:20.000000 ykenan_fragments-1.2.9/src/ykenan_fragments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 05:26:20.000000 ykenan_fragments-1.2.9/src/ykenan_fragments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-12 05:26:20.000000 ykenan_fragments-1.2.9/src/ykenan_fragments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-12 05:26:20.000000 ykenan_fragments-1.2.9/src/ykenan_fragments.egg-info/top_level.txt
```

### Comparing `ykenan_fragments-1.2.8/LICENSE` & `ykenan_fragments-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.8/PKG-INFO` & `ykenan_fragments-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_fragments
-Version: 1.2.8
+Version: 1.2.9
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_fragments-1.2.8/pyproject.toml` & `ykenan_fragments-1.2.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.11", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_fragments"
-version = "1.2.8"
+version = "1.2.9"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "fragments"]
 description = "Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ykenan_fragments-1.2.8/src/ykenan_fragments/__init__.py` & `ykenan_fragments-1.2.9/src/ykenan_fragments/__init__.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.8/src/ykenan_fragments/genome_transformation.py` & `ykenan_fragments-1.2.9/src/ykenan_fragments/genome_transformation.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.8/src/ykenan_fragments/get_fragments.py` & `ykenan_fragments-1.2.9/src/ykenan_fragments/get_fragments.py`

 * *Files 5% similar despite different names*

```diff
@@ -176,35 +176,40 @@
             # 解压文件得到内容
             return self.file.unzip_gz(file["path"], generate_file=txt_file)
 
     def fragments_file_name(self, key: str) -> str:
         return f"{key}{self.suffix_fragments}"
 
     @staticmethod
-    def judge_mtx_is_true(one_len: str, two_len: str, peaks_len: int, barcodes_len: int) -> bool:
-        return int(one_len) + 1 != peaks_len and int(two_len) + 1 != barcodes_len
+    def judge_mtx_is_true(one_len: str, two_len: str, peaks_len: int, barcodes_len: int) -> int:
+        if int(one_len) != peaks_len and int(two_len) != barcodes_len:
+            return 0
+        elif int(one_len) != barcodes_len and int(two_len) != peaks_len:
+            return 1
+        else:
+            return -1
 
     @staticmethod
-    def get_peaks(dict_: dict, index_: str) -> str:
-        peak: str = dict_[int(index_)]
+    def get_peaks(dict_: dict, index_: int) -> str:
+        peak: str = dict_[index_]
         peak_split = peak.split("_")
         return f"{peak_split[0]}\t{peak_split[1]}\t{peak_split[2]}"
 
     @staticmethod
-    def get_barcodes(dict_: dict, index_: str) -> str:
-        barcode: str = dict_[int(index_)]
+    def get_barcodes(dict_: dict, index_: int) -> str:
+        barcode: str = dict_[index_]
         return barcode.split("\t")[6]
 
     @staticmethod
-    def get_input_peaks(dict_: dict, index_: str) -> str:
-        return dict_[int(index_)]
+    def get_input_peaks(dict_: dict, index_: int) -> str:
+        return dict_[index_]
 
     @staticmethod
-    def get_input_barcodes(dict_: dict, index_: str) -> str:
-        return dict_[int(index_)]
+    def get_input_barcodes(dict_: dict, index_: int) -> str:
+        return dict_[index_]
 
     def write_fragments(self, param: list) -> None:
         """
         Form fragments file
         :return:
         """
         path: str = param[0]
@@ -232,55 +237,60 @@
         peaks_dict: dict = dict(zip(list(range(peaks_len)), peaks))
 
         self.log.info(f"Quantity or Path {self.barcodes_key}: {barcodes_len}, {self.mtx_key}: {mtx_path}, {self.peaks_key}: {peaks_len}")
         # Read quantity
         mtx_count: int = 0
         error_count: int = 0
         mtx_all_number: int = 0
+        is_peaks_barcodes: int = -1
         # create a file
         fragments_file: str = os.path.join(path, self.fragments_file_name(key))
         self.log.info(f"Starting to form {mtx_path} fragments file")
         with open(fragments_file, "w", encoding="utf-8", buffering=1, newline="\n") as w:
             with open(mtx_path, "r", encoding="utf-8") as r:
                 line: str = r.readline().strip()
                 if line.startswith("%"):
                     self.log.info(f"Annotation Information: {line}")
                 line: str = r.readline().strip()
                 split: list = line.split(" ")
                 if len(split) == 3 and line:
                     self.log.info(f"Remove Statistical Rows: {line}")
                     mtx_all_number = int(split[2])
-                    if self.judge_mtx_is_true(split[0], split[1], peaks_len, barcodes_len):
+                    is_peaks_barcodes = self.judge_mtx_is_true(split[0], split[1], peaks_len, barcodes_len)
+                    if is_peaks_barcodes == -1:
                         raise ValueError(f"File mismatch {self.peaks_key}: {int(split[0])} {peaks_len}, {self.barcodes_key}: {int(split[1])} {barcodes_len}")
                 while True:
                     line: str = r.readline().strip()
                     if not line:
                         break
                     if mtx_count >= 500000 and mtx_count % 500000 == 0:
                         self.log.info(f"Processed {mtx_count} lines, completed {round(mtx_count / mtx_all_number, 4) * 100} %")
                     split: list = line.split(" ")
+                    split_peak_index: int = int(split[0]) if is_peaks_barcodes == 0 else int(split[1])
+                    split_barcode_index: int = int(split[1]) if is_peaks_barcodes == 0 else int(split[0])
                     # To determine the removal of a length of not 3
                     if len(split) != 3:
                         mtx_count += 1
                         error_count += 1
                         self.log.error(f"mtx information ===> content: {split}, line number: {mtx_count}")
                         continue
-                    if int(split[0]) > peaks_len or int(split[1]) > barcodes_len:
+                    if split_peak_index > peaks_len or split_barcode_index > barcodes_len:
+                        self.log.warn(f"{self.mtx_key} file 中出现 {split_peak_index} > {peaks_len} or {split_barcode_index} > {barcodes_len}")
                         mtx_count += 1
                         continue
                     # peak, barcode, There is a header+1, but the index starts from 0 and the record starts from 1
-                    peak_info: str = self.get_peaks(peaks_dict, split[0])
-                    barcode_info: str = self.get_barcodes(barcodes_dict, split[1])
+                    peak_info: str = self.get_peaks(peaks_dict, split_peak_index)
+                    barcode_info: str = self.get_barcodes(barcodes_dict, split_barcode_index)
                     # Adding information, it was found that some files in mtx contain two columns, less than three columns. This line was ignored and recorded in the log
                     try:
                         w.write(f"{peak_info}\t{barcode_info}\t{split[2]}\n")
                     except Exception as e:
                         error_count += 1
-                        self.log.error(f"peak information: {self.get_input_peaks(peaks_dict, split[0])}")
-                        self.log.error(f"barcodes information: {self.get_input_barcodes(barcodes_dict, split[1])}")
+                        self.log.error(f"peak information: {self.get_input_peaks(peaks_dict, split_peak_index)}")
+                        self.log.error(f"barcodes information: {self.get_input_barcodes(barcodes_dict, split_barcode_index)}")
                         self.log.error(f"mtx information ===> content: {split}, line number: {mtx_count}")
                         self.log.error(f"Write error: {e}")
                     mtx_count += 1
         self.log.info(f"The number of rows ignored is {error_count}, {round(error_count / mtx_all_number, 4) * 100} % of total")
         self.log.info(f"Complete the formation of {mtx_path} fragments file")
         self.log.info(f"Complete processing of {key} related files (folders)")
```

### Comparing `ykenan_fragments-1.2.8/src/ykenan_fragments/get_sort_fragments.py` & `ykenan_fragments-1.2.9/src/ykenan_fragments/get_sort_fragments.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/PKG-INFO` & `ykenan_fragments-1.2.9/src/ykenan_fragments.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-fragments
-Version: 1.2.8
+Version: 1.2.9
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

