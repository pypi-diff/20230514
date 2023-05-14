# Comparing `tmp/bw_projects-0.1.tar.gz` & `tmp/bw_projects-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bw_projects-0.1.tar", last modified: Tue Nov 12 13:55:53 2019, max compression
+gzip compressed data, was "bw_projects-1.0.0.tar", last modified: Sun May 14 21:12:17 2023, max compression
```

## Comparing `bw_projects-0.1.tar` & `bw_projects-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2019-11-12 13:55:53.000000 bw_projects-0.1/
--rw-r--r--   0 cmutel     (501) staff       (20)     1519 2019-09-04 08:39:07.000000 bw_projects-0.1/LICENSE.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       58 2017-04-12 12:16:26.000000 bw_projects-0.1/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     1584 2019-11-12 13:55:53.000000 bw_projects-0.1/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      702 2019-11-12 09:11:15.000000 bw_projects-0.1/README.md
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2019-11-12 13:55:53.000000 bw_projects-0.1/bw_projects/
--rw-r--r--   0 cmutel     (501) staff       (20)      585 2019-11-12 09:11:15.000000 bw_projects-0.1/bw_projects/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)      850 2019-11-12 09:11:15.000000 bw_projects-0.1/bw_projects/base_dir.py
--rw-r--r--   0 cmutel     (501) staff       (20)      230 2019-11-12 09:11:15.000000 bw_projects-0.1/bw_projects/errors.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1658 2019-11-12 09:11:15.000000 bw_projects-0.1/bw_projects/filesystem.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1705 2019-11-12 09:11:15.000000 bw_projects-0.1/bw_projects/peewee.py
--rw-r--r--   0 cmutel     (501) staff       (20)     6865 2019-11-12 09:11:15.000000 bw_projects-0.1/bw_projects/projects.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1546 2019-11-12 09:11:15.000000 bw_projects-0.1/bw_projects/testing.py
--rw-r--r--   0 cmutel     (501) staff       (20)       17 2019-11-12 13:55:47.000000 bw_projects-0.1/bw_projects/version.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2019-11-12 13:55:53.000000 bw_projects-0.1/bw_projects.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     1584 2019-11-12 13:55:53.000000 bw_projects-0.1/bw_projects.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      404 2019-11-12 13:55:53.000000 bw_projects-0.1/bw_projects.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2019-11-12 13:55:53.000000 bw_projects-0.1/bw_projects.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       15 2019-11-12 13:55:53.000000 bw_projects-0.1/bw_projects.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       12 2019-11-12 13:55:53.000000 bw_projects-0.1/bw_projects.egg-info/top_level.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       38 2019-11-12 13:55:53.000000 bw_projects-0.1/setup.cfg
--rw-r--r--   0 cmutel     (501) staff       (20)     1363 2019-11-12 13:55:26.000000 bw_projects-0.1/setup.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-14 21:12:17.415771 bw_projects-1.0.0/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1268 2023-05-14 20:49:30.000000 bw_projects-1.0.0/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)       28 2023-05-14 20:49:30.000000 bw_projects-1.0.0/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6233 2023-05-14 21:12:17.415857 bw_projects-1.0.0/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5204 2023-05-14 20:57:37.000000 bw_projects-1.0.0/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-14 21:12:17.414684 bw_projects-1.0.0/bw_projects/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-05-14 20:49:30.000000 bw_projects-1.0.0/bw_projects/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      870 2023-05-14 20:49:30.000000 bw_projects-1.0.0/bw_projects/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      898 2023-05-14 20:49:30.000000 bw_projects-1.0.0/bw_projects/config.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5191 2023-05-14 20:49:30.000000 bw_projects-1.0.0/bw_projects/core.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      228 2023-05-14 20:49:30.000000 bw_projects-1.0.0/bw_projects/errors.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3165 2023-05-14 20:49:30.000000 bw_projects-1.0.0/bw_projects/helpers.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      819 2023-05-14 20:49:30.000000 bw_projects-1.0.0/bw_projects/model.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-14 21:12:17.415387 bw_projects-1.0.0/bw_projects.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6233 2023-05-14 21:12:17.000000 bw_projects-1.0.0/bw_projects.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)      465 2023-05-14 21:12:17.000000 bw_projects-1.0.0/bw_projects.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-05-14 21:12:17.000000 bw_projects-1.0.0/bw_projects.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-05-14 21:12:17.000000 bw_projects-1.0.0/bw_projects.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      153 2023-05-14 21:12:17.000000 bw_projects-1.0.0/bw_projects.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       17 2023-05-14 21:12:17.000000 bw_projects-1.0.0/bw_projects.egg-info/top_level.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-05-14 20:49:30.000000 bw_projects-1.0.0/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1700 2023-05-14 21:12:17.416238 bw_projects-1.0.0/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-14 21:12:17.415649 bw_projects-1.0.0/tests/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7772 2023-05-14 20:49:30.000000 bw_projects-1.0.0/tests/test_core.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      530 2023-05-14 20:49:30.000000 bw_projects-1.0.0/tests/test_model.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bw_projects-0.1/LICENSE.txt` & `bw_projects-1.0.0/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-Copyright (c) 2017, Chris Mutel and Paul Scherrer Institut
-All rights reserved.
+Copyright 2023, Mina Sami.
 
-Redistribution and use in source and binary forms, with or without 
-modification, are permitted provided that the following conditions are met:
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
 
-Redistributions of source code must retain the above copyright notice, this 
-list of conditions and the following disclaimer. Redistributions in binary 
-form must reproduce the above copyright notice, this list of conditions and the 
-following disclaimer in the documentation and/or other materials provided 
-with the distribution.
-Neither the name of the Paul Scherrer Institut nor the names of its contributors 
-may be used to endorse or promote products derived from this software without 
-specific prior written permission.
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" 
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE 
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE 
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE 
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL 
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR 
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER 
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, 
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE 
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+1. Redistributions of source code must retain the above copyright notice, this list
+of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this
+list of conditions and the following disclaimer in the documentation and/or other
+materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY
+EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES
+OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT
+SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
+INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED
+TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
+BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
+IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGE.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

