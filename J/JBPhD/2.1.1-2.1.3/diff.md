# Comparing `tmp/JBPhD-2.1.1.tar.gz` & `tmp/JBPhD-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBPhD-2.1.1.tar", last modified: Fri May 12 20:15:13 2023, max compression
+gzip compressed data, was "JBPhD-2.1.3.tar", last modified: Sun May 14 18:11:59 2023, max compression
```

## Comparing `JBPhD-2.1.1.tar` & `JBPhD-2.1.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 20:15:10.000000 JBPhD-2.1.1/
-drwxrwxrwx   0        0        0        0 2023-05-12 20:15:10.000000 JBPhD-2.1.1/JBPhD.egg-info/
--rw-rw-rw-   0        0        0      201 2023-05-12 20:15:08.000000 JBPhD-2.1.1/JBPhD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1604 2023-05-12 20:15:08.000000 JBPhD-2.1.1/JBPhD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 20:15:08.000000 JBPhD-2.1.1/JBPhD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-12 20:15:08.000000 JBPhD-2.1.1/JBPhD.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      135 2023-05-12 20:15:08.000000 JBPhD-2.1.1/JBPhD.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-12 20:15:08.000000 JBPhD-2.1.1/JBPhD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      201 2023-05-12 20:15:14.000000 JBPhD-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.1.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 20:15:10.000000 JBPhD-2.1.1/Task/
--rw-rw-rw-   0        0        0     2336 2023-04-20 18:29:48.000000 JBPhD-2.1.1/Task/Api.json
--rw-rw-rw-   0        0        0     2332 2023-04-30 20:14:46.000000 JBPhD-2.1.1/Task/Api2.json
--rw-rw-rw-   0        0        0   256511 2023-05-07 17:28:42.000000 JBPhD-2.1.1/Task/Back_Right.PNG
--rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.1.1/Task/Consent Form.docx
--rw-rw-rw-   0        0        0     1555 2023-05-12 13:01:46.000000 JBPhD-2.1.1/Task/Consent Form.txt
--rw-rw-rw-   0        0        0      998 2023-05-08 15:55:22.000000 JBPhD-2.1.1/Task/Dependencies.py
--rw-rw-rw-   0        0        0    12092 2023-05-12 14:41:32.000000 JBPhD-2.1.1/Task/Dependency Installation.py
--rw-rw-rw-   0        0        0      552 2023-05-06 17:47:44.000000 JBPhD-2.1.1/Task/Email Output.py
--rw-rw-rw-   0        0        0      202 2023-05-07 16:32:10.000000 JBPhD-2.1.1/Task/Experimental Run Trial.py
--rw-rw-rw-   0        0        0     4855 2023-05-06 18:07:04.000000 JBPhD-2.1.1/Task/Export.py
--rw-rw-rw-   0        0        0   249107 2023-05-07 17:28:42.000000 JBPhD-2.1.1/Task/Front_Left.PNG
--rw-rw-rw-   0        0        0   249006 2023-05-07 17:28:42.000000 JBPhD-2.1.1/Task/Front_Right.PNG
--rw-rw-rw-   0        0        0      883 2023-04-14 22:45:36.000000 JBPhD-2.1.1/Task/Graph.py
--rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.1.1/Task/ImageSample.PNG
--rw-rw-rw-   0        0        0   256274 2023-05-07 17:28:42.000000 JBPhD-2.1.1/Task/Inverse_Back_Left.PNG
--rw-rw-rw-   0        0        0      384 2023-04-24 19:08:56.000000 JBPhD-2.1.1/Task/Location.py
--rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.1.1/Task/MANIFEST.in.txt
--rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.1.1/Task/Manikin Back Down Left.png
--rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.1.1/Task/Manikin Back Up Right.png
--rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.1.1/Task/Manikin front Down Right.png
--rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.1.1/Task/Manikin front Up Right.png
--rw-rw-rw-   0        0        0        2 2023-05-12 14:39:40.000000 JBPhD-2.1.1/Task/N-Back count.txt
--rw-rw-rw-   0        0        0    18823 2023-05-04 21:33:20.000000 JBPhD-2.1.1/Task/N-Back.py
--rw-rw-rw-   0        0        0      625 2023-05-07 22:18:00.000000 JBPhD-2.1.1/Task/Output Test.py
-drwxrwxrwx   0        0        0        0 2023-05-12 20:15:10.000000 JBPhD-2.1.1/Task/Participant 1/
--rw-rw-rw-   0        0        0   101396 2023-05-12 14:42:14.000000 JBPhD-2.1.1/Task/Participant 1/Export Usage.csv
--rw-rw-rw-   0        0        0   128310 2023-05-12 14:42:12.000000 JBPhD-2.1.1/Task/Participant 1/Task Usage.csv
--rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.1.1/Task/Python Install.bat
--rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.1.1/Task/README.txt.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 10:25:18.000000 JBPhD-2.1.1/Task/RT count.txt
--rw-rw-rw-   0        0        0    17652 2023-05-01 10:34:26.000000 JBPhD-2.1.1/Task/Reaction Time Task - Copy.py
--rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.1.1/Task/Suffix.bat
--rw-rw-rw-   0        0        0        1 2023-05-07 20:23:30.000000 JBPhD-2.1.1/Task/Switch Count.txt
--rw-rw-rw-   0        0        0    24158 2023-05-07 20:29:12.000000 JBPhD-2.1.1/Task/Switching.py
--rw-rw-rw-   0        0        0    13618 2023-05-12 14:43:10.000000 JBPhD-2.1.1/Task/Task.py
-drwxrwxrwx   0        0        0        0 2023-05-12 20:15:10.000000 JBPhD-2.1.1/Task/__pycache__/
--rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.1.1/Task/__pycache__/Dependencies.cpython-311.pyc
--rw-rw-rw-   0        0        0     6694 2023-05-06 18:08:18.000000 JBPhD-2.1.1/Task/__pycache__/Export.cpython-311.pyc
--rw-rw-rw-   0        0        0      696 2023-05-04 10:46:06.000000 JBPhD-2.1.1/Task/__pycache__/Location.cpython-311.pyc
--rw-rw-rw-   0        0        0    18767 2023-05-07 22:15:14.000000 JBPhD-2.1.1/Task/__pycache__/Task.cpython-311.pyc
--rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.1.1/Task/__pycache__/spwf.cpython-311.pyc
--rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.1.1/Task/asterisk.png
--rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.1.1/Task/circle.jpg
--rw-rw-rw-   0        0        0      860 2023-04-30 18:46:22.000000 JBPhD-2.1.1/Task/cpudeps.py
--rw-rw-rw-   0        0        0      871 2023-04-30 19:06:50.000000 JBPhD-2.1.1/Task/cpudepsinstall.py
--rw-rw-rw-   0        0        0      854 2023-04-30 19:09:00.000000 JBPhD-2.1.1/Task/cpuexp.py
--rw-rw-rw-   0        0        0      854 2023-04-30 18:43:34.000000 JBPhD-2.1.1/Task/cpunbak.py
--rw-rw-rw-   0        0        0      861 2023-04-30 18:43:22.000000 JBPhD-2.1.1/Task/cpurt.py
--rw-rw-rw-   0        0        0      857 2023-04-30 18:43:54.000000 JBPhD-2.1.1/Task/cpuswitch.py
--rw-rw-rw-   0        0        0      852 2023-04-30 18:42:22.000000 JBPhD-2.1.1/Task/cputask.py
--rw-rw-rw-   0        0        0    12363 2023-04-07 13:54:00.000000 JBPhD-2.1.1/Task/greendot.png
--rw-rw-rw-   0        0        0    38788 2023-04-07 13:54:00.000000 JBPhD-2.1.1/Task/greentick.png
--rw-rw-rw-   0        0        0       54 2023-05-07 14:31:32.000000 JBPhD-2.1.1/Task/help.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 14:42:10.000000 JBPhD-2.1.1/Task/participant number.txt
--rw-rw-rw-   0        0        0      491 2023-05-09 09:35:40.000000 JBPhD-2.1.1/Task/pins.csv
--rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.1.1/Task/redcross.png
--rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.1.1/Task/reddot.png
--rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.1.1/Task/setup.py
--rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.1.1/Task/spwf.py
--rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.1.1/Task/spwfoutput.txt
--rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.1.1/Task/spwfvalue.txt
--rw-rw-rw-   0        0        0       14 2023-05-12 14:42:12.000000 JBPhD-2.1.1/Task/suffix.txt
--rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.1.1/Task/trial.jpeg
--rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.1.1/Task/uop.ico
--rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.1.1/Task/uop.jpeg
--rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.1.1/Task/uop.png
--rw-rw-rw-   0        0        0       42 2023-05-12 20:15:14.000000 JBPhD-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-05-12 13:08:18.000000 JBPhD-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 18:11:58.000000 JBPhD-2.1.3/
+drwxrwxrwx   0        0        0        0 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/
+-rw-rw-rw-   0        0        0      201 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1629 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      135 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-14 18:11:58.000000 JBPhD-2.1.3/JBPhD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      201 2023-05-14 18:12:00.000000 JBPhD-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.1.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 18:11:58.000000 JBPhD-2.1.3/Task/
+-rw-rw-rw-   0        0        0     2336 2023-04-20 18:29:48.000000 JBPhD-2.1.3/Task/Api.json
+-rw-rw-rw-   0        0        0     2332 2023-04-30 20:14:46.000000 JBPhD-2.1.3/Task/Api2.json
+-rw-rw-rw-   0        0        0   256511 2023-05-07 17:28:42.000000 JBPhD-2.1.3/Task/Back_Right.PNG
+-rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.1.3/Task/Consent Form.docx
+-rw-rw-rw-   0        0        0     1555 2023-05-12 13:01:46.000000 JBPhD-2.1.3/Task/Consent Form.txt
+-rw-rw-rw-   0        0        0      998 2023-05-08 15:55:22.000000 JBPhD-2.1.3/Task/Dependencies.py
+-rw-rw-rw-   0        0        0    12092 2023-05-12 14:41:32.000000 JBPhD-2.1.3/Task/Dependency Installation.py
+-rw-rw-rw-   0        0        0      552 2023-05-06 17:47:44.000000 JBPhD-2.1.3/Task/Email Output.py
+-rw-rw-rw-   0        0        0      202 2023-05-07 16:32:10.000000 JBPhD-2.1.3/Task/Experimental Run Trial.py
+-rw-rw-rw-   0        0        0     4855 2023-05-06 18:07:04.000000 JBPhD-2.1.3/Task/Export.py
+-rw-rw-rw-   0        0        0   249107 2023-05-07 17:28:42.000000 JBPhD-2.1.3/Task/Front_Left.PNG
+-rw-rw-rw-   0        0        0   249006 2023-05-07 17:28:42.000000 JBPhD-2.1.3/Task/Front_Right.PNG
+-rw-rw-rw-   0        0        0      883 2023-04-14 22:45:36.000000 JBPhD-2.1.3/Task/Graph.py
+-rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/ImageSample.PNG
+-rw-rw-rw-   0        0        0   256274 2023-05-07 17:28:42.000000 JBPhD-2.1.3/Task/Inverse_Back_Left.PNG
+-rw-rw-rw-   0        0        0      384 2023-04-24 19:08:56.000000 JBPhD-2.1.3/Task/Location.py
+-rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.1.3/Task/MANIFEST.in.txt
+-rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/Manikin Back Down Left.png
+-rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/Manikin Back Up Right.png
+-rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/Manikin front Down Right.png
+-rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/Manikin front Up Right.png
+-rw-rw-rw-   0        0        0        2 2023-05-12 14:39:40.000000 JBPhD-2.1.3/Task/N-Back count.txt
+-rw-rw-rw-   0        0        0    18823 2023-05-04 21:33:20.000000 JBPhD-2.1.3/Task/N-Back.py
+-rw-rw-rw-   0        0        0      625 2023-05-07 22:18:00.000000 JBPhD-2.1.3/Task/Output Test.py
+drwxrwxrwx   0        0        0        0 2023-05-14 18:11:58.000000 JBPhD-2.1.3/Task/Participant 1/
+-rw-rw-rw-   0        0        0      222 2023-05-13 14:00:22.000000 JBPhD-2.1.3/Task/Participant 1/Dependency Installation Usage.csv
+-rw-rw-rw-   0        0        0       70 2023-05-13 14:00:14.000000 JBPhD-2.1.3/Task/Participant 1/Export Usage.csv
+-rw-rw-rw-   0        0        0       70 2023-05-13 14:00:14.000000 JBPhD-2.1.3/Task/Participant 1/Task Usage.csv
+-rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.1.3/Task/Python Install.bat
+-rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.1.3/Task/README.txt.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 10:25:18.000000 JBPhD-2.1.3/Task/RT count.txt
+-rw-rw-rw-   0        0        0    17652 2023-05-01 10:34:26.000000 JBPhD-2.1.3/Task/Reaction Time Task - Copy.py
+-rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.1.3/Task/Suffix.bat
+-rw-rw-rw-   0        0        0        1 2023-05-07 20:23:30.000000 JBPhD-2.1.3/Task/Switch Count.txt
+-rw-rw-rw-   0        0        0    24158 2023-05-07 20:29:12.000000 JBPhD-2.1.3/Task/Switching.py
+-rw-rw-rw-   0        0        0    13325 2023-05-14 17:58:08.000000 JBPhD-2.1.3/Task/Task.py
+drwxrwxrwx   0        0        0        0 2023-05-14 18:11:58.000000 JBPhD-2.1.3/Task/__pycache__/
+-rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.1.3/Task/__pycache__/Dependencies.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6694 2023-05-06 18:08:18.000000 JBPhD-2.1.3/Task/__pycache__/Export.cpython-311.pyc
+-rw-rw-rw-   0        0        0      696 2023-05-04 10:46:06.000000 JBPhD-2.1.3/Task/__pycache__/Location.cpython-311.pyc
+-rw-rw-rw-   0        0        0    18767 2023-05-07 22:15:14.000000 JBPhD-2.1.3/Task/__pycache__/Task.cpython-311.pyc
+-rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.1.3/Task/__pycache__/spwf.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/asterisk.png
+-rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/circle.jpg
+-rw-rw-rw-   0        0        0      860 2023-04-30 18:46:22.000000 JBPhD-2.1.3/Task/cpudeps.py
+-rw-rw-rw-   0        0        0      871 2023-04-30 19:06:50.000000 JBPhD-2.1.3/Task/cpudepsinstall.py
+-rw-rw-rw-   0        0        0      854 2023-04-30 19:09:00.000000 JBPhD-2.1.3/Task/cpuexp.py
+-rw-rw-rw-   0        0        0      854 2023-04-30 18:43:34.000000 JBPhD-2.1.3/Task/cpunbak.py
+-rw-rw-rw-   0        0        0      861 2023-04-30 18:43:22.000000 JBPhD-2.1.3/Task/cpurt.py
+-rw-rw-rw-   0        0        0      857 2023-04-30 18:43:54.000000 JBPhD-2.1.3/Task/cpuswitch.py
+-rw-rw-rw-   0        0        0      852 2023-04-30 18:42:22.000000 JBPhD-2.1.3/Task/cputask.py
+-rw-rw-rw-   0        0        0    12363 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/greendot.png
+-rw-rw-rw-   0        0        0    38788 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/greentick.png
+-rw-rw-rw-   0        0        0       54 2023-05-07 14:31:32.000000 JBPhD-2.1.3/Task/help.txt
+-rw-rw-rw-   0        0        0      491 2023-05-14 16:12:16.000000 JBPhD-2.1.3/Task/pins.csv
+-rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/redcross.png
+-rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/reddot.png
+-rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.1.3/Task/setup.py
+-rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.1.3/Task/spwf.py
+-rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.1.3/Task/spwfoutput.txt
+-rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.1.3/Task/spwfvalue.txt
+-rw-rw-rw-   0        0        0       14 2023-05-13 14:00:14.000000 JBPhD-2.1.3/Task/suffix.txt
+-rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.1.3/Task/trial.jpeg
+-rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.1.3/Task/uop.ico
+-rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.1.3/Task/uop.jpeg
+-rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.1.3/Task/uop.png
+-rw-rw-rw-   0        0        0       42 2023-05-14 18:12:00.000000 JBPhD-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      837 2023-05-14 17:59:00.000000 JBPhD-2.1.3/setup.py
```

### Comparing `JBPhD-2.1.1/JBPhD.egg-info/SOURCES.txt` & `JBPhD-2.1.3/JBPhD.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -47,27 +47,27 @@
 Task/cpunbak.py
 Task/cpurt.py
 Task/cpuswitch.py
 Task/cputask.py
 Task/greendot.png
 Task/greentick.png
 Task/help.txt
