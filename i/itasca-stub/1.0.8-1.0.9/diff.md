# Comparing `tmp/itasca-stub-1.0.8.tar.gz` & `tmp/itasca-stub-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\itasca-stub-1.0.8.tar", last modified: Tue Jun 16 09:39:37 2020, max compression
+gzip compressed data, was "dist\itasca-stub-1.0.9.tar", last modified: Tue Jun 16 12:06:02 2020, max compression
```

## Comparing `itasca-stub-1.0.8.tar` & `itasca-stub-1.0.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.276263 itasca-stub-1.0.8/
--rw-rw-rw-   0        0        0     2208 2020-06-16 09:39:37.275266 itasca-stub-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1130 2020-05-25 08:52:33.000000 itasca-stub-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.222406 itasca-stub-1.0.8/itasca/
--rw-rw-rw-   0        0        0   175255 2020-06-16 09:39:34.000000 itasca-stub-1.0.8/itasca/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.223441 itasca-stub-1.0.8/itasca/ball/
--rw-rw-rw-   0        0        0    17256 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/ball/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.224437 itasca-stub-1.0.8/itasca/ball/thermal/
--rw-rw-rw-   0        0        0    10484 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/ball/thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.225430 itasca-stub-1.0.8/itasca/ballarray/
--rw-rw-rw-   0        0        0     9734 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/ballarray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.226395 itasca-stub-1.0.8/itasca/ballballarray/
--rw-rw-rw-   0        0        0     6810 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/ballballarray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.227392 itasca-stub-1.0.8/itasca/ballfacetarray/
--rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/ballfacetarray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.228390 itasca-stub-1.0.8/itasca/ballpebblearray/
--rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/ballpebblearray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.230385 itasca-stub-1.0.8/itasca/ballrblockarray/
--rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/ballrblockarray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.231382 itasca-stub-1.0.8/itasca/clump/
--rw-rw-rw-   0        0        0    27129 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/clump/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.233376 itasca-stub-1.0.8/itasca/clump/pebble/
--rw-rw-rw-   0        0        0     8700 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/clump/pebble/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.234374 itasca-stub-1.0.8/itasca/clump/template/
--rw-rw-rw-   0        0        0     8355 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/clump/template/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.235370 itasca-stub-1.0.8/itasca/clump/thermal/
--rw-rw-rw-   0        0        0    10149 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/clump/thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.237366 itasca-stub-1.0.8/itasca/clump/thermal/pebble/
--rw-rw-rw-   0        0        0     8544 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/clump/thermal/pebble/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.238364 itasca-stub-1.0.8/itasca/clumparray/
--rw-rw-rw-   0        0        0    10247 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/clumparray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.239360 itasca-stub-1.0.8/itasca/contact/
--rw-rw-rw-   0        0        0     3548 2020-06-13 12:58:34.000000 itasca-stub-1.0.8/itasca/contact/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.240358 itasca-stub-1.0.8/itasca/dfn/
--rw-rw-rw-   0        0        0     9543 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/dfn/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.241356 itasca-stub-1.0.8/itasca/dfn/fracture/
--rw-rw-rw-   0        0        0    11236 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/dfn/fracture/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.242352 itasca-stub-1.0.8/itasca/dfn/inter/
--rw-rw-rw-   0        0        0     5878 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/dfn/inter/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.244347 itasca-stub-1.0.8/itasca/dfn/setinter/
--rw-rw-rw-   0        0        0     3343 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/dfn/setinter/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.245344 itasca-stub-1.0.8/itasca/dfn/template/
--rw-rw-rw-   0        0        0     7982 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/dfn/template/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.246345 itasca-stub-1.0.8/itasca/dfn/vertex/
--rw-rw-rw-   0        0        0     2632 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/dfn/vertex/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.247340 itasca-stub-1.0.8/itasca/facetarray/
--rw-rw-rw-   0        0        0     2394 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/facetarray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.248336 itasca-stub-1.0.8/itasca/fish/
--rw-rw-rw-   0        0        0      892 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/fish/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.250350 itasca-stub-1.0.8/itasca/measure/
--rw-rw-rw-   0        0        0     5384 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/measure/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.251352 itasca-stub-1.0.8/itasca/pebblearray/
--rw-rw-rw-   0        0        0     2510 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/pebblearray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.252327 itasca-stub-1.0.8/itasca/pebblefacetarray/
--rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/pebblefacetarray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.253324 itasca-stub-1.0.8/itasca/pebblepebblearray/
--rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/pebblepebblearray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.254321 itasca-stub-1.0.8/itasca/pebblerblockarray/
--rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/pebblerblockarray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.256315 itasca-stub-1.0.8/itasca/rblock/
--rw-rw-rw-   0        0        0    26325 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/rblock/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.257314 itasca-stub-1.0.8/itasca/rblock/template/
--rw-rw-rw-   0        0        0     5633 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/rblock/template/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.258310 itasca-stub-1.0.8/itasca/rblockarray/
--rw-rw-rw-   0        0        0    10359 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/rblockarray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.259308 itasca-stub-1.0.8/itasca/rblockfacetarray/
--rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/rblockfacetarray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.260306 itasca-stub-1.0.8/itasca/rblockrblockarray/
--rw-rw-rw-   0        0        0     6818 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/rblockrblockarray/__init__.py
--rw-rw-rw-   0        0        0      386 2020-06-13 12:55:37.000000 itasca-stub-1.0.8/itasca/types.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.261302 itasca-stub-1.0.8/itasca/vertexarray/
--rw-rw-rw-   0        0        0     1177 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/vertexarray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.262300 itasca-stub-1.0.8/itasca/wall/
--rw-rw-rw-   0        0        0    16481 2020-06-14 00:18:20.000000 itasca-stub-1.0.8/itasca/wall/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.263297 itasca-stub-1.0.8/itasca/wall/facet/
--rw-rw-rw-   0        0        0    10724 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/wall/facet/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.264293 itasca-stub-1.0.8/itasca/wall/thermal/
--rw-rw-rw-   0        0        0     8075 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/wall/thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.266288 itasca-stub-1.0.8/itasca/wall/thermal/facet/
--rw-rw-rw-   0        0        0     8292 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/wall/thermal/facet/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.267286 itasca-stub-1.0.8/itasca/wall/vertex/
--rw-rw-rw-   0        0        0     5344 2020-05-24 15:49:25.000000 itasca-stub-1.0.8/itasca/wall/vertex/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.268283 itasca-stub-1.0.8/itasca/wallarray/
--rw-rw-rw-   0        0        0     5836 2020-05-24 15:49:24.000000 itasca-stub-1.0.8/itasca/wallarray/__init__.py
-drwxrwxrwx   0        0        0        0 2020-06-16 09:39:37.274267 itasca-stub-1.0.8/itasca_stub.egg-info/
--rw-rw-rw-   0        0        0     2208 2020-06-16 09:39:37.000000 itasca-stub-1.0.8/itasca_stub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1416 2020-06-16 09:39:37.000000 itasca-stub-1.0.8/itasca_stub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-06-16 09:39:37.000000 itasca-stub-1.0.8/itasca_stub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2020-06-16 09:39:37.000000 itasca-stub-1.0.8/itasca_stub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-06-16 09:39:37.276263 itasca-stub-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      926 2020-06-16 09:39:34.000000 itasca-stub-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.522992 itasca-stub-1.0.9/
+-rw-rw-rw-   0        0        0     2208 2020-06-16 12:06:02.522992 itasca-stub-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1130 2020-05-25 08:52:33.000000 itasca-stub-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.460235 itasca-stub-1.0.9/itasca/
+-rw-rw-rw-   0        0        0   175255 2020-06-16 09:39:34.000000 itasca-stub-1.0.9/itasca/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.461157 itasca-stub-1.0.9/itasca/ball/
+-rw-rw-rw-   0        0        0    17256 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/ball/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.463152 itasca-stub-1.0.9/itasca/ball/thermal/
+-rw-rw-rw-   0        0        0    10484 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/ball/thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.464148 itasca-stub-1.0.9/itasca/ballarray/
+-rw-rw-rw-   0        0        0     9827 2020-06-16 12:05:33.000000 itasca-stub-1.0.9/itasca/ballarray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.466145 itasca-stub-1.0.9/itasca/ballballarray/
+-rw-rw-rw-   0        0        0     6810 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/ballballarray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.467141 itasca-stub-1.0.9/itasca/ballfacetarray/
+-rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/ballfacetarray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.468139 itasca-stub-1.0.9/itasca/ballpebblearray/
+-rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/ballpebblearray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.470133 itasca-stub-1.0.9/itasca/ballrblockarray/
+-rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/ballrblockarray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.471130 itasca-stub-1.0.9/itasca/clump/
+-rw-rw-rw-   0        0        0    27129 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/clump/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.473126 itasca-stub-1.0.9/itasca/clump/pebble/
+-rw-rw-rw-   0        0        0     8700 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/clump/pebble/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.475128 itasca-stub-1.0.9/itasca/clump/template/
+-rw-rw-rw-   0        0        0     8355 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/clump/template/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.477115 itasca-stub-1.0.9/itasca/clump/thermal/
+-rw-rw-rw-   0        0        0    10149 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/clump/thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.478112 itasca-stub-1.0.9/itasca/clump/thermal/pebble/
+-rw-rw-rw-   0        0        0     8544 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/clump/thermal/pebble/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.480106 itasca-stub-1.0.9/itasca/clumparray/
+-rw-rw-rw-   0        0        0    10247 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/clumparray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.481118 itasca-stub-1.0.9/itasca/contact/
+-rw-rw-rw-   0        0        0     3548 2020-06-13 12:58:34.000000 itasca-stub-1.0.9/itasca/contact/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.483099 itasca-stub-1.0.9/itasca/dfn/
+-rw-rw-rw-   0        0        0     9543 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/dfn/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.484096 itasca-stub-1.0.9/itasca/dfn/fracture/
+-rw-rw-rw-   0        0        0    11236 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/dfn/fracture/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.485093 itasca-stub-1.0.9/itasca/dfn/inter/
+-rw-rw-rw-   0        0        0     5878 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/dfn/inter/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.487088 itasca-stub-1.0.9/itasca/dfn/setinter/
+-rw-rw-rw-   0        0        0     3343 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/dfn/setinter/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.488085 itasca-stub-1.0.9/itasca/dfn/template/
+-rw-rw-rw-   0        0        0     7982 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/dfn/template/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.489082 itasca-stub-1.0.9/itasca/dfn/vertex/
+-rw-rw-rw-   0        0        0     2632 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/dfn/vertex/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.490080 itasca-stub-1.0.9/itasca/facetarray/
+-rw-rw-rw-   0        0        0     2394 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/facetarray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.492075 itasca-stub-1.0.9/itasca/fish/
+-rw-rw-rw-   0        0        0      892 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/fish/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.493071 itasca-stub-1.0.9/itasca/measure/
+-rw-rw-rw-   0        0        0     5384 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/measure/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.494069 itasca-stub-1.0.9/itasca/pebblearray/
+-rw-rw-rw-   0        0        0     2510 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/pebblearray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.496064 itasca-stub-1.0.9/itasca/pebblefacetarray/
+-rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/pebblefacetarray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.497061 itasca-stub-1.0.9/itasca/pebblepebblearray/
+-rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/pebblepebblearray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.498058 itasca-stub-1.0.9/itasca/pebblerblockarray/
+-rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/pebblerblockarray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.500053 itasca-stub-1.0.9/itasca/rblock/
+-rw-rw-rw-   0        0        0    26325 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/rblock/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.501050 itasca-stub-1.0.9/itasca/rblock/template/
+-rw-rw-rw-   0        0        0     5633 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/rblock/template/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.502048 itasca-stub-1.0.9/itasca/rblockarray/
+-rw-rw-rw-   0        0        0    10359 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/rblockarray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.503045 itasca-stub-1.0.9/itasca/rblockfacetarray/
+-rw-rw-rw-   0        0        0     6527 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/rblockfacetarray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.505040 itasca-stub-1.0.9/itasca/rblockrblockarray/
+-rw-rw-rw-   0        0        0     6818 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/rblockrblockarray/__init__.py
+-rw-rw-rw-   0        0        0      386 2020-06-13 12:55:37.000000 itasca-stub-1.0.9/itasca/types.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.506037 itasca-stub-1.0.9/itasca/vertexarray/
+-rw-rw-rw-   0        0        0     1177 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/vertexarray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.508043 itasca-stub-1.0.9/itasca/wall/
+-rw-rw-rw-   0        0        0    16481 2020-06-14 00:18:20.000000 itasca-stub-1.0.9/itasca/wall/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.510027 itasca-stub-1.0.9/itasca/wall/facet/
+-rw-rw-rw-   0        0        0    10724 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/wall/facet/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.511024 itasca-stub-1.0.9/itasca/wall/thermal/
+-rw-rw-rw-   0        0        0     8075 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/wall/thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.512021 itasca-stub-1.0.9/itasca/wall/thermal/facet/
+-rw-rw-rw-   0        0        0     8292 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/wall/thermal/facet/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.514016 itasca-stub-1.0.9/itasca/wall/vertex/
+-rw-rw-rw-   0        0        0     5344 2020-05-24 15:49:25.000000 itasca-stub-1.0.9/itasca/wall/vertex/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.515013 itasca-stub-1.0.9/itasca/wallarray/
+-rw-rw-rw-   0        0        0     5836 2020-05-24 15:49:24.000000 itasca-stub-1.0.9/itasca/wallarray/__init__.py
+drwxrwxrwx   0        0        0        0 2020-06-16 12:06:02.520998 itasca-stub-1.0.9/itasca_stub.egg-info/
+-rw-rw-rw-   0        0        0     2208 2020-06-16 12:06:02.000000 itasca-stub-1.0.9/itasca_stub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1416 2020-06-16 12:06:02.000000 itasca-stub-1.0.9/itasca_stub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-06-16 12:06:02.000000 itasca-stub-1.0.9/itasca_stub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2020-06-16 12:06:02.000000 itasca-stub-1.0.9/itasca_stub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-06-16 12:06:02.522992 itasca-stub-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      926 2020-06-16 12:05:42.000000 itasca-stub-1.0.9/setup.py
```

### Comparing `itasca-stub-1.0.8/PKG-INFO` & `itasca-stub-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itasca-stub
-Version: 1.0.8
+Version: 1.0.9
 Summary: Itasca PFC python stub
 Home-page: https://github.com/panhaoyu/itasca-stub
 Author: panhaoyu
 Author-email: panhaoyu.china@outlook.com
 License: MIT
 Download-URL: https://github.com/panhaoyu/itasca-stub/archive/1.0.0.tar.gz
 Description: # itasca-stub
