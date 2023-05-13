# Comparing `tmp/komm-0.7.1.tar.gz` & `tmp/komm-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/komm-0.7.1.tar", last modified: Sun May 24 01:58:25 2020, max compression
+gzip compressed data, was "komm-0.7.2.tar", last modified: Sat May 13 23:26:15 2023, max compression
```

## Comparing `komm-0.7.1.tar` & `komm-0.7.2.tar`

### file list

```diff
@@ -1,27 +1,40 @@
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2020-05-24 01:58:25.737515 komm-0.7.1/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1445 2020-05-24 01:58:25.737515 komm-0.7.1/PKG-INFO
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1780 2020-05-09 00:45:31.000000 komm-0.7.1/README.rst
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2020-05-24 01:58:25.737515 komm-0.7.1/komm/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      662 2020-05-23 23:21:38.000000 komm-0.7.1/komm/__init__.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    32293 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_algebra.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      189 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_aux.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14962 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_channels.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    67769 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_error_control_block.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      123 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_error_control_checksum.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    20408 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_error_control_convolutional.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    18002 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_finite_state_machine.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    30592 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_modulation.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14863 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_pulses.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     8263 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_quantization.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19724 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_sequences.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    18966 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_source_coding.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2193 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_sources.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     5364 2020-05-09 00:45:31.000000 komm-0.7.1/komm/_util.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2020-05-24 01:58:25.737515 komm-0.7.1/komm.egg-info/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1445 2020-05-24 01:58:25.000000 komm-0.7.1/komm.egg-info/PKG-INFO
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      482 2020-05-24 01:58:25.000000 komm-0.7.1/komm.egg-info/SOURCES.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        1 2020-05-24 01:58:25.000000 komm-0.7.1/komm.egg-info/dependency_links.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       12 2020-05-24 01:58:25.000000 komm-0.7.1/komm.egg-info/requires.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        5 2020-05-24 01:58:25.000000 komm-0.7.1/komm.egg-info/top_level.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       38 2020-05-24 01:58:25.737515 komm-0.7.1/setup.cfg
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1623 2020-05-24 01:11:04.000000 komm-0.7.1/setup.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-13 23:26:15.274428 komm-0.7.2/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    35147 2023-05-13 23:05:18.000000 komm-0.7.2/LICENSE
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1372 2023-05-13 23:26:15.271095 komm-0.7.2/PKG-INFO
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1757 2023-05-13 23:19:40.000000 komm-0.7.2/README.rst
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-13 23:26:15.267762 komm-0.7.2/komm/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      620 2023-05-13 23:18:38.000000 komm-0.7.2/komm/__init__.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    32335 2023-05-13 23:09:56.000000 komm-0.7.2/komm/_algebra.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      189 2023-05-13 23:05:18.000000 komm-0.7.2/komm/_aux.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14967 2023-05-13 23:11:52.000000 komm-0.7.2/komm/_channels.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    67646 2023-05-13 23:12:00.000000 komm-0.7.2/komm/_error_control_block.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      123 2023-05-13 23:05:18.000000 komm-0.7.2/komm/_error_control_checksum.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    20369 2023-05-13 23:09:56.000000 komm-0.7.2/komm/_error_control_convolutional.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    18086 2023-05-13 23:08:37.000000 komm-0.7.2/komm/_finite_state_machine.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    30566 2023-05-13 23:11:52.000000 komm-0.7.2/komm/_modulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14874 2023-05-13 23:08:37.000000 komm-0.7.2/komm/_pulses.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     8251 2023-05-13 23:08:37.000000 komm-0.7.2/komm/_quantization.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19729 2023-05-13 23:08:28.000000 komm-0.7.2/komm/_sequences.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19050 2023-05-13 23:05:18.000000 komm-0.7.2/komm/_source_coding.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2190 2023-05-13 23:08:37.000000 komm-0.7.2/komm/_sources.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     5404 2023-05-13 23:13:14.000000 komm-0.7.2/komm/_util.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-13 23:26:15.271095 komm-0.7.2/komm.egg-info/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1372 2023-05-13 23:26:15.000000 komm-0.7.2/komm.egg-info/PKG-INFO
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      791 2023-05-13 23:26:15.000000 komm-0.7.2/komm.egg-info/SOURCES.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        1 2023-05-13 23:26:15.000000 komm-0.7.2/komm.egg-info/dependency_links.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       12 2023-05-13 23:26:15.000000 komm-0.7.2/komm.egg-info/requires.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        5 2023-05-13 23:26:15.000000 komm-0.7.2/komm.egg-info/top_level.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       38 2023-05-13 23:26:15.274428 komm-0.7.2/setup.cfg
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1623 2023-05-13 23:25:06.000000 komm-0.7.2/setup.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-13 23:26:15.271095 komm-0.7.2/tests/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7141 2023-05-13 23:05:18.000000 komm-0.7.2/tests/test_algebra.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      509 2023-05-13 23:05:18.000000 komm-0.7.2/tests/test_channels.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14875 2023-05-13 23:08:28.000000 komm-0.7.2/tests/test_error_control_block.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     8605 2023-05-13 23:08:28.000000 komm-0.7.2/tests/test_error_control_convolutional.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2661 2023-05-13 23:05:28.000000 komm-0.7.2/tests/test_finite_state_machine.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1860 2023-05-13 23:05:28.000000 komm-0.7.2/tests/test_modulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1802 2023-05-13 23:05:28.000000 komm-0.7.2/tests/test_quantization.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      976 2023-05-13 23:08:28.000000 komm-0.7.2/tests/test_sequences.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3028 2023-05-13 23:05:28.000000 komm-0.7.2/tests/test_source_coding.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      289 2023-05-13 23:08:28.000000 komm-0.7.2/tests/test_sources.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      509 2023-05-13 23:05:28.000000 komm-0.7.2/tests/test_util.py
```

### Comparing `komm-0.7.1/PKG-INFO` & `komm-0.7.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: komm
-Version: 0.7.1
+Version: 0.7.2
 Summary: An open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems.
 Home-page: https://github.com/rwnobrega/komm/
 Author: Roberto W. Nobrega
 Author-email: rwnobrega@gmail.com
 License: GPL
 Project-URL: Documentation, http://komm.readthedocs.io/
 Project-URL: Source, https://github.com/rwnobrega/komm/
-Description: 
-        **Komm** is an open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems. This project is inspired by---but is not meant to be compatible with---the MATLAB® `Communications System Toolbox™ <https://www.mathworks.com/help/comm/>`_. Other sources of inspiration include `GNU Radio <https://gnuradio.org/>`_, `CommPy <http://veeresht.info/CommPy/>`_, and `SageMath <https://www.sagemath.org/>`_. **Komm** is licensed under the `GNU General Public License v3.0 <https://www.gnu.org/licenses/gpl-3.0.en.html>`_.
-        
-        For installation instructions and source code, please check the project's `development page at GitHub <https://github.com/rwnobrega/komm>`_.
-        
-        For library reference, please check the project's `documentation page at Read the Docs <http://komm.readthedocs.io/>`_.
-        
-        This software is still under development. Contributions are very welcome!
-        
-Platform: UNKNOWN
-Requires-Python: >=3.4
+Requires-Python: >=3.8
+License-File: LICENSE
+
+
+**Komm** is an open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems. This project is inspired by---but is not meant to be compatible with---the MATLAB® `Communications System Toolbox™ <https://www.mathworks.com/help/comm/>`_. Other sources of inspiration include `GNU Radio <https://gnuradio.org/>`_, `CommPy <http://veeresht.info/CommPy/>`_, and `SageMath <https://www.sagemath.org/>`_. **Komm** is licensed under the `GNU General Public License v3.0 <https://www.gnu.org/licenses/gpl-3.0.en.html>`_.
+
+For installation instructions and source code, please check the project's `development page at GitHub <https://github.com/rwnobrega/komm>`_.
+
+For library reference, please check the project's `documentation page at Read the Docs <http://komm.readthedocs.io/>`_.
+
+This software is still under development. Contributions are very welcome!
```

### Comparing `komm-0.7.1/README.rst` & `komm-0.7.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -15,30 +15,30 @@
    :alt: Binder
 
 Welcome to **Komm**'s development page!
 
 **Komm** is an open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems. This project is inspired by---but is not meant to be compatible with---the MATLAB® `Communications System Toolbox™ <https://www.mathworks.com/help/comm/>`_. Other sources of inspiration include `GNU Radio <https://gnuradio.org/>`_, `CommPy <http://veeresht.info/CommPy/>`_, and `SageMath <https://www.sagemath.org/>`_. **Komm** is licensed under the `GNU General Public License v3.0 <https://www.gnu.org/licenses/gpl-3.0.en.html>`_.
 
 For library reference, please check the project's `documentation page at Read the Docs <http://komm.readthedocs.io/>`_.
- 
+
 This software is still under development. Contributions are very welcome!
 
 Installation
 ------------
 
-Before you start, make sure you have `Python <https://www.python.org/>`_ (version 3.4 or later), `NumPy <https://www.numpy.org/>`_, and `SciPy <https://www.scipy.org/>`_ installed.
+Before you start, make sure you have `Python <https://www.python.org/>`_ (version 3.8 or later), `NumPy <https://www.numpy.org/>`_, and `SciPy <https://www.scipy.org/>`_ installed.
 
 Using pip
 ~~~~~~~~~
 
 .. code-block:: bash
 
-   $ sudo pip3 install komm
+   $ pip install komm
 
 From source
 ~~~~~~~~~~~
 
 .. code-block:: bash
 
    $ git clone https://github.com/rwnobrega/komm
    $ cd komm/
-   $ sudo python3 setup.py install
+   $ pip install .
```

### Comparing `komm-0.7.1/komm/__init__.py` & `komm-0.7.2/komm/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 
 import inspect as _inspect
 import sys as _sys
 for _, _cls in _inspect.getmembers(_sys.modules[__name__], _inspect.isclass):
     if hasattr(_cls, '_process_docstring'):
         _cls._process_docstring()
 
-from pkg_resources import get_distribution as _get_distribution
-__version__ = _get_distribution('komm').version
+from importlib import metadata
+__version__ = metadata.version('komm')
```

### Comparing `komm-0.7.1/komm/_algebra.py` & `komm-0.7.2/komm/_algebra.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,39 +79,39 @@
         """
         return self._integer.bit_length() - 1
 
     def coefficients(self, width=None):
         """
         Returns the coefficients of the binary polynomial.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`width` : :obj:`int`, optional
             If this parameter is specified, the output will be filled with zeros on the right so that the its length will be the specified value.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`coefficients` : 1D-array of :obj:`int`
             Coefficients of the binary polynomial. The :math:`i`-th element of the array stands for the coefficient of :math:`X^i`.
 
         .. rubric:: Examples
 
         >>> poly = komm.BinaryPolynomial(0b11010)  # X^4 + X^3 + X
         >>> poly.coefficients()
         array([0, 1, 0, 1, 1])
         >>> poly.coefficients(width=8)
         array([0, 1, 0, 1, 1, 0, 0, 0])
         """
-        return np.array(_int2binlist(self._integer, width=width), dtype=np.int)
+        return np.array(_int2binlist(self._integer, width=width), dtype=int)
 
     def exponents(self):
         """
         Returns the exponents of the binary polynomial.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`exponents` : 1D-array of :obj:`int`
             Exponents of the nonzero terms of the binary polynomial. The exponents are returned in ascending order.
 
         .. rubric:: Examples
 
         >>> poly = komm.BinaryPolynomial(0b11010)  # X^4 + X^3 + X
