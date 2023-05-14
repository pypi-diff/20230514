# Comparing `tmp/histcite-python-0.2.0.tar.gz` & `tmp/histcite-python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcite-python-0.2.0.tar", last modified: Fri May 12 07:25:54 2023, max compression
+gzip compressed data, was "histcite-python-0.2.1.tar", last modified: Sun May 14 15:19:05 2023, max compression
```

## Comparing `histcite-python-0.2.0.tar` & `histcite-python-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:25:54.777446 histcite-python-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 07:25:37.000000 histcite-python-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-05-12 07:25:54.777446 histcite-python-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-05-12 07:25:37.000000 histcite-python-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:25:54.773446 histcite-python-0.2.0/histcite/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/parse_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-12 07:25:37.000000 histcite-python-0.2.0/histcite/recognize_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:25:54.773446 histcite-python-0.2.0/histcite_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-05-12 07:25:54.000000 histcite-python-0.2.0/histcite_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-12 07:25:54.000000 histcite-python-0.2.0/histcite_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:25:54.000000 histcite-python-0.2.0/histcite_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 07:25:54.000000 histcite-python-0.2.0/histcite_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 07:25:54.000000 histcite-python-0.2.0/histcite_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 07:25:54.000000 histcite-python-0.2.0/histcite_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 07:25:54.777446 histcite-python-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-12 07:25:37.000000 histcite-python-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:25:54.777446 histcite-python-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-12 07:25:37.000000 histcite-python-0.2.0/tests/test_compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-12 07:25:37.000000 histcite-python-0.2.0/tests/test_network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-12 07:25:37.000000 histcite-python-0.2.0/tests/test_parse_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:19:05.536476 histcite-python-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-14 15:18:51.000000 histcite-python-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-14 15:19:05.536476 histcite-python-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-14 15:18:51.000000 histcite-python-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:19:05.532476 histcite-python-0.2.1/histcite/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/parse_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-14 15:18:51.000000 histcite-python-0.2.1/histcite/recognize_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:19:05.536476 histcite-python-0.2.1/histcite_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-14 15:19:05.000000 histcite-python-0.2.1/histcite_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-14 15:19:05.000000 histcite-python-0.2.1/histcite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:19:05.000000 histcite-python-0.2.1/histcite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 15:19:05.000000 histcite-python-0.2.1/histcite_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 15:19:05.000000 histcite-python-0.2.1/histcite_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-14 15:19:05.000000 histcite-python-0.2.1/histcite_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:19:05.536476 histcite-python-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-14 15:18:51.000000 histcite-python-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:19:05.536476 histcite-python-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-14 15:18:51.000000 histcite-python-0.2.1/tests/test_compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-14 15:18:51.000000 histcite-python-0.2.1/tests/test_network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-14 15:18:51.000000 histcite-python-0.2.1/tests/test_parse_reference.py
```

### Comparing `histcite-python-0.2.0/LICENSE` & `histcite-python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `histcite-python-0.2.0/PKG-INFO` & `histcite-python-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Intended Audience :: Developers
@@ -129,15 +129,15 @@
 | 是否开源 | 是 | 否 |
 | 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 
 ## Q&A
 1、如何识别引文关系？  
-`Web of Science:` 每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` ，则判断 `一作`、`发表年份`、`期刊名称`、`期次` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用。  
+`Web of Science:` 每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` ，则判断 `一作`、`发表年份`、`文献来源`、`开始页` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用。  
 `CSSCI:` 通过 `一作 `和 `题名` 两个字段进行判断。  
 
 2、如何去重？  
 `Web of Science:` 按照 `UT` 入藏号字段进行去重。  
 `CSSCI:` 按照 `一作` 和 `题名` 两个字段进行去重。
 
 ## TODO
```

### Comparing `histcite-python-0.2.0/README.md` & `histcite-python-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 | 是否开源 | 是 | 否 |
 | 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 
 ## Q&A
 1、如何识别引文关系？  
-`Web of Science:` 每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` ，则判断 `一作`、`发表年份`、`期刊名称`、`期次` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用。  
+`Web of Science:` 每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` ，则判断 `一作`、`发表年份`、`文献来源`、`开始页` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用。  
 `CSSCI:` 通过 `一作 `和 `题名` 两个字段进行判断。  
 
 2、如何去重？  
 `Web of Science:` 按照 `UT` 入藏号字段进行去重。  
 `CSSCI:` 按照 `一作` 和 `题名` 两个字段进行去重。
 
 ## TODO
