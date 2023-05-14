# Comparing `tmp/cpmpy-0.9.8.tar.gz` & `tmp/cpmpy-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpmpy-0.9.8.tar", last modified: Fri Mar 18 21:32:02 2022, max compression
+gzip compressed data, was "cpmpy-0.9.9.tar", last modified: Tue Jun 21 05:35:58 2022, max compression
```

## Comparing `cpmpy-0.9.8.tar` & `cpmpy-0.9.9.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 21:32:02.113862 cpmpy-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-03-18 21:31:36.000000 cpmpy-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6359 2022-03-18 21:32:02.113862 cpmpy-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4876 2022-03-18 21:31:36.000000 cpmpy-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 21:32:02.109862 cpmpy-0.9.8/cpmpy/
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 21:32:02.113862 cpmpy-0.9.8/cpmpy/expressions/
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16282 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/expressions/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    10238 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/expressions/globalconstraints.py
--rw-r--r--   0 runner    (1001) docker     (121)     3151 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/expressions/python_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/expressions/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    19129 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/expressions/variables.py
--rw-r--r--   0 runner    (1001) docker     (121)     8060 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 21:32:02.113862 cpmpy-0.9.8/cpmpy/solvers/
--rw-r--r--   0 runner    (1001) docker     (121)     9770 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/solvers/TEMPLATE.py
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18625 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/solvers/gurobi.py
--rw-r--r--   0 runner    (1001) docker     (121)    20690 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/solvers/minizinc.py
--rw-r--r--   0 runner    (1001) docker     (121)    29644 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/solvers/ortools.py
--rw-r--r--   0 runner    (1001) docker     (121)    13681 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/solvers/pysat.py
--rw-r--r--   0 runner    (1001) docker     (121)    10738 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/solvers/solver_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     4277 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/solvers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 21:32:02.113862 cpmpy-0.9.8/cpmpy/transformations/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29934 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/transformations/flatten_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/transformations/get_variables.py
--rw-r--r--   0 runner    (1001) docker     (121)    14298 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/transformations/linearize.py
--rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/transformations/reification.py
--rw-r--r--   0 runner    (1001) docker     (121)     5122 2022-03-18 21:31:36.000000 cpmpy-0.9.8/cpmpy/transformations/to_cnf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 21:32:02.113862 cpmpy-0.9.8/cpmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6359 2022-03-18 21:32:01.000000 cpmpy-0.9.8/cpmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-03-18 21:32:01.000000 cpmpy-0.9.8/cpmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-18 21:32:01.000000 cpmpy-0.9.8/cpmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-18 21:32:01.000000 cpmpy-0.9.8/cpmpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-03-18 21:32:01.000000 cpmpy-0.9.8/cpmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-18 21:32:01.000000 cpmpy-0.9.8/cpmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-03-18 21:31:36.000000 cpmpy-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-18 21:32:02.113862 cpmpy-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-03-18 21:31:36.000000 cpmpy-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 05:35:58.187641 cpmpy-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-06-21 05:35:50.000000 cpmpy-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     6359 2022-06-21 05:35:58.187641 cpmpy-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4876 2022-06-21 05:35:50.000000 cpmpy-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 05:35:58.175640 cpmpy-0.9.9/cpmpy/
+-rw-r--r--   0 runner    (1001) docker     (121)      957 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 05:35:58.179641 cpmpy-0.9.9/cpmpy/expressions/
+-rw-r--r--   0 runner    (1001) docker     (121)      808 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18262 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/expressions/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14933 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/expressions/globalconstraints.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3151 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/expressions/python_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2592 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/expressions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19538 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/expressions/variables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8620 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 05:35:58.183641 cpmpy-0.9.9/cpmpy/solvers/
+-rw-r--r--   0 runner    (1001) docker     (121)     9770 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/solvers/TEMPLATE.py
+-rw-r--r--   0 runner    (1001) docker     (121)      997 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17175 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/solvers/gurobi.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20837 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/solvers/minizinc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27587 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/solvers/ortools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13681 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/solvers/pysat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8974 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/solvers/pysdd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10738 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/solvers/solver_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/solvers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 05:35:58.183641 cpmpy-0.9.9/cpmpy/transformations/
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/transformations/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26143 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/transformations/flatten_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/transformations/get_variables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14084 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/transformations/linearize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7000 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/transformations/reification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5094 2022-06-21 05:35:50.000000 cpmpy-0.9.9/cpmpy/transformations/to_cnf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 05:35:58.179641 cpmpy-0.9.9/cpmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6359 2022-06-21 05:35:57.000000 cpmpy-0.9.9/cpmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2022-06-21 05:35:58.000000 cpmpy-0.9.9/cpmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-21 05:35:57.000000 cpmpy-0.9.9/cpmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-21 05:35:57.000000 cpmpy-0.9.9/cpmpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-21 05:35:57.000000 cpmpy-0.9.9/cpmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-21 05:35:57.000000 cpmpy-0.9.9/cpmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-06-21 05:35:50.000000 cpmpy-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-21 05:35:58.187641 cpmpy-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-06-21 05:35:50.000000 cpmpy-0.9.9/setup.py
```

### Comparing `cpmpy-0.9.8/LICENSE` & `cpmpy-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cpmpy-0.9.8/PKG-INFO` & `cpmpy-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpmpy
-Version: 0.9.8
+Version: 0.9.9
 Summary: A numpy-based library for modeling constraint programming problems
 Home-page: https://github.com/CPMpy/cpmpy
 Author: Tias Guns
 Author-email: tias.guns@kuleuven.be
 License: Apache 2.0
 Description: CPMpy is a Constraint Programming and Modeling library in Python, based on numpy, with direct solver access.
```

### Comparing `cpmpy-0.9.8/README.md` & `cpmpy-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `cpmpy-0.9.8/cpmpy/__init__.py` & `cpmpy-0.9.9/cpmpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     The package constists of 4 modules:
     - `model`: a generic container for expressions (constraints and an objective), it can also search for an available solver and call it
     - `expressions`: all forms of expression objects that allow you to specify constraints and objectives over variables
     - `solvers`: CPMpy classes that translate a model into approriate calls of a solver's API
     - `transformations`: common methods for transforming expressions into other expressions, used by `solvers` modules to simplify/rewrite expressions
 """
-# Tias Guns, 2019-2021
+# Tias Guns, 2019-2022
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 
 from .expressions import *
 from .model import Model
 from .solvers.utils import SolverLookup
```

### Comparing `cpmpy-0.9.8/cpmpy/expressions/__init__.py` & `cpmpy-0.9.9/cpmpy/expressions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 
 """
 
 # we only import methods/classes that are used for modelling
 # others need to be imported by the developer explicitely
 from .variables import boolvar, intvar, cpm_array
 from .variables import BoolVar, IntVar, cparray # Old, to be deprecated
-from .globalconstraints import AllDifferent, AllEqual, Circuit, Table, Minimum, Maximum, Element
+from .globalconstraints import AllDifferent, AllEqual, Circuit, Table, Minimum, Maximum, Element, Xor
 from .globalconstraints import alldifferent, allequal, circuit # Old, to be deprecated
 from .python_builtins import all, any, max, min, sum
```

### Comparing `cpmpy-0.9.8/cpmpy/expressions/core.py` & `cpmpy-0.9.9/cpmpy/expressions/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     - x % y         Operator("mod", [x,y])
     - x ** y        Operator("pow", [x,y])
 
     Logical operators:
 
     - x & y         Operator("and", [x,y])
     - x | y         Operator("or", [x,y])
-    - x ^ y         Operator("xor", [x,y])
+    - x ^ y         Xor([x,y])  # a global constraint
 
     Finally there are two special cases for logical operators 'implies' and '~/not'.
     
     Python has no built-in operator for __implication__ that can be overloaded.
     CPMpy hence has a function 'implies()' that can be called:
 
     - x.implies(y)  Operator("->", [x,y])
@@ -118,36 +118,68 @@
                 # flatten
                 strarg = ",".join(map(str,arg.flat))
                 strargs.append( f"[{strarg}]" )
             else:
                 strargs.append( f"{arg}" )
         return "{}({})".format(self.name, ",".join(strargs))
 
+    def __hash__(self):
+        return hash(self.__str__())
+
     def is_bool(self):
         """ is it a Boolean (return type) Operator?
             Default: yes
         """
         return True
 
     def value(self):
         return None # default
 
+    def _deepcopy_args(self, memodict={}):
+        """
+            Create and return a deep copy of the arguments of the expression
+            Used in copy() methods of expressions to ensure there are no shared variables between the original expression and its copy.
+            :param: memodict: dictionary with already copied objects, similar to copy.deepcopy()
+        """
+        copied = []
+        for arg in self.args:
+            if arg not in memodict:
+                if isinstance(arg, Expression):
+                    memodict[arg] = arg.deepcopy(memodict)
+                elif is_num(arg) or isinstance(arg, bool):
+                    memodict[arg] = arg
+                else:
+                    raise ValueError(f"Not a supported argument to copy: {arg}")
+            copied.append(memodict[arg])
+        return copied
+
+    def deepcopy(self, memodict = {}):
+        """
+            Return a deep copy of the Expression
+            :param: memodict: dictionary with already copied objects, similar to copy.deepcopy()
+        """
+        copied_args = self._deepcopy_args(memodict)
+        return type(self)(self.name, copied_args)
+
     # implication constraint: self -> other
     # Python does not offer relevant syntax...
     # for double implication, use equivalence self == other
     def implies(self, other):
         # other constant
         if other is True:
             return True
         if other is False:
             return ~self
         return Operator('->', [self, other])
 
     # Comparisons
     def __eq__(self, other):
+        # BoolExpr == 1|true, then simply BoolExpr
+        if self.is_bool() and is_num(other) and other == 1:
+            return self
         return Comparison("==", self, other)
     def __ne__(self, other):
         return Comparison("!=", self, other)
     def __lt__(self, other):
         return Comparison("<", self, other)
     def __le__(self, other):
         return Comparison("<=", self, other)
@@ -189,29 +221,32 @@
             return True
         if other is False:
             return self
 
         return Operator("or", [other, self])
 
     def __xor__(self, other):
+        # avoid cyclic import
+        from .globalconstraints import Xor
         # some simple constant removal
         if other is True:
             return ~self
         if other is False:
             return self
+        return Xor([self, other])
 
-        return Operator("xor", [self, other])
     def __rxor__(self, other):
+        # avoid cyclic import
+        from .globalconstraints import Xor
         # some simple constant removal
         if other is True:
             return ~self
         if other is False:
             return self
-
-        return Operator("xor", [other, self])
+        return Xor([other, self])
 
     # Mathematical Operators, including 'r'everse if it exists
     # Addition
     def __add__(self, other):
         if is_num(other) and other == 0:
             return self
         return Operator("sum", [self, other])
@@ -232,18 +267,22 @@
         # return Operator("sub", [other, self])
         return (-self).__radd__(other)
     
     # multiplication, puts the 'constant' (other) first
     def __mul__(self, other):
         if is_num(other) and other == 1:
             return self
+        if is_num(other) and other == 0:
+            return 0
         return Operator("mul", [self, other])
     def __rmul__(self, other):
         if is_num(other) and other == 1:
             return self
+        if is_num(other) and other == 0:
+            return 0
         return Operator("mul", [other, self])
 
     # matrix multipliciation TODO?
     #object.__matmul__(self, other)
 
     # other mathematical ones
     def __truediv__(self, other):
@@ -256,14 +295,18 @@
     def __mod__(self, other):
         return Operator("mod", [self, other])
     def __rmod__(self, other):
         return Operator("mod", [other, self])
 
     def __pow__(self, other, modulo=None):
         assert (modulo is None), "Power operator: modulo not supported"
+        if other == 0:
+            return 1
+        elif other == 1:
+            return self
         return Operator("pow", [self, other])
     def __rpow__(self, other, modulo=None):
         assert (modulo is None), "Power operator: modulo not supported"
         return Operator("pow", [other, self])
 
     # Not implemented: (yet?)
     #object.__floordiv__(self, other)
@@ -283,55 +326,61 @@
 
 class Comparison(Expression):
     """Represents a comparison between two sub-expressions
     """
     allowed = {'==', '!=', '<=', '<', '>=', '>'}
 
     def __init__(self, name, left, right):
-        assert (name in Comparison.allowed), "Symbol not allowed"
+        assert (name in Comparison.allowed), f"Symbol {name} not allowed"
         super().__init__(name, [left, right])
 
     def __repr__(self):
         if all(isinstance(x, Expression) for x in self.args):
             return "({}) {} ({})".format(self.args[0], self.name, self.args[1]) 
         # if not: prettier printing without braces
         return "{} {} {}".format(self.args[0], self.name, self.args[1]) 
 
-    # a comparison itself is bool, check special case
-    def __eq__(self, other):
-        if is_num(other) and other == 1:
-            return self
-        return super().__eq__(other)
-        
+    def __hash__(self):
+        # __hash__ is None be default as __eq__ is overwritten
+        return super().__hash__()
+
     # return the value of the expression
     # optional, default: None
     def value(self):
         arg_vals = [arg.value() if isinstance(arg, Expression) else arg for arg in self.args]
         if any(a is None for a in arg_vals): return None
         if   self.name == "==": return (arg_vals[0] == arg_vals[1])
         elif self.name == "!=": return (arg_vals[0] != arg_vals[1])
         elif self.name == "<":  return (arg_vals[0] < arg_vals[1])
         elif self.name == "<=": return (arg_vals[0] <= arg_vals[1])
         elif self.name == ">":  return (arg_vals[0] > arg_vals[1])
         elif self.name == ">=": return (arg_vals[0] >= arg_vals[1])
         return None # default
 
+    def deepcopy(self, memodict={}):
+        """
+            Return a deep copy of the Comparison
+            :param: memodict: dictionary containing already copied objects, similar to copy.deepcopy()
+        """
+        copied_args = self._deepcopy_args(memodict)
+        return Comparison(self.name, *copied_args)
+
+
 
 class Operator(Expression):
     """
     All kinds of mathematical and logical operators on expressions
 
     Convention for 2-ary operators: if one of the two is a constant,
     it is stored first (as expr[0]), this eases weighted sum detection
     """
     allowed = {
         #name: (arity, is_bool)       arity 0 = n-ary, min 2
         'and': (0, True),
         'or':  (0, True),
-        'xor': (0, True),
         '->':  (2, True),
         'sum': (0, False),
         'wsum': (2, False),
         'sub': (2, False), # x - y
         'mul': (2, False),
         'div': (2, False),
         'mod': (2, False),
@@ -411,14 +460,18 @@
                 return arg
             return "{} {} {}".format(wrap_bracket(self.args[0]),
                                      printname,
                                      wrap_bracket(self.args[1]))
 
         return "{}({})".format(self.name, self.args)
 
+    def __hash__(self):
+        # __hash__ is None be default as __eq__ is overwritten
+        return super().__hash__()
+
     # if self is bool, special case
     def __eq__(self, other):
         if is_num(other) and other == 1:
             # check if bool operator, do not add == 1
             arity, is_bool = Operator.allowed[self.name]
             if is_bool:
                 return self
@@ -442,15 +495,14 @@
         elif self.name == "mod": return arg_vals[0] % arg_vals[1]
         elif self.name == "pow": return arg_vals[0] ** arg_vals[1]
         elif self.name == "-":   return -arg_vals[0]
         elif self.name == "abs": return -arg_vals[0] if arg_vals[0] < 0 else arg_vals[0]
         # boolean
         elif self.name == "and": return all(arg_vals)
         elif self.name == "or" : return any(arg_vals)
-        elif self.name == "xor": return sum(arg_vals) % 2 == 1
         elif self.name == "->": return (not arg_vals[0]) or arg_vals[1]
 
         return None # default
 
 def _wsum_should(arg):
     """ Internal helper: should the arg be in a wsum instead of sum """
     # Undecided: -x + y, -x + -y?
```

### Comparing `cpmpy-0.9.8/cpmpy/expressions/python_builtins.py` & `cpmpy-0.9.9/cpmpy/expressions/python_builtins.py`

 * *Files identical despite different names*

### Comparing `cpmpy-0.9.8/cpmpy/expressions/utils.py` & `cpmpy-0.9.9/cpmpy/expressions/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,28 +15,29 @@
         is_int
         is_num
         is_pure_list
         is_any_list
         flatlist
         all_pairs
         argval
+        eval_comparison
 """
 
 import numpy as np
 from collections.abc import Iterable # for _flatten
 from itertools import chain, combinations
 
 def is_int(arg):