```

### Comparing `itasca-stub-1.0.8/README.md` & `itasca-stub-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/__init__.py` & `itasca-stub-1.0.9/itasca/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/ball/__init__.py` & `itasca-stub-1.0.9/itasca/ball/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/ball/thermal/__init__.py` & `itasca-stub-1.0.9/itasca/ball/thermal/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/ballarray/__init__.py` & `itasca-stub-1.0.9/itasca/ballarray/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,378 +1,431 @@
-from typing import Any
+from typing import Any, Dict
+from numpy import ndarray
 
-def create(*args, **kwargs) -> Any:
+
+def create(radii: ndarray, centroids: ndarray,
+           props: Dict[str, Any] = None,
+           extra: Dict[str, Any] = None,
+           ) -> ndarray:
     """
-    (radii: array float{ball}, centroids: array float{ball,dim}, **kwds) -> array int{ball} IDs of the newly created balls.
     Create balls from two arrays.
-    The first array must contain the radii, and the second array the positions.
-    The arrays must be the correct shape.
-    Additional keyword arguments can be specified which will set the newly created ball attributes.
+    Keyword arguments can be specified which will set the newly created ball attributes.
     The keyword arguments values can be scalars, vecs or arrays of 1 or two dimensions.
-    The keyword argument props can be used to set ball properties, the value should be a dict of type {str: value}.
-    The keyword argument extra can be used to set extra variables, the value should be a dict of type {int: value}.
     The props or extra dictionary values can be a 1 or 2 dimensional array of doubles, a number, a vec or a string.
+    :param radii: array float{ball}
+    :param centroids: array float{ball,dim}
+    :param props: used to set ball properties, the value should be a dict of type {str: value}
+    :param extra: used to set extra variables, the value should be a dict of type {int: value}
+    :return: array int{ball} IDs of the newly created balls
     """
     pass
 
