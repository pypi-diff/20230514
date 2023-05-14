# Comparing `tmp/ocrmypdf-9.8.1.tar.gz` & `tmp/ocrmypdf-9.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ocrmypdf-9.8.1.tar", last modified: Thu May 28 23:15:02 2020, max compression
+gzip compressed data, was "dist/ocrmypdf-9.8.2.tar", last modified: Wed Jun  3 21:59:50 2020, max compression
```

## Comparing `ocrmypdf-9.8.1.tar` & `ocrmypdf-9.8.2.tar`

### file list

```diff
@@ -1,455 +1,455 @@
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/
--rw-r--r--   0 vsts      (1001) docker     (116)      313 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/.coveragerc
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/.docker/
--rw-r--r--   0 vsts      (1001) docker     (116)     1820 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/.docker/Dockerfile
--rw-r--r--   0 vsts      (1001) docker     (116)      243 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/.dockerignore
--rw-r--r--   0 vsts      (1001) docker     (116)       22 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/.git_archival.txt
--rw-r--r--   0 vsts      (1001) docker     (116)      282 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/.gitattributes
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/.github/
--rw-r--r--   0 vsts      (1001) docker     (116)      675 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/.github/FUNDING.yml
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 vsts      (1001) docker     (116)     1338 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 vsts      (1001) docker     (116)      467 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 vsts      (1001) docker     (116)     1219 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/.github/issue_template.md
--rw-r--r--   0 vsts      (1001) docker     (116)      554 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (116)      714 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/.pre-commit-config.yaml
--rw-r--r--   0 vsts      (1001) docker     (116)      107 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/.readthedocs.yml
--rw-r--r--   0 vsts      (1001) docker     (116)    35149 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (116)     9459 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)     6743 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (116)     8972 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/azure-pipelines.yml
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/debian/
--rw-r--r--   0 vsts      (1001) docker     (116)    83597 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/debian/copyright
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/docs/
--rw-r--r--   0 vsts      (1001) docker     (116)    13244 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/advanced.rst
--rw-r--r--   0 vsts      (1001) docker     (116)     3693 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/api.rst
--rw-r--r--   0 vsts      (1001) docker     (116)     8092 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/batch.rst
--rwxr-xr-x   0 vsts      (1001) docker     (116)    10673 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/conf.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1906 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/contributing.rst
--rw-r--r--   0 vsts      (1001) docker     (116)    11878 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/cookbook.rst
--rw-r--r--   0 vsts      (1001) docker     (116)     5657 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/docker.rst
--rw-r--r--   0 vsts      (1001) docker     (116)     1539 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/errors.rst
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/docs/images/
--rw-r--r--   0 vsts      (1001) docker     (116)     3197 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/images/bitmap_vs_svg.svg
--rw-r--r--   0 vsts      (1001) docker     (116)    31298 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/images/logo-social.png
--rw-r--r--   0 vsts      (1001) docker     (116)     9474 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/images/logo.svg
--rw-r--r--   0 vsts      (1001) docker     (116)    21644 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/images/macos-workflow.png
--rw-r--r--   0 vsts      (1001) docker     (116)      770 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/index.rst
--rw-r--r--   0 vsts      (1001) docker     (116)    24007 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/installation.rst
--rw-r--r--   0 vsts      (1001) docker     (116)     9970 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/introduction.rst
--rw-r--r--   0 vsts      (1001) docker     (116)     1949 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/jbig2.rst
--rw-r--r--   0 vsts      (1001) docker     (116)     2444 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/languages.rst
--rw-r--r--   0 vsts      (1001) docker     (116)     3201 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/optimizer.rst
--rw-r--r--   0 vsts      (1001) docker     (116)      668 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/performance.rst
--rw-r--r--   0 vsts      (1001) docker     (116)    25969 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/pipeline.svg
--rw-r--r--   0 vsts      (1001) docker     (116)      671 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/plugins.rst
--rw-r--r--   0 vsts      (1001) docker     (116)    68728 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/release_notes.rst
--rw-r--r--   0 vsts      (1001) docker     (116)     7374 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/docs/security.rst
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/misc/
--rw-r--r--   0 vsts      (1001) docker     (116)     1350 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/misc/batch.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/misc/completion/
--rw-r--r--   0 vsts      (1001) docker     (116)     3304 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/misc/completion/ocrmypdf.bash
--rw-r--r--   0 vsts      (1001) docker     (116)     6064 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/misc/completion/ocrmypdf.fish
--rw-r--r--   0 vsts      (1001) docker     (116)      353 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/misc/docker-compose.example.yml
--rw-r--r--   0 vsts      (1001) docker     (116)     2107 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/misc/synology.py
--rw-r--r--   0 vsts      (1001) docker     (116)     5293 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/misc/watcher.py
--rw-r--r--   0 vsts      (1001) docker     (116)     4577 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/misc/webservice.py
--rw-r--r--   0 vsts      (1001) docker     (116)      497 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/requirements/
--rw-r--r--   0 vsts      (1001) docker     (116)      295 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/requirements/main.txt
--rw-r--r--   0 vsts      (1001) docker     (116)      242 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/requirements/test.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       25 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/requirements/watcher.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       16 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/requirements/webservice.txt
--rw-r--r--   0 vsts      (1001) docker     (116)      638 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (116)     4402 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/ocrmypdf/
--rw-r--r--   0 vsts      (1001) docker     (116)     1200 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     2071 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (116)    10604 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/_graft.py
--rw-r--r--   0 vsts      (1001) docker     (116)     3967 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/_jobcontext.py
--rw-r--r--   0 vsts      (1001) docker     (116)    30508 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/_pipeline.py
--rw-r--r--   0 vsts      (1001) docker     (116)    15398 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/_sync.py
--rw-r--r--   0 vsts      (1001) docker     (116)     4456 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/_unicodefun.py
--rw-r--r--   0 vsts      (1001) docker     (116)    16044 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/_validation.py
--rw-r--r--   0 vsts      (1001) docker     (116)      842 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/_version.py
--rw-r--r--   0 vsts      (1001) docker     (116)     9382 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/api.py
--rw-r--r--   0 vsts      (1001) docker     (116)    16716 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/cli.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/ocrmypdf/data/
--rw-r--r--   0 vsts      (1001) docker     (116)     6922 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/data/sRGB.icc
--rw-r--r--   0 vsts      (1001) docker     (116)     3070 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/ocrmypdf/exec/
--rw-r--r--   0 vsts      (1001) docker     (116)     9560 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/exec/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)    11505 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/exec/ghostscript.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1731 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/exec/jbig2enc.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2000 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/exec/pngquant.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1636 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/exec/qpdf.py
--rw-r--r--   0 vsts      (1001) docker     (116)    12634 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/exec/tesseract.py
--rw-r--r--   0 vsts      (1001) docker     (116)     4589 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/exec/unpaper.py
--rw-r--r--   0 vsts      (1001) docker     (116)     4801 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/helpers.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)    13967 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/hocrtransform.py
--rw-r--r--   0 vsts      (1001) docker     (116)    30308 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/leptonica.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/ocrmypdf/lib/
--rw-r--r--   0 vsts      (1001) docker     (116)      745 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)    13694 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/lib/_leptonica.py
--rw-r--r--   0 vsts      (1001) docker     (116)    18388 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/lib/compile_leptonica.py
--rw-r--r--   0 vsts      (1001) docker     (116)    21951 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/optimize.py
--rw-r--r--   0 vsts      (1001) docker     (116)     4695 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/pdfa.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/ocrmypdf/pdfinfo/
--rw-r--r--   0 vsts      (1001) docker     (116)      779 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/pdfinfo/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     3549 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/pdfinfo/ghosttext.py
--rw-r--r--   0 vsts      (1001) docker     (116)    27625 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/pdfinfo/info.py
--rw-r--r--   0 vsts      (1001) docker     (116)     9285 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/pdfinfo/layout.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2134 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/src/ocrmypdf/quality.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/ocrmypdf.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (116)     9459 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/ocrmypdf.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)    20571 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/ocrmypdf.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/ocrmypdf.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       52 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/ocrmypdf.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/ocrmypdf.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (116)      141 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/ocrmypdf.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        9 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/src/ocrmypdf.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/2400dpi/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     4010 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      526 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/3small/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     3501 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      187 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     2962 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       40 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     4068 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      540 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/aspect/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     2018 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       37 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     2986 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       37 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cardinal/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    94534 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    10249 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    94534 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    11243 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     4556 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    94534 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    11513 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     4641 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    94534 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    12456 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     4635 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__osd__--psm__0__000001_rasterize_preview.jpg__stdout/
--rw-r--r--   0 vsts      (1001) docker     (116)       53 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__osd__--psm__0__000001_rasterize_preview.jpg__stdout/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      119 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__osd__--psm__0__000001_rasterize_preview.jpg__stdout/stdout.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__osd__--psm__0__000002_rasterize_preview.jpg__stdout/
--rw-r--r--   0 vsts      (1001) docker     (116)       53 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__osd__--psm__0__000002_rasterize_preview.jpg__stdout/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      122 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__osd__--psm__0__000002_rasterize_preview.jpg__stdout/stdout.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__osd__--psm__0__000003_rasterize_preview.jpg__stdout/
--rw-r--r--   0 vsts      (1001) docker     (116)       53 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__osd__--psm__0__000003_rasterize_preview.jpg__stdout/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      123 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__osd__--psm__0__000003_rasterize_preview.jpg__stdout/stdout.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__osd__--psm__0__000004_rasterize_preview.jpg__stdout/
--rw-r--r--   0 vsts      (1001) docker     (116)       53 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__osd__--psm__0__000004_rasterize_preview.jpg__stdout/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      122 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cardinal/__-l__osd__--psm__0__000004_rasterize_preview.jpg__stdout/stdout.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/ccitt/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    94530 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    10242 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cmyk/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     3610 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      336 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     3379 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       77 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     3073 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       77 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/francais/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/francais/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     3610 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/francais/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/francais/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/francais/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      336 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/francais/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/graph_ocred/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/graph_ocred/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     3610 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/graph_ocred/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/graph_ocred/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/graph_ocred/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      336 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/graph_ocred/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/graph_ocred/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     3309 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/graph_ocred/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/graph_ocred/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/graph_ocred/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      181 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/graph_ocred/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/jbig2/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    40166 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     1826 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     5909 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     1826 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     3610 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      336 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     1086 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        3 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     2860 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        3 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
--rw-r--r--   0 vsts      (1001) docker     (116)    34325 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/manifest.jsonl
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/multipage/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    28415 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       78 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     1137 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     5173 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       78 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     1137 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     2998 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       47 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    18024 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      425 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     4229 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      425 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    15960 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      362 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     3986 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      362 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    66109 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     3084 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     8535 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     3084 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    65948 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     3085 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     8060 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     3085 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/palette/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    37131 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       79 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     1666 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     5744 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       79 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     1666 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/poster/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    10842 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     4553 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/poster/__-l__osd__--psm__0__000001_rasterize_preview.jpg__stdout/
--rw-r--r--   0 vsts      (1001) docker     (116)       53 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/poster/__-l__osd__--psm__0__000001_rasterize_preview.jpg__stdout/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)      119 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/poster/__-l__osd__--psm__0__000001_rasterize_preview.jpg__stdout/stdout.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/skew/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)      702 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)     2798 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    90026 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     4545 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
--rw-r--r--   0 vsts      (1001) docker     (116)    12674 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
--rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
--rw-r--r--   0 vsts      (1001) docker     (116)     4545 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
--rw-r--r--   0 vsts      (1001) docker     (116)    10286 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/resources/
--rw-r--r--   0 vsts      (1001) docker     (116)   164306 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/2400dpi.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   165787 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/3small.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)     7203 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/README.rst
--rw-r--r--   0 vsts      (1001) docker     (116)    10733 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/acroform.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)     8874 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/aspect.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   139794 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/baiona.png
--rw-r--r--   0 vsts      (1001) docker     (116)   154331 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/baiona_alpha.png
--rw-r--r--   0 vsts      (1001) docker     (116)   148726 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/baiona_cmyk.jpg
--rw-r--r--   0 vsts      (1001) docker     (116)    50908 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/baiona_colormapped.png
--rw-r--r--   0 vsts      (1001) docker     (116)    57263 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/baiona_gray.png
--rw-r--r--   0 vsts      (1001) docker     (116)   781430 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/blank.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   185098 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/c02-22.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)    76875 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/cardinal.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   103856 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/ccitt.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   897087 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/cmyk.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   103292 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/congress.jpg
--rw-r--r--   0 vsts      (1001) docker     (116)     1374 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/crom.png
--rw-r--r--   0 vsts      (1001) docker     (116)    23966 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/encrypted_algo4.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   310761 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/enormous.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)    79979 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/epson.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)     2713 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/formxobject.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   483256 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/francais.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   296322 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/graph.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)    86459 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/graph_ocred.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)    11779 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/hugemono.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)       44 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/invalid.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)    20306 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/jbig2.pdf
--rwxr-xr-x   0 vsts      (1001) docker     (116)     4372 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/kcs.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)    44040 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/lichtenstein.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)    72954 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/link.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)    75273 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/linn.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   141404 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/linn.png
--rw-r--r--   0 vsts      (1001) docker     (116)     4567 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/linn.txt
--rw-r--r--   0 vsts      (1001) docker     (116)      537 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/livecycle.pdf
--rwxr-xr-x   0 vsts      (1001) docker     (116)   134593 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/masks.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)     1014 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/missing_docinfo.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)  1447072 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/multipage.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)     2717 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/negzero.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)      431 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/no_contents.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)    38153 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/overlay.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   750181 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/palette.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   694671 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/poster.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)    76401 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/rotated_skew.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   150846 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/skew-encrypted.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)    76013 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/skew.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)     9698 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/toc.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)      515 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/trivial.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)     7742 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/truetype_font_nomapping.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)     3967 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/type3_font_nomapping.pdf
--rw-r--r--   0 vsts      (1001) docker     (116)   104842 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/typewriter.png
--rw-r--r--   0 vsts      (1001) docker     (116)    38923 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/resources/vector.pdf
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-05-28 23:15:02.000000 ocrmypdf-9.8.1/tests/spoof/
--rw-r--r--   0 vsts      (1001) docker     (116)     1495 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/spoof/gs.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     1770 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/spoof/gs_feature_elision.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     2068 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/spoof/gs_pdfa_failure.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     1718 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/spoof/gs_raster_failure.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     1707 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/spoof/gs_render_failure.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     2592 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/spoof/tesseract_big_image_error.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     7089 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/spoof/tesseract_cache.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     2841 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/spoof/tesseract_crash.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     4720 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/spoof/tesseract_noop.py
--rwxr-xr-x   0 vsts      (1001) docker     (116)     1327 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/spoof/unpaper_oldversion.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1383 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_acroform.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2014 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_api.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1587 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_completion.py
--rw-r--r--   0 vsts      (1001) docker     (116)     4590 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_ghostscript.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1765 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_graft.py
--rw-r--r--   0 vsts      (1001) docker     (116)     3998 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1460 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_hocrtransform.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2857 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_image_input.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2785 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_lept.py
--rw-r--r--   0 vsts      (1001) docker     (116)    24128 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_main.py
--rw-r--r--   0 vsts      (1001) docker     (116)    11902 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (116)     5216 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_optimize.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2149 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_page_numbers.py
--rw-r--r--   0 vsts      (1001) docker     (116)     6081 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_pdfinfo.py
--rw-r--r--   0 vsts      (1001) docker     (116)     5465 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_preprocessing.py
--rw-r--r--   0 vsts      (1001) docker     (116)      874 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_qpdf.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1229 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_quality.py
--rw-r--r--   0 vsts      (1001) docker     (116)     8281 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_rotation.py
--rw-r--r--   0 vsts      (1001) docker     (116)     4106 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_stdio.py
--rw-r--r--   0 vsts      (1001) docker     (116)     5471 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_tess4.py
--rw-r--r--   0 vsts      (1001) docker     (116)     3579 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_unpaper.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1774 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_userunit.py
--rw-r--r--   0 vsts      (1001) docker     (116)     8045 2020-05-28 23:14:52.000000 ocrmypdf-9.8.1/tests/test_validation.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/
+-rw-r--r--   0 vsts      (1001) docker     (116)      313 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/.coveragerc
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/.docker/
+-rw-r--r--   0 vsts      (1001) docker     (116)     1820 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/.docker/Dockerfile
+-rw-r--r--   0 vsts      (1001) docker     (116)      243 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/.dockerignore
+-rw-r--r--   0 vsts      (1001) docker     (116)       22 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/.git_archival.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)      282 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/.gitattributes
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/.github/
+-rw-r--r--   0 vsts      (1001) docker     (116)      675 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/.github/FUNDING.yml
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 vsts      (1001) docker     (116)     1338 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 vsts      (1001) docker     (116)      467 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 vsts      (1001) docker     (116)     1219 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/.github/issue_template.md
+-rw-r--r--   0 vsts      (1001) docker     (116)      554 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (116)      714 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/.pre-commit-config.yaml
+-rw-r--r--   0 vsts      (1001) docker     (116)      107 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/.readthedocs.yml
+-rw-r--r--   0 vsts      (1001) docker     (116)    35149 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (116)     9459 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (116)     6743 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (116)     8972 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/azure-pipelines.yml
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/debian/
+-rw-r--r--   0 vsts      (1001) docker     (116)    83597 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/debian/copyright
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/docs/
+-rw-r--r--   0 vsts      (1001) docker     (116)    13244 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/advanced.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)     3693 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/api.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)     8092 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/batch.rst
+-rwxr-xr-x   0 vsts      (1001) docker     (116)    10673 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/conf.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1906 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/contributing.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)    11878 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/cookbook.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)     5657 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/docker.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)     1539 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/errors.rst
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/docs/images/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3197 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/images/bitmap_vs_svg.svg
+-rw-r--r--   0 vsts      (1001) docker     (116)    31298 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/images/logo-social.png
+-rw-r--r--   0 vsts      (1001) docker     (116)     9474 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/images/logo.svg
+-rw-r--r--   0 vsts      (1001) docker     (116)    21644 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/images/macos-workflow.png
+-rw-r--r--   0 vsts      (1001) docker     (116)      770 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)    25436 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/installation.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)     9970 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/introduction.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)     1949 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/jbig2.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)     2444 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/languages.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)     3201 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/optimizer.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)      668 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/performance.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)    25969 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/pipeline.svg
+-rw-r--r--   0 vsts      (1001) docker     (116)      671 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/plugins.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)    69021 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/release_notes.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)     7374 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/docs/security.rst
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/misc/
+-rw-r--r--   0 vsts      (1001) docker     (116)     1350 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/misc/batch.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/misc/completion/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3304 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/misc/completion/ocrmypdf.bash
+-rw-r--r--   0 vsts      (1001) docker     (116)     6064 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/misc/completion/ocrmypdf.fish
+-rw-r--r--   0 vsts      (1001) docker     (116)      353 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/misc/docker-compose.example.yml
+-rw-r--r--   0 vsts      (1001) docker     (116)     2107 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/misc/synology.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5293 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/misc/watcher.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4577 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/misc/webservice.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      497 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/requirements/
+-rw-r--r--   0 vsts      (1001) docker     (116)      295 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/requirements/main.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)      242 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/requirements/test.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       25 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/requirements/watcher.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       16 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/requirements/webservice.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)      638 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (116)     4402 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/ocrmypdf/
+-rw-r--r--   0 vsts      (1001) docker     (116)     1200 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (116)     2071 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    10604 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/_graft.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3967 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/_jobcontext.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    30508 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/_pipeline.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    15398 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/_sync.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4456 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/_unicodefun.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    16493 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/_validation.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      842 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     9382 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/api.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    16716 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/cli.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/ocrmypdf/data/
+-rw-r--r--   0 vsts      (1001) docker     (116)     6922 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/data/sRGB.icc
+-rw-r--r--   0 vsts      (1001) docker     (116)     3070 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/ocrmypdf/exec/
+-rw-r--r--   0 vsts      (1001) docker     (116)     9560 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/exec/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    11505 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/exec/ghostscript.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1731 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/exec/jbig2enc.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2000 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/exec/pngquant.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1636 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/exec/qpdf.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    12634 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/exec/tesseract.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4589 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/exec/unpaper.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4801 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/helpers.py
+-rwxr-xr-x   0 vsts      (1001) docker     (116)    13967 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/hocrtransform.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    30308 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/leptonica.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/ocrmypdf/lib/
+-rw-r--r--   0 vsts      (1001) docker     (116)      745 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    13694 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/lib/_leptonica.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    18388 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/lib/compile_leptonica.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    21951 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/optimize.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4695 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/pdfa.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/ocrmypdf/pdfinfo/
+-rw-r--r--   0 vsts      (1001) docker     (116)      779 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/pdfinfo/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3549 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/pdfinfo/ghosttext.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    27625 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/pdfinfo/info.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     9335 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/pdfinfo/layout.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2134 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/src/ocrmypdf/quality.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/ocrmypdf.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (116)     9459 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/ocrmypdf.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (116)    20571 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/ocrmypdf.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/ocrmypdf.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       52 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/ocrmypdf.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/ocrmypdf.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (116)      141 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/ocrmypdf.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        9 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/src/ocrmypdf.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/2400dpi/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     4010 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      526 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/3small/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3501 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      187 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     2962 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       40 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     4068 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      540 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/aspect/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     2018 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       37 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     2986 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       37 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cardinal/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    94534 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    10249 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    94534 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    11243 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     4556 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    94534 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    11513 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     4641 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    94534 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    12456 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     4635 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__osd__--psm__0__000001_rasterize_preview.jpg__stdout/
+-rw-r--r--   0 vsts      (1001) docker     (116)       53 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__osd__--psm__0__000001_rasterize_preview.jpg__stdout/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      119 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__osd__--psm__0__000001_rasterize_preview.jpg__stdout/stdout.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__osd__--psm__0__000002_rasterize_preview.jpg__stdout/
+-rw-r--r--   0 vsts      (1001) docker     (116)       53 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__osd__--psm__0__000002_rasterize_preview.jpg__stdout/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      122 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__osd__--psm__0__000002_rasterize_preview.jpg__stdout/stdout.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__osd__--psm__0__000003_rasterize_preview.jpg__stdout/
+-rw-r--r--   0 vsts      (1001) docker     (116)       53 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__osd__--psm__0__000003_rasterize_preview.jpg__stdout/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      123 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__osd__--psm__0__000003_rasterize_preview.jpg__stdout/stdout.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__osd__--psm__0__000004_rasterize_preview.jpg__stdout/
+-rw-r--r--   0 vsts      (1001) docker     (116)       53 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__osd__--psm__0__000004_rasterize_preview.jpg__stdout/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      122 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cardinal/__-l__osd__--psm__0__000004_rasterize_preview.jpg__stdout/stdout.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/ccitt/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    94530 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    10242 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     4558 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cmyk/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3610 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      336 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3379 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       77 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3073 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       77 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/francais/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/francais/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3610 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/francais/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/francais/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/francais/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      336 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/francais/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/graph_ocred/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/graph_ocred/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3610 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/graph_ocred/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/graph_ocred/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/graph_ocred/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      336 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/graph_ocred/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/graph_ocred/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3309 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/graph_ocred/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/graph_ocred/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/graph_ocred/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      181 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/graph_ocred/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/jbig2/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    40166 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     1826 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     5909 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     1826 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3610 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      336 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     1086 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        3 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     2860 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        3 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)    34325 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/manifest.jsonl
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/multipage/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    28415 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       78 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     1137 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     5173 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       78 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     1137 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     2998 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       47 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    18024 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      425 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     4229 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      425 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    15960 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      362 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     3986 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      362 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    66109 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     3084 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     8535 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     3084 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    65948 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     3085 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     8060 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     3085 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/palette/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    37131 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       79 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     1666 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     5744 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       79 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     1666 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/poster/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    10842 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     4553 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/poster/__-l__osd__--psm__0__000001_rasterize_preview.jpg__stdout/
+-rw-r--r--   0 vsts      (1001) docker     (116)       53 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/poster/__-l__osd__--psm__0__000001_rasterize_preview.jpg__stdout/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)      119 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/poster/__-l__osd__--psm__0__000001_rasterize_preview.jpg__stdout/stdout.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/skew/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)      702 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)     2798 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    90026 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     4545 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/
+-rw-r--r--   0 vsts      (1001) docker     (116)    12674 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)       55 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stderr.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/stdout.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)     4545 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin
+-rw-r--r--   0 vsts      (1001) docker     (116)    10286 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/resources/
+-rw-r--r--   0 vsts      (1001) docker     (116)   164306 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/2400dpi.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   165787 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/3small.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)     7203 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/README.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)    10733 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/acroform.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)     8874 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/aspect.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   139794 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/baiona.png
+-rw-r--r--   0 vsts      (1001) docker     (116)   154331 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/baiona_alpha.png
+-rw-r--r--   0 vsts      (1001) docker     (116)   148726 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/baiona_cmyk.jpg
+-rw-r--r--   0 vsts      (1001) docker     (116)    50908 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/baiona_colormapped.png
+-rw-r--r--   0 vsts      (1001) docker     (116)    57263 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/baiona_gray.png
+-rw-r--r--   0 vsts      (1001) docker     (116)   781430 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/blank.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   185098 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/c02-22.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)    76875 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/cardinal.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   103856 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/ccitt.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   897087 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/cmyk.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   103292 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/congress.jpg
+-rw-r--r--   0 vsts      (1001) docker     (116)     1374 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/crom.png
+-rw-r--r--   0 vsts      (1001) docker     (116)    23966 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/encrypted_algo4.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   310761 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/enormous.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)    79979 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/epson.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)     2713 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/formxobject.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   483256 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/francais.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   296322 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/graph.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)    86459 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/graph_ocred.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)    11779 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/hugemono.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)       44 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/invalid.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)    20306 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/jbig2.pdf
+-rwxr-xr-x   0 vsts      (1001) docker     (116)     4372 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/kcs.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)    44040 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/lichtenstein.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)    72954 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/link.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)    75273 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/linn.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   141404 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/linn.png
+-rw-r--r--   0 vsts      (1001) docker     (116)     4567 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/linn.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)      537 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/livecycle.pdf
+-rwxr-xr-x   0 vsts      (1001) docker     (116)   134593 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/masks.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)     1014 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/missing_docinfo.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)  1447072 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/multipage.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)     2717 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/negzero.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)      431 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/no_contents.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)    38153 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/overlay.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   750181 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/palette.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   694671 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/poster.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)    76401 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/rotated_skew.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   150846 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/skew-encrypted.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)    76013 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/skew.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)     9698 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/toc.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)      515 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/trivial.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)     7742 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/truetype_font_nomapping.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)     3967 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/type3_font_nomapping.pdf
+-rw-r--r--   0 vsts      (1001) docker     (116)   104842 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/typewriter.png
+-rw-r--r--   0 vsts      (1001) docker     (116)    38923 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/resources/vector.pdf
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-03 21:59:50.000000 ocrmypdf-9.8.2/tests/spoof/
+-rw-r--r--   0 vsts      (1001) docker     (116)     1495 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/spoof/gs.py
+-rwxr-xr-x   0 vsts      (1001) docker     (116)     1770 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/spoof/gs_feature_elision.py
+-rwxr-xr-x   0 vsts      (1001) docker     (116)     2068 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/spoof/gs_pdfa_failure.py
+-rwxr-xr-x   0 vsts      (1001) docker     (116)     1718 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/spoof/gs_raster_failure.py
+-rwxr-xr-x   0 vsts      (1001) docker     (116)     1707 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/spoof/gs_render_failure.py
+-rwxr-xr-x   0 vsts      (1001) docker     (116)     2592 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/spoof/tesseract_big_image_error.py
+-rwxr-xr-x   0 vsts      (1001) docker     (116)     7089 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/spoof/tesseract_cache.py
+-rwxr-xr-x   0 vsts      (1001) docker     (116)     2841 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/spoof/tesseract_crash.py
+-rwxr-xr-x   0 vsts      (1001) docker     (116)     4720 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/spoof/tesseract_noop.py
+-rwxr-xr-x   0 vsts      (1001) docker     (116)     1327 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/spoof/unpaper_oldversion.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1383 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_acroform.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2014 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_api.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1587 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_completion.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4590 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_ghostscript.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1765 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_graft.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3998 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1460 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_hocrtransform.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2857 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_image_input.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2785 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_lept.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    24128 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_main.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    11902 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5216 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_optimize.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2149 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_page_numbers.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     6081 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_pdfinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5465 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_preprocessing.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      874 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_qpdf.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1229 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_quality.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     8281 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_rotation.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4106 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_stdio.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5471 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_tess4.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3579 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_unpaper.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1774 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_userunit.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     8175 2020-06-03 21:59:38.000000 ocrmypdf-9.8.2/tests/test_validation.py
```

### Comparing `ocrmypdf-9.8.1/.docker/Dockerfile` & `ocrmypdf-9.8.2/.docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/.github/FUNDING.yml` & `ocrmypdf-9.8.2/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/.github/ISSUE_TEMPLATE/bug_report.md` & `ocrmypdf-9.8.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/.github/issue_template.md` & `ocrmypdf-9.8.2/.github/issue_template.md`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/.gitignore` & `ocrmypdf-9.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/.pre-commit-config.yaml` & `ocrmypdf-9.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/LICENSE` & `ocrmypdf-9.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/PKG-INFO` & `ocrmypdf-9.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocrmypdf
-Version: 9.8.1
+Version: 9.8.2
 Summary: OCRmyPDF adds an OCR text layer to scanned PDF files, allowing them to be searched
 Home-page: https://github.com/jbarlow83/OCRmyPDF
 Author: James R. Barlow
 Author-email: james@purplerock.ca
 License: UNKNOWN
 Project-URL: Documentation, https://ocrmypdf.readthedocs.io/
 Project-URL: Source, https://github.com/jbarlow83/ocrmypdf
```