-    """ is it an integer? (incl numpy variants)
+    """ can it be interpreted as an integer? (incl bool and numpy variants)
     """
-    return isinstance(arg, (int, np.integer))
+    return isinstance(arg, (bool, np.bool_, int, np.integer))
 def is_num(arg):
     """ is it an int or float? (incl numpy variants)
     """
-    return isinstance(arg, (int, np.integer, float, np.float64))
+    return isinstance(arg, (bool, np.bool_, int, np.integer, float, np.float64))
 def is_pure_list(arg):
     """ is it a list or tuple?
     """
     return isinstance(arg, (list, tuple))
 def is_any_list(arg):
     """ is it a list or tuple or numpy array?
     """
@@ -62,7 +63,38 @@
 
 def argval(a):
     """ returns .value() of Expression, otherwise the variable itself
         
         We check with hasattr instead of isinstance to avoid circular dependency
     """
     return a.value() if hasattr(a, "value") else a
+
+def eval_comparison(str_op, lhs, rhs):
+    """
+        Internal function: evaluates the textual `str_op` comparison operator
+        lhs <str_op> rhs
+
+        Valid str_op's:
+        * '=='
+        * '!='
+        * '>'
+        * '>='
+        * '<'
+        * '<='
+
+        Especially useful in decomposition and transformation functions that already involve a comparison.
+    """
+    if str_op == '==':
+        return lhs == rhs
+    elif str_op == '!=':
+        return lhs != rhs
+    elif str_op == '>':
+        return lhs > rhs
+    elif str_op == '>=':
+        return lhs >= rhs
+    elif str_op == '<':
+        return lhs < rhs
+    elif str_op == '<=':
+        return lhs <= rhs
+    else:
+        raise Exception("Not a known comparison:", str_op)
+
```

### Comparing `cpmpy-0.9.8/cpmpy/expressions/variables.py` & `cpmpy-0.9.9/cpmpy/expressions/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
         Model([ data[iv1] == iv2 ])
 
     As an alternative, you can also write the `Element` constraint directly on `data`: `Element(data, iv1) == iv2`
     """
     if not isinstance(arr, np.ndarray):
         arr = np.array(arr)
-    return NDVarArray(shape=arr.shape, dtype=type(arr.flat[0]), buffer=arr)
+    return NDVarArray(shape=arr.shape, dtype=arr.dtype, buffer=arr)
 
 
 class NullShapeError(Exception):
     def __init__(self, shape, message="Shape should be non-zero"):
         self.shape = shape
         self.message = message
         super().__init__(self.message)
@@ -238,14 +238,19 @@
     def __repr__(self):
         return self.name
 
     # for sets/dicts. Because names are unique, so is the str repr
     def __hash__(self):
         return hash(str(self))
 
+    def deepcopy(self, memodict={}):
+        copied = type(self)(self.lb, self.ub, self.name)
+        copied._value = self.value()
+        return copied
+
 class _IntVarImpl(_NumVarImpl):
     """
     **Integer** constraint variable with given lowerbound and upperbound.
 
     Do not create this object directly, use `intvar()` instead
     """
     counter = 0
@@ -346,14 +351,17 @@
 
     def __repr__(self):
         return "~{}".format(self._bv.name)
 
     def __invert__(self):
         return self._bv
 
+    def deepcopy(self, memodict={}):
+        return NegBoolView(self._bv.deepcopy(memodict))
+
 
 # subclass numericexpression for operators (first), ndarray for all the rest
 class NDVarArray(Expression, np.ndarray):
     """
     N-dimensional numpy array of variables.
 
     Do not create this object directly, use one of the functions in this module
@@ -367,14 +375,18 @@
     def is_bool(self):
         """ is it a Boolean (return type) Operator?
         """
         return False
 
     def value(self):
         return np.reshape([x.value() for x in self], self.shape)
+
+    def deepcopy(self, memodict={}):
+        copied = [arg.deepcopy(memodict) if isinstance(arg, Expression) else arg for arg in self]
+        return cpm_array(copied)
     
     def __repr__(self):
         """
             some ways in which np creates this object does not call
             the constructor, so the Expression does not have 'args'
             set..
         """
```

### Comparing `cpmpy-0.9.8/cpmpy/model.py` & `cpmpy-0.9.9/cpmpy/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,50 +112,34 @@
         """
             Maximize the given objective function
 
             `maximize()` can be called multiple times, only the last one is stored
         """
         self.objective(expr, minimize=False)
 
-    def _create_solver(self, solver):
-        """ Creates appropriate solver object
-
-        :param solver: name of a solver to use. Run SolverLookup.solvernames() to find out the valid solver names on your system. (default: None = first available solver)
-        """
-        if isinstance(solver, SolverInterface):
-            solver_class = solver
-        else:
-            solver_class = SolverLookup.lookup(solver)
-        assert(solver_class is not None)
-                
-        # instatiate solver with this model
-        if isinstance(solver, str) and ':' in solver:
-            # solver is a name that contains a subsolver
-            s = solver_class(self, subsolver=solver)
-        else:
-            # no subsolver
-            s = solver_class(self)
-
-        return s
-
     # solver: name of supported solver or any SolverInterface object
     def solve(self, solver=None, time_limit=None):
         """ Send the model to a solver and get the result
 
         :param solver: name of a solver to use. Run SolverLookup.solvernames() to find out the valid solver names on your system. (default: None = first available solver)
-        :type string: None (default) or in SolverLookup.solvernames() or a SolverInterface class (Class, not object! e.g. CPMpyOrTools, not CPMpyOrTools()!)
+        :type string: None (default) or a name in SolverLookup.solvernames() or a SolverInterface class (Class, not object!)
 
         :param time_limit: optional, time limit in seconds
         :type time_limit: int or float
 
         :return: Bool: the computed output:
             - True      if a solution is found (not necessarily optimal, e.g. could be after timeout)
             - False     if no solution is found
         """
-        s = self._create_solver(solver)
+        if isinstance(solver, SolverInterface):
+            # for advanced use, call its constructor with this model
+            s = solver(self)
+        else:
+            s = SolverLookup.get(solver, self)
+
         # call solver
         ret = s.solve(time_limit=time_limit)
         # store CPMpy status (s object has no further use)
         self.cpm_status = s.status()
         return ret
 
     def solveAll(self, solver=None, display=None, time_limit=None, solution_limit=None):
@@ -167,15 +151,20 @@
             Arguments:
                 - display: either a list of CPMpy expressions, OR a callback function, called with the variables after value-mapping
                         default/None: nothing displayed
                 - solution_limit: stop after this many solutions (default: None)
 
             Returns: number of solutions found
         """
-        s = self._create_solver(solver)
+        if isinstance(solver, SolverInterface):
+            # for advanced use, call its constructor with this model
+            s = solver(self)
+        else:
+            s = SolverLookup.get(solver, self)
+
         # call solver
         ret = s.solveAll(display=display,time_limit=time_limit,solution_limit=solution_limit)
         # store CPMpy status (s object has no further use)
         self.cpm_status = s.status()
         return ret
 
     def status(self):
