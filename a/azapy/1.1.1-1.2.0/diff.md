# Comparing `tmp/azapy-1.1.1.tar.gz` & `tmp/azapy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azapy-1.1.1.tar", last modified: Sun Apr  2 01:27:54 2023, max compression
+gzip compressed data, was "azapy-1.2.0.tar", last modified: Sat May 13 22:28:30 2023, max compression
```

## Comparing `azapy-1.1.1.tar` & `azapy-1.2.0.tar`

### file list

```diff
@@ -1,59 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 01:27:54.752852 azapy-1.1.1/
--rw-rw-rw-   0        0        0    35823 2023-04-01 04:52:56.000000 azapy-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     4566 2023-04-02 01:27:54.751850 azapy-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3855 2023-04-02 00:37:33.000000 azapy-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-02 01:27:54.691385 azapy-1.1.1/azapy/
-drwxrwxrwx   0        0        0        0 2023-04-02 01:27:54.696337 azapy-1.1.1/azapy/MkT/
--rw-rw-rw-   0        0        0     1272 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/MkT/MkTcalendar.py
--rw-rw-rw-   0        0        0    39621 2023-04-01 08:07:37.000000 azapy-1.1.1/azapy/MkT/MkTreader.py
--rw-rw-rw-   0        0        0       86 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/MkT/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/MkT/summary_MkTData.py
-drwxrwxrwx   0        0        0        0 2023-04-02 01:27:54.734236 azapy-1.1.1/azapy/PortOpt/
--rw-rw-rw-   0        0        0    30746 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/BTADAnalyzer.py
--rw-rw-rw-   0        0        0    31164 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/BTSDAnalyzer.py
--rw-rw-rw-   0        0        0    32168 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/CVaRAnalyzer.py
--rw-rw-rw-   0        0        0   107989 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/EVaRAnalyzer.py
--rw-rw-rw-   0        0        0    24543 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/GINIAnalyzer.py
--rw-rw-rw-   0        0        0     9857 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/KellyEngine.py
--rw-rw-rw-   0        0        0    32523 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/LSDAnalyzer.py
--rw-rw-rw-   0        0        0    31704 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/MADAnalyzer.py
--rw-rw-rw-   0        0        0    20356 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/MVAnalyzer.py
--rw-rw-rw-   0        0        0     5541 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_BTAD.py
--rw-rw-rw-   0        0        0     5429 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_BTSD.py
--rw-rw-rw-   0        0        0     6019 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_CVaR.py
--rw-rw-rw-   0        0        0     6862 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_ConstW.py
--rw-rw-rw-   0        0        0     5572 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_EVaR.py
--rw-rw-rw-   0        0        0     4869 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_GINI.py
--rw-rw-rw-   0        0        0      728 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_InvDD.py
--rw-rw-rw-   0        0        0      648 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_InvVar.py
--rw-rw-rw-   0        0        0     6488 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_InvVol.py
--rw-rw-rw-   0        0        0     2098 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_Kelly.py
--rw-rw-rw-   0        0        0     5010 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_LSD.py
--rw-rw-rw-   0        0        0     5087 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_MAD.py
--rw-rw-rw-   0        0        0     4808 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_MV.py
--rw-rw-rw-   0        0        0     9772 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_Rebalanced.py
--rw-rw-rw-   0        0        0      653 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_SD.py
--rw-rw-rw-   0        0        0     5337 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/Port_SMCR.py
--rw-rw-rw-   0        0        0    20965 2023-04-01 08:34:33.000000 azapy-1.1.1/azapy/PortOpt/Port_Simple.py
--rw-rw-rw-   0        0        0    20489 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/SDAnalyzer.py
--rw-rw-rw-   0        0        0    37660 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/SMCRAnalyzer.py
--rw-rw-rw-   0        0        0    80715 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/_RiskAnalyzer.py
--rw-rw-rw-   0        0        0     7885 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/_RiskEngine.py
--rw-rw-rw-   0        0        0      764 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/__init__.py
--rw-rw-rw-   0        0        0     6916 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/PortOpt/_solvers.py
--rw-rw-rw-   0        0        0      155 2023-04-02 01:27:02.000000 azapy-1.1.1/azapy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 01:27:54.738854 azapy-1.1.1/azapy/util/
--rw-rw-rw-   0        0        0     4842 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/util/MkTdata_util.py
--rw-rw-rw-   0        0        0      130 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/util/__init__.py
--rw-rw-rw-   0        0        0     3846 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/util/drawdown.py
--rw-rw-rw-   0        0        0     2503 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/util/gamblingKelly.py
--rw-rw-rw-   0        0        0     4868 2023-04-01 04:52:56.000000 azapy-1.1.1/azapy/util/schedule.py
-drwxrwxrwx   0        0        0        0 2023-04-02 01:27:54.743872 azapy-1.1.1/azapy.egg-info/
--rw-rw-rw-   0        0        0     4566 2023-04-02 01:27:54.000000 azapy-1.1.1/azapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2559 2023-04-02 01:27:54.000000 azapy-1.1.1/azapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 01:27:54.000000 azapy-1.1.1/azapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-04-02 01:27:54.000000 azapy-1.1.1/azapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-02 01:27:54.000000 azapy-1.1.1/azapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      101 2023-04-01 04:52:56.000000 azapy-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-02 01:27:54.752852 azapy-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1362 2023-04-02 01:27:14.000000 azapy-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.424109 azapy-1.2.0/
+-rw-rw-rw-   0        0        0    35823 2022-12-13 09:07:48.000000 azapy-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4777 2023-05-13 22:28:30.423111 azapy-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4066 2023-05-13 22:26:42.000000 azapy-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.347747 azapy-1.2.0/azapy/
+drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.362352 azapy-1.2.0/azapy/Analyzers/
+-rw-rw-rw-   0        0        0    33510 2023-05-12 06:16:31.000000 azapy-1.2.0/azapy/Analyzers/BTADAnalyzer.py
+-rw-rw-rw-   0        0        0    33889 2023-05-12 06:28:16.000000 azapy-1.2.0/azapy/Analyzers/BTSDAnalyzer.py
+-rw-rw-rw-   0        0        0    34639 2023-05-12 06:33:17.000000 azapy-1.2.0/azapy/Analyzers/CVaRAnalyzer.py
+-rw-rw-rw-   0        0        0   110492 2023-05-12 06:33:17.000000 azapy-1.2.0/azapy/Analyzers/EVaRAnalyzer.py
+-rw-rw-rw-   0        0        0    27119 2023-05-12 06:33:17.000000 azapy-1.2.0/azapy/Analyzers/GINIAnalyzer.py
+-rw-rw-rw-   0        0        0    34991 2023-05-12 06:45:21.000000 azapy-1.2.0/azapy/Analyzers/LSDAnalyzer.py
+-rw-rw-rw-   0        0        0    34185 2023-05-12 06:45:21.000000 azapy-1.2.0/azapy/Analyzers/MADAnalyzer.py
+-rw-rw-rw-   0        0        0    22806 2023-05-12 06:45:21.000000 azapy-1.2.0/azapy/Analyzers/MVAnalyzer.py
+-rw-rw-rw-   0        0        0    22965 2023-05-12 06:45:21.000000 azapy-1.2.0/azapy/Analyzers/SDAnalyzer.py
+-rw-rw-rw-   0        0        0    40136 2023-05-12 06:45:21.000000 azapy-1.2.0/azapy/Analyzers/SMCRAnalyzer.py
+-rw-rw-rw-   0        0        0    87044 2023-05-12 07:15:00.000000 azapy-1.2.0/azapy/Analyzers/_RiskAnalyzer.py
+-rw-rw-rw-   0        0        0      282 2023-04-02 04:58:03.000000 azapy-1.2.0/azapy/Analyzers/__init__.py
+-rw-rw-rw-   0        0        0     6918 2023-05-09 10:52:00.000000 azapy-1.2.0/azapy/Analyzers/_solvers.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.368597 azapy-1.2.0/azapy/Engines/
+-rw-rw-rw-   0        0        0     3159 2023-05-12 07:07:44.000000 azapy-1.2.0/azapy/Engines/ConstWEngine.py
+-rw-rw-rw-   0        0        0      564 2023-05-12 07:07:44.000000 azapy-1.2.0/azapy/Engines/InvDDEngine.py
+-rw-rw-rw-   0        0        0      490 2023-05-12 07:07:44.000000 azapy-1.2.0/azapy/Engines/InvVarEngine.py
+-rw-rw-rw-   0        0        0     2203 2023-05-12 07:07:44.000000 azapy-1.2.0/azapy/Engines/InvVolEngine.py
+-rw-rw-rw-   0        0        0    11177 2023-05-12 07:15:00.000000 azapy-1.2.0/azapy/Engines/KellyEngine.py
+-rw-rw-rw-   0        0        0    10169 2023-05-12 07:15:00.000000 azapy-1.2.0/azapy/Engines/_RiskEngine.py
+-rw-rw-rw-   0        0        0      143 2023-04-13 21:18:19.000000 azapy-1.2.0/azapy/Engines/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.372586 azapy-1.2.0/azapy/Generators/
+-rw-rw-rw-   0        0        0     8799 2023-05-12 07:20:44.000000 azapy-1.2.0/azapy/Generators/ModelPipeline.py
+-rw-rw-rw-   0        0        0    16203 2023-05-12 07:37:07.000000 azapy-1.2.0/azapy/Generators/Port_Generator.py
+-rw-rw-rw-   0        0        0    22241 2023-05-12 09:30:30.000000 azapy-1.2.0/azapy/Generators/Port_Simple.py
+-rw-rw-rw-   0        0        0       61 2023-04-16 00:46:11.000000 azapy-1.2.0/azapy/Generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.378980 azapy-1.2.0/azapy/MkT/
+-rw-rw-rw-   0        0        0     1201 2023-05-12 08:40:40.000000 azapy-1.2.0/azapy/MkT/MkTcalendar.py
+-rw-rw-rw-   0        0        0    38243 2023-05-12 08:48:44.000000 azapy-1.2.0/azapy/MkT/MkTreader.py
+-rw-rw-rw-   0        0        0      141 2023-05-04 05:46:31.000000 azapy-1.2.0/azapy/MkT/__init__.py
+-rw-rw-rw-   0        0        0     6552 2023-05-12 08:49:26.000000 azapy-1.2.0/azapy/MkT/readMkT.py
+-rw-rw-rw-   0        0        0     2748 2023-05-04 06:46:48.000000 azapy-1.2.0/azapy/MkT/summary_MkTdata.py
+-rw-rw-rw-   0        0        0     3176 2023-05-12 08:51:13.000000 azapy-1.2.0/azapy/MkT/update_MkTdata.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.397101 azapy-1.2.0/azapy/PortOpt/
+-rw-rw-rw-   0        0        0     5710 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_BTAD.py
+-rw-rw-rw-   0        0        0     5629 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_BTSD.py
+-rw-rw-rw-   0        0        0     5492 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_CVaR.py
+-rw-rw-rw-   0        0        0     1530 2023-05-12 08:07:47.000000 azapy-1.2.0/azapy/PortOpt/Port_ConstW.py
+-rw-rw-rw-   0        0        0     5623 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_EVaR.py
+-rw-rw-rw-   0        0        0     4931 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_GINI.py
+-rw-rw-rw-   0        0        0     1564 2023-05-12 08:10:37.000000 azapy-1.2.0/azapy/PortOpt/Port_InvDD.py
+-rw-rw-rw-   0        0        0     1558 2023-05-12 08:11:57.000000 azapy-1.2.0/azapy/PortOpt/Port_InvVar.py
+-rw-rw-rw-   0        0        0     1582 2023-05-12 08:11:57.000000 azapy-1.2.0/azapy/PortOpt/Port_InvVol.py
+-rw-rw-rw-   0        0        0     2231 2023-05-12 08:12:50.000000 azapy-1.2.0/azapy/PortOpt/Port_Kelly.py
+-rw-rw-rw-   0        0        0     5056 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_LSD.py
+-rw-rw-rw-   0        0        0     5162 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_MAD.py
+-rw-rw-rw-   0        0        0     4860 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_MV.py
+-rw-rw-rw-   0        0        0     6825 2023-05-12 08:22:23.000000 azapy-1.2.0/azapy/PortOpt/Port_Rebalanced.py
+-rw-rw-rw-   0        0        0     4868 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_SD.py
+-rw-rw-rw-   0        0        0     5393 2023-05-12 08:28:21.000000 azapy-1.2.0/azapy/PortOpt/Port_SMCR.py
+-rw-rw-rw-   0        0        0     5398 2023-05-13 05:13:25.000000 azapy-1.2.0/azapy/PortOpt/_Port_Generator.py
+-rw-rw-rw-   0        0        0      422 2023-04-17 21:10:54.000000 azapy-1.2.0/azapy/PortOpt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.401088 azapy-1.2.0/azapy/Selectors/
+-rw-rw-rw-   0        0        0     6485 2023-05-12 09:06:51.000000 azapy-1.2.0/azapy/Selectors/CorrClusterSelector.py
+-rw-rw-rw-   0        0        0     5129 2023-05-12 08:33:03.000000 azapy-1.2.0/azapy/Selectors/DualMomentumSelector.py
+-rw-rw-rw-   0        0        0     1496 2023-05-12 08:31:00.000000 azapy-1.2.0/azapy/Selectors/NullSelector.py
+-rw-rw-rw-   0        0        0      102 2023-05-07 21:41:02.000000 azapy-1.2.0/azapy/Selectors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.406976 azapy-1.2.0/azapy/Util/
+-rw-rw-rw-   0        0        0      135 2023-05-04 05:22:05.000000 azapy-1.2.0/azapy/Util/__init__.py
+-rw-rw-rw-   0        0        0     1570 2023-05-12 08:55:05.000000 azapy-1.2.0/azapy/Util/add_cash_security.py
+-rw-rw-rw-   0        0        0     3768 2023-05-12 09:04:21.000000 azapy-1.2.0/azapy/Util/drawdown.py
+-rw-rw-rw-   0        0        0     2493 2023-05-12 09:00:50.000000 azapy-1.2.0/azapy/Util/gamblingKelly.py
+-rw-rw-rw-   0        0        0     7246 2023-05-12 09:04:06.000000 azapy-1.2.0/azapy/Util/schedule.py
+-rw-rw-rw-   0        0        0      278 2023-05-13 16:59:44.000000 azapy-1.2.0/azapy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:28:30.410966 azapy-1.2.0/azapy.egg-info/
+-rw-rw-rw-   0        0        0     4777 2023-05-13 22:28:30.000000 azapy-1.2.0/azapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3639 2023-05-13 22:28:30.000000 azapy-1.2.0/azapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-13 22:28:30.000000 azapy-1.2.0/azapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-05-13 22:28:30.000000 azapy-1.2.0/azapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-13 22:28:30.000000 azapy-1.2.0/azapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      101 2022-12-13 09:07:48.000000 azapy-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-13 22:28:30.424109 azapy-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1362 2023-05-13 16:15:11.000000 azapy-1.2.0/setup.py
```

### Comparing `azapy-1.1.1/LICENSE` & `azapy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azapy-1.1.1/PKG-INFO` & `azapy-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azapy
-Version: 1.1.1
+Version: 1.2.0
 Summary: Financial Portfolio Optimization Algorithms
 Home-page: https://github.com/Mircea-MMXXI/azapy.git
 Author: Mircea Marinescu
 Author-email: mircea.marinescu@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://azapy.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/Mircea-MMXXI/azapy
@@ -42,15 +42,15 @@
   6. mBTSD - mixture BTSD (Below Threshold Semi-Deviation)
   7. GINI - Gini index (as in Corrado Gini statistician 1884-1965)
   8. SD - standard deviation
   9. MV - variance (as in mean-variance model)
   10. mEVaR - mixture EVaR (Entropic Value at Risk)
   <span style="color:red">(alpha version)</span>
 
-For each risk-based optimization class the following strategies are
+For each class of portfolio the following optimization strategies are
 available:
   1. Optimal-risk portfolio for targeted expected rate of return value
   2. Sharpe-optimal portfolio - maximization of generalized Sharpe ratio
   3. Sharpe-optimal portfolio - minimization of inverse generalized Sharpe
   ratio
   4. Minimum risk portfolio
   5. Optimal-risk portfolio for a fixed risk-aversion factor
@@ -79,14 +79,18 @@
      the asset absolute value of maximum drawdowns over a predefined
      historical period)
 
 C. Greedy portfolio optimization strategies:
   1. Kelly's portfolio (as in John Larry Kelly Jr. scientist 1923-1965) -
      maximization of portfolio log returns
 
+D. Market Selectors
+  1. Dual Momentum Selector <span style="color:red">(alpha version)</span>
+  2. Correlation Clustering Selector <span style="color:red">(alpha version)</span>
+
 Utility functions:
   * Collect historical market data from various providers.
     Supported providers:
 
     - yahoo.com
     - eodhistoricaldata.com
     - alphavantage.co
@@ -94,22 +98,21 @@
 
   * Generate business calendars. At this point only NYSE business calendar
     is implemented.
   * Generate rebalancing portfolio schedules.
   * Append a cash-like security to an existing market data object.
   * Update market data saved in a directory.
 
-
-The pollowing third-party packages were used with azapy 1.1.1
-* python 3.11.2
-* pandas 1.5.3
-* numpy 1.23.5
-* scipy 1.10.0
-* statsmodels 0.13.5
-* matplotlib 3.7.1
-* plotly 5.9.0
-* requests 2.28.1
-* pandas_market_calendars 4.1.4
-* ecos 2.0.12
-* cvxopt 1.3.0.1
-* ta 0.10.2
-* yfinance 0.2.14
+The following third-party packages were used with azapy 1.2.1:
+  * python 3.11.2
+  * pandas 1.5.3
+  * numpy 1.24.3
+  * scipy 1.10.1
+  * statsmodels 0.13.5
+  * matplotlib 3.7.1
+  * plotly 5.9.0
+  * requests 2.29.0
+  * pandas_market_calendars 4.1.4
+  * ecos 2.0.12
+  * cvxopt 1.3.0.1
+  * ta 0.10.2
+  * yfinance 0.2.14
```

### Comparing `azapy-1.1.1/README.md` & `azapy-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   6. mBTSD - mixture BTSD (Below Threshold Semi-Deviation)
   7. GINI - Gini index (as in Corrado Gini statistician 1884-1965)
   8. SD - standard deviation
   9. MV - variance (as in mean-variance model)
   10. mEVaR - mixture EVaR (Entropic Value at Risk)
   <span style="color:red">(alpha version)</span>
 
-For each risk-based optimization class the following strategies are
+For each class of portfolio the following optimization strategies are
 available:
   1. Optimal-risk portfolio for targeted expected rate of return value
   2. Sharpe-optimal portfolio - maximization of generalized Sharpe ratio
   3. Sharpe-optimal portfolio - minimization of inverse generalized Sharpe
   ratio
   4. Minimum risk portfolio
   5. Optimal-risk portfolio for a fixed risk-aversion factor
@@ -61,14 +61,18 @@
      the asset absolute value of maximum drawdowns over a predefined
      historical period)
 
 C. Greedy portfolio optimization strategies:
   1. Kelly's portfolio (as in John Larry Kelly Jr. scientist 1923-1965) -
      maximization of portfolio log returns
 
+D. Market Selectors
+  1. Dual Momentum Selector <span style="color:red">(alpha version)</span>
+  2. Correlation Clustering Selector <span style="color:red">(alpha version)</span>
+
 Utility functions:
   * Collect historical market data from various providers.
     Supported providers:
 
     - yahoo.com
     - eodhistoricaldata.com
     - alphavantage.co
@@ -76,22 +80,21 @@
 
   * Generate business calendars. At this point only NYSE business calendar
     is implemented.
   * Generate rebalancing portfolio schedules.
   * Append a cash-like security to an existing market data object.
   * Update market data saved in a directory.
 
-
-The pollowing third-party packages were used with azapy 1.1.1
-* python 3.11.2
-* pandas 1.5.3
-* numpy 1.23.5
-* scipy 1.10.0
-* statsmodels 0.13.5
-* matplotlib 3.7.1
-* plotly 5.9.0
-* requests 2.28.1
-* pandas_market_calendars 4.1.4
-* ecos 2.0.12
-* cvxopt 1.3.0.1
-* ta 0.10.2
-* yfinance 0.2.14
+The following third-party packages were used with azapy 1.2.1:
+  * python 3.11.2
+  * pandas 1.5.3
+  * numpy 1.24.3
+  * scipy 1.10.1
+  * statsmodels 0.13.5
+  * matplotlib 3.7.1
+  * plotly 5.9.0
+  * requests 2.29.0
+  * pandas_market_calendars 4.1.4
+  * ecos 2.0.12
+  * cvxopt 1.3.0.1
+  * ta 0.10.2
+  * yfinance 0.2.14
```

### Comparing `azapy-1.1.1/azapy/MkT/MkTcalendar.py` & `azapy-1.2.0/azapy/MkT/MkTcalendar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-"""
-Contains:
-
-    - NYSEgen : NYSE business calendar
-"""
-
 import numpy as np
 import pandas_market_calendars as mcal
 
+
 def NYSEgen(sdate='1980-01-01', edate='2050-12-31'):
     """
-    Generate `numpy.busdaycalendar` for NYSE between `sdate` and 
+    Returns the NYSE business calendar between `sdate` and 
     `edate`.
 
     Parameters
     ----------
-    `sdate` : date like, optional;
+    sdate : date like, optional
         Calendar start date. The default is `'1980-01-01'`.
-    `edate` : date lik, optional
+    edate : date like, optional
         Calendar end date. The default is `'2050-12-31'`.
+        
     Returns
     -------
-    `numpy.busdaycalendar`;
-        NYSE business calendar.
+    `numpy.busdaycalendar` : NYSE business calendar.
     """
     sdate_ = np.datetime64(sdate)
     edate_ = np.datetime64(edate)
     # get the NYSE holiday list from standard pandas_market_calendars
     ldates = list(mcal.get_calendar('NYSE').holidays().holidays)
     # append here additional holidays 
     # already added to the new version of pandas_market_calendars
```

### Comparing `azapy-1.1.1/azapy/MkT/MkTreader.py` & `azapy-1.2.0/azapy/MkT/MkTreader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,63 +1,35 @@
-"""
-Contains:
-    
-    - class MkTreader : collects historical time series
-    - function readMkT : a wrapper to MkTreader class
-"""
-
 import pandas as pd
 import warnings
 import os
 import yfinance as yf
 import requests
 import numpy as np
 import pathlib
 import time
 from copy import deepcopy
 
 from azapy.MkT.MkTcalendar import NYSEgen
 
-def readMkT(symbol=[], sdate="2012-01-01", edate='today', calendar=None,
-            output_format='frame', source=None, force=False, save=True,
-            file_dir="outDir", file_format='csv', api_key=None, param=None,  
-            verbose=True):
-    """
-    Retrive market data for a set of stock symbols.
-    
-    It is a wrapper for `MkTreader` class returning directly the requested
-    historical time series. The function call variables are the same as for 
-    'MkTreader' member function 'get' (see its doc).
-    """
-    return MkTreader().get(symbol, sdate, edate, calendar, 
-                           output_format, source, force, save, 
-                           file_dir, file_format, api_key, param, 
-                           verbose)
-
 
 class MkTreader:
     """ 
-    Collect historical market prices from market data providers such as
+    Collects historical market prices from market data providers such as
     'yahoo', 'eodhistoricaldata', 'alphavantage' and 'marketstack'.
     
-    Public function members:
-        - `get` : returns the historical time series requested
-        - `get_request_status` : returns info about the request status
-        - `get_error_log` : returns the list of missing dates in the \
-            time series
-    Public data members:
+    **Attributs**
         - `dsource` : dict of request instructions per symbol
         - `delta_time` : execution time of the request in seconds
-        - `rout` : pandas.DataFrame contenig historical prices for all \
-            symbols. It is created during the call of `get` function.
-        - `rout_status` : request status information. It is created during \
-            the call of `get_request_status` function or during the \
-            call of function `get` with option `verbose=True`.
-        - `error_log` : contains lists of missing historical observation \
-            dates. It is created together with `rout_status`.
+        - `rout` : pandas.DataFrame contenig historical prices for all
+          symbols. It is created during the call of `get` function.
+        - `rout_status` : request status information. It is created during 
+          the call of `get_request_status` function or during the 
+          call of function `get` with option `verbose=True`.
+        - `error_log` : contains lists of missing historical observation 
+          dates. It is created together with `rout_status`.
     """
     def __init__(self):
         '''
         Constructor
         '''
         self.dsource = None
         self.delta_time = None
@@ -76,145 +48,134 @@
         self._alphavantage_max_req_per_min = 5
  
         
     def get(self, symbol=[], sdate="2012-01-01", edate='today', calendar=None,
             output_format='frame', source=None, force=False, save=True,
             file_dir="outDir", file_format='csv', api_key=None, param=None,  
             verbose=True):
-        '''
-        Get MkT data for a set of stock symbols.
-    
-        Collect historical stock prices from various market data providers 
-        such as yahoo, alphavantage, eodhistoricaldata and marketstack as
-        well as form saved data in local files.
-    
+        """
+        Retrieves market data for a set of stock symbols.\n
+        It is a wrapper for `MkTreader` class returning directly the requested
+        historical time series. The function call variables are the same as for 
+        'MkTreader' member function 'get'.
+        
         Parameters
         ----------
-        `symbol` : `str` or `list` of `str`, optional;
+        symbol : `str` or `list` of `str`, optional
             Stock symbols to be uploaded.
             The default is `[]`.
-        `sdate` : date like, optional;
+        sdate : date like, optional
             The start date of historical time series.
             The default is `"2012-01-01"`.
-        `edate` : date like, optional;
-            The end date of historical time series (must: sdate >= edate)
+        edate : date like, optional
+            The end date of historical time series (must: `sdate` >= `edate`)
             The default is `'today'`.
-        `calendar` : `numpy.busdaycalendar`, optional;
+        calendar : `numpy.busdaycalendar`, optional
             Exchange business day calendar. If set to `None` it will default to 
             the NY stock exchange business calendar (provided by the azapy 
             function NYSEgen).
             The default is `None`.
-        `output_format` : `str`, optional;
+        output_format : `str`, optional
             The function output format. It can be:
-            
-            - `'frame'` - `pandas.DataFrame`
-            - `'dict'` - `dict` of `pandaws.DataFrame` where the keys are the \
-                symbols. 
-            
+                - `'frame'` - `pandas.DataFrame`
+                - `'dict'` - `dict` of `pandaws.DataFrame`. 
+                  The symbols are the keys.
+                  
             The default is `'frame'`
-        `source` : `str` or `dict`, optional;
+        source : `str` or `dict`, optional
             If it is a `str`, then it represents the market data provider for 
-            all historical prices requests. Possible values are: `'yahoo'`, 
+            all historical prices request. Possible values are: `'yahoo'`, 
             `'alphavantage'`, `'alphavantage_yahoo'`, `'eodhistoricaldata'`,
             `'eodhistoricaldata_yahoo'` and `'marketstack'`. If set to `None` 
-            it will default to `'yahoo'`.
-            
-            It can be set to a dictionary containing specific instructions for 
+            it will default to `'yahoo'`.\n
+            It can be set to a `dict` containing specific instructions for 
             each stock symbol. 
-            The dict keys are stock symbols. The values are dict's of 
-            instructions. Valid keys for the instructions dict are the names of
+            The `dict` keys are the symbols and the values are 'dict'
+            instructions specific to each symbol. 
+            Valid keys for the instructions `dict` are the names of
             this function call variables except `'sdate'`, `'edate'`, 
             `'calendar'` and `'output_format'`. 
             The actual set of stock symbols is given by the union 
             of variable `'symbol'` and the keys of the dict `'source'`. Missing  
             values in the symbol instruction dict's will be filled with the 
             values of the function call variables. 
             The values of the function call variables act as 
             generic values to be used in absence of specific instructions 
-            in the `'source'` dict. 
-            The default is `None`.
-            
-            Example of dict `'source'`: 
-                
-            source = \
-                {'AAPL': {'source': 'eodhistoricaldata, 'verbose': `True`}, \
-                'SPY': {'source': 'yahoo', 'force': `True`}}
-                 
+            in the `'source'` dict. The default is `None`.\n
+            *Example* of dict `'source'`: \n
+            source = {'AAPL': {'source': 'eodhistoricaldata, 'verbose': `True`},
+            'SPY': {'source': 'yahoo', 'force': `True`}}\n
             In this case there are 2 symbols that will be added (union) to 
             the set of symbols defined by 'symbol' variable. For symbol 'AAPL' 
             the provider source is eodhistoricaldata and the 'verbose' 
             instruction 
             is set to `True`. The rest of the instructions: 'force', 'save',
             'file_dir', 'file_format', 'api_key' and 'param' are set 
             to the values of the corresponding function call variables.
             Similar for symbol 'SPY'. The instructions for the rest of the 
             symbols that may be specified in the 'symbol' variable will be
             set according to the values of the function call variables.
-        `force` : Boolean, optional;
-            - `True`: will try to collect historical prices exclusive from  \
-            the market data providers.
-            - `False`: first it will try to load the historical \
-            prices form a local saved file. If such a file does not exist \
-            the market data provider will be accessed.  \
-            If the file exists but the saved historical \
-            data is too short then it will try to collect the missing values \
+        force : Boolean, optional
+                - `True`: will try to collect historical prices exclusive from
+                  the market data providers.
+                - `False`: first it will try to load the historical 
+                  prices from a local saved file. If such a file does not exist
+                  the market data provider will be accessed.  
+                  
+            If the file exists but the saved historical 
+            data is too short then it will try to collect the missing values 
             only from the market data provider.
-            
             The default is `False`.
-        `save` : Boolean, optional;
-            - `True`: It will try to save the historical price collected from \
-               the providers to a local file.
-            - `False`: No attempt to save the data is made.
-            
-           The default is `True`.
-        `file_dir` : `str`, optional;
+        save : Boolean, optional
+                - `True`: It will try to save the historical price collected from 
+                  the providers to a local file.
+                - `False`: No attempt to save the data is made.
+                
+            The default is `True`.
+        file_dir : `str`, optional
             Directory with (to save) historical market data. If it does not 
             exists then it will be created.
             The default is "outDir".
-        `file_format` : `str`, optional;
+        file_format : `str`, optional
             The saved file format for the historical prices. The following 
             files formats are supported: csv, json and feather
             The default is 'csv'.
-        `api_key` : `str`, optional;
+        api_key : `str`, optional
             Provider API key (where is required). If set to `None`  
-            then the API key is set from the global environment variables. 
-            The names of the corresponding global environment variables are:
-                
-            - `APLPHAVANTAGE_API_KEY` : for alphavantage,
-            - `EODHISTORICALDATA_API_KEY` : for eodhistoricaldata,
-            - `MARKETSTACK_API_KEY` : for marketstack.
+            then the API key is set to the value of global environment variables\n 
+                - `APLPHAVANTAGE_API_KEY` for alphavantage,
+                - `EODHISTORICALDATA_API_KEY` for eodhistoricaldata,
+                - `MARKETSTACK_API_KEY` for marketstack.
             
             The default is `None`.
-        `param` : `dict`, optional;
+        param : `dict`, optional
             Set of additional information to access the market data provider.  
             At this point in time only accessing alphavantage provider requires 
             an additional parameter specifying the maximum number of API 
             (symbols) requested per minute. 
             It varies with the level of access 
             corresponding to the API key. The minimum value is 5 for a free key 
             and starts at 75 for premium keys. This value is stored in
-            max_req_per_min variable.
-            
-            Example: param = {'max_req_per_min': 5}
-            
-            This is also the default vale for alphavantage, if param is set to 
+            `max_req_per_min` variable.\n
+            *Example*: param = {'max_req_per_min': 5}\n
+            This is also the default vale for alphavantage, if `param` is set to 
             `None`.
-            
             The default is `None`.   
-        `verbose` : Boolean, optional;
+        verbose : Boolean, optional
             If set to `True`, then additional information will be printed  
             during the loading of historical prices.
             The default is `True`.
-    
+
+
         Returns
         -------
-        The historical market data as `pandas.DataFrame` or as a dict of
-        `pandas.DataFrame` (one for each symbol), depending on the value
-        set for `output_format`.
-        '''
+        `pandas.DataFrame` or 'dict' `pandas.DataFrame` : Historical market data. 
+            The output format is designated by the value of the input parameter 
+            `output_format`.
+        """
         # Process the inputs
         if isinstance(symbol, str):
             symbol = [symbol]
         elif not isinstance(symbol, list):
             warnings.warn(f"Wrong symbol type: {type(symbol)} "
                           + "must be str or a list of str")
             return pd.DataFrame()
@@ -321,25 +282,24 @@
     
     def get_request_status(self):
         '''
         Reports abbreviated information about request status.
 
         Returns
         -------
-        `pandas.DataFrame`;
-            The column names are the symbols for which the data was requested.
-            The rows contain the actual input parameters per symbol as well
-            as:
-                
+        `pandas.DataFrame` : The status report.
+        The column names are the symbols for which the data was requested.
+        The rows contain the actual input parameters per symbol as well
+        as:   
             - `'nrow'` : the length of historical time series.
             - `'sdate'` : first date in the time series.
             - `'edate'` : end date of the time series.
-            - `'error'` : if there are missing data. If the error is `'Yes'` \
-                then the actual list of missing date per symbol can  \
-                be obtained by calling `get_error_log`.
+            - `'error'` : if there are missing data. If its value is `'Yes'`
+              then the actual list of missing date per symbol can
+              be obtained by calling `get_error_log`.
         '''
         if self.rout is None or self.rout.empty:
             warnings.warn("Warning: request was returned empty")
             self.rout_status = pd.DataFrame(self.dsource)
             return self.rout_status
         
         self.rout_status = deepcopy(self.dsource)
@@ -363,26 +323,26 @@
     def get_error_log(self):
         '''
         Returns lists of missing historical observation dates per
         symbol
 
         Returns
         -------
-        `dict`;
-            If it is an empty dict then there are no missing dates in the
-            collected historical time series.
-            Otherwise, the keys of the dict are the symbols that have missing 
-            dates. The values for these keys are also dict with the following 
-            fields:
-                
+        `dict` : The error-log.
+        
+        If it is an empty `dict` then there are no missing dates in the
+        collected historical time series.
+        Otherwise, the keys of the `dict` are the symbols that have missing 
+        dates. The values for these keys are also `dict` with the following 
+        fields: 
             - `'back'`: a list of missing date at the tail of the time series
             - `'front'` : a list of missing data at the head of the time series
             - `'mid'` : a list of missing data in the middle of the time series
-            
-            Fields with empty list of dates are omitted.
+        
+        Fields with empty list of dates are omitted.
         '''
         return self.error_log
       
     
     def _ts_analyzer(self):
         self.error_log = {}
         lbday = pd.bdate_range(self.sdate, self.edate, freq='C', 
@@ -490,15 +450,15 @@
                 return kod_web, pd.DataFrame()
             
             if flag_save:
                 if verbose: 
                     print(f"save {symbol} data to file")
                 rout_web['adjusetd'] = self._adjustDividend(rout_web)
                 self._writer_disk(rout_web, symbol, file_dir, file_format)
-            
+
             rout = rout_web.loc[sdate_adj:edate_adj].copy()
             if rout.empty:
                 warnings.warn("no data in the range "
                               + f"{self.sdate.date()} : {self.edate.date()} "
                               + f"for {symbol} from source {source}")
                 return kod_web, pd.DataFrame()
             
@@ -564,15 +524,15 @@
             return pd.DataFrame()
         
         price['symbol'] = symbol
         price['source'] = source
         price['recordDate'] = pd.to_datetime('today').strftime("%Y-%m-%d %X")
         price.index = pd.to_datetime(price.index.date, utc=False)
         price.index.name = 'date'
-   
+
         if drange is None:
             return price[self._out_col]
         else:
             return price.loc[drange[0]:drange[1], self._out_col]
     
 
     def _reader_disk(self, symbol, file_dir, file_format):
@@ -622,15 +582,15 @@
         yrprice.rename(columns={'Open': 'open', 'High': 'high',
                                 'Low': 'low', 'Close': 'close',
                                 'Adj Close': 'adjusted', 'Volume': 'volume',
                                 'Dividends': 'divd', 'Stock Splits': 'split'},
                        inplace=True)
         yrprice.index.name = 'date'
         yrprice.loc[yrprice['split'] == 0., 'split'] = 1.
- 
+    
         return yrprice[self._col]
     
     
     def _eodhistoricaldata(self, symbol, api_key=None):
         '''
         returns maximum period adjusted for splits only,
         test key OeAFFmMliFG5orCUuwAKQ8l4WWFQ67YX for MCA only,
@@ -738,16 +698,16 @@
                                 'Adjusted_close': 'adjusted', 
                                 'Volume': 'volume'},
                        inplace=True)
         eeprice.set_index('date', inplace=True)
         eeprice.index = pd.to_datetime(eeprice.index)
      
         ysymb = yf.Ticker(symbol)
+        
         edprice = pd.DataFrame({'divd': ysymb.dividends})
-
         if edprice.empty:
             eeprice['divd'] = 0.
         else:
             edprice.index = pd.to_datetime(edprice.index.date, utc=False)
             edprice.index.name = 'date'
             eeprice = pd.merge(eeprice, edprice, how='left', 
                                left_index=True, right_index=True)
```

### Comparing `azapy-1.1.1/azapy/MkT/summary_MkTData.py` & `azapy-1.2.0/azapy/MkT/summary_MkTdata.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import pandas as pd
 import numpy as np
 from collections import defaultdict 
 
-#from .readMkTData import NYSEgen
 from .MkTcalendar import NYSEgen
 
-def summary_MkTData(mktdata, calendar=None, sdate=None, edate=None):
+def summary_MkTdata(mktdata, calendar=None, sdate=None, edate=None):
     """
     Summary of MkT data time-series length and quality (checks for missing
     records).
 
     Parameters
     ----------
-    `mktdata` :`pandas.DataFrame` or a dict of `pndas.DataFrame';
+    mktdata : `pandas.DataFrame` or a dict of `pndas.DataFrame`
         Market Data in the format returned by `azapy.readMkT` function.
-    `calendar` : `numpy.busdaycalendar`, optional;
+    calendar : `numpy.busdaycalendar`, optional
         Business days calendar. If is set to None it will 
         default to NYSE business calendar.
-    `sdate` : `pandas.Timestamp`, optional;
+    sdate : `pandas.Timestamp`, optional
         Time-series start date. If it is `None` then `sdate` will be set to the 
         earliest date in mktdata.
         The default is `None`.
-    `edate` : `pandas.Timestamp`, optional;
-        Time-series end date. If it is `None` then edate will be set to 
+    edate : `pandas.Timestamp`, optional
+        Time-series end date. If it is `None` then `edate` will be set to 
         the most recent date in mktdata.
         The default is `None`.
 
     Returns
     -------
-    `pandas.DataFrame`; A table with columns:
+    `pandas.DataFrame` : A table with columns:
         - `symbol` : time-series symbol
         - `begin` : start date
         - `end` : end date
         - `length` : number of records
         - `na_total` : total number of `nan`
         - `na_b` : number of missing records at the beginning
         - `na_e` : number of missing records at the end
         - `cont` : total number of missing records
-            
-    Comment: the main application is to assess the missing data in the 
+        
+    Comments
+    --------
+    The main application is to assess the missing data in the 
     time-series extracted with `azapy.readMkT` function.
     """
     if isinstance(mktdata, dict):
         gite = mktdata.items()
     else:
         gite = mktdata.groupby('symbol')
```

### Comparing `azapy-1.1.1/azapy/PortOpt/BTADAnalyzer.py` & `azapy-1.2.0/azapy/Analyzers/BTADAnalyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,105 +4,144 @@
 import time
 
 from ._RiskAnalyzer import _RiskAnalyzer
 from ._solvers import _lp_solver
 
 class BTADAnalyzer(_RiskAnalyzer):
     """
-    Mixture BTAD based optimal portfolio strategies.
+    Mixture BTAD (Below Threshold Absolute Deviation) 
+    based optimal portfolio strategies.
     
-    Methods:
-        * getWeights
-        * getRisk
-        * getPositions
-        * getRiskComp
-        * getDiversification
-        * viewForntiers
-        * set_rrate
-        * set_mktdata
-        * set_rtype
-        * set_random_seed
+    **Attributes**
+        * `status` : `int` - the computation status (`0` - success, 
+          any other value signifies an error)
+        * `ww` : `pandas.Series` -  the portfolio weights 
+        * `RR` : `float` - portfolio rate of return
+        * `risk` : `float` - portfolio mBTAD risk
+        * `primary_risk_comp` : `list` - portfolio mBTAD components
+        * `secondary_risk_comp` : `list` - portfolio thresholds, `alpha` 
+          (input values)
+        * `sharpe` : `float` - Omega ration if `rtype` is set to `'Shapre'` 
+          or `'Sharpe2'` otherwise `None`. 
+        * `diverse` : `float` - diversification factor if `rtype` is set 
+          to `'Divers'` or `'MaxDivers'` otherwise `None`.
+        * `name` : `str` - portfolio name
+        
+    Note the following 2 important methods:
+        * `getWeights` : Computes the optimal portfolio weights.
+          During its computations the following class members are also set:
+          `risk`, `primery_risk_comp`, `secondary_risk_comp`, `sharpe`,  `RR`, 
+          `divers`.
+        * `getPositions` : Provides practical information regarding the portfolio
+          rebalancing delta positions and costs.  
     """
-    def __init__(self, alpha=[0.], coef=None, mktdata=None, 
-                 colname='adjusted', freq='Q', hlength=3.25, calendar=None, 
-                 rtype='Sharpe', detrended=False, method='ecos', name='BTAD'):
+    def __init__(self, alpha=[0.], coef=None, mktdata=None, colname='adjusted', 
+                 freq='Q', hlength=3.25, name='BTAD', rtype='Sharpe', mu=None, 
+                 d=1, mu0=0., aversion=None, ww0=None, detrended=False, 
+                 method='ecos'):
         """
         Constructor
 
         Parameters
         ----------
-        `alpha` : `list`, optional;
+        alpha : `list`, optional
             List of BTSD thresholds. The default is `[0.]`.
-        `coef` : `list`, optional;
+        coef : `list`, optional
             List of positive mixture 
-            coefficients. Must have the same size as `alpha`. 
+            coefficients. Must be the same size as `alpha`. 
             A `None` value assumes an equal weighted risk mixture.
             The vector of coefficients will be normalized to unit.
             The default is `None`.
-        `mktdata` : `pandas.DataFrame`, optional;
+        mktdata : `pandas.DataFrame`, optional
             Historic daily market data for portfolio components in the format
             returned by `azapy.mktData` function. The default is `None`.
-        `colname` : `str`, optional;
-            Name of the price column from mktdata used in the weights 
+        colname : `str`, optional
+            Name of the price column from mktdata used in the weight's 
             calibration. The default is `'adjusted'`.
-        `freq` : `str`, optional;
+        freq : `str`, optional
             Rate of return horizon. It could be 
-            `'Q'` for quarter or `'M'` for month. The default is `'Q'`.
-        `hlength` : `float`, optional;
+            `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
             History length in number of years used for calibration. A 
             fractional number will be rounded to an integer number of months.
             The default is `3.25` years.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will 
-            be set to NYSE business calendar. 
-            The default is `None`.
-        `rtype` : `str`, optional;
+        name : `str`, optional
+            Portfolio name. The default is `'BTAD'`.
+        rtype : `str`, optional
             Optimization type. Possible values: \n
-                `'Risk'` : optimal-risk portfolio for targeted expected rate of 
+                `'Risk'` : optimal risk portfolio for targeted expected rate of 
                 return.\n
-                `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
-                `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
+                `'Sharpe'` : optimal Sharpe portfolio - maximization solution.\n
+                `'Sharpe2'` : optimal Sharpe portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
-                `'RiskAverse'` : optimal-risk portfolio for a fixed 
+                `'RiskAverse'` : optimal risk portfolio for a fixed 
                 risk-aversion factor.\n
-                `'InvNrisk'` : optimal-risk portfolio with the same risk value 
+                `'InvNrisk'` : optimal risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
-                `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
-                `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                `'Diverse'` : optimal diversified portfolio for targeted
+                expected rate of return (max of inverse 1-Diverse).\n
+                `'Diverse2'` : optimal diversified portfolio for targeted
+                expected rate of return (min of 1-Diverse).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
-                `'InvNdiverse'` : optimal-diversified portfolio with the same
+                `'InvNdiverse'` : optimal diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
-                `'InvNdrr'` : optima- diversified portfolio with the same 
+                `'InvNdrr'` : optimal diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `method` : `str`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
+            Targeted portfolio expected rate of return. 
+            Relevant only if `rtype='Risk'` or `rtype='Divers'`.
+            The default is `None`.
+        d : `int`, optional
+            Frontier type. Active only if `rtype='Risk'`. A value of `1` will
+            trigger the evaluation of optimal portfolio along the efficient
+            frontier. Otherwise, it will find the portfolio with the lowest
+            rate of return along the inefficient portfolio frontier.
+            The default is `1`.
+        mu0 : `float`, optional
+            Risk-free rate accessible to the investor.
+            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            The default is `0`.
+        aversion : `float`, optional
+            The value of the risk-aversion coefficient.
+            Must be positive. Relevant only if `rtype='RiskAverse'`.
+            The default is `None`.
+        ww0 : `list`, `numpy.array` or `pandas.Series`, optional
+            Targeted portfolio weights. 
+            Relevant only if `rype='InvNrisk'`.
+            Its length must be equal to the number of symbols in `rrate` 
+            (mktdata). All weights must be >= 0 with thier sum > 0.
+            If it is a `list` or a `numpy.array` then the weights are assumed 
+            to be in order of `rrate.columns`. If it is a `pandas.Series` then 
+            the index should be compatible with the `rrate.columns` or mktdata 
+            symbols (same symbols, not necessarily in the same order).
+            If it is `None` then it will be set to equal weights.
+            The default is `None`.
+        detrendent : Boolean, optional
+            If it set to `True` then the rates of return are detrended 
+            (mean=0). The default value is `True`. 
+        method : `str`, optional
             Linear programming numerical method. 
             Could be: `'ecos'`, `'highs-ds'`, `'highs-ipm'`, `'highs'`, 
             `'interior-point'`, `'glpk'` and `'cvxopt'`.
             The default is `'ecos'`.
-        `name` : `str`, optional;
-            Object name. The default is `'BTAD'`.
-
+        
         Returns
         -------
         The object.
         """
         self.detrended = detrended
-        
-        super().__init__(mktdata, colname, freq, hlength, calendar, 
-                         rtype, name)
-        
+        super().__init__(mktdata, colname, freq, hlength, name,
+                         rtype, mu, d, mu0, aversion, ww0)
         self._set_method(method)
-
         self.alpha = np.array(alpha)
+        
         if len(np.unique(self.alpha)) != len(self.alpha):
             raise ValueError("alpha values are not unique")
         
         self.ll = len(alpha)
 
         if coef is None:
             self.coef = np.full(self.ll, 1/self.ll)
@@ -115,28 +154,32 @@
                 raise ValueError("All coef must be positive")
                 
             self.coef = self.coef / self.coef.sum()
         
         
     def set_rrate(self, rrate):
         """
-        Sets portfolio components historical rates of returns.
+        Sets portfolio components historical rates of return.
         It will overwrite the value computed by the constructor from mktdata.
 
         Parameters
         ----------
-        `rrate` : `pandas.DataFrame`
-            Portfolio components historical rates of returns. The
-            columns are: `"date"`, `"symbol1"`, `"symbol2"`, etc.
+        rrate : `pandas.DataFrame`
+            Portfolio components historical rates of return. The
+            columns are: `'date'`, `'symbol1'`, `'symbol2'`, etc.
         Returns
         -------
-        None
+        `None`
         """
+        if rrate is None:
+            # nothing to do
+            return
+        
         self.nn, self.mm = rrate.shape
-        self.muk = rrate.mean()
+        self.muk = rrate.mean(numeric_only=True)
         
         if self.detrended:
             self.rrate = rrate - self.muk
         else:
             self.rrate = rrate.copy()
```

### Comparing `azapy-1.1.1/azapy/PortOpt/BTSDAnalyzer.py` & `azapy-1.2.0/azapy/Analyzers/BTSDAnalyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,105 +4,151 @@
 import time
 
 from .BTADAnalyzer import BTADAnalyzer
 from ._solvers import _socp_solver
 
 class BTSDAnalyzer(BTADAnalyzer):
     """
-    Mixture BTSD based optimal portfolio strategies.
+    Mixture BTSD (Below Threshold Standard Deviation) 
+    based optimal portfolio strategies.
     
-    Methods:
-        * getWeights
-        * getRisk
-        * getPositions
-        * getRiskComp
-        * getDiversification
-        * viewForntiers
-        * set_rrate
-        * set_mktdata
-        * set_rtype
-        * set_random_seed
+    **Attributes**
+       * `status` : `int` - the computation status (`0` - success, 
+         any other value signifies an error)
+       * `ww` : `pandas.Series` -  the portfolio weights 
+       * `RR` : `float` - portfolio rate of return
+       * `risk` : `float` - portfolio mBTSD risk
+       * `primary_risk_comp` : `list` - portfolio mBTSD components
+       * `secondary_risk_comp` : `list` - portfolio thresholds, `alpha` 
+         (input values)
+       * `sharpe` : `float` - Omega ration if `rtype` is set to `'Shapre'` 
+         or `'Sharpe2'` otherwise `None`. 
+       * `diverse` : `float` - diversification factor if `rtype` is set 
+         to `'Divers'` or `'MaxDivers'` otherwise `None`.
+       * `name` : `str` - portfolio name
+       
+    Note the following 2 important methods:
+       * `getWeights` : Computes the optimal portfolio weights.
+         During its computations the following class members are also set:
+         `risk`, `primery_risk_comp`, `secondary_risk_comp`, `sharpe`,  `RR`, 
+         `divers`.
+       * `getPositions` : Provides practical information regarding the portfolio
+         rebalancing delta positions and costs.  
     """
-    def __init__(self, alpha=[0.], coef=None, mktdata=None, 
-                 colname='adjusted', freq='Q', hlength=3.25, calendar=None, 
-                 rtype='Sharpe', detrended=False, method='ecos', name='BTSD'):
+    def __init__(self, alpha=[0.], coef=None, mktdata=None, colname='adjusted',
+                 freq='Q', hlength=3.25, name='BTSD', rtype='Sharpe', mu=None, 
+                 d=1, mu0=0., aversion=None, ww0=None, detrended=False, 
+                 method='ecos'):
         """
-        `alpha` : `list`, optional;
+        Constructor
+
+        Parameters
+        ----------
+        alpha : `list`, optional
             List of BTSD thresholds. The default is `[0.]`.
-        `coef` : `list`, optional;
+        coef : `list`, optional
             List of positive mixture 
-            coefficients. Must have the same size as `alpha`. 
+            coefficients. Must be the same size as `alpha`. 
             A `None` value assumes an equal weighted risk mixture.
             The vector of coefficients will be normalized to unit.
             The default is `None`.
-        `mktdata` : `pandas.DataFrame`, optional;
+        mktdata : `pandas.DataFrame`, optional
             Historic daily market data for portfolio components in the format
             returned by `azapy.mktData` function. The default is `None`.
-        `colname` : `str`, optional;
-            Name of the price column from mktdata used in the weights 
+        colname : `str`, optional
+            Name of the price column from mktdata used in the weight's 
             calibration. The default is `'adjusted'`.
-        `freq` : `str`, optional
+        freq : `str`, optional
             Rate of return horizon. It could be 
-            `'Q'` for quarter or `'M'` for month. The default is `'Q'`.
-        `hlength` : `float`, optional;
+            `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
             History length in number of years used for calibration. A 
             fractional number will be rounded to an integer number of months.
             The default is `3.25` years.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will 
-            be set to NYSE business calendar. 
-            The default is `None`.
-        `rtype` : `str`, optional;
+        name : `str`, optional
+            Portfolio name. The default is `'BTSD'`.
+        rtype : `str`, optional
             Optimization type. Possible values: \n
-                `'Risk'` : optimal-risk portfolio for targeted expected rate of 
+                `'Risk'` : optimal risk portfolio for targeted expected rate of 
                 return.\n
-                `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
-                `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
+                `'Sharpe'` : optimal Sharpe portfolio - maximization solution.\n
+                `'Sharpe2'` : optimal Sharpe portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
-                `'RiskAverse'` : optimal-risk portfolio for a fixed 
+                `'RiskAverse'` : optimal risk portfolio for a fixed 
                 risk-aversion factor.\n
-                `'InvNrisk'` : optimal-risk portfolio with the same risk value 
+                `'InvNrisk'` : optimal risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
-                `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
-                `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                `'Diverse'` : optimal diversified portfolio for targeted
+                expected rate of return (max of inverse 1-Diverse).\n
+                `'Diverse2'` : optimal diversified portfolio for targeted
+                expected rate of return (min of 1-Diverse).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
-                `'InvNdiverse'` : optimal-diversified portfolio with the same
+                `'InvNdiverse'` : optimal diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
-                `'InvNdrr'` : optima- diversified portfolio with the same 
+                `'InvNdrr'` : optimal diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `method` : `str`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
+            Targeted portfolio expected rate of return. 
+            Relevant only if `rtype='Risk'` or `rtype='Divers'`.
+            The default is `None`.
+        d : `int`, optional
+            Frontier type. Active only if `rtype='Risk'`. A value of `1` will
+            trigger the evaluation of optimal portfolio along the efficient
+            frontier. Otherwise, it will find the portfolio with the lowest
+            rate of return along the inefficient portfolio frontier.
+            The default is `1`.
+        mu0 : `float`, optional
+            Risk-free rate accessible to the investor.
+            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            The default is `0`.
+        aversion : `float`, optional
+            The value of the risk-aversion coefficient.
+            Must be positive. Relevant only if `rtype='RiskAverse'`.
+            The default is `None`.
+        ww0 : `list`, `numpy.array` or `pandas.Series`, optional
+            Targeted portfolio weights. 
+            Relevant only if `rype='InvNrisk'`.
+            Its length must be equal to the number of symbols in `rrate` 
+            (mktdata). All weights must be >= 0 with thier sum > 0.
+            If it is a `list` or a `numpy.array` then the weights are assumed 
+            to be in order of `rrate.columns`. If it is a `pandas.Series` then 
+            the index should be compatible with the `rrate.columns` or mktdata 
+            symbols (same symbols, not necessarily in the same order).
+            If it is `None` then it will be set to equal weights.
+            The default is `None`.
+        detrendent : Boolean, optional
+            If it set to `True` then the rates of return are detrended 
+            (mean=0). The default value is `True`. 
+        method : `str`, optional
             SOCP numerical method. 
             Could be: `'ecos'`, or `'cvxopt'`.
             The defualt is `'ecos'`.
-        `name` : `str`, optional;
-            Object name. The default is `'BTSD'`.
-
+        
         Returns
         -------
         The object.
         """
         super().__init__(alpha, coef, mktdata, colname, freq, hlength,  
-                         calendar, rtype, detrended, method, name)
+                         name, rtype, mu, d, mu0, aversion, ww0,
+                         detrended, method)
         
         
     def _set_method(self, method):
         self._set_socp_method(method)
     
     
     def _risk_calc(self, prate, alpha):
         rr = alpha - prate
         rr[rr < 0] = 0.
         rho = np.mean(rr ** 2) ** 0.5
-        # status, alpha, rho
+        
         return 0, alpha, rho
     
     
     def _risk_min(self, d=1):
         # w <- [0 : mm]
         # then for l <- [0:ll]
         #   u_l <- mm + l(nn+1),
```

### Comparing `azapy-1.1.1/azapy/PortOpt/CVaRAnalyzer.py` & `azapy-1.2.0/azapy/Analyzers/LSDAnalyzer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,857 +1,892 @@
 import numpy as np
 import scipy.sparse as sps
 import warnings
 import time
 
-from ._RiskAnalyzer import _RiskAnalyzer
-from ._solvers import _lp_solver
+from .MADAnalyzer import MADAnalyzer
+from ._solvers import _socp_solver
 
-class CVaRAnalyzer(_RiskAnalyzer):
+class LSDAnalyzer(MADAnalyzer):
     """
-    Mixture CVaR based optimal portfolio strategies.
-        
-    Methods:
-        * getWeights
-        * getRisk
-        * getPositions
-        * getRiskComp
-        * getDiversification
-        * viewForntiers
-        * set_rrate
-        * set_mktdata
-        * set_rtype
-        * set_random_seed
+    m-level LSD (lower Standard Deviation) 
+    based optimal portfolio strategies.
+    
+    **Attributes**
+        * `status` : `int` - the computation status (`0` - success, 
+          any other value signifies an error)
+        * `ww` : `pandas.Series` -  the portfolio weights 
+        * `RR` : `float` - portfolio rate of return
+        * `risk` : `float` - portfolio mLSD risk
+        * `primary_risk_comp` : `list` - delta-risk components of 
+          portfolio mLSD
+        * `secondary_risk_comp` : `list` - cumulative delta-risk components 
+          of mLSD 
+        * `sharpe` : `float` - mLSD-Sharpe ration if `rtype` is set to 
+          `'Shapre'` or `'Sharpe2'` otherwise `None`. 
+        * `diverse` : `float` - diversification factor if `rtype` is set 
+          to `'Divers'` or `'MaxDivers'` otherwise `None`.
+        * `name` : `str` - portfolio name
+        
+    Note the following 2 important methods:
+        * `getWeights` : Computes the optimal portfolio weights.
+          During its computations the following class members are also set:
+          `risk`, `primery_risk_comp`, `secondary_risk_comp`, `sharpe`,  `RR`, 
+          `divers`.
+        * `getPositions` : Provides practical information regarding the portfolio
+          rebalancing delta positions and costs.  
     """
-    def __init__(self, alpha=[0.975], coef=None, 
-                 mktdata=None, colname='adjusted', freq='Q', 
-                 hlength=3.25, calendar=None,
-                 rtype='Sharpe', method='ecos', name='CVaR'):
+    def __init__(self, coef=[1.], mktdata=None, colname='adjusted', freq='Q', 
+                 hlength=3.25, name='LSD', rtype='Sharpe', mu=None, d=1, 
+                 mu0=0., aversion=None, ww0=None, method='ecos'):
         """
         Constructor
 
         Parameters
         ----------
-        `alpha` : `list`, optional;
-            List of distinct confidence levels. The default is `[0.975]`.
-        `coef` : `list`, optional;
-            List of positive mixture coefficients. Must have the same size with 
-            `alpha`. A `None` value assumes an equal weighted risk mixture.
-            The vector of coefficients will be normalized to unit.
-            The default is `None`.
-        `mktdata` : `pandas.DataFrame`, optional;
+        coef : `list`, optional
+            Positive non-increasing list of mixture coefficients. 
+            The default is `[1.]`.
+        mktdata : `pandas.DataFrame`, optional
             Historic daily market data for portfolio components in the format
             returned by `azapy.mktData` function. The default is `None`.
-        `colname` : `str`, optional;
-            Name of the price column from mktdata used in the weights 
+        colname : `str`, optional
+            Name of the price column from mktdata used in the weight's 
             calibration. The default is `'adjusted'`.
-        `freq` : `str`, optional
+        freq : `str`, optional
             Rate of return horizon. It could be 
-            `'Q'` for quarter or `'M'` for month. The default is `'Q'`.
-        `hlength` : `float`, optional;
+            `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
             History length in number of years used for calibration. A 
             fractional number will be rounded to an integer number of months.
             The default is `3.25` years.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will 
-            be set to NYSE business calendar. 
-            The default is `None`.
-        `rtype` : `str`, optional;
+        name : `str`, optional
+            Portfolio name. The default is `'LSD'`.
+        rtype : `str`, optional
             Optimization type. Possible values: \n
-                `'Risk'` : optimal-risk portfolio for targeted expected rate of 
+                `'Risk'` : optimal risk portfolio for targeted expected rate of 
                 return.\n
-                `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
-                `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
+                `'Sharpe'` : optimal Sharpe portfolio - maximization solution.\n
+                `'Sharpe2'` : optimal Sharpe portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
-                `'RiskAverse'` : optimal-risk portfolio for a fixed 
+                `'RiskAverse'` : optimal risk portfolio for a fixed 
                 risk-aversion factor.\n
-                `'InvNrisk'` : optimal-risk portfolio with the same risk value 
+                `'InvNrisk'` : optimal risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
-                `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
-                `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                `'Diverse'` : optimal diversified portfolio for targeted
+                expected rate of return (max of inverse 1-Diverse).\n
+                `'Diverse2'` : optimal diversified portfolio for targeted
+                expected rate of return (min of 1-Diverse).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
-                `'InvNdiverse'` : optimal-diversified portfolio with the same
+                `'InvNdiverse'` : optimal diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
-                `'InvNdrr'` : optima- diversified portfolio with the same 
+                `'InvNdrr'` : optimal diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `method` : `str`, optional;
-            Linear programming numerical method. 
-            Could be: `'ecos'`, `'highs-ds'`, `'highs-ipm'`, `'highs'`, 
-            `'interior-point'`, `'glpk'` and `'cvxopt'`.
-            The default is `'ecos'`.
-        `name` : `str`, optional;
-            Object name, Default value is `'CVaR'`.
-            
+            The default is `'Sharpe'`.
+        mu : `float`, optional
+            Targeted portfolio expected rate of return. 
+            Relevant only if `rtype='Risk'` or `rtype='Divers'`.
+            The default is `None`.
+        d : `int`, optional
+            Frontier type. Active only if `rtype='Risk'`. A value of `1` will
+            trigger the evaluation of optimal portfolio along the efficient
+            frontier. Otherwise, it will find the portfolio with the lowest
+            rate of return along the inefficient portfolio frontier.
+            The default is `1`.
+        mu0 : `float`, optional
+            Risk-free rate accessible to the investor.
+            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            The default is `0`.
+        aversion : `float`, optional
+            The value of the risk-aversion coefficient.
+            Must be positive. Relevant only if `rtype='RiskAverse'`.
+            The default is `None`.
+        ww0 : `list`, `numpy.array` or `pandas.Series`, optional
+            Targeted portfolio weights. 
+            Relevant only if `rype='InvNrisk'`.
+            Its length must be equal to the number of symbols in `rrate` 
+            (mktdata). All weights must be >= 0 with sum > 0.
+            If it is a `list` or a `numpy.array` then the weights are assumed 
+            to be in order of `rrate.columns`. If it is a `pandas.Series` then 
+            the index should be compatible with the `rrate.columns` or mktdata 
+            symbols (same symbols, not necessarily in the same order).
+            If it is `None` then it will be set to equal weights.
+            The default is `None`.
+        method : `str`, optional
+            SOCP numerical method. Could be: `'ecos'` or `'cvxopt'`.
+            The defualt is `'ecos'`.
+
         Returns
         -------
         The object.
         """
-        super().__init__(mktdata, colname, freq, hlength, calendar, 
-                         rtype, name)
-        
-        self._set_method(method)
-
-        self.alpha = np.array(alpha)
-        if any((self.alpha <= 0.) | (1. <= self.alpha)):
-            raise ValueError("All alpha coefficients must be in (0,1)")
-        if len(np.unique(self.alpha)) != len(self.alpha):
-            raise ValueError("alpha values are not unique")
-            
-        self.ll = len(alpha)
-            
-        if coef is None:
-            self.coef = np.full(self.ll, 1/self.ll)
-        else:
-            self.coef = np.array(coef)
-        
-            if len(self.coef) != len(self.alpha):
-                raise ValueError("alpha and coef must have the same length")
-            if any(self.coef <= 0.):
-                raise ValueError("All coef must be positive")
+        super().__init__(coef, mktdata, colname, freq, hlength, name, 
+                         rtype, mu, d, mu0, aversion, ww0, method)
         
-            self.coef = self.coef / self.coef.sum()
         
-
-
     def _set_method(self, method):
-        self._set_lp_method(method)
+        self._set_socp_method(method)
         
         
-    def _risk_calc_lp(self, prate, alpha):
-        # lp formulation of CVaR & VaR
-        # Order of variables:
-        # u <- 0, 
-        # s <- [1:nn] 
-        # in total dim=nn + 1
-        nn = self.nn
-        
-        # build c
-        c_data = [1.] + [1. / (1. - alpha) / nn] * nn
-        
-        # build G
-        G_icol = [0] * nn + list(range(1, nn + 1)) + list(range(nn+1))
-        G_irow = list(range(nn)) * 2 + list(range(nn, 2 * nn + 1))
-        G_data = [-1.] * (3 * nn + 1)
+    def _risk_calc_(self, prate):
+        # mu = np.mean(prate)
+        # prate = prate - mu
+        # nn = len(prate)
+        delta = []
+        mu = 0.
+        for _ in range(self.ll):
+            xrate = mu - prate
+            xrate[xrate <= 0.] = 0.
+            dd = np.sqrt(np.mean(xrate**2))
+            delta.append(dd)
+            mu -= dd
+            
+        self.primary_risk_comp = np.array(delta)
+        self.secondary_risk_comp = \
+            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
+        self.risk = np.dot(self.primary_risk_comp, self.coef)
+        self.status = 0
         
-        G_shape = (2 * nn + 1, nn + 1)
-        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
+        return self.risk
+
 
-        # build h
-        h_data = list(prate) + [0.] * (nn + 1)
-    
-        # calc
-        toc = time.perf_counter()
-        res = _lp_solver(self.method, c_data, G, h_data)
-        self.time_level2 = time.perf_counter() - toc
-        
-        if res['status'] != 0:
-            return 2, np.nan, np.nan
-        
-        VaR = res['x'][0]
-        CVaR = res['pcost']
-  
-        return 0, VaR, CVaR
-    
-    
-    def _risk_calc(self, prate, alpha):
-        # Analytic formulation of CVaR & VaR
-        ws = np.sort(prate)
-        nnl = len(ws) * (1. - alpha)
-        VaR = -ws[int(nnl)]
-        CVaR = VaR - (ws[ws <= -VaR] + VaR).sum() / nnl
-        
-        return 0, VaR, CVaR
-    
-    
     def _risk_min(self, d=1):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
         #   u_l <- mm + l(nn+1), 
         #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # in total dim = mm + ll(nn + 1)
-        ll = self.ll
         nn = self.nn
         mm = self.mm
+        ll = self.ll 
     
         # build c
-        c_data = [0] * mm
+        c_data = [0.] * mm 
         for l in range(ll):
-            c_data += [self.coef[l]] \
-                    + [self.coef[l] / (1 - self.alpha[l] ) / nn] * nn
-       
+            c_data += [self.coef[l]] + [0.] * nn
+        
         # build G
+        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + l * (nn + 1)] * nn \
-                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += list(range(l * nn, (l + 1) * nn)) \
-                + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1] * nn + [-1] * nn
+            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
+                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
+                       for _ in range(l)] \
+                  + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1.] * ((l + 1) * nn)
             
-        G_icol += list(range(mm))
-        G_irow += [nn * ll] * mm
+        G_icol += list(range(mm)) 
+        G_irow += [ll * nn] * mm
         G_data += list(-self.muk * d)
         
         G_icol += list(range(mm + ll * (nn + 1)))
-        G_irow += list(range(ll * nn + 1, ll * nn + 1 + mm + ll * (nn + 1)))
-        G_data += [-1.] * (mm + ll * (nn + 1) )
-        
-        G_shape = (nn * ll + 1 + mm + ll * (nn + 1), mm + (nn + 1) * ll)
+        G_irow += list(range(nn * ll + 1, mm + 2 * nn * ll + ll + 1))
+        G_data += [-1.] * (mm + ll * (nn + 1))
+        # cone
+        for l in range(ll):
+            G_icol += list(range((nn + 1) * l + mm , 
+                                 (nn + 1) * l + mm + 1 + nn))
+            G_irow += list(range(mm + 2 * nn * ll + ll + 1 + l * (nn + 1), 
+                                 mm + 2 * nn * ll + ll + 1 + (l + 1) * (nn + 1)))
+            G_data += [-np.sqrt(nn)] + [-1.] * nn
+            
+        G_shape = (3 * nn * ll + 1 + mm + 2 * ll, mm + ll * (nn + 1))
         G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
- 
-        # build h
-        h_data = [0.] * (nn * ll) + [-self.mu * d] + [0.] *(mm + ll * (nn + 1))
+        
+        #build h
+        h_data = [0.] * (nn * ll) + [-self.mu * d] \
+               + [0.] * (mm + 2 * ll * (nn + 1))
+        
+        # build dims
+        dims = {'l': (2 * ll * nn + ll + 1 + mm), 'q': [nn + 1] * ll}
         
         # build A
         A_icol = list(range(mm))
         A_irow = [0] * mm
         A_data = [1.] * mm
         
         A_shape = (1, mm + ll * (nn + 1))
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
-
+        
         # build b
         b_data = [1.]
         
         # calc
         toc = time.perf_counter()
-        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
+        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
         self.time_level2 = time.perf_counter() - toc
  
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-            
-        # VaR (u)
-        self.secondary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
-                                    for l in range(ll)])
-        # mCVaR
+        
+        # mLSD
         self.risk = res['pcost']
-        # CVaR (recomputed)
-        self.primary_risk_comp = \
-            np.array([res['x'][mm + l * (nn + 1)] \
-             + 1 / (1 - self.alpha[l]) * np.mean(
-                 res['x'][(mm + l * (nn + 1) + 1) : (mm + (l + 1) * (nn + 1))])
-             for l in range(ll)])
+        # delta-risk values
+        self.primary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
+                                           for l in range(ll)])
+        # delta-risk strikes
+        self.secondary_risk_comp = \
+            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
         # optimal weights
         self.ww = np.array(res['x'][:mm])
         self.ww.shape = mm
-        # rate of returns
+        # rate of return
         self.RR = np.dot(self.ww, self.muk)
         
         return self.ww
-    
+        
     
     def _sharpe_max(self):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
-        #   u_l <- mm + l(nn+1), 
-        #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
+        # u_l <- mm + l(nn+1), 
+        # s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # and last t <- [mm + ll(nn + 1)]
         # in total dim = mm + ll(nn + 1) + 1
         ll = self.ll
         nn = self.nn
         mm = self.mm
         
         # build c
         c_data = list(-self.muk) + [0.] * (ll * (nn + 1)) + [self.mu]
         
         # build G
+        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + l * (nn + 1)] * nn \
-                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += list(range(l * nn, (l + 1) * nn)) \
-                + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1] * nn + [-1] * nn
-            
+            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
+                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
+                       for _ in range(l)] \
+                  + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1.] * ((l + 1) * nn)
+
         G_icol += list(range(mm + ll * (nn + 1) + 1))
-        G_irow += list(range(ll * nn, ll * nn + mm + ll * (nn + 1) + 1))
+        G_irow += list(range(nn * ll, mm + 2 * nn * ll + ll + 1))
         G_data += [-1.] * (mm + ll * (nn + 1) + 1)
-        
-        G_shape = (ll * nn + mm + ll * (nn + 1) + 1, mm + ll * (nn + 1) + 1)
+        # cone
+        for l in range(ll):
+            G_icol += list(range((nn + 1) * l + mm , 
+                                 (nn + 1) * l + mm + 1 + nn))
+            G_irow += list(range(mm + 2 * nn * ll + ll + 1 + l * (nn + 1), 
+                                 mm + 2 * nn * ll + ll + 1 + (l + 1) * (nn + 1)))
+            G_data += [-np.sqrt(nn)] + [-1.] * nn
+            
+        G_shape = (3 * nn * ll + mm + 2 * ll + 1, mm + ll * (nn + 1) + 1)
         G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
-      
+        
         # build h
-        h_data = [0.] * (nn * ll + mm + ll * (nn + 1) + 1)
+        h_data = [0.] * (3 * nn * ll + mm + 2 * ll + 1)
+        
+        # build dims
+        dims = {'l': (2 * ll * nn + mm + ll + 1), 'q': [nn + 1] * ll}
         
         # build A
         A_icol = list(range(mm)) + [mm + ll * (nn + 1)]
         A_irow = [0] * (mm + 1)
         A_data = [1.] * mm + [-1.]
-        for l in range(ll):
-            A_icol += [mm + l * (nn + 1)] \
-                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            A_irow += [1] * (nn + 1)
-            A_data += [self.coef[l]] \
-                + [self.coef[l] / (1 - self.alpha[l]) / nn ] * nn
- 
+        
+        A_icol += [mm + l * (nn + 1) for l in range(ll)]
+        A_irow += [1] * ll
+        A_data += list(self.coef)
+        
         A_shape = (2, mm + ll * (nn + 1) + 1)
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
-  
+ 
         # build b
         b_data = [0., 1.]
         
         # calc
         toc = time.perf_counter()
-        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
+        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
         self.time_level2 = time.perf_counter() - toc
-       
+ 
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-
-        # mCVaR (1/t)
+        
+        # mLSD
         self.risk = 1. / res['x'][-1]
-        # VaR (u)
-        self.secondary_risk_comp = \
-            np.array([res['x'][mm + l * (nn + 1)] * self.risk \
-                      for l in range(ll)])
-        # Sharpe
+        # delta-risk values
+        self.primary_risk_comp = np.array(
+            [res['x'][mm + l * (nn + 1)] * self.risk for l in range(ll)])
+        # mLSD-Sharpe
         self.sharpe = -res['pcost']
         # optimal weights
         self.ww = np.array(res['x'][:mm] * self.risk)
         self.ww.shape = mm
         # rate of return
-        self.RR = np.dot(self.ww, self.muk)
-        # component CVaR (recomputed)
-        self.primary_risk_comp = \
-            np.array([(res['x'][mm + l * (nn + 1)] + 1 / (1 - self.alpha[l]) \
-            * np.mean(res['x'][(mm + l * (nn + 1) + 1) :\
-                               (mm + (l + 1) * (nn + 1))])) \
-            * self.risk for l in range(ll)])
+        self.RR = self.sharpe * self.risk + self.mu
+        # delta-risk strikes
+        self.secondary_risk_comp = \
+            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
         
         return self.ww
     
     
     def _sharpe_inv_min(self):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
-        #   u_l <- mm + l(nn+1), 
-        #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
+        # u_l <- mm + l(nn+1), 
+        # s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # and last t <- [mm + ll(nn + 1)]
         # in total dim = mm + ll(nn + 1) + 1
         ll = self.ll
         nn = self.nn
         mm = self.mm
         
-        # build c   
+        # build c
         c_data = [0.] * mm 
         for l in range(ll):
-            c_data += [self.coef[l]] \
-                    + [self.coef[l] / (1. - self.alpha[l]) / nn] * nn
+            c_data += [self.coef[l]] + [0.] * nn
         c_data += [0.]
         
         # build G
+        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + l * (nn + 1)] * nn \
-                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += list(range(l * nn, (l + 1) * nn)) \
-                + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1.] * nn + [-1.] * nn
-            
+            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
+                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
+                       for _ in range(l)]\
+                  + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1.] * ((l + 1) * nn)
+
         G_icol += list(range(mm + ll * (nn + 1) + 1))
-        G_irow += list(range(ll * nn, ll * nn + mm + ll * (nn + 1) + 1))
+        G_irow += list(range(nn * ll, mm + 2 * nn * ll + ll + 1))
         G_data += [-1.] * (mm + ll * (nn + 1) + 1)
-        
-        G_shape = (ll * nn + mm + ll * (nn + 1) + 1, mm + ll * (nn + 1) + 1)
+        # cone
+        for l in range(ll):
+            G_icol += list(range((nn + 1) * l + mm , 
+                                 (nn + 1) * l + mm + 1 + nn))
+            G_irow += list(range(mm + 2 * nn * ll + ll + 1 + l * (nn + 1), 
+                           mm + 2 * nn * ll + ll + 1 + (l + 1) * (nn + 1)))
+            G_data += [-np.sqrt(nn)] + [-1.] * nn
+            
+        G_shape = (3 * nn * ll + mm + 2 * ll + 1, mm + ll * (nn + 1) + 1)
         G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
-     
+        
         # build h
-        h_data = [0.] * (nn * ll + mm + ll * (nn + 1) + 1)
+        h_data = [0.] * (3 * nn * ll + mm + 2 * ll + 1)
         
-        #build A
-        A_icol = list(range(mm)) + [mm + ll * (nn + 1)]
-        A_irow = [0] * (mm + 1)
-        A_data = [1.] * mm + [-1.]
+        # build dims
+        dims = {'l': (2 * ll * nn + mm + ll + 1), 'q': [nn + 1] * ll}
         
-        A_icol += list(range(mm)) + [mm + ll * (nn + 1)]
-        A_irow += [1] * (mm + 1)
-        A_data += list(self.muk) + [-self.mu]
+        # build A
+        A_icol = (list(range(mm)) + [mm + ll * (nn + 1)]) * 2
+        A_irow = [0] * (mm + 1) + [1] * (mm + 1)
+        A_data = [1.] * mm + [-1.] + list(self.muk) + [-self.mu]
         
         A_shape = (2, mm + ll * (nn + 1) + 1)
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
-     
-        # build b
+ 
+        # bjuild b
         b_data = [0., 1.]
-
+        
         # calc
         toc = time.perf_counter()
-        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
+        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
         self.time_level2 = time.perf_counter() - toc
-       
+ 
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-
+        
+        # mLSD-Sharpe
+        self.sharpe = 1. / res['pcost']
+        # mLSD
         t = res['x'][-1]
-        # mCVaR (g/t)
         self.risk = res['pcost'] / t
-        # VaR (u)
-        self.secondary_risk_comp = \
-            np.array([res['x'][mm + l * (nn + 1)] / t for l in range(ll)])
-        # Sharpe
-        self.sharpe = 1. / res['pcost']
+        # delta-risk values
+        self.primary_risk_comp = np.array(
+            [res['x'][mm + l * (nn + 1)] / t for l in range(ll)])
+        
         # optimal weights
         self.ww = np.array(res['x'][:mm] / t)
         self.ww.shape = mm
         # rate of return
         self.RR = 1. / t + self.mu
-        # component CVaR (recomputed)
-        self.primary_risk_comp = \
-            np.array([(res['x'][mm + l * (nn + 1)] + 1 / (1 - self.alpha[l]) \
-            * np.mean(res['x'][(mm + l * (nn + 1) + 1) :\
-                            (mm + (l + 1) * (nn + 1))])) /t \
-            for l in range(ll)])
+        # delta-risk strikes
+        self.secondary_risk_comp = \
+            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
         
         return self.ww
-    
+        
     
     def _rr_max(self):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
         #   u_l <- mm + l(nn+1), 
         #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # in total dim = mm + ll(nn + 1)
-        ll = self.ll
         nn = self.nn
         mm = self.mm
-    
+        ll = self.ll 
+        
         # build c
-        c_data = list(-self.muk) + [0.] * ((nn + 1) * ll)
-            
+        c_data = list(-self.muk) + [0.] * (ll * (nn + 1))
+        
         # build G
+        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + l * (nn + 1)] * nn \
-                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += list(range(l * nn, (l + 1) * nn)) \
-                + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1.] * nn + [-1.] * nn
-            
+            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
+                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
+                       for _ in range(l)] \
+                  + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1.] * ((l + 1) * nn)
+
         G_icol += list(range(mm + ll * (nn + 1)))
-        G_irow += list(range(ll * nn, ll * nn + mm + ll * (nn + 1)))
+        G_irow += list(range(nn * ll, mm + 2 * nn * ll + ll))
         G_data += [-1.] * (mm + ll * (nn + 1))
-        
-        G_shape = (nn * ll + mm + (nn + 1) * ll, mm + (nn + 1) * ll )
+        # cone
+        for l in range(ll):
+            G_icol += list(range((nn + 1) * l + mm , 
+                                 (nn + 1) * l + mm + 1 + nn))
+            G_irow += list(range(mm + 2 * nn * ll + ll + l * (nn + 1), 
+                                 mm + 2 * nn * ll + ll + (l + 1) * (nn + 1)))
+            G_data += [-np.sqrt(nn)] + [-1.] * nn
+            
+        G_shape = (3 * nn * ll + mm + 2 * ll, mm + ll * (nn + 1))
         G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
-
+        
         # build h
-        h_data = [0.] * (nn * ll + mm + (nn + 1) * ll)
+        h_data = [0.] * (3 * nn * ll + mm + 2 * ll)
+        
+        # build dims
+        dims = {'l': (2 * ll * nn + mm + ll), 'q': [nn + 1] * ll}
         
         # build A
-        A_icol = list(range(mm + (nn + 1) * ll))
-        A_irow = [0] * mm + [1] * ((nn + 1) * ll)
-        A_data = [1.] * mm
-        for l in range(ll):
-            A_data += [self.coef[l]] \
-                  + [self.coef[l] / (1 - self.alpha[l]) / nn] * nn
-
-        A_shape = (2, mm + (nn + 1) * ll)
+        A_icol = list(range(mm)) + [mm + l * (nn + 1) for l in range(ll)]
+        A_irow = [0] * mm + [1] * ll
+        A_data = [1.] * mm + list(self.coef)
+        
+        A_shape = (2, mm + ll * (nn + 1))
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
-   
+        
         # build b
         b_data = [1., self.risk]
         
         # calc
         toc = time.perf_counter()
-        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
+        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
         self.time_level2 = time.perf_counter() - toc
-       
+ 
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-
-        # VaR (u)
-        self.secondary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
-                                    for l in range(ll)])
-        # CVaR (recomputed)
-        self.primary_risk_comp = \
-            np.array([res['x'][mm + l * (nn + 1)] \
-             + 1 / (1 - self.alpha[l]) * np.mean(
-                 res['x'][(mm + l * (nn + 1) + 1) : (mm + (l + 1) * (nn + 1))])
-             for l in range(ll)])
+        
+        # rate of return
+        self.RR = -res['pcost']
+        # delta-risk values
+        self.primary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
+                                           for l in range(ll)])
+        # delta-risk strikes
+        self.secondary_risk_comp = \
+            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
         # optimal weights
         self.ww = np.array(res['x'][:mm])
         self.ww.shape = mm
-        # rate of return
-        self.RR = -res['pcost']
-        # mCVaR recalculate
-        self.risk = np.dot(self.coef, self.primary_risk_comp)
+
+        return self.ww
         
-        return self.ww 
- 
     
     def _risk_averse(self):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
         #   u_l <- mm + l(nn+1), 
         #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # in total dim = mm + ll(nn + 1)
-        ll = self.ll
         nn = self.nn
         mm = self.mm
-    
+        ll = self.ll 
+        
         # build c
         c_data = list(-self.muk)
         for l in range(ll):
-            c_data += [self.Lambda * self.coef[l]] \
-               + [self.Lambda * self.coef[l] / (1 - self.alpha[l] ) / nn] * nn
-            
+            c_data += [self.Lambda * self.coef[l]] + [0.] * nn
+        
         # build G
+        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + l * (nn + 1)] * nn \
-                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += list(range(l * nn, (l + 1) * nn)) \
-                + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1] * nn + [-1] * nn
-            
+            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
+                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
+                       for _ in range(l)]\
+                  + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1.] * ((l + 1) * nn)
+
         G_icol += list(range(mm + ll * (nn + 1)))
-        G_irow += list(range(ll * nn, ll * nn + mm + ll * (nn + 1)))
+        G_irow += list(range(nn * ll, mm + 2 * nn * ll + ll))
         G_data += [-1.] * (mm + ll * (nn + 1))
-        
-        G_shape = (nn * ll + mm + (nn + 1) * ll, mm + (nn + 1) * ll)
+        # cone
+        for l in range(ll):
+            G_icol += list(range((nn + 1) * l + mm , 
+                                 (nn + 1) * l + mm + 1 + nn))
+            G_irow += list(range(mm + 2 * nn * ll + ll + l * (nn + 1), 
+                                 mm + 2 * nn * ll + ll + (l + 1) * (nn + 1)))
+            G_data += [-np.sqrt(nn)] + [-1.] * nn
+            
+        G_shape = (3 * nn * ll + mm + 2 * ll, mm + ll * (nn + 1))
         G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
-
+        
         # build h
-        h_data = [0.] * (nn * ll + mm + (nn + 1) * ll)
+        h_data = [0.] * (3 * nn * ll + mm + 2 * ll)
         
-        # build A
+        # build dims
+        dims = {'l': (2 * ll * nn + mm + ll), 'q': [nn + 1] * ll}
+        
+        # build A 
         A_icol = list(range(mm))
         A_irow = [0] * mm
         A_data = [1.] * mm
         
         A_shape = (1, mm + ll * (nn + 1))
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
-
+        
         # build b
         b_data = [1.]
         
         # calc
         toc = time.perf_counter()
-        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
+        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
         self.time_level2 = time.perf_counter() - toc
-       
+ 
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-
+        
         # optimal weights
         self.ww = np.array(res['x'][:mm])
         self.ww.shape = mm
-        # VaR (u)
-        self.secondary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
-                                    for l in range(ll)])
-        # rate of returns
+        # rate of return
         self.RR = np.dot(self.ww, self.muk)
-        # mCVaR
-        self.risk = (res['pcost'] + self.RR) / self.Lambda
-        # CVaR (recomputed)
-        self.primary_risk_comp = \
-            np.array([res['x'][mm + l * (nn + 1)] \
-             + 1 / (1 - self.alpha[l]) * np.mean(
-                 res['x'][(mm + l * (nn + 1) + 1) : (mm + (l + 1) * (nn + 1))])
-             for l in range(ll)])
+        # mLSD
+        self.risk = (self.RR + res['pcost']) / self.Lambda
+        # delta-risk values
+        self.primary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
+                                           for l in range(ll)])
+        # delta-risk strikes
+        self.secondary_risk_comp = \
+            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
         
         return self.ww
-        
+    
     
     def _risk_diversification(self, d=1):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
-        #   u_l <- mm + l(nn+1), 
-        #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
+        # u_l <- mm + l(nn+1), 
+        # s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # and last t <- [mm + ll(nn + 1)]
         # in total dim = mm + ll(nn + 1) + 1
         ll = self.ll
         nn = self.nn
         mm = self.mm
         
-        # build c   
+        # build c
         c_data = [0.] * mm 
         for l in range(ll):
-            c_data += [self.coef[l]] \
-                    + [self.coef[l] / (1. - self.alpha[l]) / nn] * nn
+            c_data += [self.coef[l]] + [0.] * nn
         c_data += [0.]
         
         # build G
+        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + l * (nn + 1)] * nn \
-                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += list(range(l * nn, (l + 1) * nn)) \
-                + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1.] * nn + [-1.] * nn
-            
+            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
+                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
+                       for _ in range(l)]\
+                  + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1.] * ((l + 1) * nn)
             
         G_icol += list(range(mm)) + [mm + ll * (nn + 1)]
-        G_irow += [ll * nn] * (mm + 1)
+        G_irow += [nn * ll] * (mm + 1)
         G_data += list(-self.muk * d) + [self.mu * d]
-            
+
         G_icol += list(range(mm + ll * (nn + 1) + 1))
-        G_irow += list(range(ll * nn + 1, ll * nn + mm + ll * (nn + 1) + 2))
+        G_irow += list(range(nn * ll + 1, mm + 2 * nn * ll + ll + 2))
         G_data += [-1.] * (mm + ll * (nn + 1) + 1)
-        
-        G_shape = (ll * nn + mm + ll * (nn + 1) + 2, mm + ll * (nn + 1) + 1)
+        # cone
+        for l in range(ll):
+            G_icol += list(range((nn + 1) * l + mm , 
+                                 (nn + 1) * l + mm + 1 + nn))
+            G_irow += list(range(mm + 2 * nn * ll + ll + 2 + l * (nn + 1), 
+                           mm + 2 * nn * ll + ll + 2 + (l + 1) * (nn + 1)))
+            G_data += [-np.sqrt(nn)] + [-1.] * nn
+            
+        G_shape = (3 * nn * ll + mm + 2 * ll + 2, mm + ll * (nn + 1) + 1)
         G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
-     
+        
         # build h
-        h_data = [0.] * (nn * ll + mm + ll * (nn + 1) + 2)
+        h_data = [0.] * (3 * nn * ll + mm + 2 * ll + 2)
         
-        #build A
+        # build dims
+        dims = {'l': (2 * ll * nn + mm + ll + 2), 'q': [nn + 1] * ll}
+        
+        # build A
         A_icol = list(range(mm)) + [mm + ll * (nn + 1)]
-        A_irow = [0] * (mm + 1)
-        A_data = [1.] * mm + [-1.]
+        A_irow = [0] * (mm + 1) 
+        A_data = [1.] * mm + [-1.] 
         
-        A_icol += list(range(mm)) 
+        A_icol += list(range(mm))
         A_irow += [1] * mm
-        A_data += list(self.risk_comp) 
-        
+        A_data += list(self.risk_comp)
+ 
         A_shape = (2, mm + ll * (nn + 1) + 1)
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
-     
-        # build b
+ 
+        # bjuild b
         b_data = [0., 1.]
-
+        
         # calc
         toc = time.perf_counter()
-        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
+        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
         self.time_level2 = time.perf_counter() - toc
-       
+ 
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-
+        
+        # mLSD-Divers
+        self.diverse= 1. - res['pcost']
+        # mLSD
         t = res['x'][-1]
-        # mCVaR (g/t)
         self.risk = res['pcost'] / t
-        # VaR (u)
-        self.secondary_risk_comp = \
-            np.array([res['x'][mm + l * (nn + 1)] / t for l in range(ll)])
-        # Diversification
-        self.diverse = 1. - res['pcost']
+        # delta-risk values
+        self.primary_risk_comp = np.array(
+            [res['x'][mm + l * (nn + 1)] / t for l in range(ll)])
+        
         # optimal weights
         self.ww = np.array(res['x'][:mm] / t)
         self.ww.shape = mm
         # rate of return
         self.RR = np.dot(self.ww, self.muk)
-        # component CVaR (recomputed)
-        self.primary_risk_comp = \
-            np.array([(res['x'][mm + l * (nn + 1)] + 1 / (1 - self.alpha[l]) \
-            * np.mean(res['x'][(mm + l * (nn + 1) + 1) :\
-                            (mm + (l + 1) * (nn + 1))])) /t \
-            for l in range(ll)])
+        # delta-risk strikes
+        self.secondary_risk_comp = \
+            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
         
         return self.ww
     
     
     def _risk_inv_diversification(self, d=1):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
-        #   u_l <- mm + l(nn+1), 
-        #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
+        # u_l <- mm + l(nn+1), 
+        # s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # and last t <- [mm + ll(nn + 1)]
         # in total dim = mm + ll(nn + 1) + 1
         ll = self.ll
         nn = self.nn
         mm = self.mm
         
-        # build c   
+        # build c
         c_data = list(-self.risk_comp) + [0.] * (ll * (nn + 1) + 1)
         
         # build G
+        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + l * (nn + 1)] * nn \
-                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += list(range(l * nn, (l + 1) * nn)) \
-                + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1.] * nn + [-1.] * nn
-            
+            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
+                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
+                       for _ in range(l)]\
+                  + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1.] * ((l + 1) * nn)
             
         G_icol += list(range(mm)) + [mm + ll * (nn + 1)]
-        G_irow += [ll * nn] * (mm + 1)
+        G_irow += [nn * ll] * (mm + 1)
         G_data += list(-self.muk * d) + [self.mu * d]
-            
+
         G_icol += list(range(mm + ll * (nn + 1) + 1))
-        G_irow += list(range(ll * nn + 1, ll * nn + mm + ll * (nn + 1) + 2))
+        G_irow += list(range(nn * ll + 1, mm + 2 * nn * ll + ll + 2))
         G_data += [-1.] * (mm + ll * (nn + 1) + 1)
-        
-        G_shape = (ll * nn + mm + ll * (nn + 1) + 2, mm + ll * (nn + 1) + 1)
+        # cone
+        for l in range(ll):
+            G_icol += list(range((nn + 1) * l + mm , 
+                                 (nn + 1) * l + mm + 1 + nn))
+            G_irow += list(range(mm + 2 * nn * ll + ll + 2 + l * (nn + 1), 
+                           mm + 2 * nn * ll + ll + 2 + (l + 1) * (nn + 1)))
+            G_data += [-np.sqrt(nn)] + [-1.] * nn
+            
+        G_shape = (3 * nn * ll + mm + 2 * ll + 2, mm + ll * (nn + 1) + 1)
         G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
-     
+        
         # build h
-        h_data = [0.] * (nn * ll + mm + ll * (nn + 1) + 2)
+        h_data = [0.] * (3 * nn * ll + mm + 2 * ll + 2)
         
-        #build A
-        A_icol = list(range(mm)) + [mm + ll * (nn + 1)]
-        A_irow = [0] * (mm + 1)
-        A_data = [1.] * mm + [-1.]
+        # build dims
+        dims = {'l': (2 * ll * nn + mm + ll + 2), 'q': [nn + 1] * ll}
         
-        A_icol += list(range(mm, mm + ll * (nn + 1))) 
-        A_irow += [1] * (ll * (nn + 1))
-        for l in range(ll):
-            A_data += [self.coef[l]] \
-                    + [self.coef[l] / (1 - self.alpha[l]) / nn] * nn
+        # build A
+        A_icol = list(range(mm)) + [mm + ll * (nn + 1)]
+        A_irow = [0] * (mm + 1) 
+        A_data = [1.] * mm + [-1.] 
         
+        A_icol += [mm + l * (nn + 1) for l in range(ll)]
+        A_irow += [1] * ll
+        A_data += list(self.coef)
+ 
         A_shape = (2, mm + ll * (nn + 1) + 1)
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
-     
-        # build b
+ 
+        # bjuild b
         b_data = [0., 1.]
         
         # calc
         toc = time.perf_counter()
-        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
+        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
         self.time_level2 = time.perf_counter() - toc
-       
+ 
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-
-        t = res['x'][-1]
-        # mCVaR (1/t)
+        
+        t = res['x'][-1] 
+        # mLSD-Divers
+        self.diverse= 1. + 1. / res['pcost']
+        # mLSD
         self.risk = 1. / t
-        # VaR (u)
-        self.secondary_risk_comp = \
-            np.array([res['x'][mm + l * (nn + 1)] / t for l in range(ll)])
-        # Diversification
-        self.diverse = 1. + 1. / res['pcost']
+        # delta-risk values
+        self.primary_risk_comp = np.array(
+            [res['x'][mm + l * (nn + 1)] / t for l in range(ll)])
         # optimal weights
-        self.ww = np.array(res['x'][:mm]) / t
+        self.ww = np.array(res['x'][:mm] / t)
         self.ww.shape = mm
         # rate of return
         self.RR = np.dot(self.ww, self.muk)
-        # component CVaR (recomputed)
-        self.primary_risk_comp = \
-            np.array([(res['x'][mm + l * (nn + 1)] + 1 / (1 - self.alpha[l]) \
-            * np.mean(res['x'][(mm + l * (nn + 1) + 1) :\
-                            (mm + (l + 1) * (nn + 1))])) /t \
-            for l in range(ll)])
+        # delta-risk strikes
+        self.secondary_risk_comp = \
+            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
         
         return self.ww
         
-        
+    
     def _rr_max_diversification(self):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
         #   u_l <- mm + l(nn+1), 
         #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # in total dim = mm + ll(nn + 1)
-        ll = self.ll
         nn = self.nn
         mm = self.mm
-    
+        ll = self.ll 
+        
         # build c
-        c_data = list(-self.muk) + [0.] * ((nn + 1) * ll)
-            
+        c_data = list(-self.muk) + [0.] * (ll * (nn + 1))
+        
         # build G
+        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + l * (nn + 1)] * nn \
-                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += list(range(l * nn, (l + 1) * nn)) \
-                + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1.] * nn + [-1.] * nn
-            
+            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
+                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
+                       for _ in range(l)] \
+                  + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1.] * ((l + 1) * nn)
+
         G_icol += list(range(mm + ll * (nn + 1)))
-        G_irow += list(range(ll * nn, ll * nn + mm + ll * (nn + 1)))
+        G_irow += list(range(nn * ll, mm + 2 * nn * ll + ll))
         G_data += [-1.] * (mm + ll * (nn + 1))
-        
-        G_shape = (nn * ll + mm + (nn + 1) * ll, mm + (nn + 1) * ll )
+        # cone
+        for l in range(ll):
+            G_icol += list(range((nn + 1) * l + mm , 
+                                 (nn + 1) * l + mm + 1 + nn))
+            G_irow += list(range(mm + 2 * nn * ll + ll + l * (nn + 1), 
+                                 mm + 2 * nn * ll + ll + (l + 1) * (nn + 1)))
+            G_data += [-np.sqrt(nn)] + [-1.] * nn
+            
+        G_shape = (3 * nn * ll + mm + 2 * ll, mm + ll * (nn + 1))
         G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
-
+        
         # build h
-        h_data = [0.] * (nn * ll + mm + (nn + 1) * ll)
+        h_data = [0.] * (3 * nn * ll + mm + 2 * ll)
+        
+        # build dims
+        dims = {'l': (2 * ll * nn + mm + ll), 'q': [nn + 1] * ll}
         
         # build A
-        A_icol = list(range(mm + (nn + 1) * ll)) + list(range(mm))
-        A_irow = [0] * mm + [1] * ((nn + 1) * ll + mm)
-        A_data = [1.] * mm
-        for l in range(ll):
-            A_data += [self.coef[l]] \
-                  + [self.coef[l] / (1 - self.alpha[l]) / nn] * nn
-        A_data += list((self.diverse - 1) * self.risk_comp)
+        A_icol = list(range(mm)) + [mm + l * (nn + 1) for l in range(ll)] + list(range(mm))
+        A_irow = [0] * mm + [1] * (ll + mm)
+        A_data = [1.] * mm + list(self.coef) + list((self.diverse- 1) * self.risk_comp)
         
-        A_shape = (2, mm + (nn + 1) * ll)
+        A_shape = (2, mm + ll * (nn + 1))
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
-   
+        
         # build b
         b_data = [1., 0.]
         
         # calc
         toc = time.perf_counter()
-        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
+        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
         self.time_level2 = time.perf_counter() - toc
-       
+ 
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-
-        # VaR (u)
-        self.secondary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
-                                    for l in range(ll)])
-        # CVaR (recomputed)
-        self.primary_risk_comp = \
-            np.array([res['x'][mm + l * (nn + 1)] \
-             + 1 / (1 - self.alpha[l]) * np.mean(
-                 res['x'][(mm + l * (nn + 1) + 1) : (mm + (l + 1) * (nn + 1))])
-             for l in range(ll)])
-        # mCVaR
+        
+        # rate of return
+        self.RR = -res['pcost']
+        # delta-risk values
+        self.primary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
+                                           for l in range(ll)])
+        # risk
         self.risk = np.dot(self.primary_risk_comp, self.coef)
+        # delta-risk strikes
+        self.secondary_risk_comp = \
+            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
         # optimal weights
         self.ww = np.array(res['x'][:mm])
         self.ww.shape = mm
-        # rate of return
-        self.RR = -res['pcost']
         # diversification
-        self.diverse = 1 - self.risk / np.dot(self.ww, self.risk_comp)
-        
-        return self.ww 
+        self.diverse= 1 - self.risk / np.dot(self.ww, self.risk_comp)
+
+        return self.ww
```

### Comparing `azapy-1.1.1/azapy/PortOpt/EVaRAnalyzer.py` & `azapy-1.2.0/azapy/Analyzers/EVaRAnalyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,105 +11,141 @@
 from ._solvers import _exp_cone_solver
 
 _PD_TOL_ = 1.e-6
 
 
 class EVaRAnalyzer(_RiskAnalyzer):
     """
-    Mixture EVaR based optimal portfolio strategies.
+    Mixture EVaR (Entropic Value at Risk) 
+    based optimal portfolio strategies.
         
-    Methods:
-        * getWeights
-        * getRisk
-        * getPositions
-        * getRiskComp
-        * getDiversification
-        * viewForntiers
-        * set_rrate
-        * set_mktdata
-        * set_rtype
-        * set_random_seed
+    **Attributes**
+        * `status` : `int` - the computation status (`0` - success, 
+          any other value signifies an error)
+        * `ww` : `pandas.Series` -  the portfolio weights 
+        * `RR` : `float` - portfolio rate of return
+        * `risk` : `float` - portfolio mEVaR risk
+        * `primary_risk_comp` : `list` - EVaR components of portfolio mEVaR
+        * `secondary_risk_comp` : `list` - effective confidence values 
+          associated with EVaR components.
+        * `sharpe` : `float` - mEVaR-Sharpe ration if `rtype` is set to  
+          `'Shapre'` or `'Sharpe2'` otherwise `None`. 
+        * `diverse` : `float` - diversification factor if `rtype` is set 
+          to `'Divers'` or `'MaxDivers'` otherwise `None`.
+        * `name` : `str` - portfolio name
+        
+    Note the following 2 important methods:
+        * `getWeights` : Computes the optimal portfolio weights.
+          During its computations the following class members are also set:
+          `risk`, `primery_risk_comp`, `secondary_risk_comp`, `sharpe`,  `RR`, 
+          `divers`.
+        * `getPositions` : Provides practical information regarding the portfolio
+          rebalancing delta positions and costs.  
     """
-    def __init__(self, alpha=[0.65], coef=None, 
-                 mktdata=None, colname='adjusted', freq='Q', 
-                 hlength=3.25, calendar=None,
-                 rtype='Sharpe', method='ncp', name='EVaR'):
+    def __init__(self, alpha=[0.65], coef=None, mktdata=None, 
+                 colname='adjusted', freq='Q', hlength=3.25, name='EVaR', 
+                 rtype='Sharpe', mu=None, d=1, mu0=0., aversion=None, 
+                 ww0=None, method='ncp'):
         """
         Constructor
 
         Parameters
         ----------
-        `alpha` : `list`, optional;
+        alpha : `list`, optional
             List of distinct confidence levels. The default is `[0.65]`.
-        `coef` : `list`, optional;
-            List of positive mixture coefficients. Must have the same size with 
+        coef : `list`, optional
+            List of positive mixture coefficients. Must be the same size as 
             `alpha`. A `None` value assumes an equal weighted risk mixture.
             The vector of coefficients will be normalized to unit.
             The default is `None`.
-        `mktdata` : `pandas.DataFrame`, optional;
+        mktdata : `pandas.DataFrame`, optional
             Historic daily market data for portfolio components in the format
             returned by `azapy.mktData` function. The default is `None`.
-        `colname` : `str`, optional;
-            Name of the price column from mktdata used in the weights 
+        colname : `str`, optional
+            Name of the price column from mktdata used in the weight's 
             calibration. The default is `'adjusted'`.
-        `freq` : `str`, optional;
+        freq : `str`, optional
             Rate of return horizon. It could be 
-            `'Q'` for quarter or `'M'` for month. The default is `'Q'`.
-        `hlength` : `float`, optional;
+            `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
             History length in number of years used for calibration. A 
             fractional number will be rounded to an integer number of months.
             The default is `3.25` years.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will 
-            be set to NYSE business calendar. 
-            The default is `None`.
-        `rtype` : `str`, optional;
+        name : `str`, optional
+            Portfolio name. The default is `'EVaR'`.
+        rtype : `str`, optional
             Optimization type. Possible values: \n
-                `'Risk'` : optimal-risk portfolio for targeted expected rate of 
+                `'Risk'` : optimal risk portfolio for targeted expected rate of 
                 return.\n
-                `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
-                `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
+                `'Sharpe'` : optimal Sharpe portfolio - maximization solution.\n
+                `'Sharpe2'` : optimal Sharpe portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
-                `'RiskAverse'` : optimal-risk portfolio for a fixed 
+                `'RiskAverse'` : optimal risk portfolio for a fixed 
                 risk-aversion factor.\n
-                `'InvNrisk'` : optimal-risk portfolio with the same risk value 
+                `'InvNrisk'` : optimal risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
-                `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
-                `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                `'Diverse'` : optimal diversified portfolio for targeted
+                expected rate of return (max of inverse 1-Diverse).\n
+                `'Diverse2'` : optimal diversified portfolio for targeted
+                expected rate of return (min of 1-Diverse).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
-                `'InvNdiverse'` : optimal-diversified portfolio with the same
+                `'InvNdiverse'` : optimal diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
-                `'InvNdrr'` : optima- diversified portfolio with the same 
+                `'InvNdrr'` : optimal diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `method` : `str`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
+            Targeted portfolio expected rate of return. 
+            Relevant only if `rtype='Risk'` or `rtype='Divers'`.
+            The default is `None`.
+        d : `int`, optional
+            Frontier type. Active only if `rtype='Risk'`. A value of `1` will
+            trigger the evaluation of optimal portfolio along the efficient
+            frontier. Otherwise, it will find the portfolio with the lowest
+            rate of return along the inefficient portfolio frontier.
+            The default is `1`.
+        mu0 : `float`, optional
+            Risk-free rate accessible to the investor.
+            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            The default is `0`.
+        aversion : `float`, optional
+            The value of the risk-aversion coefficient.
+            Must be positive. Relevant only if `rtype='RiskAverse'`.
+            The default is `None`.
+        ww0 : `list`, `numpy.array` or `pandas.Series`, optional
+            Targeted portfolio weights. 
+            Relevant only if `rype='InvNrisk'`.
+            Its length must be equal to the number of symbols in `rrate` 
+            (mktdata). All weights must be >= 0 with sum > 0.
+            If it is a `list` or a `numpy.array` then the weights are assumed 
+            to be in order of `rrate.columns`. If it is a `pandas.Series` then 
+            the index should be compatible with the `rrate.columns` or mktdata 
+            symbols (same symbols, not necessarily in the same order).
+            If it is `None` then it will be set to equal weights.
+            The default is `None`.
+        method : `str`, optional
             Numerical optimization method:
                 `'ncp'` : nonlinear convex programming (using cvxopt).\n
                 `'ncp2'` : nonlinear convex programming (using cvxopt) 
                 alternative to `'ncp'`.\n
                 `'excp'` : exponential cone programming (using ecos).\n
             The default is `'ncp'`.
-        `name` : `str`, optional;
-            Object name. The default is `'EVaR'`.
             
         Returns
         -------
         The object.
         """
-        super().__init__(mktdata, colname, freq, hlength, calendar, 
-                         rtype, name)
-        
+        super().__init__(mktdata, colname, freq, hlength, name,
+                         rtype, mu, d, mu0, aversion, ww0)
         self._set_method(method)
-
         self.alpha = np.array(alpha)
+        
         if any((self.alpha <= 0.) | (1. <= self.alpha)):
             raise ValueError("All alpha coefficients must be in (0,1)")
         if len(np.unique(self.alpha)) != len(self.alpha):
             raise ValueError("alpha values are not unique")
             
         self.ll = len(alpha)
             
@@ -124,14 +160,15 @@
                 raise ValueError("All coef must be positive")
         
             self.coef = self.coef / self.coef.sum()
         
 
     def _set_method(self, method):
         self.methods = ['ncp', 'ncp2', 'excp']
+        
         if not method in self.methods:
             raise ValueError(f"method must be one of {self.methods}")
         self.method = method
         
         
     def _risk_calc(self, prate, alpha):
         if self.method == 'excp':
@@ -213,16 +250,16 @@
             u = uu if np.abs(uu) >= MinU else MinU
             res = np.log(np.mean(np.exp(-u * data[1])) / (1 - data[0])) / u 
             return res
         
         toc = time.perf_counter()
         res = spo.minimize_scalar(fb, args=(alpha, prate))
         self.time_level2 = time.perf_counter() - toc
-        
         self.status = 0 if res['success'] else 2
+        
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['message']}")
             return 2, np.nan, np.nan
         
         EVaR = res['fun']
         astar = 1 - ECDF(prate)(-EVaR)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/GINIAnalyzer.py` & `azapy-1.2.0/azapy/Analyzers/GINIAnalyzer.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,92 +6,128 @@
 from ._RiskAnalyzer import _RiskAnalyzer
 from ._solvers import _lp_solver
 
 class GINIAnalyzer(_RiskAnalyzer):
     """
     GINI based optimal portfolio strategies.
     
-    Methods:
-        * getWeights
-        * getRisk
-        * getPositions
-        * getRiskComp
-        * getDiversification
-        * viewForntiers
-        * set_rrate
-        * set_mktdata
-        * set_rtype
-        * set_random_seed
+    **Attributes**
+        * `status` : `int` - the computation status (`0` - success, 
+          any other value signifies an error)
+        * `ww` : `pandas.Series` -  the portfolio weights 
+        * `RR` : `float` - portfolio rate of return
+        * `risk` : `float` - portfolio GINI risk
+        * `primary_risk_comp` : `list` - redundant (single element list 
+          containig GINI risk value)
+        * `secondary_risk_comp` : `list` - redundant 
+          (same as `primary_risk_comp`)
+        * `sharpe` : `float` - GINI-Sharpe ration if `rtype` is set to 
+          `'Shapre'` or `'Sharpe2'` otherwise `None`. 
+        * `diverse` : `float` - diversification factor if `rtype` is set 
+          to `'Divers'` or `'MaxDivers'` otherwise `None`.
+        * `name` : `str` - portfolio name
+        
+    Note the following 2 important methods:
+        * `getWeights` : Computes the optimal portfolio weights.
+          During its computations the following class members are also set:
+          `risk`, `primery_risk_comp`, `secondary_risk_comp`, `sharpe`,  `RR`, 
+          `divers`.
+        * `getPositions` : Provides practical information regarding the portfolio
+          rebalancing delta positions and costs.  
     """
     def __init__(self, mktdata=None, colname='adjusted', freq='Q', 
-                 hlength=1.25, calendar=None, 
-                 rtype='Sharpe', method='ecos', name='GINI'):
+                 hlength=1.25, name='GINI', rtype='Sharpe', mu=None, 
+                 d=1, mu0=0., aversion=None, ww0=None, method='ecos'):
         """
         Constructor
 
         Parameters
         ----------
-        `mktdata` : `pandas.DataFrame`, optional;
+        mktdata : `pandas.DataFrame`, optional
             Historic daily market data for portfolio components in the format
             returned by `azapy.mktData` function. The default is `None`.
-        `colname` : `str`, optional;
-            Name of the price column from mktdata used in the weights 
+        colname : `str`, optional
+            Name of the price column from mktdata used in the weight's 
             calibration. The default is `'adjusted'`.
-        `freq` : `str`, optional;
+        freq : `str`, optional
             Rate of return horizon. It could be 
-            `'Q'` for quarter or `'M'` for month. The default is `'Q'`.
-        `hlength` : `float`, optional;
+            `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
             History length in number of years used for calibration. A 
             fractional number will be rounded to an integer number of months.
-            The default is `1.25` years.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will 
-            be set to NYSE business calendar. 
-            The default is `None`.
-        `rtype` : `str`, optional;
+            The default is `3.25` years.
+        name : `str`, optional
+            Portfolio name. The default is `'GINI'`.
+        rtype : `str`, optional
             Optimization type. Possible values: \n
-                `'Risk'` : optimal-risk portfolio for targeted expected rate of 
+                `'Risk'` : optimal risk portfolio for targeted expected rate of 
                 return.\n
-                `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
-                `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
+                `'Sharpe'` : optimal Sharpe portfolio - maximization solution.\n
+                `'Sharpe2'` : optimal Sharpe portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
-                `'RiskAverse'` : optimal-risk portfolio for a fixed 
+                `'RiskAverse'` : optimal risk portfolio for a fixed 
                 risk-aversion factor.\n
-                `'InvNrisk'` : optimal-risk portfolio with the same risk value 
+                `'InvNrisk'` : optimal risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
-                `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
-                `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                `'Diverse'` : optimal diversified portfolio for targeted
+                expected rate of return (max of inverse 1-Diverse).\n
+                `'Diverse2'` : optimal diversified portfolio for targeted
+                expected rate of return (min of 1-Diverse).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
-                `'InvNdiverse'` : optimal-diversified portfolio with the same
+                `'InvNdiverse'` : optimal diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
-                `'InvNdrr'` : optima- diversified portfolio with the same 
+                `'InvNdrr'` : optimal diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `method` : `str`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
+            Targeted portfolio expected rate of return. 
+            Relevant only if `rtype='Risk'` or `rtype='Divers'`.
+            The default is `None`.
+        d : `int`, optional
+            Frontier type. Active only if `rtype='Risk'`. A value of `1` will
+            trigger the evaluation of optimal portfolio along the efficient
+            frontier. Otherwise, it will find the portfolio with the lowest
+            rate of return along the inefficient portfolio frontier.
+            The default is `1`.
+        mu0 : `float`, optional
+            Risk-free rate accessible to the investor.
+            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            The default is `0`.
+        aversion : `float`, optional
+            The value of the risk-aversion coefficient.
+            Must be positive. Relevant only if `rtype='RiskAverse'`.
+            The default is `None`.
+        ww0 : `list`, `numpy.array` or `pandas.Series`, optional
+            Targeted portfolio weights. 
+            Relevant only if `rype='InvNrisk'`.
+            Its length must be equal to the number of symbols in `rrate` 
+            (mktdata). All weights must be >= 0 with sum > 0.
+            If it is a `list` or a `numpy.array` then the weights are assumed 
+            to be in order of `rrate.columns`. If it is a `pandas.Series` then 
+            the index should be compatible with the `rrate.columns` or mktdata 
+            symbols (same symbols, not necessarily in the same order).
+            If it is `None` then it will be set to equal weights.
+            The default is `None`.
+        method : `str`, optional
             Linear programming numerical method. 
             Could be: `'ecos'`, `'highs-ds'`, `'highs-ipm'`, `'highs'`, 
             `'interior-point'`, `'glpk'` and `'cvxopt'`.
             The default is `'ecos'`.
-        `name` : `str`, optional;
-            Object name. The default is `'GINI'`.
-            
+          
         Returns
         -------
         The object.
         """
         self.drate = None
         self.nn2 = None
-        super().__init__(mktdata, colname, freq, hlength, calendar, rtype,
-                         name)
-        
+        super().__init__(mktdata, colname, freq, hlength, name,
+                         rtype, mu, d, mu0, aversion, ww0)
         self._set_method(method)
         
         
     def _set_method(self, method):
         self._set_lp_method(method)
         
     
@@ -103,16 +139,20 @@
         ----------
         rrate : `pandas.DataFrame`
             Market data. It will overwrite the value set by the constructor.
         Returns
         -------
         `None`
         """
+        if rrate is None:
+            # nothing to do
+            return
+        
         self.nn, self.mm = rrate.shape
-        self.muk = rrate.mean()
+        self.muk = rrate.mean(numeric_only=True)
         self.rrate = rrate.copy()
         
         self.nn2 = int(self.nn * (self.nn - 1) / 2)
         yy = []
         for m in range(self.mm):
             x = self.rrate.iloc[:,m]
             yy.append([x[i] - x[j] \
```

### Comparing `azapy-1.1.1/azapy/PortOpt/KellyEngine.py` & `azapy-1.2.0/azapy/Engines/KellyEngine.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,146 +1,161 @@
 import numpy as np
 import pandas as pd
 import cvxopt as cx
 import scipy.sparse as sps
 import warnings
+import time
 
 from ._RiskEngine import _RiskEngine
-from ._solvers import _qp_solver, _exp_cone_solver
+from azapy.Analyzers._solvers import _qp_solver, _exp_cone_solver
 
 class KellyEngine(_RiskEngine):
     """
     Kelly optimal portfolio.
     
-    Methods:
-        * getWeights
-        * getPositions
-        * set_rtype
-        * set_method
-        * set_rrate
-        * set_mktdata   
+    **Attributes**
+        * status : `int` - computation status (`0` - success, any other 
+          value indicates an error)
+        * ww : `pandas.Series` - portfolio weights
+        * name : `str` - portfolio name
     """
-    def __init__(self, mktdata=None, colname='adjusted', 
-                 freq='Q', hlength=3.25, calendar=None,
-                 rtype='ExpCone', method='ecos'):
+    def __init__(self, mktdata=None, colname='adjusted', freq='Q', 
+                 hlength=3.25, name='Kelly', rtype='ExpCone', method='ecos'):
         """
         Constructor
 
         Parameters
         ----------
-        `mktdata` : `pandas.DataFrame`, optional;
+        mktdata : `pandas.DataFrame`, optional
             Historic daily market data for portfolio components in the format
             returned by `azapy.mktData` function. The default is `None`.
-        `colname` : `str`, optional;
-            Name of the price column from mktdata used in the weights 
+        colname : `str`, optional
+            Name of the price column from `mktdata` used in the weight's 
             calibration. The default is `'adjusted'`.
-        `freq` : `str`, optional;
-            Rate of return horizon in number of business day. It could be 
-            'Q' for quarter or 'M' for month. The default is `'Q'`.
-        `hlength` : `float`, optional;
+        freq : `str`, optional
+            Rate of return horizon. It could be 
+            'Q' for a quarter or 'M' for a month. The default is `'Q'`.
+        hlength : `float`, optional
             History length in number of years used for calibration. A 
             fractional number will be rounded to an integer number of months.
             The default is `3.25` years.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will
-            be set to NYSE business calendar.
-            The default is `None`.
-        `rtype` : `str`, optional;
+        name : `str`, optional
+            Portfolio name. Deafult value is `'Kelly'`.
+        rtype : `str`, optional
             Optimization approximation. It can be:\n
                 'ExpCone' - exponential cone constraint programming solver 
                 for original Kelly problem. \n
                 'Full' - non-linear solver for original Kelly problem. \n
                 'Order2' - second order Taylor approximation of original Kelly 
                 problem. It is a QP problem. \n
             The default is `'ecos'`.
-        `method` : `str`, optional;
+        method : `str`, optional
             The QP solver class. It is relevant only if `rtype='Order2'`.
             It takes 2 values: 'ecos' or 'cvxopt'.
             The default is `'ecos'`.
         
         Returns
         -------
         The object.
         """
-        super().__init__(mktdata, colname, freq, hlength, calendar)
+        super().__init__(mktdata, colname, freq, hlength, name)
         
         self.rtypes = ["Full", "Order2", "ExpCone"]
         
         self.rtype = None
         self.set_rtype(rtype)
         self.method = None
         self._set_method(method)
         
         
-    def getWeights(self, rrate=None, rtype=None, method=None): 
+    def getWeights(self, rtype=None, method=None, mktdata=None, **params): 
         """
         Computes the Kelly optimal weights.
 
         Parameters
         ----------
-        `rrate` : `pandas.DataFrame`, optional;
-            Portfolio components historical rates of returns in the format 
-           "date", "symbol1", "symbol2", etc. A value different than `None` 
-           will overwrite the of 'rrate' set by the constructor from 
-           `mktdata`. The default is `None`.
-        `rtype` : `str`, optional;
+        rtype : `str`, optional
             Optimization approximation. It can be: \n
                 'ExpCone' - exponential cone constraint programming solver 
                 for original Kelly problem. \n
                 'Full' - non-linear solver for original Kelly problem. \n
                 'Order2' - second order Taylor approximation of original Kelly 
                 problem. It is a QP problem.\n  
             A value different than `None` will
             overwrite the value for `rtype` set in the constructor. \n
             The default is `None`.
-        `method` : `str`, optional;
+        method : `str`, optional
             The QP solver class. It is relevant only if `rtype='Order2'`.
             It takes 2 values: 'ecos' or 'cvxopt'.
             A value different than `None` will overwrite the
             value set in the constructor.
             The default is `None`.
+        mktdata : `pandas.DataFrame`, optional
+            The portfolio components historical, prices or rates of return, see
+            `'pclose'` definition below.
+            If it is not `None`, it will overwrite the set of historical rates
+            of return computed in the constructor from `'mktdata'`. 
+            The default is `None`. 
+        **params : other optional parameters
+            Most common: \n
+            `verbose` : Boolean, optional
+                If it set to `True`, then it will print a message when 
+                the optimal portfolio degenerates to a single asset.
+                The default is `False`.
+            `pclose` : Boolean, optional
+                If it is absent then the `mktdata` is considered to contain 
+                rates of return, with columns the asset symbols and indexed 
+                by the observation dates, \n
+                `True` : assumes `mktdata` contains closing prices only, 
+                with columns the asset symbols and indexed by the 
+                observation dates, \n
+                `False` : assumes `mktdata` is in the usual format
+                returned by `azapy.readMkT` function.
             
         Returns
         -------
-        `pandas.Series`
-            Portfolio weights.
+        `pandas.Series` : Portfolio weights per symbol.
         """
-        if rrate is not None:
-            self.set_rrate(rrate)
+        toc = time.perf_counter()
+        self._set_getWeights(mktdata, **params)
             
         if rtype is not None:
             self.set_rtype(rtype)
             
         if method is not None:
             self._set_method(method)
             
         if self.rtype == 'Full':
-            return self._calc_full()
+            self._calc_full()
         elif self.rtype == 'Order2':
-            return self._calc_order2()
+            self._calc_order2()
         elif self.rtype == 'ExpCone':
-            return self._calc_exp_cone()
+            self._calc_exp_cone()
         else:
             raise ValueError(f"rtype must be one of: {self.rtypes}")
             
+        self.time_level1 = time.perf_counter() - toc
+        
+        return self.ww
+            
     def _calc_full(self):
         mm = self.mm
         
         # local function
         def F(x=None, z=None):
             if x is None: 
                 return 0, cx.matrix(0.5/mm, (mm, 1))
             
             xx = np.array(x.T)[0]
         
             ff = self.rrate.apply(lambda row: np.dot(xx, row) + 1 , axis=1)
-            val = -np.log(ff).mean()
+            val = -np.log(ff).mean(numeric_only=True)
             
             rf = self.rrate.apply(lambda col: col / ff)
-            DF = cx.matrix(-rf.mean()).T
+            DF = cx.matrix(-rf.mean(numeric_only=True)).T
             
             if z is None: 
                 return val, DF
             
             H = np.zeros((mm, mm))
             for i in range(mm):
                 for j in range(i + 1):
@@ -155,55 +170,62 @@
         
         G = cx.spmatrix(data, irow, icol, (mm + 1, mm))
         
         h = cx.matrix([0.] * mm + [1.])
         
         dims = {'l': mm + 1, 'q': [], 's': []}
         
+        # calc
+        toc = time.perf_counter()
         res = cx.solvers.cp(F, G=G, h=h, dims=dims, 
                             options={'show_progress': False})
+        self.time_level2 = time.perf_counter() - toc
         
+        self.status = 0
         if 'optimal' not in res['status']:
+            self.status = 1
             warnings.warn(f"Warning {res['status']}")
             return pd.Series(np.nan, index=self.rrate.columns)
         
-        return pd.Series(res['x'], index=self.rrate.columns)
+        self.ww = pd.Series(res['x'], index=self.rrate.columns)
         
     
     def _calc_order2(self):
         mm = self.mm
 
         # build P and q
         P = np.zeros((mm, mm))
         for i in range(mm):
             for j in range(i+1):
-                P[i,j] = (self.rrate.iloc[:,i] * self.rrate.iloc[:,j]).mean()
+                P[i,j] = (self.rrate.iloc[:,i] * self.rrate.iloc[:,j]).mean(numeric_only=True)
                 P[j,i] = P[i,j]
         
         q_data = list(-self.muk)    
 
         #build G and h
         icol = list(range(mm)) * 2
         irow = list(range(mm)) + [mm] * mm
         data = [-1.] * mm + [1.] * mm
         
         G = sps.coo_matrix((data, (irow, icol)), shape=(mm + 1, mm))
         
         h_data = [0.] * mm + [1.]
 
         # calc
+        toc = time.perf_counter()
         res = _qp_solver(self.method, P, q_data, G, h_data)
+        self.time_level2 = time.perf_counter() - toc
         
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {res['status']}: {res['infostring']} "
                         + f"on calibration date {self.rrate.index[-1]}")
             return pd.Series(np.nan, index=self.rrate.columns)    
 
-        return pd.Series(res['x'], index=self.rrate.columns)
+        self.ww = pd.Series(res['x'], index=self.rrate.columns)
         
     
     def _calc_exp_cone(self):
         # w <- [0:mm]
         # s <- [mm: mm + nn]
         # in total dim = mm + nn
         mm = self.mm
@@ -238,36 +260,38 @@
         
         # build b
         b = [1.]
         
         dims = {'l': mm, 'q': [], 'e': nn}
         
         # calc
+        toc = time.perf_counter()
         res = _exp_cone_solver('ecos', c, G, h, dims, A, b)
+        self.time_level2 = time.perf_counter() - toc
         
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {res['status']}: {res['infostring']} "
                         + f"on calibration date {self.rrate.index[-1]}")
             return pd.Series(np.nan, index=self.rrate.columns)    
 
-        return pd.Series(res['x'][:mm], index=self.rrate.columns)
+        self.ww = pd.Series(res['x'][:mm], index=self.rrate.columns)
         
     
     def set_rtype(self, rtype):
         """
         Sets the model approximation level.
 
         Parameters
         ----------
-        `rtype` : `str`;
-            It could be: `'Full'` for a non-linear (no approximation) model, 
-            `'ExpCone'` for exponential cone constraint programming solver,
-            or `'Order2'` for a second order Taylor approximation 
-            (a QP problem).\n
+        rtype : `str`
+            It could be: \n
+                - `'Full'` for a non-linear (no approximation) model, 
+                - `'ExpCone'` for exponential cone constraint programming solver,
+                - `'Order2'` for a second order Taylor approximation (a QP problem).\n
             It will overwrite the value set by the constructor.
             
         Returns
         -------
         `None`
         """
         if not rtype in self.rtypes:
```

### Comparing `azapy-1.1.1/azapy/PortOpt/LSDAnalyzer.py` & `azapy-1.2.0/azapy/Analyzers/CVaRAnalyzer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,856 +1,893 @@
 import numpy as np
 import scipy.sparse as sps
 import warnings
 import time
 
-from .MADAnalyzer import MADAnalyzer
-from ._solvers import _socp_solver
+from ._RiskAnalyzer import _RiskAnalyzer
+from ._solvers import _lp_solver
 
-class LSDAnalyzer(MADAnalyzer):
+class CVaRAnalyzer(_RiskAnalyzer):
     """
-    m-level LSD based optimal portfolio strategies.
-    
-    Methods:
-        * getWeights
-        * getRisk
-        * getPositions
-        * getRiskComp
-        * getDiversification
-        * viewForntiers
-        * set_rrate
-        * set_mktdata
-        * set_rtype
-        * set_random_seed
+    Mixture CVaR (Conditional Value at Risk) 
+    based optimal portfolio strategies.
+        
+    **Attributes**
+        * `status` : `int` - the computation status (`0` - success, 
+          any other value signifies an error)
+        * `ww` : `pandas.Series` -  the portfolio weights 
+        * `RR` : `float` - portfolio rate of return
+        * `risk` : `float` - portfolio mCVaR risk
+        * `primary_risk_comp` : `list` - CVaR components of portfolio mCVaR
+        * `secondary_risk_comp` : `list` - VaR values associated with CVaR
+          components
+        * `sharpe` : `float` - mCVaR-Sharpe ration if `rtype` is set to 
+          `'Shapre'` or `'Sharpe2'` otherwise `None`. 
+        * `diverse` : `float` - diversification factor if `rtype` is set 
+          to `'Divers'` or `'MaxDivers'` otherwise `None`.
+        * `name` : `str` - portfolio name
+        
+    Note the following 2 important methods:
+        * `getWeights` : Computes the optimal portfolio weights.
+          During its computations the following class members are also set:
+          `risk`, `primery_risk_comp`, `secondary_risk_comp`, `sharpe`,  `RR`, 
+          `divers`.
+        * `getPositions` : Provides practical information regarding the portfolio
+          rebalancing delta positions and costs.  
     """
-    def __init__(self, coef=[1.], 
-                 mktdata=None, colname='adjusted', freq='Q', 
-                 hlength=3.25, calendar=None,
-                 rtype='Sharpe', method='ecos', name='LSD'):
+    def __init__(self, alpha=[0.975], coef=None, mktdata=None, 
+                 colname='adjusted', freq='Q', hlength=3.25, name='CVaR', 
+                 rtype='Sharpe', mu=None, d=1, mu0=0., aversion=None, 
+                 ww0=None, method='ecos'):
         """
         Constructor
 
         Parameters
         ----------
-        `coef` : `list`, optional;
-            Positive non-increasing list of mixture coefficients. 
-            The default is `[1.]`.
-        `mktdata` : `pandas.DataFrame`, optional;
+        alpha : `list`, optional
+            List of distinct confidence levels. The default is `[0.975]`.
+        coef : `list`, optional
+            List of positive mixture coefficients. Must be the same size as 
+            `alpha`. A `None` value assumes an equal weighted risk mixture.
+            The vector of coefficients will be normalized to unit.
+            The default is `None`.
+        mktdata : `pandas.DataFrame`, optional
             Historic daily market data for portfolio components in the format
             returned by `azapy.mktData` function. The default is `None`.
-        `colname` : `str`, optional;
-            Name of the price column from mktdata used in the weights 
+        colname : `str`, optional
+            Name of the price column from mktdata used in the weight's 
             calibration. The default is `'adjusted'`.
-        `freq` : `str`, optional;
+        freq : `str`, optional
             Rate of return horizon. It could be 
-            `'Q'` for quarter or `'M'` for month. The default is `'Q'`.
-        `hlength` : `float`, optional;
+            `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
             History length in number of years used for calibration. A 
             fractional number will be rounded to an integer number of months.
             The default is `3.25` years.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will 
-            be set to NYSE business calendar. 
-            The default is `None`.
-        `rtype` : `str`, optional;
+        name : `str`, optional
+            Portfolio name. The default is `'CVaR'`.
+        rtype : `str`, optional
             Optimization type. Possible values: \n
-                `'Risk'` : optimal-risk portfolio for targeted expected rate of 
+                `'Risk'` : optimal risk portfolio for targeted expected rate of 
                 return.\n
-                `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
-                `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
+                `'Sharpe'` : optimal Sharpe portfolio - maximization solution.\n
+                `'Sharpe2'` : optimal Sharpe portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
-                `'RiskAverse'` : optimal-risk portfolio for a fixed 
+                `'RiskAverse'` : optimal risk portfolio for a fixed 
                 risk-aversion factor.\n
-                `'InvNrisk'` : optimal-risk portfolio with the same risk value 
+                `'InvNrisk'` : optimal risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
-                `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
-                `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                `'Diverse'` : optimal diversified portfolio for targeted
+                expected rate of return (max of inverse 1-Diverse).\n
+                `'Diverse2'` : optimal diversified portfolio for targeted
+                expected rate of return (min of 1-Diverse).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
-                `'InvNdiverse'` : optimal-diversified portfolio with the same
+                `'InvNdiverse'` : optimal diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
-                `'InvNdrr'` : optima- diversified portfolio with the same 
+                `'InvNdrr'` : optimal diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `method` : `str`, optional;
-            SOCP numerical method. 
-            Could be: `'ecos'` or `'cvxopt'`.
-            The defualt is `'ecos'`.
-        `name` : `str`, optional;
-            Object name. The default is `'LSD'`.
-
+            The default is `'Sharpe'`.
+        mu : `float`, optional
+            Targeted portfolio expected rate of return. 
+            Relevant only if `rtype='Risk'` or `rtype='Divers'`.
+            The default is `None`.
+        d : `int`, optional
+            Frontier type. Active only if `rtype='Risk'`. A value of `1` will
+            trigger the evaluation of optimal portfolio along the efficient
+            frontier. Otherwise, it will find the portfolio with the lowest
+            rate of return along the inefficient portfolio frontier.
+            The default is `1`.
+        mu0 : `float`, optional
+            Risk-free rate accessible to the investor.
+            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            The default is `0`.
+        aversion : `float`, optional
+            The value of the risk-aversion coefficient.
+            Must be positive. Relevant only if `rtype='RiskAverse'`.
+            The default is `None`.
+        ww0 : `list`, `numpy.array` or `pandas.Series`, optional
+            Targeted portfolio weights. 
+            Relevant only if `rype='InvNrisk'`.
+            Its length must be equal to the number of symbols in `rrate` 
+            (mktdata). All weights must be >= 0 with sum > 0.
+            If it is a `list` or a `numpy.array` then the weights are assumed 
+            to be in order of `rrate.columns`. If it is a `pandas.Series` then 
+            the index should be compatible with the `rrate.columns` or mktdata 
+            symbols (same symbols, not necessarily in the same order).
+            If it is `None` then it will be set to equal weights.
+            The default is `None`.
+        method : `str`, optional
+            Linear programming numerical method. 
+            Could be: `'ecos'`, `'highs-ds'`, `'highs-ipm'`, `'highs'`, 
+            `'interior-point'`, `'glpk'` and `'cvxopt'`.
+            The default is `'ecos'`.
+        
         Returns
         -------
         The object.
         """
-        super().__init__(coef, mktdata, colname, freq, hlength, calendar,
-                         rtype, method, name)
+        super().__init__(mktdata, colname, freq, hlength, name,
+                         rtype, mu, d, mu0, aversion, ww0)
+        self._set_method(method)
+        self.alpha = np.array(alpha)
+        
+        if any((self.alpha <= 0.) | (1. <= self.alpha)):
+            raise ValueError("All alpha coefficients must be in (0,1)")
+        if len(np.unique(self.alpha)) != len(self.alpha):
+            raise ValueError("alpha values are not unique")
+            
+        self.ll = len(alpha)
+            
+        if coef is None:
+            self.coef = np.full(self.ll, 1/self.ll)
+        else:
+            self.coef = np.array(coef)
+        
+            if len(self.coef) != len(self.alpha):
+                raise ValueError("alpha and coef must have the same length")
+            if any(self.coef <= 0.):
+                raise ValueError("All coef must be positive")
         
+            self.coef = self.coef / self.coef.sum()
         
+
+
     def _set_method(self, method):
-        self._set_socp_method(method)
+        self._set_lp_method(method)
         
         
-    def _risk_calc_(self, prate):
-        # mu = np.mean(prate)
-        # prate = prate - mu
-        # nn = len(prate)
-        delta = []
-        mu = 0.
-        for _ in range(self.ll):
-            xrate = mu - prate
-            xrate[xrate <= 0.] = 0.
-            dd = np.sqrt(np.mean(xrate**2))
-            delta.append(dd)
-            mu -= dd
-            
-        self.primary_risk_comp = np.array(delta)
-        self.secondary_risk_comp = \
-            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
-        self.risk = np.dot(self.primary_risk_comp, self.coef)
-        self.status = 0
+    def _risk_calc_lp(self, prate, alpha):
+        # lp formulation of CVaR & VaR
+        # Order of variables:
+        # u <- 0, 
+        # s <- [1:nn] 
+        # in total dim=nn + 1
+        nn = self.nn
         
-        return self.risk
-
+        # build c
+        c_data = [1.] + [1. / (1. - alpha) / nn] * nn
+        
+        # build G
+        G_icol = [0] * nn + list(range(1, nn + 1)) + list(range(nn+1))
+        G_irow = list(range(nn)) * 2 + list(range(nn, 2 * nn + 1))
+        G_data = [-1.] * (3 * nn + 1)
+        
+        G_shape = (2 * nn + 1, nn + 1)
+        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
 
+        # build h
+        h_data = list(prate) + [0.] * (nn + 1)
+    
+        # calc
+        toc = time.perf_counter()
+        res = _lp_solver(self.method, c_data, G, h_data)
+        self.time_level2 = time.perf_counter() - toc
+        
+        if res['status'] != 0:
+            return 2, np.nan, np.nan
+        
+        VaR = res['x'][0]
+        CVaR = res['pcost']
+  
+        return 0, VaR, CVaR
+    
+    
+    def _risk_calc(self, prate, alpha):
+        # Analytic formulation of CVaR & VaR
+        ws = np.sort(prate)
+        nnl = len(ws) * (1. - alpha)
+        VaR = -ws[int(nnl)]
+        CVaR = VaR - (ws[ws <= -VaR] + VaR).sum() / nnl
+        
+        return 0, VaR, CVaR
+    
+    
     def _risk_min(self, d=1):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
         #   u_l <- mm + l(nn+1), 
         #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # in total dim = mm + ll(nn + 1)
+        ll = self.ll
         nn = self.nn
         mm = self.mm
-        ll = self.ll 
     
         # build c
-        c_data = [0.] * mm 
+        c_data = [0] * mm
         for l in range(ll):
-            c_data += [self.coef[l]] + [0.] * nn
-        
+            c_data += [self.coef[l]] \
+                    + [self.coef[l] / (1 - self.alpha[l] ) / nn] * nn
+       
         # build G
-        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
-                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
-                       for _ in range(l)] \
-                  + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1.] * ((l + 1) * nn)
+            G_icol += [mm + l * (nn + 1)] * nn \
+                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += list(range(l * nn, (l + 1) * nn)) \
+                + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1] * nn + [-1] * nn
             
-        G_icol += list(range(mm)) 
-        G_irow += [ll * nn] * mm
+        G_icol += list(range(mm))
+        G_irow += [nn * ll] * mm
         G_data += list(-self.muk * d)
         
         G_icol += list(range(mm + ll * (nn + 1)))
-        G_irow += list(range(nn * ll + 1, mm + 2 * nn * ll + ll + 1))
-        G_data += [-1.] * (mm + ll * (nn + 1))
-        # cone
-        for l in range(ll):
-            G_icol += list(range((nn + 1) * l + mm , 
-                                 (nn + 1) * l + mm + 1 + nn))
-            G_irow += list(range(mm + 2 * nn * ll + ll + 1 + l * (nn + 1), 
-                                 mm + 2 * nn * ll + ll + 1 + (l + 1) * (nn + 1)))
-            G_data += [-np.sqrt(nn)] + [-1.] * nn
-            
-        G_shape = (3 * nn * ll + 1 + mm + 2 * ll, mm + ll * (nn + 1))
-        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
+        G_irow += list(range(ll * nn + 1, ll * nn + 1 + mm + ll * (nn + 1)))
+        G_data += [-1.] * (mm + ll * (nn + 1) )
         
-        #build h
-        h_data = [0.] * (nn * ll) + [-self.mu * d] \
-               + [0.] * (mm + 2 * ll * (nn + 1))
-        
-        # build dims
-        dims = {'l': (2 * ll * nn + ll + 1 + mm), 'q': [nn + 1] * ll}
+        G_shape = (nn * ll + 1 + mm + ll * (nn + 1), mm + (nn + 1) * ll)
+        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
+ 
+        # build h
+        h_data = [0.] * (nn * ll) + [-self.mu * d] + [0.] *(mm + ll * (nn + 1))
         
         # build A
         A_icol = list(range(mm))
         A_irow = [0] * mm
         A_data = [1.] * mm
         
         A_shape = (1, mm + ll * (nn + 1))
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
-        
+
         # build b
         b_data = [1.]
         
         # calc
         toc = time.perf_counter()
-        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
+        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
         self.time_level2 = time.perf_counter() - toc
  
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-        
-        # mLSD
+            
+        # VaR (u)
+        self.secondary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
+                                    for l in range(ll)])
+        # mCVaR
         self.risk = res['pcost']
-        # delta-risk values
-        self.primary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
-                                           for l in range(ll)])
-        # delta-risk strikes
-        self.secondary_risk_comp = \
-            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
+        # CVaR (recomputed)
+        self.primary_risk_comp = \
+            np.array([res['x'][mm + l * (nn + 1)] \
+             + 1 / (1 - self.alpha[l]) * np.mean(
+                 res['x'][(mm + l * (nn + 1) + 1) : (mm + (l + 1) * (nn + 1))])
+             for l in range(ll)])
         # optimal weights
         self.ww = np.array(res['x'][:mm])
         self.ww.shape = mm
-        # rate of return
+        # rate of returns
         self.RR = np.dot(self.ww, self.muk)
         
         return self.ww
-        
+    
     
     def _sharpe_max(self):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
-        # u_l <- mm + l(nn+1), 
-        # s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
+        #   u_l <- mm + l(nn+1), 
+        #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # and last t <- [mm + ll(nn + 1)]
         # in total dim = mm + ll(nn + 1) + 1
         ll = self.ll
         nn = self.nn
         mm = self.mm
         
         # build c
         c_data = list(-self.muk) + [0.] * (ll * (nn + 1)) + [self.mu]
         
         # build G
-        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
-                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
-                       for _ in range(l)] \
-                  + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1.] * ((l + 1) * nn)
-
+            G_icol += [mm + l * (nn + 1)] * nn \
+                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += list(range(l * nn, (l + 1) * nn)) \
+                + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1] * nn + [-1] * nn
+            
         G_icol += list(range(mm + ll * (nn + 1) + 1))
-        G_irow += list(range(nn * ll, mm + 2 * nn * ll + ll + 1))
+        G_irow += list(range(ll * nn, ll * nn + mm + ll * (nn + 1) + 1))
         G_data += [-1.] * (mm + ll * (nn + 1) + 1)
-        # cone
-        for l in range(ll):
-            G_icol += list(range((nn + 1) * l + mm , 
-                                 (nn + 1) * l + mm + 1 + nn))
-            G_irow += list(range(mm + 2 * nn * ll + ll + 1 + l * (nn + 1), 
-                                 mm + 2 * nn * ll + ll + 1 + (l + 1) * (nn + 1)))
-            G_data += [-np.sqrt(nn)] + [-1.] * nn
-            
-        G_shape = (3 * nn * ll + mm + 2 * ll + 1, mm + ll * (nn + 1) + 1)
-        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
         
+        G_shape = (ll * nn + mm + ll * (nn + 1) + 1, mm + ll * (nn + 1) + 1)
+        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
+      
         # build h
-        h_data = [0.] * (3 * nn * ll + mm + 2 * ll + 1)
-        
-        # build dims
-        dims = {'l': (2 * ll * nn + mm + ll + 1), 'q': [nn + 1] * ll}
+        h_data = [0.] * (nn * ll + mm + ll * (nn + 1) + 1)
         
         # build A
         A_icol = list(range(mm)) + [mm + ll * (nn + 1)]
         A_irow = [0] * (mm + 1)
         A_data = [1.] * mm + [-1.]
-        
-        A_icol += [mm + l * (nn + 1) for l in range(ll)]
-        A_irow += [1] * ll
-        A_data += list(self.coef)
-        
+        for l in range(ll):
+            A_icol += [mm + l * (nn + 1)] \
+                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            A_irow += [1] * (nn + 1)
+            A_data += [self.coef[l]] \
+                + [self.coef[l] / (1 - self.alpha[l]) / nn ] * nn
+ 
         A_shape = (2, mm + ll * (nn + 1) + 1)
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
- 
+  
         # build b
         b_data = [0., 1.]
         
         # calc
         toc = time.perf_counter()
-        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
+        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
         self.time_level2 = time.perf_counter() - toc
- 
+       
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-        
-        # mLSD
+
+        # mCVaR (1/t)
         self.risk = 1. / res['x'][-1]
-        # delta-risk values
-        self.primary_risk_comp = np.array(
-            [res['x'][mm + l * (nn + 1)] * self.risk for l in range(ll)])
-        # mLSD-Sharpe
+        # VaR (u)
+        self.secondary_risk_comp = \
+            np.array([res['x'][mm + l * (nn + 1)] * self.risk \
+                      for l in range(ll)])
+        # Sharpe
         self.sharpe = -res['pcost']
         # optimal weights
         self.ww = np.array(res['x'][:mm] * self.risk)
         self.ww.shape = mm
         # rate of return
-        self.RR = self.sharpe * self.risk + self.mu
-        # delta-risk strikes
-        self.secondary_risk_comp = \
-            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
+        self.RR = np.dot(self.ww, self.muk)
+        # component CVaR (recomputed)
+        self.primary_risk_comp = \
+            np.array([(res['x'][mm + l * (nn + 1)] + 1 / (1 - self.alpha[l]) \
+            * np.mean(res['x'][(mm + l * (nn + 1) + 1) :\
+                               (mm + (l + 1) * (nn + 1))])) \
+            * self.risk for l in range(ll)])
         
         return self.ww
     
     
     def _sharpe_inv_min(self):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
-        # u_l <- mm + l(nn+1), 
-        # s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
+        #   u_l <- mm + l(nn+1), 
+        #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # and last t <- [mm + ll(nn + 1)]
         # in total dim = mm + ll(nn + 1) + 1
         ll = self.ll
         nn = self.nn
         mm = self.mm
         
-        # build c
+        # build c   
         c_data = [0.] * mm 
         for l in range(ll):
-            c_data += [self.coef[l]] + [0.] * nn
+            c_data += [self.coef[l]] \
+                    + [self.coef[l] / (1. - self.alpha[l]) / nn] * nn
         c_data += [0.]
         
         # build G
-        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
-                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
-                       for _ in range(l)]\
-                  + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1.] * ((l + 1) * nn)
-
+            G_icol += [mm + l * (nn + 1)] * nn \
+                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += list(range(l * nn, (l + 1) * nn)) \
+                + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1.] * nn + [-1.] * nn
+            
         G_icol += list(range(mm + ll * (nn + 1) + 1))
-        G_irow += list(range(nn * ll, mm + 2 * nn * ll + ll + 1))
+        G_irow += list(range(ll * nn, ll * nn + mm + ll * (nn + 1) + 1))
         G_data += [-1.] * (mm + ll * (nn + 1) + 1)
-        # cone
-        for l in range(ll):
-            G_icol += list(range((nn + 1) * l + mm , 
-                                 (nn + 1) * l + mm + 1 + nn))
-            G_irow += list(range(mm + 2 * nn * ll + ll + 1 + l * (nn + 1), 
-                           mm + 2 * nn * ll + ll + 1 + (l + 1) * (nn + 1)))
-            G_data += [-np.sqrt(nn)] + [-1.] * nn
-            
-        G_shape = (3 * nn * ll + mm + 2 * ll + 1, mm + ll * (nn + 1) + 1)
-        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
         
+        G_shape = (ll * nn + mm + ll * (nn + 1) + 1, mm + ll * (nn + 1) + 1)
+        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
+     
         # build h
-        h_data = [0.] * (3 * nn * ll + mm + 2 * ll + 1)
+        h_data = [0.] * (nn * ll + mm + ll * (nn + 1) + 1)
         
-        # build dims
-        dims = {'l': (2 * ll * nn + mm + ll + 1), 'q': [nn + 1] * ll}
+        #build A
+        A_icol = list(range(mm)) + [mm + ll * (nn + 1)]
+        A_irow = [0] * (mm + 1)
+        A_data = [1.] * mm + [-1.]
         
-        # build A
-        A_icol = (list(range(mm)) + [mm + ll * (nn + 1)]) * 2
-        A_irow = [0] * (mm + 1) + [1] * (mm + 1)
-        A_data = [1.] * mm + [-1.] + list(self.muk) + [-self.mu]
+        A_icol += list(range(mm)) + [mm + ll * (nn + 1)]
+        A_irow += [1] * (mm + 1)
+        A_data += list(self.muk) + [-self.mu]
         
         A_shape = (2, mm + ll * (nn + 1) + 1)
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
- 
-        # bjuild b
+     
+        # build b
         b_data = [0., 1.]
-        
+
         # calc
         toc = time.perf_counter()
-        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
+        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
         self.time_level2 = time.perf_counter() - toc
- 
+       
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-        
-        # mLSD-Sharpe
-        self.sharpe = 1. / res['pcost']
-        # mLSD
+
         t = res['x'][-1]
+        # mCVaR (g/t)
         self.risk = res['pcost'] / t
-        # delta-risk values
-        self.primary_risk_comp = np.array(
-            [res['x'][mm + l * (nn + 1)] / t for l in range(ll)])
-        
+        # VaR (u)
+        self.secondary_risk_comp = \
+            np.array([res['x'][mm + l * (nn + 1)] / t for l in range(ll)])
+        # Sharpe
+        self.sharpe = 1. / res['pcost']
         # optimal weights
         self.ww = np.array(res['x'][:mm] / t)
         self.ww.shape = mm
         # rate of return
         self.RR = 1. / t + self.mu
-        # delta-risk strikes
-        self.secondary_risk_comp = \
-            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
+        # component CVaR (recomputed)
+        self.primary_risk_comp = \
+            np.array([(res['x'][mm + l * (nn + 1)] + 1 / (1 - self.alpha[l]) \
+            * np.mean(res['x'][(mm + l * (nn + 1) + 1) :\
+                            (mm + (l + 1) * (nn + 1))])) /t \
+            for l in range(ll)])
         
         return self.ww
-        
+    
     
     def _rr_max(self):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
         #   u_l <- mm + l(nn+1), 
         #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # in total dim = mm + ll(nn + 1)
+        ll = self.ll
         nn = self.nn
         mm = self.mm
-        ll = self.ll 
-        
+    
         # build c
-        c_data = list(-self.muk) + [0.] * (ll * (nn + 1))
-        
+        c_data = list(-self.muk) + [0.] * ((nn + 1) * ll)
+            
         # build G
-        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
-                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
-                       for _ in range(l)] \
-                  + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1.] * ((l + 1) * nn)
-
+            G_icol += [mm + l * (nn + 1)] * nn \
+                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += list(range(l * nn, (l + 1) * nn)) \
+                + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1.] * nn + [-1.] * nn
+            
         G_icol += list(range(mm + ll * (nn + 1)))
-        G_irow += list(range(nn * ll, mm + 2 * nn * ll + ll))
+        G_irow += list(range(ll * nn, ll * nn + mm + ll * (nn + 1)))
         G_data += [-1.] * (mm + ll * (nn + 1))
-        # cone
-        for l in range(ll):
-            G_icol += list(range((nn + 1) * l + mm , 
-                                 (nn + 1) * l + mm + 1 + nn))
-            G_irow += list(range(mm + 2 * nn * ll + ll + l * (nn + 1), 
-                                 mm + 2 * nn * ll + ll + (l + 1) * (nn + 1)))
-            G_data += [-np.sqrt(nn)] + [-1.] * nn
-            
-        G_shape = (3 * nn * ll + mm + 2 * ll, mm + ll * (nn + 1))
-        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
         
+        G_shape = (nn * ll + mm + (nn + 1) * ll, mm + (nn + 1) * ll )
+        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
+
         # build h
-        h_data = [0.] * (3 * nn * ll + mm + 2 * ll)
-        
-        # build dims
-        dims = {'l': (2 * ll * nn + mm + ll), 'q': [nn + 1] * ll}
+        h_data = [0.] * (nn * ll + mm + (nn + 1) * ll)
         
         # build A
-        A_icol = list(range(mm)) + [mm + l * (nn + 1) for l in range(ll)]
-        A_irow = [0] * mm + [1] * ll
-        A_data = [1.] * mm + list(self.coef)
-        
-        A_shape = (2, mm + ll * (nn + 1))
+        A_icol = list(range(mm + (nn + 1) * ll))
+        A_irow = [0] * mm + [1] * ((nn + 1) * ll)
+        A_data = [1.] * mm
+        for l in range(ll):
+            A_data += [self.coef[l]] \
+                  + [self.coef[l] / (1 - self.alpha[l]) / nn] * nn
+
+        A_shape = (2, mm + (nn + 1) * ll)
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
-        
+   
         # build b
         b_data = [1., self.risk]
         
         # calc
         toc = time.perf_counter()
-        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
+        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
         self.time_level2 = time.perf_counter() - toc
- 
+       
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-        
-        # rate of return
-        self.RR = -res['pcost']
-        # delta-risk values
-        self.primary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
-                                           for l in range(ll)])
-        # delta-risk strikes
-        self.secondary_risk_comp = \
-            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
+
+        # VaR (u)
+        self.secondary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
+                                    for l in range(ll)])
+        # CVaR (recomputed)
+        self.primary_risk_comp = \
+            np.array([res['x'][mm + l * (nn + 1)] \
+             + 1 / (1 - self.alpha[l]) * np.mean(
+                 res['x'][(mm + l * (nn + 1) + 1) : (mm + (l + 1) * (nn + 1))])
+             for l in range(ll)])
         # optimal weights
         self.ww = np.array(res['x'][:mm])
         self.ww.shape = mm
-
-        return self.ww
+        # rate of return
+        self.RR = -res['pcost']
+        # mCVaR recalculate
+        self.risk = np.dot(self.coef, self.primary_risk_comp)
         
+        return self.ww 
+ 
     
     def _risk_averse(self):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
         #   u_l <- mm + l(nn+1), 
         #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # in total dim = mm + ll(nn + 1)
+        ll = self.ll
         nn = self.nn
         mm = self.mm
-        ll = self.ll 
-        
+    
         # build c
         c_data = list(-self.muk)
         for l in range(ll):
-            c_data += [self.Lambda * self.coef[l]] + [0.] * nn
-        
+            c_data += [self.Lambda * self.coef[l]] \
+               + [self.Lambda * self.coef[l] / (1 - self.alpha[l] ) / nn] * nn
+            
         # build G
-        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
-                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
-                       for _ in range(l)]\
-                  + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1.] * ((l + 1) * nn)
-
+            G_icol += [mm + l * (nn + 1)] * nn \
+                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += list(range(l * nn, (l + 1) * nn)) \
+                + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1] * nn + [-1] * nn
+            
         G_icol += list(range(mm + ll * (nn + 1)))
-        G_irow += list(range(nn * ll, mm + 2 * nn * ll + ll))
+        G_irow += list(range(ll * nn, ll * nn + mm + ll * (nn + 1)))
         G_data += [-1.] * (mm + ll * (nn + 1))
-        # cone
-        for l in range(ll):
-            G_icol += list(range((nn + 1) * l + mm , 
-                                 (nn + 1) * l + mm + 1 + nn))
-            G_irow += list(range(mm + 2 * nn * ll + ll + l * (nn + 1), 
-                                 mm + 2 * nn * ll + ll + (l + 1) * (nn + 1)))
-            G_data += [-np.sqrt(nn)] + [-1.] * nn
-            
-        G_shape = (3 * nn * ll + mm + 2 * ll, mm + ll * (nn + 1))
-        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
         
+        G_shape = (nn * ll + mm + (nn + 1) * ll, mm + (nn + 1) * ll)
+        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
+
         # build h
-        h_data = [0.] * (3 * nn * ll + mm + 2 * ll)
+        h_data = [0.] * (nn * ll + mm + (nn + 1) * ll)
         
-        # build dims
-        dims = {'l': (2 * ll * nn + mm + ll), 'q': [nn + 1] * ll}
-        
-        # build A 
+        # build A
         A_icol = list(range(mm))
         A_irow = [0] * mm
         A_data = [1.] * mm
         
         A_shape = (1, mm + ll * (nn + 1))
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
-        
+
         # build b
         b_data = [1.]
         
         # calc
         toc = time.perf_counter()
-        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
+        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
         self.time_level2 = time.perf_counter() - toc
- 
+       
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-        
+
         # optimal weights
         self.ww = np.array(res['x'][:mm])
         self.ww.shape = mm
-        # rate of return
+        # VaR (u)
+        self.secondary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
+                                    for l in range(ll)])
+        # rate of returns
         self.RR = np.dot(self.ww, self.muk)
-        # mLSD
-        self.risk = (self.RR + res['pcost']) / self.Lambda
-        # delta-risk values
-        self.primary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
-                                           for l in range(ll)])
-        # delta-risk strikes
-        self.secondary_risk_comp = \
-            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
+        # mCVaR
+        self.risk = (res['pcost'] + self.RR) / self.Lambda
+        # CVaR (recomputed)
+        self.primary_risk_comp = \
+            np.array([res['x'][mm + l * (nn + 1)] \
+             + 1 / (1 - self.alpha[l]) * np.mean(
+                 res['x'][(mm + l * (nn + 1) + 1) : (mm + (l + 1) * (nn + 1))])
+             for l in range(ll)])
         
         return self.ww
-    
+        
     
     def _risk_diversification(self, d=1):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
-        # u_l <- mm + l(nn+1), 
-        # s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
+        #   u_l <- mm + l(nn+1), 
+        #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # and last t <- [mm + ll(nn + 1)]
         # in total dim = mm + ll(nn + 1) + 1
         ll = self.ll
         nn = self.nn
         mm = self.mm
         
-        # build c
+        # build c   
         c_data = [0.] * mm 
         for l in range(ll):
-            c_data += [self.coef[l]] + [0.] * nn
+            c_data += [self.coef[l]] \
+                    + [self.coef[l] / (1. - self.alpha[l]) / nn] * nn
         c_data += [0.]
         
         # build G
-        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
-                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
-                       for _ in range(l)]\
-                  + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1.] * ((l + 1) * nn)
+            G_icol += [mm + l * (nn + 1)] * nn \
+                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += list(range(l * nn, (l + 1) * nn)) \
+                + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1.] * nn + [-1.] * nn
+            
             
         G_icol += list(range(mm)) + [mm + ll * (nn + 1)]
-        G_irow += [nn * ll] * (mm + 1)
+        G_irow += [ll * nn] * (mm + 1)
         G_data += list(-self.muk * d) + [self.mu * d]
-
+            
         G_icol += list(range(mm + ll * (nn + 1) + 1))
-        G_irow += list(range(nn * ll + 1, mm + 2 * nn * ll + ll + 2))
+        G_irow += list(range(ll * nn + 1, ll * nn + mm + ll * (nn + 1) + 2))
         G_data += [-1.] * (mm + ll * (nn + 1) + 1)
-        # cone
-        for l in range(ll):
-            G_icol += list(range((nn + 1) * l + mm , 
-                                 (nn + 1) * l + mm + 1 + nn))
-            G_irow += list(range(mm + 2 * nn * ll + ll + 2 + l * (nn + 1), 
-                           mm + 2 * nn * ll + ll + 2 + (l + 1) * (nn + 1)))
-            G_data += [-np.sqrt(nn)] + [-1.] * nn
-            
-        G_shape = (3 * nn * ll + mm + 2 * ll + 2, mm + ll * (nn + 1) + 1)
-        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
         
+        G_shape = (ll * nn + mm + ll * (nn + 1) + 2, mm + ll * (nn + 1) + 1)
+        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
+     
         # build h
-        h_data = [0.] * (3 * nn * ll + mm + 2 * ll + 2)
-        
-        # build dims
-        dims = {'l': (2 * ll * nn + mm + ll + 2), 'q': [nn + 1] * ll}
+        h_data = [0.] * (nn * ll + mm + ll * (nn + 1) + 2)
         
-        # build A
+        #build A
         A_icol = list(range(mm)) + [mm + ll * (nn + 1)]
-        A_irow = [0] * (mm + 1) 
-        A_data = [1.] * mm + [-1.] 
+        A_irow = [0] * (mm + 1)
+        A_data = [1.] * mm + [-1.]
         
-        A_icol += list(range(mm))
+        A_icol += list(range(mm)) 
         A_irow += [1] * mm
-        A_data += list(self.risk_comp)
- 
+        A_data += list(self.risk_comp) 
+        
         A_shape = (2, mm + ll * (nn + 1) + 1)
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
- 
-        # bjuild b
+     
+        # build b
         b_data = [0., 1.]
-        
+
         # calc
         toc = time.perf_counter()
-        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
+        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
         self.time_level2 = time.perf_counter() - toc
- 
+       
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-        
-        # mLSD-Divers
-        self.diverse= 1. - res['pcost']
-        # mLSD
+
         t = res['x'][-1]
+        # mCVaR (g/t)
         self.risk = res['pcost'] / t
-        # delta-risk values
-        self.primary_risk_comp = np.array(
-            [res['x'][mm + l * (nn + 1)] / t for l in range(ll)])
-        
+        # VaR (u)
+        self.secondary_risk_comp = \
+            np.array([res['x'][mm + l * (nn + 1)] / t for l in range(ll)])
+        # Diversification
+        self.diverse = 1. - res['pcost']
         # optimal weights
         self.ww = np.array(res['x'][:mm] / t)
         self.ww.shape = mm
         # rate of return
         self.RR = np.dot(self.ww, self.muk)
-        # delta-risk strikes
-        self.secondary_risk_comp = \
-            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
+        # component CVaR (recomputed)
+        self.primary_risk_comp = \
+            np.array([(res['x'][mm + l * (nn + 1)] + 1 / (1 - self.alpha[l]) \
+            * np.mean(res['x'][(mm + l * (nn + 1) + 1) :\
+                            (mm + (l + 1) * (nn + 1))])) /t \
+            for l in range(ll)])
         
         return self.ww
     
     
     def _risk_inv_diversification(self, d=1):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
-        # u_l <- mm + l(nn+1), 
-        # s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
+        #   u_l <- mm + l(nn+1), 
+        #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # and last t <- [mm + ll(nn + 1)]
         # in total dim = mm + ll(nn + 1) + 1
         ll = self.ll
         nn = self.nn
         mm = self.mm
         
-        # build c
+        # build c   
         c_data = list(-self.risk_comp) + [0.] * (ll * (nn + 1) + 1)
         
         # build G
-        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
-                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
-                       for _ in range(l)]\
-                  + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1.] * ((l + 1) * nn)
+            G_icol += [mm + l * (nn + 1)] * nn \
+                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += list(range(l * nn, (l + 1) * nn)) \
+                + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1.] * nn + [-1.] * nn
+            
             
         G_icol += list(range(mm)) + [mm + ll * (nn + 1)]
-        G_irow += [nn * ll] * (mm + 1)
+        G_irow += [ll * nn] * (mm + 1)
         G_data += list(-self.muk * d) + [self.mu * d]
-
+            
         G_icol += list(range(mm + ll * (nn + 1) + 1))
-        G_irow += list(range(nn * ll + 1, mm + 2 * nn * ll + ll + 2))
+        G_irow += list(range(ll * nn + 1, ll * nn + mm + ll * (nn + 1) + 2))
         G_data += [-1.] * (mm + ll * (nn + 1) + 1)
-        # cone
-        for l in range(ll):
-            G_icol += list(range((nn + 1) * l + mm , 
-                                 (nn + 1) * l + mm + 1 + nn))
-            G_irow += list(range(mm + 2 * nn * ll + ll + 2 + l * (nn + 1), 
-                           mm + 2 * nn * ll + ll + 2 + (l + 1) * (nn + 1)))
-            G_data += [-np.sqrt(nn)] + [-1.] * nn
-            
-        G_shape = (3 * nn * ll + mm + 2 * ll + 2, mm + ll * (nn + 1) + 1)
-        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
         
+        G_shape = (ll * nn + mm + ll * (nn + 1) + 2, mm + ll * (nn + 1) + 1)
+        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
+     
         # build h
-        h_data = [0.] * (3 * nn * ll + mm + 2 * ll + 2)
-        
-        # build dims
-        dims = {'l': (2 * ll * nn + mm + ll + 2), 'q': [nn + 1] * ll}
+        h_data = [0.] * (nn * ll + mm + ll * (nn + 1) + 2)
         
-        # build A
+        #build A
         A_icol = list(range(mm)) + [mm + ll * (nn + 1)]
-        A_irow = [0] * (mm + 1) 
-        A_data = [1.] * mm + [-1.] 
+        A_irow = [0] * (mm + 1)
+        A_data = [1.] * mm + [-1.]
+        
+        A_icol += list(range(mm, mm + ll * (nn + 1))) 
+        A_irow += [1] * (ll * (nn + 1))
+        for l in range(ll):
+            A_data += [self.coef[l]] \
+                    + [self.coef[l] / (1 - self.alpha[l]) / nn] * nn
         
-        A_icol += [mm + l * (nn + 1) for l in range(ll)]
-        A_irow += [1] * ll
-        A_data += list(self.coef)
- 
         A_shape = (2, mm + ll * (nn + 1) + 1)
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
- 
-        # bjuild b
+     
+        # build b
         b_data = [0., 1.]
         
         # calc
         toc = time.perf_counter()
-        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
+        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
         self.time_level2 = time.perf_counter() - toc
- 
+       
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-        
-        t = res['x'][-1] 
-        # mLSD-Divers
-        self.diverse= 1. + 1. / res['pcost']
-        # mLSD
+
+        t = res['x'][-1]
+        # mCVaR (1/t)
         self.risk = 1. / t
-        # delta-risk values
-        self.primary_risk_comp = np.array(
-            [res['x'][mm + l * (nn + 1)] / t for l in range(ll)])
+        # VaR (u)
+        self.secondary_risk_comp = \
+            np.array([res['x'][mm + l * (nn + 1)] / t for l in range(ll)])
+        # Diversification
+        self.diverse = 1. + 1. / res['pcost']
         # optimal weights
-        self.ww = np.array(res['x'][:mm] / t)
+        self.ww = np.array(res['x'][:mm]) / t
         self.ww.shape = mm
         # rate of return
         self.RR = np.dot(self.ww, self.muk)
-        # delta-risk strikes
-        self.secondary_risk_comp = \
-            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
+        # component CVaR (recomputed)
+        self.primary_risk_comp = \
+            np.array([(res['x'][mm + l * (nn + 1)] + 1 / (1 - self.alpha[l]) \
+            * np.mean(res['x'][(mm + l * (nn + 1) + 1) :\
+                            (mm + (l + 1) * (nn + 1))])) /t \
+            for l in range(ll)])
         
         return self.ww
         
-    
+        
     def _rr_max_diversification(self):
         # Order of variables:
         # w <- [0:mm] 
         # then for l <- [0:ll]
         #   u_l <- mm + l(nn+1), 
         #   s_l <- [mm + l(nn + 1) + 1: mm + (l + 1)(nn + 1)]
         # in total dim = mm + ll(nn + 1)
+        ll = self.ll
         nn = self.nn
         mm = self.mm
-        ll = self.ll 
-        
+    
         # build c
-        c_data = list(-self.muk) + [0.] * (ll * (nn + 1))
-        
+        c_data = list(-self.muk) + [0.] * ((nn + 1) * ll)
+            
         # build G
-        # linear
         G_icol = list(range(mm)) * (nn * ll)
         G_irow = [k  for k in range(nn * ll) for _ in range(mm)]
         G_data = list(np.ravel(-self.rrate)) * ll
         for l in range(ll):
-            G_icol += [mm + k * (nn + 1) for k in range(l)] * nn \
-                  + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
-            G_irow += [k for k in range(l * nn, (l + 1) * nn) \
-                       for _ in range(l)] \
-                  + list(range(l * nn, (l + 1) * nn))
-            G_data += [-1.] * ((l + 1) * nn)
-
+            G_icol += [mm + l * (nn + 1)] * nn \
+                + list(range(mm + l * (nn + 1) + 1, mm + (l + 1) * (nn + 1)))
+            G_irow += list(range(l * nn, (l + 1) * nn)) \
+                + list(range(l * nn, (l + 1) * nn))
+            G_data += [-1.] * nn + [-1.] * nn
+            
         G_icol += list(range(mm + ll * (nn + 1)))
-        G_irow += list(range(nn * ll, mm + 2 * nn * ll + ll))
+        G_irow += list(range(ll * nn, ll * nn + mm + ll * (nn + 1)))
         G_data += [-1.] * (mm + ll * (nn + 1))
-        # cone
-        for l in range(ll):
-            G_icol += list(range((nn + 1) * l + mm , 
-                                 (nn + 1) * l + mm + 1 + nn))
-            G_irow += list(range(mm + 2 * nn * ll + ll + l * (nn + 1), 
-                                 mm + 2 * nn * ll + ll + (l + 1) * (nn + 1)))
-            G_data += [-np.sqrt(nn)] + [-1.] * nn
-            
-        G_shape = (3 * nn * ll + mm + 2 * ll, mm + ll * (nn + 1))
-        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
         
+        G_shape = (nn * ll + mm + (nn + 1) * ll, mm + (nn + 1) * ll )
+        G = sps.coo_matrix((G_data, (G_irow, G_icol)), G_shape)
+
         # build h
-        h_data = [0.] * (3 * nn * ll + mm + 2 * ll)
-        
-        # build dims
-        dims = {'l': (2 * ll * nn + mm + ll), 'q': [nn + 1] * ll}
+        h_data = [0.] * (nn * ll + mm + (nn + 1) * ll)
         
         # build A
-        A_icol = list(range(mm)) + [mm + l * (nn + 1) for l in range(ll)] + list(range(mm))
-        A_irow = [0] * mm + [1] * (ll + mm)
-        A_data = [1.] * mm + list(self.coef) + list((self.diverse- 1) * self.risk_comp)
+        A_icol = list(range(mm + (nn + 1) * ll)) + list(range(mm))
+        A_irow = [0] * mm + [1] * ((nn + 1) * ll + mm)
+        A_data = [1.] * mm
+        for l in range(ll):
+            A_data += [self.coef[l]] \
+                  + [self.coef[l] / (1 - self.alpha[l]) / nn] * nn
+        A_data += list((self.diverse - 1) * self.risk_comp)
         
-        A_shape = (2, mm + ll * (nn + 1))
+        A_shape = (2, mm + (nn + 1) * ll)
         A = sps.coo_matrix((A_data, (A_irow, A_icol)), A_shape)
-        
+   
         # build b
         b_data = [1., 0.]
         
         # calc
         toc = time.perf_counter()
-        res = _socp_solver(self.method, c_data, G, h_data, dims, A, b_data)
+        res = _lp_solver(self.method, c_data, G, h_data, A, b_data)
         self.time_level2 = time.perf_counter() - toc
- 
+       
         self.status = res['status']
         if self.status != 0:
             warnings.warn(f"Warning {self.name} on {self.rrate.index[-1]} :: "
                           f"status {res['status']} :: {res['infostring']}")
             return np.array([np.nan] * mm)
-        
-        # rate of return
-        self.RR = -res['pcost']
-        # delta-risk values
-        self.primary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
-                                           for l in range(ll)])
-        # risk
+
+        # VaR (u)
+        self.secondary_risk_comp = np.array([res['x'][mm + l * (nn + 1)] \
+                                    for l in range(ll)])
+        # CVaR (recomputed)
+        self.primary_risk_comp = \
+            np.array([res['x'][mm + l * (nn + 1)] \
+             + 1 / (1 - self.alpha[l]) * np.mean(
+                 res['x'][(mm + l * (nn + 1) + 1) : (mm + (l + 1) * (nn + 1))])
+             for l in range(ll)])
+        # mCVaR
         self.risk = np.dot(self.primary_risk_comp, self.coef)
-        # delta-risk strikes
-        self.secondary_risk_comp = \
-            np.cumsum(np.insert(self.primary_risk_comp, 0, 0))[:-1]
         # optimal weights
         self.ww = np.array(res['x'][:mm])
         self.ww.shape = mm
+        # rate of return
+        self.RR = -res['pcost']
         # diversification
-        self.diverse= 1 - self.risk / np.dot(self.ww, self.risk_comp)
-
-        return self.ww
+        self.diverse = 1 - self.risk / np.dot(self.ww, self.risk_comp)
+        
+        return self.ww
```

### Comparing `azapy-1.1.1/azapy/PortOpt/MADAnalyzer.py` & `azapy-1.2.0/azapy/Analyzers/MADAnalyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,94 +4,132 @@
 import time
 
 from ._RiskAnalyzer import _RiskAnalyzer
 from ._solvers import _lp_solver
 
 class MADAnalyzer(_RiskAnalyzer):
     """
-    m-level MAD based optimal portfolio strategies.
+    m-level MAD (Mean Absolute Deviation)
+    based optimal portfolio strategies.
 
-    Methods:
-        * getWeights
-        * getRisk
-        * getPositions
-        * getRiskComp
-        * getDiversification
-        * viewForntiers
-        * set_rrate
-        * set_mktdata
-        * set_rtype
-        * set_random_seed
+    **Attributes**
+        * `status` : `int` - the computation status (`0` - success, 
+          any other value signifies an error)
+        * `ww` : `pandas.Series` -  the portfolio weights 
+        * `RR` : `float` - portfolio rate of return
+        * `risk` : `float` - portfolio mMAD risk
+        * `primary_risk_comp` : `list` - delta-risk components of 
+          portfolio mMAD
+        * `secondary_risk_comp` : `list` - cumulative delta-risk components 
+          of mMAD 
+        * `sharpe` : `float` - mMAD-Sharpe ration if `rtype` is set to 
+          `'Shapre'` or `'Sharpe2'` otherwise `None`. 
+        * `diverse` : `float` - diversification factor if `rtype` is set 
+          to `'Divers'` or `'MaxDivers'` otherwise `None`.
+        * `name` : `str` - portfolio name
+        
+    Note the following 2 important methods:
+        * `getWeights` : Computes the optimal portfolio weights.
+          During its computations the following class members are also set:
+          `risk`, `primery_risk_comp`, `secondary_risk_comp`, `sharpe`,  `RR`, 
+          `divers`.
+        * `getPositions` : Provides practical information regarding the portfolio
+          rebalancing delta positions and costs.  
     """
     def __init__(self, coef=[1.], mktdata=None, colname='adjusted', freq='Q',
-                 hlength=3.25, calendar=None, rtype='Sharpe', method='ecos',
-                 name='MAD'):
+                 hlength=3.25, name='MAD', rtype='Sharpe', mu=None, d=1, 
+                 mu0=0., aversion=None, ww0=None, method='ecos'):
         """
         Constructor
 
         Parameters
         ----------
-        `coef` : `list`, optional;
+        coef : `list`, optional
             Positive non-increasing list of mixture coefficients. 
             The default is `[1.]`.
-        `mktdata` : `pandas.DataFrame`, optional;
+        mktdata : `pandas.DataFrame`, optional
             Historic daily market data for portfolio components in the format
             returned by `azapy.mktData` function. The default is `None`.
-        `colname` : `str`, optional;
-            Name of the price column from mktdata used in the weights 
+        colname : `str`, optional
+            Name of the price column from mktdata used in the weight's 
             calibration. The default is `'adjusted'`.
-        `freq` : `str`, optional;
+        freq : `str`, optional
             Rate of return horizon. It could be 
-            `'Q'` for quarter or `'M'` for month. The default is `'Q'`.
-        `hlength` : `float`, optional;
+            `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
             History length in number of years used for calibration. A 
             fractional number will be rounded to an integer number of months.
             The default is `3.25` years.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will 
-            be set to NYSE business calendar. 
-            The default is `None`.
-        `rtype` : `str`, optional;
+        name : `str`, optional
+            Portfolio name. The default is `'MAD'`.
+        rtype : `str`, optional
             Optimization type. Possible values: \n
-                `'Risk'` : optimal-risk portfolio for targeted expected rate of 
+                `'Risk'` : optimal risk portfolio for targeted expected rate of 
                 return.\n
-                `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
-                `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
+                `'Sharpe'` : optimal Sharpe portfolio - maximization solution.\n
+                `'Sharpe2'` : optimal Sharpe portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
-                `'RiskAverse'` : optimal-risk portfolio for a fixed 
+                `'RiskAverse'` : optimal risk portfolio for a fixed 
                 risk-aversion factor.\n
-                `'InvNrisk'` : optimal-risk portfolio with the same risk value 
+                `'InvNrisk'` : optimal risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
-                `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
-                `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                `'Diverse'` : optimal diversified portfolio for targeted
+                expected rate of return (max of inverse 1-Diverse).\n
+                `'Diverse2'` : optimal diversified portfolio for targeted
+                expected rate of return (min of 1-Diverse).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
-                `'InvNdiverse'` : optimal-diversified portfolio with the same
+                `'InvNdiverse'` : optimal diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
-                `'InvNdrr'` : optima- diversified portfolio with the same 
+                `'InvNdrr'` : optimal diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `method` : `str`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
+            Targeted portfolio expected rate of return. 
+            Relevant only if `rtype='Risk'` or `rtype='Divers'`.
+            The default is `None`.
+        d : `int`, optional
+            Frontier type. Active only if `rtype='Risk'`. A value of `1` will
+            trigger the evaluation of optimal portfolio along the efficient
+            frontier. Otherwise, it will find the portfolio with the lowest
+            rate of return along the inefficient portfolio frontier.
+            The default is `1`.
+        mu0 : `float`, optional
+            Risk-free rate accessible to the investor.
+            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            The default is `0`.
+        aversion : `float`, optional
+            The value of the risk-aversion coefficient.
+            Must be positive. Relevant only if `rtype='RiskAverse'`.
+            The default is `None`.
+        ww0 : `list`, `numpy.array` or `pandas.Series`, optional
+            Targeted portfolio weights. 
+            Relevant only if `rype='InvNrisk'`.
+            Its length must be equal to the number of symbols in `rrate` 
+            (mktdata). All weights must be >= 0 with sum > 0.
+            If it is a `list` or a `numpy.array` then the weights are assumed 
+            to be in order of `rrate.columns`. If it is a `pandas.Series` then 
+            the index should be compatible with the `rrate.columns` or mktdata 
+            symbols (same symbols, not necessarily in the same order).
+            If it is `None` then it will be set to equal weights.
+            The default is `None`.
+        method : `str`, optional
             Linear programming numerical method. 
             Could be: `'ecos'`, `'highs-ds'`, `'highs-ipm'`, `'highs'`, 
             `'interior-point'`, `'glpk'` and `'cvxopt'`.
             The default is `'ecos'`.
-        `name` : `str`, optional;
-            Object name. The default is `'MAD'`.
-
+        
         Returns
         -------
         The object.
         """
-        super().__init__(mktdata, colname, freq, hlength, calendar, 
-                         rtype, name)
+        super().__init__(mktdata, colname, freq, hlength, name,
+                         rtype, mu, d, mu0, aversion, ww0)
 
         self._set_method(method)
 
         self.coef = np.array(coef)
         if any(self.coef <= 0.):
             raise ValueError("All coef must be positive")
         if any(i < j for i, j in zip(self.coef, self.coef[1:])):
@@ -107,35 +145,34 @@
         
     def _set_method(self, method):
         self._set_lp_method(method)
 
 
     def getRisk(self, ww, rrate=None):
         """
-        Returns the value of MAD for a give portfolio.
+        Returns the value of MAD for a given portfolio.
 
         Parameters
         ----------
-        `ww` : `list` (`numpy.array` or `pandas.Series`)
+        ww : `list` (`numpy.array` or `pandas.Series`)
             Portfolio weights.
-        `rrate` : `pandas.series`, optional
-            The portfolio components historical rates of returns.
-            If it is not `None`, it will overwrite the rrate computed in the
-            constructor from mktdata. The default is `None`.
+        rrate : `pandas.series`, optional
+            The portfolio components historical rates of return.
+            If it is not `None`, it will overwrite the rates of return 
+            computed in the constructor from mktdata. 
+            The default is `None`.
 
         Returns
         -------
         float :
         The value of mMAD
         """
         self._reset_output()
         toc = time.perf_counter()
-        
-        if rrate is not None:
-            self.set_rrate(rrate)
+        self.set_rrate(rrate)
 
         w = np.array(ww)
         if any(w < 0.):
             raise ValueError("All ww must be non negative")
         w = w / w.sum()
 
         prate = np.dot(self.rrate, w)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/MVAnalyzer.py` & `azapy-1.2.0/azapy/Analyzers/MVAnalyzer.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,90 +6,126 @@
 
 from ._RiskAnalyzer import _RiskAnalyzer
 from ._solvers import _socp_solver, _qp_solver, _tol_cholesky
 
 
 class MVAnalyzer(_RiskAnalyzer):
     """
-    MV (mean-variance) - Variance based optimal portfolio strategies.
+    MV (Mean-Variance) - Variance based optimal portfolio strategies.
     
-    Methods:
-        * getWeights
-        * getRisk
-        * getPositions
-        * getRiskComp
-        * getDiversification
-        * viewForntiers
-        * set_rrate
-        * set_mktdata
-        * set_rtype
-        * set_random_seed
+    **Attributes**
+        * `status` : `int` - the computation status (`0` - success, 
+          any other value signifies an error)
+        * `ww` : `pandas.Series` -  the portfolio weights 
+        * `RR` : `float` - portfolio rate of return
+        * `risk` : `float` - portfolio MV risk
+        * `primary_risk_comp` : `list` - redundant (single element list 
+          containig MV risk value)
+        * `secondary_risk_comp` : `list` - redundant 
+          (same as `primary_risk_comp`)
+        * `sharpe` : `float` - MV-Sharpe ration if `rtype` is set to 
+          `'Shapre'` or `'Sharpe2'` otherwise `None`. 
+        * `diverse` : `float` - diversification factor if `rtype` is set 
+          to `'Divers'` or `'MaxDivers'` otherwise `None`.
+        * `name` : `str` - portfolio name
+        
+    Note the following 2 important methods:
+        * `getWeights` : Computes the optimal portfolio weights.
+          During its computations the following class members are also set:
+          `risk`, `primery_risk_comp`, `secondary_risk_comp`, `sharpe`,  `RR`, 
+          `divers`.
+        * `getPositions` : Provides practical information regarding the 
+          portfolio rebalancing delta positions and costs.  
     """
     def __init__(self, mktdata=None, colname='adjusted', freq='Q', 
-                 hlength=3.25, calendar=None, rtype='Sharpe', method = 'ecos',
-                 name='MV'):
+                 hlength=3.25, name='MV', rtype='Sharpe', mu=None,  
+                 d=1, mu0=0, aversion=None, ww0=None, method='ecos'):
         """
         Constructor
 
         Parameters
         ----------
-       `mktdata` : `pandas.DataFrame`, optional;
+        mktdata : `pandas.DataFrame`, optional
            Historic daily market data for portfolio components in the format
            returned by `azapy.mktData` function. The default is `None`.
-       `colname` : `str`, optional;
-           Name of the price column from mktdata used in the weights 
+        colname : `str`, optional
+           Name of the price column from mktdata used in the weight's 
            calibration. The default is `'adjusted'`.
-       `freq` : `str`, optional;
+        freq : `str`, optional
            Rate of return horizon. It could be 
-           `'Q'` for quarter or `'M'` for month. The default is `'Q'`.
-       `hlength` : `float`, optional;
+           `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
            History length in number of years used for calibration. A 
            fractional number will be rounded to an integer number of months.
            The default is `3.25` years.
-       `calendar` : `numpy.busdaycalendar`, optional;
-           Business days calendar. If is it `None` then the calendar will 
-           be set to NYSE business calendar. 
-           The default is `None`.
-       `rtype` : `str`, optional;
+        name : `str`, optional
+           Portfolio name. The default is `'MV'`.
+        rtype : `str`, optional
            Optimization type. Possible values: \n
-               `'Risk'` : optimal-risk portfolio for targeted expected rate of 
+               `'Risk'` : optimal risk portfolio for targeted expected rate of 
                return.\n
-               `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
-               `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
+               `'Sharpe'` : optimal Sharpe portfolio - maximization solution.\n
+               `'Sharpe2'` : optimal Sharpe portfolio - minimization solution.\n
                `'MinRisk'` : minimum risk portfolio.\n
-               `'RiskAverse'` : optimal-risk portfolio for a fixed 
+               `'RiskAverse'` : optimal risk portfolio for a fixed 
                risk-aversion factor.\n
-               `'InvNrisk'` : optimal-risk portfolio with the same risk value 
+               `'InvNrisk'` : optimal risk portfolio with the same risk value 
                as a benchmark portfolio (e.g., same as equal weighted 
                portfolio).\n
-               `'Diverse'` : optimal-diversified portfolio for targeted
-               expected rate of return (maximum of inverse 1-D).\n
-               `'Diverse2'` : optimal-diversified portfolio for targeted
-               expected rate of return (minmum of 1-D).\n
+               `'Diverse'` : optimal diversified portfolio for targeted
+               expected rate of return (max of inverse 1-Diverse).\n
+               `'Diverse2'` : optimal diversified portfolio for targeted
+               expected rate of return (min of 1-Diverse).\n
                `'MaxDiverse'` : maximum diversified portfolio.\n
-               `'InvNdiverse'` : optimal-diversified portfolio with the same
+               `'InvNdiverse'` : optimal diversified portfolio with the same
                diversification factor as a benchmark portfolio 
                (e.g., same as equal weighted portfolio).\n
-               `'InvNdrr'` : optima- diversified portfolio with the same 
+               `'InvNdrr'` : optimal diversified portfolio with the same 
                expected rate of return as a benchmark portfolio
                (e.g., same as equal weighted portfolio).\n
-           The defauls is `'Sharpe'`.
-        `method` : `str`, optional;
+           The default is `'Sharpe'`.
+        mu : `float`, optional
+           Targeted portfolio expected rate of return. 
+           Relevant only if `rtype='Risk'` or `rtype='Divers'`.
+           The default is `None`.
+        d : `int`, optional
+           Frontier type. Active only if `rtype='Risk'`. A value of `1` will
+           trigger the evaluation of optimal portfolio along the efficient
+           frontier. Otherwise, it will find the portfolio with the lowest
+           rate of return along the inefficient portfolio frontier.
+           The default is `1`.
+        mu0 : `float`, optional
+           Risk-free rate accessible to the investor.
+           Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+           The default is `0`.
+        aversion : `float`, optional
+           The value of the risk-aversion coefficient.
+           Must be positive. Relevant only if `rtype='RiskAverse'`.
+           The default is `None`.
+        ww0 : `list`, `numpy.array` or `pandas.Series`, optional
+           Targeted portfolio weights. 
+           Relevant only if `rype='InvNrisk'`.
+           Its length must be equal to the number of symbols in `rrate` 
+           (mktdata). All weights must be >= 0 with sum > 0.
+           If it is a `list` or a `numpy.array` then the weights are assumed 
+           to be in order of `rrate.columns`. If it is a `pandas.Series` then 
+           the index should be compatible with the `rrate.columns` or mktdata 
+           symbols (same symbols, not necessarily in the same order).
+           If it is `None` then it will be set to equal weights.
+           The default is `None`.
+        method : `str`, optional
             Quadratic programming numerical method. Could be `'ecos'` or
-            'cvxopt'. The default is `'ecos'`.
-        `name` : `str`, optional;
-            Object name. The default is `'MV'`.
-            
+            `'cvxopt'`. The default is `'ecos'`.
+        
         Returns
         -------
         The object.
         """
-        super().__init__(mktdata, colname, freq, hlength, calendar, 
-                         rtype, name)
-        
+        super().__init__(mktdata, colname, freq, hlength, name,
+                         rtype, mu, d, mu0, aversion, ww0)
         self._set_method(method)
         
         
     def _set_method(self, method):
         self._set_qp_method(method)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_BTAD.py` & `azapy-1.2.0/azapy/PortOpt/Port_CVaR.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,118 +1,108 @@
-from .Port_CVaR import Port_CVaR
-from .BTADAnalyzer import BTADAnalyzer
+from ._Port_Generator import _Port_Generator
+from azapy.Generators.ModelPipeline import ModelPipeline
+from azapy.Analyzers.CVaRAnalyzer import CVaRAnalyzer
 
-class Port_BTAD(Port_CVaR):
-    """
-    Backtesting mBTAD optimal portfolio strategies, periodically rebalanced.
 
-    Methods:
-        * set_model
-        * get_port
-        * get_nshares
-        * get_weights
-        * get_account
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-        * port_period_returns
+class Port_CVaR(_Port_Generator):
     """
-    def set_model(self, alpha=[0.], coef=None, rtype='Sharpe', 
-                  mu=None, mu0=0., aversion=None, ww0=None,
-                  detrended=False, hlength=3.25, method='ecos', 
-                  verbose=False):
+    Backtesting CVaR (Conditional Value at Risk) portfolio periodically 
+    rebalanced.
+    
+    **Attributes**
+        * `pname` : `str` - portfolio name
+        * `ww` : `pandasDataFrame` - portfolio weights at each rebalancing date
+        * `port` : `pandas.Series` - portfolio historical time-series
+        * `schedule` : `pandas.DataFrame` - rebalancing schedule
+       
+    The most important method is `set_model`. It must be called before any
+    other method.
+    """        
+    def set_model(self, alpha=[0.975], coef=None, rtype='Sharpe',
+                  mu=None, mu0=0, aversion=None, ww0=None, 
+                  hlength=3.25, method='ecos', verbose=False):
         """
         Sets model parameters and evaluates portfolio time-series.
 
         Parameters
         ----------
-        `alpha` : `list`, optional;
-            List of thresholds. The default is `[0.]`.
-        `coef` : `list`, optional;
+        alpha : `list`, optional
+            List of alpha confidence levels. The default is `[0.975]`.
+        coef : `list`, optional
             List of positive mixture coefficients. Note that `len(coef)`
             must be equal to `len(alpha)`. A `None` value assumes an
             equal weighted risk mixture.
             The vector of coefficients will be normalized to unit.
             The default is `None`.
-        `rtype` : `str`, optional;
+        rtype : `str`, optional
             Optimization type. Possible values: \n
                 `'Risk'` : optimal-risk portfolio for targeted expected rate of 
                 return.\n
                 `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
                 `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
                 `'RiskAverse'` : optimal-risk portfolio for a fixed 
                 risk-aversion factor.\n
                 `'InvNrisk'` : optimal-risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
                 `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
+                expected rate of return (maximum of inverse of 1-D).\n
                 `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                expected rate of return (minimum of 1-D).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
                 `'InvNdiverse'` : optimal-diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
                 `'InvNdrr'` : optima- diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `mu` : `float`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
             Targeted portfolio expected rate of return. 
             Relevant only if `rtype='Risk'`
             The default is `None`.
-        `mu0` : `float`, optional;
+        mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
-        `aversion` : `float`, optional;
+        aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
-        `ww0` : `list` (also `numpy.array` or `pandas.Series`), optional;
+        ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
             Relevant only if `rype='InvNrisk'`.
             Its length must be equal to the number of
-            symbols in rrate (mktdata). 
-            All weights must be >= 0 with sum > 0.
+            symbols in `rrate` (`mktdata`). 
+            All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
-            the index should be compatible with the `rrate.columns` or mktdata 
-            symbols (same symbols, not necessary in the same order).
+            the index should be compatible with the `rrate.columns` or `mktdata` 
+            symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        `hlength` : `float`, optional;
+        hlength : `float`, optional
             The length in year of the historical calibration period relative
             to `'Dfix'`. A fractional number will be rounded to an integer 
             number of months. The default is `3.25` years.
-        `method` : `str`, optional;
+        method : `str`, optional
             Linear programming numerical method.
             Could be: `'ecos'`, `'highs-ds'`, `'highs-ipm'`, `'highs'`,
             `'interior-point'`, `'glpk'` and `'cvxopt'`.
             The default is `'ecos'`.
-        `verbose` : Boolean, optiona;
+        verbose : Boolean, optional
             If it set to `True` then it will print messages when the optimal
             portfolio degenerates to a single asset portfolio as a limited 
             case. 
             The default is `False`.
 
-         Returns
+        Returns
         -------
-        `pandas.DataFrame`;
-            The portfolio time-series in the format 'date', 'pcolname'.
+        `pandas.DataFrame` : The portfolio time-series in the format 'date', 
+        'pcolname'.
         """
-        self.detrended = detrended
-        return super().set_model(alpha=alpha, coef=coef, rtype=rtype, 
-                                 mu=mu, mu0=mu0, aversion=aversion, ww0=ww0,
-                                 hlength=hlength, method=method,
-                                 verbose=verbose)
-
-
-    def _wwgen(self):
-        return BTADAnalyzer(self.alpha, self.coef, rtype=self.rtype,
-                            detrended=self.detrended, method=self.method,
-                            name=self.pname)
+        mod = CVaRAnalyzer(alpha=alpha, coef=coef,
+                           colname=self.col_calib, freq=self.freq,
+                           hlength=hlength, rtype=rtype, mu=mu, d=1, mu0=mu0,
+                           aversion=aversion, ww0=ww0, method=method)
+        return super().set_model(ModelPipeline([mod]), verbose)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_BTSD.py` & `azapy-1.2.0/azapy/PortOpt/Port_BTSD.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,116 +1,111 @@
-from .Port_BTAD import Port_BTAD
-from .BTSDAnalyzer import BTSDAnalyzer
+from ._Port_Generator import _Port_Generator
+from azapy.Generators.ModelPipeline import ModelPipeline
+from azapy.Analyzers.BTSDAnalyzer import BTSDAnalyzer
 
-class Port_BTSD(Port_BTAD):
-    """
-    Backtesting mBTSD optimal portfolio strategies, periodically rebalanced.
 
-    Methods:
-        * set_model
-        * get_port
-        * get_nshares
-        * get_weights
-        * get_account
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-        * port_period_returns
+class Port_BTSD(_Port_Generator):
     """
-    def set_model(self, alpha=[0.], coef=None, rtype='Sharpe', 
-                  mu=None, mu0=0, aversion=None, ww0=None,
-                  detrended=False, hlength=3.25, method='ecos',
-                  verbose=False):
+    Backtesting BTSD (Below Threshold Standard Deviation) portfolio 
+    periodically rebalanced.
+    
+    **Attributes**
+        * `pname` : `str` - portfolio name
+        * `ww` : `pandasDataFrame` - portfolio weights at each rebalancing date
+        * `port` : `pandas.Series` - portfolio historical time-series
+        * `schedule` : `pandas.DataFrame` - rebalancing schedule
+        
+    The most important method is `set_model`. It must be called before any
+    other method.
+    """    
+    def set_model(self, alpha=[0.], coef=None, rtype='Sharpe', mu=None, 
+                  mu0=0, aversion=None, ww0=None, detrended=True, 
+                  hlength=3.25, method='ecos', verbose=False):
         """
         Sets model parameters and evaluates portfolio time-series.
 
         Parameters
         ----------
-        `alpha` : `list`, optional;
+        alpha : `list`, optional
             List of thresholds. The default is `[0.]`.
-        `coef` : `list`, optional;
+        coef : `list`, optional
             List of positive mixture coefficients. Note that `len(coef)`
             must be equal to `len(alpha)`. A `None` value assumes an
             equal weighted risk mixture.
             The vector of coefficients will be normalized to unit.
             The default is `None`.
-        `rtype` : `str`, optional;
+        rtype : `str`, optional
             Optimization type. Possible values: \n
                 `'Risk'` : optimal-risk portfolio for targeted expected rate of 
                 return.\n
                 `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
                 `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
                 `'RiskAverse'` : optimal-risk portfolio for a fixed 
                 risk-aversion factor.\n
                 `'InvNrisk'` : optimal-risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
                 `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
+                expected rate of return (maximum of inverse of 1-D).\n
                 `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                expected rate of return (minimum of 1-D).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
                 `'InvNdiverse'` : optimal-diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
                 `'InvNdrr'` : optima- diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `mu` : `float`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
             Targeted portfolio expected rate of return. 
             Relevant only if `rtype='Risk'`
             The default is `None`.
-        `mu0` : `float`, optional;
+        mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
-        `aversion` : `float`, optional;
+        aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
-        `ww0` : `list` (also `numpy.array` or `pandas.Series`), optional;
+        ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
             Relevant only if `rype='InvNrisk'`.
             Its length must be equal to the number of
-            symbols in rrate (mktdata). 
-            All weights must be >= 0 with sum > 0.
+            symbols in `rrate` (`mktdata`). 
+            All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
-            the index should be compatible with the `rrate.columns` or mktdata 
-            symbols (same symbols, not necessary in the same order).
+            the index should be compatible with the `rrate.columns` or `mktdata` 
+            symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        `hlength` : `float`, optional;
+        detrendent : Boolean, optional
+            If it set to `True` then the rates of return are detrended 
+            (`mean=0`). The default value is `True`. 
+        hlength : `float`, optional
             The length in year of the historical calibration period relative
             to `'Dfix'`. A fractional number will be rounded to an integer 
             number of months. The default is `3.25` years.
-        `method` : `str`, optional;
-            SOCP numerical method.
-            Could be: `'ecos'` or `'cvxopt'`.
-            The defualt is `'ecos'`.
-        `verbose` : Boolean, optiona;
+        method : `str`, optional
+            SOCP numerical method. 
+            Could be: `'ecos'`, or `'cvxopt'`.
+            The default is `'ecos'`.
+        verbose : Boolean, optional
             If it set to `True` then it will print messages when the optimal
             portfolio degenerates to a single asset portfolio as a limited 
             case. 
             The default is `False`.
-
+            
         Returns
         -------
-        `pandas.DataFrame`;
-            The portfolio time-series in the format "date", "pcolname".
+        `pandas.DataFrame` : The portfolio time-series in the format 'date', 
+        'pcolname'.
         """
-        return super().set_model(alpha=alpha, coef=coef, rtype=rtype, mu=mu,
-                                 mu0=mu0, aversion=aversion, ww0=ww0, 
-                                 detrended=detrended, hlength=hlength, 
-                                 method=method, verbose=verbose)
- 
-    
-    def _wwgen(self):
-        return BTSDAnalyzer(self.alpha, self.coef, rtype=self.rtype,
-                            detrended=self.detrended, method=self.method,
-                            name=self.pname)
+        mod = BTSDAnalyzer(alpha=alpha, coef=coef,
+                           colname=self.col_calib, freq=self.freq,
+                           hlength=hlength, rtype=rtype, mu=mu, d=1, mu0=mu0,
+                           aversion=aversion, ww0=ww0, detrended=detrended,
+                           method=method)
+        return super().set_model(ModelPipeline([mod]), verbose)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_CVaR.py` & `azapy-1.2.0/azapy/PortOpt/Port_EVaR.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,147 +1,110 @@
-from .CVaRAnalyzer import CVaRAnalyzer
-from .Port_InvVol import Port_InvVol
+from ._Port_Generator import _Port_Generator
+from azapy.Generators.ModelPipeline import ModelPipeline
+from azapy.Analyzers.EVaRAnalyzer import EVaRAnalyzer
 
 
-class Port_CVaR(Port_InvVol):
+class Port_EVaR(_Port_Generator):
     """
-    Backtesting mCVaR optimal portfolio strategies, periodically rebalanced.
-
-    Methods:
-        * set_model
-        * get_port
-        * get_nshares
-        * get_weights
-        * get_account
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-        * port_period_returns
-    """
-
-    def set_model(self, alpha=[0.975], coef=None, rtype='Sharpe',
+    Backtesting EVaR (Entropic Value at Risk) portfolio periodically 
+    rebalanced.
+    
+    **Attributes**
+        * `pname` : `str` - portfolio name
+        * `ww` : `pandasDataFrame` - portfolio weights at each rebalancing date
+        * `port` : `pandas.Series` - portfolio historical time-series
+        * `schedule` : `pandas.DataFrame` - rebalancing schedule
+       
+    The most important method is `set_model`. It must be called before any
+    other method.
+    """            
+    def set_model(self, alpha=[0.65], coef=None, rtype='Sharpe',
                   mu=None, mu0=0, aversion=None, ww0=None, 
-                  hlength=3.25, method='ecos', verbose=False):
+                  hlength=3.25, method='ncp', verbose=False):
         """
         Sets model parameters and evaluates portfolio time-series.
 
         Parameters
         ----------
-        `alpha` : `list`, optional;
-            List of alpha confidence levels. The default is `[0.975]`.
-        `coef` : `list`, optional;
+        alpha : `list`, optional
+            List of alpha confidence levels. The default is `[0.65]`.
+        coef : `list`, optional
             List of positive mixture coefficients. Note that `len(coef)`
             must be equal to `len(alpha)`. A `None` value assumes an
             equal weighted risk mixture.
             The vector of coefficients will be normalized to unit.
             The default is `None`.
-        `rtype` : `str`, optional;
+        rtype : `str`, optional
             Optimization type. Possible values: \n
                 `'Risk'` : optimal-risk portfolio for targeted expected rate of 
                 return.\n
                 `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
                 `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
                 `'RiskAverse'` : optimal-risk portfolio for a fixed 
                 risk-aversion factor.\n
                 `'InvNrisk'` : optimal-risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
                 `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
+                expected rate of return (maximum of inverse of 1-D).\n
                 `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                expected rate of return (minimum of 1-D).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
                 `'InvNdiverse'` : optimal-diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
                 `'InvNdrr'` : optima- diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `mu` : `float`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
             Targeted portfolio expected rate of return. 
             Relevant only if `rtype='Risk'`
             The default is `None`.
-        `mu0` : `float`, optional;
+        mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
-        `aversion` : `float`, optional;
+        aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
-        `ww0` : `list` (also `numpy.array` or `pandas.Series`), optional;
+        ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
             Relevant only if `rype='InvNrisk'`.
             Its length must be equal to the number of
-            symbols in rrate (mktdata). 
-            All weights must be >= 0 with sum > 0.
+            symbols in `rrate` (`mktdata`). 
+            All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
-            the index should be compatible with the `rrate.columns` or mktdata 
-            symbols (same symbols, not necessary in the same order).
+            the index should be compatible with the `rrate.columns` or `mktdata` 
+            symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        `hlength` : `float`, optional;
+        hlength : `float`, optional
             The length in year of the historical calibration period relative
             to `'Dfix'`. A fractional number will be rounded to an integer 
             number of months. The default is `3.25` years.
-        `method` : `str`, optional;
-            Linear programming numerical method.
-            Could be: `'ecos'`, `'highs-ds'`, `'highs-ipm'`, `'highs'`,
-            `'interior-point'`, `'glpk'` and `'cvxopt'`.
-            The default is `'ecos'`.
-        `verbose` : Boolean, optiona;
+        method : `str`, optional
+            Numerical optimization method:
+                `'ncp'` : nonlinear convex programming (using `cvxopt`).\n
+                `'ncp2'` : nonlinear convex programming (using `cvxopt`) 
+                alternative to `'ncp2'`.\n
+                `'excp'` : exponential cone programming (using `ecos`).\n
+            The default is `'ncp'`. 
+        verbose : Boolean, optional
             If it set to `True` then it will print messages when the optimal
             portfolio degenerates to a single asset portfolio as a limited 
             case. 
             The default is `False`.
 
-         Returns
+        Returns
         -------
-        `pandas.DataFrame`;
-            The portfolio time-series in the format 'date', 'pcolname'.
+        `pandas.DataFrame` : The portfolio time-series in the format 'date', 
+        'pcolname'.
         """
-        self._set_alpha(alpha, coef)
-        self._set_rtype(rtype)
-        self.mu = mu
-        self.mu0 = mu0
-        self.aversion = aversion
-        self.ww0 = ww0
-        self.hlength = hlength
-        self._set_method(method)
-        self.verbose = verbose
-
-        self._set_schedule()
-        self._set_weights()
-        self._port_calc()
-        return self.port
-
-
-    def _set_alpha(self, alpha, coef):
-        # alpha
-        self.alpha = alpha
-        self.coef = coef
-
-
-    def _set_rtype(self, rtype):
-        self.rtype = rtype
-
-
-    def _set_method(self, method):
-        self.method = method
-
-
-    def _wwgen(self):
-        return CVaRAnalyzer(self.alpha, self.coef, rtype=self.rtype,
-                            method=self.method, name=self.pname)
-
-
-    def _ww_calc(self, data):
-        return self._wwgen().getWeights(mu=self.mu, mu0=self.mu0,
-                aversion=self.aversion, ww0=self.ww0, rrate=data,
-                verbose=self.verbose)
+        mod = EVaRAnalyzer(alpha=alpha, coef=coef,
+                           colname=self.col_calib, freq=self.freq,
+                           hlength=hlength, rtype=rtype, mu=mu, d=1, mu0=mu0,
+                           aversion=aversion, ww0=ww0, method=method)
+        return super().set_model(ModelPipeline([mod]), verbose)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_ConstW.py` & `azapy-1.2.0/azapy/MkT/readMkT.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,166 +1,130 @@
-import pandas as pd
-import numpy as np
+from .MkTreader import MkTreader
 
-from .Port_Rebalanced import Port_Rebalanced
-from azapy.MkT.MkTcalendar import NYSEgen
-from azapy.util.schedule import schedule_roll
-
-class Port_ConstW(Port_Rebalanced):
+def readMkT(symbol=[], sdate="2012-01-01", edate='today', calendar=None,
+            output_format='frame', source=None, force=False, save=True,
+            file_dir="outDir", file_format='csv', api_key=None, param=None,  
+            verbose=True):
     """
-    Backtesting portfolio with constant weights, periodically rebalanced.
-
-    Methods:
-        * set_model
-        * get_port
-        * get_nshares
-        * get_weights
-        * get_account
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-        * port_period_returns
+    Retrieves market data for a set of stock symbols.\n
+    It is a wrapper for `MkTreader` class returning directly the requested
+    historical time series. The function call variables are the same as for 
+    'MkTreader' member function 'get'.
+    
+    Parameters
+    ----------
+    symbol : `str` or `list` of `str`, optional
+        Stock symbols to be uploaded.
+        The default is `[]`.
+    sdate : date like, optional
+        The start date of historical time series.
+        The default is `"2012-01-01"`.
+    edate : date like, optional
+        The end date of historical time series (must: `sdate` >= `edate`)
+        The default is `'today'`.
+    calendar : `numpy.busdaycalendar`, optional
+        Exchange business day calendar. If set to `None` it will default to 
+        the NY stock exchange business calendar (provided by the azapy 
+        function NYSEgen).
+        The default is `None`.
+    output_format : `str`, optional
+        The function output format. It can be:
+            - `'frame'` - `pandas.DataFrame`
+            - `'dict'` - `dict` of `pandaws.DataFrame`. 
+              The symbols are the keys.
+              
+        The default is `'frame'`
+    source : `str` or `dict`, optional
+        If it is a `str`, then it represents the market data provider for 
+        all historical prices request. Possible values are: `'yahoo'`, 
+        `'alphavantage'`, `'alphavantage_yahoo'`, `'eodhistoricaldata'`,
+        `'eodhistoricaldata_yahoo'` and `'marketstack'`. If set to `None` 
+        it will default to `'yahoo'`.\n
+        It can be set to a `dict` containing specific instructions for 
+        each stock symbol. 
+        The `dict` keys are the symbols and the values are 'dict'
+        instructions specific to each symbol. 
+        Valid keys for the instructions `dict` are the names of
+        this function call variables except `'sdate'`, `'edate'`, 
+        `'calendar'` and `'output_format'`. 
+        The actual set of stock symbols is given by the union 
+        of variable `'symbol'` and the keys of the dict `'source'`. Missing  
+        values in the symbol instruction dict's will be filled with the 
+        values of the function call variables. 
+        The values of the function call variables act as 
+        generic values to be used in absence of specific instructions 
+        in the `'source'` dict. The default is `None`.\n
+        *Example* of dict `'source'`: \n
+        source = {'AAPL': {'source': 'eodhistoricaldata, 'verbose': `True`},
+        'SPY': {'source': 'yahoo', 'force': `True`}}\n
+        In this case there are 2 symbols that will be added (union) to 
+        the set of symbols defined by 'symbol' variable. For symbol 'AAPL' 
+        the provider source is eodhistoricaldata and the 'verbose' 
+        instruction 
+        is set to `True`. The rest of the instructions: 'force', 'save',
+        'file_dir', 'file_format', 'api_key' and 'param' are set 
+        to the values of the corresponding function call variables.
+        Similar for symbol 'SPY'. The instructions for the rest of the 
+        symbols that may be specified in the 'symbol' variable will be
+        set according to the values of the function call variables.
+    force : Boolean, optional
+            - `True`: will try to collect historical prices exclusive from
+              the market data providers.
+            - `False`: first it will try to load the historical 
+              prices from a local saved file. If such a file does not exist
+              the market data provider will be accessed.  
+              
+        If the file exists but the saved historical 
+        data is too short then it will try to collect the missing values 
+        only from the market data provider.
+        The default is `False`.
+    save : Boolean, optional
+            - `True`: It will try to save the historical price collected from 
+              the providers to a local file.
+            - `False`: No attempt to save the data is made.
+            
+        The default is `True`.
+    file_dir : `str`, optional
+        Directory with (to save) historical market data. If it does not 
+        exists then it will be created.
+        The default is "outDir".
+    file_format : `str`, optional
+        The saved file format for the historical prices. The following 
+        files formats are supported: csv, json and feather
+        The default is 'csv'.
+    api_key : `str`, optional
+        Provider API key (where is required). If set to `None`  
+        then the API key is set to the value of global environment variables\n 
+            - `APLPHAVANTAGE_API_KEY` for alphavantage,
+            - `EODHISTORICALDATA_API_KEY` for eodhistoricaldata,
+            - `MARKETSTACK_API_KEY` for marketstack.
+        
+        The default is `None`.
+    param : `dict`, optional
+        Set of additional information to access the market data provider.  
+        At this point in time only accessing alphavantage provider requires 
+        an additional parameter specifying the maximum number of API 
+        (symbols) requested per minute. 
+        It varies with the level of access 
+        corresponding to the API key. The minimum value is 5 for a free key 
+        and starts at 75 for premium keys. This value is stored in
+        `max_req_per_min` variable.\n
+        *Example*: param = {'max_req_per_min': 5}\n
+        This is also the default vale for alphavantage, if `param` is set to 
+        `None`.
+        The default is `None`.   
+    verbose : Boolean, optional
+        If set to `True`, then additional information will be printed  
+        during the loading of historical prices.
+        The default is `True`.
+
+
+    Returns
+    -------
+    `pandas.DataFrame` or 'dict' `pandas.DataFrame` : Historical market data. 
+        The output format is designated by the value of the input parameter 
+        `output_format`.
     """
-    def __init__(self, mktdata, symb=None, sdate=None, edate=None,
-                 col_price='close', col_divd='divd', col_ref='adjusted',
-                 pname='Port', pcolname=None, capital=100000,
-                 schedule=None,
-                 freq='Q', noffset=-3, fixoffset=-1, calendar=None):
-        """
-        Constructor
-
-        Parameters
-        ----------
-        `mktdata` : `pandas.DataFrame`;
-            MkT data in the format "symbol", "date", "open", "high", "low",
-            "close", "volume", "adjusted", "divd", "split" (e.g. as returned
-            by `azapy.readMkT` function).
-        `symb` : `list`, optional;
-            List of symbols for the basket components. All symbols MkT data
-            should be included in mktdata. If set to `None` the `symb` will be
-            set to include all the symbols from `mktdata`. The default
-            is `None`.
-        `sdate` : date like, optional;
-            Start date for historical data. If set to `None` the `sdate` will
-            be set to the earliest date in mktdata. The default is `None`.
-        `edate` : date like, optional;
-            End date for historical dates and so the simulation. Must be
-            greater than  `sdate`. If it is `None` then `edat`e will be set
-            to the latest date in mktdata. The default is `None`.
-        `col_price` : `str`, optional;
-            Column name in the mktdata DataFrame that will be considered
-            for portfolio aggregation. The default is `'close'`.
-        `col_divd` :  `str`, optional;
-            Column name in the mktdata DataFrame that holds the dividend
-            information. The default is `'dvid'`.
-        `col_ref` : `str`, optional;
-            Column name in the mktdata DataFrame that will be used as a price
-            reference for portfolio components. The default is `'adjusted'`.
-        `pname` : `str`, optional;
-            The name of the portfolio. The default is `'Port'`.
-        `pcolname` : `str`, optional;
-            Name of the portfolio price column. If it set to `None` that
-            `pcolname=pname`. The default is `None`.
-        `capital` : `float`, optional;
-            Initial portfolio Capital in dollars. The default is `100000`.
-        `schedule` : `pandas.DataFrame`, optional;
-            Rebalancing schedule, with columns for `'Droll'` rolling date and
-            `'Dfix'` fixing date. If it is `None` than the schedule will be set
-            using the `freq`, `noffset`, `fixoffset` and `calendar`
-            information. The default is `None`.
-        `freq` : `str`, optional;
-            rebalancing frequency. It can be `'Q'` for quarterly or `'M'` for
-            monthly rebalancing, respectively. It is relevant only is schedule
-            is `None`. The default is `'Q'`.
-        `noffset` : `int`, optional;
-            Number of business days offset for rebalancing date `'Droll'`
-            relative to the end of the period (quart or month). A positive
-            value add business days beyond the calendar end of the period while
-            a negative value subtracts business days. It is relevant only is
-            schedule is `None`. The default is `-3`.
-        `fixoffset` : `int`, optional;
-            Number of business day offset of fixing date `'Dfix'` relative to
-            the rebalancing date `'Droll'`. It can be 0 or negative. It is
-            relevant only is schedule is `None`. The default is `-1`.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business calendar. If it is `None` then it will be set to NYSE
-            business calendar. The default
-            vale is `None`.
-
-        Returns
-        -------
-        The object.
-        """
-        super().__init__(mktdata=mktdata, symb=symb,
-                         sdate=sdate, edate=edate,
-                         col_price=col_price, col_divd=col_divd,
-                         col_ref=col_ref,
-                         pname=pname,
-                         pcolname=pcolname, capital=capital)
-        self.schedule = schedule
-        self.freq = freq
-        self.noffset = noffset
-        self.fixoffset = fixoffset
-        self.calendar =  calendar
-        if self.calendar is None: self._default_calendar()
-
-
-    def set_model(self, ww=None):
-        """
-        Set model parameters and evaluate the portfolio time-series.
-
-        Parameters
-        ----------
-        `ww` : `list` (also `numpy.array` or `pandas.Series`), optional
-
-            List of weights. If it is `pandas.Series` the index should match
-            the basket `symb`. Otherwise, the weights are considered in the 
-            `symb` order. 
-            If it is set to `None` than `ww` will be set to equal weights.
-            The default is `None`.
-
-        Returns
-        -------
-        `pands.DataFrame`
-            The portfolio time-series in the format "date", "pcolname".
-        """
-        self.hlength = 0.
-
-        self._set_schedule()
-        self._set_weights(ww)
-        self._port_calc()
-        return self.port
-
-    def _default_calendar(self):
-        self.calendar = NYSEgen()
-
-    def _set_schedule(self):
-        if self.schedule is None:
-            self.schedule = schedule_roll(self.sdate, self.edate, self.freq,
-                                          self.noffset, self.fixoffset,
-                                          self.calendar, self.hlength)
-
-    def _set_weights(self, ww):
-        if ww is None:
-            _ww = pd.Series(1., index=self.symb)
-        elif isinstance(ww, pd.core.series.Series):
-            _ww = ww
-        else:
-            _ww = pd.Series(ww, index=self.symb)
-
-        if _ww.size != self.symb.size:
-            raise ValueError(f"ww wrong size, it must be {self.symb.size}")
-
-        if np.any(_ww < 0.):
-            raise ValueError("All ww elements must be >= 0")
-
-        wws = _ww.sum()
-        if wws <= 0.:
-            raise ValueError("At least one ww element must be > 0")
-
-        self.ww = self.schedule
-        for sy in self.symb:
-            self.ww[sy] = _ww[sy] / wws
+    return MkTreader().get(symbol, sdate, edate, calendar, 
+                           output_format, source, force, save, 
+                           file_dir, file_format, api_key, param, 
+                           verbose)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_EVaR.py` & `azapy-1.2.0/azapy/PortOpt/Port_MAD.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,118 +1,103 @@
-from .Port_CVaR import Port_CVaR
-from .EVaRAnalyzer import EVaRAnalyzer
+from ._Port_Generator import _Port_Generator
+from azapy.Generators.ModelPipeline import ModelPipeline
+from azapy.Analyzers.MADAnalyzer import MADAnalyzer
 
 
-class Port_EVaR(Port_CVaR):
+class Port_MAD(_Port_Generator):
     """
-    Backtesting mEVaR optimal portfolio strategies, periodically rebalanced.
-
-    Methods:
-        * set_model
-        * get_port
-        * get_nshares
-        * get_weights
-        * get_account
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-        * port_period_returns
-    """
-
-    def set_model(self, alpha=[0.65], coef=None, rtype='Sharpe',
+    Backtesting MAD (Mean Absolute Deviation) portfolio periodically 
+    rebalanced.
+    
+    **Attributes**
+        * `pname` : `str` - portfolio name
+        * `ww` : `pandasDataFrame` - portfolio weights at each rebalancing date
+        * `port` : `pandas.Series` - portfolio historical time-series
+        * `schedule` : `pandas.DataFrame` - rebalancing schedule
+      
+    The most important method is `set_model`. It must be called before any
+    other method.
+    """                  
+    def set_model(self, coef=[1], rtype='Sharpe',
                   mu=None, mu0=0, aversion=None, ww0=None, 
-                  hlength=3.25, method='ncp', verbose=False):
+                  hlength=3.25, method='ecos', verbose=False):
         """
         Sets model parameters and evaluates portfolio time-series.
 
         Parameters
         ----------
-        `alpha` : `list`, optional;
-            List of alpha confidence levels. The default is `[0.65]`.
-        `coef` : `list`, optional;
-            List of positive mixture coefficients. Note that `len(coef)`
-            must be equal to `len(alpha)`. A `None` value assumes an
-            equal weighted risk mixture.
-            The vector of coefficients will be normalized to unit.
-            The default is `None`.
-        `rtype` : `str`, optional;
+        coef : `list`, optional
+            Positive non-increasing list of coefficients. 
+            The default is `[1.]`.
+        rtype : `str`, optional
             Optimization type. Possible values: \n
                 `'Risk'` : optimal-risk portfolio for targeted expected rate of 
                 return.\n
                 `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
                 `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
                 `'RiskAverse'` : optimal-risk portfolio for a fixed 
                 risk-aversion factor.\n
                 `'InvNrisk'` : optimal-risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
                 `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
+                expected rate of return (maximum of inverse of 1-D).\n
                 `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                expected rate of return (minimum of 1-D).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
                 `'InvNdiverse'` : optimal-diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
                 `'InvNdrr'` : optima- diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `mu` : `float`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
             Targeted portfolio expected rate of return. 
             Relevant only if `rtype='Risk'`
             The default is `None`.
-        `mu0` : `float`, optional;
+        mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
-        `aversion` : `float`, optional;
+        aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
-        `ww0` : `list` (also `numpy.array` or `pandas.Series`), optional;
+        ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
             Relevant only if `rype='InvNrisk'`.
             Its length must be equal to the number of
-            symbols in rrate (mktdata). 
-            All weights must be >= 0 with sum > 0.
+            symbols in `rrate` (`mktdata`). 
+            All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
-            the index should be compatible with the `rrate.columns` or mktdata 
-            symbols (same symbols, not necessary in the same order).
+            the index should be compatible with the `rrate.columns` or `mktdata` 
+            symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        `hlength` : `float`, optional;
+        hlength : `float`, optional
             The length in year of the historical calibration period relative
             to `'Dfix'`. A fractional number will be rounded to an integer 
             number of months. The default is `3.25` years.
-        `method` : `str`, optional
-            Numerical optimization method:
-                `'ncp'` : nonlinear convex programming (using cvxopt).\n
-                `'ncp2'` : nonlinear convex programming (using cvxopt) 
-                alternative to `'ncp2'`.\n
-                `'excp'` : exponential cone programming (using ecos).\n
-            The default is `'ncp'`. 
-        `verbose` : Boolean, optiona;
+        method : `str`, optional
+            Linear programming numerical method.
+            Could be: `'ecos'`, `'highs-ds'`, `'highs-ipm'`, `'highs'`,
+            `'interior-point'`, `'glpk'` and `'cvxopt'`.
+            The default is `'ecos'`.
+        verbose : Boolean, optional
             If it set to `True` then it will print messages when the optimal
             portfolio degenerates to a single asset portfolio as a limited 
             case. 
             The default is `False`.
 
-         Returns
+        Returns
         -------
-        `pandas.DataFrame`;
-            The portfolio time-series in the format 'date', 'pcolname'.
+        `pandas.DataFrame` : The portfolio time-series in the format 'date', 
+        'pcolname'.
         """
-        return super().set_model(alpha=alpha, coef=coef, rtype=rtype, mu=mu, 
-                                 mu0=mu0, aversion=aversion, ww0=ww0, 
-                                 hlength=hlength, method=method, 
-                                 verbose=verbose)
-    
-    def _wwgen(self):
-        return EVaRAnalyzer(alpha=self.alpha, coef=self.coef, rtype=self.rtype, 
-                            method=self.method, name=self.pname)
+        mod = MADAnalyzer(coef=coef,
+                          colname=self.col_calib, freq=self.freq,
+                          hlength=hlength, rtype=rtype, mu=mu, d=1, mu0=mu0,
+                          aversion=aversion, ww0=ww0, method=method)
+        return super().set_model(ModelPipeline([mod]), verbose)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_GINI.py` & `azapy-1.2.0/azapy/PortOpt/Port_GINI.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,105 +1,97 @@
-from .Port_CVaR import Port_CVaR
-from .GINIAnalyzer import GINIAnalyzer
+from ._Port_Generator import _Port_Generator
+from azapy.Generators.ModelPipeline import ModelPipeline
+from azapy.Analyzers.GINIAnalyzer import GINIAnalyzer
 
-class Port_GINI(Port_CVaR):
-    """
-    Backtesting GINI optimal portfolio strategies, periodically rebalanced.
 
-    Methods:
-        * set_model
-        * get_port
-        * get_nshares
-        * get_weights
-        * get_account
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-        * port_period_returns
+class Port_GINI(_Port_Generator):
     """
-    def set_model(self, rtype='Sharpe', mu=None, mu0=0, aversion=None,
-                  ww0=None, hlength=1.25, method='ecos', verbose=False):
+    Backtesting Gini portfolio periodically rebalanced.
+    
+    **Attributes**
+        * `pname` : `str` - portfolio name
+        * `ww` : `pandasDataFrame` - portfolio weights at each rebalancing date
+        * `port` : `pandas.Series` - portfolio historical time-series
+        * `schedule` : `pandas.DataFrame` - rebalancing schedule
+       
+    The most important method is `set_model`. It must be called before any
+    other method.
+    """       
+    def set_model(self, rtype='Sharpe', mu=None, mu0=0, aversion=None, 
+                  ww0=None, hlength=3.25, method='ecos', verbose=False):
         """
         Sets model parameters and evaluates portfolio time-series.
 
         Parameters
         ----------
-        `rtype` : `str`, optional;
+        rtype : `str`, optional
             Optimization type. Possible values: \n
                 `'Risk'` : optimal-risk portfolio for targeted expected rate of 
                 return.\n
                 `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
                 `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
                 `'RiskAverse'` : optimal-risk portfolio for a fixed 
                 risk-aversion factor.\n
                 `'InvNrisk'` : optimal-risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
                 `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
+                expected rate of return (maximum of inverse of 1-D).\n
                 `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                expected rate of return (minimum of 1-D).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
                 `'InvNdiverse'` : optimal-diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
                 `'InvNdrr'` : optima- diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `mu` : `float`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
             Targeted portfolio expected rate of return. 
             Relevant only if `rtype='Risk'`
             The default is `None`.
-        `mu0` : `float`, optional;
+        mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
-        `aversion` : `float`, optional;
+        aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
-        `ww0` : `list` (also `numpy.array` or `pandas.Series`), optional;
+        ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
             Relevant only if `rype='InvNrisk'`.
             Its length must be equal to the number of
-            symbols in rrate (mktdata). 
-            All weights must be >= 0 with sum > 0.
+            symbols in `rrate` (`mktdata`). 
+            All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
-            the index should be compatible with the `rrate.columns` or mktdata 
-            symbols (same symbols, not necessary in the same order).
+            the index should be compatible with the `rrate.columns` or `mktdata` 
+            symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        `hlength` : `float`, optional;
+        hlength : `float`, optional
             The length in year of the historical calibration period relative
             to `'Dfix'`. A fractional number will be rounded to an integer 
             number of months. The default is `3.25` years.
-        `method` : `str`, optional;
+        method : `str`, optional
             Linear programming numerical method.
             Could be: `'ecos'`, `'highs-ds'`, `'highs-ipm'`, `'highs'`,
             `'interior-point'`, `'glpk'` and `'cvxopt'`.
             The default is `'ecos'`.
-        `verbose` : Boolean, optiona;
+        verbose : Boolean, optional
             If it set to `True` then it will print messages when the optimal
             portfolio degenerates to a single asset portfolio as a limited 
             case. 
             The default is `False`.
 
-         Returns
+        Returns
         -------
-        `pandas.DataFrame`;
-            The portfolio time-series in the format 'date', 'pcolname'.
+        `pandas.DataFrame` : The portfolio time-series in the format 'date', 
+        'pcolname'.
         """
-        return super().set_model(rtype=rtype, mu=mu, mu0=mu0, 
-                                 aversion=aversion, ww0=ww0, hlength=hlength, 
-                                 method=method, verbose=verbose)
-
-
-    def _wwgen(self):
-        return GINIAnalyzer(rtype=self.rtype, method=self.method,
-                            name=self.pname)
+        mod = GINIAnalyzer(colname=self.col_calib, freq=self.freq,
+                           hlength=hlength, rtype=rtype, mu=mu, d=1, mu0=mu0,
+                           aversion=aversion, ww0=ww0, method=method)
+        return super().set_model(ModelPipeline([mod]), verbose)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_InvVol.py` & `azapy-1.2.0/azapy/PortOpt/Port_Rebalanced.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,150 +1,165 @@
 import numpy as np
 import pandas as pd
+from azapy.Generators.Port_Generator import Port_Generator
 
-from .Port_ConstW import Port_ConstW
 
-class Port_InvVol(Port_ConstW):
+class Port_Rebalanced(Port_Generator):
     """
-    Backtesting portfolio with weights proportional to the 
-    inverse of component volatilities, periodically rebalanced.
+    Backtesting a portfolio periodically rebalanced 
+    (with an external schedule of weights).
     
-    Methods:
-        * set_model
-        * get_port
-        * get_nshares
-        * get_weights
-        * get_account
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-        * port_period_returns
-    """
+    **Attributes**
+        * `pname` : `str` - portfolio name
+        * `ww` : `pandasDataFrame` - portfolio weights at each rebalancing date
+        * `port` : `pandas.Series` - portfolio historical time-series
+        * `schedule` : `pandas.DataFrame` - rebalancing schedule
+       
+    The most important method is `set_model`. It must be called before any
+    other method.
+    """                  
     def __init__(self, mktdata, symb=None, sdate=None, edate=None, 
                  col_price='close', col_divd='divd', col_ref='adjusted',
-                 col_calib='adjusted',
-                 pname='Port', pcolname=None, capital=100000, 
-                 schedule=None,
-                 freq='Q', noffset=-3, fixoffset=-1, calendar=None):
+                 pname='Port', pcolname=None, capital=100000, schedule=None,
+                 multitreading=True):
         """
         Constructor
     
         Parameters
         ----------
-        `mktdata` : `pandas.DataFrame`;
+        mktdata : `pandas.DataFrame`
             MkT data in the format "symbol", "date", "open", "high", "low",
-            "close", "volume", "adjusted", "divd", "split" (e.g. as returned
+            "close", "volume", "adjusted", "divd", "split" (e.g., as returned
             by `azapy.readMkT` function).
-        `symb` : `list`, optional;
+        symb : `list`, optional
             List of symbols for the basket components. All symbols MkT data
             should be included in mktdata. If set to `None` the `symb` will be
             set to include all the symbols from `mktdata`. The default
             is `None`.
-        `sdate` : date like, optional;
+        sdate : date like, optional
             Start date for historical data. If set to `None` the `sdate` will
             be set to the earliest date in mktdata. The default is `None`.
-        `edate` : date like, optional;
+        edate : date like, optional
             End date for historical dates and so the simulation. Must be
             greater than  `sdate`. If it is `None` then `edat`e will be set
             to the latest date in mktdata. The default is `None`.
-        `col_price` : `str`, optional;
+        col_price : `str`, optional
             Column name in the mktdata DataFrame that will be considered
             for portfolio aggregation. The default is `'close'`.
-        `col_divd` :  `str`, optional;
+        col_divd :  `str`, optional
             Column name in the mktdata DataFrame that holds the dividend
             information. The default is `'dvid'`.
-        `col_ref` : `str`, optional;
+        col_ref : `str`, optional
             Column name in the mktdata DataFrame that will be used as a price
             reference for portfolio components. The default is `'adjusted'`.
-        `col_calib` : `str`, optional;
-            Column name used for historical weights calibrations. 
-            The default is `'adjusted'`.
-        `pname` : `str`, optional;
+        pname : `str`, optional
             The name of the portfolio. The default is `'Port'`.
-        `pcolname` : `str`, optional;
-            Name of the portfolio price column. If it set to `None` that
+        pcolname : `str`, optional
+            Name of the portfolio price column. If it set to `None` then
             `pcolname=pname`. The default is `None`.
-        `capital` : `float`, optional;
+        capital : `float`, optional
             Initial portfolio Capital in dollars. The default is `100000`.
-        `schedule` : `pandas.DataFrame`, optional;
+        schedule : `pandas.DataFrame`, optional
             Rebalancing schedule, with columns for `'Droll'` rolling date and
             `'Dfix'` fixing date. If it is `None` than the schedule will be set
             using the `freq`, `noffset`, `fixoffset` and `calendar`
             information. The default is `None`.
-        `freq` : `str`, optional;
-            rebalancing frequency. It can be `'Q'` for quarterly or `'M'` for
-            monthly rebalancing, respectively. It is relevant only is schedule
-            is `None`. The default is `'Q'`.
-        `noffset` : `int`, optional;
-            Number of business days offset for rebalancing date `'Droll'`
-            relative to the end of the period (quart or month). A positive
-            value add business days beyond the calendar end of the period while
-            a negative value subtracts business days. It is relevant only is
-            schedule is `None`. The default is `-3`.
-        `fixoffset` : `int`, optional;
-            Number of business day offset of fixing date `'Dfix'` relative to
-            the rebalancing date `'Droll'`. It can be 0 or negative. It is
-            relevant only is schedule is `None`. The default is `-1`.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business calendar. If it is `None` then it will be set to NYSE
-            business calendar. The default
-            vale is `None`.
+        multitreading : Boolean, optional
+            If it is `True` then the weights at the rebalancing dates will 
+            be computed concurrent. The default is `True`.
     
         Returns
         -------
         The object.
         """
-        super().__init__(mktdata=mktdata, symb=symb, 
-                         sdate=sdate, edate=edate, 
-                         col_price=col_price, col_divd=col_divd,
-                         col_ref=col_ref, pname=pname,
-                         pcolname=pcolname, capital=capital, 
-                         schedule=schedule, freq=freq, noffset=noffset, 
-                         fixoffset=fixoffset, calendar=calendar)
-        self.col_calib = col_calib
-    
-    def set_model(self, hlength=3.25):
+        super().__init__(mktdata=mktdata, symb=symb, sdate=sdate, edate=edate, 
+                         col_price=col_price, col_divd=col_divd, 
+                         col_ref=col_ref, pname=pname, pcolname=pcolname, 
+                         capital=capital, schedule=schedule)
+        self.nshares = None
+        self.cash_invst = None
+        self.cash_roll = None
+        self.cash_divd = None
+        self.schedule = schedule
+        self.verbose = False
+        
+        
+    def set_model(self, schedule=None, verbose=False):
         """
-        Set model parameters and evaluate the portfolio time-series.
+        Sets model parameters and evaluates the portfolio time-series.
         
         Parameters
         ----------
-        `hlength` : `float`, optional;
-            The length in year of the historical calibration period relative 
-            to `'Dfix'`. A fractional number will be rounded to an integer number 
-            of months. The default is `3.25` years. 
+        schedule : `pandas.DataFrame`, optional
+            Rebalancing schedule, with columns for `'Droll'` rolling date and
+            `'Dfix'` fixing date. If it is `None` than the schedule will be set
+            using the `freq`, `noffset`, `fixoffset` and `calendar`
+            information. It is set to `None` it will overwrite the value 
+            set by the constructor. The default is `None`.
+        
+        verbose : Boolean, optional:
+            Sets teh verbose mode.
 
         Returns
         -------
-        `pandas.DataFrame`;
-            The portfolio time-series in the format "date", "pcolname".
+        `pandas.DataFrame` : The portfolio time-series in the format 'date', 
+        'pcolname'.
         """
-        self.hlength = hlength
-        
-        self._set_schedule()
-        self._set_weights()
+        if schedule is not None:
+            self.schedule = schedule
+            
+        self.ww = self.schedule
+        self.verbose = verbose
         self._port_calc()
         return self.port
     
-    def _set_weights(self):
-        mktdata = self.mktdata.pivot(columns='symbol', values=self.col_calib)
-        periods = 63 if self.freq == 'Q' else 21
+    
+    def _port_calc(self):
+        def _rank(x, ww=self.ww):
+            for k in range(len(ww)):
+                if x < ww.Droll[k]: return k
+            return len(ww)
         
-        # local function
-        def _fww(rr):
-            if rr.Dfix > self.edate:
-                return pd.Series(np.nan, index=mktdata.columns)
+        mktdata = self.mktdata.pivot(columns='symbol', values=self.col_price)
+        div = self.mktdata.pivot(columns='symbol', values=self.col_divd)
+        lw = np.zeros([div.shape[0]], dtype=int)
+        for dx in self.ww.Droll:
+            lw[div.index >= dx] += 1
+        mmix = pd.MultiIndex.from_arrays([lw, div.index], names=('lw', 'date'))
+        div.index = mmix
+        div = div.groupby(level='lw').sum()
+        symb = self.symb
+
+        mktdata.index = mmix
+        mktgr = mktdata.groupby(level='lw')
+        mktdata = mktdata.droplevel(0)
+
+        self.port = []
+        self.nshares = []    
+        self.cash_invst = []
+        self.cash_roll = []
+        self.cash_divd = [0.]   
+        cap = self.capital
+        for k, v in mktgr:
+            if k == 0:  continue
+            v = v.droplevel(0)
             
-            mm = mktdata[rr.Dhist:rr.Dfix].pct_change(periods=periods).dropna()
-            return self._ww_calc(mm)
-        
-        w = self.schedule.apply(_fww, axis=1)
- 
-        self.ww = pd.concat([self.schedule, w], axis=1)
-        
-    def _ww_calc(self, data):
-        vv = 1. / data.std()
-        return vv / vv.sum()
+            nsh = (self.ww[symb].iloc[k - 1] * cap
+                    / mktdata.loc[self.ww.Dfix[k - 1]]).round(0)
+            self.nshares.append(nsh)
+            self.port.append(v @ nsh)
+            
+            invst = nsh @ mktdata.loc[self.ww.Droll[k - 1]]
+            dcap = cap - invst
+            divd = div.loc[k] @ nsh
+            cap = self.port[-1][-1] + divd  + dcap
+            
+            self.cash_invst.append(invst)
+            self.cash_roll.append(dcap)
+            self.cash_divd.append(divd)
+
+        self.port = pd.concat(self.port) \
+            .pipe(pd.DataFrame, columns=[self.pcolname])
+
+        self.nshares = pd.DataFrame(self.nshares,
+                                    index=self.ww.Droll[:len(self.nshares)]) 
+
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_Kelly.py` & `azapy-1.2.0/azapy/PortOpt/Port_InvVar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,39 @@
-from .Port_InvVol import Port_InvVol
-from .KellyEngine import KellyEngine
+from ._Port_Generator import _Port_Generator
+from azapy.Generators.ModelPipeline import ModelPipeline
+from azapy.Engines.InvVarEngine import InvVarEngine
 
-class Port_Kelly(Port_InvVol):
+
+class Port_InvVar(_Port_Generator):
     """
-    Backtesting Kelly optimal portfolio, periodically rebalanced.
+    Backtesting Inverse Variance portfolio periodically rebalanced.
     
-    Methods:
-        * set_model
-        * get_port
-        * get_nshares
-        * get_weights
-        * get_account
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-        * port_period_returns
-    """
-    def set_model(self, rtype='ExpCone', hlength=1.25, method='ecos'):
+    **Attributes**
+        * `pname` : `str` - portfolio name
+        * `ww` : `pandasDataFrame` - portfolio weights at each rebalancing date
+        * `port` : `pandas.Series` - portfolio historical time-series
+        * `schedule` : `pandas.DataFrame` - rebalancing schedule
+       
+    The most important method is `set_model`. It must be called before any
+    other method.
+    """                     
+    def set_model(self, hlength=3.25, verbose=False):
         """
-        Sets model parameters and evaluates portfolio time-series.
-
+        Set model parameters and evaluate the portfolio time-series.
+        
         Parameters
         ----------
-        `rtype` : `str`, optional;
-            Type of optimization. It could take the values:\n
-                `'ExpCone'` - Exponential cone constraint programming solution
-                for full Kelly problem. \n
-                `'Full'` - Non-linear solver for full Kelly problem. \n
-                `'Order2'` - Second order Tayler approximation of Kelly problem. \n
-            The default is `'ExpCone'`.
-        `hlength` : `float`, optional;
+        hlength : `float`, optional
             The length in year of the historical calibration period relative 
             to `'Dfix'`. A fractional number will be rounded to an integer number 
-            of months. The default is `1.25` years. 
-        `method` : `str`, optional;
-            The QP solver class. It is relevant only if `rtype='Order2'`.
-            It takes 2 values: `'ecos'` or `'cvxopt'`.
-            The default is `'ecos'`.
+            of months. The default is `3.25` years. 
+        verbose : Boolean, optional
+            Sets verbose mode. The default is `False`.
 
         Returns
         -------
-        `pandas.DataFrame`;
-            The portfolio time-series in the format "date", "pcolname".
+        `pandas.DataFrame` : The portfolio time-series in the format 'date', 
+        'pcolname'.
         """
-        self.rtype= rtype
-        self.method = method
-        
-        return super().set_model(hlength)
- 
-            
-    def _ww_calc(self, data):
-        return KellyEngine().getWeights(rrate=data, 
-                                        rtype=self.rtype, 
-                                        method=self.method)
+        mod = InvVarEngine(colname=self.col_calib, freq=self.freq,
+                           hlength=hlength)
+        return super().set_model(ModelPipeline([mod]), verbose)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_LSD.py` & `azapy-1.2.0/azapy/PortOpt/Port_LSD.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,110 +1,101 @@
-from .Port_MAD import Port_MAD
-from .LSDAnalyzer import LSDAnalyzer
+from ._Port_Generator import _Port_Generator
+from azapy.Generators.ModelPipeline import ModelPipeline
+from azapy.Analyzers.LSDAnalyzer import LSDAnalyzer
 
-class Port_LSD(Port_MAD):
+
+class Port_LSD(_Port_Generator):
     """
-    Backtesting mLSD optimal portfolio strategies, periodically rebalanced.
+    Backtesting LSD (Lower Standard Deviation) portfolio periodically 
+    rebalanced.
     
-    Methods:
-        * set_model
-        * get_port
-        * get_nshares
-        * get_weights
-        * get_account
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-        * port_period_returns
-    """    
-    def set_model(self, coef=[1.], rtype='Sharpe', mu=None, mu0=0,
-                  aversion=None, ww0=None, hlength=3.25, method='ecos',
-                  verbose=False):
+    **Attributes**
+        * `pname` : `str` - portfolio name
+        * `ww` : `pandasDataFrame` - portfolio weights at each rebalancing date
+        * `port` : `pandas.Series` - portfolio historical time-series
+        * `schedule` : `pandas.DataFrame` - rebalancing schedule
+       
+    The most important method is `set_model`. It must be called before any
+    other method.
+    """                     
+    def set_model(self, coef=[1], rtype='Sharpe',
+                  mu=None, mu0=0, aversion=None, ww0=None, 
+                  hlength=3.25, method='ecos', verbose=False):
         """
-        Set model parameters and evaluates portfolio time-series.
+        Sets model parameters and evaluates portfolio time-series.
 
         Parameters
         ----------
-        `coef` : `list`, optional;
+        coef : `list`, optional
             Positive non-increasing list of coefficients. 
             The default is `[1.]`.
-        `rtype` : `str`, optional;
+        rtype : `str`, optional
             Optimization type. Possible values: \n
                 `'Risk'` : optimal-risk portfolio for targeted expected rate of 
                 return.\n
                 `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
                 `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
                 `'RiskAverse'` : optimal-risk portfolio for a fixed 
                 risk-aversion factor.\n
                 `'InvNrisk'` : optimal-risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
                 `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
+                expected rate of return (maximum of inverse of 1-D).\n
                 `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                expected rate of return (minimum of 1-D).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
                 `'InvNdiverse'` : optimal-diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
                 `'InvNdrr'` : optima- diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `mu` : `float`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
             Targeted portfolio expected rate of return. 
             Relevant only if `rtype='Risk'`
             The default is `None`.
-        `mu0` : `float`, optional;
+        mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
-        `aversion` : `float`, optional;
+        aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
-        `ww0` : `list` (also `numpy.array` or `pandas.Series`), optional;
+        ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
             Relevant only if `rype='InvNrisk'`.
             Its length must be equal to the number of
-            symbols in rrate (mktdata). 
-            All weights must be >= 0 with sum > 0.
+            symbols in `rrate` (`mktdata`). 
+            All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
-            the index should be compatible with the `rrate.columns` or mktdata 
-            symbols (same symbols, not necessary in the same order).
+            the index should be compatible with the `rrate.columns` or `mktdata` 
+            symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        `hlength` : `float`, optional;
+        hlength : `float`, optional
             The length in year of the historical calibration period relative
             to `'Dfix'`. A fractional number will be rounded to an integer 
             number of months. The default is `3.25` years.
-        `method` : `str`, optional;
-            SOCP numerical method.
-            It could be `'ecos'` or `'cvxopt'`.
+        method : `str`, optional
+            SOCP numerical method. Could be: `'ecos'` or `'cvxopt'`.
             The defualt is `'ecos'`.
-        `verbose` : Boolean, optiona;
+        verbose : Boolean, optional
             If it set to `True` then it will print messages when the optimal
             portfolio degenerates to a single asset portfolio as a limited 
             case. 
             The default is `False`.
 
         Returns
         -------
-        `pandas.DataFrame`;
-            The portfolio time-series in the format "date", "pcolname".
+        `pandas.DataFrame` : The portfolio time-series in the format 'date', 
+        'pcolname'.
         """
-        return super().set_model(coef=coef, rtype=rtype, mu=mu, mu0=mu0,
-                                 aversion=aversion, ww0=ww0, 
-                                 hlength=hlength, method=method,
-                                 verbose=verbose)
-    
-        
-    def _wwgen(self):
-        return LSDAnalyzer(coef=self.coef, rtype=self.rtype, 
-                           method=self.method, name=self.pname)
-    
+        mod = LSDAnalyzer(coef=coef,
+                          colname=self.col_calib, freq=self.freq,
+                          hlength=hlength, rtype=rtype, mu=mu, d=1, mu0=mu0,
+                          aversion=aversion, ww0=ww0, method=method)
+        return super().set_model(ModelPipeline([mod]), verbose)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_MAD.py` & `azapy-1.2.0/azapy/PortOpt/Port_SMCR.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,111 +1,106 @@
-from .Port_CVaR import Port_CVaR
-from .MADAnalyzer import MADAnalyzer
+from ._Port_Generator import _Port_Generator
+from azapy.Generators.ModelPipeline import ModelPipeline
+from azapy.Analyzers.SMCRAnalyzer import SMCRAnalyzer
 
 
-class Port_MAD(Port_CVaR):
+class Port_SMCR(_Port_Generator):
     """
-    Backtesting mMAD optimal portfolio strategies, periodically rebalanced.
-
-    Methods:
-        * set_model
-        * get_port
-        * get_nshares
-        * get_weights
-        * get_account
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-        * port_period_returns
-    """
-    def set_model(self, coef=[1.], rtype='Sharpe', mu=None, mu0=0,
-                  aversion=None, ww0=None, hlength=3.25, method='ecos',
-                  verbose=False):
+    Backtesting SMCR (Second Momentum Coherent Risk) portfolio periodically 
+    rebalanced.
+    
+    **Attributes**
+        * `pname` : `str` - portfolio name
+        * `ww` : `pandasDataFrame` - portfolio weights at each rebalancing date
+        * `port` : `pandas.Series` - portfolio historical time-series
+        * `schedule` : `pandas.DataFrame` - rebalancing schedule
+       
+    The most important method is `set_model`. It must be called before any
+    other method.
+    """          
+    def set_model(self, alpha=[0.90], coef=None, rtype='Sharpe',
+                  mu=None, mu0=0, aversion=None, ww0=None, 
+                  hlength=3.25, method='ecos', verbose=False):
         """
-        Set model parameters and evaluates portfolio time-series.
+        Sets model parameters and evaluates portfolio time-series.
 
         Parameters
         ----------
-        `coef` : `list`, optional;
-            Positive non-increasing list of coefficients. 
-            The default is `[1.]`.
-        `rtype` : `str`, optional;
+        alpha : `list`, optional
+            List of distinct alpha confidence levels. The default is `[0.9]`.
+        coef : `list`, optional
+            List of positive mixture coefficients. Note that `len(coef)`
+            must be equal to `len(alpha)`. A `None` value assumes an
+            equal weighted risk mixture.
+            The vector of coefficients will be normalized to unit.
+            The default is `None`.
+        rtype : `str`, optional
             Optimization type. Possible values: \n
                 `'Risk'` : optimal-risk portfolio for targeted expected rate of 
                 return.\n
                 `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
                 `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
                 `'RiskAverse'` : optimal-risk portfolio for a fixed 
                 risk-aversion factor.\n
                 `'InvNrisk'` : optimal-risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
                 `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
+                expected rate of return (maximum of inverse of 1-D).\n
                 `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                expected rate of return (minimum of 1-D).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
                 `'InvNdiverse'` : optimal-diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
                 `'InvNdrr'` : optima- diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `mu` : `float`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
             Targeted portfolio expected rate of return. 
             Relevant only if `rtype='Risk'`
             The default is `None`.
-        `mu0` : `float`, optional;
+        mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
-        `aversion` : `float`, optional;
+        aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
-        `ww0` : `list` (also `numpy.array` or `pandas.Series`), optional;
+        ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
             Relevant only if `rype='InvNrisk'`.
             Its length must be equal to the number of
-            symbols in rrate (mktdata). 
-            All weights must be >= 0 with sum > 0.
+            symbols in `rrate` (`mktdata`). 
+            All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
-            the index should be compatible with the `rrate.columns` or mktdata 
-            symbols (same symbols, not necessary in the same order).
+            the index should be compatible with the `rrate.columns` or `mktdata` 
+            symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        `hlength` : `float`, optional;
+        hlength : `float`, optional
             The length in year of the historical calibration period relative
             to `'Dfix'`. A fractional number will be rounded to an integer 
             number of months. The default is `3.25` years.
-        `method` : `str`, optional;
-            Linear programming numerical method.
-            Could be: `'ecos'`, `'highs-ds'`, `'highs-ipm'`, `'highs'`,
-            `'interior-point'`, `'glpk'` and `'cvxopt'`.
-            The default is `'ecos'`.
-        `verbose` : Boolean, optiona;
+        method : `str`, optional
+            SOCP numerical method. Could be: `'ecos'` or `'cvxopt'`.
+            The defualt is `'ecos'`.
+        verbose : Boolean, optional
             If it set to `True` then it will print messages when the optimal
             portfolio degenerates to a single asset portfolio as a limited 
             case. 
             The default is `False`.
 
-         Returns
+        Returns
         -------
-        `pandas.DataFrame`;
-            The portfolio time-series in the format 'date', 'pcolname'.
+        `pandas.DataFrame` : The portfolio time-series in the format 'date', 
+        'pcolname'.
         """
-        return super().set_model(coef=coef, rtype=rtype, 
-                                 mu=mu, mu0=mu0, aversion=aversion, ww0=ww0,
-                                 hlength=hlength, method=method,
-                                 verbose=verbose)
-
-
-    def _wwgen(self):
-        return MADAnalyzer(coef=self.coef, rtype=self.rtype,
-                           method=self.method, name=self.pname)
+        mod = SMCRAnalyzer(alpha=alpha, coef=coef,
+                           colname=self.col_calib, freq=self.freq,
+                           hlength=hlength, rtype=rtype, mu=mu, d=1, mu0=mu0,
+                           aversion=aversion, ww0=ww0, method=method)
+        return super().set_model(ModelPipeline([mod]), verbose)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_MV.py` & `azapy-1.2.0/azapy/PortOpt/Port_SD.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,105 +1,95 @@
-from .Port_CVaR import Port_CVaR
-from .MVAnalyzer import MVAnalyzer
+from ._Port_Generator import _Port_Generator
+from azapy.Generators.ModelPipeline import ModelPipeline
+from azapy.Analyzers.SDAnalyzer import SDAnalyzer
 
-class Port_MV(Port_CVaR):
-    """
-    Backtesting MV optimal portfolio strategies, periodically rebalanced.
 
-    Methods:
-        * set_model
-        * get_port
-        * get_nshares
-        * get_weights
-        * get_account
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-        * port_period_returns
+class Port_SD(_Port_Generator):
     """
+    Backtesting SD (Standard Deviation) portfolio periodically rebalanced.
+    
+    **Attributes**
+        * `pname` : `str` - portfolio name
+        * `ww` : `pandasDataFrame` - portfolio weights at each rebalancing date
+        * `port` : `pandas.Series` - portfolio historical time-series
+        * `schedule` : `pandas.DataFrame` - rebalancing schedule
+       
+    The most important method is `set_model`. It must be called before any
+    other method.
+    """                          
     def set_model(self, rtype='Sharpe', mu=None, mu0=0, aversion=None, 
                   ww0=None, hlength=3.25, method='ecos', verbose=False):
         """
         Sets model parameters and evaluates portfolio time-series.
 
         Parameters
         ----------.
-        `rtype` : `str`, optional;
+        rtype : `str`, optional
             Optimization type. Possible values: \n
                 `'Risk'` : optimal-risk portfolio for targeted expected rate of 
                 return.\n
                 `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
                 `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
                 `'RiskAverse'` : optimal-risk portfolio for a fixed 
                 risk-aversion factor.\n
                 `'InvNrisk'` : optimal-risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
                 `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
+                expected rate of return (maximum of inverse of 1-D).\n
                 `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                expected rate of return (minimum of 1-D).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
                 `'InvNdiverse'` : optimal-diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
                 `'InvNdrr'` : optima- diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `mu` : `float`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
             Targeted portfolio expected rate of return. 
             Relevant only if `rtype='Risk'`
             The default is `None`.
-        `mu0` : `float`, optional;
+        mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
-        `aversion` : `float`, optional;
+        aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
-        `ww0` : `list` (also `numpy.array` or `pandas.Series`), optional;
+        ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
             Relevant only if `rype='InvNrisk'`.
             Its length must be equal to the number of
-            symbols in rrate (mktdata). 
-            All weights must be >= 0 with sum > 0.
+            symbols in `rrate` (`mktdata`). 
+            All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
-            the index should be compatible with the `rrate.columns` or mktdata 
-            symbols (same symbols, not necessary in the same order).
+            the index should be compatible with the `rrate.columns` or `mktdata` 
+            symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        `hlength` : `float`, optional;
+        hlength : `float`, optional
             The length in year of the historical calibration period relative
             to `'Dfix'`. A fractional number will be rounded to an integer 
             number of months. The default is `3.25` years.
-        `method` : `str`, optional;
+        method : `str`, optional
             Numerical method to solve the SOCP and QP. It can be `'ecos'` or 
             `'cvxopt'`. The default is `'ecos'`.
-        `verbose` : Boolean, optiona;
+        verbose : Boolean, optional
             If it set to `True` then it will print messages when the optimal
             portfolio degenerates to a single asset portfolio as a limited 
             case. 
             The default is `False`.
 
         Returns
         -------
-        `pandas.DataFrame`;
-            The portfolio time-series in the format "date", "pcolname".
+        `pandas.DataFrame` : The portfolio time-series in the format 'date', 
+        'pcolname'.
         """
-        return super().set_model(rtype=rtype, mu=mu, mu0=mu0, 
-                                 aversion=aversion, ww0=ww0,
-                                 hlength=hlength, method=method,
-                                 verbose=verbose)
-
-
-    def _wwgen(self):
-        return MVAnalyzer(rtype=self.rtype, method=self.method, 
-                          name=self.pname)
-    
+        mod = SDAnalyzer(colname=self.col_calib, freq=self.freq,
+                         hlength=hlength, rtype=rtype, mu=mu, d=1, mu0=mu0,
+                         aversion=aversion, ww0=ww0, method=method)
+        return super().set_model(ModelPipeline([mod]), verbose)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_Rebalanced.py` & `azapy-1.2.0/azapy/Engines/_RiskEngine.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,266 +1,284 @@
+import numpy as np
 import pandas as pd
 
-from .Port_Simple import Port_Simple
-
-class Port_Rebalanced(Port_Simple):
+class _RiskEngine():
     """
-    Backtesting the portfolio with custom rebalancing schedule.
+    Base class.
+    
+    **Attributes**
+        * status : `int` - computation status (`0` - success, any other 
+          value indicates an error)
+        * ww : `pandas.Series` - portfolio weights
+        * name : `str` - portfolio name
     
-    Methods:
-        * set_model
-        * get_port
-        * get_nshares
-        * get_weights
-        * get_account
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-        * port_period_returns
+    Note: Derive class needs to implement `getWeights` method
+    
+    **Methods**
+        * getPositions
+        * set_rrate
+        * set_mktdata
     """
-    def __init__(self, mktdata, symb=None, sdate=None, edate=None, 
-                 col_price='close', col_divd='divd', col_ref='adjusted',
-                 pname='Port', pcolname=None, capital=100000):
+    def __init__(self, mktdata=None, colname='adjusted', freq='Q', 
+                 hlength=3.25, name=None):
         """
         Constructor
 
         Parameters
         ----------
-        `mktdata` : `pandas.DataFrame`;
-            MkT data in the format "symbol", "date", "open", "high", "low",
-            "close", "volume", "adjusted", "divd", "split" (e.g. as returned
-            by `azapy.readMkT` function).
-        `symb` : `list`, optional;
-            List of symbols for the basket components. All symbols MkT data
-            should be included in `mktdata`. If set to `None` the `symb` will  
-            be set to the full set of symbols included in `mktdata`. 
-            The default is `None`.
-        `sdate` : date-like, optional;
-            Start date for historical data. If set to `None` then the `sdate` 
-            will  be set to the earliest date in mktdata. 
-            The default is `None`.
-        `edate` : date-like, optional;
-            End date for historical dates and so the simulation. Must be 
-            greater than  `sdate`. If it is `None` then `edate` will be set
-            to the latest date in `mktdata`. The default is `None`.
-        `col_price` : `str`, optional;
-            Column name in the mktdata DataFrame that will be considered 
-            for portfolio aggregation. The default is `'close'`.
-        `col_divd` :  `str`, optional;
-            Column name in the mktdata DataFrame that holds the dividend 
-            information. The default is `'dvid'`.
-        `col_ref` : `str`, optional;
-            Column name in the mktdata DataFrame that will be used as a price 
-            reference for portfolio components. The default is `'adjusted'`.
-        `pname` : `str`, optional;
-            The name of the portfolio. The default is `'Port'`.
-        `pcolname` : `str`, optional;
-            Name of the portfolio price column. If it set to `None` then 
-            `pcolname=pname`. The default is `None`.
-        `capital` : `float`, optional;
-            Initial portfolio Capital in dollars. The default is `100000`.
+        mktdata : `pandas.DataFrame`, optional
+            Historic daily market data for portfolio components in the format
+            returned by `azapy.mktData` function. The default is `None`.
+        colname : `str`, optional
+            Name of the price column from mktdata used in the weights
+            calibration. The default is `'adjusted'`.
+        freq : `str`, optional
+            Rate of return horizon. It could be 
+            `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
+            History length in number of years used for calibration. A
+            fractional number will be rounded to an integer number of months.
+            The default is `3.25` years.
+        name : `str`, optional
+            Portfolio name. Deafult value is `None`
 
         Returns
         -------
         The object.
         """
-        super().__init__(mktdata=mktdata, symb=symb, 
-                         sdate=sdate, edate=edate, 
-                         col=col_ref, pname=pname, 
-                         pcolname=pcolname, capital=capital)
-        self.col_price = col_price
-        self.col_divd = col_divd
-        self.nshares = None
+        self._ptype_ = 'Optimizer'
+        self.ww = None
+        self.status = None
+        
+        self.colname = None
+        self.freq = None
+        self.hlength = None
+        self.name = name
         
-        self.cash_invst = None
-        self.cash_roll = None
-        self.cash_divd = None
+        self.verbose = False
         
-    def set_model(self, ww):
+        self.time_level1 = None
+        self.time_level2 = None
+        self.time_level3 = None
+
+        self.set_mktdata(mktdata, colname, freq, hlength)
+
+
+    def set_rrate(self, rrate):
         """
-        Set model parameters and evaluate the portfolio time-series.
+        Sets portfolio components historical rates of return in the format
+        "date", "symbol1", "symbol2", etc.
 
         Parameters
         ----------
-        `ww` : `pandas.DataFrame`;
-            Rebalance schedule. The following columns must be present: \n
-                "Droll" : rolling date (rebalancing day) \n
-                "Dfix" : fixing date (day when the close price are recorded) \n
-                name of symbol 1 : weights for symbol 1 \n
-                name of symbol 2 : weights for symbol 2 \n
-                erc. \n
-            The symbol name must match the symbol names from `mktdata`.
-            
-        Returns
-        -------
-        `pandas.DataFrame`;
-            The portfolio time-series in the format "date", "pcolname".
-        """
-        # Make sure that the weights are normalized
-        self.ww = ww.copy()
-        self.ww[self.symb] = self.ww[self.symb] \
-                                 .apply(lambda x: x / x.sum(), axis=1)
-        
-        # Calculate
-        self._port_calc()
-        return self.port
-    
-    def get_nshares(self):
-        """
-        Returns the number of shares hold after each rolling date.
+        rrate : `pandas.DataFrame`
+            The portfolio components historical rates of return.
+            If it is not `None`, it will overwrite the `rrate` computed in the
+            constructor from `mktdata`. The default is `None`.
 
         Returns
         -------
-        `pandas.DataFrame`
+        `None`
         """
-        return self.nshares.astype('int').copy()
-    
-    def get_weights(self, fancy=False):
+        if rrate is None:
+            # noting to do
+            return
+
+        self.nn, self.mm = rrate.shape
+        self.muk = rrate.mean(numeric_only=True)
+        self.rrate = rrate
+
+
+    def set_mktdata(self, mktdata, colname='adjusted', freq=None, hlength=None,
+                    pclose=False):
         """
-        Returns the portfolio weights at each rebalancing period.
-        
+        Sets historical market data. It will overwrite the choice made in the
+        constructor.
+
         Parameters
         ----------
-        `fancy` : Boolean, optional;
-            * `False`: reports the weights in algebraic format.
-            * `True`: reports the weights in percent rounded to 2 decimals.
+        mktdata : `pandas.DataFrame`
+            Historic daily market data for portfolio components in the format
+            returned by `azapy.mktData` function.
+        colname : `str`, optional
+            Name of the price column from mktdata used in the weight's
+            calibration. The default is 'adjusted'.
+        freq : `str`, optional
+            Rate of return horizon. It could be 
+            `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
+            History length in number of years used for calibration. A
+            fractional number will be rounded to an integer number of months.
+            The default is `3.25`.
+        pclose : Boolena, optiona \n
+            `True` : assumes `mktdata` contains closing prices only, 
+            with columns the asset symbols and indexed by the 
+            observation dates, \n
+            `False` : assumes `mktdata` is in the usual format
+            returned by `azapy.mktData` function.
             
-        The default is `False`.
-
         Returns
         -------
-        `pandas.DataFrame`
+        `None`
         """
-        res = self.ww.copy()
-        if not fancy:
-            return res
-        
-        res[self.symb] = res[self.symb].round(4).abs() * 100
-        
-        return res
-    
-    def _port_calc(self):
-        def _rank(x, ww=self.ww):
-            for k in range(len(ww)):
-                if x < ww.Droll[k]: return k
-            return len(ww)
-        
-        mktdata = self.mktdata.pivot(columns='symbol', values=self.col_price)
-        
-        div = self.mktdata.pivot(columns='symbol', values=self.col_divd) \
-            .groupby(_rank).sum()
-        self.port = []
-        self.nshares = []
-        
-        self.cash_invst = []
-        self.cash_roll = []
-        self.cash_divd = [0.]
-        
-        cap = self.capital
-        for k, v in mktdata.groupby(_rank):
-            if k == 0:  continue
- 
-            nsh = (self.ww[self.symb].iloc[k - 1] \
-                   / mktdata.loc[self.ww.Dfix[k - 1]] * cap).round(0)
-            self.nshares.append(nsh)
-            self.port.append(v @ nsh)
+        if colname is None:
+            if self.colname is None:
+                raise ValueError("Unspecified price colum (colname).")
+        else:
+            self.colname = colname
+        
+        if freq is None:
+            if self.freq is None:
+                raise ValueError("freq not set - it must be 'Q' or 'M'.")
+        elif freq in ['Q', 'M']:
+            self.freq = freq
+        else:
+            raise ValueError(f"wrrong value for freq: {freq}" 
+                              " - it must be 'Q' or 'M'.")
             
-            invst = nsh @ mktdata.loc[self.ww.Droll[k - 1]]
-            dcap = cap - invst
-            divd = div.iloc[k] @ nsh
-            cap = self.port[-1][-1] + divd  + dcap
+        if hlength is None:
+            if self.hlength is None:
+                raise ValueError("hlength must be set to a positive "
+                                 "value eq 1")
+        else:
+            self.hlength = hlength
+
+        if mktdata is None:
+            # nothing else to do
+            return
+        
+        periods = 63 if self.freq == 'Q' else 21
+        sdate = mktdata.index[int(-np.round(self.hlength * 12) * 21)]
+
+        if pclose == False:
+            if self.colname not in mktdata.columns:
+                raise ValueError(f"colname: {colname} not in mktdata.columns")
+            rrate = mktdata.pivot(columns='symbol', 
+                                  values=self.colname)[sdate:]
+        else:
+            rrate = mktdata[sdate:]
             
-            self.cash_invst.append(invst)
-            self.cash_roll.append(dcap)
-            self.cash_divd.append(divd)
- 
-        self.port = pd.concat(self.port) \
-            .pipe(pd.DataFrame, columns=[self.pcolname])
-
-        self.nshares = pd.DataFrame(self.nshares,
-                                    index=self.ww.Droll[:len(self.nshares)])
- 
-    def get_account(self, fancy=False):
+        self.last_data = rrate.iloc[-1]
+        rrate = rrate.pct_change(periods=periods).dropna()
+        self.set_rrate(rrate)
+
+
+    def getPositions(self, nshares=None, cash=0., ww=None, verbose=True):
         """
-        Returns additional bookkeeping information regarding rebalancing 
-        (e.g. residual cash due rounding number of shares, previous period 
-         dividend cash accumulation, etc.)
+        Computes the rebalanced number of shares.
 
         Parameters
         ----------
-        `fancy` : Boolean, optional;
-            * `False`: the values are reported in unaltered algebraic format. 
-            * `True` : the values are reported rounded.
-            
-        The default is `False`.
-
+        nshares : `panda.Series`, optional
+            Initial number of shares per portfolio component.
+            A missing component
+            entry will be considered 0. A `None` value assumes that all
+            components entries are 0. The name of the components must be
+            present in the mrkdata. The default is `None`.
+        cash : `float`, optional
+            Additional cash to be added to the capital. A
+            negative entry assumes a reduction in the total capital
+            available for rebalance. The total capital cannot be < 0.
+            The default is 0. 
+        ww : `panda.Series`, optional
+            External overwrite portfolio weights. 
+            If it not set to `None` these
+            weights will overwrite the calibration results.
+            The default is `None`. 
+        verbose : Boolean, optional
+            Is it set to `True` the function prints the closing prices date.
+            The default is `True`.
+        
         Returns
         -------
-        `pandas.DataFrame`;
-            Reports, for each rolling period identified by `'Droll'`: 
+        `pandas.DataFrame` : the rolling information.
 
-            * number of shares hold for each symbol,
-            * 'cash_invst' : cash invested at the beginning of period,
-            * 'cash_roll' : cash rolled to the next period,
-            * 'cash_divd' : cash dividend accumulated in the previous period.
-                
-        Note: The capital at the beginning of the period is 
-        cash_invst + cash_roll. It is also equal to the previous period: 
-        value of the shares on the fixing date + cash_roll + cash_divd.
-        There are 2 sources for the cash_roll. The roundup to integer 
-        number of shares and the shares close price differences between 
-        the fixing (computation) and rolling (execution) dates. It could
-        be positive or negative. The finance of the cash_roll during 
-        each rolling period is assumed to be done separately by the investor.
-        """
-        acc_tab = self.nshares.copy()
-        acc_tab['cash_invst'] = self.cash_invst
-        acc_tab['cash_roll'] = self.cash_roll
-        acc_tab['cash_divd'] = self.cash_divd[:-1]
-        
-        if not fancy: return acc_tab
-        
-        acc_tab = acc_tab.round(2)
-        acc_tab[self.symb] = acc_tab[self.symb].astype('int')
-        
-        return acc_tab
+        Columns:
 
-    def port_period_returns(self, fancy=False):
-        """
-        Computes the rolling periods rate of returns. 
+            - `'old_nsh'` :
+                initial number of shares per portfolio component and
+                the additional cash. These are input values.
+            - `'new_nsh'` :
+                the new number of shares per component plus the residual
+                cash (due to the rounding to an integer number of shares).
+                A negative entry means that the investor needs to add more
+                cash to cover for the roundup shortfall.
+                It has a small value.
+            - `'diff_nsh'` :
+                number of shares (buy/sale) needed to rebalance the 
+                portfolio.
+            - `'weights'` :
+                portfolio weights used for rebalancing. The cash entry is
+                the new portfolio value (invested capital).
+            - `'prices'` :
+                the share prices used for rebalances evaluations.
+
+            Note: Since the prices are closing prices, the rebalance can be
+            computed after the market close and before the 
+            trading execution (next day). 
+            Additional cash slippage may occur due
+            to share price differential between the previous day closing and
+            execution time.
+        """
+        ns = pd.Series(0, index=self.rrate.columns)
+        if nshares is not None:
+            ns = ns.add(nshares, fill_value=0)
+
+        if len(self.rrate.columns) != len(ns):
+            raise ValueError("nshares must by a subset "
+                             f"of {self.rrate.columns}")
 
-        Parameters
-        ----------
-        `fancy` : Boolean, optional;
-           * `False`: returns in algebraic form.
-           * `True`: returns in percent rounded to 2 decimals.
-        The default is `False`.
+        if self.last_data is None:
+            raise ValueError("The obj was not set with mktdata")
+            
+        if verbose:
+            print(f"Use closing prices as of {self.last_data.name}")
 
-        Returns
-        -------
-        `pandas.DataFrame`;
-            Each rolling period is indicated by its start date, `'Droll'`. 
-            Included are the fixing data, `'Dfix'`, and the 
-            portfolio weights.
-        """
-        # local function
-        def frr(x):
-            p2 = x.p1.shift(-1)
-            p2.iloc[-1] = self.port.iloc[-1,-1]
-            return p2 / x.p1 - 1
-        
-        rww = self.ww.merge(self.port, left_on='Droll', right_index=True)\
-                  .rename(columns={self.port.columns[0]: 'p1'})\
-                  .assign(RR=frr)[['Droll', 'Dfix', 'RR'] + list(self.symb)]
- 
-        if not fancy:
-            return rww
+        pp = self.last_data[self.rrate.columns.to_list()]
+
+        cap = ns.dot(pp) + cash
+        if ww is None:
+            ww = self.getWeights()
+        else:
+            ww0 = pd.Series(0, index=self.rrate.columns)
+            ww = ww0.add(ww, fill_value=0)
+            if len(self.rrate.columns) != len(ns):
+                raise ValueError("ww: wrong component names - "
+                                 f"must be among {self.rrate.columns}")
+
+        newns = (ww / pp * cap).round(0)
+        newcash = cap - newns.dot(pp)
+
+        ns['cash'] = cash
+        newns['cash'] = newcash
+        ww['cash'] = cap - newcash
+        pp['cash'] = 1.
+
+        res = pd.DataFrame({'old_nsh': ns,
+                            'new_nsh': newns,
+                            'diff_nsh': newns - ns,
+                            'weights' : ww.round(6),
+                            'prices': pp})
+
+        return res
+
+
+    def _set_getWeights(self, mktdata=None, **params):
+        self._reset_output()
+        self.verbose = params['verbose'] if 'verbose' in params.keys() else False
+
+        if 'pclose' in params.keys():
+            self.set_mktdata(mktdata, pclose=params['pclose'])
+        else:
+            self.set_rrate(mktdata)
+
+
+    def _reset_output(self):
+        self.status = None
+        self.ww = None
+        self.time_level1 = None
+        self.time_level2 = None
+        self.time_level3 = None
         
-        rww['RR'] = rww['RR'].round(4) * 100
-        rww[self.symb] = rww[self.symb].round(4).abs() * 100
         
-        return rww
-    
+    def getWeights(self):
+        pass
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_SMCR.py` & `azapy-1.2.0/azapy/PortOpt/Port_BTAD.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,114 +1,112 @@
-from .Port_CVaR import Port_CVaR
-from .SMCRAnalyzer import SMCRAnalyzer
+from ._Port_Generator import _Port_Generator
+from azapy.Generators.ModelPipeline import ModelPipeline
+from azapy.Analyzers.BTADAnalyzer import BTADAnalyzer
 
-class Port_SMCR(Port_CVaR):
+
+class Port_BTAD(_Port_Generator):
     """
-    Back testing the SMCR optimal portfolio periodically rebalanced.
+    Backtesting BTAD (Below Threshold Absolute Deviation) portfolio 
+    periodically rebalanced.
     
-    Methods:
-        * set_model
-        * get_port
-        * get_nshares
-        * get_weights
-        * get_account
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-        * port_period_returns
+    **Attributes**
+        * `pname` : `str` - portfolio name
+        * `ww` : `pandasDataFrame` - portfolio weights at each rebalancing date
+        * `port` : `pandas.Series` - portfolio historical time-series
+        * `schedule` : `pandas.DataFrame` - rebalancing schedule
+        
+    The most important method is `set_model`. It must be called before any
+    other method.
     """
-    def set_model(self, alpha=[0.9], coef=None, rtype='Sharpe', mu=None,
-                  mu0=0, aversion=None, ww0=None, hlength=3.25, method='ecos',
-                  verbose=False):
+    def set_model(self, alpha=[0.], coef=None, rtype='Sharpe', mu=None, 
+                  mu0=0, aversion=None, ww0=None, detrended=True, 
+                  hlength=3.25, method='ecos', verbose=False):
         """
         Sets model parameters and evaluates portfolio time-series.
 
         Parameters
         ----------
-        `alpha` : `list`, optional;
-            List of distinct alpha confidence levels. The default is `[0.9]`.
-        `coef` : `list`, optional;
+        alpha : `list`, optional
+            List of thresholds. The default is `[0.]`.
+        coef : `list`, optional
             List of positive mixture coefficients. Note that `len(coef)`
             must be equal to `len(alpha)`. A `None` value assumes an
             equal weighted risk mixture.
             The vector of coefficients will be normalized to unit.
             The default is `None`.
-        `rtype` : `str`, optional;
+        rtype : `str`, optional
             Optimization type. Possible values: \n
                 `'Risk'` : optimal-risk portfolio for targeted expected rate of 
                 return.\n
                 `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
                 `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
                 `'RiskAverse'` : optimal-risk portfolio for a fixed 
                 risk-aversion factor.\n
                 `'InvNrisk'` : optimal-risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
                 `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
+                expected rate of return (maximum of inverse of 1-D).\n
                 `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                expected rate of return (minimum of 1-D).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
                 `'InvNdiverse'` : optimal-diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
                 `'InvNdrr'` : optima- diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `mu` : `float`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
             Targeted portfolio expected rate of return. 
             Relevant only if `rtype='Risk'`
             The default is `None`.
-        `mu0` : `float`, optional;
+        mu0 : `float`, optional
             Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            Relevant only if `rtype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
-        `aversion` : `float`, optional;
+        aversion : `float`, optional
             The value of the risk-aversion factor.
             Must be positive. Relevant only if `rtype='RiskAvers'`.
             The default is `None`.
-        `ww0` : `list` (also `numpy.array` or `pandas.Series`), optional;
+        ww0 : `list` (also `numpy.array` or `pandas.Series`), optional
             Targeted portfolio weights. 
             Relevant only if `rype='InvNrisk'`.
             Its length must be equal to the number of
-            symbols in rrate (mktdata). 
-            All weights must be >= 0 with sum > 0.
+            symbols in `rrate` (`mktdata`). 
+            All weights must be >= 0 with their sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             by in order of `rrate.columns`. If it is a `pandas.Series` then 
-            the index should be compatible with the `rrate.columns` or mktdata 
-            symbols (same symbols, not necessary in the same order).
+            the index should be compatible with the `rrate.columns` or `mktdata` 
+            symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        `hlength` : `float`, optional;
+        detrendent : Boolean, optional
+            If it set to `True` then the rates of return are detrended 
+            (`mean=0`). The default value is `True`. 
+        hlength : `float`, optional
             The length in year of the historical calibration period relative
             to `'Dfix'`. A fractional number will be rounded to an integer 
             number of months. The default is `3.25` years.
-        `method` : `str`, optional;
-            SOCP numerical method.
-            It could be `'ecos'` or `'cvxopt'`.
+        method : `str`, optional
+            Linear programming numerical method.
+            Could be: `'ecos'`, `'highs-ds'`, `'highs-ipm'`, `'highs'`,
+            `'interior-point'`, `'glpk'` and `'cvxopt'`.
             The default is `'ecos'`.
-        `verbose` : Boolean, optiona;
+        verbose : Boolean, optional
             If it set to `True` then it will print messages when the optimal
             portfolio degenerates to a single asset portfolio as a limited 
             case. 
             The default is `False`.
 
         Returns
         -------
-        `pandas.DataFrame`;
-            The portfolio time-series in the format 'date', 'pcolname'.
+        `pandas.DataFrame` : The portfolio time-series in the format 'date', 
+        'pcolname'.
         """
-        return super().set_model(alpha=alpha, coef=coef, rtype=rtype, 
-                                 mu=mu, mu0=mu0, aversion=aversion,
-                                 hlength=hlength, method=method,
-                                 verbose=verbose)
-    
-        
-    def _wwgen(self):
-        return SMCRAnalyzer(self.alpha, self.coef, rtype=self.rtype,
-                            method=self.method, name=self.pname)
+        mod = BTADAnalyzer(alpha=alpha, coef=coef,
+                           colname=self.col_calib, freq=self.freq,
+                           hlength=hlength, rtype=rtype, mu=mu, d=1, mu0=mu0,
+                           aversion=aversion, ww0=ww0, detrended=detrended, 
+                           method=method)
+        return super().set_model(ModelPipeline([mod]), verbose)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/Port_Simple.py` & `azapy-1.2.0/azapy/Generators/Port_Simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,68 @@
 import pandas as pd
 import numpy as np
 import ta
 import numbers
 import plotly.graph_objects as go
 from collections import defaultdict
 
-from azapy.util.drawdown import drawdown, max_drawdown
+from azapy.Util.drawdown import drawdown, max_drawdown
 
 def _color_negative_red(val):
     if isinstance(val, numbers.Number) and (val < 0):
         return 'color: red'
     else:
         return 'color: black'
 
 
 class Port_Simple:
     """
-    Back testing the Buy and Hold portfolio.
-
-    Methods:
-        * set_model
-        * get_port
-        * get_mktdata
-        * port_view
-        * port_view_all
-        * port_drawdown
-        * port_perf
-        * port_annual_returns
-        * port_monthly_returns
-    """
+    Backtesting the Buy and Hold portfolio.
 
+    **Attributes**
+        * `pname` : `str` - portfolio name
+        * `ww` : `pandasDataFrame` - portfolio weights at each rebalancing date
+        * `port` : `pandas.Series` - portfolio historical time-series
+       
+    The most important method is `set_model`. It must be called before any
+    other method.
+    """                  
     def __init__(self, mktdata, symb=None, sdate=None, edate=None,
                  col='adjusted', pname='Port', pcolname=None,
                  capital=100000):
         """
         Constructor
 
         Parameters
         ----------
-        `mktdata` : `pandas.DataFrame`;
+        mktdata : `pandas.DataFrame`;
             MkT data in the format "symbol", "date", "open", "high", "low",
-            "close", "volume", "adjusted", "divd", "split" (e.g. as returned
+            "close", "volume", "adjusted", "divd", "split" (e.g., as returned
             by `azapy.readMkT` function).
-        `symb` : `list`, optional;
+        symb : `list`, optional
             List of symbols for the basket components. All symbols MkT data
             should be included in `mktdata`. If set to `None` the `symb` will 
             be  set to the full set of symbols included in `mktdata`. 
             The default is `None`.
-        `sdate` : date like, optional;
+        sdate : date like, optional
             Start date for historical data. If set to `None` the `sdate` will
             be set to the earliest date in `mktdata`. The default is `None`.
-        `edate` : date like, optional;
+        edate : date like, optional
             End date for historical dates and so the simulation. Must be
             greater than `sdate`. If it is `None` then `edate` will be set
             to the latest date in `mktdata`. The default is `None`.
-        `col` : `str`, optional;
+        col : `str`, optional
             Name of column in the mktdata DataFrame that will be considered
             for portfolio aggregation. The default is 'adjusted'.
-        `pname` : `str`, optional;
+        pname : `str`, optional
             The name of the portfolio. The default is 'Port'.
-        `pcolname` : `str`, optional;
+        pcolname : `str`, optional
             Name of the portfolio price column. If it set to `None` that
             `pcolname=pname`. The default is `None`.
-        `capital` : `float`, optional;
+        capital : `float`, optional
             Initial portfolio Capital in dollars. The default is 100000.
 
         Returns
         -------
         The object.
         """
         if isinstance(mktdata, list):
@@ -101,47 +97,48 @@
             self.symb = mkt_symb
         else:
             if not all(sy in mkt_symb for sy in symb):
                 raise ValueError(f"symb list {symb} incompatible"
                                  f" with mktdata {mkt_symb}")
 
             self.symb = pd.Series(symb)
-
         # set mktdata
         self.mktdata = mktdata[(mktdata.index >= self.sdate) &
                                (mktdata.index <= self.edate) &
                                mktdata.symbol.isin(self.symb)].copy()
 
         self.col = col
         self.pname = pname
         self.pcolname = self.pname if pcolname is None else pcolname
         self.capital = capital
 
         self.ww = None
         self.port = None
+        self.nshares = None
         
         self.options = None
 
+
     def set_model(self, ww=None):
         """
         Set model parameters and evaluate the portfolio time-series.
 
         Parameters
         ----------
-        `ww` : `list` (also `numpy.array` or `pandas.Series`), optional;
+        ww : `list` (also `numpy.array` or `pandas.Series`), optional
             List of weights. If it is `pandas.Series` the index should match
-            the basket `symb`. Otherwise the weights are considered in the 
+            the basket `symb`. Otherwise, the weights are considered in the 
             `symb` order. If it is set to `None` than `ww` will be set 
             to equal weights.
             The default is `None`.
 
         Returns
         -------
-        pandas.DataFrame
-            The portfolio time-series in the format "date", "pcolname".
+        `pandas.DataFrame` : The portfolio time-series in the format "date", 
+        "pcolname".
         """
         # Validate the weights
         if ww is None:
             self.ww = pd.Series(1., index=self.symb)
         elif isinstance(ww, pd.core.series.Series):
             self.ww = ww
         else:
@@ -162,60 +159,101 @@
 
     def _port_calc(self):
         mktdata = self.mktdata.pivot(columns='symbol', values=self.col)
         divid = self.ww / mktdata.iloc[0] * self.capital
 
         self.port = pd.DataFrame(mktdata @ divid, columns = [self.pcolname])
 
+
     def get_port(self):
         """
         Returns the portfolio time-series.
 
         Returns
         -------
-        `pandas.DataFrame`
+        `pandas.DataFrame` : portfolio time-series.
         """
         return self.port.copy()
+    
+    
+    def get_weights(self, fancy=False):
+        """
+        Returns the portfolio weights at each rebalancing period.
+        
+        Parameters
+        ----------
+        fancy : Boolean, optional
+            - `False`: reports the weights in algebraic format.
+            - `True`: reports the weights in percentage rounded to 2 decimals.  
+            
+            The default is `False`.
+
+        Returns
+        -------
+        `pandas.DataFrame` : portfolio weights per symbol.
+        """
+        res = self.ww.copy()
+        if not fancy:
+            return res
+        
+        res[self.symb] = res[self.symb].round(4).abs() * 100
+        
+        return res
+    
+    def get_nshares(self):
+        """
+        Returns the number of shares held after each rolling date.
+
+        Returns
+        -------
+        `pandas.DataFrame` : number of shares per symbol.
+        """
+        if self.nshares is None:
+            return None
+        
+        return self.nshares.astype('int').copy()
+
 
     def get_mktdata(self):
         """
         Returns the actual market data used for portfolio evaluations.
 
         Returns
         -------
-        `pandas.DataFrame`
+        `pandas.DataFrame` : market data.
         """
         return self.mktdata.copy()
 
+
     def port_view(self, emas=[30, 200], bollinger=False, **opt):
         """
-        Plot the portfolio time series together with optional technical
+        Plots the portfolio time series together with optional technical
         indicators.
 
         Parameters
         ----------
-        `emas` : `list` of int, optional;
+        emas : `list` of int, optional
             List of EMA durations. The default is [30, 200].
-        `bollinger` : Boolean, optional;
+        bollinger : Boolean, optional
             If set `True` it adds the Bollinger bands. The default is `False`.    
-        `opt` : other parameters:
-            * `fancy` : Boolean, optional;
+        **opt : other optional parameters
+            * `fancy` : Boolean, optional
                 - `False` : it uses the matplotlib capabilities.
-                - `True` : it uses plotly library for interactive time-series view.
+                - `True` : it uses `plotly` library for interactive time-series view.
     
                 The default is `False`.
-            * `title` : `str`, optional; plot title. The default is `'Port performance'`.
-            * `xlabel` : `str`, optional; name of x-axis. The default is `'date'`.
-            * `ylabel` : `srt`; optional; name of y-axis. The default is `None`.
+            * `title` : `str`, optional plot title. The default is `'Port performance'`.
+            * `xlabel` : `str`, optional name of x-axis. The default is `'date'`.
+            * `ylabel` : `str`; optional name of y-axis. The default is `None`.
             * `saveto` : `str`, optional
                 The name of the file where to save the plot. The default is `None`.
+                
         Returns
         -------
-        `pandas.DataFrame`;
-            Contains the time-series included in plot.
+        `pandas.DataFrame` : Contains the time-series included in plot.
         """
         options = defaultdict(lambda: None, 
                               {'title': "Port performance",
                                'xlabel': "date", 
                                'fancy': False})
         options.update(opt)
         fancy = options['fancy']
@@ -250,49 +288,46 @@
                         xlabel=options['xlabel'], 
                         ylabel=options['ylabel']).get_figure().savefig(saveto)
                         
         return df
 
     def port_view_all(self, sdate=None, edate=None, componly=False, **opt):
         """
-        Plot the portfolio and its component time-series in a relative bases.
+        Plots the portfolio and its component time-series on a relative basis.
 
         Parameters
         ----------
-        `sdate` : date like, optional;
+        sdate : date like, optional
             Start date of plotted time-series. If it is set to `None`
             then the `sdate` is set to the earliest date in the time-series.
             The default is `None`.
-        `edate` : date like, optional;
-            End date of plotted time-series. If it set to `None` then 
-            the `edate
-            is set to the most recent date of the time-series.
+        edate : date like, optional
+            End date of plotted time-series. If it set to `None`, then 
+            the `edate` is set to the most recent date of the time-series.
             The default is `None`.
-        `componly` : Boolean, optional;
-            `True` : only the portfolio components time-series are plotted.
-
-            `False`: the portfolio and its components times-series are plotted.
+        componly : Boolean, optional
+            - `True` : only the portfolio components time-series are plotted.
+            - `False`: the portfolio and its components times-series are plotted.
 
             The default is `True`.
-        `opt` : other parameters:
-            * `fancy` : Boolean, optional;
+        **opt : other parameters
+            * `fancy` : Boolean, optional
                 - `False` : it uses the pandas plot (matplotlib) capabilities.
-                - `True` : it uses plotly library for interactive time-series view.
+                - `True` : it uses `plotly` library for interactive time-series view.
 
                 The default is `False`.
-            * `title` : `str`, optional; plot title. The default is `'Relative performance'`.
-            * `xlabel` : `str`, optional; name of x-axis. The default is `'date'`.
-            * `ylabel` : `srt`; optional; name of y-axis. The default is `None`.
-            * `saveto` : `str`, optional;
+            * `title` : `str`, optional plot title. The default is `'Relative performance'`.
+            * `xlabel` : `str`, optional name of x-axis. The default is `'date'`.
+            * `ylabel` : `str`; optional name of y-axis. The default is `None`.
+            * `saveto` : `str`, optional
                 The name of the file where to save the plot. The default is `None`.
 
         Returns
         -------
-        `pandas.DataFrame`;
-            A Data Frame containing the time-series.
+        `pandas.DataFrame` : A Data Frame containing the time-series.
         """
         options = defaultdict(lambda: None, 
                               {'title': "Relative perfromance",
                                'xlable': "date", 
                                'fancy': False})
         options.update(opt)
         fancy = options['fancy']
@@ -331,85 +366,83 @@
 
     def port_drawdown(self, top=5, fancy=False):
         """
         Computes the portfolio drawdowns.
 
         Parameters
         ----------
-        `top` : `int`, optional;
+        top : `int`, optional
             The number of largest drawdowns that will be reported.
             The default is `5`.
-        `fancy` : Boolean, optional;
-            `False` : The drawdowns values are reported in unaltered
-            algebraic format.
-
-            `True` : The drawdowns values are reported in percent
-            rounded to 2 decimals.
+        fancy : Boolean, optional
+            - `False` : The drawdowns values are reported in unaltered 
+               algebraic format.
+            - `True` : The drawdowns values are reported in percentage 
+               rounded to 2 decimals.
 
             The default is `False`.
 
         Returns
         -------
-        `panda.DataFrame`;
-            Table of drawdown events. Columns: \n
-                `'DD'` : drawdown rate \n
-                `'Date'` : recorded date of the drawdown \n
-                `'Star'` : start date of the drawdown \n
-                `'End'` : end date of the drawdown
+        `panda.DataFrame` : Table of drawdown events. 
+            Columns: 
+                - `'DD'` : drawdown rate 
+                - `'Date'` : recorded date of the drawdown
+                - `'Star'` : start date of the drawdown 
+                - `'End'` : end date of the drawdown
         """
         res = drawdown(self.port, col=self.pcolname, top=top)
         if not fancy: return res
 
         res.DD = res.DD.round(4) * 100
         return res
 
     def port_perf(self, componly=False, fancy=False):
         """
         Brief description of portfolio and its components performances
         in terms of average historical rate of returns and maximum drawdowns.
 
         Parameters
         ----------
-        `componly` : Boolean, optional;
+        componly : Boolean, optional
             If `True`, only the portfolio components maximum drawdowns
             are reported. The default is `False`.
-        `fancy` : Boolean, optional;
-            * `False` : The rate of returns and drawdown values are reported
-            in unaltered algebraic format.
+        fancy : Boolean, optional
+            - `False` : The rate of returns and drawdown values are reported
+              in unaltered algebraic format.
 
-            * `True` : The rate of returns and drawdown values are reported
-            in  percent rounded to 2 decimals.
+            - `True` : The rate of returns and drawdown values are reported
+              in  percentage rounded to 2 decimals.
 
             The default is `False`.
 
         Returns
         -------
-        `pandas.DataFrame`;
-            Performance information.
-            Columns:
-
-            * `'RR'` : rate of returns
-            * `'DD'` : maximum rate of drawdown
-            * `'Beta'` : abs(RR/DD)
-            * `'DD_date'` : recorder date of maximum drawdown
-            * `'DD_start'` : start date of maximum drawdown
-            * `'DD_end'` : end date of maximum drawdown
+        `pandas.DataFrame` : Performance information.
+            Columns
+                - `'RR'` : rate of returns
+                - `'DD'` : maximum rate of drawdown
+                - `'RoMaD'` : abs(RR/DD), Rate of Return over Maximum Drawdown
+                - `'DD_date'` : recorder date of maximum drawdown
+                - `'DD_start'` : start date of maximum drawdown
+                - `'DD_end'` : end date of maximum drawdown
+            
         """
         # local function
         def rinfo(df, col):
             rr = (df[col][-1] / df[col][0]) ** (252. / len(df)) - 1
             dv, dd, ds, de = max_drawdown(df, col=col)
 
             return pd.DataFrame([[rr, dv, np.abs(rr / dv), dd, ds, de]],
-                columns=['RR', 'DD', 'Beta', 'DD_date', 'DD_start', 'DD_end' ])
+                columns=['RR', 'DD', 'RoMaD', 'DD_date', 'DD_start', 'DD_end' ])
 
         res = self.mktdata.groupby('symbol') \
             .apply(rinfo, col=self.col) \
             .droplevel(1) \
-            .sort_values(by='Beta', ascending=False)
+            .sort_values(by='RoMaD', ascending=False)
 
         if not componly:
             res2 = rinfo(self.port, self.pcolname)
             res2.index = pd.Index([self.pname], name='symbol')
             res = pd.concat([res2, res])
 
         if not fancy:
@@ -421,33 +454,32 @@
 
     def port_annual_returns(self, withcomp=False, componly=False, fancy=False):
         """
         Portfolio annual (calendar) rates of returns.
 
         Parameters
         ----------
-        `withcomp` : Boolean, optional;
+        withcomp : Boolean, optional
             If `True`, adds the portfolio components annual returns to the
             report. The default is `False`.
-        `componly` : Boolean, optional;
+        componly : Boolean, optional
             If `True`, only the portfolio components annual returns are 
             reported.
             The flag is active only if `withcomp=True`. The default is `False`.
-        `fancy` : Boolean, optional;
-            `False` : The rates are reported in unaltered
-            algebraic format.
-
-            `True` :The rates are reported in percent rounded to 2 decimals
-            and presented is color style.
+        fancy : Boolean, optional
+            - `False` : The rates are reported in unaltered
+              algebraic format.
+            - `True` :The rates are reported in percentage rounded to 2 decimals
+              and presented is color style.
 
             The default is `False`.
 
         Returns
         -------
-        `pandas.DataFrame`
+        `pandas.DataFrame` : the report.
         """
         # local function
         def frrate(df):
             return df[-1] / df[0] - 1
 
         if withcomp:
             zz = self.mktdata.pivot(columns='symbol', values=self.col) \
@@ -469,33 +501,32 @@
     def port_monthly_returns(self, withcomp=False, componly=False,
                              fancy=False):
         """
         Portfolio monthly (calendar) rate of returns.
 
         Parameters
         ----------
-        `withcomp` : Boolean, optional;
+        withcomp : Boolean, optional
             If `True`, adds the portfolio components monthly returns to the
             report. The default is `False`.
-        `componly` : Boolean, optional;
+        componly : Boolean, optional
             If `True`, only the portfolio components monthly returns are
             reported. The flag is active only if `withcomp=True`.
             The default is `False`.
-        `fancy` : Boolean, optional;
-            `False` : The rates are reported in unaltered
-            algebraic format.
-
-            `True` :The rates are reported in percent rounded to 2 decimals
-            and presented is color style.
+        fancy : Boolean, optional
+            - `False` : The rates are reported in unaltered
+              algebraic format.
+            - `True` : The rates are reported in percentage rounded to 2 decimals
+              and presented is color style.
 
             The default is `False`.
 
         Returns
         -------
-        `pandas.DataFrame`
+        `pandas.DataFrame` : the report.
         """
         def frrate(df):
             return df[-1] / df[0] - 1
 
         # res = self.port.resample('M', convention='end').apply(frrate)
         if withcomp:
             zz = self.mktdata.pivot(columns='symbol', values=self.col) \
```

### Comparing `azapy-1.1.1/azapy/PortOpt/SDAnalyzer.py` & `azapy-1.2.0/azapy/Analyzers/SDAnalyzer.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,89 +5,126 @@
 import time
 
 from ._RiskAnalyzer import _RiskAnalyzer
 from ._solvers import _socp_solver, _tol_cholesky
 
 class SDAnalyzer(_RiskAnalyzer):
     """
-    SD - Standard Deviation based optimal portfolio strategies.
+    SD (Standard Deviation) based optimal portfolio strategies.
     
-    Methods:
-        * getWeights
-        * getRisk
-        * getPositions
-        * getRiskComp
-        * getDiversification
-        * viewForntiers
-        * set_rrate
-        * set_mktdata
-        * set_rtype
-        * set_random_seed
+    **Attributes**
+        * `status` : `int` - the computation status (`0` - success, 
+          any other value signifies an error)
+        * `ww` : `pandas.Series` -  the portfolio weights 
+        * `RR` : `float` - portfolio rate of return
+        * `risk` : `float` - portfolio SD risk
+        * `primary_risk_comp` : `list` - redundant (single element list 
+          containig SD risk value)
+        * `secondary_risk_comp` : `list` - redundant 
+          (same as `primary_risk_comp`)
+        * `sharpe` : `float` - Sharpe ration if `rtype` is set to 
+          `'Shapre'` or `'Sharpe2'` otherwise `None`. 
+        * `diverse` : `float` - diversification factor if `rtype` is set 
+          to `'Divers'` or `'MaxDivers'` otherwise `None`.
+        * `name` : `str` - portfolio name
+        
+    Note the following 2 important methods:
+        * `getWeights` : Computes the optimal portfolio weights.
+          During its computations the following class members are also set:
+          `risk`, `primery_risk_comp`, `secondary_risk_comp`, `sharpe`,  `RR`, 
+          `divers`.
+        * `getPositions` : Provides practical information regarding the 
+          portfolio rebalancing delta positions and costs.  
     """
     def __init__(self, mktdata=None, colname='adjusted', freq='Q', 
-                 hlength=3.25, calendar=None, rtype='Sharpe', method = 'ecos',
-                 name='SD'):
+                 hlength=3.25, name='SD', rtype='Sharpe', mu=None, 
+                 d=1, mu0=0., aversion=None, ww0=None, method='ecos'):
         """
         Constructor
 
         Parameters
         ----------
-        `mktdata` : `pandas.DataFrame`, optional
+        mktdata : `pandas.DataFrame`, optional
             Historic daily market data for portfolio components in the format
             returned by `azapy.mktData` function. The default is `None`.
-        `colname` : `str`, optional;
-            Name of the price column from mktdata used in the weights 
+        colname : `str`, optional
+            Name of the price column from mktdata used in the weight's 
             calibration. The default is `'adjusted'`.
-        `freq` : `str`, optional;
+        freq : `str`, optional
             Rate of return horizon. It could be 
-            `'Q'` for quarter or `'M'` for month. The default is `'Q'`.
-        `hlength` : `float`, optional;
+            `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
             History length in number of years used for calibration. A 
             fractional number will be rounded to an integer number of months.
             The default is `3.25` years.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will 
-            be set to NYSE business calendar. 
-            The default is `None`.
-        `rtype` : `str`, optional;
+        name : `str`, optional
+            Portfolio name. The default is `'SD'`.
+        rtype : `str`, optional
             Optimization type. Possible values: \n
-                `'Risk'` : optimal-risk portfolio for targeted expected rate of 
+                `'Risk'` : optimal risk portfolio for targeted expected rate of 
                 return.\n
-                `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
-                `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
+                `'Sharpe'` : optimal Sharpe portfolio - maximization solution.\n
+                `'Sharpe2'` : optimal Sharpe portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
-                `'RiskAverse'` : optimal-risk portfolio for a fixed 
+                `'RiskAverse'` : optimal risk portfolio for a fixed 
                 risk-aversion factor.\n
-                `'InvNrisk'` : optimal-risk portfolio with the same risk value 
+                `'InvNrisk'` : optimal risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
-                `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
-                `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                `'Diverse'` : optimal diversified portfolio for targeted
+                expected rate of return (max of inverse 1-Diverse).\n
+                `'Diverse2'` : optimal diversified portfolio for targeted
+                expected rate of return (min of 1-Diverse).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
-                `'InvNdiverse'` : optimal-diversified portfolio with the same
+                `'InvNdiverse'` : optimal diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
-                `'InvNdrr'` : optima- diversified portfolio with the same 
+                `'InvNdrr'` : optimal diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        `method` : `str`, optional;
+            The default is `'Sharpe'`.
+        mu : `float`, optional
+            Targeted portfolio expected rate of return. 
+            Relevant only if `rtype='Risk'` or `rtype='Divers'`.
+            The default is `None`.
+        d : `int`, optional
+            Frontier type. Active only if `rtype='Risk'`. A value of `1` will
+            trigger the evaluation of optimal portfolio along the efficient
+            frontier. Otherwise, it will find the portfolio with the lowest
+            rate of return along the inefficient portfolio frontier.
+            The default is `1`.
+        mu0 : `float`, optional
+            Risk-free rate accessible to the investor.
+            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            The default is `0`.
+        aversion : `float`, optional
+            The value of the risk-aversion coefficient.
+            Must be positive. Relevant only if `rtype='RiskAverse'`.
+            The default is `None`.
+        ww0 : `list`, `numpy.array` or `pandas.Series`, optional
+            Targeted portfolio weights. 
+            Relevant only if `rype='InvNrisk'`.
+            Its length must be equal to the number of symbols in `rrate` 
+            (mktdata). All weights must be >= 0 with sum > 0.
+            If it is a `list` or a `numpy.array` then the weights are assumed 
+            to be in order of `rrate.columns`. If it is a `pandas.Series` then 
+            the index should be compatible with the `rrate.columns` or mktdata 
+            symbols (same symbols, not necessarily in the same order).
+            If it is `None` then it will be set to equal weights.
+            The default is `None`.
+        method : `str`, optional
             Quadratic programming numerical method. Could be `'ecos'` or
             `'cvxopt'`. The default is `'ecos'`.
-        `name` : `str`, optional;
-            Object name. The default is `'SD'`.
             
         Returns
         -------
         The object.
         """
-        super().__init__(mktdata, colname, freq, hlength, calendar, 
-                         rtype, name)
+        super().__init__(mktdata, colname, freq, hlength, name,
+                         rtype, mu, d, mu0, aversion, ww0)
         
         self._set_method(method)
         
         
     def _set_method(self, method):
         self._set_qp_method(method)
```

### Comparing `azapy-1.1.1/azapy/PortOpt/SMCRAnalyzer.py` & `azapy-1.2.0/azapy/Analyzers/SMCRAnalyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,97 +5,133 @@
 
 from .CVaRAnalyzer import CVaRAnalyzer
 from ._solvers import _socp_solver
 
 
 class SMCRAnalyzer(CVaRAnalyzer):
     """
-    Mixture SMCR based optimal portfolio strategies.
+    Mixture SMCR (Second Momentum Coherent Risk)
+    based optimal portfolio strategies.
     
-    Methods:
-        * getWeights
-        * getRisk
-        * getPositions
-        * getRiskComp
-        * getDiversification
-        * viewForntiers
-        * set_rrate
-        * set_mktdata
-        * set_rtype
-        * set_random_seed
+    **Attributes**
+        * `status` : `int` - the computation status (`0` - success, 
+          any other value signifies an error)
+        * `ww` : `pandas.Series` -  the portfolio weights 
+        * `RR` : `float` - portfolio rate of return
+        * `risk` : `float` - portfolio mSMCR risk
+        * `primary_risk_comp` : `list` - SMCR components of portfolio mSMCR
+        * `secondary_risk_comp` : `list` - SMVaR values associated with SMCR
+          components
+        * `sharpe` : `float` - mSMCR-Sharpe ration if `rtype` is set to 
+          `'Shapre'` or `'Sharpe2'` otherwise `None`. 
+        * `diverse` : `float` - diversification factor if `rtype` is set 
+          to `'Divers'` or `'MaxDivers'` otherwise `None`.
+        * `name` : `str` - portfolio name
+        
+    Note the following 2 important methods:
+        * `getWeights` : Computes the optimal portfolio weights.
+          During its computations the following class members are also set:
+          `risk`, `primery_risk_comp`, `secondary_risk_comp`, `sharpe`,  `RR`, 
+          `divers`.
+        * `getPositions` : Provides practical information regarding the portfolio
+          rebalancing delta positions and costs.  
     """
-    def __init__(self, alpha=[0.9], coef=None, mktdata=None, 
-                 colname='adjusted', freq='Q', hlength=3.25, calendar=None,
-                 rtype='Sharpe', method='ecos', name='SMCR'):
+    def __init__(self, alpha=[0.9], coef=None, mktdata=None, colname='adjusted', 
+                 freq='Q', hlength=3.25, name='SMCR', rtype='Sharpe', mu=None, 
+                 d=1, mu0=0., aversion=None, ww0=None, method='ecos'):
         """
         Constructor
 
         Parameters
         ----------
-        `alpha` : `list`, optional;
-            List of distinct confidence levels. The default is `[0.9]`.
-        `coef` : list, optional;
-            List of positive mixture coefficients. Must have the same size with 
+        alpha : `list`, optional
+            List of distinct confidence levels. The default is `[0.975]`.
+        coef : `list`, optional
+            List of positive mixture coefficients. Must be the same size as 
             `alpha`. A `None` value assumes an equal weighted risk mixture.
             The vector of coefficients will be normalized to unit.
             The default is `None`.
-        `mktdata` : `pandas.DataFrame`, optional;
+        mktdata : `pandas.DataFrame`, optional
             Historic daily market data for portfolio components in the format
             returned by `azapy.mktData` function. The default is `None`.
-        `colname` : `str`, optional;
-            Name of the price column from mktdata used in the weights 
+        colname : `str`, optional
+            Name of the price column from mktdata used in the weight's 
             calibration. The default is `'adjusted'`.
-        `freq` : `str`, optional;
+        freq : `str`, optional
             Rate of return horizon. It could be 
-            `'Q'` for quarter or `'M'` for month. The default is `'Q'`.
-        `hlength` : `float`, optional;
+            `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
             History length in number of years used for calibration. A 
             fractional number will be rounded to an integer number of months.
             The default is `3.25` years.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will 
-            be set to NYSE business calendar. 
-            The default is `None`.
-        `rtype` : `str`, optional;
+        name : `str`, optional
+            Portfolio name. The default is `'SMCR'`.
+        rtype : `str`, optional
             Optimization type. Possible values: \n
-                `'Risk'` : optimal-risk portfolio for targeted expected rate of 
+                `'Risk'` : optimal risk portfolio for targeted expected rate of 
                 return.\n
-                `'Sharpe'` : Sharpe-optimal portfolio - maximization solution.\n
-                `'Sharpe2'` : Sharpe-optimal portfolio - minimization solution.\n
+                `'Sharpe'` : optimal Sharpe portfolio - maximization solution.\n
+                `'Sharpe2'` : optimal Sharpe portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
-                `'RiskAverse'` : optimal-risk portfolio for a fixed 
+                `'RiskAverse'` : optimal risk portfolio for a fixed 
                 risk-aversion factor.\n
-                `'InvNrisk'` : optimal-risk portfolio with the same risk value 
+                `'InvNrisk'` : optimal risk portfolio with the same risk value 
                 as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
-                `'Diverse'` : optimal-diversified portfolio for targeted
-                expected rate of return (maximum of inverse 1-D).\n
-                `'Diverse2'` : optimal-diversified portfolio for targeted
-                expected rate of return (minmum of 1-D).\n
+                `'Diverse'` : optimal diversified portfolio for targeted
+                expected rate of return (max of inverse 1-Diverse).\n
+                `'Diverse2'` : optimal diversified portfolio for targeted
+                expected rate of return (min of 1-Diverse).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
-                `'InvNdiverse'` : optimal-diversified portfolio with the same
+                `'InvNdiverse'` : optimal diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
                 (e.g., same as equal weighted portfolio).\n
-                `'InvNdrr'` : optima- diversified portfolio with the same 
+                `'InvNdrr'` : optimal diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
                 (e.g., same as equal weighted portfolio).\n
-            The defauls is `'Sharpe'`.
-        method : `str`, optional;
-            SOCP numerical method. 
-            Could be: `'ecos'` or `'cvxopt'`.
+            The default is `'Sharpe'`.
+        mu : `float`, optional
+            Targeted portfolio expected rate of return. 
+            Relevant only if `rtype='Risk'` or `rtype='Divers'`.
+            The default is `None`.
+        d : `int`, optional
+            Frontier type. Active only if `rtype='Risk'`. A value of `1` will
+            trigger the evaluation of optimal portfolio along the efficient
+            frontier. Otherwise, it will find the portfolio with the lowest
+            rate of return along the inefficient portfolio frontier.
+            The default is `1`.
+        mu0 : `float`, optional
+            Risk-free rate accessible to the investor.
+            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            The default is `0`.
+        aversion : `float`, optional
+            The value of the risk-aversion coefficient.
+            Must be positive. Relevant only if `rtype='RiskAverse'`.
+            The default is `None`.
+        ww0 : `list`, `numpy.array` or `pandas.Series`, optional
+            Targeted portfolio weights. 
+            Relevant only if `rype='InvNrisk'`.
+            Its length must be equal to the number of symbols in `rrate` 
+            (mktdata). All weights must be >= 0 with sum > 0.
+            If it is a `list` or a `numpy.array` then the weights are assumed 
+            to be in order of `rrate.columns`. If it is a `pandas.Series` then 
+            the index should be compatible with the `rrate.columns` or mktdata 
+            symbols (same symbols, not necessarily in the same order).
+            If it is `None` then it will be set to equal weights.
+            The default is `None`.
+        method : `str`, optional
+            SOCP numerical method. Could be: `'ecos'` or `'cvxopt'`.
             The defualt is `'ecos'`.
-        `name` : `str`, optional;
-            Object name. The default is `'SMCR'`.
             
         Returns
         -------
         The object.
         """
         super().__init__(alpha, coef, mktdata, colname, freq, hlength, 
-                         calendar, rtype, method, name)
+                         name, rtype, mu, d, mu0, aversion, ww0, method)
         
         
     def _set_method(self, method):
         self._set_socp_method(method)
 
 
     def _risk_calc(self, prate, alpha):
```

### Comparing `azapy-1.1.1/azapy/PortOpt/_RiskAnalyzer.py` & `azapy-1.2.0/azapy/Analyzers/_RiskAnalyzer.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,108 +2,141 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 from collections import defaultdict
 import copy as copy
 import warnings
 import time
 
-from azapy.MkT.MkTcalendar import NYSEgen
-
 _WW_TOL_ = 1.e-10
 _MU_ABS_TOL_ = 1.e-6
 _RISK_REL_TOL_ = 0.999999
 _RR_ABS_TOL_ = 1.e-4
 
 
 class _RiskAnalyzer:
     """
     Base class for all XXXAnalyzer classes. \n
-    All derive classes need to implement: \n
-        _risk_calc(self, prate, alpha) \n
-        _risk_min(self, d=1) \n
-        _sharpe_max(self) \n
-        _sharpe_inv_min(self) \n
-        _rr_max(self) \n
-        _risk_averse(self) \n
-        _risk_diversification(self, d=1) \n
-        _risk_inv_diversification(self, d=1) \n
-        _rr_max_diversification(self) \n
-        _set_method(self, method) \n
-
-    Methods:
+    
+    **Methods**
         * getWeights
         * getRisk
         * getPositions
         * getRiskComp
         * getDiversification
         * viewForntiers
         * set_rrate
         * set_method
         * set_mktdata
         * set_rtype
         * set_random_seed
+    **Attributes**
+        * status
+        * ww
+        * RR
+        * risk
+        * primary_risk_comp
+        * secondary_risk_comp
+        * sharpe
+        * diverse
+        * name
         
-    Public members:
-        
+    All derive classes need to implement: \n
+        _risk_calc(self, prate, alpha) \n
+        _risk_min(self, d=1) \n
+        _sharpe_max(self) \n
+        _sharpe_inv_min(self) \n
+        _rr_max(self) \n
+        _risk_averse(self) \n
+        _risk_diversification(self, d=1) \n
+        _risk_inv_diversification(self, d=1) \n
+        _rr_max_diversification(self) \n
+        _set_method(self, method) \n
     """
-
     def __init__(self, mktdata=None, colname='adjusted', freq='Q', 
-                 hlength=3.25, calendar=None, rtype='Sharpe', name=None):
+                 hlength=3.25, name=None, rtype='Sharpe', mu=None, 
+                 d=1, mu0=0., aversion=None, ww0=None):
         """
         Constructor
 
         Parameters
         ----------
-        `mktdata` : `pandas.DataFrame`, optional;
+        mktdata : `pandas.DataFrame`, optional
             Historic daily market data for portfolio components in the format
             returned by `azapy.mktData` function. The default is `None`.
-        `colname` : `str`, optional;
+        colname : `str`, optional
             Name of the price column from mktdata used in the weights
             calibration. The default is `'adjusted'`.
-        `freq` : `str`, optional;
-            Rate of return horizon in number of business day. It could be
-            `'Q'` for quarter or `'M'` for month. The default is `'Q'`.
-        `hlength` : `float`, optional;
+        freq : `str`, optional
+            Rate of return horizon. It could be 
+            `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
             History length in number of years used for calibration. A
             fractional number will be rounded to an integer number of months.
             The default is `3.25` years.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will be 
-            set to NYSE business calendar. The default is `None`.
-        `rtype` : `str`, optional;
+        name : `str`, optional
+            Portfolio name. The default value is `None`.
+        rtype : `str`, optional
             Optimization type. Possible values: \n
                 `'Risk'` : optimal risk portfolio for targeted expected rate of 
                 return.\n
                 `'Sharpe'` : optimal Sharpe portfolio - maximization solution.\n
                 `'Sharpe2'` : optimal Sharpe portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
                 `'RiskAverse'` : optimal risk portfolio for a fixed 
                 risk-aversion factor.\n
                 `'InvNrisk'` : optimal risk portfolio with the same risk value 
-                as a benchmark portfolio (e.g. same as equal weighted 
+                as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
                 `'Diverse'` : optimal diversified portfolio for targeted
                 expected rate of return (max of inverse 1-Diverse).\n
                 `'Diverse2'` : optimal diversified portfolio for targeted
                 expected rate of return (min of 1-Diverse).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
                 `'InvNdiverse'` : optimal diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
-                (e.g. same as equal weighted portfolio).\n
+                (e.g., same as equal weighted portfolio).\n
                 `'InvNdrr'` : optimal diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
-                (e.g. same as equal weighted portfolio).\n
+                (e.g., same as equal weighted portfolio).\n
             The default is `'Sharpe'`.
-        `name` : `str`, optional;
-            Object name. Deafult value is `None`.
+        mu : `float`, optional
+            Targeted portfolio expected rate of return. 
+            Relevant only if `rtype='Risk'` or `rtype='Divers'`.
+            The default is `None`.
+        d : `int`, optional
+            Frontier type. Active only if `rtype='Risk'`. A value of `1` will
+            trigger the evaluation of optimal portfolio along the efficient
+            frontier. Otherwise, it will find the portfolio with the lowest
+            rate of return along the inefficient portfolio frontier.
+            The default is `1`.
+        mu0 : `float`, optional
+            Risk-free rate accessible to the investor.
+            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            The default is `0`.
+        aversion : `float`, optional
+            The value of the risk-aversion coefficient.
+            Must be positive. Relevant only if `rtype='RiskAverse'`.
+            The default is `None`.
+        ww0 : `list`, `numpy.array` or `pandas.Series`, optional
+            Targeted portfolio weights. 
+            Relevant only if `rype='InvNrisk'`.
+            Its length must be equal to the number of symbols in `rrate` 
+            (mktdata). All weights must be >= 0 with sum > 0.
+            If it is a `list` or a `numpy.array` then the weights are assumed 
+            to be in order of `rrate.columns`. If it is a `pandas.Series` then 
+            the index should be compatible with the `rrate.columns` or mktdata 
+            symbols (same symbols, not necessarily in the same order).
+            If it is `None` then it will be set to equal weights.
+            The default is `None`.
 
         Returns
         -------
         The object.
         """
+        self._ptype_ = 'Optimizer'
         self.ww = None
         self.status = None
 
         self.last_data = None
         self.rrate = None
         self.nn = None
         self.mm = None
@@ -120,34 +153,42 @@
         self.sharpe = None
         self.RR = None
         self.diverse = None
         self.time_level1 = None
         self.time_level2 = None
         self.time_level3 = None
 
-        self.rtype = None
         self.rng = None
-        self.method = None
-        
-        self.methods = None
-        self.rtypes = None
-        self.name = None
-        
+ 
         self.risk_comp = None
         self._flag_risk_comp_calc = False
         self._status_risk_comp_calc = None
+       
+        self.name = name
         
-        self.set_rtype(rtype)
+        self.freq = None
+        self.hlength = None
         
-        self.name = name
-
-        if mktdata is not None:
-            self.set_mktdata(mktdata, colname, freq, hlength)
+        self.set_mktdata(mktdata, colname, freq, hlength)
         self.set_random_seed()
         
+        self.name = None
+        
+        self.rtypes = None
+        self.rtype = None
+        self._mu = None
+        self._d = None
+        self._mu0 = None
+        self._aversion = None
+        self._ww0 = None
+        
+        self.set_rtype(rtype, mu, d, mu0, aversion, ww0)
+        
+        self.methods = None
+        
         self.verbose = False
         
         
     def _reset_output(self):
         self.status = None
         self.ww = None
         self.risk = None
@@ -158,123 +199,132 @@
         self.diverse = None
         self.time_level1 = None
         self.time_level2 = None
         self.time_level3 = None
 
         
     def getWeights(self, rtype=None, mu=None, d=1, mu0=0., aversion=None,
-                   ww0=None, rrate=None, verbose=False):  
+                   ww0=None, mktdata=None, **params):  
         """
         Computes the optimal portfolio weights.
 
         Parameters
         ----------
-        `rtype` : `str`, optional;
+        rtype : `str`, optional
             Optimization type. If is not `None` it will overwrite the value
             set by the constructor. The default is `None`.
             Other possible values: \n
                 `'Risk'` : optimal risk portfolio for targeted expected rate of 
                 return.\n
                 `'Sharpe'` : optimal Sharpe portfolio - maximization solution.\n
                 `'Sharpe2'` : optimal Sharpe portfolio - minimization solution.\n
                 `'MinRisk'` : minimum risk portfolio.\n
                 `'RiskAverse'` : optimal risk portfolio for a fixed 
                 risk-aversion factor.\n
                 `'InvNrisk'` : optimal risk portfolio with the same risk value 
-                as a benchmark portfolio (e.g. same as equal weighted 
+                as a benchmark portfolio (e.g., same as equal weighted 
                 portfolio).\n
                 `'Diverse'` : optimal diversified portfolio for targeted
                 expected rate of return (max of inverse 1-Diverse).\n
                 `'Diverse2'` : optimal diversified portfolio for targeted
                 expected rate of return (min of 1-Diverse).\n
                 `'MaxDiverse'` : maximum diversified portfolio.\n
                 `'InvNdiverse'` : optimal diversified portfolio with the same
                 diversification factor as a benchmark portfolio 
-                (e.g. same as equal weighted portfolio).\n
+                (e.g., same as equal weighted portfolio).\n
                 `'InvNdrr'` : optimal diversified portfolio with the same 
                 expected rate of return as a benchmark portfolio
-                (e.g. same as equal weighted portfolio).\n
-        `mu` : `float`, optional;
+                (e.g., same as equal weighted portfolio).\n
+        mu : `float`, optional
             Targeted portfolio expected rate of return. 
-            Relevant only if `rtype` is equalt to `'Risk'` or `'Divers'`.
+            Relevant only if `rtype='Risk'` or `rtype='Divers'`.
             The default is `None`.
-        `d` : `int`, optional;
+        d : `int`, optional
             Frontier type. Active only if `rtype='Risk'`. A value of `1` will
             trigger the evaluation of optimal portfolio along the efficient
             frontier. Otherwise, it will find the portfolio with the lowest
             rate of return along the inefficient portfolio frontier.
             The default is `1`.
-        `mu0` : `float`, optional;
+        mu0 : `float`, optional
             Risk-free rate accessible to the investor.
             Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
             The default is `0`.
-        `aversion` : `float`, optional;
+        aversion : `float`, optional
             The value of the risk-aversion coefficient.
             Must be positive. Relevant only if `rtype='RiskAverse'`.
             The default is `None`.
-        `ww0` : `list`, `numpy.array` or `pandas.Series`, optional;
+        ww0 : `list`, `numpy.array` or `pandas.Series`, optional
             Targeted portfolio weights. 
             Relevant only if `rype='InvNrisk'`.
             Its length must be equal to the number of symbols in `rrate` 
             (mktdata). All weights must be >= 0 with sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
-            symbols (same symbols, not necessary in the same order).
+            symbols (same symbols, not necessarily in the same order).
             If it is `None` then it will be set to equal weights.
             The default is `None`.
-        `rrate` : `pandas.DataFrame`, optional;
-            The portfolio components historical rates of returns.
-            If it is not `None`, it will overwrite the `rrate` computed in the
-            constructor from mktdata. The default is `None`. 
-        `verbose` : Boolean, optiona;
-            If it set to `True` then it will print messages when the optimal
-            portfolio degenerates to a single asset portfolio as a limited 
-            case. 
-            The default is `False`.
+        mktdata : `pandas.DataFrame`, optional
+            The portfolio components historical, prices or rates of return, see
+            `'pclose'` definition below.
+            If it is not `None`, it will overwrite the set of historical rates
+            of return computed in the constructor from `'mktdata'`. 
+            The default is `None`. 
+        **params : other optional paramters
+            Most common: \n
+            `verbose` : Boolean, optional
+                If it set to `True`, then it will print a message when 
+                the optimal portfolio degenerates to a single asset.
+                The default is `False`.
+            `pclose` : Boolean, optional
+                If it is absent then the `mktdata` is considered to contain 
+                rates of return, with columns the asset symbols and indexed 
+                by the observation dates, \n
+                `True` : assumes `mktdata` contains closing prices only, 
+                with columns the asset symbols and indexed by the 
+                observation dates, \n
+                `False` : assumes `mktdata` is in the usual format
+                returned by `azapy.mktData` function.
 
-       Returns
+        Returns
         -------
-        `pandas.Series` with portfolio weights.
+        `pandas.Series` : portfolio weights per symbol.
         """
         toc = time.perf_counter()
         self._reset_output()
-        self.verbose = verbose
- 
-        d = 1 if d == 1 else -1
-
-        if rrate is not None:
-            self.set_rrate(rrate)
-            
-        if not rtype is None:
-            self.set_rtype(rtype)
+        self.verbose = params['verbose'] if 'verbose' in params.keys() else self.verbose
+        if 'pclose' in params.keys():
+            self.set_mktdata(mktdata, pclose=params['pclose'])
+        else:
+            self.set_rrate(mktdata)
+        self.set_rtype(rtype, mu, d, mu0, aversion, ww0)
             
         # calc - grand dispatch 
         if self.rtype == "Risk":
-            self._calc_Risk(mu, d)
+            self._calc_Risk(self._mu, self._d)
         elif self.rtype == 'Sharpe':           
-            self._calc_Sharpe(mu0)
+            self._calc_Sharpe(self._mu0)
         elif self.rtype == 'Sharpe2':          
-            self._calc_Sharpe2(mu0)
+            self._calc_Sharpe2(self._mu0)
         elif self.rtype == "MinRisk":
             self._calc_MinRisk()
         elif self.rtype == "InvNrisk":    
-            self._calc_InvNrisk(ww0)
+            self._calc_InvNrisk(self._ww0)
         elif self.rtype == "RiskAverse":   
-            self._calc_RiskAverse(aversion) 
+            self._calc_RiskAverse(self._aversion) 
         elif self.rtype == "Diverse2":
-            self._calc_Diverse2(mu, d)
+            self._calc_Diverse2(self._mu, self._d)
         elif self.rtype == "Diverse":
-            self._calc_Diverse(mu, d)
+            self._calc_Diverse(self._mu, self._d)
         elif self.rtype == "MaxDiverse":  
             self._calc_MaxDiverse()
         elif self.rtype == "InvNdiverse":
-            self._calc_InvNdiverse(ww0)
+            self._calc_InvNdiverse(self._ww0)
         elif self.rtype == "InvNdrr":
-            self._calc_InvNdrr(ww0)
+            self._calc_InvNdrr(self._ww0)
         else:
             raise ValueError("you should not be here - ever")
 
         if self.status != 0:
             warnings.warn(f"Warning: {self.rtype} on {self.rrate.index[-1]} "
                           f"status {self.status}")
         else:
@@ -283,71 +333,71 @@
             
         self.time_level1 = time.perf_counter() - toc
         
         return self.ww
     
     
     def _calc_Risk(self, mu, d):
-        mu_max = self.muk.max()
-        mu_min = self.muk.min()
+        mu_max = self.muk.max(numeric_only=True)
+        mu_min = self.muk.min(numeric_only=True)
         if mu is None:
             raise ValueError("for rtype='Risk' mu must have a value")
         elif d == 1 and mu - mu_max > -np.abs(mu_max) * _MU_ABS_TOL_:
             self._single_asset_port('max')
             if self.verbose:
                 print(f"rtype 'Risk' for mu {mu} for {self.name} on "
-                      f"{self.rrate.index[-1]}, defaulted "
-                      f"to single portfolio [{self.muk.idxmax()}]")
+                      f"{self.rrate.index[-1]}, defaulted to single "
+                      f"portfolio [{self.muk.idxmax()}]")
         elif d == -1 and mu - mu_min < np.abs(mu_min) * _MU_ABS_TOL_:
             self._single_asset_port('min')
             if self.verbose:
                 print(f"rtype 'Risk' for mu {mu} for {self.name} on "
-                      f"{self.rrate.index[-1]}, defaulted "
-                      f"to single portfolio [{self.muk.idxmin()}]")
+                      f"{self.rrate.index[-1]}, defaulted to single "
+                      f"portfolio [{self.muk.idxmin()}]")
         else:
             self.mu = mu
             self._risk_min(d=d)
             
             
     def _calc_Sharpe(self, mu0):
-        mu_max = self.muk.max()
+        mu_max = self.muk.max(numeric_only=True)
         if mu0 is None:
             raise ValueError("for rtype='Sharpe' mu0 must have a value")
         if mu0 - mu_max >= -np.abs(mu_max) * _MU_ABS_TOL_:
             self._single_asset_port('max')
             if self.status == 0:
                 self.sharpe = (self.RR - mu0) / self.risk
                 if self.verbose:
                     print(f"rtype 'Sharpe' for mu0 {mu0} for {self.name} on "
-                          f"{self.rrate.index[-1]}, defaulted "
-                          f"to single portfolio [{self.muk.idxmax()}]")
+                          f"{self.rrate.index[-1]}, defaulted to single "
+                          f"portfolio [{self.muk.idxmax()}]")
         else:
             self.mu = mu0
             self._sharpe_max()
             
             
     def _calc_Sharpe2(self, mu0):
-        mu_max = self.muk.max()
+        mu_max = self.muk.max(numeric_only=True)
         if mu0 is None:
             raise ValueError("for rtype='Sharpe' mu0 must have a value")
         if mu0 - mu_max >= -np.abs(mu_max) * _MU_ABS_TOL_:
             self._single_asset_port('max')
             if self.status == 0:
                 self.sharpe = (self.RR - mu0) / self.risk
                 if self.verbose:
                     print(f"rtype 'Sharpe2' for mu0 {mu0} for {self.name} on "
-                          f"{self.rrate.index[-1]}, defaulted "
-                          f"to single portfolio [{self.muk.idxmax()}]")
+                          f"{self.rrate.index[-1]}, defaulted to single "
+                          f"portfolio [{self.muk.idxmax()}]")
         else:
             self.mu = mu0
             self._sharpe_inv_min() 
             
             
     def _calc_MinRisk(self):
-        self._calc_Risk(self.muk.min(), d=1)
+        self._calc_Risk(self.muk.min(numeric_only=True), d=1)
         
         
     def _calc_InvNrisk(self, ww0):
         if ww0 is None:
             ww = np.full(len(self.rrate.columns), 
                          1/len(self.rrate.columns))
         else:
@@ -387,63 +437,63 @@
             raise ValueError("aversion must be positive (>0)")
             
         self.Lambda = aversion
         self._risk_averse()
         
         
     def _calc_Diverse(self, mu, d):
-        mu_max = self.muk.max()
-        mu_min = self.muk.min()
+        mu_max = self.muk.max(numeric_only=True)
+        mu_min = self.muk.min(numeric_only=True)
         if mu is None:
             raise ValueError("for rtype='Diverse' mu must have a value")
         elif d == 1 and mu - mu_max > -np.abs(mu_max) * _MU_ABS_TOL_:
             self._single_asset_port('max')
             if self.verbose:
                 print(f"rtype 'Diverse' for mu {mu} for {self.name} on "
-                      f"{self.rrate.index[-1]}, defaulted "
-                      f"to single portfolio [{self.muk.idxmax()}]")
+                      f"{self.rrate.index[-1]}, defaulted to single "
+                      f"portfolio [{self.muk.idxmax()}]")
         elif d == -1 and mu - mu_min < np.abs(mu_min) * _MU_ABS_TOL_:
             self._single_asset_port('min')
             if self.verbose:
                 print(f"rtype 'Diverse' for mu {mu} for {self.name} on "
-                      f"{self.rrate.index[-1]}, defaulted "
-                      f"to single portfolio [{self.muk.idxmin()}]")
+                      f"{self.rrate.index[-1]}, defaulted to single "
+                      f"portfolio [{self.muk.idxmin()}]")
         else:
             self.mu = mu
             self.getRiskComp()
             if self.status == 0:
                 self._risk_inv_diversification(d=d)
                 
                 
     def _calc_Diverse2(self, mu, d):
-        mu_max = self.muk.max()
-        mu_min = self.muk.min()
+        mu_max = self.muk.max(numeric_only=True)
+        mu_min = self.muk.min(numeric_only=True)
         if mu is None:
             raise ValueError("for rtype='Diverse2' mu must have a value")
         elif d == 1 and mu - mu_max > -np.abs(mu_max) * _MU_ABS_TOL_:
             self._single_asset_port('max')
             if self.verbose:
                 print(f"rtype 'Diverse2' for mu {mu} for {self.name} on "
-                      f"{self.rrate.index[-1]}, defaulted "
-                      f"to single portfolio [{self.muk.idxmax()}]")
+                      f"{self.rrate.index[-1]}, defaulted to single "
+                      f"portfolio [{self.muk.idxmax()}]")
         elif d == -1 and mu - mu_min < np.abs(mu_min) * _MU_ABS_TOL_:
             self._single_asset_port('min')
             if self.verbose:
                 print(f"rtype 'Diverse2' for mu {mu} for {self.name} on "
-                      f"{self.rrate.index[-1]}, defaulted "
-                      f"to single portfolio [{self.muk.idxmin()}]")
+                      f"{self.rrate.index[-1]}, defaulted to single "
+                      f"portfolio [{self.muk.idxmin()}]")
         else:
             self.mu = mu
             self.getRiskComp()
             if self.status == 0:
                 self._risk_diversification(d=d)
                 
                 
     def _calc_MaxDiverse(self):
-        self._calc_Diverse(self.muk.min(), d=1)
+        self._calc_Diverse(self.muk.min(numeric_only=True), d=1)
         
         
     def _calc_InvNdiverse(self, ww0):
         if ww0 is None:
             ww = np.full(len(self.rrate.columns), 
                          1/len(self.rrate.columns))
         else:
@@ -491,38 +541,35 @@
     def getRisk(self, ww, rrate=None):
         """
         Returns the value of the dispersion (risk) measure for a give 
         portfolio.
 
         Parameters
         ----------
-        `ww` : `list`, `numpy.array` or `pandas.Series`;
+        ww : `list`, `numpy.array` or `pandas.Series`
             Portfolio weights. Its length must be equal to the number of
             symbols in `rrate` (mktdata). All weights must be >=0 with 
             sum > 0.
             If it is a `list` or a `numpy.array` then the weights are assumed 
             to be in order of `rrate.columns`. If it is a `pandas.Series` than 
             the index should be compatible with the `rrate.columns` or mktdata 
-            symbols (not necessary in the same order).
-        `rrate` : `pandas.DataFrame`, optional;
+            symbols (not necessarily in the same order).
+        rrate : `pandas.DataFrame`, optional
             Contains the portfolio components historical
-            rates of returns. If it is not `None`, it will overwrite the
-            `rrate` computed in the constructor from `mktdata`.
+            rates of return. If it is not `None`, it will overwrite the
+            rates of return computed in the constructor from `mktdata`.
             The default is `None`.
 
         Returns
         -------
-        `float`
-            The dispersion (risk) measure value.
+        `float` : The dispersion (risk) measure value.
         """
         self._reset_output()
         toc = time.perf_counter()
-        
-        if rrate is not None:
-            self.set_rrate(rrate)
+        self.set_rrate(rrate)
 
         if isinstance(ww, pd.core.series.Series):
             ww = ww[self.rrate.columns]
         w = np.array(ww)
         if any(w < 0.):
             raise ValueError("All ww must be non-negative")
         sw = w.sum()
@@ -549,119 +596,96 @@
         self.RR = np.dot(w, self.muk)
         self.ww = w
         self.time_level1 = time.perf_counter() - toc
         
         return self.risk
 
         
-    def getPositions(self, nshares=None, cash=0, ww=None, rtype=None, 
-                     mu=None, mu0=0., aversion=None, ww0=None, ):
+    def getPositions(self, nshares=None, cash=0, ww=None, verbose=True):
         """
         Computes the rebalanced number of shares.
 
         Parameters
         ----------
-        `nshares` : `panda.Series`, optional;
+        nshares : `panda.Series`, optional
             Initial number of shares per portfolio component.
             A missing component
             entry will be considered 0. A `None` value assumes that all
             components entries are 0. The name of the components must be
             present in the mrkdata. The default is `None`.
-        `cash` : `float`, optional;
+        cash : `float`, optional
             Additional cash to be added to the capital. A
             negative entry assumes a reduction in the total capital
             available for rebalance. The total capital cannot be < 0.
             The default is 0. 
-        `ww` : `panda.Series`, optional;
+        ww : `panda.Series`, optional
             External overwrite portfolio weights. 
             If it not set to `None` these
             weights will overwrite the calibration results.
             The default is `None`. 
-        `rtype` : `str`, optional;
-            Optimization type. If is not `None` it will overwrite the value
-            set by the constructor. The default is `None`.
-        `mu` : `float`, optional
-            Targeted portfolio expected rate of return. 
-            Relevant only if `rtype='Risk'` and `rtype='Divers'`.
-            The default is `None`.
-        `mu0` : `float`, optional;
-            Risk-free rate accessible to the investor.
-            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
-            The default is `0`.
-        `aversion` : `float`, optional;
-            The value of the risk-aversion coefficient.
-            Must be positive. Relevant only if `rtype='RiskAvers'`.
-            The default is `None`.
-        `ww0` : list (also `numpy.array` or `pandas.Series`), optional;
-            Targeted portfolio weights 
-            Relevant only if `rype='InvNrisk'`.
-            Its length must be equal to the number of
-            symbols in `rrate` (mktdata). 
-            All weights must be >= 0 with sum > 0.
-            If it is a `list` or a `numpy.array` then the weights are assumed to
-            be in order of `rrate.columns`. If it is a `pandas.Series` then the 
-            index should be compatible with the `rrate.columns` or mktdata 
-            symbols (same symbols, not necessary in the same order).
-            If it is `None` then it will be set to equal weights.
-            The default is `None`.
-
+        verbose : Boolean, optional
+            Is it set to `True` the function prints the closing prices date.
+            The default is `True`.
+        
         Returns
         -------
-        `pandas.DataFrame`: the rolling information.
+        `pandas.DataFrame` : the rolling information.
 
         Columns:
 
-            - `"old_nsh"` :
+            - `'old_nsh'` :
                 initial number of shares per portfolio component and
                 the additional cash. These are input values.
-            - `"new_nsh"` :
+            - `'new_nsh'` :
                 the new number of shares per component plus the residual
                 cash (due to the rounding to an integer number of shares).
                 A negative entry means that the investor needs to add more
                 cash to cover for the roundup shortfall.
                 It has a small value.
-            - `"diff_nsh"` :
-                the number of shares that needs to be both/sold in order
-                to rebalance the portfolio positions.
-            - `"weights"` :
+            - `'diff_nsh'` :
+                number of shares (buy/sale) needed to rebalance the 
+                portfolio.
+            - `'weights'` :
                 portfolio weights used for rebalancing. The cash entry is
                 the new portfolio value (invested capital).
-            - `"prices"` :
+            - `'prices'` :
                 the share prices used for rebalances evaluations.
 
-        Note: Since the prices are closing prices, the rebalance can be
-        computed after the market close and before the 
-        trading execution (next day). 
-        Additional cash slippage may occur due
-        to share price differential between the previous day closing and
-        execution time.
+            Note: Since the prices are closing prices, the rebalance can be
+            computed after the market close and before the 
+            trading execution (next day). 
+            Additional cash slippage may occur due
+            to share price differential between the previous day closing and
+            execution time.
         """
-       
-        if rtype is not None:
-            self.set_rtype(rtype)
-
         ns = pd.Series(0, index=self.rrate.columns)
         if nshares is not None:
             ns = ns.add(nshares, fill_value=0)
 
         if len(self.rrate.columns) != len(ns):
             raise ValueError("nshares must be a subset " + \
                              f"of {self.rrate.columns}")
 
+        if self.last_data is None:
+            raise ValueError("The obj was not set with mktdata")
+            
+        if verbose:
+            print(f"Use closing prices as of {self.last_data.name}")
+            
         pp = self.last_data[self.rrate.columns.to_list()]
 
         cap = ns.dot(pp) + cash
         if ww is None:
-            ww = self.getWeights(rtype=rtype, mu=mu, mu0=mu0, ww0=ww0, 
-                                 aversion=aversion)
+            ww = self.getWeights()
         else:
             wwp = pd.Series(0, index=self.rrate.columns)
             ww = wwp.add(ww, fill_value=0)
-            if len(self.rrate.columns) == len(ns):
-                raise ValueError(f"ww must be among {self.rrate.columns}")
+            if len(self.rrate.columns) != len(ns):
+                raise ValueError("ww: wrong component names - "
+                                 f"must be among {self.rrate.columns}")
 
         newns = (ww / pp * cap).round(0)
         newcash = cap - newns.dot(pp)
 
         ns['cash'] = cash
         newns['cash'] = newcash
         ww['cash'] = cap - newcash
@@ -674,240 +698,336 @@
                             'prices': pp})
 
         return res
 
 
     def set_rrate(self, rrate):
         """
-        Sets portfolio components historical rates of returns.
+        Sets portfolio components historical rates of return.
         It will overwrite the value computed by the constructor from mktdata.
 
         Parameters
         ----------
-        `rrate` : `pandas.DataFrame`;
-            Portfolio components historical rates of returns. The
-            columns are: "date", "symbol1", "symbol2", etc.
+        rrate : `pandas.DataFrame`
+            Portfolio components historical rates of return. The
+            columns are asset symbols and indexed by observation dates.
             
         Returns
         -------
-        None
+        `None`
         """
+        if rrate is None:
+            # noting to do
+            return
+        
         self._flag_risk_comp_calc = False
         self.nn, self.mm = rrate.shape
-        self.muk = rrate.mean()
+        self.muk = rrate.mean(numeric_only=True)
         self.rrate = rrate - self.muk
 
 
-    def set_mktdata(self, mktdata, colname='adjusted',
-                    freq='Q', hlength=3.25, calendar=None):
+    def set_mktdata(self, mktdata, colname=None, freq=None, hlength=None, 
+                    pclose=False):
         """
         Sets historical market data. It will overwrite the choice made in the
         constructor.
 
         Parameters
         ----------
-        `mktdata` : `pandas.DataFrame`;
+        mktdata : `pandas.DataFrame`
             Historic daily market data for portfolio components in the format
             returned by `azapy.mktData` function.
-        `colname` : `str`, optional;
-            Name of the price column from mktdata used in the weights
+        colname : `str`, optional
+            Name of the price column from mktdata used in the weight’s
             calibration. The default is 'adjusted'.
-        `freq` : `str`, optional;
-            Rate of returns horizon in number of business day. It could be
-            'Q' for quarter or 'M' for month. The default is 'Q'.
-        `hlength` : `float`, optional;
+        freq : `str`, optional
+            Rate of return horizon. It could be 
+            `'Q'` for a quarter or `'M'` for a month. The default is `'Q'`.
+        hlength : `float`, optional
             History length in number of years used for calibration. A
             fractional number will be rounded to an integer number of months.
             The default is `3.25`.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will be 
-            set to NYSE business calendar.
-            The default is `None`.
+        pclose : Boolena, optiona; \n
+            `True` : assumes `mktdata` contains closing prices only, 
+            with columns the asset symbols and indexed by the 
+            observation dates, \n
+            `False` : assumes `mktdata` is in the usual format
+            returned by `azapy.mktData` function.
+            
 
         Returns
         -------
         `None`
         """
+        if colname is None:
+            if self.colname is None:
+                raise ValueError("Unspecified price colum (colname).")
+        else:
+            self.colname = colname
+        
+        if freq is None:
+            if self.freq is None:
+                raise ValueError("freq not set - it must be 'Q' or 'M'.")
+        elif freq in ['Q', 'M']:
+            self.freq = freq
+        else:
+            raise ValueError(f"wrrong value for freq: {freq}" 
+                              " - it must be 'Q' or 'M'.")
+            
+        if hlength is None:
+            if self.hlength is None:
+                raise ValueError("hlength must be set to a positive "
+                                 "value - e.g. 1")
+        else:
+            self.hlength = hlength
+
         if mktdata is None:
+            # nothing else to do
             return
+        
+        periods = 63 if self.freq == 'Q' else 21
+        idx_sdate = int(-np.round(self.hlength * 12) * 21)
 
-        self.mktdata = mktdata
-
-        periods = 63 if freq == 'Q' else 21
-
-        if calendar is None:
-            calendar = NYSEgen()
-
-        edate = mktdata.index[-1]
-        sdate = edate - pd.offsets.DateOffset(months=round(hlength * 12, 0))
-        sdate = np.busday_offset(sdate.date(),
-                                 0, roll='backward',  busdaycal=calendar)
-        rrate = mktdata.pivot(columns='symbol', values=colname)[sdate:]
-        self.last_data = rrate.iloc[-1]
-        rrate = rrate.pct_change(periods=periods).dropna()
-
+        if pclose == False:
+            if self.colname not in mktdata.columns:
+                raise ValueError(f"colname: {colname} not in mktdata.columns")
+            mktdata = mktdata.pivot(columns='symbol', 
+                                  values=self.colname)
+            
+        if mktdata.shape[0] < -idx_sdate:
+            sdate =  mktdata.index[0]
+            warnings.warn(f"Too short history for hlength {self.hlength}"
+                          f" set sdate to {sdate} with"
+                          f" {mktdata.shape[0]} hist observations"
+                          f" instead of {-idx_sdate}")
+        else:
+            sdate = mktdata.index[idx_sdate]
+        
+        mktdata = mktdata[sdate:]
+            
+        self.last_data = mktdata.iloc[-1]
+        rrate = mktdata.pct_change(periods=periods).dropna()
         self.set_rrate(rrate)
 
 
-    def set_rtype(self, rtype):
+    def set_rtype(self, rtype=None, mu=None, d=1, mu0=0., aversion=None, 
+                  ww0=None):
         """
         Sets the optimization type. It will overwrite the value set in the
         constructor.
 
         Parameters
         ----------
-        `rtype` : `str`;
-            Optimization type.
+        rtype : `str`, optional
+            Optimization type. Possible values: \n
+                `'Risk'` : optimal risk portfolio for targeted expected rate of 
+                return.\n
+                `'Sharpe'` : optimal Sharpe portfolio - maximization solution.\n
+                `'Sharpe2'` : optimal Sharpe portfolio - minimization solution.\n
+                `'MinRisk'` : minimum risk portfolio.\n
+                `'RiskAverse'` : optimal risk portfolio for a fixed 
+                risk-aversion factor.\n
+                `'InvNrisk'` : optimal risk portfolio with the same risk value 
+                as a benchmark portfolio (e.g., same as equal weighted 
+                portfolio).\n
+                `'Diverse'` : optimal diversified portfolio for targeted
+                expected rate of return (max of inverse 1-Diverse).\n
+                `'Diverse2'` : optimal diversified portfolio for targeted
+                expected rate of return (min of 1-Diverse).\n
+                `'MaxDiverse'` : maximum diversified portfolio.\n
+                `'InvNdiverse'` : optimal diversified portfolio with the same
+                diversification factor as a benchmark portfolio 
+                (e.g., same as equal weighted portfolio).\n
+                `'InvNdrr'` : optimal diversified portfolio with the same 
+                expected rate of return as a benchmark portfolio
+                (e.g., same as equal weighted portfolio).\n
+            The default is `'Sharpe'`.
+        mu : `float`, optional
+            Targeted portfolio expected rate of return. 
+            Relevant only if `rtype='Risk'` or `rtype='Divers'`.
+            The default is `None`.
+        d : `int`, optional
+            Frontier type. Active only if `rtype='Risk'`. A value of `1` will
+            trigger the evaluation of optimal portfolio along the efficient
+            frontier. Otherwise, it will find the portfolio with the lowest
+            rate of return along the inefficient portfolio frontier.
+            The default is `1`.
+        mu0 : `float`, optional
+            Risk-free rate accessible to the investor.
+            Relevant only if `rype='Sharpe'` or `rtype='Sharpe2'`.
+            The default is `0`.
+        aversion : `float`, optional
+            The value of the risk-aversion coefficient.
+            Must be positive. Relevant only if `rtype='RiskAverse'`.
+            The default is `None`.
+        ww0 : `list`, `numpy.array` or `pandas.Series`, optional
+            Targeted portfolio weights. 
+            Relevant only if `rype='InvNrisk'`.
+            Its length must be equal to the number of symbols in `rrate` 
+            (mktdata). All weights must be >= 0 with sum > 0.
+            If it is a `list` or a `numpy.array` then the weights are assumed 
+            to be in order of `rrate.columns`. If it is a `pandas.Series` then 
+            the index should be compatible with the `rrate.columns` or mktdata 
+            symbols (same symbols, not necessarily in the same order).
+            If it is `None` then it will be set to equal weights.
+            The default is `None`.
             
         Returns
         -------
         `None`
         """
+        if rtype is None:
+            # noting else to do
+            return
+        
         self.rtypes = ['Risk', 'MinRisk', 'Sharpe', 'Sharpe2', 'RiskAverse',
                        'InvNrisk', 'Diverse', 'Diverse2', 'MaxDiverse', 
                        'InvNdiverse', 'InvNdrr']
-
         if not rtype in self.rtypes:
             raise ValueError(f"rtype (value {rtype}) must be "
                              f"one of {self.rtypes}")
         self.rtype = rtype
+        self._mu = mu
+        self._d = 1 if d == 1 else -1
+        self._mu0 = mu0
+        self._aversion = aversion
+        self._ww0 = ww0
 
 
     def viewFrontiers(self, minrisk=True, efficient=20, inefficient=20, 
                       sharpe=True, musharpe=0., maxdiverse=False, 
                       diverse_efficient=0, diverse_inefficient=0, invN=True, 
                       invNrisk=True, invNdiverse=False, invNdrr=False,
                       component=True, randomport=20, addport=None, 
                       fig_type='RR_risk', **opt):
         """
         Computes the elements of the portfolio frontiers.
 
         Parameters
         ----------
-        `minrisk` : Boolean, optional;
+        minrisk : Boolean, optional
             If it is `True` then the minimum risk portfolio will be visible. 
             The default is `True`.
-        `efficient` : `int`, optional;
+        efficient : `int`, optional
             Number of points along the efficient risk frontier 
             (equally spaced along the rate of return axis). 
             The default is `20`.
-        `inefficient` : `int`, optional;
+        inefficient : `int`, optional
             Number of points along the inefficient risk frontier 
             (equally spaced along the rate of returns axis). 
             The default is `20`.
-        `sharpe` : Boolean, optional;
+        sharpe : Boolean, optional
             If it is `True` then the maximum Sharpe portfolio will be visible. 
             The default is `True`.
-        `musharpe` : `float`, optional;
+        musharpe : `float`, optional
             Risk-free rate value used in the evaluation of
             generalized Sharpe ratio. The default is `0`.
-        `maxdiverse`: Boolean, optional;
+        maxdiverse : Boolean, optional
             If it is `True` then the maximum diversified portfolio will be 
             visible. The default is `True`.
-        `diverse_efficient`: `int`, optional;
+        diverse_efficient : `int`, optional
             Number of points along the efficient diversification frontier
             (equally spaced along the rate of return axis).
             The default is `20`.
-        `diverse_inefficient`: `int`, optional;
+        diverse_inefficient : `int`, optional
             Number of points along the inefficient diversification frontier
             (equally spaced along the rate of return axis).
             The default is `20`.
-        `invN` : Boolean, optional;
+        invN : Boolean, optional
             If it is `True`, then the equal weighted portfolio and the optimal 
             portfolio with the same risk value are added to
             the plot. The default is `True`.
-        `invNrisk` : Boolena, optional;
+        invNrisk : Boolena, optional
             If it is `True`, then the efficient risk portfolio with same risk 
             as equal weighth portfolio is added to the plot.
             The defualt is `False`.
-        `invNdiverse` : Boolean, optional:
+        invNdiverse : Boolean, optional
             If it is `True`, then the efficient diversified portfolio with the 
             same diversification factor as the equal weighted portfolio is
             added to the plot. The default is `False`.
-        `invNdrr` : Boolena, optional;
+        invNdrr : Boolena, optional
             If it is `True`, then the efficient diversified portfolio with the 
             same expected rate of return as the equal weighted portfolio is
             added to the plot. The default value is `False`.
-        `component` : Boolean, optional;
+        component : Boolean, optional
             If it is `True`, then the single component portfolios are added to 
             the plot. The default is `True`.
-        `randomport` : `int`, optional;
+        randomport : `int`, optional
             Number of portfolios with random weights (inefficient) to be
             added to the plot (for reference). The default is `20`.
-        `addport` : `dict` or `pandas.DataFrame`, optional;
+        addport : `dict` or `pandas.DataFrame`, optional
             The weights of additional portfolio to be added to the plot.
             If it is a `dict` then the keys are the labels, and the values are 
             list of weights in the order of `rrate.columns`. If it is a 
             `pandas.DataFrame` the index are the labels, and each row is a set 
             of weights. The columns names should match the symbols names. 
             The default is `None`.
-        `fig_type` : `str`, optional;
+        fig_type : `str`, optional
             Graphical representation format. \n
                 * `'RR_risk'` : expected rate of return vs risk
                 * `'Sharpe_RR'` : sharpe vs expected rate of return
                 * `'Diverse_RR'` : diversification vs expected rate of return
                 
             The default is `'RR_risk'`.
-        `opt` : optional;
+        **opt : optional
             Additonal parameters:\n
-                * `'title'` : `str`; 
-                    The default is 'Portfolio frontiers'
-                * `'xlabel'` : `str`; 
+                * `'title'` : `str` 
+                    The default is 'Portfolio frontiers'.
+                * `'xlabel'` : `str` 
                     The default is \n
                     - `'risk'` if `fig_type='RR_risk'`,
                     - `'rate of returns'` otherwise.
-                * `'ylabel'` : `str`; 
+                * `'ylabel'` : `str` 
                     The default is \n
                         - `'rate of returns'` if `fig_type='RR_risk'`
                         - `'sharpe'` if `fig_type='Sharpe_RR'`
                         - `'diversification'` if `fig_type=diverse_RR`   
-                * `'tangent'` : Boolean; 
+                * `'tangent'` : Boolean 
                     If set to `True`, then the tangent
                     (to max sharpe point) is added. It has effect only  if
                     `fig_type='RR_risk'`. The default is `True`.
-                * `saveto` : `str`; 
+                * `saveto` : `str`
                     File name to save the figure. The extension dictates the 
                     format: png, pdf, svg, etc. For more details see the 
                     `mathplotlib` documentation for `savefig`. 
                     The default is `None`.
-                * `data` : `defaultdict`; 
+                * `data` : `defaultdict` 
                     Numerical data to construct the plot. If it is not `None`,
                     then it will take precedence and no other numerical 
                     evaluations will be performed. 
                     It is meant to produce different plot representations
                     without reevaluations. The default is `None`.
-                * `invN_label` : `str`;
+                * `invN_label` : `str`
                     The label for equal weighted portfolio. 
                     The default is `'1/N'`.
-                * `invNrisk_label` : `str`;
+                * `invNrisk_label` : `str`
                     The lable for efficient portfolio with same risk as 
                     equal weighted portfolio. The default is `invNrisk`.
-                * `invNdiverse_label` : `str`;
+                * `invNdiverse_label` : `str`
                     The label for diverse-efficient portfolio with the same
                     diversificeation factor as equal weighted porfolio.
                     The default is `'invNdiv'`.
-                * `invNdrr_label` : `str`;
+                * `invNdrr_label` : `str`
                     The label of diverse-efficient portfolio with the same
                     expected rate of return as equal weighted portolio.
                     The defualt is `'invNdrr'`.
-                * `maxdiverse_label` : `str`;
+                * `maxdiverse_label` : `str`
                     The label of maximum diverified portfolio. 
                     The default is `'MaxD'`.
-                * `minrisk_label` : `'str'`;
+                * `minrisk_label` : `'str'`
                     The label of minimum risk portfolio.
                     The default is `'MinR'`.
-                * `sharpe_label` : `str`;
+                * `sharpe_label` : `str`
                     The label of maximum Sharpe portfolio. 
                     The default is `'Sharpe'`.
 
         Returns
         -------
-        `dict`
-            Numerical data used to make the plots. It can be passed back to
-            reconstruct the plots without reevaluations.
+        `dict` : Numerical data used to make the plots. It can be passed back 
+        to reconstruct the plots without reevaluations.
         """
         if fig_type == 'RR_risk':
             xlabel = 'risk'
             ylabel = 'rate of return'
             plot_ff = self._plot_f1
         elif fig_type == 'Sharpe_RR':
             xlabel = 'rate of return'
@@ -980,15 +1100,15 @@
             # efficient frontier
             res['efficient']['efficient'] = 0
             if efficient > 0:
                 if rr_min is None:
                     warnings.warn("Warning: MinRisk -> efficient failed")
                     res['efficient']['efficient'] = 0
                 else:
-                    mu_max = self.muk.max()
+                    mu_max = self.muk.max(numeric_only=True)
                     rr_upper = mu_max - np.abs(mu_max) * _RR_ABS_TOL_
                     rr_eff = np.linspace(rr_min, rr_upper, efficient)
                     risk_eff = []
                     ww_eff = []
                     RR_eff = []
                     sharpe_eff = []
                     diverse_eff = []
@@ -1014,15 +1134,15 @@
             # inefficient frontier
             res['inefficient']['inefficient'] = 0
             if inefficient > 0 :
                 if rr_min is None:
                     warnings.warn("Warning: MinRisk -> inefficient failed")
                     res['inefficient']['inefficient'] = 0
                 else:
-                    mu_min = self.muk.min()
+                    mu_min = self.muk.min(numeric_only=True)
                     rr_lower = mu_min + np.abs(mu_min) * _RR_ABS_TOL_
                     rr_ineff = np.linspace(rr_lower, rr_min, inefficient)
                     risk_ineff = []
                     ww_ineff = []
                     RR_ineff = []
                     sharpe_ineff = []
                     diverse_ineff = []
@@ -1211,15 +1331,15 @@
             res['diverse_efficient']['diverse_efficient'] = 0
             if diverse_efficient > 0 :
                 if rr_maxdiverse is None:
                     warnings.warn("Warning: maxdiverse -> diverse_efficient "
                                   "failed")
                     res['diverse_efficient']['diverse_efficient'] = 0
                 else:
-                    mu_max = self.muk.max() 
+                    mu_max = self.muk.max(numeric_only=True) 
                     rr_upper = mu_max - np.abs(mu_max) * _RR_ABS_TOL_
                     rr_d_eff = np.linspace(rr_maxdiverse, rr_upper,
                                            diverse_efficient)
                     risk_d_eff = []
                     ww_d_eff = []
                     RR_d_eff = []
                     sharpe_d_eff = []
@@ -1248,15 +1368,15 @@
             res['diverse_inefficient']['diverse_inefficient'] = 0
             if diverse_inefficient > 0 :
                 if rr_maxdiverse is None:
                     warnings.warn("Warning: maxdiverse -> diverse_inefficient "
                                   "failed")
                     res['diverse_inefficient']['diverse_inefficient'] = 0
                 else:
-                    rr_min = self.muk.min()
+                    rr_min = self.muk.min(numeric_only=True)
                     rr_lower = rr_min + np.abs(mu_min) * _RR_ABS_TOL_
                     rr_d_ineff = np.linspace(rr_lower, rr_maxdiverse, 
                                              diverse_inefficient)
                     risk_d_ineff = []
                     ww_d_ineff = []
                     RR_d_ineff = []
                     sharpe_d_ineff = []
@@ -1661,15 +1781,15 @@
     def set_random_seed(self, seed = 42):
         """
         Sets the seed for Dirichlet random generator used in viewFrontiers
         to select the random inefficient portfolios.
 
         Parameters
         ----------
-        `seed` : `int`, optional;
+        seed : `int`, optional
             The random generator seed, in case you want to set it to a weird
             value other than `42` :). The default is `42`.
 
         Returns
         -------
         `None`
         """
@@ -1708,15 +1828,15 @@
     
     def getRiskComp(self):
         """
         Returns the risk of each portfolio component.
 
         Returns
         -------
-        `pandas.Series`
+        `pandas.Series` : risk per symbol.
         """
         if self._flag_risk_comp_calc: 
             self.status = self._status_risk_comp_calc
             return self.risk_comp
             
         srisk = np.zeros(self.rrate.shape[1])
         status = 0
@@ -1743,36 +1863,34 @@
     def getDiversification(self, ww, rrate=None):
         """
         Returns the value of the diversification factor for a give 
         portfolio.
 
         Parameters
         ----------
-        `ww` : `list`, `numpy.array` or `pandas.Series`;
+        ww : `list`, `numpy.array` or `pandas.Series`;
             Portfolio weights. Its length must be equal to the number of
             symbols in `rrate` (mktdata). All weights must be >=0 with 
             sum > 0.
             If it is a list or a `numpy.array` then the weights are assumed to
             be in order of `rrate.columns`. If it is a `pandas.Series` then 
             the index should be compatible with the `rrate.columns` or mktdata 
-            symbols (not necessary in the same order).
-        `rrate` : `pandas.DataFrame`, optional;
+            symbols (not necessarily in the same order).
+        rrate : `pandas.DataFrame`, optional
             Contains the portfolio components historical
-            rates of returns. If it is not `None` then it will overwrite the
-            `rrate` computed in the constructor from `mktdata`.
+            rates of return. If it is not `None` then it will overwrite the
+            rates of return computed in the constructor from `mktdata`.
             The default is `None`.
 
         Returns
         -------
-        `float` : The diversification value. \n
+        `float` : The diversification value. 
         """
         self._reset_output()
-        
-        if rrate is not None:
-            self.set_rrate(rrate)
+        self.set_rrate(rrate)
 
         if isinstance(ww, pd.core.series.Series):
             ww = ww[self.rrate.columns]
         w = np.array(ww)
         if any(w < 0.):
             raise ValueError("All ww must be non-negative")
         sw = w.sum()
@@ -1799,32 +1917,32 @@
             self.diverse = 1 - wrisk / crisk
         
         return self.diverse
     
     
     def set_method(self, method):
         """
-        Set computation method
+        Sets computation method.
 
         Parameters
         ----------
-        `method` : `str`;
-            Must be a valid method name. It will overright the value 
+        method : `str`;
+            Must be a valid method name. It will overwrite the value 
             set by the constructor.
 
         Returns
         -------
         `None`
         """
         self._set_method(method)
     
     
     def _norm_weights(self):
         self.ww[self.ww < _WW_TOL_] = 0.
-        self.ww /= self.ww.sum()
+        self.ww /= self.ww.sum(numeric_only=True)
         
         
     def _single_asset_port(self, port):
         if port == 'min':
             psymb = self.muk.idxmin()
         elif port == 'max':
             psymb = self.muk.idxmax()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `azapy-1.1.1/azapy/PortOpt/_RiskEngine.py` & `azapy-1.2.0/azapy/Generators/ModelPipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,209 +1,223 @@
-import numpy as np
 import pandas as pd
+import numpy as np
 
-from azapy.MkT.MkTcalendar import NYSEgen
+from azapy.Selectors.NullSelector import NullSelector
 
-class _RiskEngine():
+class ModelPipeline:
     """
-    Base class. Derive class needs to implement\n
-        getWeights \n
-
-    Methods:
-        * getPositions
-        * set_rrate
-        * set_mktdata
+    Construct a portfolio weights model from a sequence of elementary models. 
+    The last element of the sequence must be an optimizer model while the 
+    rest could be any number of selector models. 
+
+    **Attributes**
+        - sequence : `list` -  the sequence of elementary models
+        - capital : `flat` -  the capital at risk as a fraction of the 
+          total capital
+        - mktdata : `pandas.DataFrame` - historical market data of selected 
+          symbols
+        - active_symb : `list` - the list of selected symbols
+        - ww : `pandas.Series` - portfolio weights per symbol (all symbols)
+        
+    **Note**
+    All unselected symbols have 0 weight. However, some of the selected symbols
+    can have 0 weight after portfolio optimization stage.
     """
-
-    def __init__(self, mktdata=None, colname='adjusted',
-                 freq='Q', hlength=3.25, calendar=None):
+    def __init__(self, sequence=[NullSelector(), "EWP"]):
         """
         Constructor
 
         Parameters
         ----------
-        `mktdata` : `pandas.DataFrame`, optional;
-            Historic daily market data for portfolio components in the format
-            returned by `azapy.mktData` function. The default is `None`.
-        `colname` : `str`, optional;
-            Name of the price column from mktdata used in the weights
-            calibration. The default is 'adjusted'.
-        `freq` : `str`, optional;
-            Rate of returns horizon in number of business day. It could be
-            'Q' for quarter or 'M' for month. The default is 'Q'.
-        `hlength` : `float`, optional;
-            History length in number of years used for calibration. A
-            fractional number will be rounded to an integer number of months.
-            The default is `3.25`.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will 
-            be set to NYSE business calendar.
-            The default is `None`.
+        sequence : `list`, optional
+            List of elementary models. The last element of the list must be 
+            an optimizer while the rest could be any number of selectors. 
+            The sequence is executed from right to left.
+            The default is `[NullSelector(), "EWP"]`.
 
         Returns
         -------
         The object.
         """
-        if mktdata is not None:
-            self.set_mktdata(mktdata, colname, freq, hlength)
-
-    def set_rrate(self, rrate):
-        """
-        Sets portfolio components historical rates of returns in the format
-        "date", "symbol1", "symbol2", etc.
-
-        Parameters
-        ----------
-        `rrate` : `pandas.DataFrame`;
-            The portfolio components historical rates of returns.
-            If it is not `None`, it will overwrite the rrate computed in the
-            constructor from mktdata. The default is `None`.
-        Returns
-        -------
-        `None`
-        """
-        self.nn, self.mm = rrate.shape
-        self.muk = rrate.mean()
-        self.rrate = rrate
-
-    def set_mktdata(self, mktdata, colname='adjusted',
-                    freq='Q', hlength=3.25, calendar=None):
+        self.lseq =  len(sequence)
+        if self.lseq < 1:
+            raise ValueError("sequence cannot be emply!")
+        self.sequence = sequence
+        self.assets_opt = None
+        self.ww = None
+        self.capital = None
+        self.mktdata = None
+        self.active_symb = None
+            
+        
+    def getWeights(self, mktdata, **params):
         """
-        Sets historical market data. It will overwrite the choice made in the
-        constructor.
+        Computes the portfolio weights.
 
         Parameters
         ----------
-        `mktdata` : `pandas.DataFrame`;
-            Historic daily market data for portfolio components in the format
-            returned by `azapy.mktData` function.
-        `colname` : `str`, optional;
-            Name of the price column from mktdata used in the weights
-            calibration. The default is `'adjusted'`.
-        `freq` : `str`, optional;
-            Rate of returns horizon in number of business day. it could be
-            'Q' for quarter or 'M' for month. The default is `'Q'`.
-        `hlength` : `float`, optional;
-            History length in number of years used for calibration. A
-            fractional number will be rounded to an integer number of months.
-            The default is `3.25` years.
-        `calendar` : `numpy.busdaycalendar`, optional;
-            Business days calendar. If is it `None` then the calendar will 
-            be set to NYSE business calendar.
-            The default is `None`.
+        mktdata : `pandas.DataFrame`
+            Historical daily market data as returned by `azapy.readMkT` 
+            function.
+        **params : optional
+            Additional parameters that may be required by the elementary 
+            models. An example is `verbose=True`.
 
         Returns
         -------
-        `None`
+        `pandas.Series` : Portfolio weights per symbol.
         """
         if mktdata is None:
-            return
-
+            raise ValueError("no mktdata!")
         self.mktdata = mktdata
-
-        periods = 63 if freq == 'Q' else 21
-
-        if calendar is None:
-            calendar = NYSEgen()
-
-        edate = mktdata.index[-1]
-        sdate = edate - pd.offsets.DateOffset(months=round(hlength * 12, 0))
-        sdate = np.busday_offset(sdate.date(),
-                                 0, roll='backward',  busdaycal=calendar)
-        rrate = mktdata.pivot(columns='symbol', values=colname)[sdate:]
-        self.last_data = rrate.iloc[-1]
-        rrate = rrate.pct_change(periods=periods).dropna()
-
-        self.set_rrate(rrate)
-
-    def getPositions(self, nshares=None, cash=0., ww=None):
+        mktd = mktdata
+        
+        verbose = params['verbose'] if 'verbose' in params.keys() else False
+ 
+        anames = np.append(mktd['symbol'].unique(),'_CASH_')
+        self.ww = pd.Series(np.zeros(len(anames)), index=anames)
+        
+        # loop through selectrs
+        self.capital = 1
+        for k in range(self.lseq - 1):
+            if pd.isnull(self.sequence[k]):
+                continue
+            if self.sequence[k]._ptype_ != 'Selector':
+                raise ValueError("unknown obj as a `Selector` !!!")
+                
+            cpt, mktd = self.sequence[k].getSelection(mktd, **params)
+            self.capital *= cpt
+            if self.capital == 0:
+                # all in cash
+                self.ww['_CASH_'] = 1
+                self.active_symb = ['_CASH_']
+                return self.ww
+
+        # selected assets
+        anames = np.append(mktd['symbol'].unique(),'_CASH_')
+        nassets = len(anames)
+            
+        self.assets_opt = anames
+        if verbose:
+            print(f"assets for optimization: {self.assets_opt[:-1]}"
+                  f"\nwith calpital in cash {1-self.capital}")
+        
+        # allocation strategy
+        
+        # strategies by name (str)
+        if type(self.sequence[-1]) == str:
+            # EWP (equal weighted portfolio)
+            if self.sequence[-1] == 'EWP':
+                self.ww[anames[:-1]] = self.capital / (nassets - 1)
+                self.ww['_CASH_'] = 1 - self.capital
+                self.active_symb = self.ww.drop('_CASH_').index.to_list()
+                return self.ww
+            else:
+                raise ValueError(f"unknown optimizer {self.sequence[-1]}")
+        # Analyzer (optimizer)
+        elif self.sequence[-1]._ptype_ == 'Optimizer':
+            params['pclose'] = False
+            ws = self.sequence[-1].getWeights(mktdata=mktd, **params)
+            self.ww[ws.index] = ws * self.capital
+            self.ww['_CASH_'] = 1 - self.capital
+            self.active_symb = ws.index.to_list()
+            return self.ww
+        else:
+            raise ValueError("unknown optimizer")
+            
+            
+    def getPositions(self, nshares=None, cash=0., ww=None, verbose=True):
         """
-        Computes the number of shares according to the weights
+        Computes the rebalanced number of shares.
 
         Parameters
         ----------
-        `nshares` : `pandas.Series`, optional;
-            Number of shares per portfolio component. A missing component
-            entry will be considered `0`. A `None` value assumes that all
-            components entries are `0`. The name of the components must be
+        nshares : `panda.Series`, optional
+            Initial number of shares per portfolio component.
+            A missing component
+            entry will be considered 0. A `None` value assumes that all
+            components entries are 0. The name of the components must be
             present in the mrkdata. The default is `None`.
-        `cash` : `float`, optional;
-            Additional cash to be considered in the overall capital. A
+        cash : `float`, optional
+            Additional cash to be added to the capital. A
             negative entry assumes a reduction in the total capital
-            available for rebalance. The remaining capital must be >0.
-            The default is `0`.
-        `ww` : `pandas.Series`, optional;
-            External portfolio weights. If it not set to `None` these
-            weights will overwrite the calibrated weights.
-            The default is `None`.
-
+            available for rebalance. The total capital cannot be < 0.
+            The default is 0. 
+        ww : `panda.Series`, optional
+            External overwrite portfolio weights. 
+            If it not set to `None` these
+            weights will overwrite the calibration results.
+            The default is `None`. 
+        verbose : Boolean, optional
+            Is it set to `True` the function prints the closing prices date.
+            The default is `True`.
+        
         Returns
         -------
-        `pandas.DataFrame`;
-            The rolling information.
+        `pandas.DataFrame` : the rolling information.
 
         Columns:
 
             - `'old_nsh'` :
-                the initial number of shares per portfolio
-                component as well as additional cash position. These are
-                present in the input.
+                initial number of shares per portfolio component and
+                the additional cash. These are input values.
             - `'new_nsh'` :
-                the new number of shares per component plus the
-                residual cash (due to the rounding to an integer number of
-                shares). A negative entry means that the investor needs to
-                add more cash to cover for the number of share
-                roundup shortfall. It has a small value.
+                the new number of shares per component plus the residual
+                cash (due to the rounding to an integer number of shares).
+                A negative entry means that the investor needs to add more
+                cash to cover for the roundup shortfall.
+                It has a small value.
             - `'diff_nsh'` :
-                the number of shares that needs to be
-                both/sold to rebalance the portfolio positions.
+                number of shares (buy/sale) needed to rebalance the 
+                portfolio.
             - `'weights'` :
-                portfolio weights used for rebalancing. The 'cash'
-                entry is the new portfolio value.
+                portfolio weights used for rebalancing. The cash entry is
+                the new portfolio value (invested capital).
             - `'prices'` :
                 the share prices used for rebalances evaluations.
 
-        Note: Since the prices are closing prices, the rebalance can be
-        executed next business. Additional cash slippage may occur due
-        to share price differential between the previous day closing and
-        execution time.
-
-        """
-        ns = pd.Series(0, index=self.rrate.columns)
-        if nshares is not None:
-            ns = ns.add(nshares, fill_value=0)
-
-        if len(self.rrate.columns) != len(ns):
-            raise ValueError("nshares must by a subset "
-                             f"of {self.rrate.columns}")
-
-        pp = self.last_data[self.rrate.columns.to_list()]
-
-        cap = ns.dot(pp) + cash
-        if ww is None:
-            ww = self.getWeights()
+            Note: Since the prices are closing prices, the rebalance can be
+            computed after the market close and before the 
+            trading execution (next day). 
+            Additional cash slippage may occur due
+            to share price differential between the previous day closing and
+            execution time.
+        """
+        price = self.mktdata.pivot(columns='symbol', values='close').iloc[-1]
+        price['_CASH_'] = 1            
+      
+        if ww is None: 
+            ww = self.ww
         else:
-            ww0 = pd.Series(0, index=self.rrate.columns)
-            ww = ww0.add(ww, fill_value=0)
-            if len(self.rrate.columns) != len(ns):
-                raise ValueError("ww: wrong component names - "
-                                 f"must be among {self.rrate.columns}")
-
-        newns = (ww / pp * cap).round(0)
-        newcash = cap - newns.dot(pp)
-
-        ns['cash'] = cash
-        newns['cash'] = newcash
-        ww['cash'] = cap - newcash
-        pp['cash'] = 1.
-
-        res = pd.DataFrame({'old_nsh': ns,
-                            'new_nsh': newns,
-                            'diff_nsh': newns - ns,
-                            'weights' : ww.round(6),
-                            'prices': pp})
-
-        return res
-
-    # need to be implemented by the derive classes
-    def getWeights(self):
-        pass
+            ww = ww / ww.sum()
+            ww = pd.Series(0, index=price.index).add(ww, fill_value=0)
+            
+        nsh_in = pd.Series(0, index=price.index)
+        if nshares is not None:
+            nsh_in = nsh_in.add(nshares, fill_value=0)
+            
+        cap = nsh_in @ price + cash
+        nsh_out = (ww * cap / price)
+        nsh_out[nsh_out.index != '_CASH_'] = nsh_out[nsh_out.index != '_CASH_'].round(0)
+
+        cap_adj = cap - nsh_out @ price
+ 
+        nsh_in['_CASH_'] = cash
+        nsh_out['_CASH_'] += cap_adj
+        
+        res = pd.DataFrame({'old_nsh': nsh_in.round(2),
+                            'new_nsh': nsh_out.round(2),
+                            'diff_nsh': (nsh_out - nsh_in).round(2),
+                            'weights' : ww.round(4),
+                            'prices': price.round(2)})
+        
+        res = res.rename(index={'_CASH_': 'cash'})
+        res = res[(res['old_nsh'] != 0) | (res['new_nsh'] != 0) | (res.index == 'cash')]
+        
+        if verbose:
+            print(f"Computed as of: {price.name.date()}")
+            print(f"previouse invested capital: {np.round(cap - cash, 2)}")
+            print(f"cash adjustment: {np.round(cash, 2)}")
+            print(f"new invsted capital: {np.round(cap * self.capital - cap_adj, 2)}")
+            print(f"cash in hands: {np.round(cap * (1 - self.capital) + cap_adj, 2)}")
+        
+        return res
```

### Comparing `azapy-1.1.1/azapy/PortOpt/_solvers.py` & `azapy-1.2.0/azapy/Analyzers/_solvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     
     # gather the results
     rout = {}
     rout['status'] = res['info']['exitFlag']
     # accept 10 Close to optimal as optimal
     if rout['status'] == 10: rout['status'] = 0
     rout['infostring'] = res['info']['infostring']
-    rout['pcost'] = np.float(res['info']['pcost'])
+    rout['pcost'] = np.float64(res['info']['pcost'])
     rout['x'] = res['x']
     
     return rout
 
 def _socp_solver(method, c_data, G, h_data,dims, A=None, b_data=None):
     if method == 'ecos':
         return _socp_ecos(c_data, G, h_data, dims, A, b_data)
```

### Comparing `azapy-1.1.1/azapy/util/drawdown.py` & `azapy-1.2.0/azapy/Util/drawdown.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+""""""  # <- add this
 """
 Contains:
-    
     - max_drawdown : returns maximum drawdown
     - drawdown : returns a list of drawdowns
 """
 import pandas as pd
 import numpy as np
 from collections import defaultdict
 
@@ -27,39 +27,36 @@
     except IndexError:
         draw_end = np.nan  # drawdown not recovered
 
     return draw_val, draw_min, draw_start, draw_end
 
 def max_drawdown(mktdata, col=None):
     """
-    Computes the max_drowdown for a price time-series
+    Computes the maximum drawdown for a time-series of prices.
 
     Parameters
     ----------
-    `mktdata` : `pandas.Series` or `pandas.DataFram`;
-        time-series of prices as a `pandas.Series` or as column in a 
+    mktdata : `pandas.Series` or `pandas.DataFram`
+        Time-series of prices as a `pandas.Series` or as column in a 
         pandas.DataFrame`
-    `col` : `str`, optional;
-        column name if mktdata is a DataFrame. If is set to `None` then 
-        `mktdata` is assumed to be a Series. The default is `None`.
+    col : `str`, optional
+        Column name if `mktdata` is a `pandas.DataFrame`. If is set to `None`, 
+        then `mktdata` is assumed to be a `pandas.Series`. 
+        The default is `None`.
 
     Returns
     -------
-    `float`;
-        The value of the drawdown.
-
-            `i_min` : `pandas.Timestamp`
-                The maximum drawdown date.
-            `i_start` : `pandas.Timestamp`
-                Date when the drawdown had started.
-            `i_end` : `pandas.Timestamp`
-                Date of the drawdown recovery. A value of `nan` indicates 
-                that the drawdown is in progress.
+    (`float`, `pandas.Timestamp`, `pandas.Timestamp`, `pandas.Timestamp`) : Tuple 
+        - value of the drawdown, 
+        - maximum drawdown date, 
+        - drawdawn start date,
+        - drawdown end date. It is set to `nan` if the drawdown is still 
+          in progress.
     """
-    rdata = mktdata if  col is None else mktdata[col]
+    rdata = mktdata if col is None else mktdata[col]
 
     val, i_min, i_start, i_end = _max_drawdown(_prep_uw(rdata))
 
     i_min = i_min.strftime('%Y-%m-%d')
     i_start = i_start.strftime('%Y-%m-%d')
     if not pd.isna(i_end):
         i_end = i_end.strftime('%Y-%m-%d')
@@ -68,36 +65,37 @@
 
 def drawdown(mktdata, col=None, top=10):
     """
     Computes the largest drawdowns for time-series of prices.
 
     Parameters
     ----------
-    `mktdata` : `pandas.Series` or `pandas.DataFrame`;
-        time-series of prices as a `pandas.Series` or as column in a 
-        `pandas.DataFrame`
-    `col` : `str`, optional;
-        Name of the column of price if mktdata is a `pandas.DataFrame`. 
-        If its value
-        is set to `None` then `mktdata` is assumed to be a `pandas.Series`.
+    mktdata : `pandas.Series` or `pandas.DataFrame`
+        Historical daily time-series of prices as a `pandas.Series` 
+        or as a `pandas.DataFrame`
+    col : `str`, optional
+        The column name if mktdata is a `pandas.DataFrame`. 
+        If it is set to `None`, then `mktdata` is assumed to be a 
+        `pandas.Series`.
         The default is `None`.
-    `top` : `int`, optional;
-        Maximum number of the largest drawdowns to be computed.
+    `top` : `int`, optional
+        Maximum number of largest drawdowns to be reported.
         The default is `10`.
 
     Returns
     -------
-    `pandas.DataFrama`;
-        Table containing the drawdowns ordered from the largest to smallest.
+    `pandas.DataFrama` : Table containing the drawdowns ordered from the 
+    largest to smallest.
         Table columns are:
 
             - 'DD': (float) drawdown max value
             - 'Date': (`pandas.Timestamp`) drawdown max value date
             - 'Start': (`pandas.Timestamp`) drawdown start date
             - 'End': (`pandas.Timestamp`) drawdown recovery date
+            
         The number of rows is <= top
     """
     rdata = mktdata if pd.isna(col) else mktdata[col]
 
     uw = _prep_uw(rdata)
     dd = defaultdict(lambda: [])
```

### Comparing `azapy-1.1.1/azapy/util/gamblingKelly.py` & `azapy-1.2.0/azapy/Util/gamblingKelly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import numpy as np
 import pandas as pd
 import cvxopt as cx
 import warnings
 
 def gamblingKelly(pp=[0.6]):
     """
-    Compute the Kelly allocation for multiple binary games.
+    Computes the Kelly allocation for multiple binary games.
 
     Parameters
     ----------
-    `pp` : `list`, optional;
-        List of wining probabilities for each game. The default is `[0.6]`.
+    pp : `list`, optional
+        List of winning probabilities for each game. The default is `[0.6]`.
 
     Returns
     -------
-    `pandas.Series`
-        Bet sizes as percentage of the capital=1.
+    `pandas.Series` : Bets size as percentage of the capital.
     """
     pp = np.array(pp)
     assert all((pp > 0) & (pp < 1)), "all pp must by in (0,1)"
     nn = len(pp)
     
     # local function 
     def _ffval(w, p):
```

### Comparing `azapy-1.1.1/azapy/util/schedule.py` & `azapy-1.2.0/azapy/Util/schedule.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,57 @@
+""""""  # <- add this
 """
 Contains:
-    
     - schedule_simple : creates a simple schedule
-    - schedule_roll : creates a rollover schedule
+    - schedule_roll : creates a rolling history schedule
+    - schedule_offset : create a simple schedule with an offset start
 """
-
 import pandas as pd
 import numpy as np
 import pandas.tseries.offsets as pt
 
 from azapy.MkT.MkTcalendar import NYSEgen
 
+
 def schedule_simple(sdate='2010-01-01',
                     edate='today',
                     freq='Q',
                     noffset=-3,
                     fixoffset=-1,
                     calendar=None):
     """
-    Creates a simple schedule 'Droll', 'Dfix'.
+    Creates a simple schedule: 'Droll', 'Dfix'.
 
     Parameters
     ----------
-    `sdate` : `str`, optional;
+    sdate : `str`, optional
         Start date (reference) of the schedule.
         The default is `'2010-01-01'`.
-    `edate` : `str`, optional;
+    edate : `str`, optional
         End date (reference) of the schedule. 
         The default is `'today'`.
-    `freq` : `str`, optional;
+    freq : `str`, optional
         Rolling period. It can take 2 values: `'Q'` for quarterly and `'M'` for
         monthly rolling periods. The default is `'Q'`.
-    `noffset` : `int`, optional;
+    noffset : `int`, optional
         Offset in number of business days for `Droll` relative to the end of 
         calendar period (quarter or month). The default is `-3`.
-    `fixoffset` : `int`, optional
+    fixoffset : `int`, optional
         Offset in number of business days for `Dfix` relative to `Droll`. It 
         must be <=0. The default is `-1`.
-    `calendar` : `numpy.busdaycalendar`, optional;
+    calendar : `numpy.busdaycalendar`, optional
         Business days calendar. If is it `None` then the calendar will be set
         to NYSE business calendar.
         The default is `None`.
 
     Returns
     -------
-    `pandas.DataFrame`
-        Table containing 2 datetime columns: 'Droll' the rolling date and
-        'Dfix' the fixing date.
+    `pandas.DataFrame` : Table containing 2 datetime columns,
+        - 'Droll' the rolling date,
+        - 'Dfix' the fixing date.
     """
     sdate = pd.to_datetime(sdate)
     if freq == 'Q': edate = pd.to_datetime(edate) + pt.QuarterEnd(1)
     elif freq == 'M': edate = pd.to_datetime(edate) + pt.MonthEnd(1)
     else: raise ValueError("Wrong freq, Must be 'Q' or 'M'")
     
     if calendar is None:
@@ -60,67 +61,123 @@
         .to_numpy(dtype='<M8[D]')
     troll = np.busday_offset(tedx, noffset, roll='backward', 
                              busdaycal=calendar)
     tfix = np.busday_offset(troll, fixoffset, roll='backward', 
                             busdaycal=calendar)
     return pd.DataFrame({'Droll': troll, 'Dfix': tfix})
 
+
 def schedule_roll(sdate='2010-01-01',
                   edate='today',
                   freq='Q',
                   noffset=-3,
                   fixoffset=-1,
                   calendar=None,
                   hlength=1.25):
     """
     Creates a schedule with rolling history: 'Droll', 'Dfix' and 'Dhist'.
 
     Parameters
     ----------
-    `sdate` : `str`, optional;
+    sdate : `str`, optional
         Start date (reference) of the schedule.
         The default is `'2010-01-01'`.
-    `edate` : `str`, optional;
+    edate : `str`, optional
         End date (reference) of the schedule. 
         The default is `'today'`.
-    `freq` : `str`, optional;
+    freq : `str`, optional
         Rolling period. It can take 2 values: `'Q'` for quarterly and `'M'` for
         monthly rolling periods. The default is `'Q'`.
-    `noffset` : `int`, optional;
+    noffset : `int`, optional
         Offset in number of business days for Droll relative to the end of 
         calendar period (quarter or month). The default is `-3`.
-    `fixoffset` : `int`, optional;
+    fixoffset : `int`, optional
         Offset in number of business days for `Dfix` relative to `Droll`. It 
         can be zero or negative. The default is `-1`.
-    `calendar` : `numpy.busdaycalendar`, optional;
+    calendar : `numpy.busdaycalendar`, optional
         Business days calendar. If is it `None` then the calendar will be set
         to NYSE business calendar.
         The default is `None`.
-    `hlength` : `float`, optional;
+    hlength : `float`, optional
         Offset in number of years for 'Dhist' relative to 'Dfix'. A fractional 
         value will be rounded to an integer number of months via
         `round(hlength * 12, 0)`. `hlength` must be non-negative.
         The default is `1.25` years.
 
     Returns
     -------
-    `pandas.DataFrame`;
-        Table containing 2 datetime columns: 'Droll' the rolling date,
-        'Dfix' the fixing date and 'Dhist' start day for a calibration period.
+    `pandas.DataFrame` : Table containing 3 datetime columns, 
+        - 'Droll' the rolling date,
+        - 'Dfix' the fixing date,
+        - 'Dhist' start date for calibration period.
     """
     sdate = pd.to_datetime(sdate)
     edate = pd.to_datetime(edate)
     if calendar is None:
         calendar = NYSEgen()
     sch = schedule_simple(sdate, edate, freq, noffset, fixoffset, calendar)
     sch['Dhist'] = sch['Dfix'] - pd.offsets \
         .DateOffset(months=round(hlength * 12, 0))
     sch['Dhist'] = np.busday_offset(sch['Dhist'].to_numpy(dtype='<M8[D]'), 
-                                    0, roll='backward', 
-                                    busdaycal=calendar)
+                                    0, roll='backward', busdaycal=calendar)
     for k in range(len(sch)):
         if sch['Dhist'][k] >= sdate: 
             schedule = sch[k:].reset_index(drop=True)
             return schedule
     
     raise ValueError("Cannot make a schedule!!")
-    
+    
+    
+def schedule_offset(sdate='2010-01-01',
+                    edate='today',
+                    freq='Q',
+                    noffset=-3,
+                    fixoffset=-1,
+                    calendar=None,
+                    hlength=1.25):
+    """
+    Creates a simple schedule ('Droll', 'Dfix') with an offset start.
+
+    Parameters
+    ----------
+    sdate : `str`, optional
+        Start date (reference) to which the offset is added.
+        The default is `'2010-01-01'`.
+    edate : `str`, optional
+        End date (reference) of the schedule. 
+        The default is `'today'`.
+    freq : `str`, optional
+        Rolling period. It can take 2 values: `'Q'` for quarterly and `'M'` for
+        monthly rolling periods. The default is `'Q'`.
+    noffset : `int`, optional
+        Offset in number of business days for Droll relative to the end of 
+        calendar period (quarter or month). The default is `-3`.
+    fixoffset : `int`, optional
+        Offset in number of business days for `Dfix` relative to `Droll`. It 
+        can be zero or negative. The default is `-1`.
+    calendar : `numpy.busdaycalendar`, optional
+        Business days calendar. If is it `None` then the calendar will be set
+        to NYSE business calendar.
+        The default is `None`.
+    hlength : `float`, optional
+        Offset, in number of years, for first 'Droll' relative to 'sdate'.  
+        A fractional value will be rounded to an integer number of months via
+        `round(hlength * 12, 0)`. `hlength` must be non-negative.
+        The default is `1.25` years.
+
+    Returns
+    -------
+    `pandas.DataFrame` : Table containing 2 datetime columns
+        - 'Droll' the rolling date,
+        - 'Dfix' the fixing date.
+    """
+    sdate = np.datetime64(pd.to_datetime(sdate).date())
+    edate = np.datetime64(pd.to_datetime(edate).date())
+    if calendar is None:
+        calendar = NYSEgen()
+    sdate = sdate + pd.offsets.DateOffset(months=round(hlength * 12, 0))
+    sdate = np.busday_offset(np.array(sdate, dtype='<M8[D]'), 
+                             0, roll='forward', busdaycal=calendar)
+    if sdate >= edate:
+        raise ValueError(f"offset sdate {sdate} > edate {edate}!!!")
+        
+    return schedule_simple(sdate, edate, freq, noffset, fixoffset, calendar)
```

### Comparing `azapy-1.1.1/azapy.egg-info/PKG-INFO` & `azapy-1.2.0/azapy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azapy
-Version: 1.1.1
+Version: 1.2.0
 Summary: Financial Portfolio Optimization Algorithms
 Home-page: https://github.com/Mircea-MMXXI/azapy.git
 Author: Mircea Marinescu
 Author-email: mircea.marinescu@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://azapy.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/Mircea-MMXXI/azapy
@@ -42,15 +42,15 @@
   6. mBTSD - mixture BTSD (Below Threshold Semi-Deviation)
   7. GINI - Gini index (as in Corrado Gini statistician 1884-1965)
   8. SD - standard deviation
   9. MV - variance (as in mean-variance model)
   10. mEVaR - mixture EVaR (Entropic Value at Risk)
   <span style="color:red">(alpha version)</span>
 
-For each risk-based optimization class the following strategies are
+For each class of portfolio the following optimization strategies are
 available:
   1. Optimal-risk portfolio for targeted expected rate of return value
   2. Sharpe-optimal portfolio - maximization of generalized Sharpe ratio
   3. Sharpe-optimal portfolio - minimization of inverse generalized Sharpe
   ratio
   4. Minimum risk portfolio
   5. Optimal-risk portfolio for a fixed risk-aversion factor
@@ -79,14 +79,18 @@
      the asset absolute value of maximum drawdowns over a predefined
      historical period)
 
 C. Greedy portfolio optimization strategies:
   1. Kelly's portfolio (as in John Larry Kelly Jr. scientist 1923-1965) -
      maximization of portfolio log returns
 
+D. Market Selectors
+  1. Dual Momentum Selector <span style="color:red">(alpha version)</span>
+  2. Correlation Clustering Selector <span style="color:red">(alpha version)</span>
+
 Utility functions:
   * Collect historical market data from various providers.
     Supported providers:
 
     - yahoo.com
     - eodhistoricaldata.com
     - alphavantage.co
@@ -94,22 +98,21 @@
 
   * Generate business calendars. At this point only NYSE business calendar
     is implemented.
   * Generate rebalancing portfolio schedules.
   * Append a cash-like security to an existing market data object.
   * Update market data saved in a directory.
 
-
-The pollowing third-party packages were used with azapy 1.1.1
-* python 3.11.2
-* pandas 1.5.3
-* numpy 1.23.5
-* scipy 1.10.0
-* statsmodels 0.13.5
-* matplotlib 3.7.1
-* plotly 5.9.0
-* requests 2.28.1
-* pandas_market_calendars 4.1.4
-* ecos 2.0.12
-* cvxopt 1.3.0.1
-* ta 0.10.2
-* yfinance 0.2.14
+The following third-party packages were used with azapy 1.2.1:
+  * python 3.11.2
+  * pandas 1.5.3
+  * numpy 1.24.3
+  * scipy 1.10.1
+  * statsmodels 0.13.5
+  * matplotlib 3.7.1
+  * plotly 5.9.0
+  * requests 2.29.0
+  * pandas_market_calendars 4.1.4
+  * ecos 2.0.12
+  * cvxopt 1.3.0.1
+  * ta 0.10.2
+  * yfinance 0.2.14
```

### Comparing `azapy-1.1.1/setup.py` & `azapy-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #from azapy import __version__
 
 with open("README.md", "r", encoding="utf-8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="azapy",
-    version="1.1.1",
+    version="1.2.0",
     author="Mircea Marinescu",
     author_email="mircea.marinescu@outlook.com",
     description="Financial Portfolio Optimization Algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Mircea-MMXXI/azapy.git",
     project_urls={
```