### Comparing `ocrmypdf-9.8.1/README.md` & `ocrmypdf-9.8.2/README.md`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/azure-pipelines.yml` & `ocrmypdf-9.8.2/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/debian/copyright` & `ocrmypdf-9.8.2/debian/copyright`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/advanced.rst` & `ocrmypdf-9.8.2/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/api.rst` & `ocrmypdf-9.8.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/batch.rst` & `ocrmypdf-9.8.2/docs/batch.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/conf.py` & `ocrmypdf-9.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/contributing.rst` & `ocrmypdf-9.8.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/cookbook.rst` & `ocrmypdf-9.8.2/docs/cookbook.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/docker.rst` & `ocrmypdf-9.8.2/docs/docker.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/errors.rst` & `ocrmypdf-9.8.2/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/images/bitmap_vs_svg.svg` & `ocrmypdf-9.8.2/docs/images/bitmap_vs_svg.svg`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/images/logo-social.png` & `ocrmypdf-9.8.2/docs/images/logo-social.png`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/images/logo.svg` & `ocrmypdf-9.8.2/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/images/macos-workflow.png` & `ocrmypdf-9.8.2/docs/images/macos-workflow.png`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/index.rst` & `ocrmypdf-9.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/installation.rst` & `ocrmypdf-9.8.2/docs/installation.rst`

 * *Files 3% similar despite different names*

