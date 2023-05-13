# Comparing `tmp/dan-build-0.1.0.tar.gz` & `tmp/dan-build-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dan-build-0.1.0.tar", last modified: Sat May 13 15:56:44 2023, max compression
+gzip compressed data, was "dan-build-0.1.1.tar", last modified: Sat May 13 23:52:19 2023, max compression
```

## Comparing `dan-build-0.1.0.tar` & `dan-build-0.1.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.134903 dan-build-0.1.0/
--rw-rw-rw-   0        0        0     1092 2023-05-13 13:14:52.000000 dan-build-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2360 2023-05-13 15:56:44.134903 dan-build-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-05-13 15:47:33.000000 dan-build-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.027891 dan-build-0.1.0/dan/
--rw-rw-rw-   0        0        0      365 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/__init__.py
--rw-rw-rw-   0        0        0       65 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/__main__.py
--rw-rw-rw-   0        0        0    11785 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.030869 dan-build-0.1.0/dan/cmake/
--rw-rw-rw-   0        0        0       51 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cmake/__init__.py
--rw-rw-rw-   0        0        0     1886 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cmake/configure_file.py
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.033860 dan-build-0.1.0/dan/conan/
--rw-rw-rw-   0        0        0       34 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/conan/__init__.py
--rw-rw-rw-   0        0        0     3135 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/conan/requirements.py
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.069373 dan-build-0.1.0/dan/core/
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/__init__.py
--rw-rw-rw-   0        0        0      933 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/aiofiles.py
--rw-rw-rw-   0        0        0     9952 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/asyncio.py
--rw-rw-rw-   0        0        0     2986 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/cache.py
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/detect.py
--rw-rw-rw-   0        0        0      100 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/errors.py
--rw-rw-rw-   0        0        0     1951 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/find.py
--rw-rw-rw-   0        0        0     1053 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/functools.py
--rw-rw-rw-   0        0        0     1063 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/generator.py
--rw-rw-rw-   0        0        0     5223 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/include.py
--rw-rw-rw-   0        0        0     4693 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/makefile.py
--rw-rw-rw-   0        0        0    14158 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/osinfo.py
--rw-rw-rw-   0        0        0      814 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/pathlib.py
--rw-rw-rw-   0        0        0     1100 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/pm.py
--rw-rw-rw-   0        0        0      602 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/register.py
--rw-rw-rw-   0        0        0     3698 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/requirements.py
--rw-rw-rw-   0        0        0     5733 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/runners.py
--rw-rw-rw-   0        0        0     2322 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/settings.py
--rw-rw-rw-   0        0        0    15359 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/target.py
--rw-rw-rw-   0        0        0     4634 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/test.py
--rw-rw-rw-   0        0        0     1672 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/utils.py
--rw-rw-rw-   0        0        0     3821 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/version.py
--rw-rw-rw-   0        0        0     3407 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/core/win.py
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.083299 dan-build-0.1.0/dan/cxx/
--rw-rw-rw-   0        0        0     2681 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cxx/__init__.py
--rw-rw-rw-   0        0        0     1395 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cxx/compile_commands.py
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.089285 dan-build-0.1.0/dan/cxx/data/
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cxx/data/__init__.py
--rwxrwxrwx   0        0        0       29 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cxx/data/detect.cmd
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cxx/data/empty.c
--rw-rw-rw-   0        0        0    21033 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cxx/detect.py
--rw-rw-rw-   0        0        0     5974 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cxx/msvc_toolchain.py
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.093274 dan-build-0.1.0/dan/cxx/support/
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cxx/support/__init__.py
--rw-rw-rw-   0        0        0     3524 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cxx/support/qt.py
--rw-rw-rw-   0        0        0    17233 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cxx/targets.py
--rw-rw-rw-   0        0        0     7265 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cxx/toolchain.py
--rw-rw-rw-   0        0        0     6509 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/cxx/unix_toolchain.py
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.099257 dan-build-0.1.0/dan/io/
--rw-rw-rw-   0        0        0       35 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/io/__init__.py
--rw-rw-rw-   0        0        0     4816 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/io/package.py
--rw-rw-rw-   0        0        0     1392 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/io/repositories.py
--rw-rw-rw-   0        0        0     1679 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/jinja.py
--rw-rw-rw-   0        0        0     4023 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/logging.py
--rw-rw-rw-   0        0        0    15672 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/make.py
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.103247 dan-build-0.1.0/dan/pkgconfig/
--rw-rw-rw-   0        0        0       71 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/pkgconfig/__init__.py
--rw-rw-rw-   0        0        0     9345 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/pkgconfig/package.py
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.107249 dan-build-0.1.0/dan/pkgconfig/templates/
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/pkgconfig/templates/__init__.py
--rw-rw-rw-   0        0        0      429 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/pkgconfig/templates/pkg.pc.jinja2
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.111225 dan-build-0.1.0/dan/smc/
--rw-rw-rw-   0        0        0       56 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/smc/__init__.py
--rw-rw-rw-   0        0        0     1851 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/smc/git.py
--rw-rw-rw-   0        0        0     1071 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/smc/tar.py
--rw-rw-rw-   0        0        0       37 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/testing.py
--rw-rw-rw-   0        0        0     6360 2023-05-13 15:47:33.000000 dan-build-0.1.0/dan/vscode.py
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.128180 dan-build-0.1.0/dan_build.egg-info/
--rw-rw-rw-   0        0        0     2360 2023-05-13 15:56:43.000000 dan-build-0.1.0/dan_build.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1488 2023-05-13 15:56:43.000000 dan-build-0.1.0/dan_build.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 15:56:43.000000 dan-build-0.1.0/dan_build.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-13 15:56:43.000000 dan-build-0.1.0/dan_build.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      102 2023-05-13 15:56:43.000000 dan-build-0.1.0/dan_build.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-13 15:56:43.000000 dan-build-0.1.0/dan_build.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1222 2023-05-13 15:56:37.000000 dan-build-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 15:56:44.134903 dan-build-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-13 15:56:44.132168 dan-build-0.1.0/tests/
--rw-rw-rw-   0        0        0     3114 2023-05-13 15:47:33.000000 dan-build-0.1.0/tests/test_cxx_libraries.py
--rw-rw-rw-   0        0        0     2950 2023-05-13 15:47:33.000000 dan-build-0.1.0/tests/test_cxx_simple.py
--rw-rw-rw-   0        0        0     2268 2023-05-13 13:04:49.000000 dan-build-0.1.0/tests/test_cxx_smc_catch2.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.531222 dan-build-0.1.1/
+-rw-rw-rw-   0        0        0     1092 2023-05-13 13:14:52.000000 dan-build-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2358 2023-05-13 23:52:19.530225 dan-build-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1828 2023-05-13 16:18:25.000000 dan-build-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.445451 dan-build-0.1.1/dan/
+-rw-rw-rw-   0        0        0      365 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/__init__.py
+-rw-rw-rw-   0        0        0       65 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/__main__.py
+-rw-rw-rw-   0        0        0    11767 2023-05-13 16:18:25.000000 dan-build-0.1.1/dan/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.448443 dan-build-0.1.1/dan/cmake/
+-rw-rw-rw-   0        0        0       51 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cmake/__init__.py
+-rw-rw-rw-   0        0        0     1886 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cmake/configure_file.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.452434 dan-build-0.1.1/dan/conan/
+-rw-rw-rw-   0        0        0       34 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/conan/__init__.py
+-rw-rw-rw-   0        0        0     3135 2023-05-13 16:29:34.000000 dan-build-0.1.1/dan/conan/requirements.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.487339 dan-build-0.1.1/dan/core/
+-rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/__init__.py
+-rw-rw-rw-   0        0        0      933 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/aiofiles.py
+-rw-rw-rw-   0        0        0     9952 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/asyncio.py
+-rw-rw-rw-   0        0        0     2986 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/cache.py
+-rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/detect.py
+-rw-rw-rw-   0        0        0      100 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/errors.py
+-rw-rw-rw-   0        0        0     1951 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/find.py
+-rw-rw-rw-   0        0        0     1053 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/functools.py
+-rw-rw-rw-   0        0        0     1063 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/generator.py
+-rw-rw-rw-   0        0        0     5226 2023-05-13 23:45:04.000000 dan-build-0.1.1/dan/core/include.py
+-rw-rw-rw-   0        0        0     4693 2023-05-13 23:45:04.000000 dan-build-0.1.1/dan/core/makefile.py
+-rw-rw-rw-   0        0        0    14158 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/osinfo.py
+-rw-rw-rw-   0        0        0      814 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/pathlib.py
+-rw-rw-rw-   0        0        0     1100 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/pm.py
+-rw-rw-rw-   0        0        0      602 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/register.py
+-rw-rw-rw-   0        0        0     3698 2023-05-13 16:29:34.000000 dan-build-0.1.1/dan/core/requirements.py
+-rw-rw-rw-   0        0        0     5733 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/runners.py
+-rw-rw-rw-   0        0        0     2322 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/settings.py
+-rw-rw-rw-   0        0        0    15359 2023-05-13 23:34:02.000000 dan-build-0.1.1/dan/core/target.py
+-rw-rw-rw-   0        0        0     4634 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/test.py
+-rw-rw-rw-   0        0        0     1672 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/utils.py
+-rw-rw-rw-   0        0        0     3821 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/version.py
+-rw-rw-rw-   0        0        0     3407 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/win.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.496315 dan-build-0.1.1/dan/cxx/
+-rw-rw-rw-   0        0        0     2678 2023-05-13 16:18:25.000000 dan-build-0.1.1/dan/cxx/__init__.py
+-rw-rw-rw-   0        0        0     1395 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/compile_commands.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.500304 dan-build-0.1.1/dan/cxx/data/
+-rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/data/__init__.py
+-rwxrwxrwx   0        0        0       29 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/data/detect.cmd
+-rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/data/empty.c
+-rw-rw-rw-   0        0        0    21030 2023-05-13 16:18:25.000000 dan-build-0.1.1/dan/cxx/detect.py
+-rw-rw-rw-   0        0        0     5974 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/msvc_toolchain.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.502301 dan-build-0.1.1/dan/cxx/support/
+-rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/support/__init__.py
+-rw-rw-rw-   0        0        0     3524 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/support/qt.py
+-rw-rw-rw-   0        0        0    17233 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/targets.py
+-rw-rw-rw-   0        0        0     7265 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/toolchain.py
+-rw-rw-rw-   0        0        0     6509 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/unix_toolchain.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.506288 dan-build-0.1.1/dan/io/
+-rw-rw-rw-   0        0        0       35 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/io/__init__.py
+-rw-rw-rw-   0        0        0     4824 2023-05-13 23:45:04.000000 dan-build-0.1.1/dan/io/package.py
+-rw-rw-rw-   0        0        0     1392 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/io/repositories.py
+-rw-rw-rw-   0        0        0     1679 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/jinja.py
+-rw-rw-rw-   0        0        0     4023 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/logging.py
+-rw-rw-rw-   0        0        0    15674 2023-05-13 23:45:04.000000 dan-build-0.1.1/dan/make.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.509292 dan-build-0.1.1/dan/pkgconfig/
+-rw-rw-rw-   0        0        0       71 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/pkgconfig/__init__.py
+-rw-rw-rw-   0        0        0     9345 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/pkgconfig/package.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.511275 dan-build-0.1.1/dan/pkgconfig/templates/
+-rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/pkgconfig/templates/__init__.py
+-rw-rw-rw-   0        0        0      429 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/pkgconfig/templates/pkg.pc.jinja2
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.515265 dan-build-0.1.1/dan/smc/
+-rw-rw-rw-   0        0        0       56 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/smc/__init__.py
+-rw-rw-rw-   0        0        0     1851 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/smc/git.py
+-rw-rw-rw-   0        0        0     1071 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/smc/tar.py
+-rw-rw-rw-   0        0        0       37 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/testing.py
+-rw-rw-rw-   0        0        0     6360 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/vscode.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.524242 dan-build-0.1.1/dan_build.egg-info/
+-rw-rw-rw-   0        0        0     2358 2023-05-13 23:52:19.000000 dan-build-0.1.1/dan_build.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1488 2023-05-13 23:52:19.000000 dan-build-0.1.1/dan_build.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-13 23:52:19.000000 dan-build-0.1.1/dan_build.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-13 23:52:19.000000 dan-build-0.1.1/dan_build.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      102 2023-05-13 23:52:19.000000 dan-build-0.1.1/dan_build.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-13 23:52:19.000000 dan-build-0.1.1/dan_build.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1222 2023-05-13 23:51:29.000000 dan-build-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-13 23:52:19.531222 dan-build-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.528230 dan-build-0.1.1/tests/
+-rw-rw-rw-   0        0        0     3114 2023-05-13 15:47:33.000000 dan-build-0.1.1/tests/test_cxx_libraries.py
+-rw-rw-rw-   0        0        0     2950 2023-05-13 15:47:33.000000 dan-build-0.1.1/tests/test_cxx_simple.py
+-rw-rw-rw-   0        0        0     2268 2023-05-13 13:04:49.000000 dan-build-0.1.1/tests/test_cxx_smc_catch2.py
```

### Comparing `dan-build-0.1.0/LICENSE` & `dan-build-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/PKG-INFO` & `dan-build-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 Project-URL: homepage, https://github.com/Garcia6L20/dan
 Project-URL: documentation, https://github.com/Garcia6L20/dan
 Project-URL: repository, https://github.com/Garcia6L20/dan
 Keywords: packaging,dependency,build system
 Classifier: Topic :: Software Development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dan
