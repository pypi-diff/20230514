# Comparing `tmp/shareddata-2.0.8.tar.gz` & `tmp/shareddata-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.0.8.tar", last modified: Tue May  9 14:12:37 2023, max compression
+gzip compressed data, was "shareddata-2.0.9.tar", last modified: Tue May  9 14:25:32 2023, max compression
```

## Comparing `shareddata-2.0.8.tar` & `shareddata-2.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 14:12:37.527450 shareddata-2.0.8/
--rw-rw-rw-   0        0        0    35823 2023-01-12 20:44:38.000000 shareddata-2.0.8/LICENSE
--rw-rw-rw-   0        0        0     1100 2023-05-09 14:12:37.528450 shareddata-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      530 2023-05-07 14:43:50.000000 shareddata-2.0.8/README.md
--rw-rw-rw-   0        0        0      108 2023-01-12 20:44:38.000000 shareddata-2.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      906 2023-05-09 14:12:37.531451 shareddata-2.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 14:12:37.508445 shareddata-2.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 14:12:37.520450 shareddata-2.0.8/src/SharedData/
--rw-rw-rw-   0        0        0     1562 2023-04-11 20:53:38.000000 shareddata-2.0.8/src/SharedData/Defaults.py
--rw-rw-rw-   0        0        0     4735 2023-01-16 18:59:43.000000 shareddata-2.0.8/src/SharedData/Logger.py
--rw-rw-rw-   0        0        0     1275 2023-02-17 15:06:53.000000 shareddata-2.0.8/src/SharedData/LoggerConsumerProcess.py
--rw-rw-rw-   0        0        0    11544 2023-05-07 12:00:04.000000 shareddata-2.0.8/src/SharedData/Metadata.py
--rw-rw-rw-   0        0        0     3862 2023-01-12 20:44:38.000000 shareddata-2.0.8/src/SharedData/MultiProc.py
--rw-rw-rw-   0        0        0     5182 2023-01-12 20:44:38.000000 shareddata-2.0.8/src/SharedData/SeriesLib.py
--rw-rw-rw-   0        0        0     3085 2023-03-02 10:46:06.000000 shareddata-2.0.8/src/SharedData/SharedData.py
--rw-rw-rw-   0        0        0    14573 2023-02-27 22:09:20.000000 shareddata-2.0.8/src/SharedData/SharedDataAWSKinesis.py
--rw-rw-rw-   0        0        0     4586 2023-05-07 14:46:16.000000 shareddata-2.0.8/src/SharedData/SharedDataAWSS3.py
--rw-rw-rw-   0        0        0     6275 2023-05-04 17:59:07.000000 shareddata-2.0.8/src/SharedData/SharedDataFeeder.py
--rw-rw-rw-   0        0        0    11176 2023-05-07 14:43:48.000000 shareddata-2.0.8/src/SharedData/SharedDataFrame.py
--rw-rw-rw-   0        0        0     5818 2023-03-17 12:56:52.000000 shareddata-2.0.8/src/SharedData/SharedDataPeriod.py
--rw-rw-rw-   0        0        0     3672 2023-01-12 20:44:38.000000 shareddata-2.0.8/src/SharedData/SharedDataRealTime.py
--rw-rw-rw-   0        0        0     2545 2023-01-12 20:44:38.000000 shareddata-2.0.8/src/SharedData/SharedDataRealTimeProcess.py
--rw-rw-rw-   0        0        0    26032 2023-05-09 10:40:45.000000 shareddata-2.0.8/src/SharedData/SharedDataTable.py
--rw-rw-rw-   0        0        0    31232 2023-05-04 13:59:43.000000 shareddata-2.0.8/src/SharedData/SharedDataTableKeys.py
--rw-rw-rw-   0        0        0    17673 2023-05-07 14:43:48.000000 shareddata-2.0.8/src/SharedData/SharedDataTimeSeries.py
--rw-rw-rw-   0        0        0     7221 2023-05-09 14:12:01.000000 shareddata-2.0.8/src/SharedData/SharedNumpy.py
--rw-rw-rw-   0        0        0        0 2023-01-12 20:44:38.000000 shareddata-2.0.8/src/SharedData/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 14:12:37.527450 shareddata-2.0.8/src/shareddata.egg-info/
--rw-rw-rw-   0        0        0     1100 2023-05-09 14:12:37.000000 shareddata-2.0.8/src/shareddata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2023-05-09 14:12:37.000000 shareddata-2.0.8/src/shareddata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 14:12:37.000000 shareddata-2.0.8/src/shareddata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-05-09 14:12:37.000000 shareddata-2.0.8/src/shareddata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 14:12:37.000000 shareddata-2.0.8/src/shareddata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 14:25:32.461357 shareddata-2.0.9/
+-rw-rw-rw-   0        0        0    35823 2023-01-12 20:44:38.000000 shareddata-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1100 2023-05-09 14:25:32.461357 shareddata-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      530 2023-05-07 14:43:50.000000 shareddata-2.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2023-01-12 20:44:38.000000 shareddata-2.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      906 2023-05-09 14:25:32.462356 shareddata-2.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 14:25:32.432356 shareddata-2.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 14:25:32.450356 shareddata-2.0.9/src/SharedData/
+-rw-rw-rw-   0        0        0     1562 2023-04-11 20:53:38.000000 shareddata-2.0.9/src/SharedData/Defaults.py
+-rw-rw-rw-   0        0        0     4735 2023-01-16 18:59:43.000000 shareddata-2.0.9/src/SharedData/Logger.py
+-rw-rw-rw-   0        0        0     1275 2023-02-17 15:06:53.000000 shareddata-2.0.9/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-rw-   0        0        0    11544 2023-05-07 12:00:04.000000 shareddata-2.0.9/src/SharedData/Metadata.py
+-rw-rw-rw-   0        0        0     3862 2023-01-12 20:44:38.000000 shareddata-2.0.9/src/SharedData/MultiProc.py
+-rw-rw-rw-   0        0        0     5182 2023-01-12 20:44:38.000000 shareddata-2.0.9/src/SharedData/SeriesLib.py
+-rw-rw-rw-   0        0        0     3085 2023-03-02 10:46:06.000000 shareddata-2.0.9/src/SharedData/SharedData.py
+-rw-rw-rw-   0        0        0    14573 2023-02-27 22:09:20.000000 shareddata-2.0.9/src/SharedData/SharedDataAWSKinesis.py
+-rw-rw-rw-   0        0        0     4586 2023-05-07 14:46:16.000000 shareddata-2.0.9/src/SharedData/SharedDataAWSS3.py
+-rw-rw-rw-   0        0        0     6275 2023-05-04 17:59:07.000000 shareddata-2.0.9/src/SharedData/SharedDataFeeder.py
+-rw-rw-rw-   0        0        0    11176 2023-05-07 14:43:48.000000 shareddata-2.0.9/src/SharedData/SharedDataFrame.py
+-rw-rw-rw-   0        0        0     5818 2023-03-17 12:56:52.000000 shareddata-2.0.9/src/SharedData/SharedDataPeriod.py
+-rw-rw-rw-   0        0        0     3672 2023-01-12 20:44:38.000000 shareddata-2.0.9/src/SharedData/SharedDataRealTime.py
+-rw-rw-rw-   0        0        0     2545 2023-01-12 20:44:38.000000 shareddata-2.0.9/src/SharedData/SharedDataRealTimeProcess.py
+-rw-rw-rw-   0        0        0    26032 2023-05-09 10:40:45.000000 shareddata-2.0.9/src/SharedData/SharedDataTable.py
+-rw-rw-rw-   0        0        0    31268 2023-05-09 14:25:12.000000 shareddata-2.0.9/src/SharedData/SharedDataTableKeys.py
+-rw-rw-rw-   0        0        0    17673 2023-05-07 14:43:48.000000 shareddata-2.0.9/src/SharedData/SharedDataTimeSeries.py
+-rw-rw-rw-   0        0        0     7221 2023-05-09 14:12:01.000000 shareddata-2.0.9/src/SharedData/SharedNumpy.py
+-rw-rw-rw-   0        0        0        0 2023-01-12 20:44:38.000000 shareddata-2.0.9/src/SharedData/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:25:32.460358 shareddata-2.0.9/src/shareddata.egg-info/
+-rw-rw-rw-   0        0        0     1100 2023-05-09 14:25:32.000000 shareddata-2.0.9/src/shareddata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2023-05-09 14:25:32.000000 shareddata-2.0.9/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 14:25:32.000000 shareddata-2.0.9/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-05-09 14:25:32.000000 shareddata-2.0.9/src/shareddata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 14:25:32.000000 shareddata-2.0.9/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.0.8/LICENSE` & `shareddata-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/PKG-INFO` & `shareddata-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.0.8
+Version: 2.0.9
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.0.8/README.md` & `shareddata-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/setup.cfg` & `shareddata-2.0.9/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6861 7265 6464 6174 610d 0a76   = shareddata..v
-00000020: 6572 7369 6f6e 203d 2032 2e30 2e38 0d0a  ersion = 2.0.8..
+00000020: 6572 7369 6f6e 203d 2032 2e30 2e39 0d0a  ersion = 2.0.9..
 00000030: 6175 7468 6f72 203d 204a 6f73 6520 4361  author = Jose Ca
 00000040: 726c 6974 6f20 6465 204f 6c69 7665 6972  rlito de Oliveir
 00000050: 6120 4669 6c68 6f0d 0a61 7574 686f 725f  a Filho..author_
 00000060: 656d 6169 6c20 3d20 6a63 6172 6c69 746f  email = jcarlito
 00000070: 6f6c 6976 6569 7261 4067 6d61 696c 2e63  oliveira@gmail.c
 00000080: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000090: 3d20 5368 6172 6564 204d 656d 6f72 7920  = Shared Memory
