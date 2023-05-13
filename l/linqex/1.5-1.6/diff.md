# Comparing `tmp/linqex-1.5.tar.gz` & `tmp/linqex-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linqex-1.5.tar", last modified: Mon May  1 00:27:34 2023, max compression
+gzip compressed data, was "linqex-1.6.tar", last modified: Sat May 13 22:56:58 2023, max compression
```

## Comparing `linqex-1.5.tar` & `linqex-1.6.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 00:27:34.531782 linqex-1.5/
--rw-rw-rw-   0        0        0     1084 2023-02-12 13:59:17.000000 linqex-1.5/LICENSE
--rw-rw-rw-   0        0        0     5936 2023-05-01 00:27:34.530780 linqex-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     5402 2023-04-30 23:59:14.000000 linqex-1.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 00:27:34.475268 linqex-1.5/linqex/
--rw-rw-rw-   0        0        0       55 2023-04-10 13:14:49.000000 linqex-1.5/linqex/__init__.py
--rw-rw-rw-   0        0        0      478 2023-04-18 21:14:02.000000 linqex-1.5/linqex/_typing.py
-drwxrwxrwx   0        0        0        0 2023-05-01 00:27:34.519896 linqex-1.5/linqex/build/
--rw-rw-rw-   0        0        0      373 2023-04-10 13:52:19.000000 linqex-1.5/linqex/build/__init__.py
--rw-rw-rw-   0        0        0     1419 2023-04-19 22:25:23.000000 linqex-1.5/linqex/build/iterablebase.py
--rw-rw-rw-   0        0        0    15234 2023-04-30 22:40:47.000000 linqex-1.5/linqex/build/iterdictbase.py
--rw-rw-rw-   0        0        0    12940 2023-04-30 23:28:45.000000 linqex-1.5/linqex/build/iteritembase.py
--rw-rw-rw-   0        0        0    13272 2023-04-30 23:05:53.000000 linqex-1.5/linqex/build/iterlistbase.py
-drwxrwxrwx   0        0        0        0 2023-05-01 00:27:34.528541 linqex-1.5/linqex/linq/
--rw-rw-rw-   0        0        0      334 2023-04-10 13:52:07.000000 linqex-1.5/linqex/linq/__init__.py
--rw-rw-rw-   0        0        0     1350 2023-04-30 23:37:35.000000 linqex-1.5/linqex/linq/iterable.py
--rw-rw-rw-   0        0        0    15400 2023-04-20 17:18:12.000000 linqex-1.5/linqex/linq/iterdict.py
--rw-rw-rw-   0        0        0    14391 2023-04-30 23:27:34.000000 linqex-1.5/linqex/linq/iteritem.py
--rw-rw-rw-   0        0        0    15035 2023-04-20 17:17:26.000000 linqex-1.5/linqex/linq/iterlist.py
-drwxrwxrwx   0        0        0        0 2023-05-01 00:27:34.511999 linqex-1.5/linqex.egg-info/
--rw-rw-rw-   0        0        0     5936 2023-05-01 00:27:34.000000 linqex-1.5/linqex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-05-01 00:27:34.000000 linqex-1.5/linqex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 00:27:34.000000 linqex-1.5/linqex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-01 00:27:34.000000 linqex-1.5/linqex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 00:27:34.531782 linqex-1.5/setup.cfg
--rw-rw-rw-   0        0        0     1240 2023-05-01 00:00:05.000000 linqex-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:56:58.829916 linqex-1.6/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 13:59:17.000000 linqex-1.6/LICENSE
+-rw-rw-rw-   0        0        0     5936 2023-05-13 22:56:58.827912 linqex-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5402 2023-04-30 23:59:14.000000 linqex-1.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-13 22:56:58.748748 linqex-1.6/linqex/
+-rw-rw-rw-   0        0        0       72 2023-05-13 18:57:28.000000 linqex-1.6/linqex/__init__.py
+-rw-rw-rw-   0        0        0      478 2023-04-18 21:14:02.000000 linqex-1.6/linqex/_typing.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:56:58.802913 linqex-1.6/linqex/abstract/
+-rw-rw-rw-   0        0        0      120 2023-05-13 19:47:55.000000 linqex-1.6/linqex/abstract/__init__.py
+-rw-rw-rw-   0        0        0    20120 2023-05-13 22:24:58.000000 linqex-1.6/linqex/abstract/iterable.py
+-rw-rw-rw-   0        0        0    17446 2023-05-13 22:25:29.000000 linqex-1.6/linqex/abstract/iterablebase.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:56:58.816916 linqex-1.6/linqex/build/
+-rw-rw-rw-   0        0        0      262 2023-05-13 19:23:04.000000 linqex-1.6/linqex/build/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-05-13 21:41:36.000000 linqex-1.6/linqex/build/iterablebase.py
+-rw-rw-rw-   0        0        0    15688 2023-05-13 22:17:24.000000 linqex-1.6/linqex/build/iterdictbase.py
+-rw-rw-rw-   0        0        0    12793 2023-05-13 21:59:21.000000 linqex-1.6/linqex/build/iteritembase.py
+-rw-rw-rw-   0        0        0    13605 2023-05-13 22:16:46.000000 linqex-1.6/linqex/build/iterlistbase.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:56:58.826910 linqex-1.6/linqex/linq/
+-rw-rw-rw-   0        0        0      217 2023-05-13 19:21:58.000000 linqex-1.6/linqex/linq/__init__.py
+-rw-rw-rw-   0        0        0     1607 2023-05-13 21:41:43.000000 linqex-1.6/linqex/linq/iterable.py
+-rw-rw-rw-   0        0        0    15777 2023-05-13 22:18:53.000000 linqex-1.6/linqex/linq/iterdict.py
+-rw-rw-rw-   0        0        0    14724 2023-05-13 22:18:45.000000 linqex-1.6/linqex/linq/iteritem.py
+-rw-rw-rw-   0        0        0    15358 2023-05-13 21:58:10.000000 linqex-1.6/linqex/linq/iterlist.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:56:58.793913 linqex-1.6/linqex.egg-info/
+-rw-rw-rw-   0        0        0     5936 2023-05-13 22:56:58.000000 linqex-1.6/linqex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-05-13 22:56:58.000000 linqex-1.6/linqex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-13 22:56:58.000000 linqex-1.6/linqex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-13 22:56:58.000000 linqex-1.6/linqex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-13 22:56:58.829916 linqex-1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1240 2023-05-13 22:34:40.000000 linqex-1.6/setup.py
```

### Comparing `linqex-1.5/LICENSE` & `linqex-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `linqex-1.5/PKG-INFO` & `linqex-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linqex
-Version: 1.5
+Version: 1.6
 Summary: The linq module in C# has been adapted for python with some modifications.
 Home-page: https://github.com/TahsinCr/python-linqex
 Author: TahsinCr
 Author-email: TahsinCr@outlook.com
 License: MIT
 Keywords: linq,linqex,ex,enumerable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linqex-1.5/README.rst` & `linqex-1.6/README.rst`

 * *Files identical despite different names*

### Comparing `linqex-1.5/linqex/build/iterablebase.py` & `linqex-1.6/linqex/linq/iterable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from linqex._typing import *
-from linqex.build.iterdictbase import EnumerableDictBase
-from linqex.build.iterlistbase import EnumerableListBase
-from linqex.build.iteritembase import EnumerableItemBase
+from linqex.abstract.iterable import AbstractEnumerable
+from linqex.linq.iterdict import EnumerableDict, EnumerableDictBase
+from linqex.linq.iterlist import EnumerableList, EnumerableListBase
+from linqex.linq.iteritem import EnumerableItem, EnumerableItemBase
 
 from typing import Dict, List, Union, Generic
 
 
-class EnumerableBase(Generic[_TK,_TV]):
+class Enumerable(Generic[_TK,_TV]):
     def __new__(cls, iterable:Union[List[_TV],Dict[_TK,_TV]]):
         return cls.Iterable(iterable)
     @classmethod
-    def Iterable(cls, iterable:Union[List[_TV],Dict[_TK,_TV]]) -> Union[EnumerableItemBase[_TV], EnumerableDictBase[_TK,_TV]]:
+    def Iterable(cls, iterable:Union[List[_TV],Dict[_TK,_TV]]) -> Union[EnumerableItem[_TV], EnumerableDict[_TK,_TV]]:
         if isinstance(iterable, list):
             return cls.Item(iterable)
         elif isinstance(iterable, dict):
             return cls.Dict(iterable)
         else:
-            raise TypeError()
+            raise TypeError("Must be list or dict, not {}".format(str(type(iterable))[8,-2]))
 
     @classmethod
-    def Item(cls, iteritem:List[_TV]=None) -> EnumerableItemBase[_TV]:
+    def Item(cls, iteritem:List[_TV]=None) -> EnumerableItem[_TV]:
         if iteritem is None:
             iteritem:List[_TV]=list()
-        return EnumerableItemBase(iteritem)
+        return EnumerableItem(iteritem)
 
     @classmethod
-    def List(cls, iterlist:List[_TV]=None) -> EnumerableListBase[_TV]:
+    def List(cls, iterlist:List[_TV]=None) -> EnumerableList[_TV]:
         if iterlist is None:
             iterlist:List[_TV]=list()
-        return EnumerableListBase(iterlist)
+        return EnumerableList(iterlist)
 
     @classmethod
-    def Dict(cls, iterdict:Dict[_TK,_TV]=None) -> EnumerableDictBase[_TK,_TV]:
+    def Dict(cls, iterdict:Dict[_TK,_TV]=None) -> EnumerableDict[_TK,_TV]:
         if iterdict is None:
             iterdict:Dict[_TK,_TV]=dict()
-        return EnumerableDictBase(iterdict)
+        return EnumerableDict(iterdict)
 
 
-
-__all__ = ["EnumerableBase"]
+__all__ = ["AbstractEnumerable", "EnumerableList", "EnumerableItem", "EnumerableDict", "Enumerable"]
```

### Comparing `linqex-1.5/linqex/build/iterdictbase.py` & `linqex-1.6/linqex/build/iterlistbase.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,395 +1,393 @@
 from linqex._typing import *
+from linqex.abstract.iterablebase import AbstractEnumerableBase
 
-from typing import Dict, List, Callable, Union as _Union, NoReturn, Optional, Tuple, Type, Generic
+from typing import Dict, List, Callable, Union as _Union, NoReturn, Optional, Tuple, Type, Generic, Self
 from numbers import Number
 from collections.abc import Iterable
 import itertools
 