-Task/participant number.txt
 Task/pins.csv
 Task/redcross.png
 Task/reddot.png
 Task/setup.py
 Task/spwf.py
 Task/spwfoutput.txt
 Task/spwfvalue.txt
 Task/suffix.txt
 Task/trial.jpeg
 Task/uop.ico
 Task/uop.jpeg
 Task/uop.png
+Task/Participant 1/Dependency Installation Usage.csv
 Task/Participant 1/Export Usage.csv
 Task/Participant 1/Task Usage.csv
 Task/__pycache__/Dependencies.cpython-311.pyc
 Task/__pycache__/Export.cpython-311.pyc
 Task/__pycache__/Location.cpython-311.pyc
 Task/__pycache__/Task.cpython-311.pyc
 Task/__pycache__/spwf.cpython-311.pyc
```

### Comparing `JBPhD-2.1.1/Task/Api.json` & `JBPhD-2.1.3/Task/Api.json`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Api2.json` & `JBPhD-2.1.3/Task/Api2.json`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Back_Right.PNG` & `JBPhD-2.1.3/Task/Back_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Consent Form.docx` & `JBPhD-2.1.3/Task/Consent Form.docx`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Consent Form.txt` & `JBPhD-2.1.3/Task/Consent Form.txt`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Dependencies.py` & `JBPhD-2.1.3/Task/Dependencies.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Dependency Installation.py` & `JBPhD-2.1.3/Task/Dependency Installation.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Email Output.py` & `JBPhD-2.1.3/Task/Email Output.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Export.py` & `JBPhD-2.1.3/Task/Export.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Front_Left.PNG` & `JBPhD-2.1.3/Task/Front_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Front_Right.PNG` & `JBPhD-2.1.3/Task/Front_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Graph.py` & `JBPhD-2.1.3/Task/Graph.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/ImageSample.PNG` & `JBPhD-2.1.3/Task/ImageSample.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Inverse_Back_Left.PNG` & `JBPhD-2.1.3/Task/Inverse_Back_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Manikin Back Down Left.png` & `JBPhD-2.1.3/Task/Manikin Back Down Left.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Manikin Back Up Right.png` & `JBPhD-2.1.3/Task/Manikin Back Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Manikin front Down Right.png` & `JBPhD-2.1.3/Task/Manikin front Down Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Manikin front Up Right.png` & `JBPhD-2.1.3/Task/Manikin front Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/N-Back.py` & `JBPhD-2.1.3/Task/N-Back.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Output Test.py` & `JBPhD-2.1.3/Task/Output Test.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Python Install.bat` & `JBPhD-2.1.3/Task/Python Install.bat`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Reaction Time Task - Copy.py` & `JBPhD-2.1.3/Task/Reaction Time Task - Copy.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Switching.py` & `JBPhD-2.1.3/Task/Switching.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/Task.py` & `JBPhD-2.1.3/Task/Task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import socket
 import tkinter
 import tkinter as tk
 import os
 
-
 def is_connected():
     websites = ['www.google.com', 'www.facebook.com']
     for website in websites:
         try:
             socket.create_connection((website, 80))
             return True
         except OSError:
@@ -40,19 +39,19 @@
                 y = int((screen_height/2) - (150/2))
 
                 self.master.geometry("600x150+{}+{}".format(x, y))
                 
                 self.pin_label = tk.Label(self.master, text="Welcome to the task\n\nTo begin, please enter your PIN. This will have been sent to you via email.\n\nEnter your PIN:")
                 self.pin_label.pack()
                 
-                self.pin_entry = tk.Entry(self.master)#, show="*")
+                self.pin_entry = tk.Entry(self.master)
                 self.pin_entry.pack()
                 
                 self.submit_button = tk.Button(self.master, text="Submit", command=self.submit_pin)
-                self.submit_button.pack()
+                self.submit_button.pack(pady=15)
                 
                 self.pins = {}
                 script_dir = os.path.dirname(os.path.abspath(__file__))
                 csv_path = os.path.join(script_dir, "pins.csv")
                 with open(csv_path) as f:
                     reader = csv.reader(f)
                     for row in reader:
@@ -66,31 +65,29 @@
                     message = f"Correct PIN\n\nYour participant number is {participant_num}.\n\nThe task will now load"
                     with open("participant number.txt", "w") as outfile:
                         outfile.write(participant_num)
                         self.master.destroy() 
                 else:
                     message = "Invalid PIN."
 
-                tk.messagebox.showinfo("Result", message)
-                
+                tk.messagebox.showinfo("Result", message)                
 
         if __name__ == "__main__":
 
             root = tk.Tk()
             PinSystem(root)
             root.mainloop()
             root.quit()
 
     import spwf
 
     print(f'Welcome to the task! Thank you for your interest in the study.\n\nYou are participant number {spwf.participant_number}.\n\nThe task is now loading, it may take a short while to load.')
 
     import subprocess
     import sys
-    import os
 
     pythonpath = sys.executable
     python_path = pythonpath
     os.environ["PATH"] += os.pathsep + python_path
 
     filename = "participant number.txt"
 
@@ -191,24 +188,21 @@
 
             USERNAME = spwf.emailadd
             PASSWORD = spwf.password
             
             def emailsupport():
                 email_window = tk.Toplevel()
                 email_window.title("Compose Email")
-
-                # Email body input
                 body_label = tk.Label(email_window, text="Please describe your issue/query in as much detail as possible")
                 body_label.pack(fill='both', expand=False, side=tk.TOP, padx=5, pady=5)
                 body_text = tk.Text(email_window, wrap=tk.WORD)
                 body_text.pack(fill='both', expand=False, side=tk.TOP, padx=5, pady=5)
 
                 def send_email(body):
                     print("Send called")
-                    # Create attachment object
                     sg = SendGridAPIClient(api_key=spwf.key)
                     message = Mail(
                         from_email=spwf.output,
                         to_emails=spwf.output,
                         subject=f'Email from Participant {spwf.participant_number}',
                         html_content=f'<strong>{body}</strong>'
                     )
@@ -218,27 +212,23 @@
                         email_window.destroy()
                     except Exception as e:
                         print(e)
                     email_window.destroy()
 
                 submit_button = tk.Button(email_window, text="Send", command=lambda: send_email(body_text.get("1.0", tk.END)))
                 submit_button.pack(expand=False, side=tk.TOP, padx=5, pady=5)
-
             
             def pis():
                 if scount > runcount:
                     messagebox.showerror("Error", errortext)
                 else:
                     file_path = "Switching.py"
                     subprocess.run([python_path, file_path], check=True)
                     subprocess.run([python_path, 'Export.py'], check=True)            
 
-            #root.iconbitmap('uop.ico')
-            #root.configure(bg='white')
-
             fontsize = ("Helvetica", 18)
             fontsize1 = ("Helvetica", 22)
             fontsize2 = ("Helvetica", 12)
 
             root.attributes('-fullscreen', True)
 
             time_label = tk.Label(root, text="", font=fontsize)
@@ -349,18 +339,15 @@
             subprocess.run([python_path, file_path], check=True)
         
     main()
 
 else:
     import tkinter as tk
     errortext = "Your device is not connected to the internet, please connect to the internet to continue the task\n\nThe task must ensure that you have the correct files installed, which requires an active internet connection"
-    #root = tk.Tk()
-    #root.configure(bg='white')
 
     fontsize = ("Helvetica", 18)
     fontsize1 = ("Helvetica", 22)
     fontsize2 = ("Helvetica", 12)
 
-    #root.attributes('-fullscreen', True)
     from tkinter import simpledialog, messagebox
 
     messagebox.showerror("Error", errortext)
```

