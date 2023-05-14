# Comparing `tmp/animateplot-0.2.1-py3-none-any.whl.zip` & `tmp/animateplot-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,14 @@
-Zip file size: 15083 bytes, number of entries: 7
+Zip file size: 18393 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx       37 b- defN 23-May-14 02:31 animateplot/__init__.py
+-rw-rw-r--  2.0 unx     3269 b- defN 23-May-14 02:31 animateplot/animat_plot.py
+-rw-rw-r--  2.0 unx       47 b- defN 23-Mar-06 03:21 animateplot/video/__init__.py
+-rw-rw-r--  2.0 unx      138 b- defN 23-Mar-06 03:02 animateplot/video/exceptions_animateplot.py
+-rw-rw-r--  2.0 unx     2122 b- defN 23-Mar-06 03:51 animateplot/video/video.py
 -rw-rw-r--  2.0 unx       35 b- defN 23-Mar-04 00:27 animatplot/__init__.py
 -rw-rw-r--  2.0 unx     2321 b- defN 23-Mar-04 05:05 animatplot/animat_plot.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-Mar-04 05:08 animateplot-0.2.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1236 b- defN 23-Mar-04 05:08 animateplot-0.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-04 05:08 animateplot-0.2.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Mar-04 05:08 animateplot-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      566 b- defN 23-Mar-04 05:08 animateplot-0.2.1.dist-info/RECORD
-7 files, 39410 bytes uncompressed, 14077 bytes compressed:  64.3%
+-rw-rw-r--  2.0 unx    35149 b- defN 23-May-14 02:40 animateplot-0.3.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2180 b- defN 23-May-14 02:40 animateplot-0.3.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-14 02:40 animateplot-0.3.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 23-May-14 02:40 animateplot-0.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      993 b- defN 23-May-14 02:40 animateplot-0.3.2.dist-info/RECORD
+12 files, 46395 bytes uncompressed, 16713 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -1,22 +1,37 @@
+Filename: animateplot/__init__.py
+Comment: 
+
+Filename: animateplot/animat_plot.py
+Comment: 
+
+Filename: animateplot/video/__init__.py
+Comment: 
+
+Filename: animateplot/video/exceptions_animateplot.py
+Comment: 
+
+Filename: animateplot/video/video.py
+Comment: 
+
 Filename: animatplot/__init__.py
 Comment: 
 
 Filename: animatplot/animat_plot.py
 Comment: 
 
-Filename: animateplot-0.2.1.dist-info/LICENSE
+Filename: animateplot-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: animateplot-0.2.1.dist-info/METADATA
+Filename: animateplot-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: animateplot-0.2.1.dist-info/WHEEL
+Filename: animateplot-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: animateplot-0.2.1.dist-info/top_level.txt
+Filename: animateplot-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: animateplot-0.2.1.dist-info/RECORD
+Filename: animateplot-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `animateplot-0.2.1.dist-info/LICENSE` & `animateplot-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `animateplot-0.2.1.dist-info/METADATA` & `animateplot-0.3.2.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,54 @@
 Metadata-Version: 2.1
 Name: animateplot
-Version: 0.2.1
+Version: 0.3.2
 Summary: Library for generate gif or video from plots
 Home-page: https://github.com/reinanbr/dreams
 Author: Reinan Br
 Author-email: slimchatuba@gmail.com
 License: BSD v3
 Keywords: gif video plot
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: imageio
 Requires-Dist: opencv-python
 
+<div align='center'>
 
+<img height='200'  width='200' src='imgs/logo.png'>
+<h2>AnimatePlot</h2>
 
+<p> Making video/gif from plot's</p>
+<a href='#'><img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/reinanbr/animatPlot?logo=codefactor">
+</a><img alt="CircleCI" src="https://img.shields.io/circleci/build/github/reinanbr/animatPlot">
+<img alt="Code Climate maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/reinanbr/animatPlot">
 
+<br/>
+<a href='https://pypi.org/project/animateplot/'><img src='https://img.shields.io/pypi/v/animateplot'></a>
+<a href='#'><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/animateplot"></a>
+<br/>
+<img alt="PyPI - License" src="https://img.shields.io/pypi/l/animateplot?color=orange">
 
 
 
+</div>
+
 
 
 ### Examples 
 
-coding:
+
+#### Gif 
+
 ```py
 import numpy as np
 import matplotlib.pyplot as ply
-from animatplot import AnimatPlot
+from animateplot import AnimatPlot # import AnimatPlot
 
 
 x = np.linspace(-10,10,200)
 np.seterr(all="ignore")
 
 def sig(x):
   return 1/(1+np.exp(-x))
@@ -44,17 +60,23 @@
   plt.xlabel('x')
   plt.ylabel('y')
   plt.xlim(-10,10)
   plt.ylim(0,1)
   return plt
 
 
+def test_render_gif():
+    anime = AnimatPlot(sig,x,callback_plot=call_plt)
+    anime.delete_cache()
+    anime.render_cache()
+    anime.render_gif('tests/gifs/sigmoid.gif')
+
 
-anime = AnimatPlot(sig,x,callback_plot=call_plt)
-anime.render_cache()
+
+test_render_gif()
 ```
 ```sh
 logs:
 ended saved cache images! 
 [200 images saved in 30.9s | speed: 6.5/img/s | ping: 15.5ms]
 [Figure size 576x396 with 0 Axes]
 ```
@@ -62,7 +84,9 @@
 ```py
 anime.render_gif(path='plot.gif',fps=8.7)
 ```
 ```sh
 logs: plot.gif saved in 6.8s
 ```
 <img src='https://github.com/reinanbr/animatPlot/blob/main/imgs/plot%20(9).gif?raw=true'>
+
+
```