-class EnumerableDictBase(Iterable[Tuple[_TK,_TV]],Generic[_TK,_TV]):
+class EnumerableListBase(AbstractEnumerableBase, Iterable[_TV], Generic[_TV]):
     
-    def __init__(self, iterdict:Optional[Dict[_TK,_TV]]=None):
-        if iterdict is None:
-            iterdict:Dict[_TK,_TV] = dict()
-        if isinstance(iterdict, dict):
-            self.iterdict:Dict[_TK,_TV] = iterdict
-        elif isinstance(iterdict, list):
-            self.iterdict:Dict[_TK,_TV] = dict(iterdict)
+    def __init__(self, iterable:Optional[List[_TV]]=None):
+        if iterable is None:
+            iterable:List[_TV] = list()
+        if isinstance(iterable, list):
+            self.iterable:List[_TV] = iterable
+        elif isinstance(iterable, (tuple, set)):
+            self.iterable:List[_TV] = list(iterable)
         else:
-            raise TypeError(iterdict)
+            raise TypeError("Must be tuple, set and list, not {}".format(str(type(iterable))[8,-2]))
 
-    def Get(self, *key:_TK) -> _Union[Dict[_TK,_TV],_TV]:
-        iterdict = self.iterdict
+    def Get(self, *key:int) -> _Union[List[_TV],_TV]:
+        iterable = self.iterable
         for k in key:
-            if  k in EnumerableDictBase(iterdict).GetKeys():
-                iterdict = iterdict[k]
+            if  k < len(iterable):
+                iterable = iterable[k]
             else:
-                raise KeyError(k)
-        return iterdict
+                raise IndexError(k)
+        return iterable
     
-    def GetKey(self, value:_TV) -> _TK:
-        return {v: k for k, v in self.GetItems()}[value]
+    def GetKey(self, value:_TV) -> int:
+        return self.iterable.index(value)
     
-    def GetKeys(self) -> List[_TK]:
-        return list(self.Get().keys())
+    def GetKeys(self) -> List[int]:
+        return list(range(len(self.Get())))
     
     def GetValues(self) -> List[_TV]:
-        return list(self.Get().values())
+        return self.Get()
     
-    def GetItems(self) -> List[Tuple[_TK,_TV]]:
-        return list(self.Get().items())
+    def GetItems(self) -> List[Tuple[int,_TV]]:
+        return list(enumerate(self.Get()))
     
-    def Copy(self) -> Dict[_TK,_TV]:
+    def Copy(self) -> List[_TV]:
         return self.Get().copy()
 
 
 
-    def Take(self, count:int) -> Dict[_TK,_TV]:
-        return dict(self.GetItems()[:count])
+    def Take(self, count:int) -> List[_TV]:
+        return self.Get()[:count]
     
-    def TakeLast(self, count:int) -> Dict[_TK,_TV]:
+    def TakeLast(self, count:int) -> List[_TV]:
         return self.Skip(self.Lenght()-count)
     
-    def Skip(self, count:int) -> Dict[_TK,_TV]:
-        return dict(self.GetItems()[count:])
+    def Skip(self, count:int) -> List[_TV]:
+        return self.Get()[count:]
     
-    def SkipLast(self, count:int) -> Dict[_TK,_TV]:
+    def SkipLast(self, count:int) -> List[_TV]:
         return self.Take(self.Lenght()-count)
     
-    def Select(self, selectFunc:Callable[[_TK,_TV],_TFV]=lambda key, value: value, selectFuncByKey:Callable[[_TK,_TV],_TFK]=lambda key, value: key) -> Dict[_TFK,_TFV]:
-        return dict(list(map(lambda key, value: (selectFuncByKey(key,value), selectFunc(key,value)), self.GetKeys(), self.GetValues())))
+    def Select(self, selectFunc:Callable[[_TV],_TFV]=lambda value: value) -> List[_TFV]:
+        return list(map(selectFunc,self.Get()))
     
-    def Distinct(self, distinctFunc:Callable[[_TK,_TV],_TFV]=lambda key, value: value) -> Dict[_TK,_TV]:
-        newIterdict = self.Copy()
+    def Distinct(self, distinctFunc:Callable[[_TV],_TFV]=lambda value: value) -> List[_TV]:
+        newIterable = self.Copy()
+        indexStep = 0
         for key, value in self.GetItems():
-            if EnumerableDictBase(EnumerableDictBase(newIterdict).Select(distinctFunc)).Count(distinctFunc(key, value)) > 1:
-                EnumerableDictBase(newIterdict).Delete(key)
-        return newIterdict
-    
-    def Except(self, exceptFunc:Callable[[_TK,_TV],_TFV]=lambda key, value: value, *value:_TV) -> Dict[_TK,_TV]:
-        newIterdict = EnumerableDictBase()
-        for k, v in self.GetItems():
-            if not exceptFunc(k,v) in value:
-                newIterdict.Add(k,v)
-        return newIterdict.Get()
-
-    def Join(self, iterdict: Dict[_TK2,_TV2], 
-        innerFunc:Callable[[_TK,_TV],_TFV]=lambda key, value: value, 
-        outerFunc:Callable[[_TK2,_TV2],_TFV]=lambda key, value: value, 
-        joinFunc:Callable[[_TK,_TV,_TK2,_TV2],_TFV2]=lambda inKey, inValue, outKey, outValue: (inValue, outValue),
-        joinFuncByKey:Callable[[_TK,_TV,_TK2,_TV2],_TFK2]=lambda inKey, inValue, outKey, outValue: inKey,
+            if EnumerableListBase(EnumerableListBase(newIterable).Select(distinctFunc)).Count(distinctFunc(value)) > 1:
+                EnumerableListBase(newIterable).Delete(key-indexStep)
+                indexStep += 1
+        return newIterable
+    
+    def Except(self, exceptFunc:Callable[[_TV],_TFV]=lambda value: value, *value:_TV) -> List[_TV]:
+        newIterable = EnumerableListBase()
+        for v in self.Get():
+            if not exceptFunc(v) in value:
+                newIterable.Add(v)
+        return newIterable.Get()
+
+    def Join(self, iterable: List[_TV2], 
+        innerFunc:Callable[[_TV],_TFV]=lambda value: value, 
+        outerFunc:Callable[[_TV2],_TFV]=lambda value: value, 
+        joinFunc:Callable[[_TV,_TV2],_TFV2]=lambda inValue, outValue: (inValue, outValue),
         joinType:JoinType=JoinType.INNER
-    ) -> Dict[_TFK2,_TFV2]:
-        def innerJoin(innerIterdict:Dict[_TK,_TV], outerIterdict:Dict[_TK2,_TV2], newIterdict:List[Tuple[_TK,_TV,_TK2,_TV2]]):
+    ) -> List[_TFV2]:
+        def innerJoin(innerIterable:List[_TV], outerIterable:List[_TV2], newIterable:EnumerableListBase[Tuple[_TV,_TV2]]):
             nonlocal outerFunc, innerFunc
-            for inKey, inValue in EnumerableDictBase(innerIterdict).GetItems():
-                outer = EnumerableDictBase(outerIterdict).Where(lambda outKey, outValue: outerFunc(outKey,outValue) == innerFunc(inKey, inValue))
+            for inValue in innerIterable:
+                outer = EnumerableListBase(outerIterable).Where(lambda outValue: outerFunc(outValue) == innerFunc(inValue))
                 if outer != []:
-                    for outKey, outValue in outer:
-                        newIterdict.append((inKey, inValue, outKey, outValue))
-        def leftJoin(innerIterdict:Dict[_TK,_TV], outerIterdict:Dict[_TK2,_TV2], newIterdict:List[Tuple[_TK,_TV,_TK2,_TV2]]):
+                    for out in outer:
+                        newIterable.Add((inValue, out[1]))
+        def leftJoin(innerIterable:List[_TV], outerIterable:List[_TV2], newIterable:EnumerableListBase[Tuple[_TV,Optional[_TV2]]]):
             nonlocal outerFunc, innerFunc
-            for inKey, inValue in EnumerableDictBase(innerIterdict).GetItems():
-                outer = EnumerableDictBase(outerIterdict).First(lambda outKey, outValue: outerFunc(outKey, outValue) == innerFunc(inKey, inValue))
+            for inValue in innerIterable:
+                outer = EnumerableListBase(outerIterable).First(lambda outValue: outerFunc(outValue) == innerFunc(inValue))
                 if outer is None:
-                    newIterdict.append((inKey, inValue, None, None))
+                    newIterable.Add((inValue, None))
                 else:
-                    newIterdict.append((inKey, inValue, outer[0], outer[1]))
-        def rightJoin(innerIterdict:Dict[_TK,_TV], outerIterdict:Dict[_TK2,_TV2], newIterdict:List[Tuple[_TK,_TV,_TK2,_TV2]]):
+                    newIterable.Add((inValue, outer[1]))
+        def rightJoin(innerIterable:List[_TV], outerIterable:List[_TV2], newIterable:EnumerableListBase[Tuple[_TV2,Optional[_TV]]]):
             nonlocal outerFunc, innerFunc
-            for outKey, outValue in EnumerableDictBase(outerIterdict).GetItems():
-                inner = EnumerableDictBase(innerIterdict).First(lambda inKey, inValue: outerFunc(outKey, outValue) == innerFunc(inKey, inValue))
+            for outValue in outerIterable:
+                inner = EnumerableListBase(innerIterable).First(lambda inValue: outerFunc(outValue) == innerFunc(inValue))
                 if inner is None:
-                    newIterdict.append((None, None, outKey, outValue))
+                    newIterable.Add((None, outValue))
                 else:
-                    newIterdict.append((inner[0], inner[1], outKey, outValue))        
-        newIterdict:List[Tuple[_TK,_TV,_TK2,_TV2]] = []
+                    newIterable.Add((inner[1], outValue))
+        newIterable = EnumerableListBase()
         if joinType == JoinType.INNER:
             joinTypeFunc = innerJoin
         elif joinType == JoinType.LEFT:
             joinTypeFunc = leftJoin
         elif joinType == JoinType.RIGHT:
             joinTypeFunc = rightJoin
-        joinTypeFunc(self.Get(), iterdict, newIterdict)
-        joinKeys = list(map(lambda value: joinFuncByKey(value[0], value[1], value[2], value[3]), newIterdict))
-        joinValues = list(map(lambda value: joinFunc(value[0], value[1], value[2], value[3]), newIterdict))
-        joinItems = list(zip(joinKeys, joinValues))
-        return dict(joinItems)        
+        joinTypeFunc(self.Get(), iterable, newIterable)
+        return newIterable.Select(lambda value: joinFunc(value[0], value[1]))         
       