```

### Comparing `shareddata-2.0.8/src/SharedData/Defaults.py` & `shareddata-2.0.9/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/Logger.py` & `shareddata-2.0.9/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.0.9/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/Metadata.py` & `shareddata-2.0.9/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/MultiProc.py` & `shareddata-2.0.9/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/SeriesLib.py` & `shareddata-2.0.9/src/SharedData/SeriesLib.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/SharedData.py` & `shareddata-2.0.9/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/SharedDataAWSKinesis.py` & `shareddata-2.0.9/src/SharedData/SharedDataAWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/SharedDataAWSS3.py` & `shareddata-2.0.9/src/SharedData/SharedDataAWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/SharedDataFeeder.py` & `shareddata-2.0.9/src/SharedData/SharedDataFeeder.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/SharedDataFrame.py` & `shareddata-2.0.9/src/SharedData/SharedDataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/SharedDataPeriod.py` & `shareddata-2.0.9/src/SharedData/SharedDataPeriod.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/SharedDataRealTime.py` & `shareddata-2.0.9/src/SharedData/SharedDataRealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/SharedDataRealTimeProcess.py` & `shareddata-2.0.9/src/SharedData/SharedDataRealTimeProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/SharedDataTable.py` & `shareddata-2.0.9/src/SharedData/SharedDataTable.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/SharedDataTableKeys.py` & `shareddata-2.0.9/src/SharedData/SharedDataTableKeys.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         n = pkey.size-1                
         minchgid = count
         maxsize = records.size
         nrec = new_records.size
         for i in range(nrec):        
             h1 = hash(new_records['date'][i])
             h2 = hash(new_records['signal'][i])