@@ -227,8 +216,33 @@
         """
             Reads a Model instance from a binary pickled file
 
             :return: an object of :class: `Model`
         """
         with open(fname, "rb") as f:
             return pickle.load(f)
-    
+
+    def copy(self):
+        """
+            Makes a shallow copy of the model.
+            Constraints and variables are shared among the original and copied model.
+        """
+        if self.objective_is_min:
+            return Model(self.constraints, minimize=self.objective_)
+        else:
+            return Model(self.constraints, maximize=self.objective_)
+
+
+    def deepcopy(self, memodict={}):
+        """
+            Deep copies a the model to a new instance.
+            :return: an object of :class: 'Model' with equivalent constraints as the current model. There are no shared variables/constraints between the original model and its copied version.
+        """
+        copied_cons = [cpm_cons.deepcopy(memodict) for cpm_cons in self.constraints]
+        if self.objective_ is not None:
+            copied_obj = self.objective_.deepcopy(memodict)
+
+        copied_model = Model(copied_cons)
+        if self.objective_ is not None:
+            copied_model.objective(copied_obj, self.objective_is_min)
+
+        return copied_model
```

### Comparing `cpmpy-0.9.8/cpmpy/solvers/TEMPLATE.py` & `cpmpy-0.9.9/cpmpy/solvers/TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `cpmpy-0.9.8/cpmpy/solvers/__init__.py` & `cpmpy-0.9.9/cpmpy/solvers/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,25 +9,28 @@
     List of submodules
     ==================
     .. autosummary::
         :nosignatures:
 
         ortools
         pysat
+        gurobi
+        pysdd
         utils
 
     ===============
     List of classes
     ===============
     .. autosummary::
         :nosignatures:
 
         CPM_ortools
         CPM_pysat
         CPM_gurobi
+        CPM_pysdd
 
     =================
     List of functions
     =================
     .. autosummary::
         :nosignatures:
 
@@ -35,7 +38,8 @@
 """
 
 from .utils import builtin_solvers, get_supported_solvers, param_combinations
 from .ortools import CPM_ortools
 from .pysat import CPM_pysat
 from .minizinc import CPM_minizinc
 from .gurobi import  CPM_gurobi
+from .pysdd import CPM_pysdd
```

### Comparing `cpmpy-0.9.8/cpmpy/solvers/gurobi.py` & `cpmpy-0.9.9/cpmpy/solvers/gurobi.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,24 +25,23 @@
     Module details
     ==============
 """
 
 from .solver_interface import SolverInterface, SolverStatus, ExitStatus
 from ..expressions.core import *
 from ..expressions.variables import _BoolVarImpl, NegBoolView, _IntVarImpl, _NumVarImpl, intvar
+from ..transformations.comparison import only_numexpr_equality
 from ..transformations.flatten_model import flatten_constraint, flatten_objective, get_or_make_var
 from ..transformations.get_variables import get_variables
 from ..transformations.linearize import linearize_constraint, only_positive_bv
-from ..transformations.reification import only_bv_implies
+from ..transformations.reification import only_bv_implies, reify_rewrite
 
 try:
     import gurobipy as gp
-    GRB_env = gp.Env()
-    GRB_env.setParam("OutputFlag",0)
-    GRB_env.start()
+    GRB_ENV = None
 except ImportError as e:
     pass
 
 
 class CPM_gurobi(SolverInterface):
     """
     Interface to Gurobi's API
@@ -62,35 +61,38 @@
     """
 
     @staticmethod
     def supported():
         # try to import the package
         try:
             import gurobipy as gp
-            from datetime import datetime
-            valid_until = gp.Model().LicenseExpiration
-            today = datetime.today()
-            return today.year * 1e4 + today.month * 1e2 + today.day <= valid_until
-        except ImportError as e:
+            global GRB_ENV
+            if GRB_ENV is None:
+                # initialise the native gurobi model object
+                GRB_ENV = gp.Env()
+                GRB_ENV.setParam("OutputFlag", 0)
+                GRB_ENV.start()
+            return True
+        except:
             return False
 
     def __init__(self, cpm_model=None, subsolver=None):
         """
         Constructor of the native solver object
 
         Arguments:
         - cpm_model: a CPMpy Model()
         """
         if not self.supported():
             raise Exception(
                 "CPM_gurobi: Install the python package 'gurobipy' and make sure your licence is activated!")
         import gurobipy as gp
 
-        # initialise the native gurobi model object
-        self.grb_model = gp.Model(env=GRB_env)
+        # TODO: subsolver could be a GRB_ENV if a user would want to hand one over
+        self.grb_model = gp.Model(env=GRB_ENV)
 
         # initialise everything else and post the constraints/objective
         # it is sufficient to implement __add__() and minimize/maximize() below
         super().__init__(name="gurobi", cpm_model=cpm_model)
 
     def solve(self, time_limit=None, solution_callback=None, **kwargs):
         """
@@ -250,16 +252,18 @@
         # add new user vars to the set
         self.user_vars.update(get_variables(cpm_con))
 
         # apply transformations, then post internally
         # expressions have to be linearized to fit in MIP model. See /transformations/linearize
 
         cpm_cons = flatten_constraint(cpm_con)
+        cpm_cons = reify_rewrite(cpm_cons)
         cpm_cons = only_bv_implies(cpm_cons)
         cpm_cons = linearize_constraint(cpm_cons)
+        cpm_cons = only_numexpr_equality(cpm_cons)
         cpm_cons = only_positive_bv(cpm_cons)
 
         for con in cpm_cons:
             self._post_constraint(con)
 
         return self
 
@@ -274,86 +278,59 @@
         """
         from gurobipy import GRB
 
         # Comparisons: only numeric ones as 'only_bv_implies()' has removed the '==' reification for Boolean expressions
         # numexpr `comp` bvar|const
         if isinstance(cpm_expr, Comparison):
             lhs, rhs = cpm_expr.args
-            rvar = self.solver_var(rhs)
+            grbrhs = self.solver_var(rhs)
 
-
-            # TODO: this should become a transformation!!
-            if cpm_expr.name != '==' and not is_num(lhs) and \
-                    not isinstance(lhs, _NumVarImpl) and \
-                    not lhs.name == "sum" and \
-                    not lhs.name == "wsum":
-                # functional globals only exist for equality in gurobi
-                # example: min(x) > 10 :: min(x) == aux, aux > 10
-                # create the equality and overwrite lhs with auxiliary (will handle appropriate bounds)
-                (lhs, cons) = get_or_make_var(lhs)
-                self += cons
-
-            # all but '==' now only have as lhs: const|ivar|sum|wsum
-            # translate ivar|sum|wsum so they can be posted directly below
-            if isinstance(lhs, _NumVarImpl):
-                lhs = self.solver_var(lhs) # Case can be omitted -> handled in _make_num_expr
-            elif isinstance(lhs, Operator) and (lhs.name == 'sum' or lhs.name == 'wsum'):
-                # a BoundedLinearExpression LHS, special case, like in objective
-                lhs = self._make_numexpr(lhs)
-                # assumes that gurobi accepts sum(x) >= y without further simplification
-
-            # post the comparison
+            # Thanks to `only_numexpr_equality()` only supported comparisons should remain
             if cpm_expr.name == '<=':
-                return self.grb_model.addLConstr(lhs, GRB.LESS_EQUAL, rvar)
-            elif cpm_expr.name == '<':
-                raise Exception(f"{cpm_expr} should have been linearized, see /transformations/linearize.py")
+                grblhs = self._make_numexpr(lhs)
+                return self.grb_model.addLConstr(grblhs, GRB.LESS_EQUAL, grbrhs)
             elif cpm_expr.name == '>=':
-                return self.grb_model.addLConstr(lhs, GRB.GREATER_EQUAL, rvar)
-            elif cpm_expr.name == '>':
-                raise Exception(f"{cpm_expr} should have been linearized, see /transformations/linearize.py")
-            elif cpm_expr.name == '!=':
-                raise Exception(f"{cpm_expr} should have been linearized, see /transformations/linearize.py")
+                grblhs = self._make_numexpr(lhs)
+                return self.grb_model.addLConstr(grblhs, GRB.GREATER_EQUAL, grbrhs)
             elif cpm_expr.name == '==':
-                if not isinstance(lhs, Expression):
-                    # base cases: const|ivar|sum|wsum with prepped lhs above
-                    return self.grb_model.addLConstr(lhs, GRB.EQUAL, rvar)
+                if isinstance(lhs, _NumVarImpl) \
+                        or (isinstance(lhs, Operator) and (lhs.name == 'sum' or lhs.name == 'wsum')):
+                    # a BoundedLinearExpression LHS, special case, like in objective
+                    grblhs = self._make_numexpr(lhs)
+                    return self.grb_model.addLConstr(grblhs, GRB.EQUAL, grbrhs)
 
                 elif lhs.name == 'mul':
                     assert len(lhs.args) == 2, "Gurobi only supports multiplication with 2 variables"
                     a, b = self.solver_vars(lhs.args)
                     self.grb_model.setParam("NonConvex", 2)
-                    return self.grb_model.addConstr(a * b == rvar)
+                    return self.grb_model.addConstr(a * b == grbrhs)
 
                 elif lhs.name == 'div':
-                    if not isinstance(lhs.args[1], _NumVarImpl):
-                        a, b = self.solver_vars(lhs.args)
-                        return self.grb_model.addLConstr(a / b, GRB.EQUAL, rvar)
-                    raise Exception("Gurobi only supports division by constants")
+                    assert is_num(lhs.args[1]), "Gurobi only supports division by constants"
+                    a, b = self.solver_vars(lhs.args)
+                    return self.grb_model.addLConstr(a / b, GRB.EQUAL, grbrhs)
 
                 # General constraints
-                # rvar should be a variable, not a constant
-                if not isinstance(rhs, _NumVarImpl):
-                    rvar = self.solver_var(intvar(lb=rhs, ub=rhs))
-
-                if lhs.name == "and" or lhs.name == "or":
-                    raise Exception(f"{cpm_expr} should have been linearized, see /transformations/linearize.py")
-                elif lhs.name == 'min':
-                    return self.grb_model.addGenConstrMin(rvar, self.solver_vars(lhs.args))
+                # grbrhs should be a variable for gurobi in the subsequent, fake it
+                if is_num(grbrhs):
+                    grbrhs = self.solver_var(intvar(lb=grbrhs, ub=grbrhs))
+
+                if lhs.name == 'min':
+                    return self.grb_model.addGenConstrMin(grbrhs, self.solver_vars(lhs.args))
                 elif lhs.name == 'max':
-                    return self.grb_model.addGenConstrMax(rvar, self.solver_vars(lhs.args))
+                    return self.grb_model.addGenConstrMax(grbrhs, self.solver_vars(lhs.args))
                 elif lhs.name == 'abs':
-                    return self.grb_model.addGenConstrAbs(rvar, self.solver_var(lhs.args[0]))
+                    return self.grb_model.addGenConstrAbs(grbrhs, self.solver_var(lhs.args[0]))
                 elif lhs.name == 'pow':
                     x, a = self.solver_vars(lhs.args)
-                    assert a == 2, "Only support quadratic constraints"
-                    assert not isinstance(a, _NumVarImpl), f"Gurobi only supports power expressions with positive exponents."
-                    return self.grb_model.addGenConstrPow(x, rvar, a)
+                    assert a == 2, "Gurobi: 'pow', only support quadratic constraints (x**2)"
+                    return self.grb_model.addGenConstrPow(x, grbrhs, a)
 
             raise NotImplementedError(
-                "Not a know supported gurobi left-hand-side '{}' {}".format(lhs.name, cpm_expr))
+                "Not a know supported gurobi comparison '{}' {}".format(lhs.name, cpm_expr))
 
         elif isinstance(cpm_expr, Operator) and cpm_expr.name == "->":
             # Indicator constraints
             # Take form bvar -> sum(x,y,z) >= rvar
             cond, sub_expr = cpm_expr.args
             assert isinstance(cond, _BoolVarImpl), f"Implication constraint {cpm_expr} must have BoolVar as lhs"
             assert isinstance(sub_expr, Comparison), "Implication must have linear constraints on right hand side"
```

### Comparing `cpmpy-0.9.8/cpmpy/solvers/minizinc.py` & `cpmpy-0.9.9/cpmpy/solvers/minizinc.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
             # infix notation
             return "{} {} {}".format(args_str[0], expr.name, args_str[1])
 
         elif isinstance(expr, Operator):
             # some names differently (the infix names!)
             printmap = {'and': '/\\', 'or': '\\/',
                         'sum': '+', 'sub': '-',
-                        'mul': '*', 'div': '/', 'pow': '^'}
+                        'mul': '*', 'pow': '^'}
             op_str = expr.name
             if op_str in printmap:
                 op_str = printmap[op_str]
 
             # TODO: pretty printing of () as in Operator?
 
             # special case: unary -
@@ -426,15 +426,15 @@
                 # wrap args that are a subexpression in ()
                 for i, arg_str in enumerate(args_str):
                     if isinstance(expr.args[i], Expression):
                         args_str[i] = "(" + args_str[i] + ")"
                 return "{} {} {}".format(args_str[0], op_str, args_str[1])
 
             # special case: n-ary (non-binary): rename operator
-            printnary = {'and': 'forall', 'or': 'exists', 'xor': 'xorall', 'sum': 'sum'}
+            printnary = {'and': 'forall', 'or': 'exists', 'sum': 'sum'}
             if expr.name in printnary:
                 op_str = printnary[expr.name]
                 return "{}([{}])".format(op_str, ",".join(args_str))
 
             # default: prefix printing
             return "{}({})".format(op_str, ",".join(args_str))
 
@@ -456,14 +456,18 @@
         # rest: global constraints
         elif expr.name.endswith('circuit'):  # circuit, subcircuit
             # minizinc is offset 1, which can be problematic here...
             if any(isinstance(e, _IntVarImpl) and e.lb == 0 for e in expr.args):
                 # redo args_str[0]
                 args_str = ["{}+1".format(self._convert_expression(e)) for e in expr.args]
 
+        print_map = {"allequal":"all_equal", "xor":"xorall"}
+        if expr.name in print_map:
+            return "{}([{}])".format(print_map[expr.name], ",".join(args_str))
+
         # default (incl name-compatible global constraints...)
         return "{}([{}])".format(expr.name, ",".join(args_str))
 
     def solveAll(self, display=None, time_limit=None, solution_limit=None, **kwargs):
         """
             Compute all solutions and optionally display the solutions.
