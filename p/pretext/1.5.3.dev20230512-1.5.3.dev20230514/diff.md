# Comparing `tmp/pretext-1.5.3.dev20230512.tar.gz` & `tmp/pretext-1.5.3.dev20230514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.5.3.dev20230512.tar", max compression
+gzip compressed data, was "pretext-1.5.3.dev20230514.tar", max compression
```

## Comparing `pretext-1.5.3.dev20230512.tar` & `pretext-1.5.3.dev20230514.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35148 2023-05-12 06:17:38.213245 pretext-1.5.3.dev20230512/LICENSE
--rw-r--r--   0        0        0     9664 2023-05-12 06:17:38.217245 pretext-1.5.3.dev20230512/README.md
--rw-r--r--   0        0        0     1440 2023-05-12 06:18:17.865734 pretext-1.5.3.dev20230512/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-05-12 06:17:38.217245 pretext-1.5.3.dev20230512/pretext/__main__.py
--rw-r--r--   0        0        0     7344 2023-05-12 06:17:38.217245 pretext-1.5.3.dev20230512/pretext/build.py
--rw-r--r--   0        0        0    22954 2023-05-12 06:17:38.217245 pretext-1.5.3.dev20230512/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-05-12 06:17:38.217245 pretext-1.5.3.dev20230512/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-05-12 06:17:38.217245 pretext-1.5.3.dev20230512/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-05-12 06:17:38.217245 pretext-1.5.3.dev20230512/pretext/core/__init__.py
--rw-r--r--   0        0        0   172432 2023-05-12 06:18:22.921793 pretext-1.5.3.dev20230512/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-05-12 06:17:38.217245 pretext-1.5.3.dev20230512/pretext/core/resources.py
--rw-r--r--   0        0        0  1026617 2023-05-12 06:18:22.921793 pretext-1.5.3.dev20230512/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-05-12 06:17:38.217245 pretext-1.5.3.dev20230512/pretext/generate.py
--rw-r--r--   0        0        0    24172 2023-05-12 06:17:38.217245 pretext-1.5.3.dev20230512/pretext/project.py
--rw-r--r--   0        0        0      516 2023-05-12 06:17:38.217245 pretext-1.5.3.dev20230512/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-05-12 06:18:22.997793 pretext-1.5.3.dev20230512/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-05-12 06:18:22.997793 pretext-1.5.3.dev20230512/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160171 2023-05-12 06:18:22.973793 pretext-1.5.3.dev20230512/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7677 2023-05-12 06:18:22.961793 pretext-1.5.3.dev20230512/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173370 2023-05-12 06:18:22.997793 pretext-1.5.3.dev20230512/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     1236 2023-05-12 06:18:22.997793 pretext-1.5.3.dev20230512/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4718 2023-05-12 06:18:22.977793 pretext-1.5.3.dev20230512/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0      630 2023-05-12 06:18:22.997793 pretext-1.5.3.dev20230512/pretext/templates/resources/postCreateCommand.sh
--rw-r--r--   0        0        0     1710 2023-05-12 06:18:22.997793 pretext-1.5.3.dev20230512/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-05-12 06:18:22.997793 pretext-1.5.3.dev20230512/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8453 2023-05-12 06:18:22.981793 pretext-1.5.3.dev20230512/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18300 2023-05-12 06:17:38.217245 pretext-1.5.3.dev20230512/pretext/utils.py
--rw-r--r--   0        0        0     1119 2023-05-12 06:18:17.865734 pretext-1.5.3.dev20230512/pyproject.toml
--rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.3.dev20230512/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-05-14 06:16:50.248904 pretext-1.5.3.dev20230514/LICENSE
+-rw-r--r--   0        0        0     9664 2023-05-14 06:16:50.248904 pretext-1.5.3.dev20230514/README.md
+-rw-r--r--   0        0        0     1440 2023-05-14 06:17:27.341256 pretext-1.5.3.dev20230514/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-14 06:16:50.252904 pretext-1.5.3.dev20230514/pretext/__main__.py
+-rw-r--r--   0        0        0     7344 2023-05-14 06:16:50.252904 pretext-1.5.3.dev20230514/pretext/build.py
+-rw-r--r--   0        0        0    22954 2023-05-14 06:16:50.252904 pretext-1.5.3.dev20230514/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-05-14 06:16:50.252904 pretext-1.5.3.dev20230514/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-05-14 06:16:50.252904 pretext-1.5.3.dev20230514/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-05-14 06:16:50.252904 pretext-1.5.3.dev20230514/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172432 2023-05-14 06:17:32.321297 pretext-1.5.3.dev20230514/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-05-14 06:16:50.252904 pretext-1.5.3.dev20230514/pretext/core/resources.py
+-rw-r--r--   0        0        0  1029053 2023-05-14 06:17:32.321297 pretext-1.5.3.dev20230514/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-05-14 06:16:50.252904 pretext-1.5.3.dev20230514/pretext/generate.py
+-rw-r--r--   0        0        0    24172 2023-05-14 06:16:50.252904 pretext-1.5.3.dev20230514/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-05-14 06:16:50.252904 pretext-1.5.3.dev20230514/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-05-14 06:17:32.397297 pretext-1.5.3.dev20230514/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-14 06:17:32.397297 pretext-1.5.3.dev20230514/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160171 2023-05-14 06:17:32.373297 pretext-1.5.3.dev20230514/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7677 2023-05-14 06:17:32.361297 pretext-1.5.3.dev20230514/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173370 2023-05-14 06:17:32.397297 pretext-1.5.3.dev20230514/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     1236 2023-05-14 06:17:32.397297 pretext-1.5.3.dev20230514/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4718 2023-05-14 06:17:32.377297 pretext-1.5.3.dev20230514/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0      630 2023-05-14 06:17:32.397297 pretext-1.5.3.dev20230514/pretext/templates/resources/postCreateCommand.sh
+-rw-r--r--   0        0        0     1710 2023-05-14 06:17:32.397297 pretext-1.5.3.dev20230514/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-05-14 06:17:32.397297 pretext-1.5.3.dev20230514/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8453 2023-05-14 06:17:32.381297 pretext-1.5.3.dev20230514/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18300 2023-05-14 06:16:50.252904 pretext-1.5.3.dev20230514/pretext/utils.py
+-rw-r--r--   0        0        0     1119 2023-05-14 06:17:27.345256 pretext-1.5.3.dev20230514/pyproject.toml
+-rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.3.dev20230514/PKG-INFO
```

### Comparing `pretext-1.5.3.dev20230512/LICENSE` & `pretext-1.5.3.dev20230514/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/README.md` & `pretext-1.5.3.dev20230514/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/__init__.py` & `pretext-1.5.3.dev20230514/pretext/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
 