```

### Comparing `histcite-python-0.2.0/histcite/cli.py` & `histcite-python-0.2.1/histcite/cli.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.2.0/histcite/compute_metrics.py` & `histcite-python-0.2.1/histcite/compute_metrics.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.2.0/histcite/network_graph.py` & `histcite-python-0.2.1/histcite/network_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,24 @@
     def __init__(self,docs_table:pd.DataFrame,source_type:str):
         self.docs_table = docs_table
         self.source_type = source_type
         self.year_empty_index = set(docs_table[docs_table['PY'].isna()].index)
 
     def __obtain_groups(self):
         """obtain groups of docs by year"""
-
         year_series = self.docs_table.loc[self.node_list,'PY']
         groups = year_series.groupby(year_series)
         year_list = [i[0] for i in groups]
         grouped_doc_index = [i[1].index.tolist() for i in groups]
         self.year_list = year_list
         for idx,year in enumerate(year_list):
             grouped_doc_index[idx].insert(0,year)
         self.grouped_doc_index = grouped_doc_index
     
     def __generate_edge(self,doc_index:int,doc_relation:str,relation_type:str):
-
         # filter docs with empty year
         related_doc_list = [int(i) for i in doc_relation.split(';') if int(i) not in self.year_empty_index]
         if relation_type=='reference':
             return {(doc_index,ref) for ref in related_doc_list}
         elif relation_type=='citation':
             return {(citation,doc_index) for citation in related_doc_list}
         
@@ -54,15 +52,15 @@
         for edge in edge_set:
             edge_list[edge[0]].append(edge[1])
 
         return edge_list
         
     def generate_dot_file(self,doc_indices,allow_external_node=False):
         """生成dot文件
-        doc_indices: 文献索引列表;
+        doc_indices: 文献索引列表\n
         allow_external_node: 是否允许出现doc_indices之外的节点，默认False
         """
         self.doc_indices = [i for i in doc_indices if i not in self.year_empty_index]
         self.allow_external_node = allow_external_node
 
         raw_edge_list = self.__generate_edge_list()
         self.__obtain_groups()
```

### Comparing `histcite-python-0.2.0/histcite/parse_reference.py` & `histcite-python-0.2.1/histcite/parse_reference.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             self.cr_count = len(self.cr_list)
         except AttributeError:
             self.cr_count = 0
         self.doc_index = doc_index
         self.source_type = source_type
 
     @staticmethod
-    def __parse_wos_cr(cr):
+    def _parse_wos_cr(cr):
         """Parse a single citation record"""
         AU,PY,J9,VL,BP,DI = None,None,None,None,None,None
         cr_data = {}
 
         try:
             AU,PY,J9,other = re.split(r', (?![^\[\]]*\])',cr,3)
         except ValueError:
@@ -65,50 +65,58 @@
             cr_data['J9'] = J9
             cr_data['VL'] = VL 
             cr_data['BP'] = BP 
             cr_data['DI'] = DI 
             return cr_data
     
     @staticmethod
-    def __parse_cssci_cr(cr):
+    def _parse_cssci_cr(cr):
 
+        pattern = re.compile(r'(?<!\d)\.(?!\d)|(?<=\d)\.(?!\d)|(?<!\d)\.(?=\d)|(?<=\d{4})\.(?=\d{4})')
         # 中文参考文献
         if re.search(r'[\u4e00-\u9fa5]',cr):
             try:
-                _,AU,TI,_ = cr.split('.',3)
+                # _,AU,TI,_ = cr.split('.',3)
+                _,AU,TI,_ = pattern.split(cr,3)
                 if ',' not in AU:
                     return {'first_AU':AU,'TI':TI}
             except ValueError:
                 return None
     
         # 英文参考文献
         else:
-            if AU := re.search(r'^\d+\.(.*?)\.[A-Z]+[a-z]+',cr):
-                AU = AU.group(1)
+            if index_AU := re.search(r'^(\d+\.(.*?))\.[A-Za-z"“\d]{1}[a-zA-Z\s\d]+',cr):
+                AU = index_AU.group(2)
                 if AU !='':
-                    other = cr.replace(f'{AU}.','')
+                    # other = cr.replace(f'{AU}.','')
+                    other = cr.replace(index_AU.group(1),'')
                     try:
-                        _,TI,_ = other.split('.',2)
+                        # _,TI,_ = other.split('.',2)
+                        _,TI,_ = pattern.split(other,2)
                         return {'first_AU':AU,'TI':TI}
                     except ValueError:
                         return None
                         
                 else:
