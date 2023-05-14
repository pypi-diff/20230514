# Comparing `tmp/t2c-0.0.3.tar.gz` & `tmp/t2c-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2c-0.0.3.tar", last modified: Sun May 14 07:32:38 2023, max compression
+gzip compressed data, was "t2c-0.0.4.tar", last modified: Sun May 14 16:26:39 2023, max compression
```

## Comparing `t2c-0.0.3.tar` & `t2c-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 07:32:38.836197 t2c-0.0.3/
--rw-r--r--   0 iguangyu   (502) staff       (20)    11356 2023-05-13 17:09:56.000000 t2c-0.0.3/LICENSE
--rw-r--r--   0 iguangyu   (502) staff       (20)     1074 2023-05-14 07:32:38.836051 t2c-0.0.3/PKG-INFO
--rw-r--r--   0 iguangyu   (502) staff       (20)      536 2023-05-14 07:20:19.000000 t2c-0.0.3/README.md
--rw-r--r--   0 iguangyu   (502) staff       (20)       38 2023-05-14 07:32:38.836241 t2c-0.0.3/setup.cfg
--rw-r--r--   0 iguangyu   (502) staff       (20)      918 2023-05-14 07:17:37.000000 t2c-0.0.3/setup.py
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 07:32:38.835190 t2c-0.0.3/t2c/
--rw-r--r--   0 iguangyu   (502) staff       (20)       86 2023-05-14 07:17:26.000000 t2c-0.0.3/t2c/__init__.py
--rw-r--r--   0 iguangyu   (502) staff       (20)     5045 2023-05-14 07:28:48.000000 t2c-0.0.3/t2c/text2cron.py
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 07:32:38.835880 t2c-0.0.3/t2c.egg-info/
--rw-r--r--   0 iguangyu   (502) staff       (20)     1074 2023-05-14 07:32:38.000000 t2c-0.0.3/t2c.egg-info/PKG-INFO
--rw-r--r--   0 iguangyu   (502) staff       (20)      193 2023-05-14 07:32:38.000000 t2c-0.0.3/t2c.egg-info/SOURCES.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)        1 2023-05-14 07:32:38.000000 t2c-0.0.3/t2c.egg-info/dependency_links.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)       15 2023-05-14 07:32:38.000000 t2c-0.0.3/t2c.egg-info/requires.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)        4 2023-05-14 07:32:38.000000 t2c-0.0.3/t2c.egg-info/top_level.txt
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 16:26:39.947018 t2c-0.0.4/
+-rw-r--r--   0 iguangyu   (502) staff       (20)    11356 2023-05-13 17:09:56.000000 t2c-0.0.4/LICENSE
+-rw-r--r--   0 iguangyu   (502) staff       (20)     1088 2023-05-14 16:26:39.946854 t2c-0.0.4/PKG-INFO
+-rw-r--r--   0 iguangyu   (502) staff       (20)      550 2023-05-14 16:25:57.000000 t2c-0.0.4/README.md
+-rw-r--r--   0 iguangyu   (502) staff       (20)       38 2023-05-14 16:26:39.947061 t2c-0.0.4/setup.cfg
+-rw-r--r--   0 iguangyu   (502) staff       (20)      918 2023-05-14 16:26:04.000000 t2c-0.0.4/setup.py
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 16:26:39.945848 t2c-0.0.4/t2c/
+-rw-r--r--   0 iguangyu   (502) staff       (20)       86 2023-05-14 16:26:08.000000 t2c-0.0.4/t2c/__init__.py
+-rw-r--r--   0 iguangyu   (502) staff       (20)     6755 2023-05-14 16:25:03.000000 t2c-0.0.4/t2c/text2cron.py
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 16:26:39.946680 t2c-0.0.4/t2c.egg-info/
+-rw-r--r--   0 iguangyu   (502) staff       (20)     1088 2023-05-14 16:26:39.000000 t2c-0.0.4/t2c.egg-info/PKG-INFO
+-rw-r--r--   0 iguangyu   (502) staff       (20)      193 2023-05-14 16:26:39.000000 t2c-0.0.4/t2c.egg-info/SOURCES.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)        1 2023-05-14 16:26:39.000000 t2c-0.0.4/t2c.egg-info/dependency_links.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)       15 2023-05-14 16:26:39.000000 t2c-0.0.4/t2c.egg-info/requires.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)        4 2023-05-14 16:26:39.000000 t2c-0.0.4/t2c.egg-info/top_level.txt
```

### Comparing `t2c-0.0.3/LICENSE` & `t2c-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `t2c-0.0.3/PKG-INFO` & `t2c-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2c
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Library that converts human readable text to Cron Expression.
 Home-page: https://github.com/iguangyu/text2cron
 Author: iguangyu
 Author-email: oofheaven7@gmail.com
 License: MIT
 Keywords: text cron text langchain gpt npl
 Classifier: Development Status :: 4 - Beta
@@ -26,10 +26,11 @@
 ``` python
 import t2c
 # normal
 cron_reg = t2c.Text2Cron('今天下午两点钟').cron()
 # use openai api key
 cron_gpt = t2c.Text2Cron('今天下午两点钟').gpt()
 # print the cron expressions