-    def OrderBy(self, *orderByFunc:Tuple[Callable[[_TK,_TV],_Union[Tuple[_TFV],_TFV]],_Desc]) -> Dict[_TK,_TV]:
+    def OrderBy(self, *orderByFunc:Tuple[Callable[[_TV],_Union[Tuple[_TFV],_TFV]],_Desc]) -> List[_TV]:
         if orderByFunc == ():
-            orderByFunc = ((lambda key, value: value, False))
-        iterdict = self.GetItems()
+            orderByFunc = ((lambda value: value, False))
+        iterable = self.Get()
         orderByFunc:list = list(reversed(orderByFunc))
         for func, desc in orderByFunc:
-            iterdict = sorted(iterdict, key=lambda x: func(x[0],x[1]), reverse=desc)
-        return dict(iterdict)
+            iterable = sorted(iterable, key=func, reverse=desc)
+        return list(iterable)
         
-    def GroupBy(self, groupByFunc:Callable[[_TK,_TV],_Union[Tuple[_TFV],_TFV]]=lambda key, value: value) -> Dict[_Union[Tuple[_TFV],_TFV], Dict[_TK,_TV]]:
-        iterdict = EnumerableDictBase(self.OrderBy((groupByFunc, False))).GetItems()
-        iterdict = itertools.groupby(iterdict, lambda items: groupByFunc(items[0], items[1]))
-        return {keys : dict(group) for keys, group in iterdict}
+    def GroupBy(self, groupByFunc:Callable[[_TV],_Union[Tuple[_TFV],_TFV]]=lambda value: value) -> List[Tuple[_Union[Tuple[_TFV],_TFV], List[_TV]]]:
+        iterable = self.OrderBy((groupByFunc, False))
+        iterable = itertools.groupby(iterable, groupByFunc)
+        return [(keys, list(group)) for keys, group in iterable]
 
-    def Reverse(self) -> Dict[_TK,_TV]:
-            return dict(zip(reversed(self.GetKeys()),reversed(self.GetValues())))
+    def Reverse(self) -> List[_TV]:
+        return list(reversed(self.Get()))
         
-    def Zip(self, iterdict:Dict[_TK2,_TV2], 
-        zipFunc:Callable[[_TK,_TV,_TK2,_TV2],_TFV]=lambda inKey, inValue, outKey, outValue: (inValue, outValue),
-        zipFuncByKey:Callable[[_TK,_TV,_TK2,_TV2],_TFK]=lambda inKey, inValue, outKey, outValue: inKey
-    ) -> Dict[_TFK,_TFV]:
-        newIterdict = EnumerableDictBase(dict(zip(self.GetKeys(),list(zip(self.GetValues(), EnumerableDictBase(iterdict).GetItems())))))
-        return newIterdict.Select(lambda key, value: zipFunc(key, value[0], value[1][0], value[1][1]), lambda key, value: zipFuncByKey(key, value[0], value[1][0], value[1][1]))
+    def Zip(self, iterable:List[_TV2], zipFunc:Callable[[_TV,_TV2],_TFV]=lambda inValue, outValue: (inValue, outValue)) -> List[_TFV]:
+        newIterable = EnumerableListBase(list(zip(self.GetValues(), EnumerableListBase(iterable).GetValues())))
+        return newIterable.Select(lambda value: zipFunc(value[0], value[1]))
 
 
 
-    def Where(self, conditionFunc:Callable[[_TK,_TV],bool]=lambda key, value: True) -> List[Tuple[_TK,_TV]]:
+    def Where(self, conditionFunc:Callable[[_TV],bool]=lambda value: True) -> List[Tuple[int,_TV]]:
         result = list()
-        for key, value in self.GetItems():
-            if conditionFunc(key, value):
-                result.append((key, value))
+        for index, value in self.GetItems():
+            if conditionFunc(value):
+                result.append((index, value))
         return result
     
-    def OfType(self, *type:Type) -> List[Tuple[_TK,_TV]]:
-        return self.Where(lambda key, value: isinstance(value,type))
+    def OfType(self, *type:Type) -> List[Tuple[int,_TV]]:
+        return self.Where(lambda value: isinstance(value,type))
     
-    def OfTypeByKey(self, *type:Type) -> List[Tuple[_TK,_TV]]:
-        return self.Where(lambda key, value: isinstance(key,type))
-    
-    def First(self, conditionFunc:Callable[[_TK,_TV],bool]=lambda key, value: True) -> Optional[Tuple[_TK,_TV]]:
-        for key, value in self.GetItems():
-            if conditionFunc(key, value):
-                return (key,value)
+    def First(self, conditionFunc:Callable[[_TV],bool]=lambda value: True) -> Optional[Tuple[int,_TV]]:
+        for index, value in self.GetItems():
+            if conditionFunc(value):
+                return (index,value)
         return None
     
-    def Last(self, conditionFunc:Callable[[_TK,_TV],bool]=lambda key, value: True) -> Optional[Tuple[_TK,_TV]]:
+    def Last(self, conditionFunc:Callable[[_TV],bool]=lambda value: True) -> Optional[Tuple[int,_TV]]:
         result = self.Where(conditionFunc)
         if len(result) == 0:
             return None
         else:
             return result[-1]
         
-    def Single(self, conditionFunc:Callable[[_TK,_TV],bool]=lambda key, value: True) -> Optional[Tuple[_TK,_TV]]:
+    def Single(self, conditionFunc:Callable[[_TV],bool]=lambda value: True) -> Optional[Tuple[int,_TV]]:
         result = self.Where(conditionFunc)
         if len(result) != 1:
             return None
         else:
             return result[0]
 
 
 
-    def Any(self, conditionFunc:Callable[[_TK,_TV],bool]=lambda key, value: True) -> bool:
+    def Any(self, conditionFunc:Callable[[_TV],bool]=lambda value: value) -> bool:
         result = False
-        for key, value in self.GetItems():
-            if conditionFunc(key, value):
+        for value in self.Get():
+            if conditionFunc(value):
                 result = True
                 break
         return result
     
-    def All(self, conditionFunc:Callable[[_TK,_TV],bool]=lambda key, value: True) -> bool:
+    def All(self, conditionFunc:Callable[[_TV],bool]=lambda value: value) -> bool:
         result = True
-        for key, value in self.GetItems():
-            if not conditionFunc(key, value):
+        for value in self.Get():
+            if not conditionFunc(value):
                 result = False
                 break
         return result
     
-    def SequenceEqual(self, iterdict:Dict[_TK2,_TV2]) -> bool:
-        if self.Lenght() != len(iterdict):
+    def SequenceEqual(self, iterable:List[_TV2]) -> bool:
+        if self.Lenght() != len(iterable):
             return False
-        for key, value in self.GetItems():
-            if key in iterdict.keys():
-                if not iterdict[key] == value:
-                    return False
-            else:
+        for value in self.Get():
+            if not value in iterable:
                 return False
         return True
 
 
 
-    def Accumulate(self, accumulateFunc:Callable[[_TV,_TK,_TV],_TFV]=lambda temp, key, nextValue: temp + nextValue) -> Dict[_TK,_TFV]:
-        firstTemp:bool = True
-        def FirstTemp(temp):
-            nonlocal firstTemp
-            if firstTemp:
-                firstTemp = False
-                return temp[1]
-            else:
-                return temp
-        if not self.IsEmpty():
-            result = dict([self.GetItems()[0]])
-            result.update(dict(zip(self.GetKeys()[1:], list(itertools.accumulate(self.GetItems(), lambda temp, next: accumulateFunc(FirstTemp(temp), next[0], next[1])))[1:])))
-            return result
-        else:
-            return {}
-        
-    def Aggregate(self, accumulateFunc:Callable[[_TV,_TK,_TV],_TFV]=lambda temp, key, nextValue: temp + nextValue) -> _TFV:
-        return EnumerableDictBase(self.Accumulate(accumulateFunc)).GetValues()[-1]
+    def Accumulate(self, accumulateFunc:Callable[[_TV,_TV],_TFV]=lambda temp, nextValue: temp + nextValue) -> List[_TFV]:
+        return list(itertools.accumulate(self.Get(), lambda temp, next: accumulateFunc(temp, next)))
+
+    def Aggregate(self, accumulateFunc:Callable[[_TV,_TV],_TFV]=lambda temp, nextValue: temp + nextValue) -> _TFV:
+        return self.Accumulate(accumulateFunc)[-1]
+
 
 
 
     def Count(self, value:_TV) -> int:
         return self.GetValues().count(value)
         
     def Lenght(self) -> int:
         return len(self.Get())
     
     def Sum(self) -> Optional[_TV]:
         if self.OfType(Number):
-            return sum(self.GetValues())
+            return sum(self.Get())
         else:
             return None
         
     def Avg(self) -> Optional[_TV]:
         if self.OfType(Number):
-            return sum(self.GetValues()) / self.Lenght()
+            return sum(self.Get()) / self.Lenght()
         else:
             return None
         
     def Max(self) -> Optional[_TV]:
         if self.OfType(Number):
-            return max(self.GetValues())
+            return max(self.Get())
         else:
             return None
         
     def Min(self) -> Optional[_TV]:
+        iterable = self.GetValues()
         if self.OfType(Number):
-            return min(self.GetValues())
+            return min(iterable)
         else:
             return None
 
 
 
+    def Add(self, value:_Value):
+        self.Get().append(value)
 
-    def Add(self, key:_Key, value:_Value):
-        self.Get()[key] = value
+    def Prepend(self, value:_Value):
+        newIterable = [value]
+        self.Clear()
+        self.Concat(newIterable)
 
-    def Update(self, key:_TK, value:_Value):
-        if key in self.GetKeys():
-            self.Get()[key] = value
-        else:
-            raise KeyError(key)
+    def Insert(self, key:_Key, value:_Value):
+        self.Get().insert(key, value)
+
+    def Update(self, key:int, value:_Value):
+        self.Get()[key] = value
 
-    def Concat(self, *iterdict:Dict[_TK2,_TV2]):
-        for i in iterdict:
-            self.Get().update(i)
-
-    def Union(self, *iterdict:Dict[_TK2,_TV2]):
-        if not iterdict in [(),[]]:
-            iterdict:list = list(iterdict)
-            newIterdict = EnumerableDictBase()
-            filter = dict(self.Where(lambda k, v: v in iterdict[0].values() and k in iterdict[0].keys()))
-            EnumerableDictBase(filter).Loop(lambda k, v: newIterdict.Add(k, v))
-            iterdict.pop(0)
+    def Concat(self, *iterable:List[_Value]):
+        for i in iterable:
+            self.Get().extend(i)
+
+    def Union(self, *iterable:List[_Value]):
+        if not iterable in [(),[]]:
+            iterable:list = list(iterable)
+            newIterable = EnumerableListBase()
+            filter = dict(self.Where(lambda v: v in iterable[0]))
+            EnumerableListBase(filter).Loop(lambda v: newIterable.Add(v))
+            iterable.pop(0)
             self.Clear()