```diff
@@ -571,14 +571,61 @@
 
 Docker
 ^^^^^^
 
 You can also :ref:`Install the Docker <docker-install>` container on Windows. Ensure that
 your command prompt can run the docker "hello world" container.
 
+Installing on Cygwin64 under Windows
+====================================
+
+First install the the following prerequisite Cygwin packages using ``setup-x86_64.exe``::
+
+    python36 (or later)
+    python3?-devel
+    python3?-pip
+    python3?-lxml
+    python3?-imaging
+
+       (where 3? means match the version of python3 you installed)
+
+    gcc-g++
+    ghostscript (<=9.50 or >=9.52-2 see note below)
+    libexempi3
+    libexempi-devel
+    libffi6
+    libffi-devel
+    pngquant
+    qpdf
+    libqpdf-devel
+    tesseract-ocr
+    tesseract-ocr-devel
+
+.. note::
+
+    The Cygwin package for Ghostscript in versions 9.52 and
+    9.52-1 contained a bug that caused an exception to occur when
+    ocrmypdf invoked gs.  Make sure you have either 9.50 (or earlier)
+    or 9.52-2 (or later).
+
+Then open a Cygwin terminal (i.e. ``mintty``), run the following commands. Note
+that if you are using the version of ``pip`` that was installed with the Cygwin
+Python package, the command name will be ``pip3``.  If you have since updated
+``pip`` (with, for instance ``pip3 install --upgrade pip``) the the command is
+likely just ``pip`` instead of ``pip3``:
+
+.. code-block:: bash
+
+    pip3 install wheel
+    pip3 install ocrmypdf
+
+The optional dependency "unpaper" that is currently not available under Cygwin.
+Without it, certain options such as ``--clean`` will produce an error message.
+However, the OCR-to-text-layer functionality is available.
+
 Installing with Python pip
 ==========================
 
 OCRmyPDF is delivered by PyPI because it is a convenient way to install
 the latest version. However, PyPI and ``pip`` cannot address the fact
 that ``ocrmypdf`` depends on certain non-Python system libraries and
 programs being instsalled.
```