@@ -162,20 +162,20 @@
     def __mod__(self, other):
         return self.__divmod__(other)[1]
 
     def evaluate(self, point):
         """
         Evaluates the polynomial at a given point. Uses Horner's method.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`point` : ring-like type
             Any Python object supporting the operations of addition, subtraction, and multiplication.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`result` : ring-like type
             The result of evaluating the binary polynomial at :code:`point`. It has the same type as :code:`point`.
 
         .. rubric:: Examples
 
         >>> poly = komm.BinaryPolynomial(0b11010)  # X^4 + X^3 + X
@@ -462,15 +462,15 @@
 
     @staticmethod
     def minimal_polynomial(x):
         """
         Returns the minimal polynomial of a given element. See :cite:`Lin.Costello.04` (Sec. 2.5) fore more details.
         """
         one = x.field(1)
-        monomials = [np.array([y, one], dtype=np.object) for y in x.conjugates()]
+        monomials = [np.array([y, one], dtype=object) for y in x.conjugates()]
         coefficients = functools.reduce(np.convolve, monomials)
         return BinaryPolynomial.from_coefficients(int(c) for c in coefficients)
 
     def __repr__(self):
         args = '{}'.format(self._degree)
         return '{}({})'.format(self.__class__.__name__, args)
 
@@ -540,20 +540,20 @@
         """
         return cls([0] * degree + [coefficient])
 
     def coefficients(self, width=None):
         """
         Returns the coefficients of the polynomial.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`width` : :obj:`int`, optional
             If this parameter is specified, the output will be filled with zeros on the right so that the its length will be the specified value.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`coefficients` : 1D-array of :obj:`int`
             Coefficients of the polynomial. The :math:`i`-th element of the array stands for the coefficient of :math:`X^i`.
 
         .. rubric:: Examples
 
         >>> poly = komm.RationalPolynomial(['0', '1/3', '2/3'])  # (1/3) X + (2/3) X^2
@@ -562,15 +562,15 @@
         >>> poly.coefficients(width=5)
         array([Fraction(0, 1), Fraction(1, 3), Fraction(2, 3), Fraction(0, 1),
                Fraction(0, 1)], dtype=object)
         """
         if width is None:
             coefficients = self._coefficients
         else:
-            coefficients = np.empty((width, ), dtype=np.object)
+            coefficients = np.empty((width, ), dtype=object)
             coefficients[:self._coefficients.size] = self._coefficients
             coefficients[self._coefficients.size:] = Fraction(0)
         return coefficients
 
     @property
     def degree(self):
         """
@@ -628,20 +628,20 @@
     def __mod__(self, other):
         return divmod(self, other)[1]
 
     def evaluate(self, point):
         """
         Evaluates the polynomial at a given point. Uses Horner's method.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`point` : ring-like type
             Any Python object supporting the operations of addition, subtraction, and multiplication.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`result` : ring-like type
             The result of evaluating the binary polynomial at :code:`point`. It has the same type as :code:`point`.
 
         .. rubric:: Examples
 
         >>> poly = komm.RationalPolynomial([0, 1, 0, -1, 2])  # X - X^3 + 2 X^4
@@ -873,15 +873,15 @@
 
     M_rref
 
     pivots
 
     Such that :obj:`M_rref = P @ M` (where :obj:`@` stands for matrix multiplication).
     """
-    eye = np.eye(M.shape[0], dtype=np.int)
+    eye = np.eye(M.shape[0], dtype=int)
 
     augmented_M = np.concatenate((np.copy(M), np.copy(eye)), axis=1)
     augmented_M_rref = rref(augmented_M)
 
     M_rref = augmented_M_rref[:, :M.shape[1]]
     P = augmented_M_rref[:, M.shape[1]:]
 
@@ -893,22 +893,22 @@
         j += 1
 
     return P, M_rref, np.array(pivots)
 
 
 def right_inverse(M):
     P, _, s_indices = xrref(M)
-    M_rref_ri = np.zeros(M.T.shape, dtype=np.int)
+    M_rref_ri = np.zeros(M.T.shape, dtype=int)
 
     M_rref_ri[s_indices] = np.eye(len(s_indices), M.shape[0])
     M_ri = np.dot(M_rref_ri, P) % 2
     return M_ri
 
 
 def null_matrix(M):
     (k, n) = M.shape
     _, M_rref, s_indices = xrref(M)
-    N = np.empty((n - k, n), dtype=np.int)
+    N = np.empty((n - k, n), dtype=int)
     p_indices = np.setdiff1d(np.arange(M.shape[1]), s_indices)
-    N[:, p_indices] = np.eye(n - k, dtype=np.int)
+    N[:, p_indices] = np.eye(n - k, dtype=int)
     N[:, s_indices] = M_rref[:, p_indices].T
     return N
```

### Comparing `komm-0.7.1/komm/_channels.py` & `komm-0.7.2/komm/_channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         """
         The channel transition probability matrix :math:`p_{Y \\mid X}`. This is a read-and-write property.
         """
         return self._transition_matrix
 
     @transition_matrix.setter
     def transition_matrix(self, value):
-        self._transition_matrix = np.array(value, dtype=np.float)
+        self._transition_matrix = np.array(value, dtype=float)
         self._input_cardinality, self._output_cardinality = self._transition_matrix.shape
 
     @property
     def input_cardinality(self):
         """
         The channel input cardinality :math:`|\\mathcal{X}|`. This property is read-only.
         """
@@ -164,23 +164,23 @@
 
            \\mathrm{I}(X ; Y) = \\mathrm{H}(X) - \\mathrm{H}(X \\mid Y),
 
         where :math:`\\mathrm{H}(X)` is the the entropy of :math:`X` and :math:`\\mathrm{H}(X \\mid Y)` is the conditional entropy of :math:`X` given :math:`Y`. By default, the base of the logarithm is :math:`2`, in which case the mutual information is measured in bits.
 
         References: :cite:`Cover.Thomas.06` (Ch. 2)
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`input_pmf` : 1D-array of :obj:`float`
             The probability mass function :math:`p_X` of the channel input :math:`X`. It must be a valid :term:`pmf`, that is, all of its values must be non-negative and sum up to :math:`1`.
 
         :code:`base` : :obj:`float` or :obj:`str`, optional
             The base of the logarithm to be used. It must be a positive float or the string :code:`'e'`. The default value is :code:`2.0`.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`mutual_information` : :obj:`float`
             The mutual information :math:`\\mathrm{I}(X ; Y)` between the input :math:`X` and the output :math:`Y`.
 
         .. rubric:: Examples
 
         >>> dmc = komm.DiscreteMemorylessChannel([[0.6, 0.3, 0.1], [0.7, 0.1, 0.2], [0.5, 0.05, 0.45]])
@@ -196,15 +196,15 @@
 
         .. rubric:: Examples
 
         >>> dmc = komm.DiscreteMemorylessChannel([[0.6, 0.3, 0.1], [0.7, 0.1, 0.2], [0.5, 0.05, 0.45]])
         >>> dmc.capacity()
         0.1616318609548566
         """
-        initial_guess = np.ones(self._input_cardinality, dtype=np.float) / self._input_cardinality
+        initial_guess = np.ones(self._input_cardinality, dtype=float) / self._input_cardinality
         optimal_input_pmf = self._arimoto_blahut(self._transition_matrix, initial_guess, **self._arimoto_blahut_kwargs)
         return _mutual_information(optimal_input_pmf, self._transition_matrix)
 
     def __call__(self, input_sequence):
         output_sequence = [np.random.choice(self._output_cardinality, p=self._transition_matrix[input_symbol])
                            for input_symbol in input_sequence]
         return np.array(output_sequence)
@@ -288,15 +288,15 @@
         >>> bsc = komm.BinarySymmetricChannel(0.25)
         >>> bsc.capacity()
         0.18872187554086717
         """
         return 1.0 - _entropy(np.array([self._crossover_probability, 1.0 - self._crossover_probability]))
 
     def __call__(self, input_sequence):
-        error_pattern = (np.random.rand(np.size(input_sequence)) < self._crossover_probability).astype(np.int)
+        error_pattern = (np.random.rand(np.size(input_sequence)) < self._crossover_probability).astype(int)
         return (input_sequence + error_pattern) % 2
 
     def __repr__(self):
         args = 'crossover_probability={}'.format(self._crossover_probability)
         return '{}({})'.format(self.__class__.__name__, args)
```

### Comparing `komm-0.7.1/komm/_error_control_block.py` & `komm-0.7.2/komm/_error_control_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,46 +104,46 @@
             self._init_from_parity_check_matrix(**kwargs)
         elif 'parity_submatrix' in kwargs:
             self._init_from_parity_submatrix(**kwargs)
         else:
             raise ValueError("Either specify 'generator_matrix' or 'parity_check_matrix' or 'parity_submatrix'")
 
     def _init_from_generator_matrix(self, generator_matrix):
-        self._generator_matrix = np.array(generator_matrix, dtype=np.int) % 2
+        self._generator_matrix = np.array(generator_matrix, dtype=int) % 2
         self._dimension, self._length = self._generator_matrix.shape
         self._redundancy = self._length - self._dimension
         self._is_systematic = False
         self._constructed_from = 'generator_matrix'
 
     def _init_from_parity_check_matrix(self, parity_check_matrix):
-        self._parity_check_matrix = np.array(parity_check_matrix, dtype=np.int) % 2
+        self._parity_check_matrix = np.array(parity_check_matrix, dtype=int) % 2
         self._redundancy, self._length = self._parity_check_matrix.shape
         self._dimension = self._length - self._redundancy
         self._is_systematic = False
         self._constructed_from = 'parity_check_matrix'
 
     def _init_from_parity_submatrix(self, parity_submatrix, information_set='left'):
-        self._parity_submatrix = np.array(parity_submatrix, dtype=np.int) % 2
+        self._parity_submatrix = np.array(parity_submatrix, dtype=int) % 2
         self._dimension, self._redundancy = self._parity_submatrix.shape
         self._length = self._dimension + self._redundancy
         if information_set == 'left':
             information_set = np.arange(self._dimension)
         elif information_set == 'right':
             information_set = np.arange(self._redundancy, self._length)
-        self._information_set = np.array(information_set, dtype=np.int)
+        self._information_set = np.array(information_set, dtype=int)
         if self._information_set.size != self._dimension or \
            self._information_set.min() < 0 or self._information_set.max() > self._length:
             raise ValueError("Parameter 'information_set' must be a 'k'-subset of 'range(n)'")
         self._parity_set = np.setdiff1d(np.arange(self._length), self._information_set)
-        self._generator_matrix = np.empty((self._dimension, self._length), dtype=np.int)
-        self._generator_matrix[:, self._information_set] = np.eye(self._dimension, dtype=np.int)
+        self._generator_matrix = np.empty((self._dimension, self._length), dtype=int)
+        self._generator_matrix[:, self._information_set] = np.eye(self._dimension, dtype=int)
         self._generator_matrix[:, self._parity_set] = self._parity_submatrix
-        self._parity_check_matrix = np.empty((self._redundancy, self._length), dtype=np.int)
+        self._parity_check_matrix = np.empty((self._redundancy, self._length), dtype=int)
         self._parity_check_matrix[:, self._information_set] = self._parity_submatrix.T
-        self._parity_check_matrix[:, self._parity_set] = np.eye(self._redundancy, dtype=np.int)
+        self._parity_check_matrix[:, self._parity_set] = np.eye(self._redundancy, dtype=int)
         self._is_systematic = True
         self._constructed_from = 'parity_submatrix'
 
     def __repr__(self):
         if self._constructed_from == 'generator_matrix':
             args = 'generator_matrix={}'.format(self._generator_matrix.tolist())
         elif self._constructed_from == 'parity_check_matrix':
@@ -231,15 +231,15 @@
 
     @property
     @functools.lru_cache()
     def codeword_table(self):
         """
         The codeword table of the code. This is a :math:`2^k \\times n` matrix whose rows are all the codewords. The codeword in row :math:`i` corresponds to the message whose binary representation (:term:`MSB` in the right) is :math:`i`.
         """
-        codeword_table = np.empty([2**self._dimension, self._length], dtype=np.int)
+        codeword_table = np.empty([2**self._dimension, self._length], dtype=int)
         for i in range(2**self._dimension):
             message = int2binlist(i, width=self._dimension)
             codeword_table[i] = self.encode(message)
         return codeword_table
 
     @property
     @functools.lru_cache()
@@ -254,19 +254,19 @@
 
     @property
     @functools.lru_cache()
     def coset_leader_table(self):
         """
         The coset leader table of the code. This is a :math:`2^m \\times n` matrix whose rows are all the coset leaders. The coset leader in row :math:`i` corresponds to the syndrome whose binary representation (:term:`MSB` in the right) is :math:`i`. This may be used as a :term:`LUT` for syndrome-based decoding.
         """
-        coset_leader_table = np.empty([2**self._redundancy, self._length], dtype=np.int)
+        coset_leader_table = np.empty([2**self._redundancy, self._length], dtype=int)
         taken = []
         for w in range(self._length + 1):
             for idx in itertools.combinations(range(self._length), w):
-                errorword = np.zeros(self._length, dtype=np.int)
+                errorword = np.zeros(self._length, dtype=int)
                 errorword[list(idx)] = 1
                 syndrome = np.dot(errorword, self.parity_check_matrix.T) % 2
                 syndrome_int = binlist2int(syndrome)
                 if syndrome_int not in taken:
                     coset_leader_table[syndrome_int] = np.array(errorword)
                     taken.append(syndrome_int)
                 if len(taken) == 2**self.redundancy:
@@ -289,23 +289,23 @@
     def _generator_matrix_right_inverse(self):
         return right_inverse(self.generator_matrix)
 
     def encode(self, message, method=None):
         """
         Encodes a given message to its corresponding codeword.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`message` : 1D-array of :obj:`int`
             The message to be encoded. Its length must be :math:`k`.
 
         :code:`method` : :obj:`str`, optional
             The encoding method to be used.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`codeword` : 1D-array of :obj:`int`
             The codeword corresponding to :code:`message`. Its length is equal to :math:`n`.
         """
         message = np.array(message)
 
         if message.size != self._dimension:
@@ -320,57 +320,57 @@
         return codeword
 
     def _encode_generator_matrix(self, message):
         codeword = np.dot(message, self.generator_matrix) % 2
         return codeword
 
     def _encode_systematic_generator_matrix(self, message):
-        codeword = np.empty(self._length, dtype=np.int)
+        codeword = np.empty(self._length, dtype=int)
         codeword[self._information_set] = message
         codeword[self._parity_set] = np.dot(message, self._parity_submatrix) % 2
         return codeword
 
     def _default_encoder(self):
         if self._is_systematic:
             return 'systematic_generator_matrix'
         else:
             return 'generator_matrix'
 
     def message_from_codeword(self, codeword):
         """
         Returns the message corresponding to a given codeword. In other words, applies the inverse encoding map.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`codeword` : 1D-array of :obj:`int`
             A codeword from the code. Its length must be :math:`n`.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`message` : 1D-array of :obj:`int`
             The message corresponding to :code:`codeword`. Its length is equal to :math:`k`.
         """
         if self._is_systematic:
             return codeword[self._information_set]
         else:
             return np.dot(codeword, self._generator_matrix_right_inverse) % 2
 
     def decode(self, recvword, method=None, **kwargs):
         """
         Decodes a received word to a message.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`recvword` : 1D-array of (:obj:`int` or :obj:`float`)
             The word to be decoded. If using a hard-decision decoding method, then the elements of the array must be bits (integers in :math:`\\{ 0, 1 \\}`). If using a soft-decision decoding method, then the elements of the array must be soft-bits (floats standing for log-probability ratios, in which positive values represent bit :math:`0` and negative values represent bit :math:`1`). Its length must be :math:`n`.
 
         :code:`method` : :obj:`str`, optional
             The decoding method to be used.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`message_hat` : 1D-array of :obj:`int`
             The message decoded from :code:`recvword`. Its length is equal to :math:`k`.
         """
         recvword = np.array(recvword)
 
         if recvword.size != self._length:
@@ -417,20 +417,20 @@
         syndrome = np.dot(recvword, self.parity_check_matrix.T) % 2
         syndrome_int = binlist2int(syndrome)
         errorword_hat = coset_leader_table[syndrome_int]
         codeword_hat = np.bitwise_xor(recvword, errorword_hat)
         return codeword_hat
 
     def _default_decoder(self, dtype):
-        if dtype == np.int:
+        if dtype == int:
             if self._dimension >= self._redundancy:
                 return 'syndrome_table'
             else:
                 return 'exhaustive_search_hard'
-        elif dtype == np.float:
+        elif dtype == float:
             return 'exhaustive_search_soft'
 
     @classmethod
     def _available_decoding_methods(cls):
         table = []
         for name in dir(cls):
             if name.startswith('_decode_'):
@@ -454,15 +454,15 @@
 def _extended_parity_submatrix(parity_submatrix):
     last_column = (1 + np.sum(parity_submatrix, axis=1)) % 2
     extended_parity_submatrix = np.hstack([parity_submatrix, last_column[np.newaxis].T])
     return extended_parity_submatrix
 
 
 def _hamming_parity_submatrix(m):
-    parity_submatrix = np.zeros((2**m - m - 1, m), dtype=np.int)
+    parity_submatrix = np.zeros((2**m - m - 1, m), dtype=int)
     i = 0
     for w in range(2, m + 1):
         for idx in itertools.combinations(range(m), w):
             parity_submatrix[i, list(idx)] = 1
             i += 1
     return parity_submatrix
 
@@ -628,18 +628,18 @@
     - The binary Golay code is a perfect code.
 
     .. rubric:: Examples
 
     >>> code = komm.GolayCode()
     >>> (code.length, code.dimension, code.minimum_distance)
     (23, 12, 7)
-    >>> recvword = np.zeros(23, dtype=np.int); recvword[[2, 10, 19]] = 1
+    >>> recvword = np.zeros(23, dtype=int); recvword[[2, 10, 19]] = 1
     >>> code.decode(recvword)  # Golay code can correct up to 3 errors.
     array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0])
-    >>> recvword = np.zeros(23, dtype=np.int); recvword[[2, 3, 10, 19]] = 1
+    >>> recvword = np.zeros(23, dtype=int); recvword[[2, 3, 10, 19]] = 1
     >>> code.decode(recvword)  # Golay code cannot correct more than 3 errors.
     array([0, 0, 1, 1, 0, 1, 0, 0, 0, 0, 1, 0])
 
     >>> code = komm.GolayCode(extended=True)
     >>> (code.length, code.dimension, code.minimum_distance)
     (24, 12, 8)
     """
