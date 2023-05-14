# Comparing `tmp/lixinger-0.1.8.tar.gz` & `tmp/lixinger-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lixinger-0.1.8.tar", last modified: Sat May 13 04:19:31 2023, max compression
+gzip compressed data, was "lixinger-0.1.9.tar", last modified: Sun May 14 10:45:18 2023, max compression
```

## Comparing `lixinger-0.1.8.tar` & `lixinger-0.1.9.tar`

### file list

```diff
@@ -1,58 +1,60 @@
--rw-r--r--   0        0        0     1541 2023-05-13 04:11:28.122994 lixinger-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.8/lixinger/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.8/lixinger/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.8/lixinger/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.8/lixinger/api/cn/company/__init__.py
--rw-r--r--   0        0        0     1859 2023-05-13 04:08:14.276289 lixinger-0.1.8/lixinger/api/cn/company/base.py
--rw-r--r--   0        0        0     1230 2023-05-13 04:19:14.460488 lixinger-0.1.8/lixinger/api/cn/company/block_deal.py
--rw-r--r--   0        0        0     1614 2023-05-13 04:19:14.460546 lixinger-0.1.8/lixinger/api/cn/company/candlestick.py
--rw-r--r--   0        0        0     1803 2023-05-13 04:19:14.460598 lixinger-0.1.8/lixinger/api/cn/company/dividend_and_alloment.py
--rw-r--r--   0        0        0     1174 2023-05-13 04:19:14.460648 lixinger-0.1.8/lixinger/api/cn/company/equity_change.py
--rw-r--r--   0        0        0      851 2023-05-13 04:19:14.460700 lixinger-0.1.8/lixinger/api/cn/company/indices.py
--rw-r--r--   0        0        0      860 2023-05-13 04:19:14.460763 lixinger-0.1.8/lixinger/api/cn/company/industries.py
--rw-r--r--   0        0        0     2014 2023-05-13 04:19:14.460814 lixinger-0.1.8/lixinger/api/cn/company/pledge.py
--rw-r--r--   0        0        0     1361 2023-05-13 04:19:14.460866 lixinger-0.1.8/lixinger/api/cn/company/senior_executive_shares_change.py
--rw-r--r--   0        0        0     1010 2023-05-13 04:19:14.460914 lixinger-0.1.8/lixinger/api/cn/company/shareholders_num.py
--rw-r--r--   0        0        0        0 2023-05-04 14:21:25.826889 lixinger-0.1.8/lixinger/api/cn/fund/__init__.py
--rw-r--r--   0        0        0     1146 2023-05-13 04:19:14.460966 lixinger-0.1.8/lixinger/api/cn/fund/exchange_traded_close_price.py
--rw-r--r--   0        0        0     1021 2023-05-13 04:19:14.461016 lixinger-0.1.8/lixinger/api/cn/fund/total_net_value.py
--rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.8/lixinger/api/cn/index/__init__.py
--rw-r--r--   0        0        0     1630 2023-05-13 04:19:14.461073 lixinger-0.1.8/lixinger/api/cn/index/base.py
--rw-r--r--   0        0        0     1290 2023-05-13 04:19:14.461123 lixinger-0.1.8/lixinger/api/cn/index/candlestick.py
--rw-r--r--   0        0        0     1279 2023-05-13 04:19:14.461171 lixinger-0.1.8/lixinger/api/cn/index/constituents.py
--rw-r--r--   0        0        0     1002 2023-05-13 04:19:14.461221 lixinger-0.1.8/lixinger/api/cn/index/drawdown.py
--rw-r--r--   0        0        0     1521 2023-05-13 04:19:14.461272 lixinger-0.1.8/lixinger/api/cn/index/fundamental.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.8/lixinger/api/hk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.8/lixinger/api/macro/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.8/lixinger/api/us/__init__.py
--rw-r--r--   0        0        0      520 2023-05-13 04:19:14.461320 lixinger-0.1.8/lixinger/client.py
--rw-r--r--   0        0        0     1644 2023-05-10 14:14:18.924307 lixinger-0.1.8/lixinger/config.py
--rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.8/lixinger/py.typed
--rw-r--r--   0        0        0       75 2023-05-03 10:06:41.922780 lixinger-0.1.8/lixinger/settings.toml
--rw-r--r--   0        0        0     5700 2023-05-13 03:33:48.391570 lixinger-0.1.8/lixinger/utils.py
--rw-r--r--   0        0        0      935 2023-05-13 04:19:31.962265 lixinger-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.8/tests/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.8/tests/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.8/tests/api/cn/company/__init__.py
--rw-r--r--   0        0        0      127 2023-05-10 13:55:25.017569 lixinger-0.1.8/tests/api/cn/company/test_base.py
--rw-r--r--   0        0        0      164 2023-05-08 14:09:59.839924 lixinger-0.1.8/tests/api/cn/company/test_block_deal.py
--rw-r--r--   0        0        0      187 2023-05-10 14:12:30.362480 lixinger-0.1.8/tests/api/cn/company/test_candlestick.py
--rw-r--r--   0        0        0      217 2023-05-06 05:43:46.770904 lixinger-0.1.8/tests/api/cn/company/test_dividend_and_alloment.py
--rw-r--r--   0        0        0      170 2023-05-06 02:12:57.131245 lixinger-0.1.8/tests/api/cn/company/test_equity_change.py
--rw-r--r--   0        0        0      127 2023-05-09 12:28:07.598154 lixinger-0.1.8/tests/api/cn/company/test_indices.py
--rw-r--r--   0        0        0      139 2023-05-10 12:17:30.914094 lixinger-0.1.8/tests/api/cn/company/test_industries.py
--rw-r--r--   0        0        0      144 2023-05-08 14:53:32.432310 lixinger-0.1.8/tests/api/cn/company/test_pledge.py
--rw-r--r--   0        0        0      235 2023-05-07 15:03:11.303695 lixinger-0.1.8/tests/api/cn/company/test_senior_executive_shares_change.py
--rw-r--r--   0        0        0      184 2023-05-07 14:29:15.357398 lixinger-0.1.8/tests/api/cn/company/test_shareholders_num.py
--rw-r--r--   0        0        0        0 2023-05-04 14:30:00.736254 lixinger-0.1.8/tests/api/cn/fund/__init__.py
--rw-r--r--   0        0        0      238 2023-05-07 02:06:30.724314 lixinger-0.1.8/tests/api/cn/fund/test_exchange_traded_close_price.py
--rw-r--r--   0        0        0      229 2023-05-04 14:32:35.703103 lixinger-0.1.8/tests/api/cn/fund/test_total_net_value.py
--rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.8/tests/api/cn/index/__init__.py
--rw-r--r--   0        0        0      119 2023-05-11 15:51:33.137778 lixinger-0.1.8/tests/api/cn/index/test_base.py
--rw-r--r--   0        0        0      182 2023-05-07 01:58:13.309631 lixinger-0.1.8/tests/api/cn/index/test_candlestick.py
--rw-r--r--   0        0        0      196 2023-05-13 03:50:07.787874 lixinger-0.1.8/tests/api/cn/index/test_constituents.py
--rw-r--r--   0        0        0      212 2023-05-12 15:25:25.088245 lixinger-0.1.8/tests/api/cn/index/test_drawdown.py
--rw-r--r--   0        0        0      270 2023-05-10 13:23:11.920162 lixinger-0.1.8/tests/api/cn/index/test_fundamental.py
--rw-r--r--   0        0        0      112 2023-05-13 03:56:27.328013 lixinger-0.1.8/tests/conftest.py
--rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 lixinger-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1541 2023-05-13 04:11:28.122994 lixinger-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.9/lixinger/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.9/lixinger/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.9/lixinger/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.9/lixinger/api/cn/company/__init__.py
+-rw-r--r--   0        0        0     1859 2023-05-13 04:08:14.276289 lixinger-0.1.9/lixinger/api/cn/company/base.py
+-rw-r--r--   0        0        0     1230 2023-05-13 04:19:14.460488 lixinger-0.1.9/lixinger/api/cn/company/block_deal.py
+-rw-r--r--   0        0        0     1614 2023-05-13 04:19:14.460546 lixinger-0.1.9/lixinger/api/cn/company/candlestick.py
+-rw-r--r--   0        0        0     1803 2023-05-13 04:19:14.460598 lixinger-0.1.9/lixinger/api/cn/company/dividend_and_alloment.py
+-rw-r--r--   0        0        0     1174 2023-05-13 04:19:14.460648 lixinger-0.1.9/lixinger/api/cn/company/equity_change.py
+-rw-r--r--   0        0        0      968 2023-05-14 10:44:23.539363 lixinger-0.1.9/lixinger/api/cn/company/fundamental_statistics.py
+-rw-r--r--   0        0        0      851 2023-05-13 04:19:14.460700 lixinger-0.1.9/lixinger/api/cn/company/indices.py
+-rw-r--r--   0        0        0      860 2023-05-13 04:19:14.460763 lixinger-0.1.9/lixinger/api/cn/company/industries.py
+-rw-r--r--   0        0        0     2014 2023-05-13 04:19:14.460814 lixinger-0.1.9/lixinger/api/cn/company/pledge.py
+-rw-r--r--   0        0        0     1361 2023-05-13 04:19:14.460866 lixinger-0.1.9/lixinger/api/cn/company/senior_executive_shares_change.py
+-rw-r--r--   0        0        0     1010 2023-05-13 04:19:14.460914 lixinger-0.1.9/lixinger/api/cn/company/shareholders_num.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:21:25.826889 lixinger-0.1.9/lixinger/api/cn/fund/__init__.py
+-rw-r--r--   0        0        0     1146 2023-05-13 04:19:14.460966 lixinger-0.1.9/lixinger/api/cn/fund/exchange_traded_close_price.py
+-rw-r--r--   0        0        0     1021 2023-05-13 04:19:14.461016 lixinger-0.1.9/lixinger/api/cn/fund/total_net_value.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.9/lixinger/api/cn/index/__init__.py
+-rw-r--r--   0        0        0     1630 2023-05-13 04:19:14.461073 lixinger-0.1.9/lixinger/api/cn/index/base.py
+-rw-r--r--   0        0        0     1290 2023-05-13 04:19:14.461123 lixinger-0.1.9/lixinger/api/cn/index/candlestick.py
+-rw-r--r--   0        0        0     1279 2023-05-13 04:19:14.461171 lixinger-0.1.9/lixinger/api/cn/index/constituents.py
+-rw-r--r--   0        0        0     1002 2023-05-13 04:19:14.461221 lixinger-0.1.9/lixinger/api/cn/index/drawdown.py
+-rw-r--r--   0        0        0     1521 2023-05-13 04:19:14.461272 lixinger-0.1.9/lixinger/api/cn/index/fundamental.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.9/lixinger/api/hk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.9/lixinger/api/macro/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.9/lixinger/api/us/__init__.py
+-rw-r--r--   0        0        0      520 2023-05-13 04:19:14.461320 lixinger-0.1.9/lixinger/client.py
+-rw-r--r--   0        0        0     1644 2023-05-10 14:14:18.924307 lixinger-0.1.9/lixinger/config.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.9/lixinger/py.typed
+-rw-r--r--   0        0        0       75 2023-05-03 10:06:41.922780 lixinger-0.1.9/lixinger/settings.toml
+-rw-r--r--   0        0        0     5700 2023-05-13 03:33:48.391570 lixinger-0.1.9/lixinger/utils.py
+-rw-r--r--   0        0        0     1055 2023-05-14 10:45:18.314302 lixinger-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.9/tests/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.9/tests/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.9/tests/api/cn/company/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-10 13:55:25.017569 lixinger-0.1.9/tests/api/cn/company/test_base.py
+-rw-r--r--   0        0        0      164 2023-05-08 14:09:59.839924 lixinger-0.1.9/tests/api/cn/company/test_block_deal.py
+-rw-r--r--   0        0        0      187 2023-05-10 14:12:30.362480 lixinger-0.1.9/tests/api/cn/company/test_candlestick.py
+-rw-r--r--   0        0        0      217 2023-05-06 05:43:46.770904 lixinger-0.1.9/tests/api/cn/company/test_dividend_and_alloment.py
+-rw-r--r--   0        0        0      170 2023-05-06 02:12:57.131245 lixinger-0.1.9/tests/api/cn/company/test_equity_change.py
+-rw-r--r--   0        0        0      262 2023-05-14 10:45:06.410848 lixinger-0.1.9/tests/api/cn/company/test_fundamental_statistics.py
+-rw-r--r--   0        0        0      127 2023-05-09 12:28:07.598154 lixinger-0.1.9/tests/api/cn/company/test_indices.py
+-rw-r--r--   0        0        0      139 2023-05-10 12:17:30.914094 lixinger-0.1.9/tests/api/cn/company/test_industries.py
+-rw-r--r--   0        0        0      144 2023-05-08 14:53:32.432310 lixinger-0.1.9/tests/api/cn/company/test_pledge.py
+-rw-r--r--   0        0        0      235 2023-05-07 15:03:11.303695 lixinger-0.1.9/tests/api/cn/company/test_senior_executive_shares_change.py
+-rw-r--r--   0        0        0      184 2023-05-07 14:29:15.357398 lixinger-0.1.9/tests/api/cn/company/test_shareholders_num.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:30:00.736254 lixinger-0.1.9/tests/api/cn/fund/__init__.py
+-rw-r--r--   0        0        0      238 2023-05-07 02:06:30.724314 lixinger-0.1.9/tests/api/cn/fund/test_exchange_traded_close_price.py
+-rw-r--r--   0        0        0      229 2023-05-04 14:32:35.703103 lixinger-0.1.9/tests/api/cn/fund/test_total_net_value.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.9/tests/api/cn/index/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-11 15:51:33.137778 lixinger-0.1.9/tests/api/cn/index/test_base.py
+-rw-r--r--   0        0        0      182 2023-05-07 01:58:13.309631 lixinger-0.1.9/tests/api/cn/index/test_candlestick.py
+-rw-r--r--   0        0        0      196 2023-05-13 03:50:07.787874 lixinger-0.1.9/tests/api/cn/index/test_constituents.py
+-rw-r--r--   0        0        0      212 2023-05-12 15:25:25.088245 lixinger-0.1.9/tests/api/cn/index/test_drawdown.py
+-rw-r--r--   0        0        0      270 2023-05-10 13:23:11.920162 lixinger-0.1.9/tests/api/cn/index/test_fundamental.py
+-rw-r--r--   0        0        0      112 2023-05-13 03:56:27.328013 lixinger-0.1.9/tests/conftest.py
+-rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 lixinger-0.1.9/PKG-INFO
```

### Comparing `lixinger-0.1.8/README.md` & `lixinger-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/company/base.py` & `lixinger-0.1.9/lixinger/api/cn/company/base.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/company/block_deal.py` & `lixinger-0.1.9/lixinger/api/cn/company/block_deal.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/company/candlestick.py` & `lixinger-0.1.9/lixinger/api/cn/company/candlestick.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/company/dividend_and_alloment.py` & `lixinger-0.1.9/lixinger/api/cn/company/dividend_and_alloment.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/company/equity_change.py` & `lixinger-0.1.9/lixinger/api/cn/company/equity_change.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/company/indices.py` & `lixinger-0.1.9/lixinger/api/cn/company/indices.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/company/industries.py` & `lixinger-0.1.9/lixinger/api/cn/company/industries.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/company/pledge.py` & `lixinger-0.1.9/lixinger/api/cn/company/pledge.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/company/senior_executive_shares_change.py` & `lixinger-0.1.9/lixinger/api/cn/company/senior_executive_shares_change.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/company/shareholders_num.py` & `lixinger-0.1.9/lixinger/api/cn/company/shareholders_num.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/fund/exchange_traded_close_price.py` & `lixinger-0.1.9/lixinger/api/cn/fund/exchange_traded_close_price.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/fund/total_net_value.py` & `lixinger-0.1.9/lixinger/api/cn/fund/total_net_value.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/index/base.py` & `lixinger-0.1.9/lixinger/api/cn/index/base.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/index/candlestick.py` & `lixinger-0.1.9/lixinger/api/cn/index/candlestick.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/index/constituents.py` & `lixinger-0.1.9/lixinger/api/cn/index/constituents.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/index/drawdown.py` & `lixinger-0.1.9/lixinger/api/cn/index/drawdown.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/api/cn/index/fundamental.py` & `lixinger-0.1.9/lixinger/api/cn/index/fundamental.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/client.py` & `lixinger-0.1.9/lixinger/client.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/config.py` & `lixinger-0.1.9/lixinger/config.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/lixinger/utils.py` & `lixinger-0.1.9/lixinger/utils.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.8/pyproject.toml` & `lixinger-0.1.9/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [tool.pytest.ini_options]
 cache_dir = ".pytest_cache/"
 addopts = "-s -p no:warnings"
 asyncio_mode = "auto"
 
 [project]
 name = "lixinger"