-            self.Concat(newIterdict.Get())
-            self.Union(*iterdict)
+            self.Concat(newIterable.Get())
+            self.Union(*iterable)
 
-    def Delete(self, *key:_TK):
-        for k in key:
+    def Delete(self, *key:int):
+        i = 0
+        for k in sorted(key):
+            k -= i
             self.Get().pop(k)
+            i += 1
 
     def Remove(self, *value:_TV):
         for v in value:
-            self.Get().pop(self.First(lambda k, val: val == v)[0])
+            self.Get().remove(v)
 
     def RemoveAll(self, *value:_TV):
         for v in value:
             while True:
                 if self.Contains(v):
                     self.Remove(v)
                 else:
                     break
 
     def Clear(self):
         self.Get().clear()
 
 
 
-    def Loop(self, loopFunc:Callable[[_TK,_TV],NoReturn]=lambda key, value: print(key,value)):
-        for key, value in self.GetItems():
-            loopFunc(key, value)
+    def Loop(self, loopFunc:Callable[[_TV],NoReturn]=lambda value: print(value)):
+        for value in self.Get():
+            loopFunc(value)
 
 
 
-    def ToDict(self) -> Dict[_TK,_TV]:
-        return self.Get()
+    def ToDict(self) -> Dict[int,_TV]:
+        return dict(self.GetItems())
 
     def ToList(self) -> List[_TV]:
-        return self.GetValues()
+        return self.Get()
 
 
 
     def IsEmpty(self) -> bool:
-        return self.Get() in [[],{},None]
-    
-    def ContainsByKey(self, *key:_TK) -> bool:
-        iterdict = self.GetKeys()
+        return self.Get() in [[],{}]
+
+    def ContainsByKey(self, *key:int) -> bool:
+        iterable = self.GetKeys()
         for k in key:
-            if not k in iterdict:
+            if not k in iterable:
                 return False
         return True
-    
+
     def Contains(self, *value:_TV) -> bool:
-        iterdict = self.GetValues()
+        iterable = self.GetValues()
         for v in value:
-            if not v in iterdict:
+            if not v in iterable:
                 return False
         return True
 
 
 
-    def __neg__(self) -> Dict[_TK,_TV]:
-        newIterdict = EnumerableDictBase(self.Copy())
-        newIterdict.Reverse()
-        return newIterdict.Get()
+    def __neg__(self) -> List[_TV]:
+        newIterable = EnumerableListBase(self.Copy())
+        return newIterable.Reverse()
     
-    def __add__(self, iterdict:Dict[_TK2,_TV2]) -> Dict[_Union[_TK,_TK2],_Union[_TV,_TV2]]:
-        return EnumerableDictBase(self.Copy()).Concat(iterdict)
+    def __add__(self, iterable:List[_TV2]) -> List[_Union[_TV,_TV2]]:
+        newIterable = EnumerableListBase(self.Copy())
+        newIterable.Concat(iterable)
+        return newIterable.Get()
     
-    def __iadd__(self, iterdict:Dict[_TK2,_TV2]):
-        self.Concat(iterdict)
+    def __iadd__(self, iterable:List[_TV2]) -> Self:
+        self.Concat(iterable)
+        return self
     
-    def __sub__(self, iterdict:Dict[_TK2,_TV2]) -> Dict[_Union[_TK,_TK2],_Union[_TV,_TV2]]:
-        return EnumerableDictBase(self.Copy()).Union(iterdict)
+    def __sub__(self, iterable:List[_TV2]) -> List[_Union[_TV,_TV2]]:
+        newIterable = EnumerableListBase(self.Copy())
+        newIterable.Union(iterable)
+        return newIterable.Get()
     
-    def __isub__(self, iterdict:Dict[_TK2,_TV2]):
-        self.Union(iterdict)
+    def __isub__(self, iterable:List[_TV2]) -> Self:
+        self.Union(iterable)
+        return self
 
     
 
-    def __eq__(self, iterdict:Dict[_TK2,_TV2]) -> bool:
-        return self.SequenceEqual(iterdict)
+    def __eq__(self, iterable:List[_TV2]) -> bool:
+        return self.SequenceEqual(iterable)
 
-    def __ne__(self, iterdict:Dict[_TK2,_TV2]) -> bool:
-        return not self.SequenceEqual(iterdict)
+    def __ne__(self, iterable:List[_TV2]) -> bool:
+        return not self.SequenceEqual(iterable)
     
     def __contains__(self, value:_Value) -> bool:
-        return value in self.Get()
+        return self.Contains(value)
 
 
 
     def __bool__(self) -> bool:
         return not self.IsEmpty()
     
     def __len__(self) -> int:
         return self.Lenght()
+    
+    def __str__(self) -> str:
+        return "{}({})".format(self.__class__.__name__, str(self.iterable))
 
 
 
-    def __iter__(self) -> Iterable[Tuple[int,_TV]]:
-        return iter(self.GetItems())
+    def __iter__(self) -> Iterable[_TV]:
+        return iter(self.GetValues())
     
-    def __getitem__(self, key:_TK) -> _TV:
+    def __getitem__(self, key:int) -> _TV:
         return self.Get(key)
     
-    def __setitem__(self, key:_TK, value:_Value):
-        if key in self.Get():
-            self.Update(key, value)
-        else:
-            self.Add(key, value)
+    def __setitem__(self, key:int, value:_Value):
+        self.Update(key, value)
 
-    def __delitem__(self, key:_TK):
+    def __delitem__(self, key:int):
         self.Delete(key)
 
+    @staticmethod
+    def Range(start:int, stop:int, step:int=1) -> List[int]:
+        return list(range(start,stop,step))
+    @staticmethod
+    def Repeat(value:_TV, count:int) -> List[_TV]:
+        return list(itertools.repeat(value, count))
+
 
 
-__all__ = ["EnumerableDictBase"]
+__all__ = ["AbstractEnumerableBase", "EnumerableListBase"]
```

### Comparing `linqex-1.5/linqex/build/iteritembase.py` & `linqex-1.6/linqex/build/iteritembase.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from linqex._typing import *
+from linqex.abstract.iterablebase import AbstractEnumerableBase
 from linqex.build.iterlistbase import EnumerableListBase
 
-from typing import Dict, List, Callable, Union as _Union, NoReturn, Optional, Tuple, Type, Generic
-from numbers import Number
+from typing import Dict, List, Callable, Union as _Union, NoReturn, Optional, Tuple, Type, Generic, Self
 from collections.abc import Iterable
 import itertools
 
-class EnumerableItemBase(EnumerableListBase,Iterable[Tuple[int,_TV]],Generic[_TV]):
+class EnumerableItemBase(EnumerableListBase, Iterable[Tuple[int,_TV]], Generic[_TK,_TV]):
         
-    def __init__(self, iterlist:Optional[List[_TV]]=None):
-        super().__init__(iterlist)
+    def __init__(self, iterable:Optional[List[_TV]]=None):
+        super().__init__(iterable)
 
     def Get(self, *key:int) -> _Union[List[_TV],_TV]:
         return super().Get(*key)
     
     def GetKey(self, value:_TV) -> int:
         return super().GetKey(value)
     
@@ -43,86 +43,88 @@
     def SkipLast(self, count:int) -> List[_TV]:
         return super().SkipLast(count)
 
     def Select(self, selectFunc:Callable[[int,_TV],_TFV]=lambda key, value: value) -> List[_TFV]:
         return list(map(selectFunc, self.GetKeys(), self.GetValues()))
     
     def Distinct(self, distinctFunc:Callable[[int,_TV],_TFV]=lambda key, value: value) -> List[_TV]:
-        newIterlist = self.Copy()
+        newIterable = self.Copy()
+        indexStep = 0
         for key, value in self.GetItems():
-            if EnumerableItemBase(EnumerableItemBase(newIterlist).Select(distinctFunc)).Count(distinctFunc(key, value)) > 1:
-                EnumerableItemBase(newIterlist).Remove(value)
-        return newIterlist
+            if EnumerableItemBase(EnumerableItemBase(newIterable).Select(distinctFunc)).Count(distinctFunc(key, value)) > 1:
+                EnumerableItemBase(newIterable).Delete(key-indexStep)
+                indexStep += 1
+        return newIterable
     
     def Except(self, exceptFunc:Callable[[int,_TV],_TFV]=lambda key, value: value, *value:_TV) -> List[_TV]:
-        newIterlist = EnumerableItemBase()
+        newIterable = EnumerableItemBase()
         for k, v in self.GetItems():
             if not exceptFunc(k, v) in value:
-                newIterlist.Add(k, v)
-        return newIterlist.Get()
+                newIterable.Add(k, v)
+        return newIterable.Get()
 