@@ -716,17 +716,17 @@
     def __init__(self, n):
         """
         Constructor for the class. It expects the following parameter:
 
         :code:`n` : :obj:`int`
             The length :math:`n` of the code. Must be a positive integer.
         """
-        super().__init__(parity_submatrix=np.ones((1, n - 1), dtype=np.int))
+        super().__init__(parity_submatrix=np.ones((1, n - 1), dtype=int))
         self._minimum_distance = n
-        self._coset_leader_weight_distribution = np.zeros(n+1, dtype=np.int)
+        self._coset_leader_weight_distribution = np.zeros(n+1, dtype=int)
         for w in range((n + 1)//2):
             self._coset_leader_weight_distribution[w] = special.comb(n, w, exact=True)
         if n % 2 == 0:
             self._coset_leader_weight_distribution[n//2] = special.comb(n, n//2, exact=True) // 2
 
     def __repr__(self):
         args = '{}'.format(self._length)
@@ -738,15 +738,15 @@
         Majority-logic decoder. A hard-decision decoder for Repetition codes only.
         """
         majority = np.argmax(np.bincount(recvword))
         codeword_hat = majority * np.ones_like(recvword)
         return codeword_hat
 
     def _default_decoder(self, dtype):
-        if dtype == np.int:
+        if dtype == int:
             return 'majority_logic'
         else:
             return super()._default_decoder(dtype)
 
 
 class SingleParityCheckCode(BlockCode):
     """
@@ -782,17 +782,17 @@
     def __init__(self, n):
         """
         Constructor for the class. It expects the following parameter:
 
         :code:`n` : :obj:`int`
             The length :math:`n` of the code. Must be a positive integer.
         """
-        super().__init__(parity_submatrix=np.ones((1, n - 1), dtype=np.int).T)
+        super().__init__(parity_submatrix=np.ones((1, n - 1), dtype=int).T)
         self._minimum_distance = 2
-        self._codeword_weight_distribution = np.zeros(n+1, dtype=np.int)
+        self._codeword_weight_distribution = np.zeros(n+1, dtype=int)
         for w in range(0, n + 1, 2):
             self._codeword_weight_distribution[w] = special.comb(n, w, exact=True)
 
     def __repr__(self):
         args = '{}'.format(self._length)
         return '{}({})'.format(self.__class__.__name__, args)
 
@@ -801,18 +801,18 @@
         """
         Wagner decoder. A soft-decision decoder for SingleParityCheck codes only. See Costello, Forney: Channel Coding: The Road to Channel Capacity.
         """
         codeword_hat = (recvword < 0)
         if np.count_nonzero(codeword_hat) % 2 != 0:
             i = np.argmin(np.abs(recvword))
             codeword_hat[i] ^= 1
-        return codeword_hat.astype(np.int)
+        return codeword_hat.astype(int)
 
     def _default_decoder(self, dtype):
-        if dtype == np.float:
+        if dtype == float:
             return 'wagner'
         else:
             return super()._default_decoder(dtype)
 
 
 class CordaroWagnerCode(BlockCode):
     """
@@ -860,17 +860,17 @@
         self._minimum_distance = h + i
 
     def __repr__(self):
         args = '{}'.format(self._length)
         return '{}({})'.format(self.__class__.__name__, args)
 
     def _default_decoder(self, dtype):
-        if dtype == np.int:
+        if dtype == int:
             return 'exhaustive_search_hard'
-        elif dtype == np.float:
+        elif dtype == float:
             return 'exhaustive_search_soft'
 
 
 class ReedMullerCode(BlockCode):
     """
     Reed--Muller code. It is a linear block code (:obj:`BlockCode`) defined by two integers :math:`\\rho` and :math:`\\mu`, which must satisfy :math:`0 \\leq \\rho < \\mu`. See references for more details. The resulting code is denoted by :math:`\\mathrm{RM}(\\rho, \\mu)`, and has the following parameters:
 
@@ -902,15 +902,15 @@
            [0, 0, 1, 1, 0, 0, 1, 1, 0, 0, 1, 1, 0, 0, 1, 1, 0, 0, 1, 1, 0, 0, 1, 1, 0, 0, 1, 1, 0, 0, 1, 1],
            [0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 1],
            [0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1],
            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
            [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]])
     >>> code.encode([0, 0, 0, 0, 0, 1])  #doctest: +NORMALIZE_WHITESPACE
     array([1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1])
-    >>> recvword = np.ones(32, dtype=np.int); recvword[[2, 10, 15, 16, 17, 19, 29]] = 0
+    >>> recvword = np.ones(32, dtype=int); recvword[[2, 10, 15, 16, 17, 19, 29]] = 0
     >>> code.decode(recvword)
     array([0, 0, 0, 0, 0, 1])
     """
     def __init__(self, rho, mu):
         """
         Constructor for the class. It expects the following parameters:
 