-version = "0.1.8"
+version = "0.1.9"
 description = "Lixinger SDK for Python (Unofficial)"
 authors = [
     { name = "Chaoying", email = "chaoying2022@gmail.com" },
 ]
 dependencies = [
     "pandera>=0.14.5",
     "pydantic>=1.10.7",
@@ -35,12 +35,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [project.license]
 text = "MIT"
 
+[project.urls]
+Homepage = "https://github.com/Chaoyingz/lixinger"
+Repository = "https://github.com/Chaoyingz/lixinger"
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `lixinger-0.1.8/PKG-INFO` & `lixinger-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: lixinger
-Version: 0.1.8
+Version: 0.1.9
 Summary: Lixinger SDK for Python (Unofficial)
 Keywords: lixinger
 Author-Email: Chaoying <chaoying2022@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Homepage, https://github.com/Chaoyingz/lixinger
+Project-URL: Repository, https://github.com/Chaoyingz/lixinger
 Requires-Python: >=3.8
 Requires-Dist: pandera>=0.14.5
 Requires-Dist: pydantic>=1.10.7
 Requires-Dist: requests>=2.29.0
 Requires-Dist: dynaconf>=3.1.12
 Requires-Dist: tenacity>=8.2.2
 Description-Content-Type: text/markdown
```