-CORE_COMMIT = '2ba910e55643be1d1b8ac0e4403d10df1481af65'
+CORE_COMMIT = 'b9a68fd34e5ffbdfd7e2935aee68d066e671874f'
 
 
 def activate():
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.5.3.dev20230512/pretext/build.py` & `pretext-1.5.3.dev20230514/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/cli.py` & `pretext-1.5.3.dev20230514/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/codechat.py` & `pretext-1.5.3.dev20230514/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/config/xml_overlay.py` & `pretext-1.5.3.dev20230514/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/core/pretext.py` & `pretext-1.5.3.dev20230514/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/core/resources.py` & `pretext-1.5.3.dev20230514/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/core/resources.zip` & `pretext-1.5.3.dev20230514/pretext/core/resources.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,142 +1,142 @@
-Zip file size: 1026617 bytes, number of entries: 140
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-May-12 06:18 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-May-12 06:18 script/mbx
--rw-r--r--  2.0 unx       92 b- defN 23-May-12 06:18 script/mjsre/update-sre
--rw-r--r--  2.0 unx      481 b- defN 23-May-12 06:18 script/mjsre/README.md
--rw-r--r--  2.0 unx      116 b- defN 23-May-12 06:18 script/mjsre/package.json
--rw-r--r--  2.0 unx     9251 b- defN 23-May-12 06:18 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx    18421 b- defN 23-May-12 06:18 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    57973 b- defN 23-May-12 06:18 schema/pretext.rnc
--rw-r--r--  2.0 unx    25290 b- defN 23-May-12 06:18 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx   133930 b- defN 23-May-12 06:18 schema/pretext.xml
--rw-r--r--  2.0 unx     1180 b- defN 23-May-12 06:18 schema/README.md
--rw-r--r--  2.0 unx   124610 b- defN 23-May-12 06:18 schema/pretext.xsd
--rw-r--r--  2.0 unx      326 b- defN 23-May-12 06:18 schema/xml.xsd
--rw-r--r--  2.0 unx    34210 b- defN 23-May-12 06:18 schema/pretext-dev.rng
--rw-r--r--  2.0 unx   101444 b- defN 23-May-12 06:18 schema/pretext.rng
--rw-r--r--  2.0 unx    17587 b- defN 23-May-12 06:18 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx     3135 b- defN 23-May-12 06:18 schema/build.sh
--rw-r--r--  2.0 unx     1367 b- defN 23-May-12 06:18 pretext/README.md
--rw-r--r--  2.0 unx   172432 b- defN 23-May-12 06:18 pretext/pretext.py
--rw-r--r--  2.0 unx     1955 b- defN 23-May-12 06:18 pretext/module-test.py
--rw-r--r--  2.0 unx    30908 b- defN 23-May-12 06:18 pretext/pretext
--rw-r--r--  2.0 unx        0 b- defN 23-May-12 06:18 pretext/__init__.py
--rw-r--r--  2.0 unx    35057 b- defN 23-May-12 06:18 pretext/braille_format.py
--rw-r--r--  2.0 unx     2566 b- defN 23-May-12 06:18 pretext/pretext.cfg
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 xsl/utilities/
--rw-r--r--  2.0 unx     9787 b- defN 23-May-12 06:18 xsl/entities.ent
--rw-r--r--  2.0 unx     3239 b- defN 23-May-12 06:18 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-May-12 06:18 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-May-12 06:18 xsl/README.md
--rw-r--r--  2.0 unx   139486 b- defN 23-May-12 06:18 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-May-12 06:18 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-May-12 06:18 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-May-12 06:18 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-May-12 06:18 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-May-12 06:18 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   261852 b- defN 23-May-12 06:18 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   103788 b- defN 23-May-12 06:18 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-May-12 06:18 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-May-12 06:18 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-May-12 06:18 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   540859 b- defN 23-May-12 06:18 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-May-12 06:18 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-May-12 06:18 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-May-12 06:18 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-May-12 06:18 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-May-12 06:18 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-May-12 06:18 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx   111553 b- defN 23-May-12 06:18 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-May-12 06:18 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-May-12 06:18 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx   544780 b- defN 23-May-12 06:18 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-May-12 06:18 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-May-12 06:18 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-May-12 06:18 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    72788 b- defN 23-May-12 06:18 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-May-12 06:18 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-May-12 06:18 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-May-12 06:18 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx   605788 b- defN 23-May-12 06:18 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-May-12 06:18 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-May-12 06:18 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-May-12 06:18 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-May-12 06:18 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-May-12 06:18 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-May-12 06:18 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-May-12 06:18 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-May-12 06:18 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-May-12 06:18 xsl/latex/pretext-latex-guide.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 23-May-12 06:18 xsl/support/README.md
--rw-r--r--  2.0 unx    10306 b- defN 23-May-12 06:18 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-May-12 06:18 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-May-12 06:18 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-May-12 06:18 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5800 b- defN 23-May-12 06:18 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     5065 b- defN 23-May-12 06:18 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     2657 b- defN 23-May-12 06:18 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx      722 b- defN 23-May-12 06:18 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     6621 b- defN 23-May-12 06:18 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    16518 b- defN 23-May-12 06:18 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-May-12 06:18 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-May-12 06:18 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-May-12 06:18 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-May-12 06:18 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-May-12 06:18 xsl/localizations/README.md
--rw-r--r--  2.0 unx    15938 b- defN 23-May-12 06:18 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-May-12 06:18 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-May-12 06:18 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-May-12 06:18 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-May-12 06:18 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx     2227 b- defN 23-May-12 06:18 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    15736 b- defN 23-May-12 06:18 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-May-12 06:18 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-May-12 06:18 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-May-12 06:18 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-May-12 06:18 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx     1810 b- defN 23-May-12 06:18 xsl/utilities/README.md
--rw-r--r--  2.0 unx    30257 b- defN 23-May-12 06:18 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-May-12 06:18 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-May-12 06:18 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-May-12 06:18 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-May-12 06:18 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     1276 b- defN 23-May-12 06:18 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     7761 b- defN 23-May-12 06:18 css/style_default.css
--rw-r--r--  2.0 unx     3473 b- defN 23-May-12 06:18 css/style_soundwriting.css
--rw-r--r--  2.0 unx    63664 b- defN 23-May-12 06:18 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     1865 b- defN 23-May-12 06:18 css/README.md
--rw-r--r--  2.0 unx     1280 b- defN 23-May-12 06:18 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-12 06:18 css/colors_blue_red.css
--rw-r--r--  2.0 unx   435680 b- defN 23-May-12 06:18 css/mathbook-3.css
--rw-r--r--  2.0 unx   146685 b- defN 23-May-12 06:18 css/mathbook-content.css
--rw-r--r--  2.0 unx    22438 b- defN 23-May-12 06:18 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-12 06:18 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-12 06:18 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     4308 b- defN 23-May-12 06:18 css/colors_blue_green.css
--rw-r--r--  2.0 unx    71198 b- defN 23-May-12 06:18 css/pretext_add_on.css
--rw-r--r--  2.0 unx     2608 b- defN 23-May-12 06:18 css/colors_default.css
--rw-r--r--  2.0 unx     2438 b- defN 23-May-12 06:18 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-12 06:18 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2446 b- defN 23-May-12 06:18 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-12 06:18 css/colors_orange_navy.css
--rw-r--r--  2.0 unx    12567 b- defN 23-May-12 06:18 css/style_oscarlevin.css
--rw-r--r--  2.0 unx      691 b- defN 23-May-12 06:18 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     1338 b- defN 23-May-12 06:18 css/colors_red_blue.css
--rw-r--r--  2.0 unx    14069 b- defN 23-May-12 06:18 css/setcolors.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-12 06:18 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     2446 b- defN 23-May-12 06:18 css/colors_martiansands.css
--rw-r--r--  2.0 unx     1362 b- defN 23-May-12 06:18 css/epub.css
--rw-r--r--  2.0 unx     2441 b- defN 23-May-12 06:18 css/kindle.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-12 06:18 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     4021 b- defN 23-May-12 06:18 css/update_css
-140 files, 4796443 bytes uncompressed, 1009289 bytes compressed:  79.0%
+Zip file size: 1029053 bytes, number of entries: 140
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-May-14 06:17 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-May-14 06:17 script/mbx
+-rw-r--r--  2.0 unx       92 b- defN 23-May-14 06:17 script/mjsre/update-sre
+-rw-r--r--  2.0 unx      481 b- defN 23-May-14 06:17 script/mjsre/README.md
+-rw-r--r--  2.0 unx      116 b- defN 23-May-14 06:17 script/mjsre/package.json
+-rw-r--r--  2.0 unx     9251 b- defN 23-May-14 06:17 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx    18421 b- defN 23-May-14 06:17 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    58086 b- defN 23-May-14 06:17 schema/pretext.rnc
+-rw-r--r--  2.0 unx    25290 b- defN 23-May-14 06:17 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx   134043 b- defN 23-May-14 06:17 schema/pretext.xml
+-rw-r--r--  2.0 unx     1180 b- defN 23-May-14 06:17 schema/README.md
+-rw-r--r--  2.0 unx   125135 b- defN 23-May-14 06:17 schema/pretext.xsd
+-rw-r--r--  2.0 unx      326 b- defN 23-May-14 06:17 schema/xml.xsd
+-rw-r--r--  2.0 unx    34210 b- defN 23-May-14 06:17 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx   101829 b- defN 23-May-14 06:17 schema/pretext.rng
+-rw-r--r--  2.0 unx    17587 b- defN 23-May-14 06:17 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx     3135 b- defN 23-May-14 06:17 schema/build.sh
+-rw-r--r--  2.0 unx     1367 b- defN 23-May-14 06:17 pretext/README.md
+-rw-r--r--  2.0 unx   172432 b- defN 23-May-14 06:17 pretext/pretext.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-May-14 06:17 pretext/module-test.py
+-rw-r--r--  2.0 unx    30908 b- defN 23-May-14 06:17 pretext/pretext
+-rw-r--r--  2.0 unx        0 b- defN 23-May-14 06:17 pretext/__init__.py
+-rw-r--r--  2.0 unx    35449 b- defN 23-May-14 06:17 pretext/braille_format.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-May-14 06:17 pretext/pretext.cfg
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 xsl/utilities/
+-rw-r--r--  2.0 unx     9787 b- defN 23-May-14 06:17 xsl/entities.ent
+-rw-r--r--  2.0 unx     3239 b- defN 23-May-14 06:17 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-May-14 06:17 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-May-14 06:17 xsl/README.md
+-rw-r--r--  2.0 unx   139486 b- defN 23-May-14 06:17 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-May-14 06:17 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-May-14 06:17 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-May-14 06:17 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-May-14 06:17 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-May-14 06:17 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx   261852 b- defN 23-May-14 06:17 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   103788 b- defN 23-May-14 06:17 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-May-14 06:17 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-May-14 06:17 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-May-14 06:17 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   540859 b- defN 23-May-14 06:17 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-May-14 06:17 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-May-14 06:17 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-May-14 06:17 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-May-14 06:17 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-May-14 06:17 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-May-14 06:17 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx   111553 b- defN 23-May-14 06:17 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-May-14 06:17 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-May-14 06:17 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx   544780 b- defN 23-May-14 06:17 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-14 06:17 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-May-14 06:17 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-May-14 06:17 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    84474 b- defN 23-May-14 06:17 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-May-14 06:17 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-May-14 06:17 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-May-14 06:17 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx   605788 b- defN 23-May-14 06:17 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-May-14 06:17 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-May-14 06:17 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-May-14 06:17 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-May-14 06:17 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-May-14 06:17 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-May-14 06:17 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-May-14 06:17 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-May-14 06:17 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-May-14 06:17 xsl/latex/pretext-latex-guide.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 23-May-14 06:17 xsl/support/README.md
+-rw-r--r--  2.0 unx    10306 b- defN 23-May-14 06:17 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-May-14 06:17 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-May-14 06:17 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-May-14 06:17 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5800 b- defN 23-May-14 06:17 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     5065 b- defN 23-May-14 06:17 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     2657 b- defN 23-May-14 06:17 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx      722 b- defN 23-May-14 06:17 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     6621 b- defN 23-May-14 06:17 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    16518 b- defN 23-May-14 06:17 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-May-14 06:17 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-May-14 06:17 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-May-14 06:17 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-May-14 06:17 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-May-14 06:17 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    15938 b- defN 23-May-14 06:17 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-May-14 06:17 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-May-14 06:17 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-May-14 06:17 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-May-14 06:17 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx     2227 b- defN 23-May-14 06:17 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    15736 b- defN 23-May-14 06:17 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-May-14 06:17 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-May-14 06:17 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-May-14 06:17 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-May-14 06:17 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx     1810 b- defN 23-May-14 06:17 xsl/utilities/README.md
+-rw-r--r--  2.0 unx    30257 b- defN 23-May-14 06:17 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-May-14 06:17 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-May-14 06:17 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4299 b- defN 23-May-14 06:17 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-May-14 06:17 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     1276 b- defN 23-May-14 06:17 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-May-14 06:17 css/style_default.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-May-14 06:17 css/style_soundwriting.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-May-14 06:17 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-May-14 06:17 css/README.md
+-rw-r--r--  2.0 unx     1280 b- defN 23-May-14 06:17 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-14 06:17 css/colors_blue_red.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-May-14 06:17 css/mathbook-3.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-May-14 06:17 css/mathbook-content.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-May-14 06:17 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-14 06:17 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-14 06:17 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-May-14 06:17 css/colors_blue_green.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-May-14 06:17 css/pretext_add_on.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-May-14 06:17 css/colors_default.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-May-14 06:17 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-14 06:17 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-14 06:17 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-14 06:17 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-May-14 06:17 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx      691 b- defN 23-May-14 06:17 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-May-14 06:17 css/colors_red_blue.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-May-14 06:17 css/setcolors.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-14 06:17 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-14 06:17 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-May-14 06:17 css/epub.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-May-14 06:17 css/kindle.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-14 06:17 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-May-14 06:17 css/update_css
+140 files, 4809657 bytes uncompressed, 1011725 bytes compressed:  79.0%
```

#### schema/pretext.rnc

```diff
@@ -812,14 +812,15 @@
                         TextLong |
                         LongLine+ |
                         Paragraph+
                     )
                 }
             TableRow =
                 element row {
+                    attribute header {"yes" | "no"}?,
                     AlignmentHorizontal?,
                     AlignmentVertical?,
                     BorderBottom?,
                     BorderLeft?,
                     TableCell+
                 }
             TableColumn =
