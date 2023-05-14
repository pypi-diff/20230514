# Comparing `tmp/mathslib-2.7.0.tar.gz` & `tmp/mathslib-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathslib-2.7.0.tar", last modified: Sat Apr  8 11:49:26 2023, max compression
+gzip compressed data, was "mathslib-2.8.0.tar", last modified: Sun May 14 10:16:15 2023, max compression
```

## Comparing `mathslib-2.7.0.tar` & `mathslib-2.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 11:49:26.004665 mathslib-2.7.0/
--rw-rw-rw-   0        0        0     1211 2022-05-22 14:55:29.000000 mathslib-2.7.0/LICENSE.txt
--rw-rw-rw-   0        0        0     6460 2023-04-08 11:49:26.006177 mathslib-2.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     5543 2023-04-08 11:46:52.000000 mathslib-2.7.0/README.rst
--rw-rw-rw-   0        0        0       85 2022-05-22 15:02:53.000000 mathslib-2.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-04-08 11:49:26.017095 mathslib-2.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1560 2023-04-08 11:43:41.000000 mathslib-2.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 11:49:25.932017 mathslib-2.7.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 11:49:25.983104 mathslib-2.7.0/src/mathslib/
--rw-rw-rw-   0        0        0     1543 2022-06-10 07:50:59.000000 mathslib-2.7.0/src/mathslib/__init__.py
--rw-rw-rw-   0        0        0    15897 2023-04-08 11:42:26.000000 mathslib-2.7.0/src/mathslib/algorithms.py
--rw-rw-rw-   0        0        0     3312 2022-12-30 14:54:46.000000 mathslib-2.7.0/src/mathslib/fib.py
--rw-rw-rw-   0        0        0     9953 2022-06-10 08:18:21.000000 mathslib-2.7.0/src/mathslib/linalg.py
--rw-rw-rw-   0        0        0    19911 2022-12-31 04:14:14.000000 mathslib-2.7.0/src/mathslib/numtheory.py
--rw-rw-rw-   0        0        0    12096 2022-06-01 03:38:22.000000 mathslib-2.7.0/src/mathslib/primes.py
--rw-rw-rw-   0        0        0     4558 2023-04-08 11:41:26.000000 mathslib-2.7.0/src/mathslib/simple.py
-drwxrwxrwx   0        0        0        0 2023-04-08 11:49:26.002208 mathslib-2.7.0/src/mathslib.egg-info/
--rw-rw-rw-   0        0        0     6460 2023-04-08 11:49:25.000000 mathslib-2.7.0/src/mathslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-04-08 11:49:25.000000 mathslib-2.7.0/src/mathslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 11:49:25.000000 mathslib-2.7.0/src/mathslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-08 11:49:25.000000 mathslib-2.7.0/src/mathslib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-08 11:49:25.000000 mathslib-2.7.0/src/mathslib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 10:16:15.927414 mathslib-2.8.0/
+-rw-rw-rw-   0        0        0     1211 2022-05-22 14:55:29.000000 mathslib-2.8.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     6734 2023-05-14 10:16:15.927414 mathslib-2.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5813 2023-05-14 10:10:16.000000 mathslib-2.8.0/README.rst
+-rw-rw-rw-   0        0        0       85 2022-05-22 15:02:53.000000 mathslib-2.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-05-14 10:16:15.930702 mathslib-2.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1560 2023-05-14 10:15:05.000000 mathslib-2.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 10:16:15.830026 mathslib-2.8.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 10:16:15.880789 mathslib-2.8.0/src/mathslib/
+-rw-rw-rw-   0        0        0     1543 2022-06-10 07:50:59.000000 mathslib-2.8.0/src/mathslib/__init__.py
+-rw-rw-rw-   0        0        0    15906 2023-05-14 09:39:13.000000 mathslib-2.8.0/src/mathslib/algorithms.py
+-rw-rw-rw-   0        0        0     3314 2023-05-14 09:50:54.000000 mathslib-2.8.0/src/mathslib/fib.py
+-rw-rw-rw-   0        0        0     9961 2023-05-14 09:49:26.000000 mathslib-2.8.0/src/mathslib/linalg.py
+-rw-rw-rw-   0        0        0    19925 2023-05-14 09:50:13.000000 mathslib-2.8.0/src/mathslib/numtheory.py
+-rw-rw-rw-   0        0        0    13999 2023-05-14 10:01:31.000000 mathslib-2.8.0/src/mathslib/primes.py
+-rw-rw-rw-   0        0        0     5272 2023-05-14 09:45:48.000000 mathslib-2.8.0/src/mathslib/simple.py
+drwxrwxrwx   0        0        0        0 2023-05-14 10:16:15.924443 mathslib-2.8.0/src/mathslib.egg-info/
+-rw-rw-rw-   0        0        0     6734 2023-05-14 10:16:15.000000 mathslib-2.8.0/src/mathslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-05-14 10:16:15.000000 mathslib-2.8.0/src/mathslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 10:16:15.000000 mathslib-2.8.0/src/mathslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-14 10:16:15.000000 mathslib-2.8.0/src/mathslib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 10:16:15.000000 mathslib-2.8.0/src/mathslib.egg-info/top_level.txt
```

### Comparing `mathslib-2.7.0/LICENSE.txt` & `mathslib-2.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mathslib-2.7.0/PKG-INFO` & `mathslib-2.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathslib
-Version: 2.7.0
+Version: 2.8.0
 Summary: Library of Mathematical functions and Algorithms
 Home-page: https://github.com/igorvanloo/mathslib
 Author: Igor van Loo
 Author-email: igorvanloo@gmail.com
 Project-URL: Bug Reports, https://github.com/igorvanloo/mathslib/issues
 Project-URL: Source, https://github.com/igorvanloo/mathslib
 Keywords: numbertheory,maths,algorithms
@@ -26,15 +26,17 @@
 .. image:: https://img.shields.io/pypi/v/mathslib.svg
         :target: https://pypi.python.org/pypi/mathslib
 
 .. image:: https://readthedocs.org/projects/mathslib/badge/?version=latest
         :target: https://mathslib.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
-`mathslib`__ is a compilation of Mathematical Functions and Algorithms I have made or come across.
+`mathslib`__ is a compilation of Mathematical Functions and Algorithms. Unless credit was given all
+of the functions were written by me. Relevant articles are also linked where the implementation is complex.
+
 I have used most of these for `Project Euler`_.
  
 See my website `ivl-projecteuler.com`_ for their implementation
 
 See the full documentation `here`_
 
 Breakdown
@@ -50,57 +52,59 @@
 |                | * mobius_k_sieve(limit, k)                                 |
 |                | * count_k_free(n, k)                                       |
 |                | * ppt(limit, non_primitive)                                |
 |                | * k_smooth_numbers(max_prime, limit)                       |
 |                | * k_powerful(k, limit, count)                              |
 |                | * legendre_factorial(x)                                    |
 |                | * tonelli_shanks(a, p)                                     |