-                    _,_,TI,_ = cr.split('.',3)
-                    return {'first_AU':AU,'TI':TI}
-            
+                    try:
+                        _,_,TI,_ = pattern.split(cr,3)
+                    except ValueError:
+                        _,_,TI,_ = cr.split('.',3)
+                    finally:
+                        return {'first_AU':AU,'TI':TI} # type:ignore
+                     
     def parse_cr_cell(self):
         if self.cr_count == 0:
             return None
         
         if self.source_type == "wos":
-            parsed_cr_list = [self.__parse_wos_cr(i) for i in self.cr_list]
+            parsed_cr_list = [self._parse_wos_cr(i) for i in self.cr_list]
             keys = ['first_AU','PY','J9','VL','BP','DI']
         elif self.source_type == "cssci":
-            parsed_cr_list = [self.__parse_cssci_cr(i) for i in self.cr_list]
+            parsed_cr_list = [self._parse_cssci_cr(i) for i in self.cr_list]
             keys = ['first_AU','TI']
         else:
             raise ValueError()
         
         result = {key:[] for key in keys}
         for single in parsed_cr_list:
             if single is not None:
```

### Comparing `histcite-python-0.2.0/histcite/process_file.py` & `histcite-python-0.2.1/histcite/process_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,15 @@
             self.file_name_list = [i for i in os.listdir(folder_path) if i[:9]=='savedrecs']
         elif source_type=='cssci':
             self.file_name_list = [i for i in os.listdir(folder_path) if i[:3]=='LY_']
         else:
             raise ValueError('Invalid source type')
         
     def _read_wos_file(self,file_name:str)->pd.DataFrame:
-        """读取表单，返回dataframe"""
-
+        """读取wos表单"""
         use_cols = ['AU','TI','SO','DT','CR','DE','C3','NR','TC','Z9','J9','PY','VL','BP','DI','UT']
         file_path = os.path.join(self.folder_path,file_name)
         try:
             df = pd.read_csv(
                 file_path,sep='\t',
                 header=0,
                 on_bad_lines='skip',
@@ -56,14 +55,15 @@
             
             # 提取一作
             first_au = df['AU'].apply(ProcessWosFile.extract_first_author)
             df.insert(1,'first_AU',first_au)
             return df
         
     def _read_cssci_file(self,file_name:str)->pd.DataFrame:
+        """读取cssci文本文件"""
         file_path = os.path.join(self.folder_path,file_name)
         with open(file_path,'r') as f:
             text = f.read()
         
         if text[:16] != '南京大学中国社会科学研究评价中心':
             raise ValueError(f'File {file_name} is not a valid cssci file')
         body_text = text.split('\n\n\n',1)[1]
```

### Comparing `histcite-python-0.2.0/histcite/recognize_reference.py` & `histcite-python-0.2.1/histcite/recognize_reference.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.2.0/histcite_python.egg-info/PKG-INFO` & `histcite-python-0.2.1/histcite_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Intended Audience :: Developers
@@ -129,15 +129,15 @@
 | 是否开源 | 是 | 否 |
 | 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 
 ## Q&A
 1、如何识别引文关系？  
-`Web of Science:` 每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` ，则判断 `一作`、`发表年份`、`期刊名称`、`期次` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用。  
+`Web of Science:` 每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` ，则判断 `一作`、`发表年份`、`文献来源`、`开始页` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用。  
 `CSSCI:` 通过 `一作 `和 `题名` 两个字段进行判断。  
 
 2、如何去重？  
 `Web of Science:` 按照 `UT` 入藏号字段进行去重。  
 `CSSCI:` 按照 `一作` 和 `题名` 两个字段进行去重。
 
 ## TODO
```

### Comparing `histcite-python-0.2.0/histcite_python.egg-info/SOURCES.txt` & `histcite-python-0.2.1/histcite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `histcite-python-0.2.0/setup.py` & `histcite-python-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="histcite-python",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.2.0",
+    version="0.2.1",
     description="A Python interface to histcite.",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["histcite","web of science","citation network"],
     license="MIT",
     url="https://github.com/doublessay/histcite-python",
     packages=["histcite"],
```

### Comparing `histcite-python-0.2.0/tests/test_compute_metrics.py` & `histcite-python-0.2.1/tests/test_compute_metrics.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.2.0/tests/test_network_graph.py` & `histcite-python-0.2.1/tests/test_network_graph.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.2.0/tests/test_parse_reference.py` & `histcite-python-0.2.1/tests/test_parse_reference.py`

 * *Files identical despite different names*

