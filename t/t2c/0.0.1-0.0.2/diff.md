# Comparing `tmp/t2c-0.0.1.tar.gz` & `tmp/t2c-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2c-0.0.1.tar", last modified: Sat May 13 17:12:45 2023, max compression
+gzip compressed data, was "t2c-0.0.2.tar", last modified: Sun May 14 06:33:17 2023, max compression
```

## Comparing `t2c-0.0.1.tar` & `t2c-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-13 17:12:45.628882 t2c-0.0.1/
--rw-r--r--   0 iguangyu   (502) staff       (20)    11356 2023-05-13 17:09:56.000000 t2c-0.0.1/LICENSE
--rw-r--r--   0 iguangyu   (502) staff       (20)      696 2023-05-13 17:12:45.628747 t2c-0.0.1/PKG-INFO
--rw-r--r--   0 iguangyu   (502) staff       (20)      158 2023-05-13 17:02:43.000000 t2c-0.0.1/README.md
--rw-r--r--   0 iguangyu   (502) staff       (20)       38 2023-05-13 17:12:45.628917 t2c-0.0.1/setup.cfg
--rw-r--r--   0 iguangyu   (502) staff       (20)     2415 2023-05-13 17:07:46.000000 t2c-0.0.1/setup.py
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-13 17:12:45.627918 t2c-0.0.1/t2c/
--rw-r--r--   0 iguangyu   (502) staff       (20)       12 2023-05-13 15:00:31.000000 t2c-0.0.1/t2c/__init__.py
--rw-r--r--   0 iguangyu   (502) staff       (20)     4251 2023-05-13 17:05:24.000000 t2c-0.0.1/t2c/text2cron.py
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-13 17:12:45.628581 t2c-0.0.1/t2c.egg-info/
--rw-r--r--   0 iguangyu   (502) staff       (20)      696 2023-05-13 17:12:45.000000 t2c-0.0.1/t2c.egg-info/PKG-INFO
--rw-r--r--   0 iguangyu   (502) staff       (20)      193 2023-05-13 17:12:45.000000 t2c-0.0.1/t2c.egg-info/SOURCES.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)        1 2023-05-13 17:12:45.000000 t2c-0.0.1/t2c.egg-info/dependency_links.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)       15 2023-05-13 17:12:45.000000 t2c-0.0.1/t2c.egg-info/requires.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)        4 2023-05-13 17:12:45.000000 t2c-0.0.1/t2c.egg-info/top_level.txt
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 06:33:17.988796 t2c-0.0.2/
+-rw-r--r--   0 iguangyu   (502) staff       (20)    11356 2023-05-13 17:09:56.000000 t2c-0.0.2/LICENSE
+-rw-r--r--   0 iguangyu   (502) staff       (20)     1088 2023-05-14 06:33:17.988660 t2c-0.0.2/PKG-INFO
+-rw-r--r--   0 iguangyu   (502) staff       (20)      550 2023-05-14 06:32:17.000000 t2c-0.0.2/README.md
+-rw-r--r--   0 iguangyu   (502) staff       (20)       38 2023-05-14 06:33:17.988833 t2c-0.0.2/setup.cfg
+-rw-r--r--   0 iguangyu   (502) staff       (20)      934 2023-05-14 06:32:56.000000 t2c-0.0.2/setup.py
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 06:33:17.987760 t2c-0.0.2/t2c/
+-rw-r--r--   0 iguangyu   (502) staff       (20)       84 2023-05-14 06:28:43.000000 t2c-0.0.2/t2c/__init__.py
+-rw-r--r--   0 iguangyu   (502) staff       (20)     5254 2023-05-14 06:26:11.000000 t2c-0.0.2/t2c/text2cron.py
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 06:33:17.988489 t2c-0.0.2/t2c.egg-info/
+-rw-r--r--   0 iguangyu   (502) staff       (20)     1088 2023-05-14 06:33:17.000000 t2c-0.0.2/t2c.egg-info/PKG-INFO
+-rw-r--r--   0 iguangyu   (502) staff       (20)      193 2023-05-14 06:33:17.000000 t2c-0.0.2/t2c.egg-info/SOURCES.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)        1 2023-05-14 06:33:17.000000 t2c-0.0.2/t2c.egg-info/dependency_links.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)       15 2023-05-14 06:33:17.000000 t2c-0.0.2/t2c.egg-info/requires.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)        4 2023-05-14 06:33:17.000000 t2c-0.0.2/t2c.egg-info/top_level.txt
```

### Comparing `t2c-0.0.1/LICENSE` & `t2c-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `t2c-0.0.1/t2c/text2cron.py` & `t2c-0.0.2/t2c/text2cron.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,13 @@
 import re
 import json
 import requests
 import pendulum
 import cn2an
 
-
-# class RegexMap:
-#     def __init__(self, n_dic: dict, val):
-#         self._items = n_dic
-#         self.__val = val
-
-#     def get(self, key):
-#         for regex in self._items.items():
-#             if search(regex, key, I):
-#                 return self._items[regex]
-#         return self.__val
-    
-
-
 re_dict = {
     "日": "天",
     "星期": "周",
     "礼拜": "周",
     "小时": "时",
     "钟头": "时",
     "点钟": "时",
@@ -44,22 +30,25 @@
     aopm = r'(早.|上.|中.|下.|晚.)?'
     hour = r'(\d+)?' + r'[点时：:]?'
     minute = r'([0-5]?[0-9]|半|一刻)?'
     
     full_pattern = period + day + aopm + hour + minute 
     short_term = r'(\d+\.?5?)?个?([分时天周月年])之?后'
     
-    def __init__(self, text: str, **kwargs) -> None:
-        print(self.full_pattern)
+    def __init__(self, text: str, usegpt = False, apikey = '') -> None:
         self.now = pendulum.now()
-        text = text.replace('\n','')
-        for key, value in re_dict.items():
-            text = text.replace(key, value)
-        self.text = cn2an.transform(text)
-        print("transform之后: "+self.text)
+        self.text = text
+        if usegpt:
+            self.apikey = apikey
+        else:
+            text = text.replace('\n','')
+            for key, value in re_dict.items():
+                text = text.replace(key, value)
+            self.text = cn2an.transform(text)
+            print("transform之后: "+self.text)
         
     def __to_cron(self) -> None:
         l, isshort = self.__find_util(self.text)
         print(l)
         if isshort:
             digit = float(l[0])
             offset = {
@@ -72,57 +61,84 @@
             }
             self.now = offset[l[1]]
         else:
             period, day, aopm, hour, minute = l
             print(period, day, aopm, hour, minute)
             if hour != '':
                 if aopm != '' and '晚' in aopm or '下' in aopm:
-                    self.now = self.now.replace(hour=int(hour % 12 + 12))
+                    self.now = self.now.replace(hour=(int(hour) % 12 + 12))
                 else:
                     self.now = self.now.replace(hour=int(hour))
             if minute != '':
                 self.now = self.now.replace(minute=int(minute))
             if day != '':
-                
                 self.now = self.now.add(days=1) # TODO
             if period != '':
                 pass
             
         print(self.now.to_datetime_string())
         print(self.now.diff_for_humans())
         return self.cron
 
-    def cron(self):
+    def cron(self) -> list:
         self.__to_cron()
         print(self.now.to_datetime_string())
         return [
             self.now.second, self.now.minute, self.now.hour, 
             self.now.day, self.now.month, '?', self.now.year,
         ]
     
     def __find_util(self, text: str) -> list[tuple, bool]:
         long_term = max(re.findall(pattern=self.full_pattern, string=text),
             key=lambda tup: sum(1 for val in tup if val != ''))
         short_term = re.findall(pattern=self.short_term, string=text)
         short_term = () if len(short_term) == 0 else short_term[0]
+        if sum(1 for val in short_term if val != '') == 2:
+            return short_term, True
         term = max([long_term, short_term],
             key=lambda tup: sum(1 for val in tup if val != ''))
         return term, term == short_term
 
+    def gpt(self) -> str:
+        if self.apikey == '':
+            raise "api key is required"
+        try:
+            import openai
+            openai.api_key = self.apikey
+            res = openai.ChatCompletion.create(
+            model="gpt-3.5-turbo",
+            messages=[{
+                    "role": "system",
+                    "content": "You are a helpful webapp that provides users with cron expressions"
+                },{
+                    "role": "user",
+                    "content": f"Write a cron expression for the following and please just output the answer, say nothing else and don't explain 'current time is {self.now.to_datetime_string} {self.text}'"
+                }]
+            )
+            return res.choices[0].message.content
+        except ImportError as e:
+            print('You need to install openai module to use gpt\npip install openai')
+        
+
+
 if __name__ == '__main__':
     import argparse
     parser = argparse.ArgumentParser(description='task tool argparse')
     parser.add_argument('--time', '-t', type=str, default=None, help="安排的任务时间")
     parser.add_argument('--cron', '-c', type=str, default=None, help="解析cron")
+    parser.add_argument('--gpt', '-g', type=str, default=None, help="使用gpt")
     
     args = parser.parse_args()
     text = args.time
-    res = Text2Cron(text).cron()
-    print(res)
-            
+    if args.gpt is not None:
+        res = Text2Cron(text, usegpt=True, apikey='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').gpt()
+    else: 
+        res = Text2Cron(text).cron()
+    print(res)        
+
     if args.cron is not None:
         print('= cron表达式如下 =')
         cron_exp = ' '.join([str(c) for c in res])
         res = requests.get('http://cron.ciding.cc/getCornTimes?cronExpression='+cron_exp+'&time=5')
         print('\n'.join(json.loads(res.text)['datas']))
 
     # import pendulum
```