```

### Comparing `cpmpy-0.9.8/cpmpy/solvers/ortools.py` & `cpmpy-0.9.9/cpmpy/solvers/ortools.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,19 @@
         CPM_ortools
 """
 import sys  # for stdout checking
 
 from .solver_interface import SolverInterface, SolverStatus, ExitStatus
 from ..expressions.core import Expression, Comparison, Operator
 from ..expressions.variables import _NumVarImpl, _IntVarImpl, _BoolVarImpl, NegBoolView
-from ..expressions.utils import is_num, is_any_list
+from ..expressions.utils import is_num, is_any_list, eval_comparison
 from ..transformations.get_variables import get_variables_model, get_variables
 from ..transformations.flatten_model import flatten_model, flatten_constraint, flatten_objective, get_or_make_var, negated_normal
-from ..transformations.reification import only_bv_implies
+from ..transformations.reification import only_bv_implies, reify_rewrite
+from ..transformations.comparison import only_numexpr_equality
 
 class CPM_ortools(SolverInterface):
     """
     Interface to the python 'ortools' CP-SAT API
 
     Requires that the 'ortools' python package is installed:
     $ pip install ortools
@@ -70,25 +71,26 @@
         calling solve(), a prime way to use more advanced solver features
 
         Arguments:
         - cpm_model: Model(), a CPMpy Model() (optional)
         - subsolver: None
         """
         if not self.supported():
-            raise Exception("Install the python 'ortools' package to use this '{}' solver interface".format(name))
+            raise Exception("Install the python 'ortools' package to use this solver interface")
 
         from ortools.sat.python import cp_model as ort
 
         assert(subsolver is None)
 
         # initialise the native solver objects
         self.ort_model = ort.CpModel()
         self.ort_solver = ort.CpSolver()
 
-        # initialize assumption dict to None
+        # for solving with assumption variables,
+        # need to store mapping from ORTools Index to CPMpy variable
         self.assumption_dict = None
 
         # initialise everything else and post the constraints/objective
         super().__init__(name="ortools", cpm_model=cpm_model)
 
 
     def solve(self, time_limit=None, assumptions=None, solution_callback=None, **kwargs):
@@ -212,15 +214,15 @@
 
 
     def solver_var(self, cpm_var):
         """
             Creates solver variable for cpmpy variable
             or returns from cache if previously created
         """
-        if is_num(cpm_var): # shortcut, eases posting constraints
+        if is_num(cpm_var):  # shortcut, eases posting constraints
             return cpm_var
 
         # special case, negative-bool-view
         # work directly on var inside the view
         if isinstance(cpm_var, NegBoolView):
             return self.solver_var(cpm_var._bv).Not()
 
@@ -247,16 +249,16 @@
             'objective()' can be called multiple times, only the last one is stored
 
             (technical side note: any constraints created during conversion of the objective
             are premanently posted to the solver)
         """
         # make objective function non-nested
         (flat_obj, flat_cons) = flatten_objective(expr)
-        self += flat_cons # add potentially created constraints
-        self.user_vars.update(get_variables(flat_obj)) # add objvars to vars
+        self += flat_cons  # add potentially created constraints
+        self.user_vars.update(get_variables(flat_obj))  # add objvars to vars
 
         # make objective function or variable and post
         obj = self._make_numexpr(flat_obj)
         if minimize:
             self.ort_model.Minimize(obj)
         else:
             self.ort_model.Maximize(obj)
@@ -283,15 +285,15 @@
         # sum or weighted sum
         if isinstance(cpm_expr, Operator):
             if cpm_expr.name == 'sum':
                 return sum(self.solver_vars(cpm_expr.args))  # OR-Tools supports this
             elif cpm_expr.name == 'wsum':
                 w = cpm_expr.args[0]
                 x = self.solver_vars(cpm_expr.args[1])
-                return sum(wi*xi for wi,xi in zip(w,x)) # XXX is there more direct way?
+                return sum(wi*xi for wi,xi in zip(w,x))  # XXX is there a more direct way?
 
         raise NotImplementedError("ORTools: Not a know supported numexpr {}".format(cpm_expr))
 
 
     def __add__(self, cpm_con):
         """
         Post a (list of) CPMpy constraints(=expressions) to the solver
@@ -303,15 +305,19 @@
         :param cpm_con CPMpy constraint, or list thereof
         :type cpm_con (list of) Expression(s)
         """
         # add new user vars to the set
         self.user_vars.update(get_variables(cpm_con))
 
         # apply transformations, then post internally
-        cpm_cons = only_bv_implies(flatten_constraint(cpm_con))
+        cpm_cons = flatten_constraint(cpm_con)
+        cpm_cons = reify_rewrite(cpm_cons)
+        cpm_cons = only_numexpr_equality(cpm_cons)
+        cpm_cons = only_bv_implies(cpm_cons) # everything that can create
+                                             # reified expr must go before this
         for con in cpm_cons:
             self._post_constraint(con)
 
         return self
 
 
     def _post_constraint(self, cpm_expr, reifiable=False):
@@ -336,136 +342,94 @@
         # Operators: base (bool), lhs=numexpr, lhs|rhs=boolexpr (reified ->)
         elif isinstance(cpm_expr, Operator):
             # 'and'/n, 'or'/n, 'xor'/n, '->'/2
             if cpm_expr.name == 'and':
                 return self.ort_model.AddBoolAnd(self.solver_vars(cpm_expr.args))
             elif cpm_expr.name == 'or':
                 return self.ort_model.AddBoolOr(self.solver_vars(cpm_expr.args))
-            elif cpm_expr.name == 'xor':
-                return self.ort_model.AddBoolXOr(self.solver_vars(cpm_expr.args))
             elif cpm_expr.name == '->':
-                assert(isinstance(cpm_expr.args[0], _BoolVarImpl)) # lhs must be boolvar
+                assert(isinstance(cpm_expr.args[0], _BoolVarImpl))  # lhs must be boolvar
                 lhs = self.solver_var(cpm_expr.args[0])
                 if isinstance(cpm_expr.args[1], _BoolVarImpl):
                     # bv -> bv
                     return self.ort_model.AddImplication(lhs, self.solver_var(cpm_expr.args[1]))
                 else:
-                    # bv -> boolexpr, natively supported by or-tools
-                    # actually, only supported for and, or, and linear expression (not xor nor any global)
-                    # XXX should we check/assert that here??
-                    # TODO: and if rhs is a global, first decompose it and reify that??
-                    assert(cpm_expr.args[1].is_bool())
-                    # Special case for 'xor', which is not natively reifiable in ortools
-                    # TODO: make xor a global constraint (so it can be decomposed generally) and get rid of this special case here
-                    if isinstance(cpm_expr.args[1], Operator) and cpm_expr.args[1].name == 'xor':
-                        if len(cpm_expr.args) == 2:
-                            return self._post_constraint((sum(cpm_expr.args[1].args) == 1), reifiable=True).OnlyEnforceIf(lhs)
-                        else:
-                            raise NotImplementedError("ORT: reified n-ary XOR not yet supported, make an issue on github if you need it")
-                    # TODO: and if something like b.implies(min(x) >= 10) that it splits up in
-                    # b.implies( aux >= 10) & (min(x) == aux)
+                    # bv -> boolexpr
+                    # the `reify_rewrite()` transformation ensures that only
+                    # the natively reifiable 'and', 'or' and 'sum' remain here
                     return self._post_constraint(cpm_expr.args[1], reifiable=True).OnlyEnforceIf(lhs)
             else:
                 raise NotImplementedError("Not a know supported ORTools Operator '{}' {}".format(
                         cpm_expr.name, cpm_expr))
 
-
-        # Comparisons: only numeric ones as 'only_bv_implies()' has removed the '==' reification for Boolean expressions
+        # Comparisons: only numeric ones as the `only_bv_implies()` transformation
+        # has removed the '==' reification for Boolean expressions
         # numexpr `comp` bvar|const
         elif isinstance(cpm_expr, Comparison):
             lhs = cpm_expr.args[0]
-            rvar = self.solver_var(cpm_expr.args[1])
-
-            # TODO: this should become a transformation!!
-            if cpm_expr.name != '==' and not is_num(lhs) and not isinstance(lhs, _NumVarImpl)\
-                    and not lhs.name == "wsum" and not lhs.name == "sum":
-                # functional globals only exist for equality in ortools
-                # example: min(x) > 10 :: min(x) == aux, aux > 10
-                # create the equality and overwrite lhs with auxiliary (will handle appropriate bounds)
-                (lhs, cons) = get_or_make_var(lhs)
-                self += cons
+            ortrhs = self.solver_var(cpm_expr.args[1])
 
-            # all but '==' now only have as lhs: const|ivar|sum|wsum
-            # translate ivar|sum|wsum so they can be posted directly below
             if isinstance(lhs, _NumVarImpl):
-                lhs = self.solver_var(lhs)
+                # both are variables, do python comparison over ORT variables
+                return self.ort_model.Add(eval_comparison(cpm_expr.name, self.solver_var(lhs), ortrhs))
             elif isinstance(lhs, Operator) and (lhs.name == 'sum' or lhs.name == 'wsum'):
                 # a BoundedLinearExpression LHS, special case, like in objective
