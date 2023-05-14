# Comparing `tmp/xzy-db-0.0.2.tar.gz` & `tmp/xzy-db-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xzy-db-0.0.2.tar", last modified: Sat May 13 00:56:13 2023, max compression
+gzip compressed data, was "xzy-db-0.0.3.tar", last modified: Sun May 14 02:29:14 2023, max compression
```

## Comparing `xzy-db-0.0.2.tar` & `xzy-db-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-13 00:56:13.485214 xzy-db-0.0.2/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      523 2023-05-13 00:56:13.485214 xzy-db-0.0.2/PKG-INFO
--rw-r--r--   0 liubola   (1000) liubola   (1000)       40 2023-01-13 02:27:03.000000 xzy-db-0.0.2/README.md
--rw-r--r--   0 liubola   (1000) liubola   (1000)       38 2023-05-13 00:56:13.485214 xzy-db-0.0.2/setup.cfg
--rw-r--r--   0 liubola   (1000) liubola   (1000)      914 2023-05-13 00:56:13.000000 xzy-db-0.0.2/setup.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-13 00:56:13.475214 xzy-db-0.0.2/xzy_db/
--rw-r--r--   0 liubola   (1000) liubola   (1000)       62 2023-05-13 00:53:10.000000 xzy-db-0.0.2/xzy_db/__init__.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-13 00:56:13.475214 xzy-db-0.0.2/xzy_db/api/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      322 2023-05-13 00:53:10.000000 xzy-db-0.0.2/xzy_db/api/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2207 2023-05-13 00:53:10.000000 xzy-db-0.0.2/xzy_db/api/get_fund_data.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2781 2023-05-13 00:53:10.000000 xzy-db-0.0.2/xzy_db/api/get_fund_list.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     3262 2023-05-13 00:53:10.000000 xzy-db-0.0.2/xzy_db/api/get_index_data.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2021 2023-05-13 00:53:10.000000 xzy-db-0.0.2/xzy_db/api/get_index_weight.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     4470 2023-05-13 00:53:10.000000 xzy-db-0.0.2/xzy_db/api/get_industry.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     3517 2023-05-13 00:53:10.000000 xzy-db-0.0.2/xzy_db/api/get_ret.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     5748 2023-05-13 00:53:10.000000 xzy-db-0.0.2/xzy_db/api/get_universe.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-13 00:56:13.485214 xzy-db-0.0.2/xzy_db/crawler/
--rw-r--r--   0 liubola   (1000) liubola   (1000)       46 2023-01-13 02:27:03.000000 xzy-db-0.0.2/xzy_db/crawler/__init__.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-13 00:56:13.485214 xzy-db-0.0.2/xzy_db/crawler/futures/
--rw-r--r--   0 liubola   (1000) liubola   (1000)        0 2023-01-13 02:27:03.000000 xzy-db-0.0.2/xzy_db/crawler/futures/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)    17469 2023-05-13 00:53:10.000000 xzy-db-0.0.2/xzy_db/crawler/futures/domestic.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     5254 2023-01-13 02:27:03.000000 xzy-db-0.0.2/xzy_db/crawler/futures/domestic_cons.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-13 00:56:13.485214 xzy-db-0.0.2/xzy_db/hk_sangreal_calendar/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      399 2023-05-13 00:53:10.000000 xzy-db-0.0.2/xzy_db/hk_sangreal_calendar/__init__.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-13 00:56:13.485214 xzy-db-0.0.2/xzy_db/sangreal_calendar/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      385 2023-05-13 00:55:56.000000 xzy-db-0.0.2/xzy_db/sangreal_calendar/__init__.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-13 00:56:13.485214 xzy-db-0.0.2/xzy_db/utils/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      112 2023-05-13 00:53:10.000000 xzy-db-0.0.2/xzy_db/utils/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2277 2023-03-30 06:40:40.000000 xzy-db-0.0.2/xzy_db/utils/commons.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)       93 2023-01-13 02:27:03.000000 xzy-db-0.0.2/xzy_db/utils/datetime_handle.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2437 2023-01-13 02:27:03.000000 xzy-db-0.0.2/xzy_db/utils/engines.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)      419 2023-01-13 02:27:03.000000 xzy-db-0.0.2/xzy_db/utils/fund_type.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-13 00:56:13.475214 xzy-db-0.0.2/xzy_db.egg-info/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      523 2023-05-13 00:56:13.000000 xzy-db-0.0.2/xzy_db.egg-info/PKG-INFO
--rw-r--r--   0 liubola   (1000) liubola   (1000)      746 2023-05-13 00:56:13.000000 xzy-db-0.0.2/xzy_db.egg-info/SOURCES.txt
--rw-r--r--   0 liubola   (1000) liubola   (1000)        1 2023-05-13 00:56:13.000000 xzy-db-0.0.2/xzy_db.egg-info/dependency_links.txt
--rw-r--r--   0 liubola   (1000) liubola   (1000)       55 2023-05-13 00:56:13.000000 xzy-db-0.0.2/xzy_db.egg-info/requires.txt
--rw-r--r--   0 liubola   (1000) liubola   (1000)        7 2023-05-13 00:56:13.000000 xzy-db-0.0.2/xzy_db.egg-info/top_level.txt
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      523 2023-05-14 02:29:14.074061 xzy-db-0.0.3/PKG-INFO
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       40 2023-01-13 02:27:03.000000 xzy-db-0.0.3/README.md
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       38 2023-05-14 02:29:14.074061 xzy-db-0.0.3/setup.cfg
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      914 2023-05-14 02:29:13.000000 xzy-db-0.0.3/setup.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       62 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/__init__.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/api/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      322 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/api/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2174 2023-05-14 02:23:05.000000 xzy-db-0.0.3/xzy_db/api/get_fund_data.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2781 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/api/get_fund_list.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     3262 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/api/get_index_data.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2021 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/api/get_index_weight.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     4470 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/api/get_industry.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     3534 2023-05-13 12:47:07.000000 xzy-db-0.0.3/xzy_db/api/get_ret.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     5755 2023-05-13 14:28:05.000000 xzy-db-0.0.3/xzy_db/api/get_universe.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/crawler/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       46 2023-01-13 02:27:03.000000 xzy-db-0.0.3/xzy_db/crawler/__init__.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/crawler/futures/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)        0 2023-01-13 02:27:03.000000 xzy-db-0.0.3/xzy_db/crawler/futures/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)    17469 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/crawler/futures/domestic.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     5254 2023-01-13 02:27:03.000000 xzy-db-0.0.3/xzy_db/crawler/futures/domestic_cons.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/hk_sangreal_calendar/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      399 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/hk_sangreal_calendar/__init__.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/sangreal_calendar/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      397 2023-05-13 12:44:00.000000 xzy-db-0.0.3/xzy_db/sangreal_calendar/__init__.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/utils/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      112 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/utils/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2277 2023-03-30 06:40:40.000000 xzy-db-0.0.3/xzy_db/utils/commons.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       93 2023-01-13 02:27:03.000000 xzy-db-0.0.3/xzy_db/utils/datetime_handle.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2436 2023-05-13 12:36:51.000000 xzy-db-0.0.3/xzy_db/utils/engines.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      419 2023-01-13 02:27:03.000000 xzy-db-0.0.3/xzy_db/utils/fund_type.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db.egg-info/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      523 2023-05-14 02:29:13.000000 xzy-db-0.0.3/xzy_db.egg-info/PKG-INFO
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      746 2023-05-14 02:29:13.000000 xzy-db-0.0.3/xzy_db.egg-info/SOURCES.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1000)        1 2023-05-14 02:29:13.000000 xzy-db-0.0.3/xzy_db.egg-info/dependency_links.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       55 2023-05-14 02:29:13.000000 xzy-db-0.0.3/xzy_db.egg-info/requires.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1000)        7 2023-05-14 02:29:13.000000 xzy-db-0.0.3/xzy_db.egg-info/top_level.txt
```

### Comparing `xzy-db-0.0.2/PKG-INFO` & `xzy-db-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xzy-db
-Version: 0.0.2
+Version: 0.0.3
 Summary: short cut api for wind
 Home-page: https://gitee.com/liubola/xzy-db
 Author: liubola
 Author-email: lby3523@gmail.com
 License: GNU General Public License v3.0
 Description: UNKNOWN
 Platform: all