+
 def damp(*args, **kwargs) -> Any:
     """
     () -> array float{ball}.
     Get a numpy array of the ball local damping.
     """
     pass
 
+
 def density(*args, **kwargs) -> Any:
     """
     () -> array float{ball}.
     Get a numpy array of the ball density.
     """
     pass
 
+
 def disp(*args, **kwargs) -> Any:
     """
     () -> array float{ball,2}.
     Get a numpy array of the ball displacement.
     """
     pass
 
+
 def extra(*args, **kwargs) -> Any:
     """
     (slot: int) -> array float{ball} or float{ball}.
     Get the ball extra data in the given slot as an array.
     Extra variables accessed by array must be of type float or vec.
     """
     pass
 
+
 def fill_damp(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Fill an existing array with the ball local damping.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_density(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Fill an existing array with the ball density.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_disp(*args, **kwargs) -> Any:
     """
     (data: array float{ball,2}) -> None.
     Fill an existing array with the ball displacement.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_force_app(*args, **kwargs) -> Any:
     """
     (data: array float{ball,2}) -> None.
     Fill an existing array with the ball applied force.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_force_contact(*args, **kwargs) -> Any:
     """
     (data: array float{ball,2}) -> None.
     Fill an existing array with the ball contact force.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_force_unbal(*args, **kwargs) -> Any:
     """
     (data: array float{ball,2}) -> None.
     Fill an existing array with the ball unbalanced force.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_mass(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Fill an existing array with the inertial ball mass.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_mass_real(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Fill an existing array with the real (gravitational) ball mass.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_moment_app(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Fill an existing array with the ball applied moment.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_moment_contact(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Fill an existing array with the ball contact moment.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_moment_unbal(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Fill an existing array with the ball unbalanced moment.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_pos(*args, **kwargs) -> Any:
     """
     (data: array float{ball,2}) -> None.
     Fill an existing array with the ball centroid location.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_radius(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Fill an existing array with the ball radii.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_rotation(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Fill an existing array with the ball orientation.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_spin(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Fill an existing array with the ball angular velocity.
     The array must be the correct shape.
     """
     pass
 
+
 def fill_vel(*args, **kwargs) -> Any:
     """
     (data: array float{ball,2}) -> None.
     Fill an existing array with the ball velocity.
     The array must be the correct shape.
     """
     pass
 
+
 def force_app(*args, **kwargs) -> Any:
     """
     () -> array float{ball,2}.
     Get a numpy array of the ball applied force.
     """
     pass
 
+
 def force_contact(*args, **kwargs) -> Any:
     """
     () -> array float{ball,2}.
     Get a numpy array of the ball contact force.
     """
     pass
 
+
 def force_unbal(*args, **kwargs) -> Any:
     """
     () -> array float{ball,2}.
     Get a numpy array of the ball unbalanced force.
     """
     pass
 
+
 def ids(*args, **kwargs) -> Any:
     """
     () -> array int{ball}.
     Get the ball ids as an array.
     """
     pass
 
+
 def in_group(*args, **kwargs) -> Any:
     """
     (group_name: str, slot=1) -> array bool{ball}.
     Return ball group membership as a Boolean array.
     """
     pass
 
+
 def mass(*args, **kwargs) -> Any:
     """
     () -> array float{ball}.
     Get a numpy array of the inertial ball mass.
     """
     pass
 
+
 def mass_real(*args, **kwargs) -> Any:
     """
     () -> array float{ball}.
     Get a numpy array of the real (gravitational) ball mass.
     """
     pass
 
+
 def moment_app(*args, **kwargs) -> Any:
     """
     () -> array float{ball}.
     Get a numpy array of the ball applied moment.
     """
     pass
 
+
 def moment_contact(*args, **kwargs) -> Any:
     """
     () -> array float{ball}.
     Get a numpy array of the ball contact moment.
     """
     pass
 
+
 def moment_unbal(*args, **kwargs) -> Any:
     """
     () -> array float{ball}.
     Get a numpy array of the ball unbalanced moment.
     """
     pass
 
+
 def pos(*args, **kwargs) -> Any:
     """
     () -> array float{ball,2}.
     Get a numpy array of the ball centroid location.
     """
     pass
 
+
 def radius(*args, **kwargs) -> Any:
     """
     () -> array float{ball}.
     Get a numpy array of the ball radii.
     """
     pass
 
+
 def rotation(*args, **kwargs) -> Any:
     """
     () -> array float{ball}.
     Get a numpy array of the ball orientation.
     """
     pass
 
+
 def set_damp(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Set the ball local damping from an array.
     """
     pass
 
+
 def set_density(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Set the ball density from an array.
     """
     pass
 
+
 def set_disp(*args, **kwargs) -> Any:
     """
     (data: array float{ball,2}) -> None.
     Set the ball displacement from an array.
     """
     pass
 
+
 def set_extra(*args, **kwargs) -> Any:
     """
     (slot: int, data: array float{ball} or float{ball}) -> None.
     Set the ball extra data in the given slot with an array.
     Extra variables set by array must be of type float or vec.
     """
     pass
 
+
 def set_force_app(*args, **kwargs) -> Any:
     """
     (data: array float{ball,2}) -> None.
     Set the ball applied force from an array.
     """
     pass
 
+
 def set_force_contact(*args, **kwargs) -> Any:
     """
     (data: array float{ball,2}) -> None.
     Set the ball contact force from an array.
     """
     pass
 
+
 def set_group(*args, **kwargs) -> Any:
     """
     (membership: array bool{ball}, group_name: str, slot=1) -> None.
     Set ball group from an array.
     Where membership True set the corresponding ball to be a member of group group_name in the given slot.
     """
     pass
 
+
 def set_moment_app(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Set the ball applied moment from an array.
     """
     pass
 
+
 def set_moment_contact(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Set the ball contact moment from an array.
     """
     pass
 
+
 def set_pos(*args, **kwargs) -> Any:
     """
     (data: array float{ball,2}) -> None.
     Set the ball centroid location from an array.
     """
     pass
 
+
 def set_radius(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Set the ball radii from an array.
     """
     pass
 
+
 def set_rotation(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Set the ball orientation from an array.
     """
     pass
 
+
 def set_spin(*args, **kwargs) -> Any:
     """
     (data: array float{ball}) -> None.
     Set the ball angular velocity from an array.
     """
     pass
 
+
 def set_vel(*args, **kwargs) -> Any:
     """
     (data: array float{ball,2}) -> None.
     Set the ball velocity from an array.
     """
     pass
 
+
 def spin(*args, **kwargs) -> Any:
     """
     () -> array float{ball}.
     Get a numpy array of the ball angular velocity.
     """
     pass
 
+
 def vel(*args, **kwargs) -> Any:
     """
     () -> array float{ball,2}.
     Get a numpy array of the ball velocity.
     """
     pass
-
```

### Comparing `itasca-stub-1.0.8/itasca/ballballarray/__init__.py` & `itasca-stub-1.0.9/itasca/ballballarray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/ballfacetarray/__init__.py` & `itasca-stub-1.0.9/itasca/ballfacetarray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/ballpebblearray/__init__.py` & `itasca-stub-1.0.9/itasca/ballpebblearray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/ballrblockarray/__init__.py` & `itasca-stub-1.0.9/itasca/ballrblockarray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/clump/__init__.py` & `itasca-stub-1.0.9/itasca/clump/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/clump/pebble/__init__.py` & `itasca-stub-1.0.9/itasca/clump/pebble/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/clump/template/__init__.py` & `itasca-stub-1.0.9/itasca/clump/template/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/clump/thermal/__init__.py` & `itasca-stub-1.0.9/itasca/clump/thermal/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/clump/thermal/pebble/__init__.py` & `itasca-stub-1.0.9/itasca/clump/thermal/pebble/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/clumparray/__init__.py` & `itasca-stub-1.0.9/itasca/clumparray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/contact/__init__.py` & `itasca-stub-1.0.9/itasca/contact/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/dfn/__init__.py` & `itasca-stub-1.0.9/itasca/dfn/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/dfn/fracture/__init__.py` & `itasca-stub-1.0.9/itasca/dfn/fracture/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/dfn/inter/__init__.py` & `itasca-stub-1.0.9/itasca/dfn/inter/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/dfn/setinter/__init__.py` & `itasca-stub-1.0.9/itasca/dfn/setinter/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/dfn/template/__init__.py` & `itasca-stub-1.0.9/itasca/dfn/template/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/dfn/vertex/__init__.py` & `itasca-stub-1.0.9/itasca/dfn/vertex/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/facetarray/__init__.py` & `itasca-stub-1.0.9/itasca/facetarray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/fish/__init__.py` & `itasca-stub-1.0.9/itasca/fish/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/measure/__init__.py` & `itasca-stub-1.0.9/itasca/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/pebblearray/__init__.py` & `itasca-stub-1.0.9/itasca/pebblearray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/pebblefacetarray/__init__.py` & `itasca-stub-1.0.9/itasca/pebblefacetarray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/pebblepebblearray/__init__.py` & `itasca-stub-1.0.9/itasca/pebblepebblearray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/pebblerblockarray/__init__.py` & `itasca-stub-1.0.9/itasca/pebblerblockarray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/rblock/__init__.py` & `itasca-stub-1.0.9/itasca/rblock/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/rblock/template/__init__.py` & `itasca-stub-1.0.9/itasca/rblock/template/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/rblockarray/__init__.py` & `itasca-stub-1.0.9/itasca/rblockarray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/rblockfacetarray/__init__.py` & `itasca-stub-1.0.9/itasca/rblockfacetarray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/rblockrblockarray/__init__.py` & `itasca-stub-1.0.9/itasca/rblockrblockarray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/vertexarray/__init__.py` & `itasca-stub-1.0.9/itasca/vertexarray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/wall/__init__.py` & `itasca-stub-1.0.9/itasca/wall/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/wall/facet/__init__.py` & `itasca-stub-1.0.9/itasca/wall/facet/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/wall/thermal/__init__.py` & `itasca-stub-1.0.9/itasca/wall/thermal/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/wall/thermal/facet/__init__.py` & `itasca-stub-1.0.9/itasca/wall/thermal/facet/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/wall/vertex/__init__.py` & `itasca-stub-1.0.9/itasca/wall/vertex/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca/wallarray/__init__.py` & `itasca-stub-1.0.9/itasca/wallarray/__init__.py`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/itasca_stub.egg-info/PKG-INFO` & `itasca-stub-1.0.9/itasca_stub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itasca-stub
-Version: 1.0.8
+Version: 1.0.9
 Summary: Itasca PFC python stub
 Home-page: https://github.com/panhaoyu/itasca-stub
 Author: panhaoyu
 Author-email: panhaoyu.china@outlook.com
 License: MIT
 Download-URL: https://github.com/panhaoyu/itasca-stub/archive/1.0.0.tar.gz
 Description: # itasca-stub
```

### Comparing `itasca-stub-1.0.8/itasca_stub.egg-info/SOURCES.txt` & `itasca-stub-1.0.9/itasca_stub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itasca-stub-1.0.8/setup.py` & `itasca-stub-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='itasca-stub',
     packages=setuptools.find_packages(),
-    version='1.0.8',
+    version='1.0.9',
     license='MIT',
     description='Itasca PFC python stub',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='panhaoyu',
     author_email='panhaoyu.china@outlook.com',
     url='https://github.com/panhaoyu/itasca-stub',
```