### Comparing `ocrmypdf-9.8.1/docs/introduction.rst` & `ocrmypdf-9.8.2/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/jbig2.rst` & `ocrmypdf-9.8.2/docs/jbig2.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/languages.rst` & `ocrmypdf-9.8.2/docs/languages.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/optimizer.rst` & `ocrmypdf-9.8.2/docs/optimizer.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/performance.rst` & `ocrmypdf-9.8.2/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/pipeline.svg` & `ocrmypdf-9.8.2/docs/pipeline.svg`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/plugins.rst` & `ocrmypdf-9.8.2/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/docs/release_notes.rst` & `ocrmypdf-9.8.2/docs/release_notes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 useful in scripts that launch OCRmyPDF processes or that wish to use
 some of its features for working with PDFs.
 
 Note that it is licensed under GPLv3, so scripts that
 ``import ocrmypdf`` and are released publicly should probably also be
 licensed under GPLv3.
 
+v9.8.2
+======
+
+-  Fixed an issue where OCRmyPDF would ignore text inside Form XObject when
+   making certain decisions about whether a document already had text.
+-  Fixed file size increase warning to take overhead of small files into account.
+-  Added instructions for installing on Cygwin.
+
 v9.8.1
 ======
 
 -  Fixed an issue where unexpected files in the ``%PROGRAMFILES%\gs`` directory
    (Windows) caused an exception.
 -  Mark pdfminer.six 20200517 as supported.
 -  If jbig2enc is missing and optimization is requested, a warning is issued