-> Makefiles - in python
+
+> _Do Anything Now_
 
 _dan_ is a build system inspired from _GNU make_, _cmake_, _meson_, ... but only in python.
 
 ## Features
 
 - Generators:
```

### Comparing `dan-build-0.1.0/README.md` & `dan-build-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # dan
-> Makefiles - in python
+
+> _Do Anything Now_
 
 _dan_ is a build system inspired from _GNU make_, _cmake_, _meson_, ... but only in python.
 
 ## Features
 
 - Generators:
```

### Comparing `dan-build-0.1.0/dan/cli.py` & `dan-build-0.1.1/dan/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,28 +31,28 @@
 click.BaseCommand.context_class = AsyncContext
 
 
 _logger = logging.getLogger('cli')
 
 _minimal_options = [
     click.option('--build-path', '-B', 'path', help='Path where dan has been initialized.',
-                 type=click.Path(resolve_path=True, path_type=Path), required=True, default='build', envvar='PYMAKE_BUILD_PATH'),
+                 type=click.Path(resolve_path=True, path_type=Path), required=True, default='build', envvar='DAN_BUILD_PATH'),
 
 ]
 
 _common_opts = [
     *_minimal_options,
     click.option('--quiet', '-q', is_flag=True,
-                 help='Dont print informations (errors only).', envvar='PYMAKE_QUIET'),
+                 help='Dont print informations (errors only).', envvar='DAN_QUIET'),
     click.option('--verbose', '-v', is_flag=True,
-                 help='Pring debug informations.', envvar='PYMAKE_VERBOSE'),
+                 help='Pring debug informations.', envvar='DAN_VERBOSE'),
     click.option('--jobs', '-j',
-                 help='Maximum jobs.', default=None, type=int, envvar='PYMAKE_JOBS'),
+                 help='Maximum jobs.', default=None, type=int, envvar='DAN_JOBS'),
     click.option('--no-progress', is_flag=True,
-                 help='Disable progress bars', envvar='PYMAKE_NOPROGRESS'),
+                 help='Disable progress bars', envvar='DAN_NOPROGRESS'),
     click.argument('TARGETS', nargs=-1),
 ]
 _base_help_ = '''
   PATH          Either build or source directory.
   [TARGETS...]  Targets to process.
 '''
 