-|                | * ChineseRemainderTheorem(a1, a2, n1, n2)                  |
-|                | * Generalised_CRT(a1, a2, n1, n2)                          |
-|                | * FrobeniusNumber(\*integers)                              |
+|                | * chinese_remainder_theorem(a1, a2, n1, n2)                |
+|                | * generalised_CRT(a1, a2, n1, n2)                          |
+|                | * frobenius_number(\*integers)                             |
 +----------------+------------------------------------------------------------+
 |prime.py        | * prime_sieve(limit, block_size, segment, values)          |
 |                | * is_prime(x)                                              |
 |                | * prime_factors(x)                                         |
 |                | * primepi(x)                                               |
+|                | * primepi_sieve(x)                                         |
 |                | * sum_of_primes(x)                                         |
 |                | * fermat_primality_test(x)                                 |
-|                | * miller(n, millerrabin, numoftests)                       |
+|                | * miller_primality_test(n, millerrabin, numoftests)        |
 +----------------+------------------------------------------------------------+
-|linalg.py       | * GaussJordanElimination(matrix, augmentedpart)            |
+|linalg.py       | * gauss_jordan_elimination(matrix, augmentedpart)          |
 |                | * solve(M, b)                                              |
 |                | * inverse(matrix)                                          |
 |                | * determinant(matrix)                                      |
 |                | * matrix_addition(A, B, subtract)                          |
 |                | * identity(l, val)                                         |
 |                | * concatenate(A, B)                                        |
 |                | * argmax(alist)                                            |
 |                | * fillmatrix(size, val)                                    |
 |                | * matrix_mul(A, B)                                         |
 +----------------+------------------------------------------------------------+
 |fib.py          | * fibonacci(n)                                             |
 |                | * fib_till(limit)                                          |
-|                | * ZeckendorfRepresentation(x)                              |
+|                | * zeckendorf_representation(x)                             |
 +----------------+------------------------------------------------------------+
-|algorithms.py   | * PrimsAlgorithm(matrix)                                   |
-|                | * DijkstrasAlgorithm(graph, start_node, INFINITY)          |
-|                | * FloydWarshallAlgorithm(graph, INFINITY)                  |
-|                | * KnapSack(values, weights, n, W, no_values)               |
-|                | * KnapSackValues(values, weights, n, W, no_values)         |
-|                | * BFSSearch(g, start_node, end_node)                       |
-|                | * DFSSearch(g, start_node, end_node)                       |
-|                | * ConvexHullGiftWrapping(pts)                              |
-|                | * ConvexHullDC(pts)                                        |
+|algorithms.py   | * prims_algorithm(matrix)                                  |
+|                | * dijkstras_algorithm(graph, start_node, INFINITY)         |
+|                | * floyd_warshall_algorithm(graph, INFINITY)                |
+|                | * knap_sack(values, weights, n, W, no_values)              |
+|                | * knap_sack_values(values, weights, n, W, no_values)       |
+|                | * BFS(g, start_node, end_node)                             |
+|                | * DFS(g, start_node, end_node)                             |
+|                | * convex_hull_gift_wrapping(pts)                           |
+|                | * convex_hull_DC(pts)                                      |
 +----------------+------------------------------------------------------------+
 |simple.py       | * n_choose_r(n, r)                                         | 
-|                | * numberToBase(n, b)                                       |
-|                | * ExtendedEuclideanAlgorithm(n, b)                         |
+|                | * number_to_base(n, b)                                     |
+|                | * extended_euclidean_algorithm(n, b)                       |
 |                | * lcm(a_list)                                              |
-|                | * ModDivision(a, b, m)                                     |
-|                | * IsClockwise(a, b, c)                                     |
+|                | * mod_division(a, b, m)                                    |
+|                | * bisect(alist, goal)                                      |
+|                | * is_clockwise(a, b, c)                                    |
 +----------------+------------------------------------------------------------+
 
 .. _Project Euler: https://projecteuler.net
 .. _ivl-projecteuler.com: https://ivl-projecteuler.com
 .. _mathslib1: https://pypi.python.org/pypi/mathslib
 .. _here: https://mathslib.readthedocs.io/en/latest/index.html
 __ mathslib1_
```

### Comparing `mathslib-2.7.0/README.rst` & `mathslib-2.8.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 .. image:: https://img.shields.io/pypi/v/mathslib.svg
         :target: https://pypi.python.org/pypi/mathslib
 
 .. image:: https://readthedocs.org/projects/mathslib/badge/?version=latest
         :target: https://mathslib.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
-`mathslib`__ is a compilation of Mathematical Functions and Algorithms I have made or come across.
+`mathslib`__ is a compilation of Mathematical Functions and Algorithms. Unless credit was given all
+of the functions were written by me. Relevant articles are also linked where the implementation is complex.
+
 I have used most of these for `Project Euler`_.
  
 See my website `ivl-projecteuler.com`_ for their implementation
 
 See the full documentation `here`_
 
 Breakdown
@@ -29,57 +31,59 @@
 |                | * mobius_k_sieve(limit, k)                                 |
 |                | * count_k_free(n, k)                                       |
 |                | * ppt(limit, non_primitive)                                |
 |                | * k_smooth_numbers(max_prime, limit)                       |
 |                | * k_powerful(k, limit, count)                              |
 |                | * legendre_factorial(x)                                    |
 |                | * tonelli_shanks(a, p)                                     |
-|                | * ChineseRemainderTheorem(a1, a2, n1, n2)                  |
-|                | * Generalised_CRT(a1, a2, n1, n2)                          |
-|                | * FrobeniusNumber(\*integers)                              |
+|                | * chinese_remainder_theorem(a1, a2, n1, n2)                |
+|                | * generalised_CRT(a1, a2, n1, n2)                          |
+|                | * frobenius_number(\*integers)                             |
 +----------------+------------------------------------------------------------+
 |prime.py        | * prime_sieve(limit, block_size, segment, values)          |
 |                | * is_prime(x)                                              |
 |                | * prime_factors(x)                                         |
 |                | * primepi(x)                                               |
+|                | * primepi_sieve(x)                                         |
 |                | * sum_of_primes(x)                                         |
 |                | * fermat_primality_test(x)                                 |
-|                | * miller(n, millerrabin, numoftests)                       |
+|                | * miller_primality_test(n, millerrabin, numoftests)        |
 +----------------+------------------------------------------------------------+
