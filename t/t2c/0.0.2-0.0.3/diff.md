# Comparing `tmp/t2c-0.0.2.tar.gz` & `tmp/t2c-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2c-0.0.2.tar", last modified: Sun May 14 06:33:17 2023, max compression
+gzip compressed data, was "t2c-0.0.3.tar", last modified: Sun May 14 07:32:38 2023, max compression
```

## Comparing `t2c-0.0.2.tar` & `t2c-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 06:33:17.988796 t2c-0.0.2/
--rw-r--r--   0 iguangyu   (502) staff       (20)    11356 2023-05-13 17:09:56.000000 t2c-0.0.2/LICENSE
--rw-r--r--   0 iguangyu   (502) staff       (20)     1088 2023-05-14 06:33:17.988660 t2c-0.0.2/PKG-INFO
--rw-r--r--   0 iguangyu   (502) staff       (20)      550 2023-05-14 06:32:17.000000 t2c-0.0.2/README.md
--rw-r--r--   0 iguangyu   (502) staff       (20)       38 2023-05-14 06:33:17.988833 t2c-0.0.2/setup.cfg
--rw-r--r--   0 iguangyu   (502) staff       (20)      934 2023-05-14 06:32:56.000000 t2c-0.0.2/setup.py
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 06:33:17.987760 t2c-0.0.2/t2c/
--rw-r--r--   0 iguangyu   (502) staff       (20)       84 2023-05-14 06:28:43.000000 t2c-0.0.2/t2c/__init__.py
--rw-r--r--   0 iguangyu   (502) staff       (20)     5254 2023-05-14 06:26:11.000000 t2c-0.0.2/t2c/text2cron.py
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 06:33:17.988489 t2c-0.0.2/t2c.egg-info/
--rw-r--r--   0 iguangyu   (502) staff       (20)     1088 2023-05-14 06:33:17.000000 t2c-0.0.2/t2c.egg-info/PKG-INFO
--rw-r--r--   0 iguangyu   (502) staff       (20)      193 2023-05-14 06:33:17.000000 t2c-0.0.2/t2c.egg-info/SOURCES.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)        1 2023-05-14 06:33:17.000000 t2c-0.0.2/t2c.egg-info/dependency_links.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)       15 2023-05-14 06:33:17.000000 t2c-0.0.2/t2c.egg-info/requires.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)        4 2023-05-14 06:33:17.000000 t2c-0.0.2/t2c.egg-info/top_level.txt
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 07:32:38.836197 t2c-0.0.3/
+-rw-r--r--   0 iguangyu   (502) staff       (20)    11356 2023-05-13 17:09:56.000000 t2c-0.0.3/LICENSE
+-rw-r--r--   0 iguangyu   (502) staff       (20)     1074 2023-05-14 07:32:38.836051 t2c-0.0.3/PKG-INFO
+-rw-r--r--   0 iguangyu   (502) staff       (20)      536 2023-05-14 07:20:19.000000 t2c-0.0.3/README.md
+-rw-r--r--   0 iguangyu   (502) staff       (20)       38 2023-05-14 07:32:38.836241 t2c-0.0.3/setup.cfg
+-rw-r--r--   0 iguangyu   (502) staff       (20)      918 2023-05-14 07:17:37.000000 t2c-0.0.3/setup.py
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 07:32:38.835190 t2c-0.0.3/t2c/
+-rw-r--r--   0 iguangyu   (502) staff       (20)       86 2023-05-14 07:17:26.000000 t2c-0.0.3/t2c/__init__.py
+-rw-r--r--   0 iguangyu   (502) staff       (20)     5045 2023-05-14 07:28:48.000000 t2c-0.0.3/t2c/text2cron.py
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 07:32:38.835880 t2c-0.0.3/t2c.egg-info/
+-rw-r--r--   0 iguangyu   (502) staff       (20)     1074 2023-05-14 07:32:38.000000 t2c-0.0.3/t2c.egg-info/PKG-INFO
+-rw-r--r--   0 iguangyu   (502) staff       (20)      193 2023-05-14 07:32:38.000000 t2c-0.0.3/t2c.egg-info/SOURCES.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)        1 2023-05-14 07:32:38.000000 t2c-0.0.3/t2c.egg-info/dependency_links.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)       15 2023-05-14 07:32:38.000000 t2c-0.0.3/t2c.egg-info/requires.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)        4 2023-05-14 07:32:38.000000 t2c-0.0.3/t2c.egg-info/top_level.txt
```

### Comparing `t2c-0.0.2/LICENSE` & `t2c-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `t2c-0.0.2/PKG-INFO` & `t2c-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2c
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python Library that converts human readable text to Cron Expression.
 Home-page: https://github.com/iguangyu/text2cron
 Author: iguangyu
 Author-email: oofheaven7@gmail.com
 License: MIT
 Keywords: text cron text langchain gpt npl
 Classifier: Development Status :: 4 - Beta
@@ -15,18 +15,18 @@
 License-File: LICENSE
 
 ## A Python Library that converts human readable text to Cron Expression(Currently only supports Chinese)
 ## 可以将人类语言转换为cron表达式的Python库(目前仅支持中文)
 
 ### Installation
 ``` bash
