# Comparing `tmp/munch-2.5.1.dev12.tar.gz` & `tmp/munch-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/munch-2.5.1.dev12.tar", last modified: Mon Mar  9 16:20:41 2020, max compression
+gzip compressed data, was "munch-3.0.0.tar", last modified: Sun May 14 12:28:55 2023, max compression
```

## Comparing `munch-2.5.1.dev12.tar` & `munch-3.0.0.tar`

### file list

```diff
@@ -1,33 +1,38 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4277 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/ChangeLog
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1079 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        4 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6654 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/munch.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6654 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/munch.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/munch.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/munch.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/munch.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/munch.egg-info/pbr.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      487 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/munch.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/munch.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4400 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      410 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)      282 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/.editorconfig
--rw-rw-r--   0 travis    (2000) travis    (2000)      373 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/tox.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      191 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/.pylintrc
--rw-rw-r--   0 travis    (2000) travis    (2000)     1040 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      945 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     3624 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/CHANGELOG.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/munch/
--rw-rw-r--   0 travis    (2000) travis    (2000)      258 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/munch/python3_compat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22383 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/munch/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      718 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/tests/test_readme.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15701 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/tests/test_munch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      596 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2277 2020-03-09 16:20:13.000000 munch-2.5.1.dev12/tests/test_yaml.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      691 2020-03-09 16:20:41.000000 munch-2.5.1.dev12/AUTHORS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:55.100046 munch-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-14 12:28:32.000000 munch-3.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:55.096045 munch-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:55.096045 munch-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-14 12:28:32.000000 munch-3.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-14 12:28:32.000000 munch-3.0.0/.github/workflows/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-14 12:28:32.000000 munch-3.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-14 12:28:32.000000 munch-3.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-14 12:28:32.000000 munch-3.0.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 12:28:55.000000 munch-3.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-14 12:28:32.000000 munch-3.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-14 12:28:55.000000 munch-3.0.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-14 12:28:32.000000 munch-3.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 12:28:32.000000 munch-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-14 12:28:32.000000 munch-3.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-14 12:28:55.100046 munch-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-14 12:28:32.000000 munch-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:55.096045 munch-3.0.0/munch/
+-rw-r--r--   0 runner    (1001) docker     (123)    22544 2023-05-14 12:28:32.000000 munch-3.0.0/munch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-14 12:28:32.000000 munch-3.0.0/munch/python3_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:55.100046 munch-3.0.0/munch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 12:28:32.000000 munch-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-14 12:28:55.100046 munch-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-14 12:28:32.000000 munch-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:55.100046 munch-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:32.000000 munch-3.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-14 12:28:32.000000 munch-3.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16017 2023-05-14 12:28:32.000000 munch-3.0.0/tests/test_munch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-14 12:28:32.000000 munch-3.0.0/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-14 12:28:32.000000 munch-3.0.0/tests/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-14 12:28:32.000000 munch-3.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `munch-2.5.1.dev12/LICENSE.txt` & `munch-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `munch-2.5.1.dev12/README.md` & `munch-3.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 munch is a fork of David Schoonover's **Bunch** package, providing similar functionality. 99% of the work was done by him, and the fork was made mainly for lack of responsiveness for fixes and maintenance on the original code.
 
 Munch is a dictionary that supports attribute-style access, a la JavaScript:
 
 ```python
 
+>>> from munch import Munch
 >>> b = Munch()
 >>> b.hello = 'world'
 >>> b.hello
 'world'
 >>> b['hello'] += "!"
 >>> b.hello
 'world!'
@@ -106,14 +107,15 @@
 Default Values
 --------------
 
 ``DefaultMunch`` instances return a specific default value when an attribute is missing from the collection. Like ``collections.defaultdict``, the first argument is the value to use for missing keys:
 
 ```python
 
+>>> from munch import DefaultMunch
 >>> undefined = object()
 >>> b = DefaultMunch(undefined, {'hello': 'world!'})
 >>> b.hello
 'world!'
 >>> b.foo is undefined
 True
 