-            h3 = hash(new_records['symbol'][i])            
+            h3 = hash(new_records['riskfactor'][i])            
             h4 = h1 ^ h2 ^ h3
             h = h4 % n
             id = pkey[h]
             if id == -1: 
                 # new record doesnt exist
                 pkey[h] = count
                 records[count] = new_records[i]
@@ -149,15 +149,15 @@
                 else:
                     break
             else:
                 # check for hash collision
                 j = 1
                 while (records[id]['date'] != new_records[i]['date'])\
                     | (records[id]['signal'] != new_records[i]['signal'])\
-                    | (records[id]['symbol'] != new_records[i]['symbol']):
+                    | (records[id]['riskfactor'] != new_records[i]['riskfactor']):
                     h = (h + j**2) % n
                     id = pkey[h]
                     if id==-1:
                         break
                     j += 1
 
                 if id == -1: 
@@ -458,26 +458,26 @@
     @njit(cache=True)
     def create_pkey_signals_jit(records,count,pkey,start):
         n = pkey.size-1        
         pkey[:] = -1
         for i in range(start,count):
             h1 = hash(records['date'][i])
             h2 = hash(records['signal'][i])
-            h3 = hash(records['symbol'][i])
+            h3 = hash(records['riskfactor'][i])
             h4 = h1 ^ h2 ^ h3
             h = h4 % n            
             id = pkey[h]
             if id == -1:                 
                 pkey[h] = i
             else:
                 # check for hash collision
                 j = 1
                 while (records[id]['date'] != records[i]['date'])\
                     | (records[id]['signal'] != records[i]['signal'])\
-                    | (records[id]['symbol'] != records[i]['symbol']):
+                    | (records[id]['riskfactor'] != records[i]['riskfactor']):
                     h = (h + j**2) % n
                     id = pkey[h]
                     if id==-1:
                         break
                     j += 1
 
                 if id == -1: 
@@ -679,26 +679,26 @@
     @njit(cache=True)
     def get_loc_signals_jit(records,pkey,keys):
         n = pkey.size-1
         loc = np.empty((keys.size, ))
         for i in range(keys.size):
             h1 = hash(records['date'][i])
             h2 = hash(records['signal'][i])
-            h3 = hash(records['symbol'][i])
+            h3 = hash(records['riskfactor'][i])
             h4 = h1 ^ h2 ^ h3
             h = h4 % n
             id = pkey[h]
             if id == -1:
                 loc[i] = id
             else:
                 # check for hash collision
                 j = 1
                 while (records[id]['date'] != records[i]['date'])\
                     | (records[id]['signal'] != records[i]['signal'])\
-                    | (records[id]['symbol'] != records[i]['symbol']):
+                    | (records[id]['riskfactor'] != records[i]['riskfactor']):
                     h = (h + j**2) % n
                     id = pkey[h]
                     if id==-1:
                         break
                     j += 1
                 loc[i] = id
         return loc
```

### Comparing `shareddata-2.0.8/src/SharedData/SharedDataTimeSeries.py` & `shareddata-2.0.9/src/SharedData/SharedDataTimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/SharedData/SharedNumpy.py` & `shareddata-2.0.9/src/SharedData/SharedNumpy.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.8/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.0.9/src/shareddata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.0.8
+Version: 2.0.9
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.0.8/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.0.9/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

