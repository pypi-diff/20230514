# Comparing `tmp/guppy3-3.1.2.tar.gz` & `tmp/guppy3-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/guppy3-3.1.2.tar", last modified: Fri Oct  8 17:32:25 2021, max compression
+gzip compressed data, was "guppy3-3.1.3.tar", last modified: Sat May 13 23:14:01 2023, max compression
```

## Comparing `guppy3-3.1.2.tar` & `guppy3-3.1.3.tar`

### file list

```diff
@@ -1,136 +1,138 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-08 17:32:25.000000 guppy3-3.1.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)    31823 2021-10-08 17:32:22.000000 guppy3-3.1.2/ChangeLog
--rw-rw-r--   0 travis    (2000) travis    (2000)       62 2021-10-08 17:32:22.000000 guppy3-3.1.2/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-08 17:32:25.000000 guppy3-3.1.2/guppy3.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6744 2021-10-08 17:32:25.000000 guppy3-3.1.2/guppy3.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-10-08 17:32:25.000000 guppy3-3.1.2/guppy3.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-10-08 17:32:25.000000 guppy3-3.1.2/guppy3.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2746 2021-10-08 17:32:25.000000 guppy3-3.1.2/guppy3.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6744 2021-10-08 17:32:25.000000 guppy3-3.1.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     5063 2021-10-08 17:32:22.000000 guppy3-3.1.2/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-08 17:32:25.000000 guppy3-3.1.2/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-08 17:32:25.000000 guppy3-3.1.2/src/include/
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/include/guppy.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-08 17:32:25.000000 guppy3-3.1.2/src/sets/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3539 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/sets/bitset.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3282 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/sets/sets.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/sets/sets.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1842 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/sets/nodeset.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2419 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/sets/sets_internal.h
--rw-rw-r--   0 travis    (2000) travis    (2000)   119837 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/sets/bitset.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    30112 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/sets/nodeset.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    11033 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/sets/immnodeset.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-08 17:32:25.000000 guppy3-3.1.2/src/heapy/
--rw-rw-r--   0 travis    (2000) travis    (2000)      808 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/hv_cli_id.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     6680 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/hv_cli_dictof.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1334 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/roundupsize.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    52346 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/hv.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2137 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/hv_cli.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2072 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/hv_cli_indisize.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1650 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/impsets.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     7474 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/hv_cli_and.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     6709 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/xmemstats.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1258 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/heapy.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      991 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/classifier.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      990 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/initheapyc.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    13022 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/stdtypes.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1006 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/nodegraph.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    24330 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/rootstate.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5322 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/hv_cli_prod.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4535 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/hv_cli_rcs.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     8619 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/classifier.c
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/hpinit.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4360 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/hv_cli_findex.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     8358 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/interpreter.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     7169 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/heapyc.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    25298 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/nodegraph.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2351 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/hv_cli_user.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      972 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/hv_cli_idset.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    10046 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/hv_cli_rel.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/stdtypes.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      222 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/relation.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3253 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/heapdef.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5963 2021-10-08 17:32:22.000000 guppy3-3.1.2/src/heapy/horizon.c
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-10-08 17:32:25.000000 guppy3-3.1.2/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-08 17:32:25.000000 guppy3-3.1.2/guppy/
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-08 17:32:25.000000 guppy3-3.1.2/guppy/etc/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1056 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/Code.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24154 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/RE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4088 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/Cat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      903 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/Descriptor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2273 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/IterPermute.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13871 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/Glue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9023 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/KnuthBendix.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2177 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/tkcursors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1697 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/etc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3146 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/textView.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15070 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7376 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/FSA.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2365 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/xterm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6873 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/Help.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21205 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/KanExtension.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10635 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/etc/RE_Rect.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1065 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-08 17:32:25.000000 guppy3-3.1.2/guppy/sets/
--rw-rw-r--   0 travis    (2000) travis    (2000)    46597 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/sets/test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1578 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/sets/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-08 17:32:25.000000 guppy3-3.1.2/guppy/gsl/
--rw-rw-r--   0 travis    (2000) travis    (2000)    68513 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/Main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      402 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/Exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8791 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/DottedTree.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    58933 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/Document.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18819 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/XHTML.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18920 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/SpecNodes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25761 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/Latex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17879 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/Html.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31882 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/Text.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3926 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/Filer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1018 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/Help.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2757 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/Gsml.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2658 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/FileIO.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24566 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/gsl/Tester.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-08 17:32:25.000000 guppy3-3.1.2/guppy/heapy/
--rw-rw-r--   0 travis    (2000) travis    (2000)      843 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/Console.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14849 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/Monitor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15678 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/Remote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23601 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/Use.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/Target.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7996 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/Doc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    49755 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/Spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11792 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/OutputHandling.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68009 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/UniSet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23808 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/Part.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14365 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/Path.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92556 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/Prof.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      870 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/ImpSet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18615 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/RefPat.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-10-08 17:32:25.000000 guppy3-3.1.2/guppy/heapy/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)    28155 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_Path.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      682 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_all.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       95 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_RetaGraph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8180 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_View.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10398 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_Part.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1376 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_OutputHandling.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12877 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_ER.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      583 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_sf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15972 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_heapyc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3196 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_menuleak.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16991 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_RefPat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      214 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_dependencies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1241 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_UniSet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_Spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      421 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_gsl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3814 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/support.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29059 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/test/test_Classifiers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      209 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      119 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/RM.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19503 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/View.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      209 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/RemoteConstants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21232 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/pbhelp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46239 2021-10-08 17:32:22.000000 guppy3-3.1.2/guppy/heapy/Classifiers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      691 2021-10-08 17:32:22.000000 guppy3-3.1.2/ANNOUNCE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2527 2021-10-08 17:32:22.000000 guppy3-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:14:01.625823 guppy3-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-13 23:13:45.000000 guppy3-3.1.3/ANNOUNCE
+-rw-r--r--   0 runner    (1001) docker     (123)    32408 2023-05-13 23:13:45.000000 guppy3-3.1.3/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-13 23:13:45.000000 guppy3-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-13 23:13:45.000000 guppy3-3.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-13 23:14:01.625823 guppy3-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-13 23:13:45.000000 guppy3-3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:14:01.609823 guppy3-3.1.3/guppy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:14:01.613823 guppy3-3.1.3/guppy/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/Cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/Code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/Descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/FSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/Glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/Help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/IterPermute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21205 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/KanExtension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/KnuthBendix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24154 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/RE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/RE_Rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/etc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/textView.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/tkcursors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/etc/xterm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:14:01.613823 guppy3-3.1.3/guppy/gsl/
+-rw-r--r--   0 runner    (1001) docker     (123)    58933 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/Document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/DottedTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/FileIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/Filer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/Gsml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/Help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17879 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/Html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25761 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/Latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68513 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/Main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/SpecNodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24566 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/Tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31882 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/Text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18819 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/XHTML.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/gsl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:14:01.617823 guppy3-3.1.3/guppy/heapy/
+-rw-r--r--   0 runner    (1001) docker     (123)    46239 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/Classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/Console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/Doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/ImpSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/Monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/OutputHandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/Part.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/Path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92546 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/Prof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/RM.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18615 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/RefPat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/Remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/RemoteConstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49755 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/Spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/Target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68096 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/UniSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/Use.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/View.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/pbhelp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:14:01.621823 guppy3-3.1.3/guppy/heapy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29059 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_Classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_ER.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_OutputHandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_Part.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29516 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_Path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_RefPat.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_RetaGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_Spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_UniSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_View.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_gsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_heapyc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_menuleak.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/heapy/test/test_sf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:14:01.621823 guppy3-3.1.3/guppy/sets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46597 2023-05-13 23:13:45.000000 guppy3-3.1.3/guppy/sets/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:14:01.621823 guppy3-3.1.3/guppy3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-13 23:14:01.000000 guppy3-3.1.3/guppy3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-13 23:14:01.000000 guppy3-3.1.3/guppy3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 23:14:01.000000 guppy3-3.1.3/guppy3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-13 23:14:01.000000 guppy3-3.1.3/guppy3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 23:14:01.625823 guppy3-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-13 23:13:45.000000 guppy3-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:14:01.609823 guppy3-3.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:14:01.625823 guppy3-3.1.3/src/heapy/
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/classifier.c
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/classifier.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/heapdef.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/heapy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/heapyc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/horizon.c
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/hpinit.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52775 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/hv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/hv_cli.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/hv_cli_and.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/hv_cli_dictof.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/hv_cli_findex.c
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/hv_cli_id.c
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/hv_cli_idset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/hv_cli_indisize.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/hv_cli_prod.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/hv_cli_rcs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/hv_cli_rel.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/hv_cli_user.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/impsets.c
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/initheapyc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/interpreter.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25299 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/nodegraph.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/nodegraph.h
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/relation.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26499 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/rootstate.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/roundupsize.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/stdtypes.c
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/stdtypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/heapy/xmemstats.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:14:01.625823 guppy3-3.1.3/src/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/include/guppy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/include/pythoncapi_compat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:14:01.625823 guppy3-3.1.3/src/sets/
+-rw-r--r--   0 runner    (1001) docker     (123)   119758 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/sets/bitset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/sets/bitset.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/sets/immnodeset.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30224 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/sets/nodeset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/sets/nodeset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/sets/sets.c
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/sets/sets.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-13 23:13:45.000000 guppy3-3.1.3/src/sets/sets_internal.h
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `guppy3-3.1.2/ChangeLog` & `guppy3-3.1.3/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+    Version 3.1.3
+
+2023-05-13  YiFei Zhu  <zhuyifei1999@gmail.com>
+
+    * Python 3.11 support - the traverse will create all the lazily-created
+      frame objects and materialize object managed dicts; this will consume
+      additional memory.
+
+2022-02-12  YiFei Zhu  <zhuyifei1999@gmail.com>
+
+    * Fix profile browser initialization on Python 3.10+
+
+2022-01-05  YiFei Zhu  <zhuyifei1999@gmail.com>
+
+    * Fix crash doing path calculation when a path component is non-compariable
+
+2022-01-04  YiFei Zhu  <zhuyifei1999@gmail.com>
+
+    * Fix crash when a type doesn't have __module__
+
     Version 3.1.2
 
 2021-10-08  YiFei Zhu  <zhuyifei1999@gmail.com>
 
     * Nothing changed, just releasing 3.1.2
 
 2020-10-06  YiFei Zhu  <zhuyifei1999@gmail.com>
```

### Comparing `guppy3-3.1.2/guppy3.egg-info/PKG-INFO` & `guppy3-3.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,141 @@
 Metadata-Version: 2.1
 Name: guppy3
-Version: 3.1.2
+Version: 3.1.3
 Summary: Guppy 3 -- Guppy-PE ported to Python 3
 Home-page: https://github.com/zhuyifei1999/guppy3/
 Author: YiFei Zhu
 Author-email: zhuyifei1999@gmail.com
 License: MIT