@@ -378,15 +378,15 @@
 def process_result(result, **kwargs):
     asyncio.run(Cache.save_all())
 
 
 def main():
     import sys
     try:
-        cli(auto_envvar_prefix='PYMAKE')
+        cli(auto_envvar_prefix='DAN')
     except Exception as err:
         _logger.error(str(err))
         _ex_type, _ex, tb = sys.exc_info()
         import traceback
         _logger.debug(' '.join(traceback.format_tb(tb)))
         try:
             # wait asyncio loop to terminate
```

### Comparing `dan-build-0.1.0/dan/cmake/configure_file.py` & `dan-build-0.1.1/dan/cmake/configure_file.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/conan/requirements.py` & `dan-build-0.1.1/dan/conan/requirements.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/aiofiles.py` & `dan-build-0.1.1/dan/core/aiofiles.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/asyncio.py` & `dan-build-0.1.1/dan/core/asyncio.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/cache.py` & `dan-build-0.1.1/dan/core/cache.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/find.py` & `dan-build-0.1.1/dan/core/find.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/functools.py` & `dan-build-0.1.1/dan/core/functools.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/generator.py` & `dan-build-0.1.1/dan/core/generator.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/include.py` & `dan-build-0.1.1/dan/core/include.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,39 +125,39 @@
 def include_makefile(name: str | Path, build_path: Path = None) -> set[Target]:
     ''' Include a sub-directory (or a sub-makefile).
     :returns: The set of exported targets.
     '''
     global context
     if not context.root:
         assert type(name) == type(Path())