-|linalg.py       | * GaussJordanElimination(matrix, augmentedpart)            |
+|linalg.py       | * gauss_jordan_elimination(matrix, augmentedpart)          |
 |                | * solve(M, b)                                              |
 |                | * inverse(matrix)                                          |
 |                | * determinant(matrix)                                      |
 |                | * matrix_addition(A, B, subtract)                          |
 |                | * identity(l, val)                                         |
 |                | * concatenate(A, B)                                        |
 |                | * argmax(alist)                                            |
 |                | * fillmatrix(size, val)                                    |
 |                | * matrix_mul(A, B)                                         |
 +----------------+------------------------------------------------------------+
 |fib.py          | * fibonacci(n)                                             |
 |                | * fib_till(limit)                                          |
-|                | * ZeckendorfRepresentation(x)                              |
+|                | * zeckendorf_representation(x)                             |
 +----------------+------------------------------------------------------------+
-|algorithms.py   | * PrimsAlgorithm(matrix)                                   |
-|                | * DijkstrasAlgorithm(graph, start_node, INFINITY)          |
-|                | * FloydWarshallAlgorithm(graph, INFINITY)                  |
-|                | * KnapSack(values, weights, n, W, no_values)               |
-|                | * KnapSackValues(values, weights, n, W, no_values)         |
-|                | * BFSSearch(g, start_node, end_node)                       |
-|                | * DFSSearch(g, start_node, end_node)                       |
-|                | * ConvexHullGiftWrapping(pts)                              |
-|                | * ConvexHullDC(pts)                                        |
+|algorithms.py   | * prims_algorithm(matrix)                                  |
+|                | * dijkstras_algorithm(graph, start_node, INFINITY)         |
+|                | * floyd_warshall_algorithm(graph, INFINITY)                |
+|                | * knap_sack(values, weights, n, W, no_values)              |
+|                | * knap_sack_values(values, weights, n, W, no_values)       |
+|                | * BFS(g, start_node, end_node)                             |
+|                | * DFS(g, start_node, end_node)                             |
+|                | * convex_hull_gift_wrapping(pts)                           |
+|                | * convex_hull_DC(pts)                                      |
 +----------------+------------------------------------------------------------+
 |simple.py       | * n_choose_r(n, r)                                         | 
-|                | * numberToBase(n, b)                                       |
-|                | * ExtendedEuclideanAlgorithm(n, b)                         |
+|                | * number_to_base(n, b)                                     |
+|                | * extended_euclidean_algorithm(n, b)                       |
 |                | * lcm(a_list)                                              |
-|                | * ModDivision(a, b, m)                                     |
-|                | * IsClockwise(a, b, c)                                     |
+|                | * mod_division(a, b, m)                                    |
+|                | * bisect(alist, goal)                                      |
+|                | * is_clockwise(a, b, c)                                    |
 +----------------+------------------------------------------------------------+
 
 .. _Project Euler: https://projecteuler.net
 .. _ivl-projecteuler.com: https://ivl-projecteuler.com
 .. _mathslib1: https://pypi.python.org/pypi/mathslib
 .. _here: https://mathslib.readthedocs.io/en/latest/index.html
 __ mathslib1_
```

### Comparing `mathslib-2.7.0/setup.py` & `mathslib-2.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (here / "README.rst").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name = "mathslib",  # Required
-    version="2.7.0",  # Required
+    version="2.8.0",  # Required
     description="Library of Mathematical functions and Algorithms",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/x-rst",  # Optional
     url="https://github.com/igorvanloo/mathslib",  # Optional
     author="Igor van Loo",  # Optional
     author_email="igorvanloo@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `mathslib-2.7.0/src/mathslib/__init__.py` & `mathslib-2.8.0/src/mathslib/__init__.py`

 * *Files identical despite different names*

### Comparing `mathslib-2.7.0/src/mathslib/algorithms.py` & `mathslib-2.8.0/src/mathslib/algorithms.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 
 '''
 Various known algorithms. They are graph theory and optimization related
 
 Author: Igor van Loo
 '''
 
-from .simple import IsClockwise
+from .simple import is_clockwise
 
-def PrimsAlgorithm(matrix):
+def prims_algorithm(matrix):
     '''
     Implementation of `Prim's algorithm <https://en.wikipedia.org/wiki/Prim%27s_algorithm>`_
     It finds a Minimum Spanning Tree (MST) for a weighted undirected graph.
         
     :param matrix: Takes a `Adjacency matrix <https://en.wikipedia.org/wiki/Adjacency_matrix>`_ as input
     
     :returns Weight: The sum of the minimum spanning tree
@@ -50,15 +50,15 @@
                   [16, 0, 0, 17, 20, 0, 0], 
                   [12, 0, 0, 28, 0, 31, 0], 
                   [21, 17, 28, 0, 18, 19, 23], 
                   [0, 20, 0, 18, 0, 0, 11], 
                   [0, 0, 31, 19, 0, 0, 27], 
                   [0, 0, 0, 23, 11, 27, 0]]
         
-        print(PrimsAlgorithm(matrix)) #(93, 
+        print(prims_algorithm(matrix)) #(93, 
                                       #[[0, 16, 12, 0, 0, 0, 0],
                                       #[16, 0, 0, 17, 0, 0, 0],
                                       #[12, 0, 0, 0, 0, 0, 0],
                                       #[0, 17, 0, 0, 18, 19, 0],
                                       #[0, 0, 0, 18, 0, 0, 11],
                                       #[0, 0, 0, 19, 0, 0, 0],
                                       #[0, 0, 0, 0, 11, 0, 0]])
@@ -74,15 +74,15 @@
         mask[a][b] = matrix[a][b]
         mask[b][a] = matrix[a][b]
         Weight += Minimum_edge
         if len(Tree) == dimension:
             break
     return Weight, mask
 
-def DijkstrasAlgorithm(graph, start_node = 0, INFINITY = 10**10):
+def dijkstras_algorithm(graph, start_node = 0, INFINITY = 10**10):
     '''
     Implementation of `Dijkstra's algorithm <https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm>`_ 
     It finds the the shortest paths between nodes in a graph
 
     :param graph: Takes an adjacency list as input
     :param start_node: Optional tuple, default is node 0.
     :param INFINITY: Optional integer, default is 10^10. It is used to set the "Infinty" value
@@ -97,15 +97,15 @@
              [[0, 7], [2, 10], [3, 15]],
              [[0, 9], [1, 10], [3, 11], [5, 2]],
              [[1, 15], [2, 11], [4, 6]],
              [[3, 6], [5, 9]],
              [[0, 14], [2, 2], [4, 9]]
             ]
         
-        print(DijkstrasAlgorithm(g)) #[0, 7, 9, 20, 20, 11]
+        print(dijkstras_algorithm(g)) #[0, 7, 9, 20, 20, 11]
     
     .. note::
         
         A quick comment on this adjacency list. The way it works is for example g[i] contains all the nodes
         node i is connected to. For example, using the above graph g[0] = [[1, 7], [2, 9], [5, 14]] means node 0 is connected to nodes
         1, 2, and 5 and the weight between the edges are 7, 9, and 14 respectively
         
