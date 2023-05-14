# Comparing `tmp/mml_qae-1.0.1.2.tar.gz` & `tmp/mml_qae-1.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mml_qae-1.0.1.2.tar", last modified: Sun May 14 06:54:34 2023, max compression
+gzip compressed data, was "dist\mml_qae-1.0.1.3.tar", last modified: Sun May 14 08:20:01 2023, max compression
```

## Comparing `mml_qae-1.0.1.2.tar` & `mml_qae-1.0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/
--rw-rw-rw-   0        0        0     3380 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2638 2023-05-14 06:46:51.000000 mml_qae-1.0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/mml_qae/
--rw-rw-rw-   0        0        0        0 2023-05-13 07:17:18.000000 mml_qae-1.0.1.2/mml_qae/__init__.py
--rw-rw-rw-   0        0        0     2808 2023-05-14 05:11:34.000000 mml_qae-1.0.1.2/mml_qae/lists_of_number.py
--rw-rw-rw-   0        0        0     1363 2023-05-13 08:27:02.000000 mml_qae-1.0.1.2/mml_qae/one_list_of_number.py
-drwxrwxrwx   0        0        0        0 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/mml_qae.egg-info/
--rw-rw-rw-   0        0        0     3380 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/mml_qae.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/mml_qae.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/mml_qae.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/mml_qae.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      668 2023-05-14 06:54:30.000000 mml_qae-1.0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/
+-rw-rw-rw-   0        0        0     3651 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2829 2023-05-14 08:19:44.000000 mml_qae-1.0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/mml_qae/
+-rw-rw-rw-   0        0        0     1664 2023-05-14 08:17:49.000000 mml_qae-1.0.1.3/mml_qae/MoreErrors.py
+-rw-rw-rw-   0        0        0        0 2023-05-13 07:17:18.000000 mml_qae-1.0.1.3/mml_qae/__init__.py
+-rw-rw-rw-   0        0        0     2897 2023-05-14 08:16:28.000000 mml_qae-1.0.1.3/mml_qae/lists_of_number.py
+-rw-rw-rw-   0        0        0     1399 2023-05-14 08:18:15.000000 mml_qae-1.0.1.3/mml_qae/one_list_of_number.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/mml_qae.egg-info/
+-rw-rw-rw-   0        0        0     3651 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/mml_qae.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/mml_qae.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/mml_qae.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/mml_qae.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      668 2023-05-14 08:19:54.000000 mml_qae-1.0.1.3/setup.py
```

### Comparing `mml_qae-1.0.1.2/PKG-INFO` & `mml_qae-1.0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 Metadata-Version: 2.1
 Name: mml_qae
-Version: 1.0.1.2
+Version: 1.0.1.3
 Summary: The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.
 Home-page: https://www.python.org
 Author: ETRO_secondleader
 Author-email: ETRO_gfyx@163.com
 License: UNKNOWN
 Description: # Python:mml-qae库帮助文档
         ## 使用环境
         + Python环境:最好使用3.7.2。如果不在3.7.2环境下出现报错，请区分ImportError(由mml内部引入包的版本错误)和其他错误。
         + 编译格式：没什么好说的，Python默认使用的Unicode和UTF-8解码格式。
         + 请尽可能保持mml-qae包的最新版本。1.2及以前的版本并不全面！
         ---
         ## 开发者发言
-        ##### We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with nature language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more porperly way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I can't promise how long the interval between two updataions. Another thing need to be attentioned, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will tell all of those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name to the built-in functions! And that's all. Have a nice day with MachineLearning and DataDealing!
+        + We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with nature language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more porperly way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I can't promise how long the interval between two updataions. Another thing need to be attentioned, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will tell all of those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name to the built-in functions! And that's all. Have a nice day with MachineLearning and DataDealing!
+        + Packages needed
+        > + statsmodels
+        > + sklearn
+        > + jieba
+        > + spaCy
+        > + pandas
+        > + numpy
+        > + matplotlib
+        > + wordcloud
         ---
         ## 历史版本(包括部分未公布的版本)
         + 1 简易大数据处理与网络构建
         > +  1.0 预发布版本
         > > + 1.0.0 
         >      初代版本，无项目描述。
         > > + 1.0.1
         >      修复1.0.0中的明显问题。
         > > > + 1.0.1.1  加入项目描述.
         > > > + 1.0.1.2  加入帮助文档README.md并修复一些小问题
+        > > > + 1.0.1.3  加入一些自定义错误和修复一些小问题
         > >  + 1.0.2
         >      加入封装好的自然语言处理快捷方法。
         > > > + 1.0.2.1  加入中文处理模型.
         > > > + 1.0.2.2  加入英语处理模型.
         > >  + 1.0.3     修复1.0版本的bug和问题。
         > +  1.1 完善版本
         > >  + 1.1.1 加入数据库处理方法。