-                lhs = self._make_numexpr(lhs)
-                # assumes that ortools accepts sum(x) >= y without further simplification
-
-            # post the comparison
-            if cpm_expr.name == '<=':
-                return self.ort_model.Add(lhs <= rvar)
-            elif cpm_expr.name == '<':
-                return self.ort_model.Add(lhs < rvar)
-            elif cpm_expr.name == '>=':
-                return self.ort_model.Add(lhs >= rvar)
-            elif cpm_expr.name == '>':
-                return self.ort_model.Add(lhs > rvar)
-            elif cpm_expr.name == '!=':
-                return self.ort_model.Add(lhs != rvar)
+                ortlhs = self._make_numexpr(lhs)
+                # ortools accepts sum(x) >= y over ORT variables
+                return self.ort_model.Add(eval_comparison(cpm_expr.name, ortlhs, ortrhs))
             elif cpm_expr.name == '==':
-                if not isinstance(lhs, Expression): 
-                    # base cases: const|ivar|sum|wsum with prepped lhs above
-                    return self.ort_model.Add(lhs == rvar)
-                elif lhs.name == 'min':
-                    return self.ort_model.AddMinEquality(rvar, self.solver_vars(lhs.args))
+                # NumExpr == IV, supported by ortools (thanks to `only_numexpr_equality()` transformation)
+                if lhs.name == 'min':
+                    return self.ort_model.AddMinEquality(ortrhs, self.solver_vars(lhs.args))
                 elif lhs.name == 'max':
-                    return self.ort_model.AddMaxEquality(rvar, self.solver_vars(lhs.args))
+                    return self.ort_model.AddMaxEquality(ortrhs, self.solver_vars(lhs.args))
                 elif lhs.name == 'abs':
-                    return self.ort_model.AddAbsEquality(rvar, self.solver_var(lhs.args[0]))
+                    return self.ort_model.AddAbsEquality(ortrhs, self.solver_var(lhs.args[0]))
                 elif lhs.name == 'mul':
-                    return self.ort_model.AddMultiplicationEquality(rvar, self.solver_vars(lhs.args))
+                    return self.ort_model.AddMultiplicationEquality(ortrhs, self.solver_vars(lhs.args))
                 elif lhs.name == 'div':
-                    return self.ort_model.AddDivisionEquality(rvar, *self.solver_vars(lhs.args))
+                    return self.ort_model.AddDivisionEquality(ortrhs, *self.solver_vars(lhs.args))
                 elif lhs.name == 'element':
                     # arr[idx]==rvar (arr=arg0,idx=arg1), ort: (idx,arr,target)
                     return self.ort_model.AddElement(self.solver_var(lhs.args[1]),
-                                                     self.solver_vars(lhs.args[0]), rvar)
+                                                     self.solver_vars(lhs.args[0]), ortrhs)
                 elif lhs.name == 'mod':
                     # catch tricky-to-find ortools limitation
                     divisor = lhs.args[1]
                     if not is_num(divisor):
                         if divisor.lb <= 0 and divisor.ub >= 0:
                             raise Exception(
                                     f"Expression '{lhs}': or-tools does not accept a 'modulo' operation where '0' is in the domain of the divisor {divisor}:domain({divisor.lb}, {divisor.ub}). Even if you add a constraint that it can not be '0'. You MUST use a variable that is defined to be higher or lower than '0'.")
-                    return self.ort_model.AddModuloEquality(rvar, *self.solver_vars(lhs.args))
+                    return self.ort_model.AddModuloEquality(ortrhs, *self.solver_vars(lhs.args))
                 elif lhs.name == 'pow':
-                    # translate to multiplications
-                    # TODO: perhaps this should be a transformation too? pow to (binary) mult
-                    x = self.solver_var(lhs.args[0])
-                    y = lhs.args[1]
-                    assert is_num(y), f"Ort: 'pow' only supports constants as power, not {y}"
-                    if y == 0:
-                        return 1
-                    elif y == 1:
-                        return self.ort_model.Add(x == rvar)
-                    # mul([x,x,x,...]) with 'y' elements
-                    assert (y == 2), "Ort: 'pow' with an exponent larger than 2 has lead to crashes..."
-                    return self.ort_model.AddMultiplicationEquality(rvar, [x] * y)
+                    # only `POW(b,2) == IV` supported, post as b*b == IV
+                    assert (lhs.args[1] == 2), "Ort: 'pow', only var**2 supported, no other exponents"
+                    b = self.solver_var(lhs.args[0])
+                    return self.ort_model.AddMultiplicationEquality(ortrhs, [b,b])
             raise NotImplementedError(
                         "Not a know supported ORTools left-hand-side '{}' {}".format(lhs.name, cpm_expr))
 
 
         # rest: base (Boolean) global constraints
+        elif cpm_expr.name == 'xor':
+            return self.ort_model.AddBoolXOr(self.solver_vars(cpm_expr.args))
         elif cpm_expr.name == 'alldifferent':
             return self.ort_model.AddAllDifferent(self.solver_vars(cpm_expr.args))
         elif cpm_expr.name == 'table':
             assert (len(cpm_expr.args) == 2)  # args = [array, table]
             array, table = self.solver_vars(cpm_expr.args)
             return self.ort_model.AddAllowedAssignments(array, table)
         else:
-            # TODO: NOT YET MAPPED: Automaton, Circuit, Cumulative,
+            # NOT (YET?) MAPPED: Automaton, Circuit, Cumulative,
             #    ForbiddenAssignments, Inverse?, NoOverlap, NoOverlap2D,
             #    ReservoirConstraint, ReservoirConstraintWithActive
             
             # global constraint not known, try posting generic decomposition
-            self += cpm_expr.decompose() # assumes a decomposition exists...
-            # TODO: dynamic mapping of cpm_expr.name to API call? see #74
+            self += cpm_expr.decompose()  # assumes a decomposition exists...
+            # TODO: DirectConstraint/NativeConstraint from cpm_expr.name to API call? see #74
             return None # will throw error if used in reification
         
         raise NotImplementedError(cpm_expr)  # if you reach this... please report on github
 
 
     def solution_hint(self, cpm_vars, vals):
         """
@@ -476,15 +440,15 @@
         The solution hint does NOT need to satisfy all constraints, it should just provide reasonable default values for the variables. It can decrease solving times substantially, especially when solving a similar model repeatedly
 
         :param cpm_vars: list of CPMpy variables
         :param vals: list of (corresponding) values for the variables
         """
         self.ort_model.ClearHints() # because add just appends
         for (cpm_var, val) in zip(cpm_vars, vals):
-            self.ort_model.AddHint(self.ort_var(cpm_var), val)
+            self.ort_model.AddHint(self.solver_var(cpm_var), val)
 
 
     def get_core(self):
         from ortools.sat.python import cp_model as ort
         """
             For use with s.solve(assumptions=[...]). Only meaningful if the solver returned UNSAT. In that case, get_core() returns a small subset of assumption variables that are unsat together.
```

### Comparing `cpmpy-0.9.8/cpmpy/solvers/pysat.py` & `cpmpy-0.9.9/cpmpy/solvers/pysat.py`

 * *Files identical despite different names*

### Comparing `cpmpy-0.9.8/cpmpy/solvers/solver_interface.py` & `cpmpy-0.9.9/cpmpy/solvers/solver_interface.py`

 * *Files identical despite different names*

### Comparing `cpmpy-0.9.8/cpmpy/solvers/utils.py` & `cpmpy-0.9.9/cpmpy/solvers/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 import warnings # for deprecation warning
 
 from .gurobi import CPM_gurobi
 from .ortools import CPM_ortools
 from .minizinc import CPM_minizinc
 from .pysat import CPM_pysat
+from .pysdd import CPM_pysdd
 
 def param_combinations(all_params, remaining_keys=None, cur_params=None):
     """
         Recursively yield all combinations of param values
 
         For example usage, see `examples/advanced/hyperparameter_search.py`
 
@@ -63,17 +64,18 @@
         """
             Return ordered list of (name, class) of base CPMpy
             solvers
 
             First one is default
         """
         return [("ortools", CPM_ortools),
-                ("minizinc", CPM_minizinc),
+                ("gurobi", CPM_gurobi),
                 ("pysat", CPM_pysat),
-                ("gurobi", CPM_gurobi)
+                ("pysdd", CPM_pysdd),
+                ("minizinc", CPM_minizinc),
                ]
 
     @staticmethod
     def solvernames():
         names = []
         for (basename, CPM_slv) in SolverLookup.base_solvers():
             if CPM_slv.supported():
@@ -91,15 +93,15 @@
 
             This is the preferred way to initialise a solver from its name
         """
         cls = SolverLookup.lookup(name=name)
 
         # check for a 'solver:subsolver' name
         subname = None
-        if ':' in name:
+        if name is not None and ':' in name:
             _,subname = name.split(':',maxsplit=1)
         return cls(model, subsolver=subname)
 
     @staticmethod
     def lookup(name=None):
         """
             lookup a solver _class_ by its name
@@ -123,17 +125,17 @@
             if basename == solvername:
                 # CPM_slv is assigned the right one
                 break
 
         return CPM_slv
 
 
-# using builtin_solvers is DEPRECATED
+# using `builtin_solvers` is DEPRECATED, use `SolverLookup` object instead
 # Order matters! first is default, then tries second, etc...
-builtin_solvers=[CPM_ortools,CPM_minizinc,CPM_pysat]
+builtin_solvers = [CPM_ortools, CPM_gurobi, CPM_minizinc, CPM_pysat]
 def get_supported_solvers():
     """
         Returns a list of solvers supported on this machine.
 
     :return: a list of SolverInterface sub-classes :list[SolverInterface]:
     """
     warnings.warn("Deprecated, use Model.solvernames() instead, will be removed in stable version", DeprecationWarning)
```

### Comparing `cpmpy-0.9.8/cpmpy/transformations/__init__.py` & `cpmpy-0.9.9/cpmpy/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cpmpy-0.9.8/cpmpy/transformations/flatten_model.py` & `cpmpy-0.9.9/cpmpy/transformations/flatten_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,225 +70,182 @@
 
 The output after calling flatten_model() or flatten_constraint() will ONLY contain expressions
 of the form specified above.
 
 The flattening does not promise to do common subexpression elimination or to automatically group
 commutative expressions (and, or, sum, wsum, ...) but such optimisations should be added later.
 
-TODO: remove zipcycle (no longer needed)
-TODO: use normalized_boolexpr when possible in the flatten_cons operator case.
 TODO: update behind_the_scenes.rst doc with the new 'flat normal form'
 TODO: small optimisations, e.g. and/or chaining (potentially after negation), see test_flatten
 """
 import copy
 import math
 import numpy as np
 from ..expressions.core import *
 from ..expressions.variables import _NumVarImpl, _IntVarImpl, _BoolVarImpl, NegBoolView
 from ..expressions.utils import is_num, is_any_list
 
-from itertools import cycle
-def __zipcycle(vars1, vars2):
-    v1 = [vars1] if not is_any_list(vars1) else vars1
-    v2 = [vars2] if not is_any_list(vars2) else vars2
-    return zip(v1, cycle(v2)) if len(v2) < len(v1) else zip(cycle(v1), v2)
-
 def flatten_model(orig_model):
     """
         Receives model, returns new model where every constraint is in 'flat normal form'
     """
-    from ..model import Model # otherwise circular dependency...
+    from ..model import Model  # otherwise circular dependency...
 
     # the top-level constraints
     basecons = []
     for con in orig_model.constraints:
         basecons += flatten_constraint(con)
 
     # the objective
     if orig_model.objective_ is None:
-        return Model(*basecons) # no objective, satisfaction problem
+        return Model(*basecons)  # no objective, satisfaction problem
     else:
         (newobj, newcons) = flatten_objective(orig_model.objective_)
         basecons += newcons
         if orig_model.objective_is_min:
             return Model(*basecons, minimize=newobj)
         else:
             return Model(*basecons, maximize=newobj)
 
 
 def flatten_constraint(expr):
     """