@@ -970,75 +970,75 @@
                [ 8, 12],
                [ 9, 13],
                [10, 14],
                [11, 15]])
         """
         reed_partitions = []
         for ell in range(self._rho, -1, -1):
-            binary_vectors_I = np.fliplr(np.array(list(itertools.product([0, 1], repeat=ell)), dtype=np.int))
-            binary_vectors_J = np.fliplr(np.array(list(itertools.product([0, 1], repeat=self._mu - ell)), dtype=np.int))
+            binary_vectors_I = np.fliplr(np.array(list(itertools.product([0, 1], repeat=ell)), dtype=int))
+            binary_vectors_J = np.fliplr(np.array(list(itertools.product([0, 1], repeat=self._mu - ell)), dtype=int))
             for I in itertools.combinations(range(self._mu), ell):
-                I = np.array(I, dtype=np.int)
+                I = np.array(I, dtype=int)
                 E = np.setdiff1d(np.arange(self._mu), I, assume_unique=True)
                 S = np.dot(binary_vectors_I, 2**I)
                 Q = np.dot(binary_vectors_J, 2**E)
                 reed_partitions.append(S[np.newaxis] + Q[np.newaxis].T)
         return reed_partitions
 
     @staticmethod
     def _reed_muller_generator_matrix(rho, mu):
         """
         [1] Lin, Costello, 2Ed, p. 105--114. Assumes 0 <= rho < mu.
         """
-        v = np.empty((mu, 2**mu), dtype=np.int)
+        v = np.empty((mu, 2**mu), dtype=int)
         for i in range(mu):
-            block = np.hstack((np.zeros(2**(mu - i - 1), dtype=np.int), np.ones(2**(mu - i - 1), dtype=np.int)))
+            block = np.hstack((np.zeros(2**(mu - i - 1), dtype=int), np.ones(2**(mu - i - 1), dtype=int)))
             v[mu - i - 1] = np.tile(block, 2**i)
 
         G_list = []
         for ell in range(rho, 0, -1):
             for I in itertools.combinations(range(mu), ell):
                 row = functools.reduce(np.multiply, v[I, :])
                 G_list.append(row)
-        G_list.append(np.ones(2**mu, dtype=np.int))
+        G_list.append(np.ones(2**mu, dtype=int))
 
-        return np.array(G_list, dtype=np.int)
+        return np.array(G_list, dtype=int)
 
     @tag(name='Reed', input_type='hard', target='message')
     def _decode_reed(self, recvword):
         """
         Reed decoding algorithm for Reed--Muller codes. It's a majority-logic decoding algorithm. See Lin, Costello, 2Ed, p. 105--114, 439--440.
         """
-        message_hat = np.empty(self._generator_matrix.shape[0], dtype=np.int)
+        message_hat = np.empty(self._generator_matrix.shape[0], dtype=int)
         bx = np.copy(recvword)
         for idx, partition in enumerate(self.reed_partitions):
             checksums = np.count_nonzero(bx[partition], axis=1) % 2
             message_hat[idx] = np.count_nonzero(checksums) > len(checksums) // 2
             bx ^= message_hat[idx] * self._generator_matrix[idx]
         return message_hat
 
     @tag(name='Weighted Reed', input_type='soft', target='message')
     def _decode_weighted_reed(self, recvword):
         """
         Weighted Reed decoding algorithm for Reed--Muller codes. See Lin, Costello, 2Ed, p. 440-442.
         """
-        message_hat = np.empty(self._generator_matrix.shape[0], dtype=np.int)
+        message_hat = np.empty(self._generator_matrix.shape[0], dtype=int)
         bx = (recvword < 0) * 1
         for idx, partition in enumerate(self.reed_partitions):
             checksums = np.count_nonzero(bx[partition], axis=1) % 2
             min_reliability = np.min(np.abs(recvword[partition]), axis=1)
             decision_var = np.dot(1 - 2*checksums, min_reliability)
             message_hat[idx] = decision_var < 0
             bx ^= message_hat[idx] * self._generator_matrix[idx]
         return message_hat
 
     def _default_decoder(self, dtype):
-        if dtype == np.int:
+        if dtype == int:
             return 'reed'
-        elif dtype == np.float:
+        elif dtype == float:
             return 'weighted_reed'
 
 
 class CyclicCode(BlockCode):
     """
     General binary cyclic code. A cyclic code is a linear block code (:class:`BlockCode`) such that, if :math:`c` is a codeword, then every cyclic shift of :math:`c` is also a codeword. It is characterized by its *generator polynomial* :math:`g(X)`, of degree :math:`m` (the redundancy of the code), and by its *parity-check polynomial* :math:`h(X)`, of degree :math:`k` (the dimension of the code). Those polynomials are related by :math:`g(X) h(X) = X^n + 1`, where :math:`n = k + m` is the length of the code. See references for more details.
 
@@ -1175,25 +1175,25 @@
         else:
             return 'cyclic_direct'
 
     @property
     @functools.lru_cache(maxsize=None)
     def generator_matrix(self):
         n, k = self.length, self.dimension
-        generator_matrix = np.empty((k, n), dtype=np.int)
+        generator_matrix = np.empty((k, n), dtype=int)
         row = self._generator_polynomial.coefficients(width=n)
         for i in range(k):
             generator_matrix[i] = np.roll(row, i)
         return generator_matrix
 
     @property
     @functools.lru_cache(maxsize=None)
     def parity_check_matrix(self):
         n, k = self.length, self.dimension
-        parity_check_matrix = np.empty((n - k, n), dtype=np.int)
+        parity_check_matrix = np.empty((n - k, n), dtype=int)
         row = self._parity_check_polynomial.coefficients(width=n)[::-1]
         for i in range(n - k):
             parity_check_matrix[n - k - i - 1] = np.roll(row, -i)
         return parity_check_matrix
 
     @tag(name='Meggitt decoder', input_type='hard', target='codeword')
     def _decode_meggitt(self, recvword):
@@ -1210,15 +1210,15 @@
             if syndrome_polynomial in meggitt_table:
                 errorword_polynomial_hat = meggitt_table[syndrome_polynomial] // (1 << j)
                 break
             syndrome_polynomial = (syndrome_polynomial << 1) % self._generator_polynomial
         return (recvword_polynomial + errorword_polynomial_hat).coefficients(self._length)
 
     def _default_decoder(self, dtype):
-        if dtype == np.int:
+        if dtype == int:
             return 'meggitt'
         else:
             return super()._default_decoder(dtype)
 
 
 class BCHCode(CyclicCode):
     """
@@ -1310,15 +1310,15 @@
         errorword = np.bincount(error_locations, minlength=recvword.size)
         return np.bitwise_xor(recvword, errorword)
 
     def _bch_syndrome(self, recvword_polynomial):
         """
         BCH syndrome computation. See :cite:`Lin.Costello.04` (p. 205--209).
         """
-        syndrome_polynomial = np.empty(len(self._beta), dtype=np.object)
+        syndrome_polynomial = np.empty(len(self._beta), dtype=object)
         for i, (b, b_min_polynomial) in enumerate(zip(self._beta, self._beta_minimal_polynomial)):
             syndrome_polynomial[i] = (recvword_polynomial % b_min_polynomial).evaluate(b)
         return syndrome_polynomial
 
     def _find_roots(self, polynomial):
         """
         Exhaustive search.
@@ -1339,36 +1339,36 @@
     def _berlekamp_algorithm(self, syndrome_polynomial):
         """
         Berlekamp's iterative procedure for finding the error-location polynomial of a BCH code. See  :cite:`Lin.Costello.04` (p. 209--212) and :cite:`Ryan.Lin.09` (p. 114-121).
         """
         field = self._field
         t = self._packing_radius
 
-        sigma = {-1: np.array([field(1)], dtype=np.object), 0: np.array([field(1)], dtype=np.object)}
+        sigma = {-1: np.array([field(1)], dtype=object), 0: np.array([field(1)], dtype=object)}
         discrepancy = {-1: field(1), 0: syndrome_polynomial[0]}
         degree = {-1: 0, 0: 0}
 
         #TODO: This mu is not the same as the mu in __init__...
         for mu in range(2*t):
             if discrepancy[mu] == field(0):
                 degree[mu + 1] = degree[mu]
                 sigma[mu + 1] = sigma[mu]
             else:
                 rho, max_so_far = -1, -1
                 for i in range(-1, mu):
                     if discrepancy[i] != field(0) and i - degree[i] > max_so_far:
                         rho, max_so_far = i, i - degree[i]
                 degree[mu + 1] = max(degree[mu], degree[rho] + mu - rho)
-                sigma[mu + 1] = np.array([field(0)] * (degree[mu + 1] + 1), dtype=np.object)
-                first_guy = np.array([field(0)] * (degree[mu + 1] + 1), dtype=np.object)
+                sigma[mu + 1] = np.array([field(0)] * (degree[mu + 1] + 1), dtype=object)
+                first_guy = np.array([field(0)] * (degree[mu + 1] + 1), dtype=object)
                 first_guy[:degree[mu] + 1] = sigma[mu]
-                second_guy = np.array([field(0)] * (degree[mu + 1] + 1), dtype=np.object)
+                second_guy = np.array([field(0)] * (degree[mu + 1] + 1), dtype=object)
                 second_guy[mu-rho : degree[rho] + mu - rho + 1] = sigma[rho]
                 e = discrepancy[mu] / discrepancy[rho]
-                second_guy = np.array([e * x for x in second_guy], dtype=np.object)
+                second_guy = np.array([e * x for x in second_guy], dtype=object)
                 sigma[mu + 1] = first_guy + second_guy
             if mu < 2*t - 1:
                 discrepancy[mu + 1] = syndrome_polynomial[mu + 1]
                 for idx in range(1, degree[mu + 1] + 1):
                     discrepancy[mu + 1] += sigma[mu + 1][idx] * syndrome_polynomial[mu + 1 - idx]
 
         return sigma[2*t]
@@ -1377,15 +1377,15 @@
     def _decode_berlekamp(self, recvword):
         return self._bch_general_decoder(recvword,
                                          syndrome_computer=self._bch_syndrome,
                                          key_equation_solver=self._berlekamp_algorithm,
                                          root_finder=self._find_roots)
 
     def _default_decoder(self, dtype):
-        if dtype == np.int:
+        if dtype == int:
             return 'berlekamp'
         else:
             return super()._default_decoder(dtype)
 
 
 class TerminatedConvolutionalCode(BlockCode):
     """
@@ -1462,15 +1462,15 @@
 
         if mode == 'zero-termination':
             AnB_message = np.concatenate([np.dot(B, np.linalg.matrix_power(A, j)) % 2 for j in range(mu + h - 1, mu - 1, -1)], axis=0)
             AnB_tail = np.concatenate([np.dot(B, np.linalg.matrix_power(A, j)) % 2 for j in range(mu - 1, -1, -1)], axis=0)
             self._tail_projector = np.dot(AnB_message, right_inverse(AnB_tail)) % 2
         elif mode == 'tail-biting':
             try:
-                M = (np.linalg.matrix_power(A, h) + np.eye(nu, dtype=np.int)) % 2
+                M = (np.linalg.matrix_power(A, h) + np.eye(nu, dtype=int)) % 2
                 self._M_inv = right_inverse(M)
             except:
                 raise ValueError("This convolutional code does not support tail-biting for this number of blocks")
 
         cache_bit = np.array([int2binlist(y, width=n0) for y in range(2**n0)])
         self._metric_function_viterbi_hard = lambda y, z: np.count_nonzero(cache_bit[y] != z)
         self._metric_function_viterbi_soft = lambda y, z: np.dot(cache_bit[y], z)
@@ -1495,16 +1495,16 @@
         """
         return self._mode
 
     @property
     @functools.lru_cache(maxsize=None)
     def generator_matrix(self):
         k0, n0 = self._convolutional_code.num_input_bits, self._convolutional_code.num_output_bits
-        generator_matrix = np.zeros((self._dimension, self._length), dtype=np.int)
-        top_rows = np.apply_along_axis(self._encode_finite_state_machine, 1, np.eye(k0, self._dimension, dtype=np.int))
+        generator_matrix = np.zeros((self._dimension, self._length), dtype=int)
+        top_rows = np.apply_along_axis(self._encode_finite_state_machine, 1, np.eye(k0, self._dimension, dtype=int))
         for t in range(self._num_blocks):
             generator_matrix[k0*t : k0*(t + 1), :] = np.roll(top_rows, shift=n0*t, axis=1)
             if self._mode == 'direct-truncation':
                 generator_matrix[k0*t : k0*(t + 1), : n0*t] = 0
         return generator_matrix
 
     def _encode_finite_state_machine(self, message):
@@ -1591,11 +1591,11 @@
         if output_type == 'soft':
             return np.log(input_posteriors[:, 0] / input_posteriors[:, 1])
         elif output_type == 'hard':
             input_sequence_hat = np.argmax(input_posteriors, axis=1)
             return unpack(input_sequence_hat, width=k0)
 
     def _default_decoder(self, dtype):
-        if dtype == np.int:
+        if dtype == int:
             return 'viterbi_hard'
-        elif dtype == np.float:
+        elif dtype == float:
             return 'viterbi_soft'
```

### Comparing `komm-0.7.1/komm/_error_control_convolutional.py` & `komm-0.7.2/komm/_error_control_convolutional.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,33 +159,33 @@
         self._feedforward_polynomials = np.empty_like(feedforward_polynomials, dtype=BinaryPolynomial)
         for (i, j), p in np.ndenumerate(feedforward_polynomials):
             self._feedforward_polynomials[i, j] = BinaryPolynomial(p)
 
         k, n = self._feedforward_polynomials.shape
 
         if feedback_polynomials is None:
-            self._feedback_polynomials = np.array([BinaryPolynomial(0b1) for _ in range(k)], dtype=np.object)
+            self._feedback_polynomials = np.array([BinaryPolynomial(0b1) for _ in range(k)], dtype=object)
             self._constructed_from = 'no_feedback_polynomials'
         else:
-            self._feedback_polynomials = np.empty_like(feedback_polynomials, dtype=np.object)
+            self._feedback_polynomials = np.empty_like(feedback_polynomials, dtype=object)
             for i, q in np.ndenumerate(feedback_polynomials):
                 self._feedback_polynomials[i] = BinaryPolynomial(q)
             self._constructed_from = 'feedback_polynomials'
 
-        nus = np.empty(k, dtype=np.int)
+        nus = np.empty(k, dtype=int)
         for i, (ps, q) in enumerate(zip(self._feedforward_polynomials, self._feedback_polynomials)):
             nus[i] = max(np.amax([p.degree for p in ps]), q.degree)
 
         self._num_input_bits = k
         self._num_output_bits = n
         self._constraint_lengths = nus
         self._overall_constraint_length = np.sum(nus)
         self._memory_order = np.amax(nus)
 