-    def Join(self, iterlist: List[_TV2], 
+    def Join(self, iterable: List[_TV2], 
         innerFunc:Callable[[int,_TV],_TFV]=lambda key, value: value, 
         outerFunc:Callable[[int,_TV2],_TFV]=lambda key, value: value, 
         joinFunc:Callable[[int,_TV,int,_TV2],_TFV2]=lambda inKey, inValue, outKey, outValue: (inValue, outValue),
         joinType:JoinType=JoinType.INNER
     ) -> List[_TFV2]:
-        def innerJoin(innerIterlist:List[_TV], outerIterlist:List[_TV2], newIterlist:EnumerableItemBase[Tuple[_TV,_TV2]]):
+        def innerJoin(innerIterable:List[_TV], outerIterable:List[_TV2], newIterable:EnumerableItemBase[Tuple[_TV,_TV2]]):
             nonlocal outerFunc, innerFunc
-            for inKey, inValue in EnumerableItemBase(innerIterlist).GetItems():
-                outer = EnumerableItemBase(outerIterlist).Where(lambda outKey, outValue: outerFunc(outKey, outValue) == innerFunc(inKey, inValue))
+            for inKey, inValue in EnumerableItemBase(innerIterable).GetItems():
+                outer = EnumerableItemBase(outerIterable).Where(lambda outKey, outValue: outerFunc(outKey, outValue) == innerFunc(inKey, inValue))
                 if outer != []:
                     for out in outer:
-                        newIterlist.Add(-1,(inKey, inValue, out[0], out[1]))
-        def leftJoin(innerIterlist:List[_TV], outerIterlist:List[_TV2], newIterlist:EnumerableItemBase[Tuple[_TV,Optional[_TV2]]]):
+                        newIterable.Add(-1,(inKey, inValue, out[0], out[1]))
+        def leftJoin(innerIterable:List[_TV], outerIterable:List[_TV2], newIterable:EnumerableItemBase[Tuple[_TV,Optional[_TV2]]]):
             nonlocal outerFunc, innerFunc
-            for inKey, inValue in EnumerableItemBase(innerIterlist).GetItems():
-                outer = EnumerableItemBase(outerIterlist).Where(lambda outKey, outValue: outerFunc(outKey, outValue) == innerFunc(inKey, inValue))
+            for inKey, inValue in EnumerableItemBase(innerIterable).GetItems():
+                outer = EnumerableItemBase(outerIterable).Where(lambda outKey, outValue: outerFunc(outKey, outValue) == innerFunc(inKey, inValue))
                 if outer is None:
-                    newIterlist.Add(-1,(inKey, inValue, None, None))
+                    newIterable.Add(-1,(inKey, inValue, None, None))
                 else:
-                    newIterlist.Add((inKey, inValue, outer[0], outer[1]))
-        def rightJoin(innerIterlist:List[_TV], outerIterlist:List[_TV2], newIterlist:EnumerableItemBase[Tuple[_TV2,Optional[_TV]]]):
+                    newIterable.Add((inKey, inValue, outer[0], outer[1]))
+        def rightJoin(innerIterable:List[_TV], outerIterable:List[_TV2], newIterable:EnumerableItemBase[Tuple[_TV2,Optional[_TV]]]):
             nonlocal outerFunc, innerFunc
-            for outKey, outValue in EnumerableItemBase(outerIterlist).GetItems():
-                inner = EnumerableItemBase(innerIterlist).First(lambda inKey, inValue: outerFunc(outKey, outValue) == innerFunc(inKey, inValue))
+            for outKey, outValue in EnumerableItemBase(outerIterable).GetItems():
+                inner = EnumerableItemBase(innerIterable).First(lambda inKey, inValue: outerFunc(outKey, outValue) == innerFunc(inKey, inValue))
                 if inner is None:
-                    newIterlist.Add(-1,(None, None, outKey, outValue))
+                    newIterable.Add(-1,(None, None, outKey, outValue))
                 else:
-                    newIterlist.Add(-1,(inner[0], inner[1], outKey, outValue))
-        newIterlist = EnumerableItemBase()
+                    newIterable.Add(-1,(inner[0], inner[1], outKey, outValue))
+        newIterable = EnumerableItemBase()
         if joinType == JoinType.INNER:
             joinTypeFunc = innerJoin
         elif joinType == JoinType.LEFT:
             joinTypeFunc = leftJoin
         elif joinType == JoinType.RIGHT:
             joinTypeFunc = rightJoin
-        joinTypeFunc(self.Get(), iterlist, newIterlist)
-        return newIterlist.Select(lambda key, value: joinFunc(value[0], value[1], value[2], value[3]))         
+        joinTypeFunc(self.Get(), iterable, newIterable)
+        return newIterable.Select(lambda key, value: joinFunc(value[0], value[1], value[2], value[3]))         
       
     def OrderBy(self, *orderByFunc:Tuple[Callable[[int,_TV],_Union[Tuple[_TFV],_TFV]],_Desc]) -> List[_TV]:
         if orderByFunc == ():
             orderByFunc = ((lambda key, value: value))
-        iterlist = self.GetItems()
+        iterable = self.GetItems()
         orderByFunc = list(reversed(orderByFunc))
         for func, desc in orderByFunc:
-            iterlist = sorted(iterlist, key=lambda v: func(v[0], v[1]), reverse=desc)
-        return list(zip(*iterlist))[1]
+            iterable = sorted(iterable, key=lambda x: func(x[0], x[1]), reverse=desc)
+        return list(zip(*iterable))[1]
         
     def GroupBy(self, groupByFunc:Callable[[int,_TV],_Union[Tuple[_TFV],_TFV]]=lambda value: value) -> List[Tuple[_Union[Tuple[_TFV],_TFV], List[_TV]]]:
-        iterlist = EnumerableItemBase(self.OrderBy((groupByFunc, False))).GetItems()
-        iterlist = itertools.groupby(iterlist, lambda items: groupByFunc(items[0], items[1]))
-        return [(keys, list(zip(*list(group)))[1]) for keys, group in iterlist]
+        iterable = EnumerableItemBase(self.OrderBy((groupByFunc, False))).GetItems()
+        iterable = itertools.groupby(iterable, lambda items: groupByFunc(items[0], items[1]))
+        return [(keys, list(zip(*list(group)))[1]) for keys, group in iterable]
     
     def Reverse(self) -> List[_TV]:
         return super().Reverse()
           
-    def Zip(self, iterlist:List[_TV2], zipFunc:Callable[[int,_TV,int,_TV2],_TFV]=lambda inKey, inValue, outKey, outValue: (inValue, outValue)) -> List[_TFV]:
-        newIterlist = EnumerableItemBase(list(zip(self.GetValues(), EnumerableItemBase(iterlist).GetKeys(), EnumerableItemBase(iterlist).GetValues())))
-        return newIterlist.Select(lambda key, value: zipFunc(key, value[0], value[1], value[2]))
+    def Zip(self, iterable:List[_TV2], zipFunc:Callable[[int,_TV,int,_TV2],_TFV]=lambda inKey, inValue, outKey, outValue: (inValue, outValue)) -> List[_TFV]:
+        newIterable = EnumerableItemBase(list(zip(self.GetValues(), EnumerableItemBase(iterable).GetKeys(), EnumerableItemBase(iterable).GetValues())))
+        return newIterable.Select(lambda key, value: zipFunc(key, value[0], value[1], value[2]))
 
 
 
     def Where(self, conditionFunc:Callable[[int,_TV],bool]=lambda key, value: True) -> List[Tuple[int,_TV]]:
         result = list()
         for index, value in self.GetItems():
             if conditionFunc(index, value):
@@ -150,32 +152,32 @@
         if len(result) != 1:
             return None
         else:
             return result[0]
 
 
 
-    def Any(self, conditionFunc:Callable[[int,_TV],bool]=lambda key, value: True) -> bool:
+    def Any(self, conditionFunc:Callable[[int,_TV],bool]=lambda key, value: value) -> bool:
         result = False
         for key, value in self.GetItems():
             if conditionFunc(key, value):
                 result = True
                 break
         return result
     
-    def All(self, conditionFunc:Callable[[int,_TV],bool]=lambda key, value: True) -> bool:
+    def All(self, conditionFunc:Callable[[int,_TV],bool]=lambda key, value: value) -> bool:
         result = True
         for key, value in self.GetItems():
             if not conditionFunc(key, value):
                 result = False
                 break
         return result
  
-    def SequenceEqual(self, iterlist:List[_TV2]) -> bool:
-        return super().SequenceEqual(iterlist)
+    def SequenceEqual(self, iterable:List[_TV2]) -> bool:
+        return super().SequenceEqual(iterable)
 
 
 
     def Accumulate(self, accumulateFunc:Callable[[_TV,int,_TV],_TFV]=lambda temp, key, nextValue: temp + nextValue) -> List[_TFV]:
         firstTemp:bool = True
         def FirstTemp(temp):
             nonlocal firstTemp
@@ -208,15 +210,14 @@
     def Avg(self) -> Optional[_TV]:
         return super().Avg()
         
     def Max(self) -> Optional[_TV]:
         return super().Max()
         
     def Min(self) -> Optional[_TV]:
-        iterlist = self.GetValues()
         return super().Min()
 
 
 
     def Add(self, key:Optional[int], value:_Value):
         if key is None:
             super().Add(value)
@@ -228,46 +229,38 @@
             super().Prepend(value)
         else:
             self.Insert(key, value)
 
     def Insert(self, key:_Key, value:_Value):
         super().Insert(key, value)
 
-    def Update(self, key:_TK, value:_Value):
+    def Update(self, key:int, value:_Value):
         super().Update(key, value)
 
-    def Concat(self, *iterlist:List[_Value]):
-        super().Concat(*iterlist)
+    def Concat(self, *iterable:List[_Value]):
+        super().Concat(*iterable)
 
-    def Union(self, *iterlist:List[_Value]):
-        if not iterlist in [(),[]]:
-            iterlist:list = list(iterlist)
-            newIterlist = EnumerableListBase()
-            filter = dict(self.Where(lambda v: v in iterlist[0]))
-            EnumerableListBase(filter).Loop(lambda v: newIterlist.Add(v))
-            iterlist.pop(0)
-            self.Clear()
-            self.Concat(newIterlist.Get())
-            self.Union(*iterlist)
+    def Union(self, *iterable:List[_Value]):
+        super().Union(*iterable)
 
-    def Delete(self, *key:_TK):
+    def Delete(self, *key:int):
         super().Delete(*key)
 
     def Remove(self, *value:_TV):
         super().Remove(*value)
 
     def RemoveAll(self, *value:_TV):
         super().RemoveAll(*value)
 
     def Clear(self):
         super().Clear()
 
 
 
-    def Loop(self, loopFunc:Callable[[_TV],NoReturn]=lambda value: print(value)):
+    def Loop(self, loopFunc:Callable[[int,_TV],NoReturn]=lambda value: print(value)):
         for key, value in self.GetItems():
             loopFunc(key, value)
 
 
 
     def ToDict(self) -> Dict[int,_TV]:
         return super().ToDict()
@@ -287,64 +280,69 @@
         return super().Contains(*value)
 
 
 
     def __neg__(self) -> List[_TV]:
         return super().__neg__()
     
-    def __add__(self, iterlist:List[_TV2]) -> List[_Union[_TV,_TV2]]:
-        return super().__add__(iterlist)
+    def __add__(self, iterable:List[_TV2]) -> List[_Union[_TV,_TV2]]:
+        return super().__add__(iterable)
     
-    def __iadd__(self, iterlist:List[_TV2]):
-        super().__iadd__(iterlist)
+    def __iadd__(self, iterable:List[_TV2]) -> Self:
+        super().__iadd__(iterable)
+        return self
 
-    def __sub__(self, iterlist:List[_TV2]) -> List[_Union[_TV,_TV2]]:
-        return super().__sub__(iterlist)
+    def __sub__(self, iterable:List[_TV2]) -> List[_Union[_TV,_TV2]]:
+        return super().__sub__(iterable)
     
-    def __isub__(self, iterlist:List[_TV2]):
-        super().__isub__(iterlist)
+    def __isub__(self, iterable:List[_TV2]) -> Self:
+        super().__isub__(iterable)
+        return self
 
     
 
-    def __eq__(self, iterlist:List[_TV2]) -> bool:
-        return super().__eq__(iterlist)
+    def __eq__(self, iterable:List[_TV2]) -> bool:
+        return super().__eq__(iterable)
 
-    def __ne__(self, iterlist:List[_TV2]) -> bool:
-        return super().__eq__(iterlist)
+    def __ne__(self, iterable:List[_TV2]) -> bool:
+        return super().__eq__(iterable)
     
     def __contains__(self, value:_Value) -> bool:
         return super().__sub__(value)
 
 
 
     def __bool__(self) -> bool:
         return super().__bool__()
     
     def __len__(self) -> int:
         return super().__len__()
+    
+    def __str__(self) -> str:
+        return super().__str__()
 
 
 
     def __iter__(self) -> Iterable[Tuple[int,_TV]]:
-        return iter(self.GetItems())
+        return super().__iter__()
     
     def __getitem__(self, key:int) -> _TV:
-        return self.Get(key)
+        return super().__getitem__(key)
     
     def __setitem__(self, key:int, value:_Value):
-        self.Update(key, value)
+        super().__setitem__(key, value)
 
     def __delitem__(self, key:int):
-        self.Delete(key)
+        super().__delitem__(key)
 
     @staticmethod
-    def Range(start:int, stop:int, step:int=1) -> "EnumerableListBase[int]":
+    def Range(start:int, stop:int, step:int=1) -> List[int]:
         return EnumerableListBase.Range(start, stop, step)
     
     @staticmethod
-    def Repeat(value:_Value, count:int) -> "EnumerableListBase[int]":
+    def Repeat(value:_TV, count:int) -> List[_TV]:
         return EnumerableListBase.Repeat(value, count)
 
 
 
 
-__all__ = ["EnumerableItemBase"]
+__all__ = ["AbstractEnumerableBase","EnumerableItemBase"]
```

### Comparing `linqex-1.5/linqex/linq/iterable.py` & `linqex-1.6/linqex/build/iterablebase.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from linqex._typing import *
-from linqex.linq.iterdict import EnumerableDict
-from linqex.linq.iterlist import EnumerableList
-from linqex.linq.iteritem import EnumerableItem
+from linqex.abstract.iterablebase import AbstractEnumerableBase
+from linqex.build.iterdictbase import EnumerableDictBase
+from linqex.build.iterlistbase import EnumerableListBase
+from linqex.build.iteritembase import EnumerableItemBase
 
 from typing import Dict, List, Union, Generic
 
 
-class Enumerable(Generic[_TK,_TV]):
+class EnumerableBase(Generic[_TK,_TV]):
     def __new__(cls, iterable:Union[List[_TV],Dict[_TK,_TV]]):
         return cls.Iterable(iterable)
     @classmethod
-    def Iterable(cls, iterable:Union[List[_TV],Dict[_TK,_TV]]) -> Union[EnumerableItem[_TV], EnumerableDict[_TK,_TV]]:
+    def Iterable(cls, iterable:Union[List[_TV],Dict[_TK,_TV]]) -> Union[EnumerableItemBase[_TV], EnumerableDictBase[_TK,_TV]]:
         if isinstance(iterable, list):
             return cls.Item(iterable)
         elif isinstance(iterable, dict):
             return cls.Dict(iterable)
         else:
-            raise TypeError()
+            raise TypeError("Must be list or dict, not {}".format(str(type(iterable))[8,-2]))
 
     @classmethod
-    def Item(cls, iteritem:List[_TV]=None) -> EnumerableItem[_TV]:
+    def Item(cls, iteritem:List[_TV]=None) -> EnumerableItemBase[_TV]:
         if iteritem is None:
             iteritem:List[_TV]=list()
-        return EnumerableItem(iteritem)
+        return EnumerableItemBase(iteritem)
 
     @classmethod
-    def List(cls, iterlist:List[_TV]=None) -> EnumerableList[_TV]:
+    def List(cls, iterlist:List[_TV]=None) -> EnumerableListBase[_TV]:
         if iterlist is None:
             iterlist:List[_TV]=list()
-        return EnumerableList(iterlist)
+        return EnumerableListBase(iterlist)
 
     @classmethod
-    def Dict(cls, iterdict:Dict[_TK,_TV]=None) -> EnumerableDict[_TK,_TV]:
+    def Dict(cls, iterdict:Dict[_TK,_TV]=None) -> EnumerableDictBase[_TK,_TV]:
         if iterdict is None:
             iterdict:Dict[_TK,_TV]=dict()
-        return EnumerableDict(iterdict)
+        return EnumerableDictBase(iterdict)
 
 
-__all__ = ["Enumerable"]
+
+__all__ = ["AbstractEnumerableBase", "EnumerableListBase", "EnumerableItemBase", "EnumerableDictBase", "EnumerableBase"]
```

### Comparing `linqex-1.5/linqex/linq/iteritem.py` & `linqex-1.6/linqex/linq/iteritem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from linqex._typing import *
+from linqex.abstract.iterable import AbstractEnumerable
 from linqex.build.iteritembase import EnumerableItemBase
-from linqex.linq.iterlist import EnumerableList
+from linqex.linq.iterlist import EnumerableList, EnumerableListCatch
 
-from typing import Dict, List, Callable, Union as _Union, NoReturn, Optional, Tuple, Type, Generic, overload
+from typing import Dict, List, Callable, Union as _Union, NoReturn, Optional, Tuple, Type, Generic, overload, Self
 from collections.abc import Iterable
 
-def EnumerableItemCatch(enumerableItem:"EnumerableItem", iterlist:Optional[List[_TV]], *keyHistoryAdd:_Key, oneValue:bool=False) -> Optional["EnumerableItem[_TV]"]:
-    if iterlist is None:
+def EnumerableItemCatch(enumerableItem:"EnumerableItem", iterable:Optional[List[_TV]], *keyHistoryAdd:_Key, oneValue:bool=False) -> Optional["EnumerableItem[_TV]"]:
+    if iterable is None:
         return None
     else:
-        newEnumerableItem = EnumerableItem(iterlist)
+        newEnumerableItem = EnumerableItem(iterable)
         newEnumerableItem._main = enumerableItem._main
         newEnumerableItem._orderby = enumerableItem._orderby
         newEnumerableItem.keyHistory = enumerableItem.keyHistory.copy()
         if keyHistoryAdd != ():
             if isinstance(keyHistoryAdd[0], (list, tuple)) and len(enumerableItem.keyHistory) != 0:
                 if isinstance(enumerableItem.keyHistory[-1], (list, tuple)):
                     newEnumerableItem.keyHistory[-1].extend(keyHistoryAdd[0])
@@ -26,303 +27,311 @@
 
 def EnumerableItemToValue(enumerableItemOrValue:_Union["EnumerableItem[_TV]",List[_TV]]) -> List[_TV]:
     if isinstance(enumerableItemOrValue, EnumerableItem):
         return enumerableItemOrValue.ToValue
     else:
         return enumerableItemOrValue
 
-class EnumerableItem(EnumerableList,Iterable[Tuple[int,_TV]],Generic[_TV]):
+class EnumerableItem(EnumerableList, Iterable[Tuple[int,_TV]], Generic[_TK,_TV]):
     
-    def __init__(self, iterlist:List[_TV]=None):
-        self.iterlist:List[_TV] = EnumerableItemBase(EnumerableItemToValue(iterlist)).iterlist
+    def __init__(self, iterable:List[_TV]=None):
+        self.iterable:List[_TV] = EnumerableItemBase(EnumerableItemToValue(iterable)).iterable
         self.keyHistory:list = list()
         self._main:EnumerableItem = self
         self._orderby:list = list()
         self._oneValue:bool = False
 
-    def __call__(self, iterlist:List[_TV]=None):
-        self.__init__(iterlist)
+    def __call__(self, iterable:List[_TV]=None):
+        self.__init__(iterable)
 
     def Get(self, *key:int) -> _Union["EnumerableItem[_TV]",_TV]:
-        iterlist = EnumerableItemBase(self.iterlist).Get(*key)
-        if isinstance(iterlist,list):
-            return EnumerableItemCatch(self, iterlist, key)
+        iterable = EnumerableItemBase(self.iterable).Get(*key)
+        if isinstance(iterable,list):
+            return EnumerableItemCatch(self, iterable, key)
         else:
-            return iterlist
+            return iterable
     
     def GetKey(self, value:_TV) -> int:
-        return EnumerableItemBase(self.iterlist).GetKey(EnumerableItemToValue(value))
+        return EnumerableItemBase(self.iterable).GetKey(EnumerableItemToValue(value))
     
-    def GetKeys(self) -> "EnumerableItem[int]":
-        return EnumerableItemCatch(self,EnumerableItemBase(self.iterlist).GetKeys())
+    def GetKeys(self) -> EnumerableList[int]:
+        return EnumerableListCatch(self,EnumerableItemBase(self.iterable).GetKeys())
     
-    def GetValues(self) -> "EnumerableItem[_TV]":
-        return EnumerableItemCatch(self,EnumerableItemBase(self.iterlist).GetValues())
+    def GetValues(self) -> EnumerableList[_TV]:
+        return EnumerableListCatch(self,EnumerableItemBase(self.iterable).GetValues())
     
-    def GetItems(self) -> "EnumerableItem[Tuple[int,_TV]]":
-        return EnumerableItemCatch(self,EnumerableItemBase(self.iterlist).GetItems())
+    def GetItems(self) -> EnumerableList[Tuple[int,_TV]]:
+        return EnumerableListCatch(self,EnumerableItemBase(self.iterable).GetItems())
     
     def Copy(self) -> "EnumerableItem[_TV]":
-        return EnumerableItem(EnumerableItemBase(self.iterlist).Copy())
+        return EnumerableItem(EnumerableItemBase(self.iterable).Copy())
 
 
 
     def Take(self, count:int) -> "EnumerableItem[_TV]":
-        return EnumerableItemCatch(self,EnumerableItemBase(self.iterlist).Take(count))
+        return EnumerableItemCatch(self,EnumerableItemBase(self.iterable).Take(count))
     
     def TakeLast(self, count:int) -> "EnumerableItem[_TV]":
-        return EnumerableItemCatch(self,EnumerableItemBase(self.iterlist).TakeLast(count))
+        return EnumerableItemCatch(self,EnumerableItemBase(self.iterable).TakeLast(count))
     
     def Skip(self, count:int) -> "EnumerableItem[_TV]":
-        return EnumerableItemCatch(self,EnumerableItemBase(self.iterlist).Skip(count))
+        return EnumerableItemCatch(self,EnumerableItemBase(self.iterable).Skip(count))
     
     def SkipLast(self, count:int) -> "EnumerableItem[_TV]":
-        return EnumerableItemCatch(self,EnumerableItemBase(self.iterlist).SkipLast(count))
+        return EnumerableItemCatch(self,EnumerableItemBase(self.iterable).SkipLast(count))
     
     def Select(self, selectFunc:Callable[[int,_TV],_TFV]=lambda key, value: value) -> "EnumerableItem[_TFV]":
-        return EnumerableItemCatch(self,EnumerableItemBase(self.iterlist).Select(selectFunc))
+        return EnumerableItemCatch(self,EnumerableItemBase(self.iterable).Select(selectFunc))
     
     def Distinct(self, distinctFunc:Callable[[int,_TV],_TFV]=lambda key, value: value) -> "EnumerableItem[_TV]":
-        return EnumerableItemCatch(self,EnumerableItemBase(self.iterlist).Distinct(distinctFunc))
+        return EnumerableItemCatch(self,EnumerableItemBase(self.iterable).Distinct(distinctFunc))
     
     def Except(self, exceptFunc:Callable[[int,_TV],_TFV]=lambda key, value: value, *value:_TV) -> "EnumerableItem[_TV]":
-        return EnumerableItemCatch(self,EnumerableItemBase(self.iterlist).Except(exceptFunc, *map(EnumerableItemToValue, value)))
+        return EnumerableItemCatch(self,EnumerableItemBase(self.iterable).Except(exceptFunc, *map(EnumerableItemToValue, value)))
 
-    def Join(self, iterlist: List[_TV2], 
+    def Join(self, iterable: List[_TV2], 
         innerFunc:Callable[[int,_TV],_TFV]=lambda key, value: value, 
         outerFunc:Callable[[int,_TV2],_TFV]=lambda key, value: value, 
         joinFunc:Callable[[int,_TV,int,_TV2],_TFV2]=lambda inKey, inValue, outKey, outValue: (inValue, outValue),
         joinType:JoinType=JoinType.INNER
     ) -> "EnumerableItem[_TFV2]":
-        return EnumerableItem(EnumerableItemBase(self.iterlist).Join(EnumerableItemToValue(iterlist), innerFunc, outerFunc, joinFunc, joinType))
+        return EnumerableItem(EnumerableItemBase(self.iterable).Join(EnumerableItemToValue(iterable), innerFunc, outerFunc, joinFunc, joinType))
       
-    def OrderBy(self, orderByFunc:Callable[[int,_TV],_Union[Tuple[_TFV],_TFV]], desc:bool=False) -> "EnumerableItem[_TV]":
+    def OrderBy(self, orderByFunc:Callable[[int,_TV],_Union[Tuple[_TFV],_TFV]]=lambda key, value: value, desc:bool=False) -> "EnumerableItem[_TV]":
         self._orderby.clear()
         self._orderby.append((orderByFunc, desc))
-        return EnumerableItemCatch(self,EnumerableItemBase(self.iterlist).OrderBy((orderByFunc, desc)))
+        return EnumerableItemCatch(self,EnumerableItemBase(self.iterable).OrderBy((orderByFunc, desc)))
 
-    def ThenBy(self, orderByFunc:Callable[[int,_TV],_Union[Tuple[_TFV],_TFV]], desc:bool=False) -> "EnumerableItem[_TV]":
+    def ThenBy(self, orderByFunc:Callable[[int,_TV],_Union[Tuple[_TFV],_TFV]]=lambda key, value: value, desc:bool=False) -> "EnumerableItem[_TV]":
         self._orderby.append((orderByFunc, desc))
-        return EnumerableItemCatch(self,EnumerableItemBase(self.iterlist).OrderBy(*self._orderby))
+        return EnumerableItemCatch(self,EnumerableItemBase(self.iterable).OrderBy(*self._orderby))
         
     def GroupBy(self, groupByFunc:Callable[[int,_TV],_Union[Tuple[_TFV],_TFV]]=lambda key, value: value) -> "EnumerableItem[Tuple[_Union[Tuple[_TFV],_TFV], List[_TV]]]":
-        return EnumerableItem(EnumerableItemBase(self.iterlist).GroupBy(groupByFunc))
+        return EnumerableItem(EnumerableItemBase(self.iterable).GroupBy(groupByFunc))
 
     def Reverse(self) -> "EnumerableItem[_TV]":
-        return EnumerableItemCatch(self,EnumerableItemBase(self.iterlist).Reverse())
+        return EnumerableItemCatch(self,EnumerableItemBase(self.iterable).Reverse())
         
-    def Zip(self, iterlist:List[_TV2], zipFunc:Callable[[int,_TV,int,_TV2],_TFV]=lambda inKey, inValue, outKey, outValue: (inValue, outValue)) -> "EnumerableItem[_TFV]":
-        return EnumerableItem(EnumerableItemBase(self.iterlist).Zip(EnumerableItemToValue(iterlist), zipFunc))
+    def Zip(self, iterable:List[_TV2], zipFunc:Callable[[int,_TV,int,_TV2],_TFV]=lambda inKey, inValue, outKey, outValue: (inValue, outValue)) -> "EnumerableItem[_TFV]":
+        return EnumerableItem(EnumerableItemBase(self.iterable).Zip(EnumerableItemToValue(iterable), zipFunc))
 
 
 
     def Where(self, conditionFunc:Callable[[int,_TV],bool]=lambda key, value: True) -> "EnumerableItem[_TV]":
-        items = dict(EnumerableItemBase(self.iterlist).Where(conditionFunc))
+        items = dict(EnumerableItemBase(self.iterable).Where(conditionFunc))
         return EnumerableItemCatch(self, list(items.values()), list(items.keys()))
     
     def OfType(self, *type:Type) -> "EnumerableItem[_TV]":
-        items = dict(EnumerableItemBase(self.iterlist).OfType(*type))
+        items = dict(EnumerableItemBase(self.iterable).OfType(*type))
         return EnumerableItemCatch(self, list(items.values()), list(items.keys()))
     
     def First(self, conditionFunc:Callable[[int,_TV],bool]=lambda key, value: True) -> Optional["EnumerableItem[_TV]"]:
-        firstValue = EnumerableItemBase(self.iterlist).First(conditionFunc)
+        firstValue = EnumerableItemBase(self.iterable).First(conditionFunc)
         if firstValue is None:
             return None
         else:
             return EnumerableItemCatch(self, [firstValue[1]], firstValue[0], oneValue=True)
     
     def Last(self, conditionFunc:Callable[[int,_TV],bool]=lambda key, value: True) -> Optional["EnumerableItem[_TV]"]:
-        lastValue = EnumerableItemBase(self.iterlist).Last(conditionFunc)
+        lastValue = EnumerableItemBase(self.iterable).Last(conditionFunc)
         if lastValue is None:
             return None
         else:
             return EnumerableItemCatch(self, [lastValue[1]], lastValue[0], oneValue=True)
         
     def Single(self, conditionFunc:Callable[[int,_TV],bool]=lambda key, value: True) -> Optional["EnumerableItem[_TV]"]:
-        singleValue = EnumerableItemBase(self.iterlist).Single(conditionFunc)
+        singleValue = EnumerableItemBase(self.iterable).Single(conditionFunc)
         if singleValue is None:
             return None
         else:
             return EnumerableItemCatch(self, [singleValue[1]], singleValue[0], oneValue=True)
 
 
 
-    def Any(self, conditionFunc:Callable[[int,_TV],bool]=lambda key, value: True) -> bool:
-        return EnumerableItemBase(self.iterlist).Any(conditionFunc)
+    def Any(self, conditionFunc:Callable[[int,_TV],bool]=lambda key, value: value) -> bool:
+        return EnumerableItemBase(self.iterable).Any(conditionFunc)
     
-    def All(self, conditionFunc:Callable[[int,_TV],bool]=lambda key, value: True) -> bool:
-        return EnumerableItemBase(self.iterlist).All(conditionFunc)
+    def All(self, conditionFunc:Callable[[int,_TV],bool]=lambda key, value: value) -> bool:
+        return EnumerableItemBase(self.iterable).All(conditionFunc)
     
-    def SequenceEqual(self, iterlist:List[_TV2]) -> bool:
-        return EnumerableItemBase(self.iterlist).SequenceEqual(EnumerableItemToValue(iterlist))
+    def SequenceEqual(self, iterable:List[_TV2]) -> bool:
+        return EnumerableItemBase(self.iterable).SequenceEqual(EnumerableItemToValue(iterable))
 
 
 
     def Accumulate(self, accumulateFunc:Callable[[_TV,int,_TV],_TFV]=lambda temp, key, nextValue: temp + nextValue) -> "EnumerableItem[_TFV]":
-        return EnumerableItem(EnumerableItemBase(self.iterlist).Accumulate(accumulateFunc))
+        return EnumerableItem(EnumerableItemBase(self.iterable).Accumulate(accumulateFunc))
 
     def Aggregate(self, aggregateFunc:Callable[[_TV,int,_TV],_TFV]=lambda temp, key, nextValue: temp + nextValue) -> _TFV:
-        return EnumerableItemBase(self.iterlist).Aggregate(aggregateFunc)
+        return EnumerableItemBase(self.iterable).Aggregate(aggregateFunc)
 
 
 
     def Count(self, value:_TV) -> int:
-        return EnumerableItemBase(self.iterlist).Count(value)
+        return EnumerableItemBase(self.iterable).Count(value)
 
     @property
     def Lenght(self) -> int:
-        return EnumerableItemBase(self.iterlist).Lenght()
+        return EnumerableItemBase(self.iterable).Lenght()
     
     def Sum(self) -> Optional[_TV]:
-        return EnumerableItemBase(self.iterlist).Sum()
+        return EnumerableItemBase(self.iterable).Sum()
         
     def Avg(self) -> Optional[_TV]:
-        return EnumerableItemBase(self.iterlist).Avg()
+        return EnumerableItemBase(self.iterable).Avg()
         
     def Max(self) -> Optional[_TV]:
-        return EnumerableItemBase(self.iterlist).Max()
+        return EnumerableItemBase(self.iterable).Max()
         
     def Min(self) -> Optional[_TV]:
-        return EnumerableItemBase(self.iterlist).Min()
+        return EnumerableItemBase(self.iterable).Min()
 
     @overload
-    def Set(): ...
+    def Set(self): ...
     @overload
     def Set(self, value:_Value): ...
     def Set(self, value=...):
         super().Set(value)
 
     def Add(self, key:Optional[int], value:_Value):
-        EnumerableItemBase(self.iterlist).Add(key, EnumerableItemToValue(value))
+        EnumerableItemBase(self.iterable).Add(key, EnumerableItemToValue(value))
 
     def Prepend(self, key:Optional[int], value:_Value):
-        EnumerableItemBase(self.iterlist).Prepend(key, EnumerableItemToValue(value))
+        EnumerableItemBase(self.iterable).Prepend(key, EnumerableItemToValue(value))
 
     def Insert(self, key:int, value:_Value):
-        EnumerableItemBase(self.iterlist).Insert(key, EnumerableItemToValue(value))
+        EnumerableItemBase(self.iterable).Insert(key, EnumerableItemToValue(value))
 
     def Update(self, key:int, value:_Value):
-        EnumerableItemBase(self.iterlist).Update(key, EnumerableItemToValue(value))
+        EnumerableItemBase(self.iterable).Update(key, EnumerableItemToValue(value))
 
-    def Concat(self, *iterlist:List[_TV2]):
-        EnumerableItemBase(self.iterlist).Concat(*map(EnumerableItemToValue, iterlist))
+    def Concat(self, *iterable:List[_TV2]):
+        EnumerableItemBase(self.iterable).Concat(*map(EnumerableItemToValue, iterable))
 
-    def Union(self, *iterlist:List[_TV2]):
-        EnumerableItemBase(self.iterlist).Union(*map(EnumerableItemToValue, iterlist))
+    def Union(self, *iterable:List[_TV2]):
+        EnumerableItemBase(self.iterable).Union(*map(EnumerableItemToValue, iterable))
 
     @overload
     def Delete(self): ...
     @overload
     def Delete(self, *key:int): ...
     def Delete(self, *key):
         if key == ():
             if isinstance(self.ToKey, (list,tuple)):
                 key = self.ToKey
             else:
                 key = [self.ToKey]
             self._main.Get(*filter(lambda k: not isinstance(k, (list,tuple)),self.keyHistory[:len(self.keyHistory)-1])).Delete(*key)
         else:
-            EnumerableItemBase(self.iterlist).Delete(*key)
+            EnumerableItemBase(self.iterable).Delete(*key)
 
     def Remove(self, *value:_TV):
-        EnumerableItemBase(self.iterlist).Remove(*map(EnumerableItemToValue, value))
+        EnumerableItemBase(self.iterable).Remove(*map(EnumerableItemToValue, value))
 
     def RemoveAll(self, *value:_TV):
-        EnumerableItemBase(self.iterlist).RemoveAll(*map(EnumerableItemToValue, value))
+        EnumerableItemBase(self.iterable).RemoveAll(*map(EnumerableItemToValue, value))
 
     def Clear(self):
-        EnumerableItemBase(self.iterlist).Clear()
+        EnumerableItemBase(self.iterable).Clear()
 
 
 
     def Loop(self, loopFunc:Callable[[int,_TV],NoReturn]=lambda key, value: print(value)):
-        EnumerableItemBase(self.iterlist).Loop(loopFunc)
+        EnumerableItemBase(self.iterable).Loop(loopFunc)
 
 
 
     @property
     def ToKey(self) -> int:
         return super().ToKey
+    
     @property
     def ToValue(self) -> _Union[List[_TV],_TV]:
         return super().ToValue
+    
     @property
     def ToDict(self) -> Dict[int,_TV]:
-        return EnumerableItemBase(self.iterlist).ToDict()
+        return EnumerableItemBase(self.iterable).ToDict()
+    
     @property
     def ToList(self) -> List[_TV]:
-        return EnumerableItemBase(self.iterlist).ToList()
+        return EnumerableItemBase(self.iterable).ToList()
 
 
 
     @property
     def IsEmpty(self) -> bool:
-        return EnumerableItemBase(self.iterlist).IsEmpty()
+        return EnumerableItemBase(self.iterable).IsEmpty()
 
     def ContainsByKey(self, *key:int) -> bool:
-        return EnumerableItemBase(self.iterlist).ContainsByKey(*key)
+        return EnumerableItemBase(self.iterable).ContainsByKey(*key)
 
     def Contains(self, *value:_TV) -> bool:
-        return EnumerableItemBase(self.iterlist).Contains(*map(EnumerableItemToValue, value))
+        return EnumerableItemBase(self.iterable).Contains(*map(EnumerableItemToValue, value))
 
 
 
     def __neg__(self) -> "EnumerableItem[_TV]":
-        return EnumerableItem(EnumerableItemBase(self.Copy().iterlist).__neg__())
+        return EnumerableItem(EnumerableItemBase(self.Copy().iterable).__neg__())
     
-    def __add__(self, iterlist:List[_TV]) -> "EnumerableItem[_Union[_TV,_TV2]]":
-        return EnumerableItem(EnumerableItemBase(self.Copy().iterlist).__add__(EnumerableItemToValue(iterlist)))
+    def __add__(self, iterable:List[_TV]) -> "EnumerableItem[_Union[_TV,_TV2]]":
+        return EnumerableItem(EnumerableItemBase(self.Copy().iterable).__add__(EnumerableItemToValue(iterable)))
     
-    def __iadd__(self, iterlist:List[_TV]):
-        EnumerableItemBase(self.iterlist).__iadd__(EnumerableItemToValue(iterlist))
-    
-    def __sub__(self, iterlist:List[_TV]) -> "EnumerableItem[_Union[_TV,_TV2]]":
-        return EnumerableItem(EnumerableItemBase(self.Copy().iterlist).__sub__(EnumerableItemToValue(iterlist)))
+    def __iadd__(self, iterable:List[_TV]) -> Self:
+        EnumerableItemBase(self.iterable).__iadd__(EnumerableItemToValue(iterable))
+        return self
+
+    def __sub__(self, iterable:List[_TV]) -> "EnumerableItem[_Union[_TV,_TV2]]":
+        return EnumerableItem(EnumerableItemBase(self.Copy().iterable).__sub__(EnumerableItemToValue(iterable)))
     
-    def __isub__(self, iterlist:List[_TV]):
-        EnumerableItemBase(self.iterlist).__isub__(EnumerableItemToValue(iterlist))
+    def __isub__(self, iterable:List[_TV]) -> Self:
+        EnumerableItemBase(self.iterable).__isub__(EnumerableItemToValue(iterable))
+        return self
 
     
 
-    def __eq__(self, iterlist:List[_TV]) -> bool:
-        return EnumerableItemBase(self.iterlist).__eq__(EnumerableItemToValue(iterlist))
+    def __eq__(self, iterable:List[_TV]) -> bool:
+        return EnumerableItemBase(self.iterable).__eq__(EnumerableItemToValue(iterable))
 
-    def __ne__(self, iterlist:List[_TV]) -> bool:
-        return EnumerableItemBase(self.iterlist).__ne__(EnumerableItemToValue(iterlist))
+    def __ne__(self, iterable:List[_TV]) -> bool:
+        return EnumerableItemBase(self.iterable).__ne__(EnumerableItemToValue(iterable))
     
     def __contains__(self, value:_Value) -> bool:
-        return EnumerableItemBase(self.iterlist).__contains__(EnumerableItemToValue(value))
+        return EnumerableItemBase(self.iterable).__contains__(EnumerableItemToValue(value))
 
 
 
     def __bool__(self) -> bool:
-        return EnumerableItemBase(self.iterlist).__bool__()
+        return EnumerableItemBase(self.iterable).__bool__()
     
     def __len__(self) -> int:
-        return EnumerableItemBase(self.iterlist).__len__()
+        return EnumerableItemBase(self.iterable).__len__()
+    
+    def __str__(self) -> str:
+        return "{}({})".format(self.__class__.__name__, str(self.iterable))
 
 
 
     def __iter__(self) -> Iterable[Tuple[int,_TV]]:
         return EnumerableItemBase(self.GetItems().ToValue).__iter__()
     
     def __getitem__(self, key:int) -> _TV:
-        return EnumerableItemBase(self.iterlist).__getitem__(key)
+        return EnumerableItemBase(self.iterable).__getitem__(key)
     
     def __setitem__(self, key:int, value:_Value):
-        return EnumerableItemBase(self.iterlist).__setitem__(key, EnumerableItemToValue(value))
+        return EnumerableItemBase(self.iterable).__setitem__(key, EnumerableItemToValue(value))
 
     def __delitem__(self, key:int):
-        return EnumerableItemBase(self.iterlist).__delitem__(key)
+        return EnumerableItemBase(self.iterable).__delitem__(key)
 
 
 
     @staticmethod
     def Range(start:int, stop:int, step:int=1) -> "EnumerableItem[int]":
-        return EnumerableItem(EnumerableItemBase.Range(start, stop, step).Get())
+        return EnumerableItem(EnumerableItemBase.Range(start, stop, step))
     @staticmethod
-    def Repeat(value:_Value, count:int) -> "EnumerableItem[int]":
-        return EnumerableItem(EnumerableItemBase.Repeat(value, count).Get())
+    def Repeat(value:_TV, count:int) -> "EnumerableItem[_TV]":
+        return EnumerableItem(EnumerableItemBase.Repeat(value, count))
 
 
 
-__all__ = ["EnumerableItem"]
+__all__ = ["AbstractEnumerable", "EnumerableItem"]
```

### Comparing `linqex-1.5/linqex.egg-info/PKG-INFO` & `linqex-1.6/linqex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linqex
-Version: 1.5
+Version: 1.6
 Summary: The linq module in C# has been adapted for python with some modifications.
 Home-page: https://github.com/TahsinCr/python-linqex
 Author: TahsinCr
 Author-email: TahsinCr@outlook.com
 License: MIT
 Keywords: linq,linqex,ex,enumerable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linqex-1.5/setup.py` & `linqex-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r', encoding='utf-8') as file:
     LONG_DESCRIPTION = file.read() 
 LONG_DESCRIPTION_CONTENT_TYPE = "text/markdown"
 
 NAME = 'linqex'
-VERSION = '1.5'
+VERSION = '1.6'
 DESCRIPTION = 'The linq module in C# has been adapted for python with some modifications.'
 URL = 'https://github.com/TahsinCr/python-linqex'
 AUTHOR = 'TahsinCr'
 AUTHOR_EMAIL = 'TahsinCr@outlook.com'
 LICENSE = 'MIT'
 KEYWORDS = ['linq', 'linqex', 'ex', 'enumerable']
 SRC = 'linqex'
```