@@ -132,14 +134,15 @@
 
 ```
 
 Or you can use ``DefaultFactoryMunch`` to specify a factory for generating missing attributes. The first argument is the factory:
 
 ```python
 
+>>> from munch import DefaultFactoryMunch
 >>> b = DefaultFactoryMunch(list, {'hello': 'world!'})
 >>> b.hello
 'world!'
 >>> b.foo
 []
 >>> b.bar.append('hello')
 >>> b.bar
```

### Comparing `munch-2.5.1.dev12/.travis.yml` & `munch-3.0.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `munch-2.5.1.dev12/CHANGELOG.md` & `munch-3.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 Changelog
 =========
 
 Next Version
 ------------
 
+3.0.0 (2023-05-14)
+------------------
+
+* Fix munchify for tuples of lists  
+* Require Python >=3.6 and upgrade syntax - thanks @EwoutH
+* Update __init__.py  to work with non standard version - thanks @mboisson
+* Allow importing even when VERSION read fails - thanks @mdornseif and @dangillet
+* Add imports to README  
+* replace pkg_resources with importlib.metadata - thanks @dhellmann  
+* Added RecursiveMunch object - thanks @GuillaumeRochette
+
 2.5.0 (2019-10-30)
 ------------------
 
 * Support ``fromJSON`` classmethod for all Munch subclasses (PR [#55](https://github.com/Infinidat/munch/pull/55))
 * Fix return value of DefaultMunch and DefaultFactoryMunch's get method (fixes [#53](https://github.com/Infinidat/munch/issues/53))
 * Support ``fromYAML`` classmethod for all Munch subclasses (PR [#52](https://github.com/Infinidat/munch/pull/52) fixes [#34](https://github.com/Infinidat/munch/issues/34)
```

### Comparing `munch-2.5.1.dev12/munch/__init__.py` & `munch-3.0.0/munch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,20 +17,33 @@
 
         __all__ = ('Munch', 'munchify','unmunchify')
 
     un/munchify provide dictionary conversion; Munches can also be
     converted via Munch.to/fromDict().
 """
 
-import pkg_resources
-
 from .python3_compat import iterkeys, iteritems, Mapping, u
 
-__version__ = pkg_resources.get_distribution('munch').version
-VERSION = tuple(map(int, __version__.split('.')[:3]))
+try:
+    # For python 3.8 and later
+    import importlib.metadata as importlib_metadata
+except ImportError:
+    # For everyone else
+    import importlib_metadata
+try:
+    __version__ = importlib_metadata.version(__name__)
+except importlib_metadata.PackageNotFoundError:
+    # package is not installed
+    __version__ = "0.0.0"
+
+
+try:
+    VERSION = tuple(map(int, __version__.split('+')[0].split('.')[:3]))
+except ValueError:
+    VERSION = (0, 0, 0)
 
 __all__ = ('Munch', 'munchify', 'DefaultMunch', 'DefaultFactoryMunch', 'RecursiveMunch', 'unmunchify')
 
 
 
 class Munch(dict):
     """ A dictionary that provides attribute-style access.
@@ -185,15 +198,15 @@
             >>> print (repr(with_spaces))
             Munch({'a b': 9, 1: 2, 'c': Munch({'simple': 5})})
             >>> eval(repr(with_spaces))
             Munch({'a b': 9, 1: 2, 'c': Munch({'simple': 5})})
 
             (*) Invertible so long as collection contents are each repr-invertible.
         """
-        return '{0}({1})'.format(self.__class__.__name__, dict.__repr__(self))
+        return f'{self.__class__.__name__}({dict.__repr__(self)})'
 
     def __dir__(self):
         return list(iterkeys(self))
 
     def __getstate__(self):
         """ Implement a serializable interface used for pickling.
 
