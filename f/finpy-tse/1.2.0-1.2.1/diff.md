# Comparing `tmp/finpy_tse-1.2.0.tar.gz` & `tmp/finpy_tse-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finpy_tse-1.2.0.tar", last modified: Thu Jan 12 07:43:34 2023, max compression
+gzip compressed data, was "finpy_tse-1.2.1.tar", last modified: Sun May 14 08:02:36 2023, max compression
```

## Comparing `finpy_tse-1.2.0.tar` & `finpy_tse-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 07:43:34.579887 finpy_tse-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-01-12 07:43:23.000000 finpy_tse-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-01-12 07:43:34.579887 finpy_tse-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-01-12 07:43:23.000000 finpy_tse-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 07:43:34.579887 finpy_tse-1.2.0/finpy_tse/
--rw-r--r--   0 runner    (1001) docker     (123)   162684 2023-01-12 07:43:23.000000 finpy_tse-1.2.0/finpy_tse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 07:43:34.579887 finpy_tse-1.2.0/finpy_tse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-01-12 07:43:34.000000 finpy_tse-1.2.0/finpy_tse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-01-12 07:43:34.000000 finpy_tse-1.2.0/finpy_tse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 07:43:34.000000 finpy_tse-1.2.0/finpy_tse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-12 07:43:34.000000 finpy_tse-1.2.0/finpy_tse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-12 07:43:34.000000 finpy_tse-1.2.0/finpy_tse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 07:43:34.579887 finpy_tse-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-01-12 07:43:23.000000 finpy_tse-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 08:02:36.417531 finpy_tse-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-14 08:02:05.000000 finpy_tse-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-14 08:02:36.417531 finpy_tse-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-05-14 08:02:05.000000 finpy_tse-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 08:02:36.417531 finpy_tse-1.2.1/finpy_tse/
+-rw-r--r--   0 runner    (1001) docker     (123)   163676 2023-05-14 08:02:05.000000 finpy_tse-1.2.1/finpy_tse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 08:02:36.417531 finpy_tse-1.2.1/finpy_tse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-14 08:02:36.000000 finpy_tse-1.2.1/finpy_tse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-14 08:02:36.000000 finpy_tse-1.2.1/finpy_tse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 08:02:36.000000 finpy_tse-1.2.1/finpy_tse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-14 08:02:36.000000 finpy_tse-1.2.1/finpy_tse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 08:02:36.000000 finpy_tse-1.2.1/finpy_tse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 08:02:36.417531 finpy_tse-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-14 08:02:05.000000 finpy_tse-1.2.1/setup.py
```

### Comparing `finpy_tse-1.2.0/LICENSE.txt` & `finpy_tse-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finpy_tse-1.2.0/PKG-INFO` & `finpy_tse-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finpy_tse
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data
 Author: ALI RAHIMI  AND  RASOOL GHAFOURI
 Author-email: a.rahimi.aut@gmail.com
 License: BSD (3-clause)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `finpy_tse-1.2.0/README.md` & `finpy_tse-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `finpy_tse-1.2.0/finpy_tse/__init__.py` & `finpy_tse-1.2.1/finpy_tse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,30 +245,40 @@
         df_history = df_history[start_date:end_date]
     return df_history
 
 
 ################################################################################################################################################################################
 ################################################################################################################################################################################
 
-def Get_RI_History(stock = 'خودرو', start_date = '1400-01-01', end_date='1401-01-01', ignore_date = False, show_weekday = False, double_date = False):
+def Get_RI_History(stock = 'خودرو', start_date = '1400-01-01', end_date='1401-01-01', ignore_date = False, show_weekday = False, double_date = False, alt = False):
     """
     دریافت سابقه اطلاعات حقیقی-حقوقی یک سهم در روزهای معاملاتی بین تاریخ شروع و پایان
     قابلیت دریافت همه سابقه حقیقی-حقوقی بدون توجه به تاریخ شروع و پایان
     قابلیت ارائه تاریخ میلادی علاوه بر تاریخ شمسی، قابلیت نمایش روزهای هفته
     """
     # a function to get ri data from a given page ----------------------------------------------------------------------------------
     def get_ri_data(ticker_no,ticker,name, data_part):