```

### Comparing `mml_qae-1.0.1.2/README.md` & `mml_qae-1.0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 # Python:mml-qae库帮助文档
 ## 使用环境
 + Python环境:最好使用3.7.2。如果不在3.7.2环境下出现报错，请区分ImportError(由mml内部引入包的版本错误)和其他错误。
 + 编译格式：没什么好说的，Python默认使用的Unicode和UTF-8解码格式。
 + 请尽可能保持mml-qae包的最新版本。1.2及以前的版本并不全面！
 ---
 ## 开发者发言
-##### We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with nature language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more porperly way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I can't promise how long the interval between two updataions. Another thing need to be attentioned, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will tell all of those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name to the built-in functions! And that's all. Have a nice day with MachineLearning and DataDealing!
++ We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with nature language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more porperly way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I can't promise how long the interval between two updataions. Another thing need to be attentioned, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will tell all of those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name to the built-in functions! And that's all. Have a nice day with MachineLearning and DataDealing!
++ Packages needed
+> + statsmodels
+> + sklearn
+> + jieba
+> + spaCy
+> + pandas
+> + numpy
+> + matplotlib
+> + wordcloud
 ---
 ## 历史版本(包括部分未公布的版本)
 + 1 简易大数据处理与网络构建
 > +  1.0 预发布版本
 > > + 1.0.0 
 >      初代版本，无项目描述。
 > > + 1.0.1
 >      修复1.0.0中的明显问题。
 > > > + 1.0.1.1  加入项目描述.
 > > > + 1.0.1.2  加入帮助文档README.md并修复一些小问题
+> > > + 1.0.1.3  加入一些自定义错误和修复一些小问题
 > >  + 1.0.2
 >      加入封装好的自然语言处理快捷方法。
 > > > + 1.0.2.1  加入中文处理模型.
 > > > + 1.0.2.2  加入英语处理模型.
 > >  + 1.0.3     修复1.0版本的bug和问题。
 > +  1.1 完善版本
 > >  + 1.1.1 加入数据库处理方法。
```

### Comparing `mml_qae-1.0.1.2/mml_qae/lists_of_number.py` & `mml_qae-1.0.1.3/mml_qae/lists_of_number.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 #对多组数字参数的分析: 通过多组数据判断某一特征的目标
 import pandas as pd 
 import numpy as np
 from sklearn.model_selection import train_test_split as tts
 from sklearn.neighbors import KNeighborsClassifier as knc 
 from sklearn.metrics import accuracy_score as acc
-
+import MoreErrors as me
 def max_of_list(l:list):
     
     maxium=l[0]
     for i in l:
         try:
             i=float(i)
         except:
-            raise ValueError("列表含有非法的非纯数字项.")  
+            raise me.DataError2   
     for j in range(0,len(l)-1):
         a=l[j];b=l[j+1]
         if b>a:
             maxium=b
     return maxium        
 
 def cut(path:str,to_name:str,useless_name:str ):
     """给定csv文件路径path(以*.csv结尾)、csv文件中的目标组所在列名、csv文件中的无用列(如序号等)\n返回划分好的四个集合和初步预测模型"""
-    data1=pd.read_csv(path,header=0)#读入csv数据
-    data=data1.drop([useless_name],axis=1)#去除无用的id列
-    x_data=data.drop([to_name],axis=1)#从data中摘取特征组
-    y_data=np.ravel(data[[to_name]])#从data中摘取目标组
+    try:data1=pd.read_csv(path,header=0)#读入csv数据
+    except:raise me.CSVError
+    try: 
+        data=data1.drop([useless_name],axis=1)#去除无用的id列
+        x_data=data.drop([to_name],axis=1)#从data中摘取特征组
+        y_data=np.ravel(data[[to_name]])#从data中摘取目标组
+    except:raise me.DataError3    
     x_trainset , x_testset , y_trainset , y_testset = tts(x_data,y_data,random_state=1)
     #建立训练集(训练特征组 和 训练目标组)和测试集(测试特征组 和 训练目标组)
     n=range(1,30)
     KNNs=[knc(n_neighbors=i) for i in n]
     scores=[KNNs[i].fit(x_trainset,y_trainset).score(x_testset,y_testset) for i in range(len(KNNs))]
     best=max_of_list(scores)
     model=knc(algorithm="kd_tree",n_neighbors=best)#建立基础模型,用kd_tree算法做超级参数