```

### Comparing `ocrmypdf-9.8.1/docs/security.rst` & `ocrmypdf-9.8.2/docs/security.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/misc/batch.py` & `ocrmypdf-9.8.2/misc/batch.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/misc/completion/ocrmypdf.bash` & `ocrmypdf-9.8.2/misc/completion/ocrmypdf.bash`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/misc/completion/ocrmypdf.fish` & `ocrmypdf-9.8.2/misc/completion/ocrmypdf.fish`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/misc/synology.py` & `ocrmypdf-9.8.2/misc/synology.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/misc/watcher.py` & `ocrmypdf-9.8.2/misc/watcher.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/misc/webservice.py` & `ocrmypdf-9.8.2/misc/webservice.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/setup.cfg` & `ocrmypdf-9.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/setup.py` & `ocrmypdf-9.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/__init__.py` & `ocrmypdf-9.8.2/src/ocrmypdf/__init__.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/__main__.py` & `ocrmypdf-9.8.2/src/ocrmypdf/__main__.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/_graft.py` & `ocrmypdf-9.8.2/src/ocrmypdf/_graft.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/_jobcontext.py` & `ocrmypdf-9.8.2/src/ocrmypdf/_jobcontext.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/_pipeline.py` & `ocrmypdf-9.8.2/src/ocrmypdf/_pipeline.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/_sync.py` & `ocrmypdf-9.8.2/src/ocrmypdf/_sync.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/_unicodefun.py` & `ocrmypdf-9.8.2/src/ocrmypdf/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/_validation.py` & `ocrmypdf-9.8.2/src/ocrmypdf/_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import locale
 import logging
 import os
 import sys
 from pathlib import Path
 from shutil import copyfileobj
 