-        module_path: Path = name / 'makefile.py'
+        module_path: Path = name / 'dan-build.py'
         spec = importlib.util.spec_from_file_location(
             'root', module_path)
         name = 'root'
     else:
         lookups = [
-            os.path.join(name, 'makefile.py'),
+            os.path.join(name, 'dan-build.py'),
             f'{name}.py',
         ]
         for lookup in lookups:
             module_path = context.current.source_path / lookup
             if module_path.exists():
                 spec = importlib.util.spec_from_file_location(
                     f'{context.current.name}.{name}', module_path)
                 break
         else:
             raise RuntimeError(
                 f'Cannot find anything to include for "{name}" (looked for: {", ".join(lookups)})')
     module = importlib.util.module_from_spec(spec)
     _init_makefile(module, name, build_path)
 
-    requirements_file = module_path.with_stem('requirements')
-    if module_path.stem == 'makefile' and requirements_file.exists():
+    requirements_file = module_path.with_stem('dan-requires')
+    if module_path.stem == 'dan-build' and requirements_file.exists():
         context.current.requirements = load_makefile(
-            requirements_file, name='requirements', module_name=f'{name}.requirements')
+            requirements_file, name='dan-requires', module_name=f'{name}.requirements')
 
     try:
         spec.loader.exec_module(module)
     except TargetNotFound as err:
         if len(context.missing) == 0:
             raise err
     context.up()