```

### Comparing `xzy-db-0.0.2/setup.py` & `xzy-db-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xzy-db',
-    version='0.0.2',
+    version='0.0.3',
     description=('short cut api for wind'),
     install_requires=[
         'sangreal-db',
         'sangreal-calendar >= 0.0.36',
         'sqlalchemy',
         'attrs',
     ],
```

### Comparing `xzy-db-0.0.2/xzy_db/api/get_fund_data.py` & `xzy-db-0.0.3/xzy_db/api/get_fund_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,43 +14,44 @@
         end_dt {str} -- [description] (default: {'20990101'})
 
     Returns:
         [pd.DataFrame] -- [f_sid|trade_dt|s_close]
     """
 
     table = WIND_DB.CHINAMUTUALFUNDNAV
-    tmp_query = WIND_DB.query(table.F_INFO_WINDCODE, table.PRICE_DATE,
-                              table.F_NAV_ADJFACTOR, table.F_NAV_UNIT).filter(
-                                  table.PRICE_DATE >= begin_dt,
-                                  table.PRICE_DATE <= end_dt).order_by(
-                                      table.PRICE_DATE, table.F_INFO_WINDCODE)
+    tmp_query = WIND_DB.query(table.fcode, table.price_dt,
+                              table.adj_factor, table.nav_unit).filter(
+                                  table.price_dt >= begin_dt,
+                                  table.price_dt <= end_dt).order_by(
+                                      table.price_dt, table.fcode)
     try:
         if isinstance(fund_list, str):
             tmp_query = tmp_query.filter(func.substring(
-                table.F_INFO_WINDCODE, 1, 6) == fund_list[:6])
+                table.fcode, 1, 6) == fund_list[:6])
         elif isinstance(fund_list, Iterable):
             tmp_query = tmp_query.filter(func.substring(
-                table.F_INFO_WINDCODE, 1, 6).in_([f[:6] for f in fund_list]))
+                table.fcode, 1, 6).in_([f[:6] for f in fund_list]))
         else:
             pass
     except:
         if isinstance(fund_list, str):
             tmp_query = tmp_query.filter(func.substr(
-                table.F_INFO_WINDCODE, 1, 6) == fund_list[:6])
+                table.fcode, 1, 6) == fund_list[:6])
         elif isinstance(fund_list, Iterable):
             tmp_query = tmp_query.filter(func.substr(
-                table.F_INFO_WINDCODE, 1, 6).in_([f[:6] for f in fund_list]))
+                table.fcode, 1, 6).in_([f[:6] for f in fund_list]))
         else:
             pass
 
     df = tmp_query.to_df()
     df.columns = ['f_sid', 'trade_dt', 'adjfactor', 'unit']
     df['s_close'] = df['adjfactor'] * df['unit']
     df.drop(['unit', 'adjfactor'], axis=1, inplace=True)
     trade_dt_list = CALENDAR.dates
+    df.trade_dt = df.trade_dt.astype(str)
     df = df[df.trade_dt.isin(trade_dt_list)].reset_index(drop=True)
     return df
 
 
 if __name__ == '__main__':
     print(get_fund_nav('163407.OF'))
     # print(get_fund_nav(['000001.OF', '000002.OF']))
```

### Comparing `xzy-db-0.0.2/xzy_db/api/get_fund_list.py` & `xzy-db-0.0.3/xzy_db/api/get_fund_list.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.2/xzy_db/api/get_index_data.py` & `xzy-db-0.0.3/xzy_db/api/get_index_data.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.2/xzy_db/api/get_index_weight.py` & `xzy-db-0.0.3/xzy_db/api/get_index_weight.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.2/xzy_db/api/get_industry.py` & `xzy-db-0.0.3/xzy_db/api/get_industry.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.2/xzy_db/api/get_ret.py` & `xzy-db-0.0.3/xzy_db/api/get_ret.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,28 +27,29 @@
     if universe not in ('A', 'HK'):
         raise ValueError('universe only support A or HK!')
     begin_dt, end_dt = dt_handle(begin_dt), dt_handle(end_dt)
     if universe == 'A':
         table = getattr(WIND_DB, 'AShareEODPrices'.upper())
     else:
         table = getattr(WIND_DB, 'HKSHAREEODPRICES'.upper())
-    query = WIND_DB.query(table.S_INFO_WINDCODE, table.TRADE_DT,
-                          table.S_DQ_ADJCLOSE)
+    query = WIND_DB.query(table.stcode, table.trade_dt,
+                          table.adj_close)
     if sid is not None:
         if isinstance(sid, str):
-            query = query.filter(table.S_INFO_WINDCODE == sid)
+            query = query.filter(table.stcode == sid)
         else:
-            query = query.filter(table.S_INFO_WINDCODE.in_(sid))
+            query = query.filter(table.stcode.in_(sid))
 
     if trade_dt is not None:
         begin_dt = end_dt = dt_handle(trade_dt)
     df = query.filter(
         table.TRADE_DT >= step_trade_dt(begin_dt, -1), table.TRADE_DT <= end_dt).order_by(
             table.TRADE_DT).to_df()
     df.columns = ['sid', 'trade_dt', 'pct_change']
+    df['trade_dt'] = df['trade_dt'].astype(str)
     df = df.pivot(values='pct_change', index='trade_dt', columns='sid')
 
     # # 防止出现0的情况，强制缺失na
     df = df.pct_change(fill_method=None)
     df.dropna(how='all', inplace=True)
     return df.T
```

### Comparing `xzy-db-0.0.2/xzy_db/api/get_universe.py` & `xzy-db-0.0.3/xzy_db/api/get_universe.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,17 +104,17 @@
         return universe_normal(indx, cur_sign=cur_sign)
 
 
 @lru_cache()
 def get_all_normal_index(index):
     table = getattr(WIND_DB, 'AIndexMembers'.upper())
     df = WIND_DB.query(
-        table.S_CON_WINDCODE.label(
-            'sid'), table.S_CON_INDATE.label('entry_dt'),
-        table.S_CON_OUTDATE.label('out_dt')).filter(table.S_INFO_WINDCODE == index).to_df()
+        table.stcode.label(
+            'sid'), table.indate.label('entry_dt'),
+        table.outdate.label('out_dt')).filter(table.indexcode == index).to_df()
     return df
 
 
 @lru_cache()
 def get_all_msci():
     table = getattr(WIND_DB, 'AshareMSCIMembers'.upper())
     df = WIND_DB.query(table.S_INFO_WINDCODE.label('sid'),
@@ -187,14 +187,15 @@
             df = get_all_bond()
         elif self.index.endswith('HI'):
             df = get_all_hk(self.index)
         elif self.index != '':
             df = get_all_normal_index(self.index)
 
         trade_dt = dt_handle(trade_dt)
+        trade_dt = int(trade_dt)
         df = df.loc[(df['entry_dt'] <= trade_dt) & (
             (df['out_dt'] >= trade_dt) | (df['out_dt'].isnull()))]
         return set(df.sid)
 
 
 if __name__ == '__main__':
     f_list = DynamicUniverse('HS300').preview('20180105')
```

### Comparing `xzy-db-0.0.2/xzy_db/crawler/futures/domestic.py` & `xzy-db-0.0.3/xzy_db/crawler/futures/domestic.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.2/xzy_db/crawler/futures/domestic_cons.py` & `xzy-db-0.0.3/xzy_db/crawler/futures/domestic_cons.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.2/xzy_db/utils/commons.py` & `xzy-db-0.0.3/xzy_db/utils/commons.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.2/xzy_db/utils/engines.py` & `xzy-db-0.0.3/xzy_db/utils/engines.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import yaml
 from sangreal_db import DataBase
 from sqlalchemy import create_engine
 
 """""" """""" """""" """""" """""" ""
 "        读取配置文件内容         "
 """""" """""" """""" """""" """""" ""
-CONFIG_FILE_NAME = "wind.yaml"
+CONFIG_FILE_NAME = "xzy.yaml"
 HOME_PATH = os.path.expanduser(f'~{os.sep}.sangreal{os.sep}wind')
 if not os.path.exists(HOME_PATH):
     os.makedirs(HOME_PATH)
 CONFIG_FILE = os.path.join(HOME_PATH, CONFIG_FILE_NAME)
 
 YAML_TYPE = f"""
 wind.config:
```

### Comparing `xzy-db-0.0.2/xzy_db.egg-info/PKG-INFO` & `xzy-db-0.0.3/xzy_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xzy-db
-Version: 0.0.2
+Version: 0.0.3
 Summary: short cut api for wind
 Home-page: https://gitee.com/liubola/xzy-db
 Author: liubola
 Author-email: lby3523@gmail.com
 License: GNU General Public License v3.0
 Description: UNKNOWN
 Platform: all
```

### Comparing `xzy-db-0.0.2/xzy_db.egg-info/SOURCES.txt` & `xzy-db-0.0.3/xzy_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