@@ -254,15 +267,15 @@
 class AutoMunch(Munch):
     def __setattr__(self, k, v):
         """ Works the same as Munch.__setattr__ but if you supply
             a dictionary as value it will convert it to another Munch.
         """
         if isinstance(v, Mapping) and not isinstance(v, (AutoMunch, Munch)):
             v = munchify(v, AutoMunch)
-        super(AutoMunch, self).__setattr__(k, v)
+        super().__setattr__(k, v)
 
 
 class DefaultMunch(Munch):
     """
     A Munch that returns a user-specified value for missing keys.
     """
 
@@ -273,34 +286,34 @@
         """
         # Mimic collections.defaultdict constructor
         if args:
             default = args[0]
             args = args[1:]
         else:
             default = None
-        super(DefaultMunch, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.__default__ = default
 
     def __getattr__(self, k):
         """ Gets key if it exists, otherwise returns the default value."""
         try:
-            return super(DefaultMunch, self).__getattr__(k)
+            return super().__getattr__(k)
         except AttributeError:
             return self.__default__
 
     def __setattr__(self, k, v):
         if k == '__default__':
             object.__setattr__(self, k, v)
         else:
-            super(DefaultMunch, self).__setattr__(k, v)
+            super().__setattr__(k, v)
 
     def __getitem__(self, k):
         """ Gets key if it exists, otherwise returns the default value."""
         try:
-            return super(DefaultMunch, self).__getitem__(k)
+            return super().__getitem__(k)
         except KeyError:
             return self.__default__
 
     def __getstate__(self):
         """ Implement a serializable interface used for pickling.
 
         See https://docs.python.org/3.6/library/pickle.html.
@@ -322,16 +335,15 @@
         # pylint: disable=arguments-differ
         return munchify(d, factory=lambda d_: cls(default, d_))
 
     def copy(self):
         return type(self).fromDict(self, default=self.__default__)
 
     def __repr__(self):
-        return '{0}({1!r}, {2})'.format(
-            type(self).__name__, self.__undefined__, dict.__repr__(self))
+        return f'{type(self).__name__}({self.__undefined__!r}, {dict.__repr__(self)})'
 
 
 class DefaultFactoryMunch(Munch):
     """ A Munch that calls a user-specified function to generate values for
         missing keys like collections.defaultdict.
 
         >>> b = DefaultFactoryMunch(list, {'hello': 'world!'})
@@ -341,35 +353,34 @@
         []
         >>> b.bar.append('hello')
         >>> b.bar
         ['hello']
     """
 
     def __init__(self, default_factory, *args, **kwargs):