@@ -128,15 +128,15 @@
                 if D[i] != INFINITY:
                     flag = False
                     break
         if flag:
             break
     return D
 
-def FloydWarshallAlgorithm(graph, INFINITY = 10**10):
+def floyd_warshall_algorithm(graph, INFINITY = 10**10):
     '''
     Implementation of the `Floyd-Warshall algorithm <https://en.wikipedia.org/wiki/Floyd%E2%80%93Warshall_algorithm>`_ 
     It finds the the shortest paths between every node in the graph to every node in the graph
 
     :param graph: Takes an adjacency list as input
     :param INFINITY: Optional integer, default is 10^10. It is used to set the "Infinty" value
 
@@ -150,15 +150,15 @@
              [[0, 7], [2, 10], [3, 15]],
              [[0, 9], [1, 10], [3, 11], [5, 2]],
              [[1, 15], [2, 11], [4, 6]],
              [[3, 6], [5, 9]],
              [[0, 14], [2, 2], [4, 9]]
             ]
         
-        print(FloydWarshallAlgorithm(g)) #[[0, 7, 9, 20, 20, 11],
+        print(floyd_warshall_algorithm(g)) #[[0, 7, 9, 20, 20, 11],
                                           # [7, 0, 10, 15, 21, 12],
                                           # [9, 10, 0, 11, 11, 2],
                                           # [20, 15, 11, 0, 6, 13],
                                           # [20, 21, 11, 6, 0, 9],
                                           # [11, 12, 2, 13, 9, 0]]
     .. note::
         
@@ -173,15 +173,15 @@
             D[0][v][e] = w            
     for k in range(n):
         for i in range(n):
             for j in range(n):
                 D[k+1][i][j] = min(D[k][i][j], D[k][i][k] + D[k][k][j])
     return D[n][:][:]
 
-def KnapSack(values, weights, n, W, no_values = True):
+def knap_sack(values, weights, n, W, no_values = True):
     '''
     Implementation of dynamic programming solution to the 0-1 `Knapsack Problem <https://en.wikipedia.org/wiki/Knapsack_problem>`_
     
     :param values: A list of values
     :param weights: A list with weight of corresponding values
     :param n: Number of items
     :param W: Desired weight
@@ -194,15 +194,15 @@
     .. code-block:: python
         
         values = [60, 100, 120]
         weights = [10, 20, 30]
         W = 50
         n = len(values)
         
-        print(KnapSack(values, weights, n, W)) #220
+        print(knap_sack(values, weights, n, W)) #220
     '''
     array = [[0 for _ in range(W + 1)] for _ in range(n + 1)]
         
     for i in range(n + 1):
         for j in range(W + 1):
             if i == 0 or j == 0:
                 array[i][j] = 0
@@ -214,15 +214,15 @@
     
     if no_values:
         return array[n][W]
     
     if no_values == False:
         return array
     
-def KnapSackValues(values, weights, n, W):
+def knap_sack_values(values, weights, n, W):
     '''
     Extension to KnapSack function
     It finds the actual values used to obtain the optimal sum
 
     :param values: A list of values
     :param weights: A list with weight of corresponding values
     :param n: Number of items
@@ -233,26 +233,26 @@
     .. code-block:: python
         
         values = [60, 100, 120]
         weights = [10, 20, 30]
         W = 50
         n = len(values)
         
-        print(KnapSackValues(values, weights, n, W)) #{20, 30}
+        print(knap_sack_values(values, weights, n, W)) #{20, 30}
     
     '''
-    array = KnapSack(values, weights, n, W, no_values = False)
+    array = knap_sack(values, weights, n, W, no_values = False)
     if n == 0:
         return {}
     if array[n][W] > array[n - 1][W]:
-        return {weights[n - 1]}.union(KnapSackValues(values, weights, n - 1, W - weights[n - 1]))
+        return {weights[n - 1]}.union(knap_sack_values(values, weights, n - 1, W - weights[n - 1]))
     else:
-        return KnapSackValues(values, weights, n - 1, W - weights[n - 1])
+        return knap_sack_values(values, weights, n - 1, W - weights[n - 1])
 
-def BFSSearch(g, start_node = 0, end_node = False):
+def BFS(g, start_node = 0, end_node = False):
     '''
     Implementation of `Breadth First Search <https://en.wikipedia.org/wiki/Breadth-first_search>`_
 
     :param g: An `Adjacency List <https://en.wikipedia.org/wiki/Adjacency_list>`_
     :param start_node: Optional, pick your start node. Default is 1st node
     :param end_node: Optional, pick your end node. Default is last node
 
@@ -261,15 +261,15 @@
     .. code-block:: python
         
         G = [[4, 1], [0, 5], [6, 3], [2, 7],
              [0, 8], [1, 6], [2, 5, 10], [3, 11],
              [4, 9], [8, 13], [6], [7, 15],
              [13], [9, 12, 14], [13, 15], [11, 14] ]
         
-        print(BFSSearch(G)) #[0, 4, 8, 9, 13, 14, 15]
+        print(BFS(G)) #[0, 4, 8, 9, 13, 14, 15]
     
     .. note::
         
         A quick comment on adjacency lists. The way it works is for example G[i] contains all the nodes
         node i is connected to. For example using the above graph G[0] = [4, 1] means node 0 is connected to nodes 1, and 4.
         
     '''
@@ -289,15 +289,15 @@
             
             for v in g[curr_v]:
                 if vertices[v] != 1:
                     new_path = path + [v]
                     queue.append((v, new_path))
     return []
 
-def DFSSearch(g, start_node = 0, end_node = False):
+def DFS(g, start_node = 0, end_node = False):
     '''
     Implementation of `Depth First Search <https://en.wikipedia.org/wiki/Depth-first_search>`_
 
     :param g: An `Adjacency List <https://en.wikipedia.org/wiki/Adjacency_list>`_
     :param start_node: Optional, pick your start node. Default is 1st node
     :param end_node: Optional, pick your end node. Default is last node
 
@@ -306,15 +306,15 @@
     .. code-block:: python
         
         G = [[4, 1], [0, 5], [6, 3], [2, 7],
              [0, 8], [1, 6], [2, 5, 10], [3, 11],
              [4, 9], [8, 13], [6], [7, 15],
              [13], [9, 12, 14], [13, 15], [11, 14] ]
         