-        input is any expression; except is_num(), pure _NumVarImpl,
+        input is any expression; except bool, is_num(), pure _NumVarImpl,
         or Operator/GlobalConstraint with not is_bool()
         
         output: see definition of 'flat normal form' above.
 
         it will return 'Exception' if something is not supported
         TODO, what built-in python error is best?
     """
     # base cases
-    if isinstance(expr, _BoolVarImpl) or isinstance(expr, bool):
+    if isinstance(expr, bool):
+        if expr:
+            return []
+        else:
+            return [expr]  # not sure about this one... means False is a valid FNF expression
+    elif isinstance(expr, _BoolVarImpl):
         return [expr]
     elif is_num(expr) or isinstance(expr, _NumVarImpl):
         raise Exception("Numeric constants or numeric variables not allowed as base constraint")
 
     # recursively flatten list of constraints
     if is_any_list(expr):
-        flatcons = [flatten_constraint(e) for e in expr]
-        return [c for con in flatcons for c in con]
+        flatcons = []
+        for e in expr:
+            flatcons += flatten_constraint(e)  # add all at end
+        return flatcons
     # recursively flatten top-level 'and'
     if isinstance(expr, Operator) and expr.name == 'and':
-        flatcons = [flatten_constraint(e) for e in expr.args]
-        return [c for con in flatcons for c in con]
+        flatcons = []
+        for e in expr.args:
+            flatcons += flatten_constraint(e)  # add all at end
+        return flatcons
 
     assert expr.is_bool(), f"Boolean expressions only in flatten_constraint, `{expr}` not allowed."
 
     if isinstance(expr, Operator):
         """
-            - Base Boolean operators: and([Var]), or([Var]), xor([Var]) (CPMpy class 'Operator', is_bool())
-            - Base Boolean impliciation: Var -> Var                     (CPMpy class 'Operator', is_bool())
+            - Base Boolean operators: and([Var]), or([Var])        (CPMpy class 'Operator', is_bool())
+            - Base Boolean impliciation: Var -> Var                (CPMpy class 'Operator', is_bool())
             - Implication: Boolexpr -> Var                         (CPMpy class 'Operator', is_bool())
                            Var -> Boolexpr                         (CPMpy class 'Operator', is_bool())
         """
         # does not type-check that arguments are bool... Could do now with expr.is_bool()!
         if all(__is_flat_var(arg) for arg in expr.args):
             return [expr]
-        elif not expr.name == '->':
-            # and, or, xor
-            # recursively flatten all children
-            flatvars, flatcons = zip(*[get_or_make_var(arg) for arg in expr.args])
 
-            newexpr = Operator(expr.name, flatvars)
-            return [newexpr]+[c for con in flatcons for c in con]
-        else:
+        if expr.name == '->':
             # ->, allows a boolexpr on one side
             if isinstance(expr.args[0], _BoolVarImpl):
                 # LHS is var, ensure RHS is normalized 'Boolexpr'
                 lhs = expr.args[0]
                 (rhs,flatcons) = normalized_boolexpr(expr.args[1])
             else:
                 # make LHS normalized 'Boolexpr', RHS must be a var
                 (lhs,lcons) = normalized_boolexpr(expr.args[0])
                 (rhs,rcons) = get_or_make_var(expr.args[1])
                 flatcons = lcons+rcons
 
             newexpr = Operator(expr.name, (lhs,rhs))
-            return [newexpr]+[c for c in flatcons]
+            return [newexpr]+flatcons
+        else:
+            # a normalizable boolexpr
+            (con, flatcons) = normalized_boolexpr(expr)
+            return [con]+flatcons
+
 
     elif isinstance(expr, Comparison):
         """
     - Base Boolean equality: Var == Var                         (CPMpy class 'Comparison')
                              Var == Constant                    (CPMpy class 'Comparison')
     - Numeric equality:  Numexpr == Var                    (CPMpy class 'Comparison')
                          Numexpr == Constant               (CPMpy class 'Comparison')
     - Numeric disequality: Numexpr != Var                  (CPMpy class 'Comparison')
                            Numexpr != Constant             (CPMpy class 'Comparison')
     - Numeric inequality (>=,>,<,<=,): Numexpr >=< Var     (CPMpy class 'Comparison')
     - Reification (double implication): Boolexpr == Var    (CPMpy class 'Comparison')
         """
+        if all(__is_flat_var(arg) for arg in expr.args):
+            return [expr]
 
-        flatcons = []
-        # zipcycle: unfolds 'arr1 == arr2' pairwise
-        # XXX: zipcycle no longer needed, vectorized now handled at creation level!
-        for lexpr, rexpr in __zipcycle(expr.args[0], expr.args[1]):
-            if __is_flat_var(lexpr) and __is_flat_var(rexpr):
-                flatcons += [Comparison(expr.name, lexpr, rexpr)]
+        # swap 'Var == Expr' to normal 'Expr == Var'
+        lexpr, rexpr = expr.args
+        if (expr.name == '==' or expr.name == '!=') \
+                and __is_flat_var(lexpr) and not __is_flat_var(rexpr):
+            lexpr, rexpr = rexpr, lexpr
+
+        # ensure rhs is var
+        (rvar, rcons) = get_or_make_var(rexpr)
+
+        exprname = expr.name  # so it can be modified
+        # 'BoolExpr != Rvar' to normal 'BoolExpr == ~Rvar'
+        if exprname == '!=' and lexpr.is_bool():  # negate rvar
+            exprname = '=='
+            rvar = ~rvar
+
+        # Reification (double implication): Boolexpr == Var
+        if exprname == '==' and lexpr.is_bool():
+            if is_num(rexpr):
+                # shortcut, full original one is normalizable BoolExpr
+                # such as And(v1,v2,v3) == 0
+                (con, flatcons) = normalized_boolexpr(expr)
+                return [con]+flatcons
             else:
-                # RHS must be var (or const)
-                lexpr,rexpr = expr.args
-                exprname = expr.name
-                # ==,!=: can swap if lhs is var and rhs is not
-                # TODO: this is very similar to (part of) normalize_boolexpr??
-                # XXX indeed, every case that is not 'reification' can be
-                # delegated to normalize_boolexpr... TODO
-                if (exprname == '==' or exprname == '!=') and \
-                    not __is_flat_var(rexpr) and __is_flat_var(lexpr):
-                    (lexpr,rexpr) = (rexpr,lexpr)
-                # ensure rhs is var
-                (rvar, rcons) = get_or_make_var(rexpr)
-
-                # LHS: check if Boolexpr == smth:
-                if (exprname == '==' or exprname == '!=') and lexpr.is_bool():
-                    if is_num(rexpr):
-                        # BoolExpr == 0|False
-                        # special case, handled in normalized_boolexpr()
-                        (con, subs) = normalized_boolexpr(expr)
-                        flatcons += [con] + subs
-                        continue # ready with this one
-
-                    # Reification (double implication): Boolexpr == Var
-                    if __is_flat_var(lexpr):
-                        (lhs, lcons) = (lexpr, [])
-                    else:
-                        (lhs, lcons) = normalized_boolexpr(lexpr)
-                    if expr.name == '!=':
-                        # != not needed, negate RHS variable
-                        rhs = ~rvar
-                        exprname = '=='
-                else:
-                    # other cases: LHS is numexpr
-                    (lhs, lcons) = normalized_numexpr(lexpr)
-
-                flatcons += [Comparison(exprname, lhs, rvar)]+lcons+rcons
+                (lhs, lcons) = normalized_boolexpr(lexpr)
+        else:
+            # other cases: LHS is numexpr
+            (lhs, lcons) = normalized_numexpr(lexpr)
 
-        return flatcons
+        return [Comparison(exprname, lhs, rvar)]+lcons+rcons
 
     else:
         """
     - Global constraint (Boolean): global([Var]*)          (CPMpy class 'GlobalConstraint', is_bool())
         """
-        # just recursively flatten args, which can be lists
-        if all(__is_flat_var_or_list(arg) for arg in expr.args):
-            return [expr]
-        else:
-            # recursively flatten all children
-            flatvars, flatcons = zip(*[get_or_make_var_or_list(arg) for arg in expr.args])
-
-            # take copy, replace args
-            newexpr = copy.copy(expr) # shallow or deep? currently shallow
-            newexpr.args = flatvars
-            return [newexpr]+[c for con in flatcons for c in con]
+        (con, flatcons) = normalized_boolexpr(expr)
+        return [con] + flatcons
 
 
-def flatten_objective(expr):
+def flatten_objective(expr, supported=frozenset(["sum","wsum"])):
     """
     - Decision variable: Var
     - Linear: sum([Var])                                   (CPMpy class 'Operator', name 'sum')
               wsum([Const],[Var])                          (CPMpy class 'Operator', name 'wsum')
     """
-    if __is_flat_var(expr):
-        return (expr, [])
-
     # lets be very explicit here
     if is_any_list(expr):
         # one source of errors is sum(v) where v is a matrix, use v.sum() instead
         raise Exception(f"Objective expects a single variable/expression, not a list of expressions")
 
-    if isinstance(expr, Operator) and (expr.name == 'sum' or expr.name == 'wsum'):
-        if expr.name == 'sum':
-            if all(__is_flat_var(arg) for arg in expr.args):
-                return (expr, [])
-            else:
-                # one of the arguments is not flat, flatten all
-                flatvars, flatcons = zip(*[get_or_make_var(arg) for arg in expr.args])
-                newexpr = Operator(expr.name, flatvars)
-                return (newexpr, [c for con in flatcons for c in con])
-        elif expr.name == 'wsum':
-            w, x = expr.args
-            if all(__is_flat_var(arg) for arg in x):
-                return (expr, [])
-            else:
-                # one of the arguments is not flat, flatten all
-                flatvars, flatcons = zip(*[get_or_make_var(arg) for arg in x])
-                # one of the expressions in x is not flat, flatten all
-                newexpr = Operator(expr.name, (w, flatvars))
-                return (newexpr, [c for con in flatcons for c in con])
-    
-    # any other numeric expression
-    return get_or_make_var(expr)
+    if isinstance(expr, Expression) and expr.name in supported:
+        return normalized_numexpr(expr)
+    else:
+        # any other numeric expression
+        return get_or_make_var(expr)
 
 
 def __is_flat_var(arg):
     """ True if the variable is a numeric constant, or a _NumVarImpl (incl subclasses)
     """
     return is_num(arg) or isinstance(arg, _NumVarImpl)
 
@@ -310,113 +267,90 @@
         return (expr, [])
 
     if is_any_list(expr):
         raise Exception(f"Expected single variable, not a list for: {expr}")
 
     if expr.is_bool():
         # normalize expr into a boolexpr LHS, reify LHS == bvar
-        (newexpr, flatcons) = normalized_boolexpr(expr)
+        (flatexpr, flatcons) = normalized_boolexpr(expr)
 
         bvar = _BoolVarImpl()
-        return (bvar, [newexpr == bvar]+flatcons)
+        return (bvar, [flatexpr == bvar]+flatcons)
 
-    #else:
-    # normalize expr into a numexpr LHS, return LHS == intvar
-    # includes estimating appropriate bounds for intvar...
-
-    # special case, -var... 
-    if isinstance(expr, Operator) and expr.name == '-': # unary
-        return get_or_make_var(-1*expr.args[0])
-
-    elif isinstance(expr, Operator) and expr.name == "wsum":
-        weights, sub_exprs  = expr.args
-        flatvars, flatcons = zip(*[get_or_make_var(arg) for arg in sub_exprs]) # also bool, reified...
-        bounds = np.array([[w * fvar.lb for w, fvar in zip(weights, flatvars)],
-                           [w * fvar.ub for w, fvar in zip(weights, flatvars)]])
-        lb, ub = bounds.min(axis=1).sum(), bounds.max(axis=1).sum()
-        ivar = _IntVarImpl(lb, ub)
-        newexpr = (Operator(expr.name, (weights, flatvars)) == ivar)
-        return (ivar, [newexpr]+[c for con in flatcons for c in con])
+    else:
+        # normalize expr into a numexpr LHS,
+        # then compute bounds and return (newintvar, LHS == newintvar)
+        (flatexpr, flatcons) = normalized_numexpr(expr)
+
+        if isinstance(flatexpr, Operator) and expr.name == "wsum":
+            # more complex args, and weights can be negative, so more complex lbs/ubs
+            weights, flatvars  = flatexpr.args
+            bounds = np.array([[w * fvar.lb for w, fvar in zip(weights, flatvars)],
+                               [w * fvar.ub for w, fvar in zip(weights, flatvars)]])
+            lb, ub = bounds.min(axis=0).sum(), bounds.max(axis=0).sum() # for every column is axis=0...
+            ivar = _IntVarImpl(lb, ub)
+            return (ivar, [flatexpr == ivar]+flatcons)
 
-    elif isinstance(expr, Operator):
-        # TODO: more like above, call normalized_numexpr() on expr, then equate...
-        flatvars, flatcons = zip(*[get_or_make_var(arg) for arg in expr.args]) # also bool, reified...
-        lbs = [var.lb if isinstance(var, _NumVarImpl) else var for var in flatvars]
-        ubs = [var.ub if isinstance(var, _NumVarImpl) else var for var in flatvars]
-
-        if expr.name == 'abs': # unary
-            if lbs[0] < 0 and ubs[0] > 0:
-                lb = 0 # from neg to pos, so includes 0
+        elif isinstance(flatexpr, Operator):
+            lbs = [var.lb if isinstance(var, _NumVarImpl) else var for var in flatexpr.args]
+            ubs = [var.ub if isinstance(var, _NumVarImpl) else var for var in flatexpr.args]
+
+            if flatexpr.name == 'abs': # unary
+                if lbs[0] < 0 and ubs[0] > 0:
+                    lb = 0 # from neg to pos, so includes 0
+                else:
+                    lb = min(abs(lbs[0]), abs(ubs[0])) # same sign, take smallest
+                ub = max(abs(lbs[0]), abs(ubs[0])) # largest abs value
+                ivar = _IntVarImpl(lb, ub)
+            elif flatexpr.name == 'mul': # binary
+                v0 = [lbs[0], ubs[0]]
+                v1 = [lbs[1], ubs[1]]
+                bnds = [v0[i]*v1[j] for i in [0,1] for j in [0,1]]
+                ivar = _IntVarImpl(min(bnds),max(bnds))
+            elif flatexpr.name == 'div': # binary
+                num = [lbs[0], ubs[0]]
+                denom = [lbs[1], ubs[1]]
+                bnds = [num[i]/denom[j] for i in [0,1] for j in [0,1]]
+                # the above can give fractional values, tighten bounds to integer
+                ivar = _IntVarImpl(math.ceil(min(bnds)), math.floor(max(bnds)))
+            elif flatexpr.name == 'mod': # binary
+                l = np.arange(lbs[0], ubs[0]+1)
+                r = np.arange(lbs[1], ubs[1]+1)
+                # check all possibilities
+                remainders = np.mod(l[:,None],r)
+                lb, ub = np.min(remainders), np.max(remainders)
+                ivar = _IntVarImpl(lb,ub)
+            elif flatexpr.name == 'pow': # binary
+                base = [lbs[0], ubs[0]]
+                exp = [lbs[1], ubs[1]]
+                if exp[0] < 0:
+                    raise NotImplementedError("Power operator: For integer values, exponent must be non-negative")
+                bnds = [base[i]**exp[j] for i in [0,1] for j in [0,1]]
+                if exp[1] > 0: # even/uneven behave differently when base is negative
+                    bnds += [base[0]**(exp[1]-1), base[1]**(exp[1]-1)]
+                ivar = _IntVarImpl(min(bnds), max(bnds))
+            elif flatexpr.name == 'sum': # n-ary
+                ivar = _IntVarImpl(sum(lbs), sum(ubs))
+            elif flatexpr.is_bool(): # Boolean
+                ivar = _BoolVarImpl() # TODO: we can support Bool? check, update docs
             else:
-                lb = min(abs(lbs[0]), abs(ubs[0])) # same sign, take smallest
-            ub = max(abs(lbs[0]), abs(ubs[0])) # largest abs value
-            ivar = _IntVarImpl(lb, ub)
-        elif expr.name == 'mul': # binary
-            v0 = [lbs[0], ubs[0]]
-            v1 = [lbs[1], ubs[1]]
-            bnds = [v0[i]*v1[j] for i in [0,1] for j in [0,1]]
-            ivar = _IntVarImpl(min(bnds),max(bnds)) 
-        elif expr.name == 'div': # binary
-            num = [lbs[0], ubs[0]]
-            denom = [lbs[1], ubs[1]]
-            bnds = [num[i]/denom[j] for i in [0,1] for j in [0,1]]
-            # the above can give fractional values, tighten bounds to integer
-            ivar = _IntVarImpl(math.ceil(min(bnds)), math.floor(max(bnds))) 
-        elif expr.name == 'mod': # binary 
-            # check all possibilities...
-            l = np.arange(lbs[0], ubs[0]+1)
-            lb = np.min(np.mod(l, lbs[1]))
-            ub = np.max(np.mod(l, lbs[1]))
-            for m in range(lbs[1]+1, lbs[1]+1):
-                lb = np.min(lb, np.min(np.mod(l, m)))
-                ub = np.max(lb, np.max(np.mod(l, m)))
-            ivar = _IntVarImpl(lb,ub)
-        elif expr.name == 'pow': # binary
-            base = [lbs[0], ubs[0]]
-            exp = [lbs[1], ubs[1]]
-            if exp[0] < 0:
-                raise NotImplementedError("Power operator: For integer values, exponent must be non-negative")
-            bnds = [base[i]**exp[j] for i in [0,1] for j in [0,1]]
-            if exp[1] > 0: # even/uneven behave differently when base is negative
-                bnds += [base[0]**(exp[1]-1), base[1]**(exp[1]-1)]
-            ivar = _IntVarImpl(min(bnds), max(bnds))
-        elif expr.name == 'sum': # n-ary
-            ivar = _IntVarImpl(sum(lbs), sum(ubs)) 
-        elif expr.is_bool(): # Boolean
-            ivar = _BoolVarImpl() # TODO: we can support Bool? check, update docs
-        else:
-            raise Exception("Operator '{}' not known in get_or_make_var".format(expr.name)) # or bug
+                raise Exception("Operator '{}' not known in get_or_make_var".format(expr.name)) # or bug
 
-        newexpr = (Operator(expr.name, flatvars) == ivar)
-        return (ivar, [newexpr]+[c for con in flatcons for c in con])
+            return (ivar, [flatexpr == ivar]+flatcons)
 
-    else:
-        """
-        - Global constraint (non-Boolean) (examples: Max,Min,Element)
-        """
-        # just recursively flatten args, which can be lists
-        if all(__is_flat_var_or_list(arg) for arg in expr.args):
-            newexpr = expr
-            flatcons = []
         else:
-            flatvars, flatcons = zip(*[get_or_make_var_or_list(arg) for arg in expr.args]) # also bool, reified...
-            #idx, icons = flatten_numexpr(idx)
-            #arr, acons = zip(*[flatten_numexpr(e) for e in arr])
-            #basecons = icons+[c for con in acons for c in con]
-
-            # take copy, replace args
-            newexpr = copy.copy(expr) # shallow or deep? currently shallow
-            newexpr.args = flatvars
+            """
+            - Global constraint (non-Boolean) (examples: Max,Min,Element)
+            """
+            # we don't currently have a generic way to get bounds from non-Boolean globals...
+            # XXX Add to GlobalCons as function? e.g. (lb,ub) = expr.get_bounds()? would also work for Operator...
+            ivar = _IntVarImpl(-2147483648, 2147483647) # TODO, this can breaks solvers
 
-        # XXX Also, how to get the bounds on the new variable? have the solver handle it?
-        # XXX Add to GlobalCons as function? e.g. (lb,ub) = expr.get_bounds()? would also work for Operator...
-        ivar = _IntVarImpl(-2147483648, 2147483647) # TODO, this can breaks solvers
+            return (ivar, [flatexpr == ivar]+flatcons)
 
-        return (ivar, [newexpr == ivar]+[c for con in flatcons for c in con])
-    
 
 def get_or_make_var_or_list(expr):
     """ Like get_or_make_var() but also accepts and recursively transforms lists
         Used to convert arguments of globals
     """
     if __is_flat_var_or_list(expr):
         return (expr,[])
@@ -434,28 +368,28 @@
             - expr == BoolVar
             - expr != BoolVar
             - expr -> BoolVar
 
         are valid expressions.
 
         Currently, this is the case for:
-        - Boolean operators: and([Var]), or([Var]), xor([Var]) (CPMpy class 'Operator', is_bool())
+        - Boolean operators: and([Var]), or([Var])             (CPMpy class 'Operator', is_bool())
         - Boolean equality: Var == Var                         (CPMpy class 'Comparison')
         - Global constraint (Boolean): global([Var]*)          (CPMpy class 'GlobalConstraint', is_bool())
         - Comparison constraint (see elsewhere)                (CPMpy class 'Comparison')
 
         output: (base_expr, base_cons) with:
             base_expr: same as 'expr', but all arguments are variables
             base_cons: list of flat normal constraints
     """
     assert(not __is_flat_var(expr))
     assert(expr.is_bool()) 
 
     if isinstance(expr, Operator):