-        super(DefaultFactoryMunch, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.default_factory = default_factory
 
     @classmethod
     def fromDict(cls, d, default_factory):
         # pylint: disable=arguments-differ
         return munchify(d, factory=lambda d_: cls(default_factory, d_))
 
     def copy(self):
         return type(self).fromDict(self, default_factory=self.default_factory)
 
     def __repr__(self):
         factory = self.default_factory.__name__
-        return '{0}({1}, {2})'.format(
-            type(self).__name__, factory, dict.__repr__(self))
+        return f'{type(self).__name__}({factory}, {dict.__repr__(self)})'
 
     def __setattr__(self, k, v):
         if k == 'default_factory':
             object.__setattr__(self, k, v)
         else:
-            super(DefaultFactoryMunch, self).__setattr__(k, v)
+            super().__setattr__(k, v)
 
     def __missing__(self, k):
         self[k] = self.default_factory()
         return self[k]
 
 
 class RecursiveMunch(DefaultFactoryMunch):
@@ -386,15 +397,15 @@
         RecursiveMunch(RecursiveMunch, {'okay': 'hello'})
         >>> b
         RecursiveMunch(RecursiveMunch, {'hello': 'world!', 'foo': RecursiveMunch(RecursiveMunch, {}),
         'bar': RecursiveMunch(RecursiveMunch, {'okay': 'hello'})})
     """
 
     def __init__(self, *args, **kwargs):
-        super(RecursiveMunch, self).__init__(RecursiveMunch, *args, **kwargs)
+        super().__init__(RecursiveMunch, *args, **kwargs)
 
     @classmethod
     def fromDict(cls, d):
         # pylint: disable=arguments-differ
         return munchify(d, factory=cls)
 
     def copy(self):
@@ -427,35 +438,40 @@
 
         nb. As dicts are not hashable, they cannot be nested in sets/frozensets.
     """
     # Munchify x, using `seen` to track object cycles
     seen = dict()
 
     def munchify_cycles(obj):
+        partial, already_seen = pre_munchify_cycles(obj)
+        if already_seen:
+            return partial
+        return post_munchify(partial, obj)
+
+    def pre_munchify_cycles(obj):
         # If we've already begun munchifying obj, just return the already-created munchified obj
         try:
-            return seen[id(obj)]
+            return seen[id(obj)], True
         except KeyError:
             pass
 
         # Otherwise, first partly munchify obj (but without descending into any lists or dicts) and save that
         seen[id(obj)] = partial = pre_munchify(obj)
-        # Then finish munchifying lists and dicts inside obj (reusing munchified obj if cycles are encountered)
-        return post_munchify(partial, obj)
+        return partial, False
 
     def pre_munchify(obj):
         # Here we return a skeleton of munchified obj, which is enough to save for later (in case
         # we need to break cycles) but it needs to filled out in post_munchify
         if isinstance(obj, Mapping):
             return factory({})
         elif isinstance(obj, list):
             return type(obj)()
         elif isinstance(obj, tuple):
             type_factory = getattr(obj, "_make", type(obj))
-            return type_factory(munchify_cycles(item) for item in obj)
+            return type_factory(pre_munchify_cycles(item)[0] for item in obj)
         else:
             return obj
 
     def post_munchify(partial, obj):
         # Here we finish munchifying the parts of obj that were deferred by pre_munchify because they
         # might be involved in a cycle
         if isinstance(obj, Mapping):
```

### Comparing `munch-2.5.1.dev12/tests/test_munch.py` & `munch-3.0.0/tests/test_munch.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,15 +516,15 @@
 
 
 def test_setitem_dunder_for_subclass():
 
     def test_class(cls, *args):
         class CustomMunch(cls):
             def __setitem__(self, k, v):
-                super(CustomMunch, self).__setitem__(k, [v] * 2)
+                super().__setitem__(k, [v] * 2)
         custom_munch = CustomMunch(*args, a='foo')
         assert custom_munch.a == ['foo', 'foo']
         regular_dict = {}
         regular_dict.update(custom_munch)
         assert regular_dict['a'] == ['foo', 'foo']
         assert repr(regular_dict) == "{'a': ['foo', 'foo']}"
         custom_munch.setdefault('bar', 'baz')
@@ -553,7 +553,21 @@
     assert isinstance(munch_obj.toJSON(), str)
     assert isinstance(munch_obj.toYAML(), str)
     munch_obj.copy()
     data = munch_obj.toDict()
     munch_cls = type(munch_obj)
     kwargs = {} if munch_cls != DefaultFactoryMunch else {"default_factory": munch_obj.default_factory}
     munch_cls.fromDict(data, **kwargs)
+
+
+def test_munchify_tuple_list():
+    data = ([{'A': 'B'}],)
+    actual = munchify(data)
+    expected = ([Munch(A='B')],)
+    assert actual == expected
+
+
+def test_munchify_tuple_list_more_elements():
+    data = (1, 2, [{'A': 'B'}])
+    actual = munchify(data)
+    expected = (1, 2, [Munch({'A': 'B'})])
+    assert actual == expected
```

### Comparing `munch-2.5.1.dev12/tests/conftest.py` & `munch-3.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `munch-2.5.1.dev12/tests/test_yaml.py` & `munch-3.0.0/tests/test_yaml.py`

 * *Files identical despite different names*