-        self._transfer_function_matrix = np.empty((k, n), dtype=np.object)
+        self._transfer_function_matrix = np.empty((k, n), dtype=object)
         for (i, j), p in np.ndenumerate(feedforward_polynomials):
             q = self._feedback_polynomials[i]
             self._transfer_function_matrix[i, j] = BinaryPolynomialFraction(p) / BinaryPolynomialFraction(q)
 
         self._setup_finite_state_machine_direct_form()
         self._setup_space_state_representation()
 
@@ -209,17 +209,17 @@
             feedforward_taps.append(taps)
 
         feedback_taps = []
         for i in range(k):
             taps = (BinaryPolynomial(0b1) + self._feedback_polynomials[i]).exponents() + x_indices[i]
             feedback_taps.append(taps)
 
-        bits = np.empty(k + nu, dtype=np.int)
-        next_states = np.empty((2**nu, 2**k), dtype=np.int)
-        outputs = np.empty((2**nu, 2**k), dtype=np.int)
+        bits = np.empty(k + nu, dtype=int)
+        next_states = np.empty((2**nu, 2**k), dtype=int)
+        outputs = np.empty((2**nu, 2**k), dtype=int)
 
         for s, x in np.ndindex(2**nu, 2**k):
             bits[s_indices] = int2binlist(s, width=nu)
             bits[x_indices] = int2binlist(x, width=k)
             bits[x_indices] ^= [np.count_nonzero(bits[feedback_taps[i]]) % 2 for i in range(k)]
 
             next_state_bits = bits[s_indices - 1]
@@ -232,25 +232,25 @@
 
     def _setup_finite_state_machine_transposed_form(self):
         pass
 
     def _setup_space_state_representation(self):
         k, n, nu = self._num_input_bits, self._num_output_bits, self._overall_constraint_length
 
-        self._state_matrix = np.empty((nu, nu), dtype=np.int)
-        self._observation_matrix = np.empty((nu, n), dtype=np.int)
+        self._state_matrix = np.empty((nu, nu), dtype=int)
+        self._observation_matrix = np.empty((nu, n), dtype=int)
         for i in range(nu):
             s0 = 2**i
             s1 = self._finite_state_machine.next_states[s0, 0]
             y = self._finite_state_machine.outputs[s0, 0]
             self._state_matrix[i, :] = int2binlist(s1, width=nu)
             self._observation_matrix[i, :] = int2binlist(y, width=n)
 
-        self._control_matrix = np.empty((k, nu), dtype=np.int)
-        self._transition_matrix = np.empty((k, n), dtype=np.int)
+        self._control_matrix = np.empty((k, nu), dtype=int)
+        self._transition_matrix = np.empty((k, n), dtype=int)
         for i in range(k):
             x = 2**i
             s1 = self._finite_state_machine.next_states[0, x]
             y = self._finite_state_machine.outputs[0, x]
             self._control_matrix[i, :] = int2binlist(s1, width=nu)
             self._transition_matrix[i, :] = int2binlist(y, width=n)
 
@@ -389,15 +389,15 @@
 
     .. rubric:: Examples
 
     >>> convolutional_code = komm.ConvolutionalCode([[0o7, 0o5]])
     >>> convolutional_decoder = komm.ConvolutionalStreamDecoder(convolutional_code, traceback_length=10)
     >>> convolutional_decoder([1, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 1, 0, 0, 0, 1, 0, 1, 1, 1])
     array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0])
-    >>> convolutional_decoder(np.zeros(2*10, dtype=np.int))
+    >>> convolutional_decoder(np.zeros(2*10, dtype=int))
     array([1, 0, 1, 1, 1, 0, 1, 1, 0, 0])
     """
     def __init__(self, convolutional_code, traceback_length, initial_state=0, input_type='hard'):
         """
         Constructor for the class. It expects the following parameters:
 
         :code:`convolutional_code` : :class:`ConvolutionalCode`
@@ -416,15 +416,15 @@
 
         n = convolutional_code.num_output_bits
         num_states = convolutional_code.finite_state_machine.num_states
 
         self._memory = {}
         self._memory['metrics'] = np.full((num_states, traceback_length + 1), fill_value=np.inf)
         self._memory['metrics'][initial_state, -1] = 0.0
-        self._memory['paths'] = np.zeros((num_states, traceback_length + 1), dtype=np.int)
+        self._memory['paths'] = np.zeros((num_states, traceback_length + 1), dtype=int)
 
         cache_bit = np.array([int2binlist(y, width=n) for y in range(2**n)])
         self._metric_function_hard = lambda y, z: np.count_nonzero(cache_bit[y] != z)
         self._metric_function_soft = lambda y, z: np.dot(cache_bit[y], z)
 
     def __call__(self, inp):
         n, k = self._convolutional_code.num_output_bits, self._convolutional_code.num_input_bits
```

### Comparing `komm-0.7.1/komm/_finite_state_machine.py` & `komm-0.7.2/komm/_finite_state_machine.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         :code:`outputs` : 2D-array of :obj:`int`
             The matrix of outputs of the machine, of shape :math:`|\\mathcal{S}| \\times |\\mathcal{X}|`. The element in row :math:`s` and column :math:`x` should be the output of the machine (an element in :math:`\\mathcal{Y}`), given that the current state is :math:`s \\in \\mathcal{S}` and the input is :math:`x \\in \\mathcal{X}`.
 
         .. rubric:: Examples
 
         >>> fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
         """
-        self._next_states = np.array(next_states, dtype=np.int)
-        self._outputs = np.array(outputs, dtype=np.int)
+        self._next_states = np.array(next_states, dtype=int)
+        self._outputs = np.array(outputs, dtype=int)
         self._num_states, self._num_input_symbols = self._next_states.shape
         self._num_output_symbols = np.amax(self._outputs)
 
         self._input_edges = np.full((self._num_states, self._num_states), fill_value=-1)
         self._output_edges = np.full((self._num_states, self._num_states), fill_value=-1)
         for state_from in range(self._num_states):
             for x, state_to in enumerate(self._next_states[state_from, :]):
@@ -99,15 +99,15 @@
         return self._outputs
 
     @property
     def input_edges(self):
         """
         The matrix of input edges of the machine. It has shape :math:`|\\mathcal{S}| \\times |\\mathcal{S}|`. If there is an edge from :math:`s_0 \\in \\mathcal{S}` to :math:`s_1 \\in \\mathcal{S}`, then the element in row :math:`s_0` and column :math:`s_1` is the input associated with that edge (an element of :math:`\\mathcal{X}`); if there is no such edge, then the element is :math:`-1`. This property is read-only.
 
-        .. rubric:: Example
+        .. rubric:: Examples
 
         >>> fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
         >>> fsm.input_edges
         array([[ 0,  1, -1, -1],
                [-1, -1,  0,  1],
                [ 0,  1, -1, -1],
                [-1, -1,  0,  1]])
@@ -115,106 +115,106 @@
         return self._input_edges
 
     @property
     def output_edges(self):
         """
         The matrix of output edges of the machine. It has shape :math:`|\\mathcal{S}| \\times |\\mathcal{S}|`. If there is an edge from :math:`s_0 \\in \\mathcal{S}` to :math:`s_1 \\in \\mathcal{S}`, then the element in row :math:`s_0` and column :math:`s_1` is the output associated with that edge (an element of :math:`\\mathcal{Y}`); if there is no such edge, then the element is :math:`-1`. This property is read-only.
 
-        .. rubric:: Example
+        .. rubric:: Examples
 
         >>> fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
         >>> fsm.output_edges
         array([[ 0,  3, -1, -1],
                [-1, -1,  1,  2],
                [ 3,  0, -1, -1],
                [-1, -1,  2,  1]])
         """
         return self._output_edges
 
     def process(self, input_sequence, initial_state):
         """
         Returns the output sequence corresponding to a given input sequence. It assumes the machine starts at a given initial state :math:`s_\\mathrm{i}`. The input sequence and the output sequence are denoted by :math:`\\mathbf{x} = (x_0, x_1, \\ldots, x_{L-1}) \\in \\mathcal{X}^L` and :math:`\\mathbf{y} = (y_0, y_1, \\ldots, y_{L-1}) \\in \\mathcal{Y}^L`, respectively.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`input_sequence` : 1D-array of :obj:`int`
             The input sequence :math:`\\mathbf{x} \\in \\mathcal{X}^L`. It should be a 1D-array with elements in :math:`\\mathcal{X}`.
 
         :code:`initial_state` : :obj:`int`
             The initial state :math:`s_\\mathrm{i}` of the machine. Should be an integer in :math:`\\mathcal{S}`.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`output_sequence` : 1D-array of :obj:`int`
             The output sequence :math:`\\mathbf{y} \\in \\mathcal{Y}^L` corresponding to :code:`input_sequence`, assuming the machine starts at the state given by :code:`initial_state`. It is a 1D-array with elements in :math:`\\mathcal{Y}`.
 
         :code:`final_state` : :obj:`int`
             The final state :math:`s_\\mathrm{f}` of the machine. It is an integer in :math:`\\mathcal{S}`.
 
-        .. rubric:: Example
+        .. rubric:: Examples
 
         >>> fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
         >>> input_sequence, initial_state = [1, 1, 0, 1, 0], 0
         >>> output_sequence, final_state = fsm.process(input_sequence, initial_state)
         >>> output_sequence
         array([3, 2, 2, 0, 1])
         >>> final_state
         2
         """
-        output_sequence = np.empty_like(input_sequence, dtype=np.int)
+        output_sequence = np.empty_like(input_sequence, dtype=int)
         s = initial_state
         for t, x in np.ndenumerate(input_sequence):
             y = self._outputs[s, x]
             s = self._next_states[s, x]
             output_sequence[t] = y
         final_state = s
         return output_sequence, final_state
 
     def viterbi(self, observed_sequence, metric_function, initial_metrics=None):
         """
         Applies the Viterbi algorithm on a given observed sequence. The Viterbi algorithm finds the most probable input sequence :math:`\\hat{\\mathbf{x}}(s) \\in \\mathcal{X}^L` ending in state :math:`s`, for all :math:`s \\in \\mathcal{S}`, given an observed sequence :math:`\\mathbf{z} \\in \\mathcal{Z}^L`. It is assumed uniform input priors.
 
         References: :cite:`Lin.Costello.04` (Sec. 12.1).
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`observed_sequence` : 1D-array
             The observed sequence :math:`\\mathbf{z} \\in \\mathcal{Z}^L`.
 
         :code:`metric_function` : function
             The metric function :math:`\\mathcal{Y} \\times \\mathcal{Z} \\to \\mathbb{R}`.
 
         :code:`initial_metrics` : 1D-array of :obj:`float`, optional
             The initial metrics for each state. It must be a 1D-array of length :math:`|\\mathcal{S}|`. The default value is :code:`0.0` for all states.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`input_sequences_hat` : 2D-array of :obj:`int`
             The most probable input sequence :math:`\\hat{\\mathbf{x}}(s) \\in \\mathcal{X}^L` ending in state :math:`s`, for all :math:`s \\in \\mathcal{S}`. It is a 2D-array of shape :math:`L \\times |\\mathcal{S}|`, in which column :math:`s` is equal to :math:`\\hat{\\mathbf{x}}(s)`.
 
         :code:`final_metrics` : 1D-array of :obj:`float`
             The final metrics for each state. It is a 1D-array of length :math:`|\\mathcal{S}|`.
         """
         L, num_states = len(observed_sequence), self._num_states
-        choices = np.empty((L, num_states), dtype=np.int)
+        choices = np.empty((L, num_states), dtype=int)
         metrics = np.full((L + 1, num_states), fill_value=np.inf)
         if initial_metrics is None:
-            metrics[0, :] = np.zeros(num_states, dtype=np.float)
+            metrics[0, :] = np.zeros(num_states, dtype=float)
         else:
             metrics[0, :] = initial_metrics
         for t, z in enumerate(observed_sequence):
             for s0 in range(num_states):
                 for (s1, y) in zip(self._next_states[s0], self._outputs[s0]):
                     candidate_metrics = metrics[t, s0] + metric_function(y, z)
                     if candidate_metrics < metrics[t + 1, s1]:
                         metrics[t + 1, s1] = candidate_metrics
                         choices[t, s1] = s0
 
         # Backtrack
