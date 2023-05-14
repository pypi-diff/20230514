# Comparing `tmp/quant_invest_ab-0.1.0.tar.gz` & `tmp/quant_invest_ab-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant_invest_ab-0.1.0.tar", max compression
+gzip compressed data, was "quant_invest_ab-0.2.0.tar", max compression
```

## Comparing `quant_invest_ab-0.1.0.tar` & `quant_invest_ab-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1994 2023-05-14 18:11:45.604751 quant_invest_ab-0.1.0/README.md
--rw-r--r--   0        0        0      977 2023-05-14 17:31:55.684751 quant_invest_ab-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    18278 2023-05-14 17:42:39.234752 quant_invest_ab-0.1.0/quant_invest_lab/backtest.py
--rw-r--r--   0        0        0    17111 2023-05-14 17:05:21.454752 quant_invest_ab-0.1.0/quant_invest_lab/data_provider.py
--rw-r--r--   0        0        0    19099 2023-05-14 17:22:56.994752 quant_invest_ab-0.1.0/quant_invest_lab/indicators.py
--rw-r--r--   0        0        0     8038 2023-05-14 15:47:17.294752 quant_invest_ab-0.1.0/quant_invest_lab/metrics.py
--rw-r--r--   0        0        0    20361 2023-05-14 18:09:36.804750 quant_invest_ab-0.1.0/quant_invest_lab/portfolio.py
--rw-r--r--   0        0        0     3577 2023-05-14 17:30:20.244749 quant_invest_ab-0.1.0/quant_invest_lab/screener.py
--rw-r--r--   0        0        0     8477 2023-05-14 17:22:27.984752 quant_invest_ab-0.1.0/quant_invest_lab/simulation.py
--rw-r--r--   0        0        0     1107 2023-05-14 17:21:39.694751 quant_invest_ab-0.1.0/quant_invest_lab/utils.py
--rw-r--r--   0        0        0     3279 1970-01-01 00:00:00.000000 quant_invest_ab-0.1.0/setup.py
--rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 quant_invest_ab-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1994 2023-05-14 18:11:45.604751 quant_invest_ab-0.2.0/README.md
+-rw-r--r--   0        0        0      977 2023-05-14 18:13:44.504753 quant_invest_ab-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    18278 2023-05-14 17:42:39.234752 quant_invest_ab-0.2.0/quant_invest_lab/backtest.py
+-rw-r--r--   0        0        0    17111 2023-05-14 17:05:21.454752 quant_invest_ab-0.2.0/quant_invest_lab/data_provider.py
+-rw-r--r--   0        0        0    19099 2023-05-14 17:22:56.994752 quant_invest_ab-0.2.0/quant_invest_lab/indicators.py
+-rw-r--r--   0        0        0     8038 2023-05-14 15:47:17.294752 quant_invest_ab-0.2.0/quant_invest_lab/metrics.py
+-rw-r--r--   0        0        0    20361 2023-05-14 18:09:36.804750 quant_invest_ab-0.2.0/quant_invest_lab/portfolio.py
+-rw-r--r--   0        0        0     3577 2023-05-14 17:30:20.244749 quant_invest_ab-0.2.0/quant_invest_lab/screener.py
+-rw-r--r--   0        0        0     8477 2023-05-14 17:22:27.984752 quant_invest_ab-0.2.0/quant_invest_lab/simulation.py
+-rw-r--r--   0        0        0     1107 2023-05-14 17:21:39.694751 quant_invest_ab-0.2.0/quant_invest_lab/utils.py
+-rw-r--r--   0        0        0     3279 1970-01-01 00:00:00.000000 quant_invest_ab-0.2.0/setup.py
+-rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 quant_invest_ab-0.2.0/PKG-INFO
```

### Comparing `quant_invest_ab-0.1.0/README.md` & `quant_invest_ab-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `quant_invest_ab-0.1.0/pyproject.toml` & `quant_invest_ab-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quant-invest-ab"
-version = "0.1.0"
+version = "0.2.0"
 description = "Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project."
 authors = ["BaptisteZloch <bzloch@hotmail.fr>"]
 readme = "README.md"
 packages = [{include = "quant_invest_lab"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `quant_invest_ab-0.1.0/quant_invest_lab/backtest.py` & `quant_invest_ab-0.2.0/quant_invest_lab/backtest.py`

 * *Files identical despite different names*

### Comparing `quant_invest_ab-0.1.0/quant_invest_lab/data_provider.py` & `quant_invest_ab-0.2.0/quant_invest_lab/data_provider.py`

 * *Files identical despite different names*

### Comparing `quant_invest_ab-0.1.0/quant_invest_lab/indicators.py` & `quant_invest_ab-0.2.0/quant_invest_lab/indicators.py`

 * *Files identical despite different names*

### Comparing `quant_invest_ab-0.1.0/quant_invest_lab/metrics.py` & `quant_invest_ab-0.2.0/quant_invest_lab/metrics.py`

 * *Files identical despite different names*

### Comparing `quant_invest_ab-0.1.0/quant_invest_lab/portfolio.py` & `quant_invest_ab-0.2.0/quant_invest_lab/portfolio.py`

 * *Files identical despite different names*

### Comparing `quant_invest_ab-0.1.0/quant_invest_lab/screener.py` & `quant_invest_ab-0.2.0/quant_invest_lab/screener.py`

 * *Files identical despite different names*

### Comparing `quant_invest_ab-0.1.0/quant_invest_lab/simulation.py` & `quant_invest_ab-0.2.0/quant_invest_lab/simulation.py`

 * *Files identical despite different names*

### Comparing `quant_invest_ab-0.1.0/quant_invest_lab/utils.py` & `quant_invest_ab-0.2.0/quant_invest_lab/utils.py`

 * *Files identical despite different names*

### Comparing `quant_invest_ab-0.1.0/setup.py` & `quant_invest_ab-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'seaborn>=0.12.2,<0.13.0',
  'statsmodels>=0.14.0,<0.15.0',
  'ta>=0.10.2,<0.11.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'quant-invest-ab',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project.',
     'long_description': '# Quant Invest Lab\n**Quant Invest Lab** is a project aimed to provide a set of basic tools for quantitative experiments. By quantitative experiment I mean trying to build you own set of investments solution. The project is still in its early stage, but I hope it will grow in the future.\n\nInitially this project was aimed to be a set of tools for my own experiments, but I decided to make it open source. Of courses it already exists some awesome packages, more detailed, better suited for some use cases. But I hope it will be useful for someone else. Feel free to use it, modify it and contribute to it.*\n## Main features\n- **Data**: download data from external data provider without restriction on candle stick, the main provider is kucoin for now (currently only crypto data are supported).\n- **Backtesting**: backtest your trading strategy (Long only for now but soon short and leverage) on historical data for different timeframe. Optimize you take profit, stop loss. Access full metrics of your strategy.\n- **Indicators**: a set of indicators to help you build your strategy.\n- **Portfolio**: a set of portfolio optimization tools to help you build your portfolio.\n- **Simulation**: simulate your data based on real data using statistics to get a better understanding of its behavior during backtesting.\n- **Metrics**: a set of metrics to help you evaluate your strategy through performances and risks.\n\n## Installation\nTo install **Quant Invest Lab** through pip, run the following command:\n```bash\npip install quant-invest-lab --upgrade\n```\nYou can install it using poetry the same way :\n```bash\npoetry add quant-invest-lab\n```\n\n# Basic examples\n## Backtest a basic EMA crossover strategy\n```python\n``` \n\n## Next steps create official docs and add more examples\n## Disclaimer\nThis package is only for educational purpose or experimentation it is not intended to be used in production. I am not responsible for any loss of money you may have using this package. Use it at your own risk.',
     'author': 'BaptisteZloch',
     'author_email': 'bzloch@hotmail.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `quant_invest_ab-0.1.0/PKG-INFO` & `quant_invest_ab-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant-invest-ab
-Version: 0.1.0
+Version: 0.2.0
 Summary: Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project.
 Author: BaptisteZloch
 Author-email: bzloch@hotmail.fr
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