```

### Comparing `dan-build-0.1.0/dan/core/makefile.py` & `dan-build-0.1.1/dan/core/makefile.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.source_path = source_path
         self.build_path = build_path
         self.__requirements = requirements
         self.parent: MakeFile = self.parent if hasattr(
             self, 'parent') else None
         self.__cache: Cache = None
         self.children: list[MakeFile] = list()
-        if self.name != 'requirements' and self.parent:
+        if self.name != 'dan-requires' and self.parent:
             self.parent.children.append(self)
         self.options = Options(self)
         self.__targets: set[Target] = set()
         self.__tests: set[Test] = set()
 
     @property
     def fullname(self):
@@ -84,15 +84,15 @@
                 return t
     
     def __getitem__(self, name_or_class) -> Target:
         return self.find(name_or_class)
 
     @property
     def requirements(self):
-        if self.name == 'requirements':
+        if self.name == 'dan-requires':
             return self
         if self.__requirements is not None:
             return self.__requirements
         elif self.parent is not None:
             return self.parent.requirements
 
     @property
```

### Comparing `dan-build-0.1.0/dan/core/osinfo.py` & `dan-build-0.1.1/dan/core/osinfo.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/pathlib.py` & `dan-build-0.1.1/dan/core/pathlib.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/pm.py` & `dan-build-0.1.1/dan/core/pm.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/register.py` & `dan-build-0.1.1/dan/core/register.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/requirements.py` & `dan-build-0.1.1/dan/core/requirements.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/runners.py` & `dan-build-0.1.1/dan/core/runners.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/settings.py` & `dan-build-0.1.1/dan/core/settings.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/target.py` & `dan-build-0.1.1/dan/core/target.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/test.py` & `dan-build-0.1.1/dan/core/test.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/utils.py` & `dan-build-0.1.1/dan/core/utils.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/version.py` & `dan-build-0.1.1/dan/core/version.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/core/win.py` & `dan-build-0.1.1/dan/core/win.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/cxx/__init__.py` & `dan-build-0.1.1/dan/cxx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,13 +79,13 @@
         try:
             return sys.argv[sys.argv.index(name) + 1]
         except ValueError:
             continue
     return default
 
 #def __init_toolchains():