-        input_sequences_hat = np.empty((L, num_states), dtype=np.int)
+        input_sequences_hat = np.empty((L, num_states), dtype=int)
         for final_state in range(num_states):
             s1 = final_state
             for t in reversed(range(L)):
                 s0 = choices[t, s1]
                 input_sequences_hat[t, final_state] = self._input_edges[s0, s1]
                 s1 = s0
 
@@ -222,38 +222,37 @@
 
     def viterbi_streaming(self, observed_sequence, metric_function, memory):
         """
         Applies the streaming version of the Viterbi algorithm on a given observed sequence. The path memory (or traceback length) is denoted by :math:`\\tau`. It chooses the survivor with best metric and selects the information block on this path.
 
         References: :cite:`Lin.Costello.04` (Sec. 12.3).
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`observed_sequence` : 1D-array
             The observed sequence :math:`\\mathbf{z} \\in \\mathcal{Z}^L`.
 
         :code:`metric_function` : function
             The metric function :math:`\\mathcal{Y} \\times \\mathcal{Z} \\to \\mathbb{R}`.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`input_sequence_hat` : 1D-array of :obj:`int`
-            The most probable input sequence. It is a 1D-array of length :math:`L`.
+            The most probable input sequence :math:`\\hat{\\mathbf{x}} \\in \\mathcal{X}^L`
 
-        **Input and output:**
+        .. rubric:: Input and Output
 
         :code:`memory` : :obj:`dict`
-            The past metrics for each state. It must be a 2D-array of shape :math:`|\\mathcal{S}| \\times (\\tau + 1)`.
-            The initial metrics for each state. It must be a 2D-array of shape :math:`|\\mathcal{S}| \\times (\\tau + 1)`.
+            The metrics for each state. It must be a dictionary containing two keys: :code:`'paths'`, a 2D-array of :obj:`int` of shape :math:`|\\mathcal{S}| \\times (\\tau + 1)`; and :code:`'metrics'`, a 2D-array of :obj:`float` of shape :math:`|\\mathcal{S}| \\times (\\tau + 1)`.
         """
         num_states = self._num_states
-        input_sequences_hat = np.empty(len(observed_sequence), dtype=np.int)
+        input_sequences_hat = np.empty(len(observed_sequence), dtype=int)
         for t, z in enumerate(observed_sequence):
             new_metrics = np.full(num_states, fill_value=np.inf)
-            choices = np.zeros(num_states, dtype=np.int)
+            choices = np.zeros(num_states, dtype=int)
             for s0 in range(num_states):
                 for (s1, y) in zip(self._next_states[s0], self._outputs[s0]):
                     candidate_metric = memory['metrics'][s0, -1] + metric_function(y, z)
                     if candidate_metric < new_metrics[s1]:
                         new_metrics[s1] = candidate_metric
                         choices[s1] = s0
 
@@ -274,15 +273,15 @@
 
     def forward_backward(self, observed_sequence, metric_function, input_priors=None, initial_state_distribution=None, final_state_distribution=None):
         """
         Applies the forward-backward algorithm on a given observed sequence. The forward-backward algorithm computes the posterior :term:`pmf` of each input :math:`x_0, x_1, \\ldots, x_{L-1} \\in \\mathcal{X}` given an observed sequence :math:`\\mathbf{z} = (z_0, z_1, \\ldots, z_{L-1}) \\in \\mathcal{Z}^L`. The prior :term:`pmf` of each input may also be provided.
 
         References: :cite:`Lin.Costello.04` (Sec. 12.6).
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`observed_sequence` : 1D-array
             The observed sequence :math:`\\mathbf{z} \\in \\mathcal{Z}^L`.
 
         :code:`metric_function` : function
             The metric function :math:`\\mathcal{Y} \\times \\mathcal{Z} \\to \\mathbb{R}`.
 
@@ -291,15 +290,15 @@
 
         :code:`initial_state_distribution` : 1D-array of :obj:`float`, optional
             The :term:`pmf` of the initial state of the machine. It must be a 1D-array of length :math:`|\\mathcal{S}|`. The default value is uniform over all states.
 
         :code:`final_state_distribution` : 1D-array of :obj:`float`, optional
             The :term:`pmf` of the final state of the machine. It must be a 1D-array of length :math:`|\\mathcal{S}|`. The default value is uniform over all states.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`input_posteriors` : 2D-array of :obj:`float`
             The posterior :term:`pmf` of each input, given the observed sequence, of shape :math:`L \\times |\\mathcal{X}|`. The element in row :math:`t \\in [0 : L)` and column :math:`x \\in \\mathcal{X}` is :math:`p(x_t = x \\mid \\mathbf{z})`.
         """
         L, num_states, num_input_symbols = len(observed_sequence), self._num_states, self._num_input_symbols
 
         if input_priors is None:
@@ -327,16 +326,16 @@
             for s1 in range(num_states):
                 log_alpha[t + 1, s1] = special.logsumexp(log_gamma[t, :, s1] + log_alpha[t, :])
 
         for t in range(L - 1, -1, -1):
             for s0 in range(num_states):
                 log_beta[t, s0] = special.logsumexp(log_gamma[t, s0, :] + log_beta[t + 1, :])
 
-        log_input_posteriors = np.empty((L, num_input_symbols), dtype=np.float)
-        edge_labels = np.empty(num_states, dtype=np.float)
+        log_input_posteriors = np.empty((L, num_input_symbols), dtype=float)
+        edge_labels = np.empty(num_states, dtype=float)
         for t in range(L):
             for x in range(num_input_symbols):
                 for s0 in range(num_states):
                     s1 = self._next_states[s0, x]
                     edge_labels[s0] = log_alpha[t, s0] + log_gamma[t, s0, s1] + log_beta[t + 1, s1]
                 log_input_posteriors[t, x] = special.logsumexp(edge_labels)
```

### Comparing `komm-0.7.1/komm/_modulation.py` & `komm-0.7.2/komm/_modulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def __init__(self, constellation, labeling):
         self._constellation = np.array(constellation)
         self._order = self._constellation.size
         if self._order & (self._order - 1):
             raise ValueError("The length of constellation must be a power of two")
         self._bits_per_symbol = (self._order - 1).bit_length()
 
-        self._labeling = np.array(labeling, dtype=np.int)
+        self._labeling = np.array(labeling, dtype=int)
         if not np.array_equal(np.sort(self._labeling), np.arange(self._order)):
             raise ValueError("The labeling must be a permutation of [0 : order)")
         self._mapping = {symbol: tuple(int2binlist(label, width=self._bits_per_symbol)) \
                          for (symbol, label) in enumerate(self._labeling)}
         self._inverse_mapping = dict((value, key) for key, value in self._mapping.items())
 
         self._channel_snr = 1.0
@@ -97,49 +97,49 @@
         self._channel_snr = value
         self._channel_N0 = self.energy_per_symbol / self._channel_snr
 
     def bits_to_symbols(self, bits):
         """
         Converts bits to symbols using the modulation binary labeling.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`bits` : 1D-array of :obj:`int`
             The bits to be converted. It should be a 1D-array of integers in the set :math:`\\{ 0, 1 \\}`. Its length must be a multiple of :math:`m`.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`symbols` : 1D-array of :obj:`int`
             The symbols corresponding to :code:`bits`. It is a 1D-array of integers in the set :math:`[0 : M)`. Its length is equal to the length of :code:`bits` divided by :math:`m`.
         """
         m = self._bits_per_symbol
         n_symbols = len(bits) // m
         assert len(bits) == n_symbols * m
-        symbols = np.empty(n_symbols, dtype=np.int)
+        symbols = np.empty(n_symbols, dtype=int)
         for i, bit_sequence in enumerate(np.reshape(bits, newshape=(n_symbols, m))):
             symbols[i] = self._inverse_mapping[tuple(bit_sequence)]
         return symbols
 
     def symbols_to_bits(self, symbols):
         """
         Converts symbols to bits using the modulation binary labeling.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`symbols` : 1D-array of :obj:`int`
             The symbols to be converted. It should be a 1D-array of integers in the set :math:`[0 : M)`. It may be of any length.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`bits` : 1D-array of :obj:`int`
             The bits corresponding to :code:`symbols`. It is a 1D-array of integers in the set :math:`\\{ 0, 1 \\}`. Its length is equal to the length of :code:`symbols` multiplied by :math:`m`.
         """
         m = self._bits_per_symbol
         n_bits = len(symbols) * m
-        bits = np.empty(n_bits, dtype=np.int)
+        bits = np.empty(n_bits, dtype=int)
         for i, symbol in enumerate(symbols):
             bits[i*m : (i + 1)*m] = self._mapping[symbol]
         return bits
 
     def modulate(self, bits):
         """
         Modulates a sequence of bits to its corresponding constellation points.
@@ -153,25 +153,25 @@
         return np.argmin(np.absolute(mpoints - mconst), axis=0)
 
     def _soft_bit_demodulator(self, received):
         """Computes L-values of received points"""
         m = self._bits_per_symbol
 
         def pdf_received_given_bit(bit_index, bit_value):
-            bits = np.empty(m, dtype=np.int)
+            bits = np.empty(m, dtype=int)
             bits[bit_index] = bit_value
             rest_index = np.setdiff1d(np.arange(m), [bit_index])
             f = 0.0
             for b_rest in itertools.product([0, 1], repeat=m-1):
                 bits[rest_index] = b_rest
                 point = self._constellation[self._inverse_mapping[tuple(bits)]]
                 f += np.exp(-np.abs(received - point)**2 / self._channel_N0)
             return f
 
-        soft_bits = np.empty(len(received)*m, dtype=np.float)
+        soft_bits = np.empty(len(received)*m, dtype=float)
         for bit_index in range(m):
             p0 = pdf_received_given_bit(bit_index, 0)
             p1 = pdf_received_given_bit(bit_index, 1)
             soft_bits[bit_index::m] = np.log(p0 / p1)
 
         return soft_bits
 
@@ -198,15 +198,15 @@
         labeling ^= (labeling >> 1)
         return labeling
 
     @staticmethod
     def _labeling_reflected_2d(order_I, order_Q):
         labeling_I = _Modulation._labeling_reflected(order_I)
         labeling_Q = _Modulation._labeling_reflected(order_Q)
-        labeling = np.empty(order_I * order_Q, dtype=np.int)
+        labeling = np.empty(order_I * order_Q, dtype=int)
         for i, (i_Q, i_I) in enumerate(itertools.product(labeling_Q, labeling_I)):
             labeling[i] = i_I + order_I * i_Q
         return labeling
 
 
 class RealModulation(_Modulation):
     """
@@ -226,15 +226,15 @@
 
         >>> mod = komm.RealModulation(constellation=[-0.5, 0, 0.5, 2], labeling=[0, 1, 3, 2])
         >>> mod.constellation
         array([-0.5,  0. ,  0.5,  2. ])
         >>> mod.modulate([0, 0, 1, 1, 0, 0, 1, 0, 1, 0])
         array([-0.5,  0.5, -0.5,  0. ,  0. ])
         """
-        super().__init__(np.array(constellation, dtype=np.float), labeling)
+        super().__init__(np.array(constellation, dtype=float), labeling)
 
 
 class PAModulation(RealModulation):
     """
     Pulse-amplitude modulation (PAM). It is a real modulation scheme (:class:`RealModulation`) in which the points of the constellation :math:`\\mathcal{S}` are *uniformly arranged* in the real line. More precisely,
 
     .. math::
@@ -268,15 +268,15 @@
         array([-6., -2.,  2.,  6.])
         >>> pam.labeling
         array([0, 1, 3, 2])
         >>> pam.modulate([0, 0, 1, 1, 0, 0, 1, 0, 1, 0])
         array([-6.,  2., -6., -2., -2.])
 
         """
-        constellation = base_amplitude * np.arange(-order + 1, order, step=2, dtype=np.int)
+        constellation = base_amplitude * np.arange(-order + 1, order, step=2, dtype=int)
 
         if isinstance(labeling, str):
             if labeling in ['natural', 'reflected']:
                 labeling = getattr(_Modulation, '_labeling_' + labeling)(order)
             else:
                 raise ValueError("Only 'natural' or 'reflected' are supported for {}".format(self.__class__.__name__))
 
@@ -307,15 +307,15 @@
 
         >>> mod = komm.ComplexModulation(constellation=[0.0, -1, 1, 1j], labeling=[0, 1, 2, 3])
         >>> mod.constellation
         array([ 0.+0.j, -1.+0.j,  1.+0.j,  0.+1.j])
         >>> mod.modulate([0, 0, 1, 1, 0, 0, 1, 0, 1, 0])
         array([ 0.+0.j,  0.+1.j,  0.+0.j, -1.+0.j, -1.+0.j])
         """