### Comparing `JBPhD-2.1.1/Task/__pycache__/Dependencies.cpython-311.pyc` & `JBPhD-2.1.3/Task/__pycache__/Dependencies.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/__pycache__/Export.cpython-311.pyc` & `JBPhD-2.1.3/Task/__pycache__/Export.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/__pycache__/Location.cpython-311.pyc` & `JBPhD-2.1.3/Task/__pycache__/Location.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/__pycache__/Task.cpython-311.pyc` & `JBPhD-2.1.3/Task/__pycache__/Task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/__pycache__/spwf.cpython-311.pyc` & `JBPhD-2.1.3/Task/__pycache__/spwf.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/asterisk.png` & `JBPhD-2.1.3/Task/asterisk.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/circle.jpg` & `JBPhD-2.1.3/Task/circle.jpg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/cpudeps.py` & `JBPhD-2.1.3/Task/cpudeps.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/cpudepsinstall.py` & `JBPhD-2.1.3/Task/cpudepsinstall.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/cpuexp.py` & `JBPhD-2.1.3/Task/cpuexp.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/cpunbak.py` & `JBPhD-2.1.3/Task/cpunbak.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/cpurt.py` & `JBPhD-2.1.3/Task/cpurt.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/cpuswitch.py` & `JBPhD-2.1.3/Task/cpuswitch.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/cputask.py` & `JBPhD-2.1.3/Task/cputask.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/greendot.png` & `JBPhD-2.1.3/Task/greendot.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/greentick.png` & `JBPhD-2.1.3/Task/greentick.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/redcross.png` & `JBPhD-2.1.3/Task/redcross.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/reddot.png` & `JBPhD-2.1.3/Task/reddot.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/setup.py` & `JBPhD-2.1.3/Task/setup.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/trial.jpeg` & `JBPhD-2.1.3/Task/trial.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/uop.ico` & `JBPhD-2.1.3/Task/uop.ico`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/uop.jpeg` & `JBPhD-2.1.3/Task/uop.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.1.1/Task/uop.png` & `JBPhD-2.1.3/Task/uop.png`

 * *Files identical despite different names*