-#    init_toolchains(__pick_arg('-t', '--toolchain', env='PYMAKE_TOOLCHAIN'))
+#    init_toolchains(__pick_arg('-t', '--toolchain', env='DAN_TOOLCHAIN'))
 
 #__init_toolchains()
 
 from .targets import Executable, Library, LibraryType, Module
 from .targets import CXXObjectsTarget as Objects
```

### Comparing `dan-build-0.1.0/dan/cxx/compile_commands.py` & `dan-build-0.1.1/dan/cxx/compile_commands.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/cxx/detect.py` & `dan-build-0.1.1/dan/cxx/detect.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,15 +478,15 @@
 
 
 _home_var = 'USERPROFILE' if os.name == 'nt' else 'HOME'
 
 
 @functools.cache
 def get_dan_path():
-    path = Path(os.getenv('PYMAKE_DATA', os.getenv(_home_var))) / '.dan'
+    path = Path(os.getenv('DAN_DATA', os.getenv(_home_var))) / '.dan'
     path.mkdir(exist_ok=True, parents=False)
     return path
 
 
 def get_toolchain_path():
     return get_dan_path() / 'toolchains.yaml'
```

### Comparing `dan-build-0.1.0/dan/cxx/msvc_toolchain.py` & `dan-build-0.1.1/dan/cxx/msvc_toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/cxx/support/qt.py` & `dan-build-0.1.1/dan/cxx/support/qt.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/cxx/targets.py` & `dan-build-0.1.1/dan/cxx/targets.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/cxx/toolchain.py` & `dan-build-0.1.1/dan/cxx/toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/cxx/unix_toolchain.py` & `dan-build-0.1.1/dan/cxx/unix_toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/io/package.py` & `dan-build-0.1.1/dan/io/package.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 
 
 class PackageBuild(Target, internal=True):
     
     def __init__(self, name, version, repository, *args, **kwargs):
         packages_path = get_packages_path()
         from dan.cxx import target_toolchain as toolchain
-        build_path = packages_path / toolchain.system / toolchain.arch / toolchain.build_type.name / name / str(version) / 'data'
+        build_path = packages_path / 'dist' / toolchain.system / toolchain.arch / toolchain.build_type.name / name / str(version) / 'data'
         super().__init__(name, *args, build_path=build_path, version=version, **kwargs)
         self.repo = get_repo_instance(repository, self.makefile)
         self.preload_dependencies.add(self.repo)
         self.output = self.build_path.parent
         self.install_settings = InstallSettings(self.output)
         self.sources = GitSources(
             name=f'{self.name}-package-sources',
             url=self.repo.url,
             refspec='main',
-            build_path=build_path,
+            build_path=packages_path / 'src',
             makefile=self.makefile,
-            dirname='package-sources',
+            dirname=name,
             subdirectory=f'packages/{self.name}')
         self.dependencies.add(self.sources)
 
     async def __build__(self):
         from dan.core.include import load_makefile
         root = self.sources.output / 'packages' / self.name