@@ -46,10 +49,10 @@
     """给定csv文件路径path(以*.csv结尾)、csv文件中的目标组所在列名、csv文件中的无用列(如序号等)、需要预测的数据列(以pandas阅读csv文件结果的list格式给入)\n返回预测后的数据目标,过程中如果有错误则返回127错误."""
     model,x_trainset,y_trainset,x_testset,y_testset=cut(path=path,to_name=to_name,useless_name=useless_name)
     model.fit(x_trainset,y_trainset) 
     try:
         y_predict=model.predict(need_predict_list) 
         return y_predict
     except:
-        return 127
+        return me.DataError4
     
     #pip install -i https://pypi.org/project mml-qae
```

### Comparing `mml_qae-1.0.1.2/mml_qae/one_list_of_number.py` & `mml_qae-1.0.1.3/mml_qae/one_list_of_number.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import matplotlib.pyplot as plt 
 import statsmodels.api as sm
 import numpy as np 
+import MoreErrors as me
 def make_results(lista,listb,i=False):#给定两列表返回预测组 
     """给定两个列表(顺序:特征组,目标组)\n i值默认为假,不打印模型准确度;为真则打印准确度""" 
     X=lista
     Y=listb
     dX=np.column_stack((X,np.power(X,2),np.power(X,3),np.power(X,4),np.sin(X),np.tan(X),np.cos(X)  ))
     X_added=sm.add_constant(dX)
     model=sm.OLS(Y,X_added)
@@ -23,8 +24,8 @@
 def predict(X:list,Y:list,x:float ):
     """给定两个列表(顺序:特征组,目标组)和需要预测的数字\n返回需要预测的数字的预测结果(如果返回0则说明该值存在问题(如inf或nan)"""
     results=make_results(X,Y)
     try:
         p=results.predict([1,x,np.power(x,2),np.power(x,3),np.power(x,4),np.sin(x),np.tan(x),np.cos(x)])
         return p
     except:
-        return 0
+        raise me.DataError5
```

### Comparing `mml_qae-1.0.1.2/mml_qae.egg-info/PKG-INFO` & `mml_qae-1.0.1.3/mml_qae.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 Metadata-Version: 2.1
 Name: mml-qae
-Version: 1.0.1.2
+Version: 1.0.1.3
 Summary: The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.
 Home-page: https://www.python.org
 Author: ETRO_secondleader
 Author-email: ETRO_gfyx@163.com
 License: UNKNOWN
 Description: # Python:mml-qae库帮助文档
         ## 使用环境
         + Python环境:最好使用3.7.2。如果不在3.7.2环境下出现报错，请区分ImportError(由mml内部引入包的版本错误)和其他错误。
         + 编译格式：没什么好说的，Python默认使用的Unicode和UTF-8解码格式。
         + 请尽可能保持mml-qae包的最新版本。1.2及以前的版本并不全面！
         ---
         ## 开发者发言
-        ##### We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with nature language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more porperly way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I can't promise how long the interval between two updataions. Another thing need to be attentioned, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will tell all of those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name to the built-in functions! And that's all. Have a nice day with MachineLearning and DataDealing!
+        + We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with nature language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more porperly way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I can't promise how long the interval between two updataions. Another thing need to be attentioned, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will tell all of those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name to the built-in functions! And that's all. Have a nice day with MachineLearning and DataDealing!
+        + Packages needed
+        > + statsmodels
+        > + sklearn
+        > + jieba
+        > + spaCy
+        > + pandas
+        > + numpy
+        > + matplotlib
+        > + wordcloud
         ---
         ## 历史版本(包括部分未公布的版本)
         + 1 简易大数据处理与网络构建
         > +  1.0 预发布版本
         > > + 1.0.0 
         >      初代版本，无项目描述。
         > > + 1.0.1
         >      修复1.0.0中的明显问题。
         > > > + 1.0.1.1  加入项目描述.
         > > > + 1.0.1.2  加入帮助文档README.md并修复一些小问题
+        > > > + 1.0.1.3  加入一些自定义错误和修复一些小问题
         > >  + 1.0.2
         >      加入封装好的自然语言处理快捷方法。
         > > > + 1.0.2.1  加入中文处理模型.
         > > > + 1.0.2.2  加入英语处理模型.
         > >  + 1.0.3     修复1.0版本的bug和问题。
         > +  1.1 完善版本
         > >  + 1.1.1 加入数据库处理方法。
```

### Comparing `mml_qae-1.0.1.2/setup.py` & `mml_qae-1.0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools 
 
 with open("README.md", "r",encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='mml_qae',
-      version='1.0.1.2',
+      version='1.0.1.3',
       description='The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='ETRO_secondleader',
       author_email='ETRO_gfyx@163.com',
       url='https://www.python.org', 
       packages=setuptools.find_packages(),
```