-        print(DFSSearch(G)) #[0, 1, 5, 6, 2, 3, 7, 11, 15]
+        print(DFS(G)) #[0, 1, 5, 6, 2, 3, 7, 11, 15]
     
     '''
     if end_node == False:
         end_node = len(g) - 1
         
     vertices = [0 for _ in range(len(g))]
     path = [start_node]
@@ -329,15 +329,15 @@
             
             for v in g[curr_v]:
                 if vertices[v] != 1:
                     new_path = path + [v]
                     stack.append((v, new_path))
     return []
 
-def ConvexHullGiftWrapping(pts):
+def convex_hull_gift_wrapping(pts):
     '''
     Implementation of the Convex Hull `Gift Wrapping Algorithm <https://en.wikipedia.org/wiki/Gift_wrapping_algorithm>`_
     
     :param pts: A list containing 2D points
         
     :returns: A list of points consisting of the convex hull starting from leftmost point going around
         
@@ -348,39 +348,39 @@
     while hull_not_finished:
         p = convex_hull[-1] 
         for q in pts:
             if q != p:
                 flag = True 
                 for r in pts:
                     if (r != p) and (r != q):
-                        if IsClockwise(p, q, r) == False:
+                        if is_clockwise(p, q, r) == False:
                             flag = False
                             break    
                 if flag:
                     if q == lp:
                         hull_not_finished = False
                     else:
                         convex_hull.append(q)
     return convex_hull
 
-def ConvexHullDC(pts):
+def convex_hull_DC(pts):
     '''
     Implementation of the Convex Hull Divide and conquer Algorithm
     
     :param pts: A list containing 2D points
         
     :returns: A list of points consisting of the convex hull starting from leftmost point going around
         
     '''
     x_sort = sorted(pts)
     
     def divideCH(alist):
         l = len(alist) #Length of alist
         if l <= 5:
-            return ConvexHullGiftWrapping(alist)
+            return convex_hull_gift_wrapping(alist)
         mid = l//2
         left = divideCH(alist[:mid])
         right = divideCH(alist[mid:])
         return mergeCH(left, right)
 
     def mergeCH(left, right):
         top_r = max(left) 
@@ -400,38 +400,38 @@
         bot_r_index = bot_l_index + 1
         
         prev_r = None
         prev_l = None
         while True:
             prev_r = top_r
             prev_l = top_l
-            while IsClockwise(top_r, top_l, hull_copy[top_l_index + 1]) == False:
+            while is_clockwise(top_r, top_l, hull_copy[top_l_index + 1]) == False:
                 top_l_index += 1
                 top_l = hull_copy[top_l_index]
 
-            while IsClockwise(top_l, top_r, hull_copy[top_r_index - 1]):
+            while is_clockwise(top_l, top_r, hull_copy[top_r_index - 1]):
                 top_r_index -= 1            
                 top_r = hull_copy[top_r_index]
             
             if top_r == prev_r and top_l == prev_l:
                 break
         
         prev_r = None
         prev_l = None
         while True:
             prev_r = bot_r
             prev_l = bot_l
             
-            while IsClockwise(bot_r, bot_l, hull_copy[bot_l_index - 1]):
+            while is_clockwise(bot_r, bot_l, hull_copy[bot_l_index - 1]):
                 bot_l_index -= 1
                 bot_l = hull_copy[bot_l_index]
                 
             while True:
                 if bot_r_index + 1 < len_h:
-                    if IsClockwise(bot_l, bot_r, hull_copy[bot_r_index + 1]) == False:
+                    if is_clockwise(bot_l, bot_r, hull_copy[bot_r_index + 1]) == False:
                         bot_r_index += 1
                         bot_r = hull_copy[bot_r_index]
                     else:
                         break
                 else:
                     bot_r_index = -1     
             if bot_r == prev_r and bot_l == prev_l:
```

### Comparing `mathslib-2.7.0/src/mathslib/fib.py` & `mathslib-2.8.0/src/mathslib/fib.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,25 +70,25 @@
     fibnumbers = []
     n = 1
     while fibonacci(n) <= limit:
         fibnumbers.append(fibonacci(n))
         n += 1
     return fibnumbers
 
-def ZeckendorfRepresentation(x):
+def zeckendorf_representation(x):
     '''
     Finds the `Zeckendorf Representation <https://en.wikipedia.org/wiki/Zeckendorf%27s_theorem>`_ of x 
 
     :param x: An integer
 
     :returns: A list containing the zeckendorf representation of x
     
     .. code-block:: python
         
-        print(ZeckendorfRepresentation(64)) #[55, 8, 1]
+        print(zeckendorf_representation(64)) #[55, 8, 1]
 
     '''
     if type(x) != int:
         return "x must be an integer"
     zeckrep = []
     fibs = fib_till(x)[::-1]
```

### Comparing `mathslib-2.7.0/src/mathslib/linalg.py` & `mathslib-2.8.0/src/mathslib/linalg.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,29 +25,29 @@
 
 '''
 Various Linear Algebra Functions
 
 Author: Igor van Loo
 '''
 
-def GaussJordanElimination(matrix, augmentedpart = None):
+def gauss_jordan_elimination(matrix, augmentedpart = None):
     '''
     Performs `Gauss Jordan Elimination on the given matrix <https://en.wikipedia.org/wiki/Gaussian_elimination>`_
 
     :param matrix: Matrix to perform Algoithm on
     :param augmentedpart: Optional argument, will attach the augmented part onto the matrix and then perform the algorithm
 
     :returns: True if algorithm was successful, false otherwise
     
     .. code-block:: python
     
         matrix = [[2, 1, -1],
                   [-3, -1, 2],
                   [-2, 1, 2]]
-        print(GaussJordanElimination(matrix)) #True
+        print(gauss_jordan_elimination(matrix)) #True
     
     .. note::
         
         This function simply performs the Gauss Jordan Algorithm, it is used with with solve and inverse to solve Ax = b, and the find
         the inverse of a matrix
 
     '''
@@ -112,15 +112,15 @@
     if type(M) != list:
         return "M must be a list"
     m, n = len(M), len(M[0])
     if len(b[0]) > 1:
         return "b must be a vector"
     if m != len(b):
         return "Impossible to solve"
-    if GaussJordanElimination(M, b):
+    if gauss_jordan_elimination(M, b):
         return [M[x][n:] for x in range(m)]
     else:
         return "No solution, or infinite solutions"
     
 def inverse(matrix):
     '''
     Finds the inverse of the given matrix by performing Gauss Jordan Elimination
@@ -138,15 +138,15 @@
     
     '''
     if type(matrix) != list:
         return "matrix must be a list"
     m, n = len(matrix), len(matrix[0])
     if m != n:
         return "Must be a square matrix"