-print(cron_reg) # output: [4, 47, 14, 15, 5, '?', 2023]
+# current time: 2023/5/15 00:25
+print(cron_reg) # output: 0 14 15 5 ?
 print(cron_gpt) # output: 0 14 * * *
 ```
```

### Comparing `t2c-0.0.3/README.md` & `t2c-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -10,10 +10,11 @@
 ``` python
 import t2c
 # normal
 cron_reg = t2c.Text2Cron('今天下午两点钟').cron()
 # use openai api key
 cron_gpt = t2c.Text2Cron('今天下午两点钟').gpt()
 # print the cron expressions
-print(cron_reg) # output: [4, 47, 14, 15, 5, '?', 2023]
+# current time: 2023/5/15 00:25
+print(cron_reg) # output: 0 14 15 5 ?
 print(cron_gpt) # output: 0 14 * * *
 ```
```

### Comparing `t2c-0.0.3/setup.py` & `t2c-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Get the long description from the relevant file
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='t2c',
-    version='0.0.3',
+    version='0.0.4',
     description='A Python Library that converts human readable text to Cron Expression.',
     long_description=long_description,
     url='https://github.com/iguangyu/text2cron',
     author='iguangyu',
     author_email='oofheaven7@gmail.com',
     license='MIT',
     classifiers=[
```

### Comparing `t2c-0.0.3/t2c/text2cron.py` & `t2c-0.0.4/t2c/text2cron.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,107 +1,142 @@
 import re
 import json
 import requests
 import pendulum
 import cn2an
 
-re_dict = {
-    "日": "天",
-    "星期": "周",
-    "礼拜": "周",
-    "小时": "时",
-    "钟头": "时",
-    "点钟": "时",
-    "点": "时",
-    "小时": "时",
-    "分钟": "分",
-    "个半": ".5",
-    "天半": ".5天",
-    "半时":"30分",
-    "半个时":"30分",
-    "半个小时":"30分",
-    "半":"30分",
-    "一刻": "15分",
-    "minute": "分",
-}
 class Text2Cron(object):
-    
-    period = r'(每个?|下个?|这个?)?'
-    day = r'(今.|明[天]?|后[天]?|周[天1234567]?|[天周月年])?'
+    now = pendulum.now()
+    current_datetime = f"{now.hour}时{now.minute}分"
+    re_dict = {
+        ' ': '',
+        '号': '日',
+        "日": "天",
+        "星期": "周",
+        "礼拜": "周",
+        "小时": "时",
+        "钟头": "时",
+        "点钟": "时",
+        "点": "时",
+        "小时": "时",
+        "分钟": "分",
+        "个半": ".5",
+        "天半": ".5天",
+        "半时":"30分",
+        "半个时":"30分",
+        "半个小时":"30分",
+        "半":"30分",
+        "一刻": "15分",
+        "minute": "分",
+        "这时候": current_datetime,
+        "这个时候": current_datetime
+    }
+    period = r'(每个?|下[^午]|这个?)?'
+    day = r'(今.|明[天]?|后[天]?|周[天1234567]?|月\d+天|[天周月年])?'
     aopm = r'(早.|上.|中.|下.|晚.)?'
     hour = r'(\d+)?' + r'[点时：:]?'
     minute = r'([0-5]?[0-9]|半|一刻)?'
     
     full_pattern = period + day + aopm + hour + minute 
     short_term = r'(\d+\.?5?)?个?([分时天周月年])之?后'
+    day_pattern = r'周(\d|天)|月(\d+)天|(今.)|(明.)|(大*后.)'
+    
     
-    def __init__(self, text: str, usegpt = False, apikey = '') -> None:
-        self.now = pendulum.now()
+    def __init__(self, text: str, usegpt = False) -> None:
         self.text = text
-        if usegpt:
-            self.apikey = apikey
-        else:
+        # print(self.full_pattern)
+        if not usegpt:
             text = text.replace('\n','')
-            for key, value in re_dict.items():
+            for key, value in self.re_dict.items():
                 text = text.replace(key, value)
             self.text = cn2an.transform(text)
         
-    def __to_cron(self) -> None:
+    def __to_cron(self) -> list:
         l, isshort = self.__find_util(self.text)
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
+            return [
+                0, self.now.minute, self.now.hour, 
+                self.now.day, self.now.month, '?', self.now.year,
+            ]
         else:
             period, day, aopm, hour, minute = l
+            everyday = False
+            # period_matches = re.search(self.period_pattern, period)
+            day_matches = re.search(self.day_pattern, day)
+            if day_matches is not None:
+                matches = day_matches.groups()
+                date_day, offset_days = matches[0:2], matches[2::]
+                if date_day != (None, None):
+                    self.now = self.now.replace(day=int(date_day[1])) \
+                        if date_day[0] is None else self.now.next(
+                            int(date_day[0]) if date_day[0] != '天' else 0)
+                else:
+                    a,b,c = offset_days
+                    self.now = self.now.add(
+                        days=0 if a is not None else 1 \
+                            if b is not None else c.count('大') + 2 \
+                                if c is not None else 0)
             if period != '':
-                pass
-            if day != '':
-                self.now = self.now.add(days=1) # TODO
+                if '每' in period:
+                    if '天' in day:
+                        everyday = True
+                    # TODO
             if hour != '' and 0<= int(hour) < 24:
-                if aopm != '' and '晚' in aopm or '下' in aopm:
-                    self.now = self.now.replace(hour=(int(hour) % 12 + 12))
+                hour = int(hour)
+                if '晚' in aopm or '下' in aopm and hour <= 12:
+                    if hour == 12:
+                        self.now = self.now.replace(hour=0)
+                        self.now.add(days=1)
+                    else:
+                        self.now = self.now.replace(hour=(12 + hour % 12))
                 else:
                     self.now = self.now.replace(hour=int(hour))
-            
             self.now = self.now.replace(minute=int(minute) if minute != '' else 0)
             self.now = self.now.replace(second=0)
-        return self.cron
-
-    def cron(self) -> list:
-        self.__to_cron()
-        return [
-            self.now.second, self.now.minute, self.now.hour, 
-            self.now.day, self.now.month, '?', self.now.year,
-        ]
+            return [
+                self.now.minute, self.now.hour, 
+                self.now.day if not everyday else '*', 
+                self.now.month if not everyday else '*',
+                '?',
+            ]
+
+    def show_args(self):
+        l, _ = self.__find_util(self.text)
+        return l
+
+    def cron(self) -> str:
+        cron_list = self.__to_cron()
+        return ' '.join([str(i) for i in cron_list])
+    
     
     def __find_util(self, text: str) -> list[tuple, bool]:
         long_term = max(re.findall(pattern=self.full_pattern, string=text),
             key=lambda tup: sum(1 for val in tup if val != ''))
         short_term = re.findall(pattern=self.short_term, string=text)
         short_term = () if len(short_term) == 0 else short_term[0]
         if sum(1 for val in short_term if val != '') == 2:
             return short_term, True
         term = max([long_term, short_term],
             key=lambda tup: sum(1 for val in tup if val != ''))
         return term, term == short_term
 
-    def gpt(self) -> str:
-        if self.apikey == '':
-            raise "api key is required"
+    def gpt(self, apikey: str) -> str:        
         try:
             import openai
-            openai.api_key = self.apikey
+            openai.api_key = apikey
             res = openai.ChatCompletion.create(
             model="gpt-3.5-turbo",
             messages=[{
                     "role": "system",
                     "content": "You are a helpful webapp that provides users with cron expressions"
                 },{
                     "role": "user",
@@ -123,14 +158,15 @@
     
     args = parser.parse_args()
     text = args.time
     if args.gpt is not None:
         res = Text2Cron(text, usegpt=True, apikey='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').gpt()
     else: 
         res = Text2Cron(text).cron()
+        print(res)
 
     if args.cron is not None:
         print('= cron表达式如下 =')
         cron_exp = ' '.join([str(c) for c in res])
         res = requests.get('http://cron.ciding.cc/getCornTimes?cronExpression='+cron_exp+'&time=5')
         print('\n'.join(json.loads(res.text)['datas']))
```

### Comparing `t2c-0.0.3/t2c.egg-info/PKG-INFO` & `t2c-0.0.4/t2c.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2c
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Library that converts human readable text to Cron Expression.
 Home-page: https://github.com/iguangyu/text2cron
 Author: iguangyu
 Author-email: oofheaven7@gmail.com
 License: MIT
 Keywords: text cron text langchain gpt npl
 Classifier: Development Status :: 4 - Beta
@@ -26,10 +26,11 @@
 ``` python
 import t2c
 # normal
 cron_reg = t2c.Text2Cron('今天下午两点钟').cron()
 # use openai api key
 cron_gpt = t2c.Text2Cron('今天下午两点钟').gpt()
 # print the cron expressions
-print(cron_reg) # output: [4, 47, 14, 15, 5, '?', 2023]
+# current time: 2023/5/15 00:25
+print(cron_reg) # output: 0 14 15 5 ?
 print(cron_gpt) # output: 0 14 * * *
 ```
```