-pip install --upgrade openai
+pip install t2c
 ```
 
-### useage
+### usage
 ``` python
 import t2c
 # normal
 cron_reg = t2c.Text2Cron('今天下午两点钟').cron()
 # use openai api key
 cron_gpt = t2c.Text2Cron('今天下午两点钟').gpt()
 # print the cron expressions
```

### Comparing `t2c-0.0.2/README.md` & `t2c-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ## A Python Library that converts human readable text to Cron Expression(Currently only supports Chinese)
 ## 可以将人类语言转换为cron表达式的Python库(目前仅支持中文)
 
 ### Installation
 ``` bash
-pip install --upgrade openai
+pip install t2c
 ```
 
-### useage
+### usage
 ``` python
 import t2c
 # normal
 cron_reg = t2c.Text2Cron('今天下午两点钟').cron()
 # use openai api key
 cron_gpt = t2c.Text2Cron('今天下午两点钟').gpt()
 # print the cron expressions
```

### Comparing `t2c-0.0.2/setup.py` & `t2c-0.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 from codecs import open
 
 # Get the long description from the relevant file
-with open('README.md', 'r', encoding='utf-8') as f:
-    long_description = f.read()
+with open('README.md', 'r') as fh:
+    long_description = fh.read()
 
 setup(
     name='t2c',
-    version='0.0.2',
+    version='0.0.3',
     description='A Python Library that converts human readable text to Cron Expression.',
     long_description=long_description,
     url='https://github.com/iguangyu/text2cron',
     author='iguangyu',
     author_email='oofheaven7@gmail.com',
     license='MIT',
     classifiers=[
```

### Comparing `t2c-0.0.2/t2c/text2cron.py` & `t2c-0.0.3/t2c/text2cron.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,52 +40,46 @@
         if usegpt:
             self.apikey = apikey
         else:
             text = text.replace('\n','')
             for key, value in re_dict.items():
                 text = text.replace(key, value)
             self.text = cn2an.transform(text)
-            print("transform之后: "+self.text)
         
     def __to_cron(self) -> None:
         l, isshort = self.__find_util(self.text)
-        print(l)
         if isshort:
             digit = float(l[0])
             offset = {
                 '年': self.now.add(years=int(digit)), 
                 '月': self.now.add(months=int(digit)),
                 '周': self.now.add(weeks=digit),
                 '天': self.now.add(days=digit),
                 '时': self.now.add(hours=digit),
                 '分': self.now.add(minutes=digit)
             }
             self.now = offset[l[1]]
         else:
             period, day, aopm, hour, minute = l
-            print(period, day, aopm, hour, minute)
-            if hour != '':
+            if period != '':
+                pass
+            if day != '':
+                self.now = self.now.add(days=1) # TODO
+            if hour != '' and 0<= int(hour) < 24:
                 if aopm != '' and '晚' in aopm or '下' in aopm:
                     self.now = self.now.replace(hour=(int(hour) % 12 + 12))
                 else:
                     self.now = self.now.replace(hour=int(hour))
-            if minute != '':
-                self.now = self.now.replace(minute=int(minute))
-            if day != '':
-                self.now = self.now.add(days=1) # TODO
-            if period != '':
-                pass
             
-        print(self.now.to_datetime_string())
-        print(self.now.diff_for_humans())
+            self.now = self.now.replace(minute=int(minute) if minute != '' else 0)
+            self.now = self.now.replace(second=0)
         return self.cron
 
     def cron(self) -> list:
         self.__to_cron()
-        print(self.now.to_datetime_string())
         return [
             self.now.second, self.now.minute, self.now.hour, 
             self.now.day, self.now.month, '?', self.now.year,
         ]
     
     def __find_util(self, text: str) -> list[tuple, bool]:
         long_term = max(re.findall(pattern=self.full_pattern, string=text),
@@ -129,15 +123,14 @@
     
     args = parser.parse_args()
     text = args.time
     if args.gpt is not None:
         res = Text2Cron(text, usegpt=True, apikey='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').gpt()
     else: 
         res = Text2Cron(text).cron()
-    print(res)        
 
     if args.cron is not None:
         print('= cron表达式如下 =')
         cron_exp = ' '.join([str(c) for c in res])
         res = requests.get('http://cron.ciding.cc/getCornTimes?cronExpression='+cron_exp+'&time=5')
         print('\n'.join(json.loads(res.text)['datas']))
```

### Comparing `t2c-0.0.2/t2c.egg-info/PKG-INFO` & `t2c-0.0.3/t2c.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2c
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python Library that converts human readable text to Cron Expression.
 Home-page: https://github.com/iguangyu/text2cron
 Author: iguangyu
 Author-email: oofheaven7@gmail.com
 License: MIT
 Keywords: text cron text langchain gpt npl
 Classifier: Development Status :: 4 - Beta
@@ -15,18 +15,18 @@
 License-File: LICENSE
 
 ## A Python Library that converts human readable text to Cron Expression(Currently only supports Chinese)
 ## 可以将人类语言转换为cron表达式的Python库(目前仅支持中文)
 
 ### Installation
 ``` bash
-pip install --upgrade openai
+pip install t2c
 ```
 
-### useage
+### usage
 ``` python
 import t2c
 # normal
 cron_reg = t2c.Text2Cron('今天下午两点钟').cron()
 # use openai api key
 cron_gpt = t2c.Text2Cron('今天下午两点钟').gpt()
 # print the cron expressions
```