-    if GaussJordanElimination(matrix, identity(m)):
+    if gauss_jordan_elimination(matrix, identity(m)):
         return [matrix[x][m:] for x in range(m)]
     else:
         return "Matrix is not invertible"
 
 def determinant(matrix):
     '''
     Finds the determinant of a matrix
```

### Comparing `mathslib-2.7.0/src/mathslib/numtheory.py` & `mathslib-2.8.0/src/mathslib/numtheory.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 '''
 Various Number Theory functions
 
 Author: Igor van Loo
 '''
 import math
 from .primes import prime_factors, prime_sieve
-from .simple import ExtendedEuclideanAlgorithm
+from .simple import extended_euclidean_algorithm
 
 def divisors_of(x, include_x = True):
     '''
     Finds all the divisors of x
 
     :param x: Integer to be checked
     :param include_x: Optional boolean value, If true it will include x as a divisor of x
@@ -535,87 +535,87 @@
             return x
         gs = pow(g, 2**(r - m - 1), p)
         g = (gs * gs) % p
         x = (x * gs) % p
         b = (b * g) % p
         r = m
         
-def ChineseRemainderTheorem(a1, a2, n1, n2):
+def chinese_remainder_theorem(a1, a2, n1, n2):
     '''
     Simple `Chinese Remiander Theorem <https://en.wikipedia.org/wiki/Chinese_remainder_theorem>`__ to solve x = a1 mod n1, x = a2 mod n2
 
     :param a1: An integer
     :param a2: An integer
     :param n1: An integer
     :param n2: An integer
 
     :returns: Unique solution to x = a1 mod n1, x = a2 mod n2
     
     .. code-block:: python
         
         #We solve x = 2 mod 3 = 3 mod 5 = 2 mod 7
         #First we solve x = 2 mod = 3 mod 5
-        print(ChineseRemainderTheorem(2, 3, 3, 5)) #8 
+        print(chinese_remainder_theorem(2, 3, 3, 5)) #8 
         #Then we solve x = 8 mod 15 = 2 mod 7
-        print(ChineseRemainderTheorem(8, 2, 15, 7)) #23 
+        print(chinese_remainder_theorem(8, 2, 15, 7)) #23 
         
     '''
     if (type(a1) != int) or (type(a2) != int) or (type(n1) != int) or (type(n2) != int):
         return "All values must be integers"
     if a1 > n1 or a2 > n2:
         return "Wrong values were input"
     #x = a1 (mod n1)
     #x = a2 (mod n2)
     #We find p = n1^-1 (mod n2), q = n2^-1 (mod n1)
     p, q = pow(n1, -1, n2), pow(n2, -1, n1)
     #The unique solution to this system is a1*q*n2 + a2*p*n1 % n1*n2
     return (a1*q*n2+ a2*p*n1) % (n1*n2)
 
-def Generalised_CRT(a1, a2, n1, n2):
+def generalised_CRT(a1, a2, n1, n2):
     '''
     A generalised `Chinese Remiander Theorem <https://en.wikipedia.org/wiki/Chinese_remainder_theorem#Generalization_to_non-coprime_moduli>`__ which solves for non-coprime moduli
 
     :param a1: An integer
     :param a2: An integer
     :param n1: An integer
     :param n2: An integer
 
     :returns: Unique solution to x = a1 mod n1, x = a2 mod n2
     
     .. code-block:: python
         
-        print(Generalised_CRT(2, 3, 3, 5)) #8, note that we can use ChineseRemainderTheorem function for this case
-        print(Generalised_CRT(2, 4, 4, 6)) #10
-        print(Generalised_CRT(3, 4, 4, 6)) #'No solution'
+        print(generalised_CRT(2, 3, 3, 5)) #8, note that we can use ChineseRemainderTheorem function for this case
+        print(generalised_CRT(2, 4, 4, 6)) #10
+        print(generalised_CRT(3, 4, 4, 6)) #'No solution'
         
     '''