@@ -830,14 +831,15 @@
                     attribute width {text}?
                 }
             Tabular =
                 element tabular {
                     PermanentID?,
                     attribute width {text}?,
                     attribute margins {text}?,
+                    attribute row-headers {"yes" | "no"}?,
                     AlignmentHorizontal?,
                     AlignmentVertical?,
                     BorderTop?,
                     BorderBottom?,
                     BorderLeft?,
                     BorderRight?,
                     TableColumn*,
```

#### schema/pretext.xml

##### schema/pretext.xml

```diff
@@ -1997,14 +1997,15 @@
                         TextLong |
                         LongLine+ |
                         Paragraph+
                     )
                 }
             TableRow =
                 element row {
+                    attribute header {&quot;yes&quot; | &quot;no&quot;}?,
                     AlignmentHorizontal?,
                     AlignmentVertical?,
                     BorderBottom?,
                     BorderLeft?,
                     TableCell+
                 }
             TableColumn =
@@ -2015,14 +2016,15 @@
                     attribute width {text}?
                 }
             Tabular =
                 element tabular {
                     PermanentID?,
                     attribute width {text}?,
                     attribute margins {text}?,
+                    attribute row-headers {&quot;yes&quot; | &quot;no&quot;}?,
                     AlignmentHorizontal?,
                     AlignmentVertical?,
                     BorderTop?,
                     BorderBottom?,
                     BorderLeft?,
                     BorderRight?,
                     TableColumn*,
```

#### schema/pretext.xsd

##### schema/pretext.xsd

```diff
@@ -1881,14 +1881,22 @@
     </xs:complexType>
   </xs:element>
   <xs:element name="row">
     <xs:complexType>
       <xs:sequence>
         <xs:element maxOccurs="unbounded" ref="cell"/>
       </xs:sequence>
+      <xs:attribute name="header">
+        <xs:simpleType>
+          <xs:restriction base="xs:token">
+            <xs:enumeration value="yes"/>
+            <xs:enumeration value="no"/>
+          </xs:restriction>
+        </xs:simpleType>
+      </xs:attribute>
       <xs:attribute name="halign">
         <xs:simpleType>
           <xs:restriction base="xs:token">
             <xs:enumeration value="left"/>
             <xs:enumeration value="center"/>
             <xs:enumeration value="right"/>
             <xs:enumeration value="justify"/>
@@ -1930,14 +1938,22 @@
       <xs:sequence>
         <xs:element minOccurs="0" maxOccurs="unbounded" ref="col"/>
         <xs:element maxOccurs="unbounded" ref="row"/>
       </xs:sequence>
       <xs:attribute name="permid"/>
       <xs:attribute name="width"/>
       <xs:attribute name="margins"/>
+      <xs:attribute name="row-headers">
+        <xs:simpleType>
+          <xs:restriction base="xs:token">
+            <xs:enumeration value="yes"/>
+            <xs:enumeration value="no"/>
+          </xs:restriction>
+        </xs:simpleType>
+      </xs:attribute>
       <xs:attribute name="halign">
         <xs:simpleType>
           <xs:restriction base="xs:token">
             <xs:enumeration value="left"/>
             <xs:enumeration value="center"/>
             <xs:enumeration value="right"/>
             <xs:enumeration value="justify"/>
```

#### schema/pretext.rng

##### schema/pretext.rng

```diff
@@ -2083,14 +2083,22 @@
         </oneOrMore>
       </choice>
     </element>
   </define>
   <define name="TableRow">
     <element name="row">
       <optional>
+        <attribute name="header">
+          <choice>
+            <value>yes</value>
+            <value>no</value>
+          </choice>
+        </attribute>
+      </optional>
+      <optional>
         <ref name="AlignmentHorizontal"/>
       </optional>
       <optional>
         <ref name="AlignmentVertical"/>
       </optional>
       <optional>
         <ref name="BorderBottom"/>
@@ -2127,14 +2135,22 @@
       <optional>
         <attribute name="width"/>
       </optional>
       <optional>
         <attribute name="margins"/>
       </optional>
       <optional>
+        <attribute name="row-headers">
+          <choice>
+            <value>yes</value>
+            <value>no</value>
+          </choice>
+        </attribute>
+      </optional>
+      <optional>
         <ref name="AlignmentHorizontal"/>
       </optional>
       <optional>
         <ref name="AlignmentVertical"/>
       </optional>
       <optional>
         <ref name="BorderTop"/>
```

#### pretext/braille_format.py

```diff
@@ -658,14 +658,16 @@
         children = list(sxml)
         for c in children:
             if c.text:
                 if 'punctuation' in c.attrib:
                     math_punctuation = c.attrib['punctuation']
                 else:
                     math_punctuation = None
+                # Following can help debug nested segments
+                # print("SUSPECT TYPEFACE", c.tag, c.text)
                 self.write_fragment(c.tag, c.text, math_punctuation, s)
             if c.tail:
                 self.write_fragment("text", c.tail, None, s)
 
         # Release width restriction to finish ToC entry
         if self.toc_mode:
             self.adjust_text_width(6)
@@ -858,17 +860,20 @@
         elif typeface == "italic":
             typeforms = [1] * len(aline)
         elif typeface == "bold":
             typeforms = [4] * len(aline)
         elif typeface == "code":
             typeforms = [BRF.trans1_bit] * len(aline)
         else:
-            print("BUG: did not recognize typeface", typeface)
-            # Just to keep going while developing, if necessary
-            # typeforms = None
+            print('BUG: did not recognize typeface "{}"'.format(typeface) )
+            # When this error message reports "segment" as the typeface,
+            # it means there are nested segments.  Search this module for
+            # "SUSPECT TYPEFACE" to find a useful debugging statement to use.
+            # Setting "typeforms = None" here can keep processing alive but is
+            # likely to lead to incorrect reesults.
 
         return louis.translateString(tableList, aline, typeforms, 0)
 
     # End BRF object definition
 
 
 # Current entry point, sort of
```

#### xsl/pretext-braille-preprint.xsl

##### xsl/pretext-braille-preprint.xsl

```diff
@@ -141,16 +141,27 @@
   <!--     @lines-following - default: 0, else positive integer               -->
   <!-- This is the main event, hidden within the formulation of a  -->
   <!-- variable holding an RTF.  This is formed by the totality of -->
   <!-- non-modal templates.  It will be converted into a node set, -->
   <!-- for a post-processing step to incorporate "runin"           -->
   <!-- title/heading elements into a subsequent segment.           -->
   <xsl:variable name="segmented-rtf">
+    <xsl:call-template name="warning-unimplemented"/>
+    <xsl:call-template name="missing-warning"/>
     <xsl:apply-templates select="$root"/>
   </xsl:variable>
+  <!-- And we sneak in a warning that this conversion is underway, but not complete. -->
+  <xsl:template name="warning-unimplemented">
+    <xsl:message>** Some PreTeXt elements lack full implementation in the braille conversion.</xsl:message>
+    <xsl:message>** Smaller items will simply be missing from your output.</xsl:message>
+    <xsl:message>** Larger items may have all-caps placeholders in your output.</xsl:message>
+    <xsl:message>** These will all be reported as &quot;Overlooked&quot; in the log.</xsl:message>
+    <xsl:message>** Please report the complete list in the PreTeXt support forum,</xsl:message>
+    <xsl:message>** so we can prioritize making the output for your project complete.</xsl:message>
+  </xsl:template>
   <!-- The entry template "waits" for the "$math-meld-rtf" and    -->
   <!-- "$segmented-rtf" global variables to form, then the actual -->
   <!-- output is a run of modal "meld-runin" templates as a sort  -->
   <!-- of post-processing step.                                   -->
   <xsl:template match="/">
     <xsl:apply-templates select="exsl:node-set($segmented-rtf)/brf" mode="meld-runin"/>
   </xsl:template>
@@ -804,16 +815,16 @@
   <!-- ##### -->
   <!-- Lists -->
   <!-- ##### -->
   <!-- Lists are containers full of list items.  All by   -->
   <!-- themselves they have no real impact on the braille -->
   <!-- output.  The list items are another matter.        -->
   <!-- 2023-04-06: very prelimnary, e.g. no runover       -->
+  <!-- 2023-04-10: excessive nesting => excessive run-in  -->
   <xsl:template match="ul|ol|dl">
-    <!-- <segment>LIST</segment> -->
     <xsl:apply-templates select="li"/>
   </xsl:template>
   <xsl:template match="li">
     <!-- Marker as a "runin" element -->
     <runin indentation="0" separator=" ">
       <xsl:choose>
         <xsl:when test="parent::ol">
@@ -996,14 +1007,26 @@
     <!-- recurse if there is more to do -->
     <xsl:if test="following-sibling::cell">
       <xsl:apply-templates select="following-sibling::cell" mode="describe-column-headings">
         <xsl:with-param name="prior-column-number" select="$last-column"/>
       </xsl:apply-templates>
     </xsl:if>
   </xsl:template>
+  <!-- A "p" normally becomes a "segment".  But an entire row of a "tabular" -->
+  <!-- is a segment and we can't nest them.  So we just dribble out the      -->
+  <!-- entire "p" without any indentation or anything, so it becomes one     -->
+  <!-- very long cell in the braille.  Worse, two "p" in a cell will just    -->
+  <!-- get concatenated and the distinction between the two will be lost.    -->
+  <xsl:template match="cell/p">
+    <xsl:apply-templates select="node()"/>
+    <!-- At least provide a space between consecutive "p" -->
+    <xsl:if test="following-sibling::p">
+      <xsl:text/>
+    </xsl:if>
+  </xsl:template>
   <!-- ########## -->
   <!-- References -->
   <!-- ########## -->
   <!-- Bibliography [BANA-2016, 22.2.1]                           -->
   <!-- Bibliographic items in a "references" division have a      -->
   <!-- bracketed number leading each new entry, then two spaces   -->
   <!-- of indentation for the remainder .                         -->
@@ -1046,42 +1069,150 @@
   </xsl:template>
   <xsl:template match="ie">
     <xsl:text>i.e.</xsl:text>
   </xsl:template>
   <xsl:template match="etc">
     <xsl:text>etc.</xsl:text>
   </xsl:template>
-  <xsl:template match="copyright">
-    <xsl:text>(c)</xsl:text>
-  </xsl:template>
-  <!-- [BANA-2016] Appendix G                 -->
-  <!-- Says UEB uses three periods (dots-256) -->
-  <!-- liblouis seems to translate as such    -->
-  <xsl:template match="ellipsis">
-    <xsl:text>...</xsl:text>
-  </xsl:template>
   <!-- Empty Elements, Characters -->
-  <!-- Unicode Character 'NO-BREAK SPACE' (U+00A0)     -->
-  <!-- yields a template for "nbsp" in -common         -->
-  <!-- liblouis seems to pass this through in-kind     -->
-  <!-- Used in teh manufacture of a cross-reference,   -->
-  <!--we'll want to strip just before it eds up in BRF -->
+  <!-- Generally Unicode values get translated into UEB equivalents  -->
+  <!-- by liblouis.  This is based on a reading of                   -->
+  <!--                                                               -->
+  <!--     /usr/share/liblouis/tables/en-ueb-chardefs.uti            -->
+  <!--                                                               -->
+  <!-- which is incorporated via the English-UEB Grade 1 and Grade 2 -->
+  <!-- tables.  As of 2023-05-12.  We document the Unicode character -->
+  <!-- and the cells described in the liblouis table.                -->
+  <!-- Unicode Character 'NO-BREAK SPACE' (U+00A0)   -->
+  <!-- yields a template for "nbsp" in -common       -->
+  <!-- liblouis seems to pass this through in-kind   -->
+  <!-- Used in the manufacture of a cross-reference, -->
+  <!-- we will want to strip just before it ends up  -->
+  <!-- in BRF .                                      -->
   <xsl:template name="nbsp-character">
     <xsl:text/>
   </xsl:template>
   <!-- Unicode Character 'EN DASH' (U+2013) -->
-  <!-- Seems to become ",-"                 -->
+  <!-- Liblouis: 6-36                       -->
   <xsl:template name="ndash-character">
     <xsl:text>–</xsl:text>
   </xsl:template>
   <!-- Unicode Character 'EM DASH' (U+2014) -->
-  <!-- Seems to also become ",-"            -->
+  <!-- Liblouis: 6-36                       -->
   <xsl:template name="mdash-character">
     <xsl:text>—</xsl:text>
   </xsl:template>
+  <!-- Unicode Character 'COPYRIGHT SIGN' (U+00A9) -->
+  <!-- Liblouis: 45-14                             -->
+  <xsl:template name="copyright-character">
+    <xsl:text>©</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'REGISTERED SIGN' (U+00AE) -->
+  <!-- Liblouis: 45-1235                            -->
+  <xsl:template name="registered-character">
+    <xsl:text>®</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'TRADE MARK SIGN' (U+2122) -->
+  <!-- Liblouis: 45-2345                            -->
+  <xsl:template name="trademark-character">
+    <xsl:text>™</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'DEGREE SIGN' (U+00B0) -->
+  <!-- Liblouis: 45-245                         -->
+  <xsl:template name="degree-character">
+    <xsl:text>°</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'PRIME' (U+2032) -->
+  <!-- Liblouis: 2356                     -->
+  <xsl:template name="prime-character">
+    <xsl:text>′</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'DOUBLE PRIME' (U+2033) -->
+  <!-- Liblouis: 2356-2356                       -->
+  <xsl:template name="dblprime-character">
+    <xsl:text>″</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'LEFT SINGLE QUOTATION MARK' (U+2018) -->
+  <!-- Liblouis: 6-236                                         -->
+  <xsl:template name="lsq-character">
+    <xsl:text>‘</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'RIGHT SINGLE QUOTATION MARK' (U+2019) -->
+  <!-- Liblouis: 6-356                                          -->
+  <xsl:template name="rsq-character">
+    <xsl:text>’</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'LEFT DOUBLE QUOTATION MARK' (U+201C) -->
+  <!-- Liblouis: 236                                           -->
+  <xsl:template name="lq-character">
+    <xsl:text>“</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'RIGHT DOUBLE QUOTATION MARK' (U+201D) -->
+  <!-- Liblouis: 356                                            -->
+  <xsl:template name="rq-character">
+    <xsl:text>”</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'LEFT ANGLE BRACKET' (U+3008) -->
+  <!-- Liblouis: 4-126                                 -->
+  <xsl:template name="langle-character">
+    <xsl:text>〈</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'RIGHT ANGLE BRACKET' (U+3009) -->
+  <!-- Liblouis: 4-345                                  -->
+  <xsl:template name="rangle-character">
+    <xsl:text>〉</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'HORIZONTAL ELLIPSIS' (U+2026) -->
+  <!-- Liblouis: 256-256-256                            -->
+  <!-- [BANA-2016] Appendix G, UEB is three periods/256 -->
+  <xsl:template name="ellipsis-character">
+    <xsl:text>…</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'MIDDLE DOT' (U+00B7) -->
+  <!-- Liblouis: 4-16                          -->
+  <xsl:template name="midpoint-character">
+    <xsl:text>·</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'PILCROW SIGN' (U+00B6) -->
+  <!-- Liblouis: 45-1234                         -->
+  <xsl:template name="pilcrow-character">
+    <xsl:text>¶</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'SECTION SIGN' (U+00A7) -->
+  <!-- Liblouis: 45-234                          -->
+  <xsl:template name="section-mark-character">
+    <xsl:text>§</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'MINUS SIGN' (U+2212) -->
+  <!-- Liblouis: 5-36                          -->
+  <xsl:template name="minus-character">
+    <xsl:text>−</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'MULTIPLICATION SIGN' (U+00D7) -->
+  <!-- Liblouis: 5-236                                  -->
+  <xsl:template name="times-character">
+    <xsl:text>×</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'DIVISION SIGN' (U+00F7) -->
+  <!-- Liblouis: 5-34                             -->
+  <xsl:template name="obelus-character">
+    <xsl:text>÷</xsl:text>
+  </xsl:template>
+  <!-- Unicode Character 'PLUS-MINUS SIGN' (U+00B1) -->
+  <!-- Liblouis: 456-235                            -->
+  <xsl:template name="plusminus-character">
+    <xsl:text>±</xsl:text>
+  </xsl:template>
+  <!-- ############ -->
+  <!-- Font Changes -->
+  <!-- ############ -->
+  <!-- Certain PreTeXt groupings in running text naturally yield just  -->
+  <!-- a font change.  Braille and liblouis have facilities for italic -->
+  <!-- and bold.  This is "internal" markup that eventually gets       -->
+  <!-- interpreted by  lxml  in Python.                                -->
   <!-- Italics -->
   <xsl:template match="em|foreign|articletitle|pubtitle">
     <!-- Python will assume "italic" as element name -->
     <italic>
       <xsl:apply-templates select="node()"/>
     </italic>
   </xsl:template>
@@ -1114,28 +1245,15 @@
   </xsl:template>
   <!-- "idx" must be dealt with from source otherwise during    -->
   <!-- index construction, but when encountered in a paragraph  -->
   <!-- or a block they should just be killed.  Should never     -->
   <!-- reach an interior "h".  Entirely similar for "notation"  -->
   <!-- and an interior "usage", and "description".              -->
   <xsl:template match="idx|notation"/>
-  <!-- non-breaking space -->
-  <!-- will liblouis preserve? -->
-  <!-- or do we need markup for page-formatting? -->
-  <!-- Groupings -->
-  <xsl:template match="q">
-    <xsl:text>&quot;</xsl:text>
-    <xsl:apply-templates select="node()"/>
-    <xsl:text>&quot;</xsl:text>
-  </xsl:template>
-  <xsl:template match="sq">
-    <xsl:text>'</xsl:text>
-    <xsl:apply-templates select="node()"/>
-    <xsl:text>'</xsl:text>
-  </xsl:template>
+  <!-- Documenting PreText itself -->
   <xsl:template match="tag">
     <xsl:text>&lt;</xsl:text>
     <xsl:value-of select="."/>
     <xsl:text>&gt;</xsl:text>
   </xsl:template>
   <xsl:template match="tage">
     <xsl:text>&lt;</xsl:text>
@@ -1408,26 +1526,14 @@
               <xsl:apply-templates select="$rightward"/>
             </segment>
           </xsl:if>
         </xsl:otherwise>
       </xsl:choose>
     </xsl:for-each>
   </xsl:template>
-  <!-- segment with placeholder content at this stage -->
-  <xsl:template match="cd">
-    <segment>CODE DISPLAY</segment>
-  </xsl:template>
-  <!-- segment with placeholder content at this stage -->
-  <xsl:template match="pre">
-    <segment>PREFORMATTED TEXT</segment>
-  </xsl:template>
-  <!-- segment with placeholder content at this stage -->
-  <xsl:template match="program">
-    <segment>PROGRAM</segment>
-  </xsl:template>
   <!-- We support books and articles, though nothing in particular -->
   <!-- needs to be done at these root elements.  Yet?              -->
   <xsl:template match="book|article">
     <xsl:apply-templates select="*"/>
   </xsl:template>
   <!-- "docinfo" should *always* be mined directly for pieces that affect output -->
   <xsl:template match="docinfo"/>
@@ -1451,32 +1557,194 @@
   <!-- These elements have full implementations in -common, or       -->
   <!-- partial/abstract implementations which we extend hee.         -->
   <!-- So we just hit them with "apply-imports" so they do not       -->
   <!-- all into the (temporary, development) template below          -->
   <!-- reporting missed elements.   "Commenting out this template    -->
   <!-- should have zero effect, except to generate more debugging    -->
   <!-- messages, since this reporting template will take precedence. -->
-  <xsl:template match="nbsp|ndash|mdash|xref">
+  <!-- "apply-imports" items necessary during development -->
+  <!-- nbsp, ndash, mdash characters defined above -->
+  <xsl:template match="nbsp|ndash|mdash">
+    <xsl:apply-imports/>
+  </xsl:template>
+  <!-- empty elements, characters, defined above -->
+  <xsl:template match="copyright|registered|trademark|degree|prime|dblprime|lsq|rsq|lq|rq|langle|rangle|ellipsis|midpoint|pilcrow|section-mark|minus|times|obelus|plusminus">
+    <xsl:apply-imports/>
+  </xsl:template>
+  <!-- These elements/characters lack translations in liblouis.      -->
+  <!-- We get/use their versions in -common, which will throw an     -->
+  <!-- "unimplemented character" warning, which is accurate now,     -->
+  <!-- *and* accurate later when the "overlooked" warning goes away. -->
+  <!-- As characters get implemented, move to above template         -->
+  <!-- (in proper order) as a way to keep track of the situation.    -->
+  <xsl:template match="phonomark|copyleft|servicemark|ldblbracket|rdblbracket|swungdash|permille|solidus">
+    <xsl:apply-imports/>
+  </xsl:template>
+  <!-- Groupings, based on characters defined above -->
+  <!-- dblbrackets raises warnings since left/right -->
+  <!-- characters are not implemented               -->
+  <xsl:template match="q|sq|dblbrackets|angles">
+    <xsl:apply-imports/>
+  </xsl:template>
+  <!-- xref-number, xref-link defined above -->
+  <xsl:template match="xref">
+    <xsl:apply-imports/>
+  </xsl:template>
+  <!-- pure text in -common -->
+  <xsl:template match="today|timeofday">
+    <xsl:apply-imports/>
+  </xsl:template>
+  <!-- Latin Abbreviations -->
+  <!-- Fully defined as text in -common, including an "abbreviation-period" -->
+  <xsl:template match="ad|am|bc|ca|eg|etal|etc|ie|nb|pm|ps|vs|viz">
     <xsl:apply-imports/>
   </xsl:template>
   <!-- titles get killed in -common so we don't need to see them here -->
   <xsl:template match="title|subtitle|shorttitle|plaintitle|creator">
     <xsl:apply-imports/>
   </xsl:template>
   <!-- captions get killed in -common so we don't need to see them here -->
   <xsl:template match="caption">
     <xsl:apply-imports/>
   </xsl:template>
-  <!-- *Every* element needs an implementation, or it ends up here being -->
-  <!-- reported as overlooked.  This is temporary during development.    -->
-  <xsl:template match="*">
+  <!-- Larger structures, needing implementation, *along with* interior -->
+  <!-- structures.  We report AND include a textual place holder.       -->
+  <xsl:template match="sage">
+    <xsl:text>SAGECELL</xsl:text>
+  </xsl:template>
+  <xsl:template match="notation-list">
+    <xsl:text>NOTATIONLIST</xsl:text>
+  </xsl:template>
+  <xsl:template match="index-list">
+    <xsl:text>INDEXLIST</xsl:text>
+  </xsl:template>
+  <xsl:template match="cd">
+    <segment>CODE DISPLAY</segment>
+  </xsl:template>
+  <xsl:template match="pre">
+    <segment>PREFORMATTED TEXT</segment>
+  </xsl:template>
+  <xsl:template match="program">
+    <segment>PROGRAM</segment>
+  </xsl:template>
+  <xsl:template match="console">
+    <segment>CONSOLE</segment>
+  </xsl:template>
+  <xsl:template match="poem">
+    <segment>POEM</segment>
+  </xsl:template>
+  <!-- Next three are not structures, so as "text" -->
+  <xsl:template match="quantity">
+    <xsl:text>QUANTITY</xsl:text>
+  </xsl:template>
+  <xsl:template match="kbd"/>
+  <xsl:template match="icon">
+    <xsl:text>ICON</xsl:text>
+  </xsl:template>
+  <xsl:template name="missing-warning">
+    <xsl:if test="//sage">
+      <xsl:call-template name="missing-implementation">
+        <xsl:with-param name="element" select="'sage'"/>
+        <xsl:with-param name="ntimes" select="count(//sage)"/>
+      </xsl:call-template>
+    </xsl:if>
+    <!--  -->
+    <xsl:if test="//notation-list">
+      <xsl:call-template name="missing-implementation">
+        <xsl:with-param name="element" select="'notation-list'"/>
+        <xsl:with-param name="ntimes" select="count(//notation-list)"/>
+      </xsl:call-template>
+    </xsl:if>
+    <!--  -->
+    <xsl:if test="//index-list">
+      <xsl:call-template name="missing-implementation">
+        <xsl:with-param name="element" select="'index-list'"/>
+        <xsl:with-param name="ntimes" select="count(//index-list)"/>
+      </xsl:call-template>
+    </xsl:if>
+    <!--  -->
+    <xsl:if test="//cd">
+      <xsl:call-template name="missing-implementation">
+        <xsl:with-param name="element" select="'cd'"/>
+        <xsl:with-param name="ntimes" select="count(//cd)"/>
+      </xsl:call-template>
+    </xsl:if>
+    <!--  -->
+    <xsl:if test="//pre">
+      <xsl:call-template name="missing-implementation">
+        <xsl:with-param name="element" select="'pre'"/>
+        <xsl:with-param name="ntimes" select="count(//pre)"/>
+      </xsl:call-template>
+    </xsl:if>
+    <!--  -->
+    <xsl:if test="//program">
+      <xsl:call-template name="missing-implementation">
+        <xsl:with-param name="element" select="'program'"/>
+        <xsl:with-param name="ntimes" select="count(//program)"/>
+      </xsl:call-template>
+    </xsl:if>
+    <!--  -->
+    <xsl:if test="//console">
+      <xsl:call-template name="missing-implementation">
+        <xsl:with-param name="element" select="'console'"/>
+        <xsl:with-param name="ntimes" select="count(//console)"/>
+      </xsl:call-template>
+    </xsl:if>
+    <!--  -->
+    <xsl:if test="//poem">
+      <xsl:call-template name="missing-implementation">
+        <xsl:with-param name="element" select="'poem'"/>
+        <xsl:with-param name="ntimes" select="count(//poem)"/>
+      </xsl:call-template>
+    </xsl:if>
+    <!--  -->
+    <xsl:if test="//quantity">
+      <xsl:call-template name="missing-implementation">
+        <xsl:with-param name="element" select="'quantity'"/>
+        <xsl:with-param name="ntimes" select="count(//quantity)"/>
+      </xsl:call-template>
+    </xsl:if>
+    <!--  -->
+    <xsl:if test="//kbd">
+      <xsl:call-template name="missing-implementation">
+        <xsl:with-param name="element" select="'kbd'"/>
+        <xsl:with-param name="ntimes" select="count(//kbd)"/>
+      </xsl:call-template>
+    </xsl:if>
+    <!--  -->
+    <xsl:if test="//icon">
+      <xsl:call-template name="missing-implementation">
+        <xsl:with-param name="element" select="'icon'"/>
+        <xsl:with-param name="ntimes" select="count(//icon)"/>
+      </xsl:call-template>
+    </xsl:if>
+    <!--  -->
+  </xsl:template>
+  <xsl:template name="missing-implementation">
+    <xsl:param name="element"/>
+    <xsl:param name="ntimes"/>
+    <xsl:message>
+      Unimplemented:
+      <xsl:value-of select="$element"/>
+      (
+      <xsl:value-of select="$ntimes"/>
+      times)
+    </xsl:message>
+  </xsl:template>
+  <xsl:template match="*" mode="overlooked">
     <xsl:message>
       Overlooked:
       <xsl:value-of select="local-name()"/>
     </xsl:message>
+  </xsl:template>
+  <!-- *Every* element needs an implementation, or it ends up here being -->
+  <!-- reported as overlooked.  This is temporary during development.    -->
+  <xsl:template match="*">
+    <xsl:apply-templates select="." mode="overlooked"/>
+    <!-- <xsl:message>Overlooked: <xsl:value-of select="local-name()"/></xsl:message> -->
     <!-- recurse into child elements to find more "missing" elements -->
     <xsl:apply-templates select="*"/>
   </xsl:template>
   <!-- ######### -->
   <!-- Utilities -->
   <!-- ######### -->
   <!-- Transcriber Notes -->
```

### Comparing `pretext-1.5.3.dev20230512/pretext/generate.py` & `pretext-1.5.3.dev20230514/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/project.py` & `pretext-1.5.3.dev20230514/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/templates/__init__.py` & `pretext-1.5.3.dev20230514/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/templates/resources/.gitignore` & `pretext-1.5.3.dev20230514/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/templates/resources/article.zip` & `pretext-1.5.3.dev20230514/pretext/templates/resources/article.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 160171 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 source/
--rw-r--r--  2.0 unx       86 b- defN 23-May-12 06:17 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-12 06:18 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-12 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-12 06:18 .gitignore
--rw-r--r--  2.0 unx   154806 b- defN 23-May-12 06:17 assets/frog.jpg
--rw-r--r--  2.0 unx     1236 b- defN 23-May-12 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-12 06:18 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx      242 b- defN 23-May-12 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-May-12 06:17 source/main.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-May-12 06:17 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-May-12 06:17 source/section-2.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 source/
+-rw-r--r--  2.0 unx       86 b- defN 23-May-14 06:16 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-14 06:17 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-14 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-14 06:17 .gitignore
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-14 06:16 assets/frog.jpg
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-14 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-14 06:17 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx      242 b- defN 23-May-14 06:16 publication/publication.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-May-14 06:16 source/main.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-May-14 06:16 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-May-14 06:16 source/section-2.ptx
 15 files, 164515 bytes uncompressed, 158505 bytes compressed:  3.7%
```

### Comparing `pretext-1.5.3.dev20230512/pretext/templates/resources/book.zip` & `pretext-1.5.3.dev20230514/pretext/templates/resources/book.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 7677 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 source/
--rw-r--r--  2.0 unx       82 b- defN 23-May-12 06:17 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-12 06:18 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-12 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-12 06:18 .gitignore
--rw-r--r--  2.0 unx     1236 b- defN 23-May-12 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-12 06:18 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     6114 b- defN 23-May-12 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-May-12 06:17 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-May-14 06:16 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-14 06:17 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-14 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-14 06:17 .gitignore
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-14 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-14 06:17 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     6114 b- defN 23-May-14 06:16 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-May-14 06:16 source/main.ptx
 11 files, 15483 bytes uncompressed, 6439 bytes compressed:  58.4%
```

### Comparing `pretext-1.5.3.dev20230512/pretext/templates/resources/demo.zip` & `pretext-1.5.3.dev20230514/pretext/templates/resources/demo.zip`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,37 +1,37 @@
 Zip file size: 173370 bytes, number of entries: 35
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 source/
--rw-r--r--  2.0 unx       82 b- defN 23-May-12 06:17 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-12 06:18 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-12 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-12 06:18 .gitignore
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-May-12 06:17 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-May-12 06:17 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     1236 b- defN 23-May-12 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-12 06:18 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     6092 b- defN 23-May-12 06:17 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 source/images/
--rw-r--r--  2.0 unx      847 b- defN 23-May-12 06:17 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-May-12 06:17 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-May-12 06:17 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-May-12 06:17 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-May-12 06:17 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-May-12 06:17 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-May-12 06:17 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-May-12 06:17 source/frontmatter.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-May-12 06:17 source/ch-features.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-May-12 06:17 source/ch-generate.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-May-12 06:17 source/sec-features.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-May-12 06:17 source/backmatter.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-May-12 06:17 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-May-12 06:17 source/ch-empty.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-May-12 06:17 source/ex-first.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-May-12 06:17 source/docinfo.ptx
--rw-r--r--  2.0 unx       10 b- defN 23-May-12 06:17 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-May-12 06:17 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 23-May-12 06:17 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-May-12 06:17 source/images/sageplot3d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-May-14 06:16 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-14 06:17 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-14 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-14 06:17 .gitignore
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-14 06:16 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-May-14 06:16 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-14 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-14 06:17 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     6092 b- defN 23-May-14 06:16 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 source/images/
+-rw-r--r--  2.0 unx      847 b- defN 23-May-14 06:16 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-May-14 06:16 source/main.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-May-14 06:16 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-May-14 06:16 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-May-14 06:16 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-May-14 06:16 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-May-14 06:16 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-May-14 06:16 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-May-14 06:16 source/ch-features.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-May-14 06:16 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-May-14 06:16 source/sec-features.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-May-14 06:16 source/backmatter.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-May-14 06:16 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-May-14 06:16 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-May-14 06:16 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-May-14 06:16 source/docinfo.ptx
+-rw-r--r--  2.0 unx       10 b- defN 23-May-14 06:16 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-May-14 06:16 source/images/cflag.asy
+-rw-r--r--  2.0 unx      357 b- defN 23-May-14 06:16 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 23-May-14 06:16 source/images/sageplot3d.sage
 35 files, 189778 bytes uncompressed, 169270 bytes compressed:  10.8%
```

### Comparing `pretext-1.5.3.dev20230512/pretext/templates/resources/devcontainer.json` & `pretext-1.5.3.dev20230514/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/templates/resources/hello.zip` & `pretext-1.5.3.dev20230514/pretext/templates/resources/hello.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 4718 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 source/
--rw-r--r--  2.0 unx       69 b- defN 23-May-12 06:17 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-May-12 06:17 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-12 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-12 06:18 .gitignore
--rw-r--r--  2.0 unx     1236 b- defN 23-May-12 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-12 06:18 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx      242 b- defN 23-May-12 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-May-12 06:17 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 source/
+-rw-r--r--  2.0 unx       69 b- defN 23-May-14 06:16 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-May-14 06:16 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-14 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-14 06:17 .gitignore
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-14 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-14 06:17 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx      242 b- defN 23-May-14 06:16 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-May-14 06:16 source/main.ptx
 11 files, 7494 bytes uncompressed, 3480 bytes compressed:  53.6%
```

### Comparing `pretext-1.5.3.dev20230512/pretext/templates/resources/postCreateCommand.sh` & `pretext-1.5.3.dev20230514/pretext/templates/resources/postCreateCommand.sh`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/templates/resources/project.ptx` & `pretext-1.5.3.dev20230514/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pretext/templates/resources/slideshow.zip` & `pretext-1.5.3.dev20230514/pretext/templates/resources/slideshow.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 8453 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 06:17 xsl/
--rw-r--r--  2.0 unx      784 b- defN 23-May-12 06:17 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-12 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-12 06:18 .gitignore
--rw-r--r--  2.0 unx     1236 b- defN 23-May-12 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-12 06:18 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx      190 b- defN 23-May-12 06:17 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-May-12 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-May-12 06:17 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 06:16 xsl/
+-rw-r--r--  2.0 unx      784 b- defN 23-May-14 06:16 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-14 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-14 06:17 .gitignore
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-14 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      630 b- defN 23-May-14 06:17 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx      190 b- defN 23-May-14 06:16 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 23-May-14 06:16 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-May-14 06:16 source/main.ptx
 12 files, 20081 bytes uncompressed, 7121 bytes compressed:  64.5%
```

### Comparing `pretext-1.5.3.dev20230512/pretext/utils.py` & `pretext-1.5.3.dev20230514/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230512/pyproject.toml` & `pretext-1.5.3.dev20230514/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.5.3.dev20230512"
+version = "1.5.3.dev20230514"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.5.3.dev20230512/PKG-INFO` & `pretext-1.5.3.dev20230514/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.5.3.dev20230512
+Version: 1.5.3.dev20230514
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