-Description: # Guppy 3
-        [![Build Status](https://img.shields.io/travis/com/zhuyifei1999/guppy3?label=tests)](https://travis-ci.com/zhuyifei1999/guppy3) [![Codecov](https://img.shields.io/codecov/c/github/zhuyifei1999/guppy3)](https://codecov.io/gh/zhuyifei1999/guppy3) [![PyPI version](https://img.shields.io/pypi/v/guppy3)](https://pypi.org/project/guppy3/) [![Repology - Repositories](https://img.shields.io/repology/repositories/python:guppy3)](https://repology.org/project/python:guppy3/versions)  
-        [![PyPI - Implementation](https://img.shields.io/pypi/implementation/guppy3)](https://pypi.org/project/guppy3/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/guppy3)](https://pypi.org/project/guppy3/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/guppy3)](https://pypistats.org/packages/guppy3) [![PyPI - License](https://img.shields.io/pypi/l/guppy3)](https://github.com/zhuyifei1999/guppy3/blob/master/LICENSE)
-        
-        A Python Programming Environment & Heap analysis toolset.
-        
-        This package contains the following subpackages:
-        * etc - Support modules. Contains especially the Glue protocol module.
-        * gsl - The Guppy Specification Language implementation. This can be used
-          to create documents and tests from a common source.
-        * heapy - The heap analysis toolset. It can be used to find information about
-          the objects in the heap and display the information in various ways.
-        * sets - Bitsets and 'nodesets' implemented in C.
-        
-        Guppy 3 is a fork of Guppy-PE, created by Sverker Nilsson for Python 2.
-        
-        ## Requirements
-        
-        You should have Python 3.6, 3.7, 3.8, or 3.9. This package is CPython only;
-        PyPy and other Python implementations are not supported. Python 2 support
-        can be obtained from [guppy-pe](http://guppy-pe.sourceforge.net/) by
-        Sverker Nilsson, from which this package is forked.
-        
-        To use the graphical browser, Tkinter is needed.
-        To use the remote monitor, threading must be available.
-        
-        ## Installation
-        
-        Install with pip by:
-        
-        ```
-        pip install guppy3
-        ```
-        
-        Install with conda by:
-        ```
-        conda install -c conda-forge guppy3
-        ```
-        
-        ## Usage
-        
-        The following example shows
-        
-        1. How to create the session context: `h=hpy()`
-        2. How to show the reachable objects in the heap: `h.heap()`
-        4. How to show the shortest paths from the root to the single largest object: `h.heap().byid[0].sp`
-        3. How to create and show a set of objects: `h.iso(1,[],{})`
-        
-        ```python
-        >>> from guppy import hpy; h=hpy()
-        >>> h.heap()
-        Partition of a set of 30976 objects. Total size = 3544220 bytes.
-         Index  Count   %     Size   % Cumulative  % Kind (class / dict of class)
-             0   8292  27   739022  21    739022  21 str
-             1   7834  25   625624  18   1364646  39 tuple
-             2   2079   7   300624   8   1665270  47 types.CodeType
-             3    400   1   297088   8   1962358  55 type
-             4   4168  13   279278   8   2241636  63 bytes
-             5   1869   6   269136   8   2510772  71 function
-             6    400   1   228464   6   2739236  77 dict of type
-             7     79   0   139704   4   2878940  81 dict of module
-             8   1061   3    93368   3   2972308  84 types.WrapperDescriptorType
-             9    172   1    81712   2   3054020  86 dict (no owner)
-        <89 more rows. Type e.g. '_.more' to view.>
-        >>> h.heap().byid[0].sp
-         0: h.Root.i0_modules['os'].__dict__
-        >>> h.iso(1,[],{})
-        Partition of a set of 3 objects. Total size = 348 bytes.
-         Index  Count   %     Size   % Cumulative  % Kind (class / dict of class)
-             0      1  33      248  71       248  71 dict (no owner)
-             1      1  33       72  21       320  92 list
-             2      1  33       28   8       348 100 int
-        >>>
-        ```
-        
-        People have written awesome posts on how to use this toolset, including:
-        * [How to use guppy/heapy for tracking down memory usage](https://smira.ru/wp-content/uploads/2011/08/heapy.html)
-        * [Debugging Django memory leak with TrackRefs and Guppy](https://opensourcehacker.com/2008/03/07/debugging-django-memory-leak-with-trackrefs-and-guppy/)
-        * [Diagnosing Memory "Leaks" in Python](https://chase-seibert.github.io/blog/2013/08/03/diagnosing-memory-leaks-python.html)
-        * [Digging into python memory issues in ckan with heapy](https://leastsignificant.blogspot.com/2015/06/digging-into-python-memory-issues-in.html)
-        
-        Formal and API documentation are [also available](https://zhuyifei1999.github.io/guppy3/).
-        
-        ## Contributing
-        
-        Issues and pull requests are welcome. You may also ask for help on using this
-        toolset; however, in such cases, we will only provide guidance, and not profile
-        your code for you.
-        
-        Please make sure to update tests as appropriate.
-        
-        ### Testing
-        
-        To test if the heapy build and installation was ok, you can do:
-        
-        ```python
-        >>> from guppy import hpy
-        >>> hpy().test()
-        Testing sets
-        Test #0
-        Test #1
-        Test #2
-        ...
-        ```
-        
-        There will be several more tests. Some tests may take a while.
-        
-        ## License
-        
-        Copyright (C) 2005-2013 Sverker Nilsson, S. Nilsson Computer System AB  
-        Copyright (C) 2019-2021 YiFei Zhu
-        
-        The right is granted to copy, use, modify and redistribute this code
-        according to the rules in what is commonly referred to as an MIT
-        license.
-        
-        *** USE AT YOUR OWN RISK AND BE AWARE THAT THIS IS AN EARLY RELEASE ***
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: C
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Guppy 3
+[![Build Status](https://img.shields.io/github/actions/workflow/status/zhuyifei1999/guppy3/workflow.yml?branch=master)](https://github.com/zhuyifei1999/guppy3/actions/workflows/workflow.yml) [![Codecov](https://img.shields.io/codecov/c/github/zhuyifei1999/guppy3)](https://codecov.io/gh/zhuyifei1999/guppy3) [![PyPI version](https://img.shields.io/pypi/v/guppy3)](https://pypi.org/project/guppy3/) [![Repology - Repositories](https://img.shields.io/repology/repositories/python:guppy3)](https://repology.org/project/python:guppy3/versions)  
+[![PyPI - Implementation](https://img.shields.io/pypi/implementation/guppy3)](https://pypi.org/project/guppy3/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/guppy3)](https://pypi.org/project/guppy3/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/guppy3)](https://pypistats.org/packages/guppy3) [![PyPI - License](https://img.shields.io/pypi/l/guppy3)](https://github.com/zhuyifei1999/guppy3/blob/master/LICENSE)
+
+A Python Programming Environment & Heap analysis toolset.
+
+This package contains the following subpackages:
+* etc - Support modules. Contains especially the Glue protocol module.
+* gsl - The Guppy Specification Language implementation. This can be used
+  to create documents and tests from a common source.
+* heapy - The heap analysis toolset. It can be used to find information about
+  the objects in the heap and display the information in various ways.
+* sets - Bitsets and 'nodesets' implemented in C.
+
+Guppy 3 is a fork of Guppy-PE, created by Sverker Nilsson for Python 2.
+
+## Requirements
+
+You should have Python 3.7, 3.8, 3.9, 3.10, or 3.11. This package is CPython
+only; PyPy and other Python implementations are not supported. Python 2 support
+can be obtained from [guppy-pe](http://guppy-pe.sourceforge.net/) by
+Sverker Nilsson, from which this package is forked.
+
+To use the graphical browser, Tkinter is needed.
+To use the remote monitor, threading must be available.
+
+## Installation
+
+Install with pip by:
+
+```
+pip install guppy3
+```
+
+Install with conda by:
+```
+conda install -c conda-forge guppy3
+```
+
+## Usage
+
+The following example shows
+
+1. How to create the session context: `h=hpy()`
+2. How to show the reachable objects in the heap: `h.heap()`
+4. How to show the shortest paths from the root to the single largest object: `h.heap().byid[0].sp`
+3. How to create and show a set of objects: `h.iso(1,[],{})`
+
+```python
+>>> from guppy import hpy; h=hpy()
+>>> h.heap()
+Partition of a set of 30976 objects. Total size = 3544220 bytes.
+ Index  Count   %     Size   % Cumulative  % Kind (class / dict of class)
+     0   8292  27   739022  21    739022  21 str
+     1   7834  25   625624  18   1364646  39 tuple
+     2   2079   7   300624   8   1665270  47 types.CodeType
+     3    400   1   297088   8   1962358  55 type
+     4   4168  13   279278   8   2241636  63 bytes
+     5   1869   6   269136   8   2510772  71 function
+     6    400   1   228464   6   2739236  77 dict of type
+     7     79   0   139704   4   2878940  81 dict of module
+     8   1061   3    93368   3   2972308  84 types.WrapperDescriptorType
+     9    172   1    81712   2   3054020  86 dict (no owner)
+<89 more rows. Type e.g. '_.more' to view.>
+>>> h.heap().byid[0].sp
+ 0: h.Root.i0_modules['os'].__dict__
+>>> h.iso(1,[],{})
+Partition of a set of 3 objects. Total size = 348 bytes.
+ Index  Count   %     Size   % Cumulative  % Kind (class / dict of class)
+     0      1  33      248  71       248  71 dict (no owner)
+     1      1  33       72  21       320  92 list
+     2      1  33       28   8       348 100 int
+>>>
+```
+
+People have written awesome posts on how to use this toolset, including:
+* [How to use guppy/heapy for tracking down memory usage](https://smira.ru/wp-content/uploads/2011/08/heapy.html)
+* [Debugging Django memory leak with TrackRefs and Guppy](https://opensourcehacker.com/2008/03/07/debugging-django-memory-leak-with-trackrefs-and-guppy/)
+* [Diagnosing Memory "Leaks" in Python](https://chase-seibert.github.io/blog/2013/08/03/diagnosing-memory-leaks-python.html)
+* [Digging into python memory issues in ckan with heapy](https://leastsignificant.blogspot.com/2015/06/digging-into-python-memory-issues-in.html)
+
+Formal and API documentation are [also available](https://zhuyifei1999.github.io/guppy3/).
+
+## Contributing
+
+Issues and pull requests are welcome. You may also ask for help on using this
+toolset; however, in such cases, we will only provide guidance, and not profile
+your code for you.
+
+Please make sure to update tests as appropriate.
+
+### Testing
+
+To test if the heapy build and installation was ok, you can do:
+
+```python
+>>> from guppy import hpy
+>>> hpy().test()
+Testing sets
+Test #0
+Test #1
+Test #2
+...
+```
+
+There will be several more tests. Some tests may take a while.
+
+## License
+
+Copyright (C) 2005-2013 Sverker Nilsson, S. Nilsson Computer System AB  
+Copyright (C) 2019-2021 YiFei Zhu  
+Copyright (C) 2021-2023 YiFei Zhu, Google LLC
+
+The right is granted to copy, use, modify and redistribute this code
+according to the rules in what is commonly referred to as an MIT
+license.
+
+This is not an official Google product.
+
+*** USE AT YOUR OWN RISK AND BE AWARE THAT THIS IS AN EARLY RELEASE ***
```

### Comparing `guppy3-3.1.2/guppy3.egg-info/SOURCES.txt` & `guppy3-3.1.3/guppy3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ANNOUNCE
 ChangeLog
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 guppy/__init__.py
 guppy/_version.py
 guppy/etc/Cat.py
 guppy/etc/Code.py
@@ -108,14 +109,15 @@
 src/heapy/relation.h
 src/heapy/rootstate.c
 src/heapy/roundupsize.c
 src/heapy/stdtypes.c
 src/heapy/stdtypes.h
 src/heapy/xmemstats.c
 src/include/guppy.h
+src/include/pythoncapi_compat.h
 src/sets/bitset.c
 src/sets/bitset.h
 src/sets/immnodeset.c
 src/sets/nodeset.c
 src/sets/nodeset.h
 src/sets/sets.c
 src/sets/sets.h
```

### Comparing `guppy3-3.1.2/PKG-INFO` & `guppy3-3.1.3/guppy3.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,141 @@
 Metadata-Version: 2.1
 Name: guppy3
-Version: 3.1.2
+Version: 3.1.3
 Summary: Guppy 3 -- Guppy-PE ported to Python 3
 Home-page: https://github.com/zhuyifei1999/guppy3/
 Author: YiFei Zhu
 Author-email: zhuyifei1999@gmail.com
 License: MIT
-Description: # Guppy 3
-        [![Build Status](https://img.shields.io/travis/com/zhuyifei1999/guppy3?label=tests)](https://travis-ci.com/zhuyifei1999/guppy3) [![Codecov](https://img.shields.io/codecov/c/github/zhuyifei1999/guppy3)](https://codecov.io/gh/zhuyifei1999/guppy3) [![PyPI version](https://img.shields.io/pypi/v/guppy3)](https://pypi.org/project/guppy3/) [![Repology - Repositories](https://img.shields.io/repology/repositories/python:guppy3)](https://repology.org/project/python:guppy3/versions)  
-        [![PyPI - Implementation](https://img.shields.io/pypi/implementation/guppy3)](https://pypi.org/project/guppy3/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/guppy3)](https://pypi.org/project/guppy3/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/guppy3)](https://pypistats.org/packages/guppy3) [![PyPI - License](https://img.shields.io/pypi/l/guppy3)](https://github.com/zhuyifei1999/guppy3/blob/master/LICENSE)
-        
-        A Python Programming Environment & Heap analysis toolset.
-        
-        This package contains the following subpackages:
-        * etc - Support modules. Contains especially the Glue protocol module.
-        * gsl - The Guppy Specification Language implementation. This can be used
-          to create documents and tests from a common source.
-        * heapy - The heap analysis toolset. It can be used to find information about
-          the objects in the heap and display the information in various ways.
-        * sets - Bitsets and 'nodesets' implemented in C.
-        
-        Guppy 3 is a fork of Guppy-PE, created by Sverker Nilsson for Python 2.
-        
-        ## Requirements
-        
-        You should have Python 3.6, 3.7, 3.8, or 3.9. This package is CPython only;
-        PyPy and other Python implementations are not supported. Python 2 support
-        can be obtained from [guppy-pe](http://guppy-pe.sourceforge.net/) by
-        Sverker Nilsson, from which this package is forked.
-        
-        To use the graphical browser, Tkinter is needed.
-        To use the remote monitor, threading must be available.
-        
-        ## Installation
-        
-        Install with pip by:
-        
-        ```
-        pip install guppy3
-        ```
-        
-        Install with conda by:
-        ```
-        conda install -c conda-forge guppy3
-        ```
-        
-        ## Usage
-        
-        The following example shows
-        
-        1. How to create the session context: `h=hpy()`
-        2. How to show the reachable objects in the heap: `h.heap()`
-        4. How to show the shortest paths from the root to the single largest object: `h.heap().byid[0].sp`
-        3. How to create and show a set of objects: `h.iso(1,[],{})`
-        
-        ```python
-        >>> from guppy import hpy; h=hpy()
-        >>> h.heap()
-        Partition of a set of 30976 objects. Total size = 3544220 bytes.
-         Index  Count   %     Size   % Cumulative  % Kind (class / dict of class)
-             0   8292  27   739022  21    739022  21 str
-             1   7834  25   625624  18   1364646  39 tuple
-             2   2079   7   300624   8   1665270  47 types.CodeType
-             3    400   1   297088   8   1962358  55 type
-             4   4168  13   279278   8   2241636  63 bytes
-             5   1869   6   269136   8   2510772  71 function
-             6    400   1   228464   6   2739236  77 dict of type
-             7     79   0   139704   4   2878940  81 dict of module
-             8   1061   3    93368   3   2972308  84 types.WrapperDescriptorType
-             9    172   1    81712   2   3054020  86 dict (no owner)
-        <89 more rows. Type e.g. '_.more' to view.>
-        >>> h.heap().byid[0].sp
-         0: h.Root.i0_modules['os'].__dict__
-        >>> h.iso(1,[],{})
-        Partition of a set of 3 objects. Total size = 348 bytes.
-         Index  Count   %     Size   % Cumulative  % Kind (class / dict of class)
-             0      1  33      248  71       248  71 dict (no owner)
-             1      1  33       72  21       320  92 list
-             2      1  33       28   8       348 100 int
-        >>>
-        ```
-        
-        People have written awesome posts on how to use this toolset, including:
-        * [How to use guppy/heapy for tracking down memory usage](https://smira.ru/wp-content/uploads/2011/08/heapy.html)
-        * [Debugging Django memory leak with TrackRefs and Guppy](https://opensourcehacker.com/2008/03/07/debugging-django-memory-leak-with-trackrefs-and-guppy/)
-        * [Diagnosing Memory "Leaks" in Python](https://chase-seibert.github.io/blog/2013/08/03/diagnosing-memory-leaks-python.html)
-        * [Digging into python memory issues in ckan with heapy](https://leastsignificant.blogspot.com/2015/06/digging-into-python-memory-issues-in.html)
-        
-        Formal and API documentation are [also available](https://zhuyifei1999.github.io/guppy3/).
-        
-        ## Contributing
-        
-        Issues and pull requests are welcome. You may also ask for help on using this
-        toolset; however, in such cases, we will only provide guidance, and not profile
-        your code for you.
-        
-        Please make sure to update tests as appropriate.
-        
-        ### Testing
-        
-        To test if the heapy build and installation was ok, you can do:
-        
-        ```python
-        >>> from guppy import hpy
-        >>> hpy().test()
-        Testing sets
-        Test #0
-        Test #1
-        Test #2
-        ...
-        ```
-        
-        There will be several more tests. Some tests may take a while.
-        
-        ## License
-        
-        Copyright (C) 2005-2013 Sverker Nilsson, S. Nilsson Computer System AB  
-        Copyright (C) 2019-2021 YiFei Zhu
-        
-        The right is granted to copy, use, modify and redistribute this code
-        according to the rules in what is commonly referred to as an MIT
-        license.
-        
-        *** USE AT YOUR OWN RISK AND BE AWARE THAT THIS IS AN EARLY RELEASE ***
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: C
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Guppy 3
+[![Build Status](https://img.shields.io/github/actions/workflow/status/zhuyifei1999/guppy3/workflow.yml?branch=master)](https://github.com/zhuyifei1999/guppy3/actions/workflows/workflow.yml) [![Codecov](https://img.shields.io/codecov/c/github/zhuyifei1999/guppy3)](https://codecov.io/gh/zhuyifei1999/guppy3) [![PyPI version](https://img.shields.io/pypi/v/guppy3)](https://pypi.org/project/guppy3/) [![Repology - Repositories](https://img.shields.io/repology/repositories/python:guppy3)](https://repology.org/project/python:guppy3/versions)  
+[![PyPI - Implementation](https://img.shields.io/pypi/implementation/guppy3)](https://pypi.org/project/guppy3/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/guppy3)](https://pypi.org/project/guppy3/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/guppy3)](https://pypistats.org/packages/guppy3) [![PyPI - License](https://img.shields.io/pypi/l/guppy3)](https://github.com/zhuyifei1999/guppy3/blob/master/LICENSE)
+
+A Python Programming Environment & Heap analysis toolset.
+
+This package contains the following subpackages:
+* etc - Support modules. Contains especially the Glue protocol module.
+* gsl - The Guppy Specification Language implementation. This can be used
+  to create documents and tests from a common source.
+* heapy - The heap analysis toolset. It can be used to find information about
+  the objects in the heap and display the information in various ways.
+* sets - Bitsets and 'nodesets' implemented in C.
+
+Guppy 3 is a fork of Guppy-PE, created by Sverker Nilsson for Python 2.
+
+## Requirements
+
+You should have Python 3.7, 3.8, 3.9, 3.10, or 3.11. This package is CPython
+only; PyPy and other Python implementations are not supported. Python 2 support
+can be obtained from [guppy-pe](http://guppy-pe.sourceforge.net/) by
+Sverker Nilsson, from which this package is forked.
+
+To use the graphical browser, Tkinter is needed.
+To use the remote monitor, threading must be available.
+
+## Installation
+
+Install with pip by:
+
+```
+pip install guppy3
+```
+
+Install with conda by:
+```
+conda install -c conda-forge guppy3
+```
+
+## Usage
+
+The following example shows
+
+1. How to create the session context: `h=hpy()`
+2. How to show the reachable objects in the heap: `h.heap()`
+4. How to show the shortest paths from the root to the single largest object: `h.heap().byid[0].sp`
+3. How to create and show a set of objects: `h.iso(1,[],{})`
+
+```python
+>>> from guppy import hpy; h=hpy()
+>>> h.heap()
+Partition of a set of 30976 objects. Total size = 3544220 bytes.
+ Index  Count   %     Size   % Cumulative  % Kind (class / dict of class)
+     0   8292  27   739022  21    739022  21 str
+     1   7834  25   625624  18   1364646  39 tuple
+     2   2079   7   300624   8   1665270  47 types.CodeType
+     3    400   1   297088   8   1962358  55 type
+     4   4168  13   279278   8   2241636  63 bytes
+     5   1869   6   269136   8   2510772  71 function
+     6    400   1   228464   6   2739236  77 dict of type
+     7     79   0   139704   4   2878940  81 dict of module
+     8   1061   3    93368   3   2972308  84 types.WrapperDescriptorType
+     9    172   1    81712   2   3054020  86 dict (no owner)
+<89 more rows. Type e.g. '_.more' to view.>
+>>> h.heap().byid[0].sp
+ 0: h.Root.i0_modules['os'].__dict__
+>>> h.iso(1,[],{})
+Partition of a set of 3 objects. Total size = 348 bytes.
+ Index  Count   %     Size   % Cumulative  % Kind (class / dict of class)
+     0      1  33      248  71       248  71 dict (no owner)
+     1      1  33       72  21       320  92 list
+     2      1  33       28   8       348 100 int
+>>>
+```
+
+People have written awesome posts on how to use this toolset, including:
+* [How to use guppy/heapy for tracking down memory usage](https://smira.ru/wp-content/uploads/2011/08/heapy.html)
+* [Debugging Django memory leak with TrackRefs and Guppy](https://opensourcehacker.com/2008/03/07/debugging-django-memory-leak-with-trackrefs-and-guppy/)
+* [Diagnosing Memory "Leaks" in Python](https://chase-seibert.github.io/blog/2013/08/03/diagnosing-memory-leaks-python.html)
+* [Digging into python memory issues in ckan with heapy](https://leastsignificant.blogspot.com/2015/06/digging-into-python-memory-issues-in.html)
+
+Formal and API documentation are [also available](https://zhuyifei1999.github.io/guppy3/).
+
+## Contributing
+
+Issues and pull requests are welcome. You may also ask for help on using this
+toolset; however, in such cases, we will only provide guidance, and not profile
+your code for you.
+
+Please make sure to update tests as appropriate.
+
+### Testing
+
+To test if the heapy build and installation was ok, you can do:
+
+```python
+>>> from guppy import hpy
+>>> hpy().test()
+Testing sets
+Test #0
+Test #1
+Test #2
+...
+```
+
+There will be several more tests. Some tests may take a while.
+
+## License
+
+Copyright (C) 2005-2013 Sverker Nilsson, S. Nilsson Computer System AB  
+Copyright (C) 2019-2021 YiFei Zhu  
+Copyright (C) 2021-2023 YiFei Zhu, Google LLC
+
+The right is granted to copy, use, modify and redistribute this code
+according to the rules in what is commonly referred to as an MIT
+license.
+
+This is not an official Google product.
+
+*** USE AT YOUR OWN RISK AND BE AWARE THAT THIS IS AN EARLY RELEASE ***
```

### Comparing `guppy3-3.1.2/README.md` & `guppy3-3.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Guppy 3
-[![Build Status](https://img.shields.io/travis/com/zhuyifei1999/guppy3?label=tests)](https://travis-ci.com/zhuyifei1999/guppy3) [![Codecov](https://img.shields.io/codecov/c/github/zhuyifei1999/guppy3)](https://codecov.io/gh/zhuyifei1999/guppy3) [![PyPI version](https://img.shields.io/pypi/v/guppy3)](https://pypi.org/project/guppy3/) [![Repology - Repositories](https://img.shields.io/repology/repositories/python:guppy3)](https://repology.org/project/python:guppy3/versions)  
+[![Build Status](https://img.shields.io/github/actions/workflow/status/zhuyifei1999/guppy3/workflow.yml?branch=master)](https://github.com/zhuyifei1999/guppy3/actions/workflows/workflow.yml) [![Codecov](https://img.shields.io/codecov/c/github/zhuyifei1999/guppy3)](https://codecov.io/gh/zhuyifei1999/guppy3) [![PyPI version](https://img.shields.io/pypi/v/guppy3)](https://pypi.org/project/guppy3/) [![Repology - Repositories](https://img.shields.io/repology/repositories/python:guppy3)](https://repology.org/project/python:guppy3/versions)  
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/guppy3)](https://pypi.org/project/guppy3/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/guppy3)](https://pypi.org/project/guppy3/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/guppy3)](https://pypistats.org/packages/guppy3) [![PyPI - License](https://img.shields.io/pypi/l/guppy3)](https://github.com/zhuyifei1999/guppy3/blob/master/LICENSE)
 
 A Python Programming Environment & Heap analysis toolset.
 
 This package contains the following subpackages:
 * etc - Support modules. Contains especially the Glue protocol module.
 * gsl - The Guppy Specification Language implementation. This can be used
@@ -12,16 +12,16 @@
   the objects in the heap and display the information in various ways.
 * sets - Bitsets and 'nodesets' implemented in C.
 
 Guppy 3 is a fork of Guppy-PE, created by Sverker Nilsson for Python 2.
 
 ## Requirements
 
-You should have Python 3.6, 3.7, 3.8, or 3.9. This package is CPython only;
-PyPy and other Python implementations are not supported. Python 2 support
+You should have Python 3.7, 3.8, 3.9, 3.10, or 3.11. This package is CPython
+only; PyPy and other Python implementations are not supported. Python 2 support
 can be obtained from [guppy-pe](http://guppy-pe.sourceforge.net/) by
 Sverker Nilsson, from which this package is forked.
 
 To use the graphical browser, Tkinter is needed.
 To use the remote monitor, threading must be available.
 
 ## Installation
@@ -104,14 +104,17 @@
 ```
 
 There will be several more tests. Some tests may take a while.
 
 ## License
 
 Copyright (C) 2005-2013 Sverker Nilsson, S. Nilsson Computer System AB  
-Copyright (C) 2019-2021 YiFei Zhu
+Copyright (C) 2019-2021 YiFei Zhu  
+Copyright (C) 2021-2023 YiFei Zhu, Google LLC
 
 The right is granted to copy, use, modify and redistribute this code
 according to the rules in what is commonly referred to as an MIT
 license.
 
+This is not an official Google product.
+
 *** USE AT YOUR OWN RISK AND BE AWARE THAT THIS IS AN EARLY RELEASE ***
```

### Comparing `guppy3-3.1.2/src/sets/bitset.h` & `guppy3-3.1.3/src/sets/bitset.h`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/sets/sets.c` & `guppy3-3.1.3/src/sets/sets.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/sets/nodeset.h` & `guppy3-3.1.3/src/sets/nodeset.h`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/sets/sets_internal.h` & `guppy3-3.1.3/src/sets/sets_internal.h`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/sets/bitset.c` & `guppy3-3.1.3/src/sets/bitset.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 /* BitSet implementation */
 
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 
 #include "structmember.h"
-#include "longintrepr.h"
+// #include "longintrepr.h"
 
 #include "../include/guppy.h"
+#include "../include/pythoncapi_compat.h"
 #include "../heapy/heapdef.h"
 #include "sets_internal.h"
 
 /* Docstrings */
 
 char bitset_doc[] =
 
@@ -804,21 +805,16 @@
 {
     NyMutBitSetObject *v = (NyMutBitSetObject *)type->tp_alloc(type, 0);
     if (v) {
         v->cur_field = 0;
         v->cpl = 0;
         v->splitting_size = 500/*1000*/;
 
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 9
         Py_SET_REFCNT(&v->fst_root, 1);
         Py_SET_SIZE(&v->fst_root, 0);
-#else
-        Py_REFCNT(&v->fst_root) = 1;
-        Py_SIZE(&v->fst_root) = 0;
-#endif
 
         v->fst_root.cur_size = 0;
         if (!root) {
             v->root = &v->fst_root;
             if (mutbitset_initset(v, set) == -1) {
                 Py_DECREF(v);
                 return 0;
@@ -923,15 +919,15 @@
         if (bs == &v->fst_root) {
             if (cur_size >= NyUnion_MINSIZE) {
                 assert(cur_size == NyUnion_MINSIZE);
                 bs = union_realloc(0, cur_size + 1);
                 if (!bs) return 0;
                 sfp_move(&bs->ob_field[0], &v->fst_root.ob_field[0], cur_size);
             } else {
-                Py_SIZE(bs) = cur_size + 1;
+                Py_SET_SIZE(bs, cur_size + 1);
             }
         } else {
             bs = union_realloc(bs, cur_size + 1);
             if (!bs) return 0;
         }
         assert(cur_size < Py_SIZE(bs));
         v->root = bs;
@@ -1353,15 +1349,15 @@
     } else {
         NyBit i;
         for (i = 0; i < v->root->cur_size; i++)
             Py_DECREF(v->root->ob_field[i].set);
     }
     v->cur_field = 0;
     v->root = &v->fst_root;
-    Py_SIZE(&v->fst_root) = 0;
+    Py_SET_SIZE(&v->fst_root, 0);
     v->fst_root.cur_size = 0;
     return 0;
 }
 
 
 static void
 mutbitset_dealloc(NyMutBitSetObject *v)
@@ -4348,16 +4344,16 @@
 };
 
 
 int fsb_dx_nybitset_init(PyObject *m)
 {
     PyObject *d;
 
-    Py_TYPE(&_NyImmBitSet_EmptyStruct) = &NyImmBitSet_Type;
-    Py_TYPE(&_NyImmBitSet_OmegaStruct) = &NyCplBitSet_Type;
+    Py_SET_TYPE(&_NyImmBitSet_EmptyStruct, &NyImmBitSet_Type);
+    Py_SET_TYPE(&_NyImmBitSet_OmegaStruct, &NyCplBitSet_Type);
 
     NYFILL(NyBitSet_Type);
     NYFILL(NyImmBitSet_Type);
     NYFILL(NyCplBitSet_Type);
     NYFILL(NyMutBitSet_Type);
     NYFILL(NyImmBitSetIter_Type);
     NYFILL(NyUnion_Type);
```

### Comparing `guppy3-3.1.2/src/sets/nodeset.c` & `guppy3-3.1.3/src/sets/nodeset.c`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 
 #include "structmember.h"
 
 #include "../include/guppy.h"
+#include "../include/pythoncapi_compat.h"
 #include "../heapy/heapdef.h"
 #include "sets_internal.h"
 
 PyDoc_STRVAR(nodeset_doc,
 "The class NodeSet is the base class for ImmNodeSet and MutNodeSet.\n"
 "A nodeset is a set of objects with equality based on heap address.\n"
 "The following operations are defined for both mutable and immutable\n"
@@ -260,15 +261,15 @@
 NyMutNodeSet_SubtypeNewFlags(PyTypeObject *type, int flags, PyObject *hiding_tag)
 {
     NyNodeSetObject *v = (void *)type->tp_alloc(type, 0);
     if (!v)
         return NULL;
     /*assert (flags & NS_HOLDOBJECTS); */
     v->flags = flags;
-    Py_SIZE(v) = 0;
+    Py_SET_SIZE(v, 0);
     v->u.bitset = (PyObject *)NyMutBitSet_New();
     if (!v->u.bitset) {
         Py_DECREF(v);
         return 0;
     }
     v->_hiding_tag_ = hiding_tag;
     Py_XINCREF(hiding_tag);
@@ -385,18 +386,18 @@
     return 0;
 }
 
 static void
 mutnodeset_dealloc(NyNodeSetObject *v)
 {
     PyObject_GC_UnTrack(v);
-    Py_TRASHCAN_SAFE_BEGIN(v)
+    Ny_TRASHCAN_BEGIN(v, mutnodeset_dealloc)
     mutnodeset_gc_clear(v);
     Py_TYPE(v)->tp_free((PyObject *)v);
-    Py_TRASHCAN_SAFE_END(v)
+    Ny_TRASHCAN_END(v)
 }
 
 size_t
 nodeset_indisize(PyObject *v)
 {
     NyNodeSetObject *ns = (void *)v;
     NyBit r = generic_indisize(v);
@@ -601,15 +602,15 @@
 {
     if (NyMutNodeSet_Check(v)) {
         NyBit bitno = nodeset_obj_to_bitno(obj);
         int r = NyMutBitSet_setbit((NyMutBitSetObject *)v->u.bitset, bitno);
         if (r == -1)
             return -1;
         if (!r) {
-            Py_SIZE(v)++;
+            Py_SET_SIZE(v, Py_SIZE(v) + 1);
             if (v->flags & NS_HOLDOBJECTS) {
                 Py_INCREF(obj);
             }
         }
         return r;
     } else {
         PyErr_Format(PyExc_ValueError,
@@ -623,15 +624,15 @@
 {
     if (NyMutNodeSet_Check(v) && v->u.bitset) {
         if (v->flags & NS_HOLDOBJECTS) {
             NyNodeSet_iterate(v, nodeset_dealloc_iter, v);
         }
         if (NyMutBitSet_clear((NyMutBitSetObject *)v->u.bitset) == -1)
             return -1;
-        Py_SIZE(v) = 0;
+        Py_SET_SIZE(v, 0);
     } else {
         PyErr_Format(PyExc_ValueError,
                      "mutable nodeset required");
         return -1;
     }
     return 0;
 }
@@ -642,15 +643,15 @@
 {
     if (NyMutNodeSet_Check(v)) {
         NyBit bitno = nodeset_obj_to_bitno(obj);
         int r = NyMutBitSet_clrbit((NyMutBitSetObject *)v->u.bitset, bitno);
         if (r == -1)
             return -1;
         if (r) {
-            Py_SIZE(v)--;
+            Py_SET_SIZE(v, Py_SIZE(v) - 1);
             if (v->flags & NS_HOLDOBJECTS) {
                 Py_DECREF(obj);
             }
         }
         return r;
     } else {
         PyErr_Format(PyExc_ValueError,
@@ -747,15 +748,15 @@
     if (!(NyMutNodeSet_Check(v))) {
         PyErr_SetString(PyExc_TypeError, "pop: argument must be mutable");
         return 0;
     } else {
         NyBit bitno = NyMutBitSet_pop((NyMutBitSetObject *)v->u.bitset, 0);
         if (bitno == -1 && PyErr_Occurred())
             return 0;
-        Py_SIZE(v)--;
+        Py_SET_SIZE(v, Py_SIZE(v) - 1);
         return nodeset_bitno_to_obj(bitno);
     }
 }
 
 static char remove_doc[] =
 "S.remove(e)\n"
 "\n"
```

### Comparing `guppy3-3.1.2/src/sets/immnodeset.c` & `guppy3-3.1.3/src/sets/immnodeset.c`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 } NyImmNodeSetIterObject;
 
 
 static void
 immnsiter_dealloc(NyImmNodeSetIterObject *it)
 {
     PyObject_GC_UnTrack(it);
-    Py_TRASHCAN_SAFE_BEGIN(it)
-        Py_XDECREF(it->nodeset);
-        PyObject_GC_Del(it);
-    Py_TRASHCAN_SAFE_END(it)
+    Ny_TRASHCAN_BEGIN(it, immnsiter_dealloc)
+    Py_XDECREF(it->nodeset);
+    PyObject_GC_Del(it);
+    Ny_TRASHCAN_END(it)
 }
 
 static PyObject *
 immnsiter_getiter(PyObject *it)
 {
     Py_INCREF(it);
     return it;
@@ -218,18 +218,18 @@
     return 0;
 }
 
 static void
 immnodeset_dealloc(NyNodeSetObject *v)
 {
     PyObject_GC_UnTrack(v);
-    Py_TRASHCAN_SAFE_BEGIN(v)
+    Ny_TRASHCAN_BEGIN(v, immnodeset_dealloc)
     immnodeset_gc_clear(v);
     Py_TYPE(v)->tp_free((PyObject *)v);
-    Py_TRASHCAN_SAFE_END(v)
+    Ny_TRASHCAN_END(v)
 }
 
 
 
 static int
 immnodeset_gc_traverse(NyNodeSetObject *v, visitproc visit, void *arg)
 {
```

### Comparing `guppy3-3.1.2/src/heapy/hv_cli_id.c` & `guppy3-3.1.3/src/heapy/hv_cli_id.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/hv_cli_dictof.c` & `guppy3-3.1.3/src/heapy/hv_cli_dictof.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/roundupsize.c` & `guppy3-3.1.3/src/heapy/roundupsize.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/hv.c` & `guppy3-3.1.3/src/heapy/hv.c`

 * *Files 0% similar despite different names*

```diff
@@ -518,14 +518,23 @@
     return xt->xt_size(obj);
 }
 
 
 static int
 xt_traverse(ExtraType *xt, PyObject *obj, visitproc visit, void *arg)
 {
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+    if (Py_TYPE(obj)->tp_flags & Py_TPFLAGS_MANAGED_DICT) {
+        // FIXME: There's no way to distinguish between managed dict entries
+        // and other references. To keep our results stable we have to
+        // materialize this managed dict, which allocates a lot of memory
+        // and will add additional overhead.
+        _PyObject_GetDictPtr(obj);
+    }
+#endif
     if (xt->xt_trav_code == XT_NO)
         return 0;
     else if (xt->xt_trav_code == XT_TP)
         return Py_TYPE(obj)->tp_traverse(obj, visit, arg);
     else
         return xt->xt_traverse(xt, obj, visit, arg);
 }
@@ -736,18 +745,18 @@
     return NyHeapView_SubTypeNew(type, root, (PyTupleObject *)heapdefs);
 }
 
 static void
 hv_dealloc(PyObject *v)
 {
     PyObject_GC_UnTrack(v);
-    Py_TRASHCAN_SAFE_BEGIN(v)
+    Ny_TRASHCAN_BEGIN(v, hv_dealloc)
     hv_gc_clear((NyHeapViewObject *)v);
     Py_TYPE(v)->tp_free(v);
-    Py_TRASHCAN_SAFE_END(v)
+    Ny_TRASHCAN_END(v)
 }
 
 PyDoc_STRVAR(hv_delete_extra_type_doc,
 "HV.delete_extra_type(weakref)\n\
 \n\
 Delete extra type information. For internal use as a weak-ref callback.");
```

### Comparing `guppy3-3.1.2/src/heapy/hv_cli.c` & `guppy3-3.1.3/src/heapy/hv_cli.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/hv_cli_indisize.c` & `guppy3-3.1.3/src/heapy/hv_cli_indisize.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/impsets.c` & `guppy3-3.1.3/src/heapy/impsets.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/hv_cli_and.c` & `guppy3-3.1.3/src/heapy/hv_cli_and.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/xmemstats.c` & `guppy3-3.1.3/src/heapy/xmemstats.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/heapy.h` & `guppy3-3.1.3/src/heapy/heapy.h`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/classifier.h` & `guppy3-3.1.3/src/heapy/classifier.h`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/initheapyc.c` & `guppy3-3.1.3/src/heapy/initheapyc.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/nodegraph.h` & `guppy3-3.1.3/src/heapy/nodegraph.h`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/rootstate.c` & `guppy3-3.1.3/src/heapy/rootstate.c`

 * *Files 21% similar despite different names*

```diff
@@ -150,69 +150,66 @@
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 8
     MEMBER(dict),
 #endif
 
     MEMBER(builtins_copy),
     MEMBER(import_func),
 
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
-# ifdef HAVE_FORK
+#ifdef HAVE_FORK
     MEMBER(before_forkers),
     MEMBER(after_forkers_parent),
     MEMBER(after_forkers_child),
-# endif
-# if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION < 10
+#endif
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION < 10
     MEMBER(pyexitmodule),
-# endif
 #endif
 
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 8
     MEMBER(audit_hooks),
 #endif
     {0} /* Sentinel */
 };
 
 #undef MEMBER
 
 #define MEMBER(name) {#name, T_OBJECT, offsetof(PyThreadState, name)}
 #define RENAMEMEMBER(name, newname) {#newname, T_OBJECT, offsetof(PyThreadState, name)}
 
 static struct PyMemberDef ts_members[] = {
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION < 11
     MEMBER(frame),
+#endif
+
     MEMBER(c_profileobj),
     MEMBER(c_traceobj),
 
     MEMBER(curexc_type),
     MEMBER(curexc_value),
     MEMBER(curexc_traceback),
 
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+    RENAMEMEMBER(exc_state.exc_value, exc_value),
+#else
     RENAMEMEMBER(exc_state.exc_type, exc_type),
     RENAMEMEMBER(exc_state.exc_value, exc_value),
     RENAMEMEMBER(exc_state.exc_traceback, exc_traceback),
-#else
-    MEMBER(exc_type),
-    MEMBER(exc_value),
-    MEMBER(exc_traceback),
 #endif
 
     MEMBER(dict),
     MEMBER(async_exc),
     // trash_delete_later not included
 
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION < 8
     MEMBER(coroutine_wrapper),
 #endif
 
     MEMBER(async_gen_firstiter),
     MEMBER(async_gen_finalizer),
 
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
     MEMBER(context),
-#endif
     {0} /* Sentinel */
 };
 
 #undef MEMBER
 
 #define ISATTR(name)                                                                  \
     if ((PyObject *)is->name == r->tgt) {                                             \
@@ -284,76 +281,87 @@
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 8
         ISATTR(dict);
 #endif
 
         ISATTR(builtins_copy);
         ISATTR(import_func);
 
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
-# ifdef HAVE_FORK
+#ifdef HAVE_FORK
         ISATTR(before_forkers);
         ISATTR(after_forkers_parent);
         ISATTR(after_forkers_child);
-# endif
-# if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION < 10
+#endif
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION < 10
         ISATTR(pyexitmodule);
-# endif
 #endif
 
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 8
         ISATTR(audit_hooks);
 #endif
 
-        for (ts = is->tstate_head; ts; ts = ts->next) {
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+        ts = is->threads.head;
+#else
+        ts = is->tstate_head;
+#endif
+        for (; ts; ts = ts->next) {
             if ((ts == bts && r->tgt == hv->limitframe) ||
                     (!hv->limitframe && isframe)) {
                 int frameno = -1;
                 int numframes = 0;
                 PyFrameObject *frame;
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+                for (frame = PyThreadState_GetFrame(ts); frame;) {
+                    PyFrameObject *next_frame = PyFrame_GetBack(frame);
+                    numframes++;
+                    if ((PyObject *)frame == r->tgt)
+                        frameno = numframes;
+
+                    Py_DECREF(frame);
+                    frame = next_frame;
+                }
+#else
                 for (frame = (PyFrameObject *)ts->frame; frame; frame = frame->f_back) {
                     numframes++;
-                    if (r->tgt == (PyObject *)frame)
+                    if ((PyObject *)frame == r->tgt)
                         frameno = numframes;
                 }
+#endif
                 if (frameno != -1) {
                     frameno = numframes - frameno;
                     if (r->visit(NYHR_ATTRIBUTE, PyUnicode_FromFormat("i%d_t%lu_f%d", isno, THREAD_ID(ts), frameno), r))
                         return 1;
                 }
             }
             TSATTR(c_profileobj);
             TSATTR(c_traceobj);
 
             TSATTR(curexc_type);
             TSATTR(curexc_value);
             TSATTR(curexc_traceback);
 
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+            RENAMETSATTR(exc_state.exc_value, exc_value);
+#else
             RENAMETSATTR(exc_state.exc_type, exc_type);
             RENAMETSATTR(exc_state.exc_value, exc_value);
             RENAMETSATTR(exc_state.exc_traceback, exc_traceback);
-#else
-            TSATTR(exc_type);
-            TSATTR(exc_value);
-            TSATTR(exc_traceback);
 #endif
 
             TSATTR(dict);
             TSATTR(async_exc);
 
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION < 8
             TSATTR(coroutine_wrapper);
 #endif
 
             TSATTR(async_gen_firstiter);
             TSATTR(async_gen_finalizer);
 
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
             TSATTR(context);
-#endif
         }
     }
     return 0;
 }
 
 
 int
@@ -387,65 +395,70 @@
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 8
         Py_VISIT(is->dict);
 #endif
 
         Py_VISIT(is->builtins_copy);
         Py_VISIT(is->import_func);
 
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
-# ifdef HAVE_FORK
+#ifdef HAVE_FORK
         Py_VISIT(is->before_forkers);
         Py_VISIT(is->after_forkers_parent);
         Py_VISIT(is->after_forkers_child);
-# endif
-# if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION < 10
+#endif
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION < 10
         Py_VISIT(is->pyexitmodule);
-# endif
 #endif
 
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 8
         Py_VISIT(is->audit_hooks);
 #endif
 
-        for (ts = is->tstate_head; ts; ts = ts->next) {
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+        ts = is->threads.head;
+#else
+        ts = is->tstate_head;
+#endif
+        for (; ts; ts = ts->next) {
             if (ts == bts && hv->limitframe) {
                 Py_VISIT(hv->limitframe);
             } else if (!hv->limitframe) {
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+                PyFrameObject *frame = PyThreadState_GetFrame(ts);
+                Py_VISIT(frame);
+                Py_XDECREF(frame);
+#else
                 Py_VISIT(ts->frame);
+#endif
             }
             Py_VISIT(ts->c_profileobj);
             Py_VISIT(ts->c_traceobj);
 
             Py_VISIT(ts->curexc_type);
             Py_VISIT(ts->curexc_value);
             Py_VISIT(ts->curexc_traceback);
 
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+            Py_VISIT(ts->exc_state.exc_value);
+#else
             Py_VISIT(ts->exc_state.exc_type);
             Py_VISIT(ts->exc_state.exc_value);
             Py_VISIT(ts->exc_state.exc_traceback);
-#else
-            Py_VISIT(ts->exc_type);
-            Py_VISIT(ts->exc_value);
-            Py_VISIT(ts->exc_traceback);
 #endif
 
             Py_VISIT(ts->dict);
             Py_VISIT(ts->async_exc);
 
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION < 8
             Py_VISIT(ts->coroutine_wrapper);
 #endif
 
             Py_VISIT(ts->async_gen_firstiter);
             Py_VISIT(ts->async_gen_finalizer);
 
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
             Py_VISIT(ts->context);
-#endif
         }
     }
     return 0;
 }
 
 // Ported from py2
 static PyObject *
@@ -464,14 +477,15 @@
 
 
 static PyObject *
 rootstate_getattr(PyObject *obj, PyObject *name)
 {
     const char *s = PyUnicode_AsUTF8(name);
     PyInterpreterState *is;
+    PyThreadState *ts;
     int n = 0;
     int ino;
     unsigned long tno;
     if (!s)
         return 0;
     Py_INCREF(name);
     if (sscanf(s, "i%d_%n", &ino, &n) == 1) {
@@ -488,32 +502,59 @@
             if (is != PyInterpreterState_Get())
                 continue;
 #endif
             int isno = numis - countis - 1;
             if (isno == ino) {
                 if (sscanf(s, "t%lu_%n", &tno, &n) == 1) {
                     s += n;
-                    PyThreadState *ts;
-                    for (ts = is->tstate_head; ts; ts = ts->next) {
+
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+                    ts = is->threads.head;
+#else
+                    ts = is->tstate_head;
+#endif
+                    for (; ts; ts = ts->next) {
                         if (THREAD_ID(ts) == tno) {
                             int frameno = 0;
                             if (sscanf(s, "f%d%n", &frameno, &n) == 1 && s[n] == '\0') {
-                                PyFrameObject *frame;
                                 int numframes = 0;
+                                PyFrameObject *frame;
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+                                PyFrameObject *current_frame = PyThreadState_GetFrame(ts);
+                                for (frame = (PyFrameObject *)Py_XNewRef(current_frame); frame;) {
+                                    PyFrameObject *next_frame = PyFrame_GetBack(frame);
+                                    numframes++;
+                                    Py_DECREF(frame);
+                                    frame = next_frame;
+                                }
+                                for (frame = (PyFrameObject *)Py_XNewRef(current_frame); frame;) {
+                                    PyFrameObject *next_frame = PyFrame_GetBack(frame);
+                                    numframes--;
+                                    if (numframes == frameno) {
+                                        Py_DECREF(current_frame);
+                                        Py_DECREF(name);
+                                        return (PyObject *)frame;
+                                    }
+                                    Py_DECREF(frame);
+                                    frame = next_frame;
+                                }
+                                Py_DECREF(current_frame);
+#else
                                 for (frame = ts->frame; frame; frame = frame->f_back) {
-                                    numframes ++;
+                                    numframes++;
                                 }
                                 for (frame = ts->frame; frame; frame = frame->f_back) {
-                                    numframes --;
+                                    numframes--;
                                     if (numframes == frameno) {
                                         Py_INCREF(frame);
                                         Py_DECREF(name);
                                         return (PyObject *)frame;
                                     }
                                 }
+#endif
                                 PyErr_Format(PyExc_AttributeError,
                                              "thread state has no frame numbered %d from bottom",
                                              frameno);
                                 Py_DECREF(name);
                                 return 0;
                             } else {
                                 PyObject *ret = _shim_PyMember_Get((char *)ts, ts_members, s);
@@ -555,16 +596,21 @@
              is;
              is = PyInterpreterState_Next(is), countis++) {
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 9
             if (is != PyInterpreterState_Get())
                 continue;
 #endif
             int isno = numis - countis - 1;
-            PyThreadState *ts;
-            for (ts = is->tstate_head; ts; ts = ts->next) {
+
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+            ts = is->threads.head;
+#else
+            ts = is->tstate_head;
+#endif
+            for (; ts; ts = ts->next) {
                 if (THREAD_ID(ts) == tno) {
                     PyObject *fullname = PyUnicode_FromFormat("i%d_%U", isno, name);
                     if (!fullname) {
                         Py_DECREF(name);
                         return 0;
                     }
                     PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
@@ -632,45 +678,59 @@
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 8
         ISATTR_DIR(dict);
 #endif
 
         ISATTR_DIR(builtins_copy);
         ISATTR_DIR(import_func);
 
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
-# ifdef HAVE_FORK
+#ifdef HAVE_FORK
         ISATTR_DIR(before_forkers);
         ISATTR_DIR(after_forkers_parent);
         ISATTR_DIR(after_forkers_child);
-# endif
-# if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION < 10
+#endif
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION < 10
         ISATTR_DIR(pyexitmodule);
-# endif
 #endif
 
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 8
         ISATTR_DIR(audit_hooks);
 #endif
 
-        for (ts = is->tstate_head; ts; ts = ts->next) {
+
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+        ts = is->threads.head;
+#else
+        ts = is->tstate_head;
+#endif
+        for (; ts; ts = ts->next) {
             int numframes = 0;
             PyFrameObject *frame;
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+            for (frame = PyThreadState_GetFrame(ts); frame;) {
+                PyFrameObject *next_frame = PyFrame_GetBack(frame);
+                numframes++;
+                Py_DECREF(frame);
+                frame = next_frame;
+            }
+#else
             for (frame = (PyFrameObject *)ts->frame; frame; frame = frame->f_back) {
                 numframes++;
             }
+#endif
             int frameno;
             for (frameno = 0; frameno < numframes; frameno++) {
                 attr = PyUnicode_FromFormat("i%d_t%lu_f%d", isno, THREAD_ID(ts), frameno);
-                if (attr) {
-                    if (PyList_Append(list, attr)) {
-                        Py_DECREF(attr);
-                        goto Err;
-                    }
+                if (!attr)
+                    goto Err;
+
+                if (PyList_Append(list, attr)) {
                     Py_DECREF(attr);
+                    goto Err;
                 }
+                Py_DECREF(attr);
             }
             TSATTR_DIR(c_profileobj);
             TSATTR_DIR(c_traceobj);
 
             TSATTR_DIR(curexc_type);
             TSATTR_DIR(curexc_value);
             TSATTR_DIR(curexc_traceback);
@@ -685,17 +745,15 @@
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION < 8
             TSATTR_DIR(coroutine_wrapper);
 #endif
 
             TSATTR_DIR(async_gen_firstiter);
             TSATTR_DIR(async_gen_finalizer);
 
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
             TSATTR_DIR(context);
-#endif
         }
     }
 
     return list;
 
 Err:
     Py_DECREF(list);
```

### Comparing `guppy3-3.1.2/src/heapy/hv_cli_prod.c` & `guppy3-3.1.3/src/heapy/hv_cli_prod.c`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 "The classification of an object is the file name and line number\n"
 "in which the object is produced (allocated).\n"
 "\n"
 "    memo        A dict object used to\n"
 "                memoize the classification sets.\n"
 );
 
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+# define Py_BUILD_CORE
+#  undef _PyObject_LookupSpecial
+/* _PyType_PreHeaderSize */
+#  include <internal/pycore_object.h>
+# undef Py_BUILD_CORE
+#endif
+
 // The sizeof of PyGC_Head is not to be trusted upon even across Python minor
 // releases. Eg: python/cpython@8766cb7
 static Py_ssize_t sizeof_PyGC_Head;
 
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 9
 # define INTERNAL_MODULE "_testinternalcapi"
 #else
@@ -96,14 +104,23 @@
     // Refer to _tracemalloc.c:_tracemalloc__get_object_traceback
     if (PyType_IS_GC(Py_TYPE(obj))) {
         ptr = (Py_uintptr_t)((char *)obj - sizeof_PyGC_Head);
     } else {
         ptr = (Py_uintptr_t)obj;
     }
 
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11
+    // https://github.com/python/cpython/issues/101430
+    ptr -= _PyType_PreHeaderSize(Py_TYPE(obj));
+    // _PyType_PreHeaderSize would add an extra compile-time sizeof(PyGC_Head),
+    // which may be different from the true value in sizeof_PyGC_Head
+    if (PyType_IS_GC(Py_TYPE(obj)))
+        ptr += sizeof(PyGC_Head);
+#endif
+
     tb = _PyTraceMalloc_GetTraceback(0, (Py_uintptr_t)ptr);
 
     if (!tb)
         goto Err;
 
     if (PySequence_Check(tb) && PySequence_Length(tb)) {
         kind = PySequence_GetItem(tb, 0);
```

### Comparing `guppy3-3.1.2/src/heapy/hv_cli_rcs.c` & `guppy3-3.1.3/src/heapy/hv_cli_rcs.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/classifier.c` & `guppy3-3.1.3/src/heapy/classifier.c`

 * *Files 0% similar despite different names*

```diff
@@ -35,18 +35,18 @@
     }
 }
 
 static void
 cli_dealloc(NyObjectClassifierObject *op)
 {
     PyObject_GC_UnTrack(op);
-    Py_TRASHCAN_SAFE_BEGIN(op)
+    Ny_TRASHCAN_BEGIN(op, cli_dealloc)
     Py_XDECREF(op->self);
     PyObject_GC_Del(op);
-    Py_TRASHCAN_SAFE_END(op)
+    Ny_TRASHCAN_END(op)
 }
 
 static int
 cli_traverse(NyObjectClassifierObject *op, visitproc visit, void *arg)
 {
     if (op->self)
         return visit(op->self, arg);
```

### Comparing `guppy3-3.1.2/src/heapy/hv_cli_findex.c` & `guppy3-3.1.3/src/heapy/hv_cli_findex.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/interpreter.c` & `guppy3-3.1.3/src/heapy/interpreter.c`

 * *Files 13% similar despite different names*

```diff
@@ -34,69 +34,18 @@
 #include "eval.h"
 
 #if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 8
 # define Py_BUILD_CORE
 /* _PyMem_SetDefaultAllocator */
 #  include <internal/pycore_pymem.h>
 # undef Py_BUILD_CORE
-#elif PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
+#else
 PyAPI_FUNC(int) _PyMem_SetDefaultAllocator(
     PyMemAllocatorDomain domain,
     PyMemAllocatorEx *old_alloc);
-#else
-// source: cpython: Objects/obmalloc.c
-static void *
-_PyMem_RawMalloc(void *ctx, size_t size)
-{
-    if (size == 0)
-        size = 1;
-    return malloc(size);
-}
-
-static void *
-_PyMem_RawCalloc(void *ctx, size_t nelem, size_t elsize)
-{
-    if (nelem == 0 || elsize == 0) {
-        nelem = 1;
-        elsize = 1;
-    }
-    return calloc(nelem, elsize);
-}
-
-static void *
-_PyMem_RawRealloc(void *ctx, void *ptr, size_t size)
-{
-    if (size == 0)
-        size = 1;
-    return realloc(ptr, size);
-}
-
-static void
-_PyMem_RawFree(void *ctx, void *ptr)
-{
-    free(ptr);
-}
-
-static int _PyMem_SetDefaultAllocator(
-    PyMemAllocatorDomain domain,
-    PyMemAllocatorEx *old_alloc)
-{
-    assert(domain == PYMEM_DOMAIN_RAW);
-    PyMem_GetAllocator(domain, old_alloc);
-
-    PyMemAllocatorEx alloc = {
-        .malloc  = _PyMem_RawMalloc,
-        .calloc  = _PyMem_RawCalloc,
-        .realloc = _PyMem_RawRealloc,
-        .free    = _PyMem_RawFree,
-        .ctx     = NULL
-    };
-    PyMem_SetAllocator(domain, &alloc);
-    return 0;
-}
 #endif
 
 struct bootstate {
     PyObject *cmd;
     PyObject *locals;
     // used by child to signal parent that thread has started
     PyThread_type_lock evt_ready;
```

### Comparing `guppy3-3.1.2/src/heapy/heapyc.c` & `guppy3-3.1.3/src/heapy/heapyc.c`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 
 #include "structmember.h"
 #include "compile.h"
 #include "frameobject.h"
 #include "../include/guppy.h"
+#include "../include/pythoncapi_compat.h"
 #include "../sets/nodeset.h"
 #include "hpinit.h"
 #include "heapdef.h"
 #include "heapy.h"
 #include "classifier.h"
 #include "nodegraph.h"
 #include "relation.h"
@@ -220,15 +221,15 @@
 
 PyMODINIT_FUNC
 INITFUNC (void)
 {
     PyObject *m = NULL;
     PyObject *d;
 
-    Py_TYPE(&_Ny_RootStateStruct) = &NyRootState_Type;
+    Py_SET_TYPE(&_Ny_RootStateStruct, &NyRootState_Type);
 
     // This has to be here because of 'initializer is not a constant'
     // build error on Windows.
     NyNodeTuple_Type.tp_base = &PyTuple_Type;
     if (nyfills() == -1) {
         goto error;
     }
```

### Comparing `guppy3-3.1.2/src/heapy/nodegraph.c` & `guppy3-3.1.3/src/heapy/nodegraph.c`

 * *Files 0% similar despite different names*

```diff
@@ -107,25 +107,24 @@
 }
 
 static void
 ng_dealloc(PyObject *v)
 {
     NyNodeGraphObject *ng = (void *)v;
     Py_ssize_t i;
-    Py_TRASHCAN_SAFE_BEGIN(v)
     PyObject_GC_UnTrack(v);
+    Ny_TRASHCAN_BEGIN(v, ng_dealloc)
     ng_gc_clear(ng);
     for (i = 0; i < ng->used_size; i++) {
         Py_DECREF(ng->edges[i].src);
         Py_DECREF(ng->edges[i].tgt);
     }
     PyMem_FREE(ng->edges);
     Py_TYPE(ng)->tp_free(v);
-    Py_TRASHCAN_SAFE_END(v)
-
+    Ny_TRASHCAN_END(v)
 }
 
 static int
 ng_gc_traverse(NyNodeGraphObject *ng, visitproc visit, void *arg)
 {
     Py_ssize_t i;
     int err = 0;
```

### Comparing `guppy3-3.1.2/src/heapy/hv_cli_user.c` & `guppy3-3.1.3/src/heapy/hv_cli_user.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/hv_cli_idset.c` & `guppy3-3.1.3/src/heapy/hv_cli_idset.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/hv_cli_rel.c` & `guppy3-3.1.3/src/heapy/hv_cli_rel.c`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 PyDoc_STRVAR(rel_doc,
 "");
 
 static void
 rel_dealloc(NyRelationObject *op)
 {
     PyObject_GC_UnTrack(op);
-    Py_TRASHCAN_SAFE_BEGIN(op)
+    Ny_TRASHCAN_BEGIN(op, rel_dealloc)
     Py_XDECREF(op->relator);
     Py_TYPE(op)->tp_free(op);
-    Py_TRASHCAN_SAFE_END(op)
+    Ny_TRASHCAN_END(op)
 }
 
 PyObject *
 NyRelation_SubTypeNew(PyTypeObject *type, int kind, PyObject *relator)
 {
     NyRelationObject *rel = (NyRelationObject *)type->tp_alloc(type, 1);
     if (!rel)
```

### Comparing `guppy3-3.1.2/src/heapy/heapdef.h` & `guppy3-3.1.3/src/heapy/heapdef.h`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/src/heapy/horizon.c` & `guppy3-3.1.3/src/heapy/horizon.c`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/Code.py` & `guppy3-3.1.3/guppy/etc/Code.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/RE.py` & `guppy3-3.1.3/guppy/etc/RE.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/Cat.py` & `guppy3-3.1.3/guppy/etc/Cat.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/Descriptor.py` & `guppy3-3.1.3/guppy/etc/Descriptor.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/IterPermute.py` & `guppy3-3.1.3/guppy/etc/IterPermute.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/Glue.py` & `guppy3-3.1.3/guppy/etc/Glue.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,28 +93,29 @@
                 complete.append(a)
         complete.sort()
         for a in complete:
             print('    ', a)
 
 
 class Share:
+    __slots__ = ('module', 'parent', 'name', 'Clamp', 'setable', 'chgable',
+                 'importedfrom', 'nowrap', 'wrapattr', 'wrapping', 'data',
+                 'owners', 'ispackage', 'recursion', 'preload')
     has_getattr_logging_enabled = False
-    Clamp = None
 
     def __init__(self, module, parent, name, Clamp):
         if parent is None:
             parent = self
             root = self
         else:
             root = parent.data['_root']
         self.module = module
         self.parent = parent
         self.name = name
-        if Clamp is not None:
-            self.Clamp = Clamp
+        self.Clamp = Clamp
 
         self.setable = getattr(Clamp, '_setable_', ())
         if not isinstance(self.setable, tuple):
             raise TypeError(self.message(
                 'the _setable_ attribute must be a tuple'))
 
         self.chgable = getattr(Clamp, '_chgable_', ())
@@ -419,9 +420,8 @@
 
 All functionality in the system may be accessed from this object.
 Modules are imported on demand when accessed. Other objects may be
 created or imported on demand using Guppy Glue+ directives.
 """
     share = Share(None, None, '', None)
     r = Owner('').makeInterface({'_name': ''}, share, '')
-    share.root_interface = r
     return r
```

### Comparing `guppy3-3.1.2/guppy/etc/KnuthBendix.py` & `guppy3-3.1.3/guppy/etc/KnuthBendix.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/tkcursors.py` & `guppy3-3.1.3/guppy/etc/tkcursors.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/etc.py` & `guppy3-3.1.3/guppy/etc/etc.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/textView.py` & `guppy3-3.1.3/guppy/etc/textView.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/cmd.py` & `guppy3-3.1.3/guppy/etc/cmd.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/FSA.py` & `guppy3-3.1.3/guppy/etc/FSA.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/xterm.py` & `guppy3-3.1.3/guppy/etc/xterm.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/Help.py` & `guppy3-3.1.3/guppy/etc/Help.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/KanExtension.py` & `guppy3-3.1.3/guppy/etc/KanExtension.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/etc/RE_Rect.py` & `guppy3-3.1.3/guppy/etc/RE_Rect.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/__init__.py` & `guppy3-3.1.3/guppy/__init__.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/sets/test.py` & `guppy3-3.1.3/guppy/sets/test.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/sets/__init__.py` & `guppy3-3.1.3/guppy/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/gsl/Main.py` & `guppy3-3.1.3/guppy/gsl/Main.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/gsl/DottedTree.py` & `guppy3-3.1.3/guppy/gsl/DottedTree.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/gsl/Document.py` & `guppy3-3.1.3/guppy/gsl/Document.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/gsl/XHTML.py` & `guppy3-3.1.3/guppy/gsl/XHTML.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/gsl/SpecNodes.py` & `guppy3-3.1.3/guppy/gsl/SpecNodes.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/gsl/Latex.py` & `guppy3-3.1.3/guppy/gsl/Latex.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/gsl/Html.py` & `guppy3-3.1.3/guppy/gsl/Html.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/gsl/Text.py` & `guppy3-3.1.3/guppy/gsl/Text.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/gsl/Filer.py` & `guppy3-3.1.3/guppy/gsl/Filer.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/gsl/Help.py` & `guppy3-3.1.3/guppy/gsl/Help.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/gsl/Gsml.py` & `guppy3-3.1.3/guppy/gsl/Gsml.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/gsl/FileIO.py` & `guppy3-3.1.3/guppy/gsl/FileIO.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/gsl/Tester.py` & `guppy3-3.1.3/guppy/gsl/Tester.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/Console.py` & `guppy3-3.1.3/guppy/heapy/Console.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/Monitor.py` & `guppy3-3.1.3/guppy/heapy/Monitor.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/Remote.py` & `guppy3-3.1.3/guppy/heapy/Remote.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/Use.py` & `guppy3-3.1.3/guppy/heapy/Use.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/Doc.py` & `guppy3-3.1.3/guppy/heapy/Doc.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/Spec.py` & `guppy3-3.1.3/guppy/heapy/Spec.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/OutputHandling.py` & `guppy3-3.1.3/guppy/heapy/OutputHandling.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/UniSet.py` & `guppy3-3.1.3/guppy/heapy/UniSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -2067,15 +2067,17 @@
     str_traceback._idpart_header = 'Frame at Address'
 
     def str_type(self, x, longer=False):
         if x in self.shorter_invtypes and not longer:
             return self.shorter_invtypes[x]
         if x in self.invtypes:
             return self.invtypes[x]
-        return '%s.%s' % (x.__module__, x.__name__)
+        if not hasattr(x, '__module__'):
+            return f'<unknown module>.{x.__name__}'
+        return f'{x.__module__}.{x.__name__}'
     str_type._idpart_header = 'Name'
 
     def str_type_longer(self, x):
         if x in self.invtypes:
             return self.invtypes[x]
         return '%s.%s' % (x.__module__, x.__name__)
     str_type._longer_method = lambda x: str_type
```

### Comparing `guppy3-3.1.2/guppy/heapy/Part.py` & `guppy3-3.1.3/guppy/heapy/Part.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/Path.py` & `guppy3-3.1.3/guppy/heapy/Path.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,20 +84,24 @@
     __slots__ = 'r', 'isinverted'
 
     def __init__(self, r, isinverted=0):
         self.r = r
         self.isinverted = isinverted
 
     def __lt__(self, other):
-        if isinstance(other, RelationBase):
-            if self.code != other.code:
-                return self.code < other.code
-            return self.r < other.r
-        else:
+        if not isinstance(other, RelationBase):
             return id(type(self)) < id(type(other))
+        if self.code != other.code:
+            return self.code < other.code
+        if type(self.r) is not type(other.r):
+            return id(type(self.r)) < id(type(other.r))
+        try:
+            return self.r < other.r
+        except TypeError:
+            return id(self.r) < id(other.r)
 
     def __eq__(self, other):
         if isinstance(other, RelationBase):
             if self.code != other.code:
                 return False
             return self.r == other.r
         else:
```

### Comparing `guppy3-3.1.2/guppy/heapy/Prof.py` & `guppy3-3.1.3/guppy/heapy/Prof.py`

 * *Files 0% similar despite different names*

```diff
@@ -814,18 +814,18 @@
         self.master = master
         self.scale_table = scale_table
         self.numkindrows = numkindrows
         self.getkindcolor = getkindcolor
         self.xrange = xrange
         self.yrange = yrange
         self.xgrid = xgrid
-        self.var_xgrid = BooleanVar(xgrid)
-        self.var_xgrid.set(xgrid)
-        self.var_ygrid = BooleanVar(xgrid)
         self.ygrid = ygrid
+        self.var_xgrid = BooleanVar()
+        self.var_xgrid.set(xgrid)
+        self.var_ygrid = BooleanVar()
         self.var_ygrid.set(ygrid)
         self.graphtype = graphtype
         self.statype = statype
 
         self.numstats = 0
         self.ymaxs = []
         self.ymins = []
```

### Comparing `guppy3-3.1.2/guppy/heapy/ImpSet.py` & `guppy3-3.1.3/guppy/heapy/ImpSet.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/RefPat.py` & `guppy3-3.1.3/guppy/heapy/RefPat.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/test/test_Path.py` & `guppy3-3.1.3/guppy/heapy/test/test_Path.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,16 +63,20 @@
         def f():
             a = 3
             return self, a
         co = f.__code__
         # xxx brittle test but catches a bug
         self.chkpath(co, 3, '%s.co_consts[1]')
         # commented in notes Sep 27 2004
-        relAttr = ('co_code', 'co_consts', 'co_names', 'co_varnames',
-                   'co_freevars', 'co_cellvars', 'co_filename', 'co_name')
+        relAttr = ('co_code', 'co_consts', 'co_names',
+                   'co_filename', 'co_name')
+        if self.version_info < (3, 11):
+            relAttr += ('co_varnames', 'co_freevars', 'co_cellvars')
+        else:
+            relAttr += ('co_exceptiontable', 'co_qualname')
         if self.version_info >= (3, 10):
             relAttr += ('co_linetable',)
         else:
             relAttr += ('co_lnotab',)
         self.chkrelattr(co, *relAttr)
 
     def test_dict_relation(self):
@@ -321,17 +325,21 @@
 
         # Thread attributes
 
         try:
             1/0
         except ZeroDivisionError:
             exc_type, exc_value, exc_traceback = sys.exc_info()
-            for name in 'exc_type', 'exc_value', 'exc_traceback':
-                rel = str(self.relation(root, eval(name)))
-                self.asis(eval(rel % 'root'), eval(name))
+            if sys.version_info >= (3, 11):
+                rel = str(self.relation(root, exc_value))
+                self.asis(eval(rel % 'root'), exc_value)
+            else:
+                for name in 'exc_type', 'exc_value', 'exc_traceback':
+                    rel = str(self.relation(root, eval(name)))
+                    self.asis(eval(rel % 'root'), eval(name))
 
             # There are more, untested, attributes, but the code is farily regular...
             # More complication is to do with frames which I concentrate on for now.
 
             # We need to find out what level we are at - count to lowest frame
             level = 0
             frame = exc_traceback.tb_frame
@@ -356,27 +364,27 @@
 
         def task(self):
             import sys
             try:
                 1/0
             except ZeroDivisionError:
                 exc_type, exc_value, exc_traceback = sys.exc_info()
-                self.exc_traceback = exc_traceback
+                self.exc_value = exc_value
                 self.sync = 1
                 while self.sync:
                     pass
                 self.sync = 1
 
         self.sync = 0
         _thread.start_new_thread(task, (self,))
         while not self.sync:
             pass
-        exc_traceback = self.exc_traceback
-        rel = str(self.relation(root, exc_traceback))
-        self.asis(eval(rel % 'root'), exc_traceback)
+        exc_value = self.exc_value
+        rel = str(self.relation(root, exc_value))
+        self.asis(eval(rel % 'root'), exc_value)
         self.sync = 0
         while not self.sync:
             pass
 
         def task(self):
             self.test_1()
             self.sync = 1
@@ -761,15 +769,19 @@
 
         it = iter(shp)
         a = list(it)
         it.isatend = 0
         b = list(it)
         self.aseq(str(a), str(b))
 
-        self.aseq(o.getvalue(), """\
+        # The sort order is based on the source set's byid partition (see
+        # Path.PathsIter.reset), which sorts based on the size, then render
+        # (see Part.IdentityPartition.__init__)
+        if sys.getsizeof(y) > sys.getsizeof(ob):
+            self.aseq(o.getvalue(), """\
  0: hpy().Root.i0_sysdict
  0: Src.i0_modules['sys'].__dict__
  0: hpy().Root.i0_sysdict
  0: hpy().Root.i0_sysdict
  0: Src[0][0][0]
  0: Src[0][0][0]
  0: Src[0]
@@ -777,14 +789,31 @@
  0: <1 list: <address>*1>[0]
  0: <1 list: <address>*1>[0]
  0: <1 list: <address>*1>[0]
  1: <1 __main__.O: <address>>.x
  0: <1 list: <address>*1>[0]
  1: <1 __main__.O: <address>>.x
 """.replace('__main__', self.__module__))
+        else:
+            self.aseq(o.getvalue(), """\
+ 0: hpy().Root.i0_sysdict
+ 0: Src.i0_modules['sys'].__dict__
+ 0: hpy().Root.i0_sysdict
+ 0: hpy().Root.i0_sysdict
+ 0: Src[0][0][0]
+ 0: Src[0][0][0]
+ 0: Src[0]
+ 0: Src.x
+ 0: <1 list: <address>*1>[0]
+ 0: <1 list: <address>*1>[0]
+ 0: <1 __main__.O: <address>>.x
+ 1: <1 list: <address>*1>[0]
+ 0: <1 __main__.O: <address>>.x
+ 1: <1 list: <address>*1>[0]
+""".replace('__main__', self.__module__))
 
     def test_2(self):
         # To assist interactivity,
         # the more attribute is defined to return an object which
         # the repr() of gives more lines; and has a similar more attribute.
         # Testing this functionality here.
 
@@ -930,14 +959,27 @@
  6: Src[6]
  7: Src[7]
  8: Src[8]
  9: Src[9]
 10: Src[10]
 """)
 
+    def test_comparison(self):
+        # Test that non-compariable keys won't crash
+        # output order may be arbitrary not the output is not tested
+
+        iso = self.iso
+        dst = []
+
+        shp = iso(dst).get_shpaths(iso({0: dst, '': dst}))
+        str(shp)
+
+        shp = iso(dst).get_shpaths(iso({object(): dst, object(): dst}))
+        str(shp)
+
 
 def run_test(case, debug=0):
     support.run_unittest(case, debug)
 
 
 def test_main(debug=0):
     run_test(NewTestCase, debug)
```

### Comparing `guppy3-3.1.2/guppy/heapy/test/test_all.py` & `guppy3-3.1.3/guppy/heapy/test/test_all.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/test/test_View.py` & `guppy3-3.1.3/guppy/heapy/test/test_View.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/test/test_Part.py` & `guppy3-3.1.3/guppy/heapy/test/test_Part.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/test/test_OutputHandling.py` & `guppy3-3.1.3/guppy/heapy/test/test_OutputHandling.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/test/test_ER.py` & `guppy3-3.1.3/guppy/heapy/test/test_ER.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,16 +228,15 @@
             cref = [c]
             cref.append(cref)
             c.cref = cref
 
             hp = self.heapy.Use
             hp.reprefix = 'hp.'
 
-            import sys
-            s = hp.iso(C.__dict__, C, c, c.__dict__, d, sys)
+            s = hp.iso(C.__dict__, C, c, c.__dict__, d, inspect)
 
             for pre in (
                 'Unity',
                 'Clodo',
                 'Id',
                 'Module',
                 'Prod',
```

### Comparing `guppy3-3.1.2/guppy/heapy/test/test_sf.py` & `guppy3-3.1.3/guppy/heapy/test/test_sf.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/test/test_heapyc.py` & `guppy3-3.1.3/guppy/heapy/test/test_heapyc.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/test/test_menuleak.py` & `guppy3-3.1.3/guppy/heapy/test/test_menuleak.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/test/test_RefPat.py` & `guppy3-3.1.3/guppy/heapy/test/test_RefPat.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,16 +417,21 @@
         b = {'dst': dst}
 
         src = (a, b)
 
         gc.collect()
         rp = self.rp(dst, src, depth=10)
         rp.mod.View._is_clear_drg_enabled = 0  # Note Apr 19 2005
-        self.asis(rp.a.theone, b)
-        self.asis(rp.b.theone, a.__dict__)
+
+        if sys.getsizeof(b) > sys.getsizeof(a.__dict__):
+            self.asis(rp.a.theone, b)
+            self.asis(rp.b.theone, a.__dict__)
+        else:
+            self.asis(rp.a.theone, a.__dict__)
+            self.asis(rp.b.theone, b)
 
         # Test that the dict is eventually automatically removed from dictowners -
         # First test that dictowners is nonzero
 
         ln = len(rp.mod.View.dict_ownership)
         self.assertTrue(ln > 0)
```

### Comparing `guppy3-3.1.2/guppy/heapy/test/test_UniSet.py` & `guppy3-3.1.3/guppy/heapy/test/test_UniSet.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/test/support.py` & `guppy3-3.1.3/guppy/heapy/test/support.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/test/test_Classifiers.py` & `guppy3-3.1.3/guppy/heapy/test/test_Classifiers.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/View.py` & `guppy3-3.1.3/guppy/heapy/View.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/guppy/heapy/Classifiers.py` & `guppy3-3.1.3/guppy/heapy/Classifiers.py`

 * *Files identical despite different names*

### Comparing `guppy3-3.1.2/setup.py` & `guppy3-3.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
               "guppy.etc",
               "guppy.gsl",
               "guppy.heapy",
               "guppy.heapy.test",
               "guppy.sets",
           ],
           ext_modules=[setsc, heapyc],
-          python_requires='>=3.6',
+          python_requires='>=3.7',
           classifiers=[
               "Programming Language :: Python :: 3",
               "Programming Language :: Python :: Implementation :: CPython",
               "Programming Language :: C",
               "License :: OSI Approved :: MIT License",
               "Operating System :: OS Independent",
               "Development Status :: 4 - Beta",
```