+import pikepdf
 import PIL
 
 from ._unicodefun import verify_python3_env
 from .exceptions import (
     BadArgsError,
     InputFileError,
     MissingDependencyError,
@@ -406,16 +407,23 @@
 
 def report_output_file_size(options, input_file, output_file):
     try:
         output_size = Path(output_file).stat().st_size
         input_size = Path(input_file).stat().st_size
     except FileNotFoundError:
         return  # Outputting to stream or something
+    with pikepdf.open(output_file) as p:
+        # Overhead constants obtained by estimating amount of data added by OCR
+        # PDF/A conversion, and possible XMP metadata addition, with compression
+        FILE_OVERHEAD = 4000
+        OCR_PER_PAGE_OVERHEAD = 3000
+        reasonable_overhead = FILE_OVERHEAD + OCR_PER_PAGE_OVERHEAD * len(p.pages)
     ratio = output_size / input_size
-    if ratio < 1.35 or input_size < 25000:
+    reasonable_ratio = output_size / (input_size + reasonable_overhead)
+    if reasonable_ratio < 1.35 or input_size < 25000:
         return  # Seems fine
 
     reasons = []
     image_preproc = {
         'deskew',
         'clean_final',
         'remove_background',
```

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/_version.py` & `ocrmypdf-9.8.2/src/ocrmypdf/_version.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/api.py` & `ocrmypdf-9.8.2/src/ocrmypdf/api.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/cli.py` & `ocrmypdf-9.8.2/src/ocrmypdf/cli.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/data/sRGB.icc` & `ocrmypdf-9.8.2/src/ocrmypdf/data/sRGB.icc`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/exceptions.py` & `ocrmypdf-9.8.2/src/ocrmypdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/exec/__init__.py` & `ocrmypdf-9.8.2/src/ocrmypdf/exec/__init__.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/exec/ghostscript.py` & `ocrmypdf-9.8.2/src/ocrmypdf/exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/exec/jbig2enc.py` & `ocrmypdf-9.8.2/src/ocrmypdf/exec/jbig2enc.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/exec/pngquant.py` & `ocrmypdf-9.8.2/src/ocrmypdf/exec/pngquant.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/exec/qpdf.py` & `ocrmypdf-9.8.2/src/ocrmypdf/exec/qpdf.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/exec/tesseract.py` & `ocrmypdf-9.8.2/src/ocrmypdf/exec/tesseract.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/exec/unpaper.py` & `ocrmypdf-9.8.2/src/ocrmypdf/exec/unpaper.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/helpers.py` & `ocrmypdf-9.8.2/src/ocrmypdf/helpers.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/hocrtransform.py` & `ocrmypdf-9.8.2/src/ocrmypdf/hocrtransform.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/leptonica.py` & `ocrmypdf-9.8.2/src/ocrmypdf/leptonica.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/lib/__init__.py` & `ocrmypdf-9.8.2/src/ocrmypdf/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/lib/_leptonica.py` & `ocrmypdf-9.8.2/src/ocrmypdf/lib/_leptonica.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/lib/compile_leptonica.py` & `ocrmypdf-9.8.2/src/ocrmypdf/lib/compile_leptonica.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/optimize.py` & `ocrmypdf-9.8.2/src/ocrmypdf/optimize.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/pdfa.py` & `ocrmypdf-9.8.2/src/ocrmypdf/pdfa.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/pdfinfo/__init__.py` & `ocrmypdf-9.8.2/src/ocrmypdf/pdfinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/pdfinfo/ghosttext.py` & `ocrmypdf-9.8.2/src/ocrmypdf/pdfinfo/ghosttext.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/pdfinfo/info.py` & `ocrmypdf-9.8.2/src/ocrmypdf/pdfinfo/info.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/pdfinfo/layout.py` & `ocrmypdf-9.8.2/src/ocrmypdf/pdfinfo/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,17 @@
 
     def get_result(self):
         return self.result
 
 
 def get_page_analysis(infile, pageno, pscript5_mode):
     rman = pdfminer.pdfinterp.PDFResourceManager(caching=True)
-    dev = TextPositionTracker(rman, laparams=LAParams())
+    dev = TextPositionTracker(
+        rman, laparams=LAParams(all_texts=True, detect_vertical=True)
+    )
     interp = pdfminer.pdfinterp.PDFPageInterpreter(rman, dev)
 
     if pscript5_mode:
         patcher = patch.multiple(
             'pdfminer.pdffont.PDFType3Font',
             spec=True,
             get_ascent=PDFType3Font__PScript5_get_ascent,
```

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf/quality.py` & `ocrmypdf-9.8.2/src/ocrmypdf/quality.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf.egg-info/PKG-INFO` & `ocrmypdf-9.8.2/src/ocrmypdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocrmypdf
-Version: 9.8.1
+Version: 9.8.2
 Summary: OCRmyPDF adds an OCR text layer to scanned PDF files, allowing them to be searched
 Home-page: https://github.com/jbarlow83/OCRmyPDF
 Author: James R. Barlow
 Author-email: james@purplerock.ca
 License: UNKNOWN
 Project-URL: Documentation, https://ocrmypdf.readthedocs.io/
 Project-URL: Source, https://github.com/jbarlow83/ocrmypdf
```

### Comparing `ocrmypdf-9.8.1/src/ocrmypdf.egg-info/SOURCES.txt` & `ocrmypdf-9.8.2/src/ocrmypdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/2400dpi/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/3small/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/aspect/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_hocr__hocr__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/cardinal/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/ccitt/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cmyk/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/cmyk/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/cmyk/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/francais/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/francais/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/graph_ocred/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/graph_ocred/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/graph_ocred/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/graph_ocred/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/jbig2/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__deu__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/lichtenstein/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/manifest.jsonl` & `ocrmypdf-9.8.2/tests/cache/manifest.jsonl`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000002_ocr.png__000002_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000003_ocr.png__000003_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000004_ocr.png__000004_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_hocr__hocr__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000005_ocr.png__000005_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_hocr__hocr__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/multipage/__-l__eng__000006_ocr.png__000006_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/palette/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/poster/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__--psm__7__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin` & `ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/hocr.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_hocr__hocr__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin` & `ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/pdf.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin` & `ocrmypdf-9.8.2/tests/cache/skew/__-l__eng__000001_ocr.png__000001_ocr_tess__pdf__txt/txt.bin`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/conftest.py` & `ocrmypdf-9.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/2400dpi.pdf` & `ocrmypdf-9.8.2/tests/resources/2400dpi.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/3small.pdf` & `ocrmypdf-9.8.2/tests/resources/3small.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/README.rst` & `ocrmypdf-9.8.2/tests/resources/README.rst`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/acroform.pdf` & `ocrmypdf-9.8.2/tests/resources/acroform.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/aspect.pdf` & `ocrmypdf-9.8.2/tests/resources/aspect.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/baiona.png` & `ocrmypdf-9.8.2/tests/resources/baiona.png`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/baiona_alpha.png` & `ocrmypdf-9.8.2/tests/resources/baiona_alpha.png`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/baiona_cmyk.jpg` & `ocrmypdf-9.8.2/tests/resources/baiona_cmyk.jpg`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/baiona_colormapped.png` & `ocrmypdf-9.8.2/tests/resources/baiona_colormapped.png`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/baiona_gray.png` & `ocrmypdf-9.8.2/tests/resources/baiona_gray.png`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/blank.pdf` & `ocrmypdf-9.8.2/tests/resources/blank.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/c02-22.pdf` & `ocrmypdf-9.8.2/tests/resources/c02-22.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/cardinal.pdf` & `ocrmypdf-9.8.2/tests/resources/cardinal.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/ccitt.pdf` & `ocrmypdf-9.8.2/tests/resources/ccitt.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/cmyk.pdf` & `ocrmypdf-9.8.2/tests/resources/cmyk.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/congress.jpg` & `ocrmypdf-9.8.2/tests/resources/congress.jpg`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/crom.png` & `ocrmypdf-9.8.2/tests/resources/crom.png`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/encrypted_algo4.pdf` & `ocrmypdf-9.8.2/tests/resources/encrypted_algo4.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/enormous.pdf` & `ocrmypdf-9.8.2/tests/resources/enormous.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/epson.pdf` & `ocrmypdf-9.8.2/tests/resources/epson.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/formxobject.pdf` & `ocrmypdf-9.8.2/tests/resources/formxobject.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/francais.pdf` & `ocrmypdf-9.8.2/tests/resources/francais.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/graph.pdf` & `ocrmypdf-9.8.2/tests/resources/graph.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/graph_ocred.pdf` & `ocrmypdf-9.8.2/tests/resources/graph_ocred.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/hugemono.pdf` & `ocrmypdf-9.8.2/tests/resources/hugemono.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/jbig2.pdf` & `ocrmypdf-9.8.2/tests/resources/jbig2.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/kcs.pdf` & `ocrmypdf-9.8.2/tests/resources/kcs.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/lichtenstein.pdf` & `ocrmypdf-9.8.2/tests/resources/lichtenstein.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/link.pdf` & `ocrmypdf-9.8.2/tests/resources/link.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/linn.pdf` & `ocrmypdf-9.8.2/tests/resources/linn.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/linn.png` & `ocrmypdf-9.8.2/tests/resources/linn.png`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/linn.txt` & `ocrmypdf-9.8.2/tests/resources/linn.txt`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/livecycle.pdf` & `ocrmypdf-9.8.2/tests/resources/livecycle.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/masks.pdf` & `ocrmypdf-9.8.2/tests/resources/masks.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/missing_docinfo.pdf` & `ocrmypdf-9.8.2/tests/resources/missing_docinfo.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/multipage.pdf` & `ocrmypdf-9.8.2/tests/resources/multipage.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/negzero.pdf` & `ocrmypdf-9.8.2/tests/resources/negzero.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/overlay.pdf` & `ocrmypdf-9.8.2/tests/resources/overlay.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/palette.pdf` & `ocrmypdf-9.8.2/tests/resources/palette.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/poster.pdf` & `ocrmypdf-9.8.2/tests/resources/poster.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/rotated_skew.pdf` & `ocrmypdf-9.8.2/tests/resources/rotated_skew.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/skew-encrypted.pdf` & `ocrmypdf-9.8.2/tests/resources/skew-encrypted.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/skew.pdf` & `ocrmypdf-9.8.2/tests/resources/skew.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/toc.pdf` & `ocrmypdf-9.8.2/tests/resources/toc.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/trivial.pdf` & `ocrmypdf-9.8.2/tests/resources/trivial.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/truetype_font_nomapping.pdf` & `ocrmypdf-9.8.2/tests/resources/truetype_font_nomapping.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/type3_font_nomapping.pdf` & `ocrmypdf-9.8.2/tests/resources/type3_font_nomapping.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/typewriter.png` & `ocrmypdf-9.8.2/tests/resources/typewriter.png`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/resources/vector.pdf` & `ocrmypdf-9.8.2/tests/resources/vector.pdf`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/spoof/gs.py` & `ocrmypdf-9.8.2/tests/spoof/gs.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/spoof/gs_feature_elision.py` & `ocrmypdf-9.8.2/tests/spoof/gs_feature_elision.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/spoof/gs_pdfa_failure.py` & `ocrmypdf-9.8.2/tests/spoof/gs_pdfa_failure.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/spoof/gs_raster_failure.py` & `ocrmypdf-9.8.2/tests/spoof/gs_raster_failure.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/spoof/gs_render_failure.py` & `ocrmypdf-9.8.2/tests/spoof/gs_render_failure.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/spoof/tesseract_big_image_error.py` & `ocrmypdf-9.8.2/tests/spoof/tesseract_big_image_error.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/spoof/tesseract_cache.py` & `ocrmypdf-9.8.2/tests/spoof/tesseract_cache.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/spoof/tesseract_crash.py` & `ocrmypdf-9.8.2/tests/spoof/tesseract_crash.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/spoof/tesseract_noop.py` & `ocrmypdf-9.8.2/tests/spoof/tesseract_noop.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/spoof/unpaper_oldversion.py` & `ocrmypdf-9.8.2/tests/spoof/unpaper_oldversion.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_acroform.py` & `ocrmypdf-9.8.2/tests/test_acroform.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_api.py` & `ocrmypdf-9.8.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_completion.py` & `ocrmypdf-9.8.2/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_ghostscript.py` & `ocrmypdf-9.8.2/tests/test_ghostscript.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_graft.py` & `ocrmypdf-9.8.2/tests/test_graft.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_helpers.py` & `ocrmypdf-9.8.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_hocrtransform.py` & `ocrmypdf-9.8.2/tests/test_hocrtransform.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_image_input.py` & `ocrmypdf-9.8.2/tests/test_image_input.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_lept.py` & `ocrmypdf-9.8.2/tests/test_lept.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_main.py` & `ocrmypdf-9.8.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_metadata.py` & `ocrmypdf-9.8.2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_optimize.py` & `ocrmypdf-9.8.2/tests/test_optimize.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_page_numbers.py` & `ocrmypdf-9.8.2/tests/test_page_numbers.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_pdfinfo.py` & `ocrmypdf-9.8.2/tests/test_pdfinfo.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_preprocessing.py` & `ocrmypdf-9.8.2/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_qpdf.py` & `ocrmypdf-9.8.2/tests/test_qpdf.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_quality.py` & `ocrmypdf-9.8.2/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_rotation.py` & `ocrmypdf-9.8.2/tests/test_rotation.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_stdio.py` & `ocrmypdf-9.8.2/tests/test_stdio.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_tess4.py` & `ocrmypdf-9.8.2/tests/test_tess4.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_unpaper.py` & `ocrmypdf-9.8.2/tests/test_unpaper.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_userunit.py` & `ocrmypdf-9.8.2/tests/test_userunit.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf-9.8.1/tests/test_validation.py` & `ocrmypdf-9.8.2/tests/test_validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with OCRmyPDF.  If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 import os
 from unittest.mock import patch
 
+import pikepdf
 import pytest
 
 import ocrmypdf._validation as vd
 from ocrmypdf.api import create_options
 from ocrmypdf.exceptions import BadArgsError, MissingDependencyError
 from ocrmypdf.pdfinfo import PdfInfo
 
@@ -107,23 +108,28 @@
         with pytest.raises(BadArgsError):
             vd.check_requested_output_file(make_opts(output_file='-'))
 
 
 def test_report_file_size(tmp_path, caplog):
     in_ = tmp_path / 'a.pdf'
     out = tmp_path / 'b.pdf'
-    in_.write_bytes(b'123')
-    out.write_bytes(b'')
+    pdf = pikepdf.new()
+    pdf.save(in_)
+    pdf.save(out)
     opts = make_opts()
     vd.report_output_file_size(opts, in_, out)
     assert caplog.text == ''
     caplog.clear()
 
-    os.truncate(in_, 25001)
-    os.truncate(out, 50000)
+    waste_of_space = b'Dummy' * 5000
+    pdf.root.Dummy = waste_of_space
+    pdf.save(in_)
+    pdf.root.Dummy2 = waste_of_space + waste_of_space
+    pdf.save(out)
+
     with patch('ocrmypdf._validation.jbig2enc.available', return_value=True), patch(
         'ocrmypdf._validation.pngquant.available', return_value=True
     ):
         vd.report_output_file_size(opts, in_, out)
         assert 'No reason' in caplog.text
     caplog.clear()
```