-    g, u, v = ExtendedEuclideanAlgorithm(n1, n2)
+    g, u, v = extended_euclidean_algorithm(n1, n2)
     if g == 1:
         return (a1*v*n2 + a2*u*n1) % (n1*n2)
     M = (n1*n2)//g
     if a1 % g != a2 % g:
         return "No solution"
     return ((a1*v*n2 + a2*u*n1)//g) % M
 
-def FrobeniusNumber(*integers):
+def frobenius_number(*integers):
     '''
     Generates the `Frobenius Number <https://en.wikipedia.org/wiki/Coin_problem>`_ for given integers.
     
     The below algorithm is based on `Faster Algorithms for Frobenius Numbers <https://www.cis.upenn.edu/~cis511/Frobenius-numbers-Nijenhuis-Wagon.pdf>`_
     specifically, this is an implementation of their Breadth-First Method which you may find on page 9
 
     :param: integers
 
     :returns: Frobenius number 
     
     .. code-block:: python3
     
-        print(FrobeniusNumber(3, 5)) #7
-        print(FrobeniusNumber(6, 9, 20)) #43
-        print(FrobeniusNumber(1000, 1476, 3764, 4864, 4871, 7773)) #47350
+        print(frobenius_number(3, 5)) #7
+        print(frobenius_number(6, 9, 20)) #43
+        print(frobenius_number(1000, 1476, 3764, 4864, 4871, 7773)) #47350
         
     '''
     #Set is first sorted
     A = sorted(integers) 
     #Initalize n value for future reference
     n = len(A) 
     #Initalize a1 and an for readability
```

### Comparing `mathslib-2.7.0/src/mathslib/primes.py` & `mathslib-2.8.0/src/mathslib/primes.py`

 * *Files 20% similar despite different names*

```diff
@@ -164,27 +164,84 @@
                 if d in factors:
                     factors[n] += 1
                 else:
                     factors[n] = 1
             break
     return factors
 
-def primepi(limit):
+def primepi(x):
+    '''
+    Primepi function is commonly known as `Prime Counting Function <https://en.wikipedia.org/wiki/Prime-counting_function>`_
+    
+    This function computes primepi(x) based on the `Meissel-Lehmer Method <https://mathworld.wolfram.com/LehmersFormula.html>`_
+    
+    The following `article <https://acgan.sh/posts/2016-12-23-prime-counting.html>`_ by Adithya Ganesh helped me a lot in understanding and implementing this function
+    
+    :param x: An integer
+
+    :returns: primepi(x)
+    
+    .. code-block:: python
+    
+        print(primepi(10**6)) #78498
+        print(primepi(10**7)) #664579
+        print(primepi(10**8)) #5761455
+        print(primepi(10**9)) #50847534
+        
+    '''
+    limit = int(math.sqrt(x))
+    primes = prime_sieve(limit)
+    array = primepi_sieve(limit)
+    
+    phiCache = {}
+    def phi(x, a):
+        if (x, a) in phiCache:
+            return phiCache[(x, a)]
+        if a == 0:
+            return int(x)
+        if a == 1:
+            return int(x) - x//2
+        result = phi(x, a - 1) - phi(int(x / primes[a - 1]), a - 1)
+        phiCache[(x, a)] = result
+        return result
+    
+    piCache = {}
+    def pi(x):
+        if int(x) in piCache:
+            return piCache[int(x)]
+        if x <= limit:
+            return array[math.floor(x)]
+        a = pi(pow(x, 1/4))
+        b = pi(pow(x, 1/2))
+        c = pi(pow(x, 1/3))
+        result = phi(int(x), int(a)) + ((b + a - 2) * (b - a + 1))//2
+        for i in range(a + 1, b + 1):
+            w = x / primes[i - 1]
+            result -= pi(w)
+            if i <= c:
+                bi = pi(int(math.sqrt(w)))
+                for j in range(i, bi + 1):
+                    result -= (pi(w / primes[j - 1]) - j + 1)
+        piCache[int(x)] = result
+        return int(result)
+    return int(pi(x))
+
+def primepi_sieve(limit):
     '''
     Primepi function is commonly known as `Prime Counting Function <https://en.wikipedia.org/wiki/Prime-counting_function>`_
     
     This function generates an array such that array[x] = primepi(x)
 
     :param limit: An integer, 
 
     :returns: An array length limit such that array[x] = primepi(x)
     
     .. code-block:: python
     
-        print(primepi(10)) #[0, 0, 1, 2, 2, 3, 3, 4, 4, 4, 4]
+        print(primepi_sieve(10)) #[0, 0, 1, 2, 2, 3, 3, 4, 4, 4, 4]
         
     '''
     if type(limit) != int:
         return "limit must be an integer"
     
     prime_gen = prime_sieve(limit + 50, values = False)
     primes = [x for x in range(len(prime_gen)) if prime_gen[x]]
@@ -260,31 +317,31 @@
         return is_prime(n)
     else: 
         for x in range(tests):
             if pow(2*(x + 2), n - 1, n) != 1:
                 return False
         return True
     
-def miller(n, millerrabin = False, numoftests = 2):
+def miller_primality_test(n, millerrabin = False, numoftests = 2):
     '''
     The `Miller Primality Test <https://en.wikipedia.org/wiki/Miller%E2%80%93Rabin_primality_test#Miller_test>`_
     with the option to use the `Miller-Rabin test <https://en.wikipedia.org/wiki/Miller%E2%80%93Rabin_primality_test>`_
 
     :param n: The integer to be tested
     :param millerrabin: Optional, default False. Decides with the use Miller-Rabin or Miller primality test 
     :param numoftests: Optional, default is 2. If millerrabin is True, it uses numoftests bases
 
     :returns: True if n is probably prime, False if n is not prime
     
     .. code-block:: python
     
-        print(miller(17969800575241)) #True
-        print(miller(101101)) #False
-        print(len([x for x in range(1, 10**6) if miller(x, True, 1)])) #78544, 46 more primes than needed
-        print(len([x for x in range(1, 10**6) if miller(x, True, 2)])) #78498, correct now
+        print(miller_primality_test(17969800575241)) #True
+        print(miller_primality_test(101101)) #False
+        print(len([x for x in range(1, 10**6) if miller_primality_test(x, True, 1)])) #78544, 46 more primes than needed
+        print(len([x for x in range(1, 10**6) if miller_primality_test(x, True, 2)])) #78498, correct now
         
     .. note::
         Automatically uses the Miller Primality Test to get an exact an answer if n < 3317044064679887385961981 and swaps
         to using the first 17 primes, but no longer guarantees a correct answer. You may optionally use a regular miller-rabin test
         with a specified number of tests
 
     '''
```

### Comparing `mathslib-2.7.0/src/mathslib/simple.py` & `mathslib-2.8.0/src/mathslib/simple.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,59 +41,63 @@
     :returns: n choose r
     
     .. code-block:: python
     
         print(n_choose_r(50, 30)) #47129212243960
         
     '''
+    if (type(n) != int) or (type(r) != int):
+        return "n and r must be an integers"
     if r > n:
         return "n must be greter than r"
     else:
         return int(math.factorial(n) / (math.factorial(r) * math.factorial(n-r)))
     
-def numberToBase(n, b):
+def number_to_base(n, b):
     '''
     Changes n from base 10 to base b
 
     :param n: An integer, number to be changed
     :param b: An integer, base in question
 
     :returns: n in base b
         
     .. code-block:: python
     
-        print(numberToBase(10, 2)) #[1, 0, 1, 0]
-        print(numberToBase(10, 3)) #[1, 0, 1]
+        print(number_to_base(10, 2)) #[1, 0, 1, 0]
+        print(number_to_base(10, 3)) #[1, 0, 1]
         
     '''
     if (type(n) != int) or (type(b) != int):
         return "n and b must be an integer"
     if n == 0:
         return [0]
     digits = []
     while n != 0:
         digits.append(int(n % b))
         n //= b
     return digits[::-1]
 
-def ExtendedEuclideanAlgorithm(a, b):
+def extended_euclidean_algorithm(a, b):
     '''
     Standard `Extended Euclidean Algorithm
     <https://en.wikipedia.org/wiki/Extended_Euclidean_algorithm#Pseudocode>`_
 
     :param a: An integer
     :param b: An integer
 
     :returns: A tuple (g, s, t) where gcd(a, b) = g = as + bt
     
     .. code-block:: python
     
-        print(ExtendedEuclideanAlgorithm(240, 46)) #(2, -9, 47)
+        print(extended_euclidean_algorithm(240, 46)) #(2, -9, 47)
 
     '''
+    if (type(a) != int) or (type(b) != int):
+        return "a and b must be integers"
     old_r, r = a, b
     old_s, s = 1, 0
     while r != 0:
         q = old_r // r
         old_r, r = r, old_r - q*r
         old_s, s = s, old_s - q*s 
     if b != 0:
@@ -120,42 +124,66 @@
     n = sorted(a_list)
     curr = n.pop(-1)
     while len(n) != 0:
         temp = n.pop(-1)
         curr = int(abs(curr*temp)/math.gcd(curr, temp))
     return curr
 
-def ModDivision(a, b, m):
+def mod_division(a, b, m):
     '''
     Finds a/b mod m
 
     :param a: An integer, the numerator
     :param b: An integer, the denominator
     :param m: An integer, the modulus
 
     :returns: a/b mod m
     
     .. code-block:: python
     
-        print(ModDivision(8, 4, 5)) #2
+        print(mod_division(8, 4, 5)) #2
         
     '''
     if (type(a) != int) or (type(b) != int) or (type(m) != int):
         return "n and b must be an integer"
     try:
         inv = pow(b, -1, m)
     except ValueError:
         if a % b == 0:
             answer = (a % m * b) // b
     else:
         a = a % m
         answer = (inv * a) % m
     return answer
 
-def IsClockwise(a,b,c):
+def bisect(alist, goal):
+    '''
+    This function is equivalent to bisect_right from the bisect module
+
+    :param alist: A list
+    :param goal: A number
+
+    :returns: index i of A such that A[i - 1] < g <= A[i]
+    
+    .. code-block:: python
+    
+        print(bisect([2, 3, 5, 7], 6)) #3 since A[2] = 5 < 6 <= A[3] = 7
+        
+    '''
+    lo = 0
+    hi = len(alist)
+    while lo < hi:
+        mid = (lo + hi)//2
+        if goal < alist[mid]:
+            hi = mid
+        else:
+            lo = mid + 1
+    return lo
+
+def is_clockwise(a,b,c):
     '''
     Finds if 3 points a going to b going to c are in clockwise order. It is used in convex
     hull algorithm
 
     :param a: A tuple, representing a point in 2D
     :param b: A tuple, representing a point in 2D
     :param c: A tuple, representing a point in 2D
```

### Comparing `mathslib-2.7.0/src/mathslib.egg-info/PKG-INFO` & `mathslib-2.8.0/src/mathslib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathslib
-Version: 2.7.0
+Version: 2.8.0
 Summary: Library of Mathematical functions and Algorithms
 Home-page: https://github.com/igorvanloo/mathslib
 Author: Igor van Loo
 Author-email: igorvanloo@gmail.com
 Project-URL: Bug Reports, https://github.com/igorvanloo/mathslib/issues
 Project-URL: Source, https://github.com/igorvanloo/mathslib
 Keywords: numbertheory,maths,algorithms
@@ -26,15 +26,17 @@
 .. image:: https://img.shields.io/pypi/v/mathslib.svg
         :target: https://pypi.python.org/pypi/mathslib
 
 .. image:: https://readthedocs.org/projects/mathslib/badge/?version=latest
         :target: https://mathslib.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
-`mathslib`__ is a compilation of Mathematical Functions and Algorithms I have made or come across.
+`mathslib`__ is a compilation of Mathematical Functions and Algorithms. Unless credit was given all
+of the functions were written by me. Relevant articles are also linked where the implementation is complex.
+
 I have used most of these for `Project Euler`_.
  
 See my website `ivl-projecteuler.com`_ for their implementation
 
 See the full documentation `here`_
 
 Breakdown
@@ -50,57 +52,59 @@
 |                | * mobius_k_sieve(limit, k)                                 |
 |                | * count_k_free(n, k)                                       |
 |                | * ppt(limit, non_primitive)                                |
 |                | * k_smooth_numbers(max_prime, limit)                       |
 |                | * k_powerful(k, limit, count)                              |
 |                | * legendre_factorial(x)                                    |
 |                | * tonelli_shanks(a, p)                                     |
-|                | * ChineseRemainderTheorem(a1, a2, n1, n2)                  |
-|                | * Generalised_CRT(a1, a2, n1, n2)                          |
-|                | * FrobeniusNumber(\*integers)                              |
+|                | * chinese_remainder_theorem(a1, a2, n1, n2)                |
+|                | * generalised_CRT(a1, a2, n1, n2)                          |
+|                | * frobenius_number(\*integers)                             |
 +----------------+------------------------------------------------------------+
 |prime.py        | * prime_sieve(limit, block_size, segment, values)          |
 |                | * is_prime(x)                                              |
 |                | * prime_factors(x)                                         |
 |                | * primepi(x)                                               |
+|                | * primepi_sieve(x)                                         |
 |                | * sum_of_primes(x)                                         |
 |                | * fermat_primality_test(x)                                 |
-|                | * miller(n, millerrabin, numoftests)                       |
+|                | * miller_primality_test(n, millerrabin, numoftests)        |
 +----------------+------------------------------------------------------------+
-|linalg.py       | * GaussJordanElimination(matrix, augmentedpart)            |
+|linalg.py       | * gauss_jordan_elimination(matrix, augmentedpart)          |
 |                | * solve(M, b)                                              |
 |                | * inverse(matrix)                                          |
 |                | * determinant(matrix)                                      |
 |                | * matrix_addition(A, B, subtract)                          |
 |                | * identity(l, val)                                         |
 |                | * concatenate(A, B)                                        |
 |                | * argmax(alist)                                            |
 |                | * fillmatrix(size, val)                                    |
 |                | * matrix_mul(A, B)                                         |
 +----------------+------------------------------------------------------------+
 |fib.py          | * fibonacci(n)                                             |
 |                | * fib_till(limit)                                          |
-|                | * ZeckendorfRepresentation(x)                              |
+|                | * zeckendorf_representation(x)                             |
 +----------------+------------------------------------------------------------+
-|algorithms.py   | * PrimsAlgorithm(matrix)                                   |
-|                | * DijkstrasAlgorithm(graph, start_node, INFINITY)          |
-|                | * FloydWarshallAlgorithm(graph, INFINITY)                  |
-|                | * KnapSack(values, weights, n, W, no_values)               |
-|                | * KnapSackValues(values, weights, n, W, no_values)         |
-|                | * BFSSearch(g, start_node, end_node)                       |
-|                | * DFSSearch(g, start_node, end_node)                       |
-|                | * ConvexHullGiftWrapping(pts)                              |
-|                | * ConvexHullDC(pts)                                        |
+|algorithms.py   | * prims_algorithm(matrix)                                  |
+|                | * dijkstras_algorithm(graph, start_node, INFINITY)         |
+|                | * floyd_warshall_algorithm(graph, INFINITY)                |
+|                | * knap_sack(values, weights, n, W, no_values)              |
+|                | * knap_sack_values(values, weights, n, W, no_values)       |
+|                | * BFS(g, start_node, end_node)                             |
+|                | * DFS(g, start_node, end_node)                             |
+|                | * convex_hull_gift_wrapping(pts)                           |
+|                | * convex_hull_DC(pts)                                      |
 +----------------+------------------------------------------------------------+
 |simple.py       | * n_choose_r(n, r)                                         | 
-|                | * numberToBase(n, b)                                       |
-|                | * ExtendedEuclideanAlgorithm(n, b)                         |
+|                | * number_to_base(n, b)                                     |
+|                | * extended_euclidean_algorithm(n, b)                       |
 |                | * lcm(a_list)                                              |
-|                | * ModDivision(a, b, m)                                     |
-|                | * IsClockwise(a, b, c)                                     |
+|                | * mod_division(a, b, m)                                    |
+|                | * bisect(alist, goal)                                      |
+|                | * is_clockwise(a, b, c)                                    |
 +----------------+------------------------------------------------------------+
 
 .. _Project Euler: https://projecteuler.net
 .. _ivl-projecteuler.com: https://ivl-projecteuler.com
 .. _mathslib1: https://pypi.python.org/pypi/mathslib
 .. _here: https://mathslib.readthedocs.io/en/latest/index.html
 __ mathslib1_
```