-        super().__init__(np.array(constellation, dtype=np.complex), labeling)
+        super().__init__(np.array(constellation, dtype=complex), labeling)
 
 
 class ASKModulation(ComplexModulation):
     """
     Amplitude-shift keying (ASK) modulation. It is a complex modulation scheme (:class:`ComplexModulation`) in which the points of the constellation :math:`\\mathcal{S}` are *uniformly arranged* in a ray. More precisely,
 
     .. math::
@@ -352,15 +352,15 @@
         >>> ask.labeling
         array([0, 1, 3, 2])
         >>> ask.modulate([0, 0, 1, 1, 0, 0, 1, 0, 1, 0])
         array([0.+0.j, 4.+0.j, 0.+0.j, 2.+0.j, 2.+0.j])
         >>> ask.demodulate([(0.99+0.3j), (1.01-0.5j), (4.99+0.7j), (5.01-0.9j)])
         array([0, 0, 1, 0, 1, 1, 0, 1])
         """
-        constellation = base_amplitude * np.arange(order, dtype=np.int) * np.exp(1j*phase_offset)
+        constellation = base_amplitude * np.arange(order, dtype=int) * np.exp(1j*phase_offset)
 
         if isinstance(labeling, str):
             if labeling in ['natural', 'reflected']:
                 labeling = getattr(_Modulation, '_labeling_' + labeling)(order)
             else:
                 raise ValueError("Only 'natural' or 'reflected' are supported for {}".format(self.__class__.__name__))
 
@@ -575,16 +575,16 @@
         if isinstance(base_amplitudes, (tuple, list)):
             base_amplitude_I, base_amplitude_Q = float(base_amplitudes[0]), float(base_amplitudes[1])
             self._base_amplitudes = (base_amplitude_I, base_amplitude_Q)
         else:
             base_amplitude_I = base_amplitude_Q = float(base_amplitudes)
             self._base_amplitudes = base_amplitude_I
 
-        constellation_I = base_amplitude_I * np.arange(-order_I + 1, order_I, step=2, dtype=np.int)
-        constellation_Q = base_amplitude_Q * np.arange(-order_Q + 1, order_Q, step=2, dtype=np.int)
+        constellation_I = base_amplitude_I * np.arange(-order_I + 1, order_I, step=2, dtype=int)
+        constellation_Q = base_amplitude_Q * np.arange(-order_Q + 1, order_Q, step=2, dtype=int)
         constellation = (constellation_I + 1j*constellation_Q[np.newaxis].T).flatten() * np.exp(1j * phase_offset)
 
         if isinstance(labeling, str):
             if labeling == 'natural':
                 labeling = _Modulation._labeling_natural(order_I * order_Q)
             elif labeling == 'reflected_2d':
                 labeling = _Modulation._labeling_reflected_2d(order_I, order_Q)
@@ -600,40 +600,40 @@
     def __repr__(self):
         args = '{}, base_amplitudes={}, phase_offset={}'.format(self._orders, self._base_amplitudes, self._phase_offset)
         return '{}({})'.format(self.__class__.__name__, args)
 
 
 
 def uniform_real_hard_demodulator(received, order):
-    return np.clip(np.around((received + order - 1) / 2), 0, order - 1).astype(np.int)
+    return np.clip(np.around((received + order - 1) / 2), 0, order - 1).astype(int)
 
 
 def uniform_real_soft_bit_demodulator(received, snr):
     return -4 * snr * received
 
 
 def ask_hard_demodulator(received, order):
-    return np.clip(np.around((received.real + order - 1) / 2), 0, order - 1).astype(np.int)
+    return np.clip(np.around((received.real + order - 1) / 2), 0, order - 1).astype(int)
 
 
 def psk_hard_demodulator(received, order):
     phase_in_turns = np.angle(received) / (2 * np.pi)
-    return np.mod(np.around(phase_in_turns * order).astype(np.int), order)
+    return np.mod(np.around(phase_in_turns * order).astype(int), order)
 
 
 def bpsk_soft_bit_demodulator(received, snr):
     return 4 * snr * received.real
 
 
 def qpsk_soft_bit_demodulator_reflected(received, snr):
     received_rotated = received * np.exp(2j * np.pi / 8)
-    soft_bits = np.empty(2*received.size, dtype=np.float)
+    soft_bits = np.empty(2*received.size, dtype=float)
     soft_bits[0::2] = np.sqrt(8) * snr * received_rotated.real
     soft_bits[1::2] = np.sqrt(8) * snr * received_rotated.imag
     return soft_bits
 
 
 def rectangular_hard_demodulator(received, order):
     L = int(np.sqrt(order))
-    s_real = np.clip(np.around((received.real + L - 1) / 2), 0, L - 1).astype(np.int)
-    s_imag = np.clip(np.around((received.imag + L - 1) / 2), 0, L - 1).astype(np.int)
+    s_real = np.clip(np.around((received.real + L - 1) / 2), 0, L - 1).astype(int)
+    s_imag = np.clip(np.around((received.imag + L - 1) / 2), 0, L - 1).astype(int)
     return s_real + L * s_imag
```

### Comparing `komm-0.7.1/komm/_pulses.py` & `komm-0.7.2/komm/_pulses.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,29 +447,29 @@
         """
         return self._samples_per_symbol
 
     def __call__(self, inp):
         """
         Formats a sequence of symbols.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`inp` : 1D-array of :obj:`float`
             The input signal, containing symbols of a modulation.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`outp` : 1D-array of :obj:`float`
             The output signal, formatted.
         """
         sps = self._samples_per_symbol
         t0, t1 = self.Pulse.interval
         t = np.arange(t0, t1, step=1/sps)
         taps = (np.vectorize(self.Pulse.impulse_response))(t)
-        inp_interp = np.zeros((len(inp) - 1) * sps + 1, dtype=np.float)
+        inp_interp = np.zeros((len(inp) - 1) * sps + 1, dtype=float)
         inp_interp[::sps] = inp
         outp = np.convolve(taps, inp_interp)
         return outp
 
 
 class ReceiveFilter:
     """
```

### Comparing `komm-0.7.1/komm/_quantization.py` & `komm-0.7.2/komm/_quantization.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,22 +44,22 @@
         >>> quantizer = komm.ScalarQuantizer(levels=[-2.0, -1.0, 0.0, 1.0, 2.0], thresholds=[-1.5, -0.3, 0.8, 1.4])
         >>> x = np.linspace(-2.5, 2.5, num=11)
         >>> y = quantizer(x)
         >>> np.vstack([x, y])
         array([[-2.5, -2. , -1.5, -1. , -0.5,  0. ,  0.5,  1. ,  1.5,  2. ,  2.5],
                [-2. , -2. , -1. , -1. , -1. ,  0. ,  0. ,  1. ,  2. ,  2. ,  2. ]])
         """
-        self._levels = np.array(levels, dtype=np.float)
-        self._thresholds = np.array(thresholds, dtype=np.float)
+        self._levels = np.array(levels, dtype=float)
+        self._thresholds = np.array(thresholds, dtype=float)
         self._num_levels = self._levels.size
 
         if self._thresholds.size != self._num_levels - 1:
             raise ValueError("The length of 'thresholds' must be 'num_levels - 1'")
 
-        interleaved = np.empty(2*self._num_levels - 1, dtype=np.float)
+        interleaved = np.empty(2*self._num_levels - 1, dtype=float)
         interleaved[0::2] = self._levels
         interleaved[1::2] = self._thresholds
 
         if not np.array_equal(np.unique(interleaved), interleaved):
             raise ValueError("Invalid values for 'levels' and 'thresholds'")
 
     @property
@@ -188,15 +188,15 @@
     def choice(self):
         """
         The choice for the uniform quantizer (:code:`'unsigned'` | :code:`'mid-riser'` | :code:`'mid-tread'`).
         """
         return self._choice
 
     def __call__(self, input_signal):
-        input_signal = np.array(input_signal, dtype=np.float, ndmin=1)
+        input_signal = np.array(input_signal, dtype=float, ndmin=1)
         delta = self._quantization_step
         if self._choice in ['unsigned', 'mid-tread']:
             quantized = delta * np.floor(input_signal / delta + 0.5)
         elif self._choice == 'mid-riser':
             quantized = delta * (np.floor(input_signal / delta) + 0.5)
         output_signal = np.clip(quantized, a_min=self._levels[0], a_max=self._levels[-1])
         return output_signal
```

### Comparing `komm-0.7.1/komm/_sequences.py` & `komm-0.7.2/komm/_sequences.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,19 @@
             The binary sequence in bit format. Must be an 1D-array with elements in :math:`\\{ 0, 1 \\}`.
 
         :code:`polar_sequence` : 1D-array of :obj:`int`
             The binary sequence in polar format. Must be an 1D-array with elements in :math:`\\{ \\pm 1 \\}`.
         """
         kwargs_set = set(kwargs.keys())
         if kwargs_set == {'bit_sequence'}:
-            self._bit_sequence = np.array(kwargs['bit_sequence'], dtype=np.int)
+            self._bit_sequence = np.array(kwargs['bit_sequence'], dtype=int)
             self._polar_sequence = (-1)**self._bit_sequence
             self._constructed_from = 'bit_sequence'
         elif kwargs_set == {'polar_sequence'}:
-            self._polar_sequence = np.array(kwargs['polar_sequence'], dtype=np.int)
+            self._polar_sequence = np.array(kwargs['polar_sequence'], dtype=int)
             self._bit_sequence = 1 * (self._polar_sequence < 0)
             self._constructed_from = 'polar_sequence'
         else:
             raise ValueError("Either specify 'bit_sequence' or 'polar_sequence'")
 
         self._length = self._bit_sequence.size
 
@@ -87,15 +87,15 @@
 
         .. math::
 
             R[\\ell] = \\sum_{n \\in \\mathbb{Z}} a[n] a_{\\ell}[n],
 
         where :math:`a[n]` is the binary sequence in polar format, and :math:`a_{\\ell}[n] = a[n - \\ell]` is the sequence :math:`a[n]` shifted by :math:`\\ell` positions. The autocorrelation :math:`R[\\ell]` is even and satisfies :math:`R[\\ell] = 0` for :math:`|\\ell| \\geq L`, where :math:`L` is the length of the binary sequence.
 
-        **Parameters:**
+        .. rubric:: Parameters
 
         :code:`shifts` : 1D-array of :obj:`int`, optional.
             An 1D array containing the values of :math:`\\ell` for which the autocorrelation will be computed. The default value is :code:`range(L)`, that is, :math:`[0 : L)`.
 
         :code:`normalized` : :obj:`boolean`, optional
             If :code:`True`, returns the autocorrelation divided by :math:`L`, where :math:`L` is the length of the binary sequence, so that :math:`R[0] = 1`. The default value is :code:`False`.
         """
@@ -113,15 +113,15 @@
 
         .. math::
 
             \\tilde{R}[\\ell] = \\sum_{n \\in [0:L)} a[n] \\tilde{a}_{\\ell}[n],
 
         where :math:`a[n]` is the binary sequence in polar format, and :math:`\\tilde{a}_{\\ell}[n]` is the sequence :math:`a[n]` cyclic-shifted by :math:`\\ell` positions. The cyclic autocorrelation :math:`\\tilde{R}[\\ell]` is even and periodic with period :math:`L`, where :math:`L` is the period of the binary sequence.
 
-        **Parameters:**
+        .. rubric:: Parameters
 
         :code:`shifts` : 1D-array of :obj:`int`, optional.
             An 1D array containing the values of :math:`\\ell` for which the cyclic autocorrelation will be computed. The default value is :code:`range(L)`, that is, :math:`[0 : L)`.
 
         :code:`normalized` : :obj:`boolean`, optional
             If :code:`True`, returns the cyclic autocorrelation divided by :math:`L`, where :math:`L` is the length of the binary sequence, so that :math:`\\tilde{R}[0] = 1`. The default value is :code:`False`.
         """
@@ -424,15 +424,15 @@
     @staticmethod
     def _lfsr_sequence(feedback_polynomial, start_state_polynomial):
         taps = (feedback_polynomial + BinaryPolynomial(1)).exponents()
         start_state = start_state_polynomial.coefficients(width=feedback_polynomial.degree)
         m = taps[-1]
         L = 2**m - 1
         state = np.copy(start_state)