-        r = requests.get(f'http://www.tsetmc.com/tsev2/data/clienttype.aspx?i={ticker_no}', headers=headers)
-        df_RI_tab=pd.DataFrame(r.text.split(';'))
-        # define columns
-        columns=['Date','No_Buy_R','No_Buy_I','No_Sell_R','No_Sell_I','Vol_Buy_R','Vol_Buy_I','Vol_Sell_R','Vol_Sell_I','Val_Buy_R','Val_Buy_I','Val_Sell_R','Val_Sell_I']
-        # split data into defined columns
-        df_RI_tab[columns] = df_RI_tab[0].str.split(",",expand=True)
-        # drop old column 0
-        df_RI_tab.drop(columns=[0],inplace=True)
+        if(alt):
+            r = requests.get(f'http://cdn.tsetmc.com/api/ClientType/GetClientTypeHistory/{ticker_no}',headers=headers)
+            df_RI_tab = pd.DataFrame(r.json()['clientType'])
+            cols = ['Date','WebID','Vol_Buy_R','Vol_Buy_I','Val_Buy_R','Val_Buy_I','No_Buy_I','Vol_Sell_R','No_Buy_R','Vol_Sell_I','Val_Sell_R','Val_Sell_I','No_Sell_I','No_Sell_R']
+            df_RI_tab.columns = cols
+            df_RI_tab = df_RI_tab[['Date','No_Buy_R','No_Buy_I','No_Sell_R','No_Sell_I','Vol_Buy_R','Vol_Buy_I','Vol_Sell_R','Vol_Sell_I','Val_Buy_R','Val_Buy_I','Val_Sell_R','Val_Sell_I']]
+            df_RI_tab['Date'] = df_RI_tab['Date'].apply(lambda x: str(x))
+            cols = ['No_Buy_R','No_Buy_I','No_Sell_R','No_Sell_I','Vol_Buy_R','Vol_Buy_I','Vol_Sell_R','Vol_Sell_I','Val_Buy_R','Val_Buy_I','Val_Sell_R','Val_Sell_I']
+            df_RI_tab[cols] = df_RI_tab[cols].astype('int64')
+        else:
+            r = requests.get(f'http://www.tsetmc.com/tsev2/data/clienttype.aspx?i={ticker_no}', headers=headers)
+            df_RI_tab=pd.DataFrame(r.text.split(';'))
+            # define columns
+            columns=['Date','No_Buy_R','No_Buy_I','No_Sell_R','No_Sell_I','Vol_Buy_R','Vol_Buy_I','Vol_Sell_R','Vol_Sell_I','Val_Buy_R','Val_Buy_I','Val_Sell_R','Val_Sell_I']
+            # split data into defined columns
+            df_RI_tab[columns] = df_RI_tab[0].str.split(",",expand=True)
+            # drop old column 0
+            df_RI_tab.drop(columns=[0],inplace=True)
         df_RI_tab['Date']=pd.to_datetime(df_RI_tab['Date'])
         df_RI_tab['Ticker'] = ticker
         df_RI_tab['Name'] = name
         df_RI_tab['Market'] = data_part
         df_RI_tab = df_RI_tab.set_index('Date')
         return df_RI_tab
     # check date validity --------------------------------------------------------------------------------------------------------------
@@ -1760,15 +1770,15 @@
     # --------------------------------------------------------------------------------------------------
     if(payeh):
         if(show_progress):
             clear_output(wait=True)
             print('Gathering Payeh market stock list ...')
         url = "https://www.ifb.ir/StockQoute.aspx"
         header = {"__EVENTTARGET": "exportbtn"}
-        response = requests.post(url, header)
+        response = requests.post(url, header, verify=False)
         table = pd.read_html(response.content.decode('utf-8'))[0]
         payeh_lookup = table.iloc[2:,:3]
         payeh_lookup.columns = ['Ticker','Name','Market']
         payeh_lookup = payeh_lookup[payeh_lookup['Market'].isin(['تابلو پایه زرد','تابلو پایه نارنجی','تابلو پایه قرمز'])] 
         payeh_lookup['Market'] = payeh_lookup['Market'].apply(lambda x: (x.replace('تابلو','')).strip())
         # drop other than normal trades:
         payeh_lookup = payeh_lookup[payeh_lookup['Ticker'].apply(lambda x: x[-1].isdigit())==False]
```

### Comparing `finpy_tse-1.2.0/finpy_tse.egg-info/PKG-INFO` & `finpy_tse-1.2.1/finpy_tse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finpy-tse
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data
 Author: ALI RAHIMI  AND  RASOOL GHAFOURI
 Author-email: a.rahimi.aut@gmail.com
 License: BSD (3-clause)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `finpy_tse-1.2.0/setup.py` & `finpy_tse-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='finpy_tse',                           # should match the package folder
     packages=['finpy_tse'],                     # should match the package folder
-    version='1.2.0',                                # important for updates
+    version='1.2.1',                                # important for updates
     license='BSD (3-clause)',                                  # should match your chosen license
     description='A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='ALI RAHIMI  AND  RASOOL GHAFOURI',
     author_email='a.rahimi.aut@gmail.com',
     install_requires=['requests','jdatetime','pandas','numpy','requests','bs4','asyncio','urllib3','aiohttp','unsync','IPython','persiantools','datetime','XlsxWriter','lxml'],                  # list all packages that your package uses
```