-        # and, or, xor, ->
+        # and, or, ->
 
         # apply De Morgan's transform for "implies"
         if expr.name == '->':
             # TODO, optimisation if args0 is an 'and'?
             (lhs,lcons) = get_or_make_var(expr.args[0])
             # TODO, optimisation if args1 is an 'or'?
             (rhs,rcons) = get_or_make_var(expr.args[1])
@@ -507,64 +441,61 @@
 
                 # make LHS like objective, RHS var
                 (lrich, lcons) = flatten_objective(lexpr)
                 (rvar, rcons) = flatten_numexpr(rexpr)
                 flatcons += [Comparison(newname, lrich, rvar)]+lcons+rcons
             """
 
-            # XXX This is duplicate code from flatten_constraint!!! (except return)
-            # -> move into shared function??? or call this one there?
-            # But should support one 'less' level of nesting?
-
             # RHS must be var (or const)
-            lexpr,rexpr = expr.args
+            lexpr, rexpr = expr.args
             exprname = expr.name
+
             # ==,!=: can swap if lhs is var and rhs is not
             if (exprname == '==' or exprname == '!=') and \
                 not __is_flat_var(rexpr) and __is_flat_var(lexpr):
-                (lexpr,rexpr) = (rexpr,lexpr)
+                lexpr, rexpr = rexpr, lexpr
+
             # ensure rhs is var
             (rvar, rcons) = get_or_make_var(rexpr)
 
             # LHS: check if Boolexpr == smth:
             if (exprname == '==' or exprname == '!=') and lexpr.is_bool():
                 if is_num(rexpr):
                     # BoolExpr == 0|False
-                    assert(not rexpr) # 'true' is preprocessed away
+                    assert (not rexpr), f"should be false: {rexpr}" # 'true' is preprocessed away
 
                     nnexpr = negated_normal(lexpr)
                     return normalized_boolexpr(nnexpr)
 
-                # Reification (double implication): Boolexpr == Var
-                (lhs, lcons) = normalized_boolexpr(lexpr)
+                # this is a reified constraint, so lhs must be var too to be in normal form
+                (lhs, lcons) = get_or_make_var(lexpr)
                 if expr.name == '!=':
                     # != not needed, negate RHS variable
                     rhs = ~rvar
                     exprname = '=='
             else:
                 # other cases: LHS is numexpr
                 (lhs, lcons) = normalized_numexpr(lexpr)
 
             return (Comparison(exprname, lhs, rvar), lcons+rcons)
 
     else:
         """
         - Global constraint (Boolean): global([Var]*)          (CPMpy class 'GlobalConstraint', is_bool())
         """
-        # XXX literal copy from flatten_cons... (except return)
         # just recursively flatten args, which can be lists
         if all(__is_flat_var_or_list(arg) for arg in expr.args):
             return (expr, [])
         else:
             # recursively flatten all children
-            flatvars, flatcons = zip(*[get_or_make_var_or_list(arg) for arg in expr.args])
+            flatargs, flatcons = zip(*[get_or_make_var_or_list(arg) for arg in expr.args])
 
             # take copy, replace args
             newexpr = copy.copy(expr) # shallow or deep? currently shallow
-            newexpr.args = flatvars
+            newexpr.args = flatargs
             return (newexpr, [c for con in flatcons for c in con])
 
 
 def normalized_numexpr(expr):
     """
         all 'flat normal form' numeric expressions...
 