-        code = np.empty(L, dtype=np.int)
+        code = np.empty(L, dtype=int)
         for i in range(L):
             code[i] = state[-1]
             state[-1] = np.count_nonzero(state[taps - 1]) % 2
             state = np.roll(state, 1)
         return code
```

### Comparing `komm-0.7.1/komm/_source_coding.py` & `komm-0.7.2/komm/_source_coding.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,20 +83,20 @@
         """
         return self._dec_mapping
 
     def rate(self, pmf):
         """
         Computes the expected rate :math:`R` of the code, assuming a given :term:`pmf`. It is given in bits per source symbol.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`pmf` : 1D-array of :obj:`float`
             The (first-order) probability mass function :math:`p_X(x)` to be assumed.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`rate` : :obj:`float`
             The expected rate :math:`R` of the code.
 
         .. rubric:: Examples
 
         >>> code = komm.FixedToVariableCode([(0,), (1,0), (1,1)])
@@ -107,20 +107,20 @@
         lengths = [len(bits) for bits in self._codewords]
         return np.dot(lengths, probabilities) / self._source_block_size
 
     def encode(self, symbol_sequence):
         """
         Encodes a given sequence of symbols to its corresponding sequence of bits.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`symbol_sequence` : 1D-array of :obj:`int`
             The sequence of symbols to be encoded. Must be a 1D-array with elements in :math:`\\mathcal{X} = \\{0, 1, \\ldots, |\\mathcal{X} - 1| \\}`. Its length must be a multiple of :math:`k`.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`bit_sequence` : 1D-array of :obj:`int`
             The sequence of bits corresponding to :code:`symbol_sequence`.
 
         .. rubric:: Examples
 
         >>> code = komm.FixedToVariableCode([(0,), (1,0), (1,1)])
@@ -130,20 +130,20 @@
         symbols_reshaped = np.reshape(symbol_sequence, newshape=(-1, self._source_block_size))
         return np.concatenate([self._enc_mapping[tuple(symbols)] for symbols in symbols_reshaped])
 
     def decode(self, bit_sequence):
         """
         Decodes a given sequence of bits to its corresponding sequence of symbols.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`bit_sequence` : 1D-array of :obj:`int`
             The sequence of bits to be decoded. Must be a 1D-array with elements in :math:`\\{ 0, 1 \\}`.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`symbol_sequence` : 1D-array of :obj:`int`
             The sequence of symbols corresponding to :code:`bits`.
 
         .. rubric:: Examples
 
         >>> code = komm.FixedToVariableCode([(0,), (1,0), (1,1)])
@@ -324,20 +324,20 @@
         """
         return self._dec_mapping
 
     def rate(self, pmf):
         """
         Computes the expected rate :math:`R` of the code, assuming a given :term:`pmf`. It is given in bits per source symbol.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`pmf` : 1D-array of :obj:`float`
             The (first-order) probability mass function :math:`p_X(x)` to be assumed.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`rate` : :obj:`float`
             The expected rate :math:`R` of the code.
 
         .. rubric:: Examples
 
         >>> code = komm.VariableToFixedCode([(0,0,0), (0,0,1), (0,1), (1,)])
@@ -348,20 +348,20 @@
         lengths = [len(symbols) for symbols in self._sourcewords]
         return self._code_block_size / np.dot(lengths, probabilities)
 
     def encode(self, symbol_sequence):
         """
         Encodes a given sequence of symbols to its corresponding sequence of bits.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`symbol_sequence` : 1D-array of :obj:`int`
             The sequence of symbols to be encoded. Must be a 1D-array with elements in :math:`\\mathcal{X} = \\{0, 1, \\ldots, |\\mathcal{X} - 1| \\}`.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`bit_sequence` : 1D-array of :obj:`int`
             The sequence of bits corresponding to :code:`symbol_sequence`.
 
         .. rubric:: Examples
 
         >>> code = komm.VariableToFixedCode([(0,0,0), (0,0,1), (0,1), (1,)])
@@ -370,20 +370,20 @@
         """
         return np.array(_parse_prefix_free(symbol_sequence, self._enc_mapping))
 
     def decode(self, bit_sequence):
         """
         Decodes a given sequence of bits to its corresponding sequence of symbols.
 
-        **Input:**
+        .. rubric:: Input
 
         :code:`bit_sequence` : 1D-array of :obj:`int`
             The sequence of bits to be decoded. Must be a 1D-array with elements in :math:`\\{ 0, 1 \\}`.  Its length must be a multiple of :math:`n`.
 
-        **Output:**
+        .. rubric:: Output
 
         :code:`symbol_sequence` : 1D-array of :obj:`int`
             The sequence of symbols corresponding to :code:`bits`.
 
         .. rubric:: Examples
 
         >>> code = komm.VariableToFixedCode([(0,0,0), (0,0,1), (0,1), (1,)])
```

### Comparing `komm-0.7.1/komm/_sources.py` & `komm-0.7.2/komm/_sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         """
         The source probability mass function :math:`p_X`. This is a read-and-write property.
         """
         return self._pmf
 
     @pmf.setter
     def pmf(self, value):
-        self._pmf = np.array(value, dtype=np.float)
+        self._pmf = np.array(value, dtype=float)
         self._cardinality = self._pmf.size
 
     @property
     def cardinality(self):
         """
         The cardinality :math:`|\\mathcal{X}|` of the source alphabet. This property is read-only.
         """
```

### Comparing `komm-0.7.1/komm/_util.py` & `komm-0.7.2/komm/_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from scipy import special
 
 __all__ = ['binlist2int', 'int2binlist', 'pack', 'unpack',
            'qfunc', 'qfuncinv',  'entropy']
 
 
-# Functions beggining with underscore:
+# Functions beginning with underscore:
 # - Should not be used by the end user.
 # - Should be as fast as possible.
 # - May have assumptions on the input and on the output
 #   (e.g., may assume the input is a list, or a numpy array, etc.).
 #
 # Functions without underscore:
 # - Are available to the end user.
 # - Should work when the input is a list, a numpy array, etc.
 # - Should check the input whenever possible.
-# - Should return a numpy array (intead of a list) whenever possible.
+# - Should return a numpy array (instead of a list) whenever possible.
 
 # TODO: Rename binlist2int and int2binlist to something better.
 # TODO: Vectorize those functions (e.g., axis=1).
 
 
 def _binlist2int(list_):
     return sum(1 << i for (i, b) in enumerate(list_) if b != 0)
@@ -71,20 +71,20 @@
     """
     Computes the gaussian Q-function. It is given by
 
     .. math::
 
        \\mathrm{Q}(x) = \\frac{1}{\\sqrt{2\\pi}} \\int_x^\\infty \\mathrm{e}^{-u^2/2} \\, \\mathrm{d}u.
 
-    **Input:**
+    .. rubric:: Input
 
     :code:`x` : :obj:`float` or array of :obj:`float`
         The input to the function. May be any float or array of floats.
 
-    **Output:**
+    .. rubric:: Output
 
     :code:`y` : same as input
         The value :math:`y = \\mathrm{Q}(x)`.
 
     .. rubric:: Examples
 
     >>> komm.qfunc(0.0)
@@ -99,20 +99,20 @@
 def _qfuncinv(y):
     return np.sqrt(2) * special.erfcinv(2 * y)
 
 def qfuncinv(x):
     """
     Computes the inverse gaussian Q-function.
 
-    **Input:**
+    .. rubric:: Input
 
     :code:`y` : :obj:`float` or array of :obj:`float`
         The input to the function. Should be a float or array of floats in the real interval :math:`[0, 1]`.
 
-    **Output:**
+    .. rubric:: Output
 
     :code:`x` : same as input
         The value :math:`x = \\mathrm{Q^{-1}}(y)`.
 
     >>> komm.qfuncinv(0.5)  #doctest:+SKIP
     0.0
 
@@ -149,23 +149,23 @@
 
        \\mathrm{H}(X) = \\sum_{x \\in \\mathcal{X}} p_X(x) \\log \\frac{1}{p_X(x)},
 
     By default, the base of the logarithm is :math:`2`, in which case the entropy is measured in bits.
 
     References: :cite:`Cover.Thomas.06` (Ch. 2)
 
-    **Input:**
+    .. rubric:: Input
 
     :code:`pmf` : 1D-array of :obj:`float`
         The probability mass function :math:`p_X` of the random variable. It must be a valid :term:`pmf`, that is, all of its values must be non-negative and sum up to :math:`1`.
 
     :code:`base` : :obj:`float` or :obj:`str`, optional
         The base of the logarithm to be used. It must be a positive float or the string :code:`'e'`. The default value is :code:`2.0`.
 
-    **Output:**
+    .. rubric:: Output
 
     :code:`entropy` : :obj:`float`
         The entropy :math:`\\mathrm{H}(X)` of the random variable.
 
     .. rubric:: Examples
 
     >>> komm.entropy([1/4, 1/4, 1/4, 1/4])
@@ -175,15 +175,15 @@
     1.0
 
     >>> komm.entropy([1.0, 1.0])
     Traceback (most recent call last):
      ...
     ValueError: Invalid pmf
     """
-    pmf = np.array(pmf, dtype=np.float)
+    pmf = np.array(pmf, dtype=float)
     if not np.allclose(np.sum(pmf), 1.0) or not np.alltrue(pmf >= 0.0):
         raise ValueError("Invalid pmf")
     return _entropy(pmf, base)
 
 
 def _mutual_information(input_pmf, transition_probabilities, base=2.0):
     output_pmf = np.dot(input_pmf, transition_probabilities)
```

### Comparing `komm-0.7.1/komm.egg-info/PKG-INFO` & `komm-0.7.2/komm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: komm
-Version: 0.7.1
+Version: 0.7.2
 Summary: An open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems.
 Home-page: https://github.com/rwnobrega/komm/
 Author: Roberto W. Nobrega
 Author-email: rwnobrega@gmail.com
 License: GPL
 Project-URL: Documentation, http://komm.readthedocs.io/
 Project-URL: Source, https://github.com/rwnobrega/komm/
-Description: 
-        **Komm** is an open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems. This project is inspired by---but is not meant to be compatible with---the MATLAB® `Communications System Toolbox™ <https://www.mathworks.com/help/comm/>`_. Other sources of inspiration include `GNU Radio <https://gnuradio.org/>`_, `CommPy <http://veeresht.info/CommPy/>`_, and `SageMath <https://www.sagemath.org/>`_. **Komm** is licensed under the `GNU General Public License v3.0 <https://www.gnu.org/licenses/gpl-3.0.en.html>`_.
-        
-        For installation instructions and source code, please check the project's `development page at GitHub <https://github.com/rwnobrega/komm>`_.
-        
-        For library reference, please check the project's `documentation page at Read the Docs <http://komm.readthedocs.io/>`_.
-        
-        This software is still under development. Contributions are very welcome!
-        
-Platform: UNKNOWN
-Requires-Python: >=3.4
+Requires-Python: >=3.8
+License-File: LICENSE
+
+
+**Komm** is an open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems. This project is inspired by---but is not meant to be compatible with---the MATLAB® `Communications System Toolbox™ <https://www.mathworks.com/help/comm/>`_. Other sources of inspiration include `GNU Radio <https://gnuradio.org/>`_, `CommPy <http://veeresht.info/CommPy/>`_, and `SageMath <https://www.sagemath.org/>`_. **Komm** is licensed under the `GNU General Public License v3.0 <https://www.gnu.org/licenses/gpl-3.0.en.html>`_.
+
+For installation instructions and source code, please check the project's `development page at GitHub <https://github.com/rwnobrega/komm>`_.
+
+For library reference, please check the project's `documentation page at Read the Docs <http://komm.readthedocs.io/>`_.
+
+This software is still under development. Contributions are very welcome!
```

### Comparing `komm-0.7.1/setup.py` & `komm-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 For library reference, please check the project's `documentation page at Read the Docs <http://komm.readthedocs.io/>`_.
 
 This software is still under development. Contributions are very welcome!
 '''
 
 setup(
     name='komm',
-    version='0.7.1',
+    version='0.7.2',
     description='An open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems.',
     long_description=_long_description,
     url='https://github.com/rwnobrega/komm/',
     author='Roberto W. Nobrega',
     author_email='rwnobrega@gmail.com',
     license='GPL',
     project_urls={
         'Documentation': 'http://komm.readthedocs.io/',
         'Source': 'https://github.com/rwnobrega/komm/'},
     packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
     install_requires=['numpy', 'scipy'],
-    python_requires='>=3.4',
+    python_requires='>=3.8',
 )
```