-        if (root / 'requirements.py').exists():
-            requirements = load_makefile(root / 'requirements.py', f'{self.name}-requirements')
+        if (root / 'dan-requires.py').exists():
+            requirements = load_makefile(root / 'dan-requires.py', f'{self.name}-requirements')
         else:
             requirements = None
-        makefile = load_makefile(root / 'makefile.py', self.name, requirements=requirements, build_path=self.build_path)
+        makefile = load_makefile(root / 'dan-build.py', self.name, requirements=requirements, build_path=self.build_path)
         makefile.options.get('version').value = str(self.version)
 
         async with asyncio.TaskGroup(f'installing {self.name}\'s targets') as group:
             for target in makefile.all_installed:
                 group.create_task(target.install(self.install_settings, InstallMode.dev))
 
         makefile.cache.ignore()
```

### Comparing `dan-build-0.1.0/dan/io/repositories.py` & `dan-build-0.1.1/dan/io/repositories.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/jinja.py` & `dan-build-0.1.1/dan/jinja.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/logging.py` & `dan-build-0.1.1/dan/logging.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/make.py` & `dan-build-0.1.1/dan/make.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         logging.getLogger().setLevel(log_level)
 
         super().__init__('make')
 
         self.no_progress = no_progress
         self.for_install = for_install
         path = Path(path)
-        if not path.exists() or not (path / 'makefile.py').exists():
+        if not path.exists() or not (path / 'dan-build.py').exists():
             self.source_path = Path.cwd().absolute()
             self.build_path = path.absolute().resolve()
         else:
             self.source_path = path.absolute().resolve()
             self.build_path = Path.cwd().absolute()
 
         self.config_path = self.build_path / self._config_name
@@ -98,15 +98,15 @@
         #     'source_path', self.source_path))
 
         self.debug(f'source path: {self.source_path}')
         self.debug(f'build path: {self.build_path}')
         self.debug(f'jobs: {jobs}')
 
         assert (self.source_path /
-                'makefile.py').exists(), f'no makefile in {self.source_path}'
+                'dan-build.py').exists(), f'no makefile in {self.source_path}'
         assert (self.source_path !=
                 self.build_path), f'in-source build are not allowed'
         
     @property
     def config(self) -> Config:
         return self._config.data
```

### Comparing `dan-build-0.1.0/dan/pkgconfig/package.py` & `dan-build-0.1.1/dan/pkgconfig/package.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/smc/git.py` & `dan-build-0.1.1/dan/smc/git.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/smc/tar.py` & `dan-build-0.1.1/dan/smc/tar.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan/vscode.py` & `dan-build-0.1.1/dan/vscode.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/dan_build.egg-info/PKG-INFO` & `dan-build-0.1.1/dan_build.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 Project-URL: homepage, https://github.com/Garcia6L20/dan
 Project-URL: documentation, https://github.com/Garcia6L20/dan
 Project-URL: repository, https://github.com/Garcia6L20/dan
 Keywords: packaging,dependency,build system
 Classifier: Topic :: Software Development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dan
-> Makefiles - in python
+
+> _Do Anything Now_
 
 _dan_ is a build system inspired from _GNU make_, _cmake_, _meson_, ... but only in python.
 
 ## Features
 
 - Generators:
```

### Comparing `dan-build-0.1.0/dan_build.egg-info/SOURCES.txt` & `dan-build-0.1.1/dan_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/pyproject.toml` & `dan-build-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dan-build"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python-based build system."
 authors = [
     {name = "Garcia Sylvain", email="garcia.6l20@gmail.com"},
     {email = "garcia.6l20@gmail.com"}
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
```

### Comparing `dan-build-0.1.0/tests/test_cxx_libraries.py` & `dan-build-0.1.1/tests/test_cxx_libraries.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/tests/test_cxx_simple.py` & `dan-build-0.1.1/tests/test_cxx_simple.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.0/tests/test_cxx_smc_catch2.py` & `dan-build-0.1.1/tests/test_cxx_smc_catch2.py`

 * *Files identical despite different names*