@@ -579,40 +510,42 @@
             base_expr: same as 'expr', but all arguments are variables
             base_cons: list of flat normal constraints
     """
     # XXX a boolexpr is also a valid numexpr... e.g. 30*(iv > 5) + ... see mario obj.
     if __is_flat_var(expr):
         return (expr, [])
 
-    # special case, -var... 
-    # XXX until we do weighted sum, turn into -1*args[0]
-    if isinstance(expr, Operator) and expr.name == '-': # unary
-        return normalized_numexpr(-1*expr.args[0])
-
-    elif isinstance(expr, Operator) and expr.name == 'wsum': # unary
-        weights, sub_exprs  = expr.args
-        flatvars, flatcons = map(list, zip(*[get_or_make_var(arg) for arg in sub_exprs])) # also bool, reified...
-        newexpr = Operator(expr.name, (weights, flatvars))
-        return (newexpr, [c for con in flatcons for c in con])
+    elif expr.is_bool():
+        # unusual case, but its truth-value is a valid numexpr
+        # so reify and return the boolvar
+        return get_or_make_var(expr)
+
+    elif isinstance(expr, Operator):
+        # special case, -var, turn into -1*args[0]
+        if expr.name == '-': # unary
+            return normalized_numexpr(-1*expr.args[0])
 
-    if isinstance(expr, Operator):
         if all(__is_flat_var(arg) for arg in expr.args):
             return (expr, [])
-        
-        # recursively flatten all children
-        flatvars, flatcons = zip(*[get_or_make_var(arg) for arg in expr.args])
 
-        newexpr = Operator(expr.name, flatvars)
-        return (newexpr, [c for con in flatcons for c in con])
+        elif expr.name == 'wsum': # unary
+            weights, sub_exprs  = expr.args
+            flatvars, flatcons = map(list, zip(*[get_or_make_var(arg) for arg in sub_exprs])) # also bool, reified...
+            newexpr = Operator(expr.name, (weights, flatvars))
+            return (newexpr, [c for con in flatcons for c in con])
 
+        else: # generic operator
+            # recursively flatten all children
+            flatvars, flatcons = zip(*[get_or_make_var(arg) for arg in expr.args])
+
+            newexpr = Operator(expr.name, flatvars)
+            return (newexpr, [c for con in flatcons for c in con])
     else:
-        """
-        - Global constraint (non-Boolean) (examples: Max,Min,Element)
-        """
-        # XXX literal copy from flatten_cons... (except return)
+        # Global constraint (non-Boolean) (examples: Max,Min,Element)
+
         # just recursively flatten args, which can be lists
         if all(__is_flat_var_or_list(arg) for arg in expr.args):
             return (expr, [])
         else:
             # recursively flatten all children
             flatvars, flatcons = zip(*[get_or_make_var_or_list(arg) for arg in expr.args])
 
@@ -655,23 +588,22 @@
 
         if expr.name == 'and':
             return Operator('or', [negated_normal(arg) for arg in expr.args])
         elif expr.name == 'or':
             return Operator('and', [negated_normal(arg) for arg in expr.args])
         elif expr.name == '->':
             return expr.args[0] & negated_normal(expr.args[1])
-        elif expr.name == 'xor':
-            assert (len(expr.args) == 2)
-            # not xor: must be equal to each other
-            return (expr.args[0] == expr.args[1])
-            # one could also stay in xor-space:
-            # doesn't matter which one is negated
-            #return expr.args[0] ^ negated_normal(expr.args[1])
         else:
             #raise NotImplementedError("negate_normal {}".format(expr))
             return expr == 0 # can't do better than this...
 
+    elif expr.name == 'xor':
+        # avoid circular import
+        from ..expressions.globalconstraints import Xor
+        # stay in xor space
+        # only negated last element
+        return Xor(expr.args[:-1]) ^ negated_normal(expr.args[-1])
+
     else:
         # global...
         #raise NotImplementedError("negate_normal {}".format(expr))
         return expr == 0 # can't do better than this...
-
```

### Comparing `cpmpy-0.9.8/cpmpy/transformations/get_variables.py` & `cpmpy-0.9.9/cpmpy/transformations/get_variables.py`

 * *Files identical despite different names*

### Comparing `cpmpy-0.9.8/cpmpy/transformations/linearize.py` & `cpmpy-0.9.9/cpmpy/transformations/linearize.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,23 +66,19 @@
         raise Exception("Numeric constants or numeric variables not allowed as base constraint")
 
     if cpm_expr.name == "or":
         if all(arg.is_bool() for arg in cpm_expr.args):
             return [sum(cpm_expr.args) >= 1]
         raise Exception("Numeric constants or numeric variables not allowed as base constraint")
 
-    if cpm_expr.name == "xor":
-        assert len(cpm_expr.args) == 2, "Only supports xor with 2 vars"
-        if all(arg.is_bool() for arg in cpm_expr.args):
-            return [sum(cpm_expr.args) == 1]
-        raise Exception("Numeric constants or numeric variables not allowed as base constraint")
+    if cpm_expr.name == "xor" and len(cpm_expr.args) == 2:
+        return [sum(cpm_expr.args) == 1]
 
     if cpm_expr.name == "->":
         cond, sub_expr = cpm_expr.args
-        var_cons = []
         if not cond.is_bool() or not sub_expr.is_bool():
             raise Exception(
                 f"Numeric constants or numeric variables not allowed as base constraint, cannot linearize {cpm_expr}")
         lin_comps = linearize_constraint(sub_expr)
         lin_exprs = []
         for l_expr in lin_comps:
             lhs, rhs = l_expr.args
@@ -100,15 +96,15 @@
                     new_lhs = lhs + (-1 * rhs)
                 else:
                     raise Exception(f"Unsupported expression {lhs} on right hand side of implication {l_expr}, resulting from linearization of {cpm_expr}")
                 lin_exprs += [Comparison(l_expr.name, new_lhs, 0)]
             else:
                 lin_exprs += [l_expr]
 
-        return var_cons + [cond.implies(l_expr) for l_expr in lin_exprs]
+        return [cond.implies(l_expr) for l_expr in lin_exprs]
 
     # Binary operators
     if cpm_expr.name == "<":
         # TODO: this can be optimized, see https://github.com/CPMpy/cpmpy/issues/97
         lhs, rhs = cpm_expr.args
         if lhs.name == "wsum":
             return [Operator("wsum", [lhs.args[0] + [1], lhs.args[1] + [1]]) <= rhs]
@@ -184,15 +180,15 @@
         if lhs.is_bool() and not isinstance(lhs, _BoolVarImpl) and isinstance(rhs, _BoolVarImpl):
             # BE == BV :: ~BV -> ~BE, BV -> BE
             if lhs.name in gen_constr:
                 return [cpm_expr]
             else:
                 c1 = (~rhs).implies(negated_normal(lhs))
                 c2 = rhs.implies(lhs)
-                return linearize_constraint([c1,c2])
+                return linearize_constraint(flatten_constraint([c1,c2]))
 
 
     if cpm_expr.name == "alldifferent":
         """
             More efficient implementations possible
             http://yetanothermathprogrammingconsultant.blogspot.com/2016/05/all-different-and-mixed-integer.html
             This method avoids bounds computation
```

### Comparing `cpmpy-0.9.8/cpmpy/transformations/to_cnf.py` & `cpmpy-0.9.9/cpmpy/transformations/to_cnf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ..expressions.core import Operator, Comparison
+from ..expressions.globalconstraints import GlobalConstraint
 from ..expressions.variables import _BoolVarImpl, NegBoolView
 from .flatten_model import flatten_constraint, negated_normal
 """
   Converts the logical constraints into disjuctions using the tseitin transform.
   
   Other constraints are copied verbatim so this transformation
   can also be used in non-pure CNF settings
@@ -89,23 +90,22 @@
         elif is_operator and expr.name == "and":
             # special case: top-level AND constraint,
             # flatten into toplevel conjunction
             cnf += expr.args
             continue
 
         # xor() constraints
-        elif is_operator and expr.name == "xor":
+        elif isinstance(expr, GlobalConstraint) and expr.name == "xor":
             if len(expr.args) == 2:
                 a0,a1 = expr.args
                 cnf += flat2cnf([(a0|a1), (~a0|~a1)]) # one true and one false
                 continue
             else:
-                # xor(x,y,z) = (~x&y&z) | (x&~y~z) | (x&y&~z)
-                # need to flatten and tseitin that accordingly
-                raise NotImplementedError("TODO: nary xor")
+                cnf += to_cnf(expr.decompose())
+                continue
 
         # BE != BE (same as xor)
         elif isinstance(expr, Comparison) and expr.name == "!=" and expr.args[0].is_bool():
             a0,a1 = expr.args
             # using 'implies' means it will recursively work for BE's too
             cnf += flat2cnf([a0.implies(~a1), (~a0).implies(a1)]) # one true and one false
             continue
```

### Comparing `cpmpy-0.9.8/cpmpy.egg-info/PKG-INFO` & `cpmpy-0.9.9/cpmpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpmpy
-Version: 0.9.8
+Version: 0.9.9
 Summary: A numpy-based library for modeling constraint programming problems
 Home-page: https://github.com/CPMpy/cpmpy
 Author: Tias Guns
 Author-email: tias.guns@kuleuven.be
 License: Apache 2.0
 Description: CPMpy is a Constraint Programming and Modeling library in Python, based on numpy, with direct solver access.
```

### Comparing `cpmpy-0.9.8/cpmpy.egg-info/SOURCES.txt` & `cpmpy-0.9.9/cpmpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 cpmpy/expressions/variables.py
 cpmpy/solvers/TEMPLATE.py
 cpmpy/solvers/__init__.py
 cpmpy/solvers/gurobi.py
 cpmpy/solvers/minizinc.py
 cpmpy/solvers/ortools.py
 cpmpy/solvers/pysat.py
+cpmpy/solvers/pysdd.py
 cpmpy/solvers/solver_interface.py
 cpmpy/solvers/utils.py
 cpmpy/transformations/__init__.py
+cpmpy/transformations/comparison.py
 cpmpy/transformations/flatten_model.py
 cpmpy/transformations/get_variables.py
 cpmpy/transformations/linearize.py
 cpmpy/transformations/reification.py
 cpmpy/transformations/to_cnf.py
```

### Comparing `cpmpy-0.9.8/setup.py` & `cpmpy-0.9.9/setup.py`

 * *Files identical despite different names*

