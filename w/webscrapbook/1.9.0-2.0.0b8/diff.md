# Comparing `tmp/webscrapbook-1.9.0.tar.gz` & `tmp/webscrapbook-2.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscrapbook-1.9.0.tar", last modified: Sun Mar 26 13:48:00 2023, max compression
+gzip compressed data, was "webscrapbook-2.0.0b8.tar", last modified: Sun May 14 14:29:18 2023, max compression
```

## Comparing `webscrapbook-1.9.0.tar` & `webscrapbook-2.0.0b8.tar`

### file list

```diff
@@ -1,124 +1,110 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.088171 webscrapbook-1.9.0/
--rw-rw-rw-   0        0        0     1092 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/LICENSE.txt
--rw-rw-rw-   0        0        0     5422 2023-03-26 13:48:00.088171 webscrapbook-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     4173 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/README.md
--rw-rw-rw-   0        0        0      494 2023-03-26 13:48:00.088171 webscrapbook-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0     2543 2023-03-26 06:42:51.000000 webscrapbook-1.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.010047 webscrapbook-1.9.0/tests/
--rw-rw-rw-   0        0        0   265526 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/tests/test_app_actions.py
--rw-rw-rw-   0        0        0    21865 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/tests/test_app_config.py
--rw-rw-rw-   0        0        0    46945 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_app_helpers.py
--rw-rw-rw-   0        0        0    24358 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/tests/test_cli.py
--rw-rw-rw-   0        0        0    11308 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_init.py
--rw-rw-rw-   0        0        0     7653 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_locales.py
--rw-rw-rw-   0        0        0    45991 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_book.py
--rw-rw-rw-   0        0        0   136912 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_cache.py
--rw-rw-rw-   0        0        0    35991 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_check.py
--rw-rw-rw-   0        0        0    31914 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_convert_file2wsb.py
--rw-rw-rw-   0        0        0    58056 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_convert_items.py
--rw-rw-rw-   0        0        0    58963 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_convert_migrate.py
--rw-rw-rw-   0        0        0    26916 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_convert_sb2wsb.py
--rw-rw-rw-   0        0        0    23247 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_convert_wsb2file.py
--rw-rw-rw-   0        0        0    51845 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/tests/test_scrapbook_convert_wsb2sb.py
--rw-rw-rw-   0        0        0    24094 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_exporter.py
--rw-rw-rw-   0        0        0    24746 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_host.py
--rw-rw-rw-   0        0        0    58506 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_importer.py
--rw-rw-rw-   0        0        0    86635 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_indexer.py
--rw-rw-rw-   0        0        0    13455 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_server.py
--rw-rw-rw-   0        0        0    83786 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_util.py
--rw-rw-rw-   0        0        0    19327 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_util_html.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.025675 webscrapbook-1.9.0/webscrapbook/
--rw-rw-rw-   0        0        0     9042 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/webscrapbook/__init__.py
--rw-rw-rw-   0        0        0      165 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/__main__.py
--rw-rw-rw-   0        0        0    68272 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/webscrapbook/app.py
--rw-rw-rw-   0        0        0    42102 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/webscrapbook/cli.py
--rw-rw-rw-   0        0        0     3217 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/locales.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.041299 webscrapbook-1.9.0/webscrapbook/resources/
--rw-rw-rw-   0        0        0      144 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/resources/app.py
--rw-rw-rw-   0        0        0      948 2023-03-26 12:46:27.000000 webscrapbook-1.9.0/webscrapbook/resources/config.ini
--rw-rw-rw-   0        0        0    12038 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/webscrapbook/resources/config.md
--rw-rw-rw-   0        0        0     1505 2021-12-07 15:19:04.000000 webscrapbook-1.9.0/webscrapbook/resources/mimetypes.md
--rw-rw-rw-   0        0        0      128 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/resources/serve.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.041299 webscrapbook-1.9.0/webscrapbook/scrapbook/
--rw-rw-rw-   0        0        0        0 2021-12-07 15:19:04.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/__init__.py
--rw-rw-rw-   0        0        0    12822 2023-03-26 13:19:57.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/book.py
--rw-rw-rw-   0        0        0    38152 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/cache.py
--rw-rw-rw-   0        0        0    27605 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/check.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.041299 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/
--rw-rw-rw-   0        0        0        0 2021-12-07 15:19:04.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/__init__.py
--rw-rw-rw-   0        0        0    12576 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/file2wsb.py
--rw-rw-rw-   0        0        0    13623 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/items.py
--rw-rw-rw-   0        0        0    41527 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/migrate.py
--rw-rw-rw-   0        0        0    15877 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/sb2wsb.py
--rw-rw-rw-   0        0        0     5902 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/wsb2file.py
--rw-rw-rw-   0        0        0    25939 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/wsb2sb.py
--rw-rw-rw-   0        0        0     6619 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/exporter.py
--rw-rw-rw-   0        0        0    15228 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/host.py
--rw-rw-rw-   0        0        0    15255 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/importer.py
--rw-rw-rw-   0        0        0    39353 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/indexer.py
--rw-rw-rw-   0        0        0     2356 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/server.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:47:59.956670 webscrapbook-1.9.0/webscrapbook/themes/
-drwxrwxrwx   0        0        0        0 2023-03-26 13:47:59.956670 webscrapbook-1.9.0/webscrapbook/themes/default/
-drwxrwxrwx   0        0        0        0 2023-03-26 13:47:59.956670 webscrapbook-1.9.0/webscrapbook/themes/default/locales/
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.041299 webscrapbook-1.9.0/webscrapbook/themes/default/locales/ar/
--rw-rw-rw-   0        0        0       36 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/ar/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.056923 webscrapbook-1.9.0/webscrapbook/themes/default/locales/en/
--rw-rw-rw-   0        0        0     7705 2023-03-26 13:24:56.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/en/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.056923 webscrapbook-1.9.0/webscrapbook/themes/default/locales/es/
--rw-rw-rw-   0        0        0     8763 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/es/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.056923 webscrapbook-1.9.0/webscrapbook/themes/default/locales/fa/
--rw-rw-rw-   0        0        0       36 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/fa/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.056923 webscrapbook-1.9.0/webscrapbook/themes/default/locales/he/
--rw-rw-rw-   0        0        0       36 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/he/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.056923 webscrapbook-1.9.0/webscrapbook/themes/default/locales/zh/
--rw-rw-rw-   0        0        0     7843 2023-03-26 13:24:56.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/zh/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.056923 webscrapbook-1.9.0/webscrapbook/themes/default/locales/zh_cn/
--rw-rw-rw-   0        0        0     7860 2023-03-26 13:24:56.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/zh_cn/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.072546 webscrapbook-1.9.0/webscrapbook/themes/default/static/
--rw-rw-rw-   0        0        0      281 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/collapse.png
--rw-rw-rw-   0        0        0      728 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/comment.png
--rw-rw-rw-   0        0        0      877 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/common.css
--rw-rw-rw-   0        0        0     4140 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/common.js
--rw-rw-rw-   0        0        0     1055 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/edit.css
--rw-rw-rw-   0        0        0     1563 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/edit.js
--rw-rw-rw-   0        0        0     2438 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/editx.js
--rw-rw-rw-   0        0        0      279 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/expand.png
--rw-rw-rw-   0        0        0      523 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/external.png
--rw-rw-rw-   0        0        0      752 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/fclose.png
--rw-rw-rw-   0        0        0      449 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/file.png
--rw-rw-rw-   0        0        0      790 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/fopen.png
--rw-rw-rw-   0        0        0     3810 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/index-ex.css
--rw-rw-rw-   0        0        0    60629 2023-03-26 13:24:56.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/index-ex.js
--rw-rw-rw-   0        0        0     2210 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/index.css
--rw-rw-rw-   0        0        0     2156 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/index.js
--rw-rw-rw-   0        0        0      502 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/item.png
--rw-rw-rw-   0        0        0      387 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/link.png
--rw-rw-rw-   0        0        0      445 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/note.png
--rw-rw-rw-   0        0        0      515 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/postit.png
--rw-rw-rw-   0        0        0      661 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/search.png
--rw-rw-rw-   0        0        0      807 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/toggle.png
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.088171 webscrapbook-1.9.0/webscrapbook/themes/default/templates/
--rw-rw-rw-   0        0        0      482 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/base.html
--rw-rw-rw-   0        0        0      632 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/cli.html
--rw-rw-rw-   0        0        0     1053 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/edit.html
--rw-rw-rw-   0        0        0      965 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/editx.html
--rw-rw-rw-   0        0        0     5632 2023-03-26 13:24:56.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/index.html
--rw-rw-rw-   0        0        0      510 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/maff_index.html
--rw-rw-rw-   0        0        0      490 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/markdown.html
--rw-rw-rw-   0        0        0      568 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_frame.html
--rw-rw-rw-   0        0        0     1751 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_index.html
--rw-rw-rw-   0        0        0    12917 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_map.html
--rw-rw-rw-   0        0        0    26419 2023-03-08 13:49:02.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_search.html
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.088171 webscrapbook-1.9.0/webscrapbook/util/
--rw-rw-rw-   0        0        0      120 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/webscrapbook/util/__init__.py
--rw-rw-rw-   0        0        0     5867 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/util/css.py
--rw-rw-rw-   0        0        0    15308 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/util/html.py
--rw-rw-rw-   0        0        0    52535 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/util/util.py
--rw-rw-rw-   0        0        0      568 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/webscrapbook/util/zipstream.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.025675 webscrapbook-1.9.0/webscrapbook.egg-info/
--rw-rw-rw-   0        0        0     5422 2023-03-26 13:47:59.000000 webscrapbook-1.9.0/webscrapbook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3840 2023-03-26 13:47:59.000000 webscrapbook-1.9.0/webscrapbook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 13:47:59.000000 webscrapbook-1.9.0/webscrapbook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-03-26 13:47:59.000000 webscrapbook-1.9.0/webscrapbook.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      255 2023-03-26 13:47:59.000000 webscrapbook-1.9.0/webscrapbook.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-26 13:47:59.000000 webscrapbook-1.9.0/webscrapbook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:18.080429 webscrapbook-2.0.0b8/
+-rw-rw-rw-   0        0        0     1092 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/LICENSE.txt
+-rw-rw-rw-   0        0        0       13 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5611 2023-05-14 14:29:18.080429 webscrapbook-2.0.0b8/PKG-INFO
+-rw-rw-rw-   0        0        0     4300 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/README.md
+-rw-rw-rw-   0        0        0     2507 2023-05-14 14:29:18.084429 webscrapbook-2.0.0b8/setup.cfg
+-rw-rw-rw-   0        0        0       63 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.947815 webscrapbook-2.0.0b8/webscrapbook/
+-rw-rw-rw-   0        0        0     7184 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/__init__.py
+-rw-rw-rw-   0        0        0      165 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.955816 webscrapbook-2.0.0b8/webscrapbook/_polyfill/
+-rw-rw-rw-   0        0        0        0 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/_polyfill/__init__.py
+-rw-rw-rw-   0        0        0     1445 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/_polyfill/argparse.py
+-rw-rw-rw-   0        0        0     2084 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/_polyfill/mimetypes.py
+-rw-rw-rw-   0        0        0      393 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/_polyfill/zipfile.py
+-rw-rw-rw-   0        0        0    55732 2023-05-14 13:47:20.000000 webscrapbook-2.0.0b8/webscrapbook/app.py
+-rw-rw-rw-   0        0        0    46417 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/cli.py
+-rw-rw-rw-   0        0        0     3131 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/locales.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.963214 webscrapbook-2.0.0b8/webscrapbook/resources/
+-rw-rw-rw-   0        0        0      144 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/resources/app.py
+-rw-rw-rw-   0        0        0     1040 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/resources/config.ini
+-rw-rw-rw-   0        0        0    13234 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/resources/config.md
+-rw-rw-rw-   0        0        0     1505 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/resources/mimetypes.md
+-rw-rw-rw-   0        0        0      128 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/resources/serve.py
+-rw-rw-rw-   0        0        0     1542 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/resources/themes.md
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.971217 webscrapbook-2.0.0b8/webscrapbook/scrapbook/
+-rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/__init__.py
+-rw-rw-rw-   0        0        0    51823 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/book.py
+-rw-rw-rw-   0        0        0    38510 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/cache.py
+-rw-rw-rw-   0        0        0    27924 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/check.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.979487 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/
+-rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/__init__.py
+-rw-rw-rw-   0        0        0    11866 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/file2wsb.py
+-rw-rw-rw-   0        0        0    13580 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/items.py
+-rw-rw-rw-   0        0        0    41549 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/migrate.py
+-rw-rw-rw-   0        0        0    15455 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/sb2wsb.py
+-rw-rw-rw-   0        0        0     5934 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/wsb2file.py
+-rw-rw-rw-   0        0        0    26003 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/wsb2sb.py
+-rw-rw-rw-   0        0        0     8784 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/exporter.py
+-rw-rw-rw-   0        0        0    15902 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/host.py
+-rw-rw-rw-   0        0        0    18101 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/importer.py
+-rw-rw-rw-   0        0        0    38988 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/indexer.py
+-rw-rw-rw-   0        0        0    19924 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/search.py
+-rw-rw-rw-   0        0        0     7705 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/scrapbook/util.py
+-rw-rw-rw-   0        0        0     2356 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/server.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.929467 webscrapbook-2.0.0b8/webscrapbook/themes/
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.933469 webscrapbook-2.0.0b8/webscrapbook/themes/default/
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.933469 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.980188 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/ar/
+-rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/ar/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.980188 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/en/
+-rw-rw-rw-   0        0        0     7783 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/en/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.980188 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/es/
+-rw-rw-rw-   0        0        0     8853 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/es/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.980188 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/fa/
+-rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/fa/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.980188 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/he/
+-rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/he/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.984191 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/zh/
+-rw-rw-rw-   0        0        0     7912 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/zh/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.984191 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/zh_cn/
+-rw-rw-rw-   0        0        0     7929 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/zh_cn/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:18.039025 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/
+-rw-rw-rw-   0        0        0      281 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/collapse.png
+-rw-rw-rw-   0        0        0      728 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/comment.png
+-rw-rw-rw-   0        0        0      877 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/common.css
+-rw-rw-rw-   0        0        0     3900 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/common.js
+-rw-rw-rw-   0        0        0     1055 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/edit.css
+-rw-rw-rw-   0        0        0     1563 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/edit.js
+-rw-rw-rw-   0        0        0     2438 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/editx.js
+-rw-rw-rw-   0        0        0      279 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/expand.png
+-rw-rw-rw-   0        0        0      523 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/external.png
+-rw-rw-rw-   0        0        0      752 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/fclose.png
+-rw-rw-rw-   0        0        0      449 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/file.png
+-rw-rw-rw-   0        0        0      790 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/fopen.png
+-rw-rw-rw-   0        0        0     3810 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index-ex.css
+-rw-rw-rw-   0        0        0    61757 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index-ex.js
+-rw-rw-rw-   0        0        0     2210 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index.css
+-rw-rw-rw-   0        0        0     2156 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index.js
+-rw-rw-rw-   0        0        0      502 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/item.png
+-rw-rw-rw-   0        0        0      387 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/link.png
+-rw-rw-rw-   0        0        0      445 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/note.png
+-rw-rw-rw-   0        0        0      515 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/postit.png
+-rw-rw-rw-   0        0        0      661 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/search.png
+-rw-rw-rw-   0        0        0      807 2023-04-08 19:20:00.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/static/toggle.png
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:18.076428 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/
+-rw-rw-rw-   0        0        0      482 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/base.html
+-rw-rw-rw-   0        0        0      632 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/cli.html
+-rw-rw-rw-   0        0        0     1053 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/edit.html
+-rw-rw-rw-   0        0        0      965 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/editx.html
+-rw-rw-rw-   0        0        0     5632 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/index.html
+-rw-rw-rw-   0        0        0      510 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/maff_index.html
+-rw-rw-rw-   0        0        0      490 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/markdown.html
+-rw-rw-rw-   0        0        0      568 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_frame.html
+-rw-rw-rw-   0        0        0     1751 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_index.html
+-rw-rw-rw-   0        0        0    12917 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_map.html
+-rw-rw-rw-   0        0        0    26766 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_search.html
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:18.080429 webscrapbook-2.0.0b8/webscrapbook/util/
+-rw-rw-rw-   0        0        0       72 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/util/__init__.py
+-rw-rw-rw-   0        0        0     5867 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/util/css.py
+-rw-rw-rw-   0        0        0    44456 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/util/fs.py
+-rw-rw-rw-   0        0        0    15308 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/util/html.py
+-rw-rw-rw-   0        0        0    36829 2023-05-14 13:37:39.000000 webscrapbook-2.0.0b8/webscrapbook/util/util.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:29:17.951818 webscrapbook-2.0.0b8/webscrapbook.egg-info/
+-rw-rw-rw-   0        0        0     5611 2023-05-14 14:29:17.000000 webscrapbook-2.0.0b8/webscrapbook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3428 2023-05-14 14:29:17.000000 webscrapbook-2.0.0b8/webscrapbook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:29:17.000000 webscrapbook-2.0.0b8/webscrapbook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-05-14 14:29:17.000000 webscrapbook-2.0.0b8/webscrapbook.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      264 2023-05-14 14:29:17.000000 webscrapbook-2.0.0b8/webscrapbook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-14 14:29:17.000000 webscrapbook-2.0.0b8/webscrapbook.egg-info/top_level.txt
```

### Comparing `webscrapbook-1.9.0/LICENSE.txt` & `webscrapbook-2.0.0b8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/PKG-INFO` & `webscrapbook-2.0.0b8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: webscrapbook
-Version: 1.9.0
+Version: 2.0.0b8
 Summary: A backend toolkit for management of WebScrapBook collection.
 Home-page: https://github.com/danny0838/PyWebScrapBook
 Author: Danny Lin
 Author-email: danny0838@gmail.com
-License: MIT
+License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
@@ -72,18 +73,21 @@
         check (k)  check and fix scrapbook data
         export (x)
                    export data items into archive files (*.wsba)
         import (i)
                    import data items from archive files (*.wsba)
         convert (v)
                    convert scrapbook data between different formats
+        query (q)  perform queries on the scrapbook(s)
+        search (r)
+                   search for data items in the scrapbook(s)
         help       show detailed information about certain topics
         view       view archive file in the browser
 
-    optional arguments:
+    options:
       -h, --help   show this help message and exit
       --version    show version information and exit
       --root ROOT  root directory to manipulate (default: current working directory)
 
 Run `wsb <command> --help` for help about `<command>`. For example, `wsb config --help` for help about `wsb config`.
 
 ### Host a scrapbook
```

### Comparing `webscrapbook-1.9.0/README.md` & `webscrapbook-2.0.0b8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,18 +43,21 @@
         check (k)  check and fix scrapbook data
         export (x)
                    export data items into archive files (*.wsba)
         import (i)
                    import data items from archive files (*.wsba)
         convert (v)
                    convert scrapbook data between different formats
+        query (q)  perform queries on the scrapbook(s)
+        search (r)
+                   search for data items in the scrapbook(s)
         help       show detailed information about certain topics
         view       view archive file in the browser
 
-    optional arguments:
+    options:
       -h, --help   show this help message and exit
       --version    show version information and exit
       --root ROOT  root directory to manipulate (default: current working directory)
 
 Run `wsb <command> --help` for help about `<command>`. For example, `wsb config --help` for help about `wsb config`.
 
 ### Host a scrapbook
```

### Comparing `webscrapbook-1.9.0/webscrapbook/app.py` & `webscrapbook-2.0.0b8/webscrapbook/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """The WGSI application.
 """
 import functools
-import io
 import json
-import mimetypes
 import os
-import re
-import shutil
 import time
 import traceback
-import zipfile
-from contextlib import contextmanager, nullcontext
+import types
+from collections import namedtuple
+from contextlib import nullcontext
 from secrets import token_urlsafe
 from urllib.parse import quote, unquote, urljoin, urlsplit, urlunsplit
 from zlib import adler32
 
 import commonmark
 import flask
 import jinja2
@@ -35,17 +32,26 @@
     parse_options_header,
 )
 from werkzeug.local import LocalProxy
 from werkzeug.middleware.proxy_fix import ProxyFix
 from werkzeug.utils import cached_property
 
 from . import WSB_CONFIG, WSB_DIR, WSB_EXTENSION_MIN_VERSION, __version__, util
+from ._polyfill import mimetypes, zipfile
 from .scrapbook import cache as wsb_cache
 from .scrapbook import check as wsb_check
 from .scrapbook import host as wsb_host
+from .scrapbook import search as wsb_search
+from .scrapbook import util as wsb_util
+from .util.fs import (
+    ZIP_SUBPATH_DIR,
+    ZIP_SUBPATH_DIR_IMPLICIT,
+    ZIP_SUBPATH_DIR_ROOT,
+    ZIP_SUBPATH_FILE,
+)
 
 # see: https://url.spec.whatwg.org/#percent-encoded-bytes
 quote_path = functools.partial(quote, safe=":/[]@!$&'()*+,;=")
 quote_path.__doc__ = 'Escape reserved chars for the path part of a URL.'
 
 bp = flask.Blueprint('default', __name__)
 host = LocalProxy(lambda: current_app.config['WEBSCRAPBOOK_HOST'])
@@ -90,15 +96,15 @@
         except KeyError:
             abort(404)
     else:
         info = subpath
 
     fh = zh.open(info, 'r')
 
-    lm = util.zip_timestamp(info)
+    lm = util.fs.zip_timestamp(info)
     last_modified = http_date(lm)
 
     etag = '%s-%s-%s' % (
         lm,
         info.file_size,
         adler32(info.filename.encode('utf-8')) & 0xFFFFFFFF,
     )
@@ -118,260 +124,85 @@
 
 def stream_template(template_name, **context):
     current_app.update_template_context(context)
     t = current_app.jinja_env.get_template(template_name)
     return t.stream(context)
 
 
-def http_response(body='', status=None, headers=None, format=None):
+def generate_server_sent_events(gen):
+    try:
+        for data in gen:
+            yield 'data: ' + data + '\n\n'
+    except Exception:
+        traceback.print_exc()
+        err = {'type': 'critical', 'msg': 'Internal Server Error'}
+        yield 'data: ' + json.dumps(err, ensure_ascii=False) + '\n\n'
+
+    yield 'event: complete' + '\n'
+    yield 'data: ' + '\n\n'
+
+
+def http_response(body=None, status=None, headers=None, format=None):
     """Handle formatted response.
 
     ref: https://jsonapi.org
     """
     if not format:
         mimetype = None
+        if body is None:
+            body = ''
 
-    # expect body to be a JSON-serializable object
+    # expect body to be a JSON-serializable object (including str)
     elif format == 'json':
         mimetype = 'application/json'
 
-        body = {
-            'success': True,
-            'data': body,
-        }
+        if status == 204:
+            status = None
+            body = None
 
-        body = json.dumps(body, ensure_ascii=False)
+        body = json.dumps({
+            'data': body,
+        }, ensure_ascii=False)
 
     # expect body to be a generator of text (mostly JSON) data
     elif format == 'sse':
         mimetype = 'text/event-stream'
 
-        def wrapper(gen):
-            try:
-                for data in gen:
-                    yield 'data: ' + data + '\n\n'
-            except Exception:
-                traceback.print_exc()
-                err = {'error': {'message': 'Internal Server Error'}}
-                yield 'data: ' + json.dumps(err, ensure_ascii=False) + '\n\n'
+        if status == 204:
+            status = None
+            body = None
 
-            yield 'event: complete' + '\n'
-            yield 'data: ' + '\n\n'
+        if body is None:
+            body = generate_server_sent_events(iter(()))
+        else:
+            if not isinstance(body, types.GeneratorType):
+                abort(500, 'Invalid generator for an event stream')
 
-        body = wrapper(body)
+            body = generate_server_sent_events(body)
 
     else:
-        abort(400, f'Output format "{format}" is not supported.')
+        abort(400, f'Output format {format!r} is not supported.')
 
     return Response(body, status, headers, mimetype=mimetype)
 
 
 def get_localpath(path):
     """Convert a request path to local filesystem path.
     """
     # Don't use os.path.join as it doesn't concatenate if path looks like
     # absolute (e.g. "/path/to/foo" on POSIX or "X:/foo" on Windows), which
     # can cause a security issue.
     return os.path.normpath(host.chroot + os.sep + path)
 
 
-def _get_archive_path_tidy(path, striproot=False):
-    has_initial_slash = path.startswith('/')
-    comps = path.split('/')
-    new_comps = []
-    for comp in comps:
-        if comp in ('', '.'):
-            continue
-        if comp == '..':
-            if new_comps:
-                new_comps.pop()
-            continue
-        new_comps.append(comp)
-    return ('/' if has_initial_slash and not striproot else '') + '/'.join(new_comps)
-
-
-def _get_archive_path_add_subpath(paths, zh, subpath):
-    for m in reversed(list(re.finditer(r'!/', subpath, flags=re.I))):
-        archivepath = _get_archive_path_tidy(subpath[:m.start(0)], True)
-        conflicting = archivepath + '!/'
-
-        if any(i.startswith(conflicting) for i in zh.namelist()):
-            break
-
-        try:
-            fh = zh.open(archivepath, 'r')
-        except KeyError:
-            continue
-
-        with fh as fh:
-            try:
-                zh1 = zipfile.ZipFile(fh, 'r')
-            except zipfile.BadZipFile:
-                continue
-
-            with zh1 as zh1:
-                paths.append(archivepath)
-                _get_archive_path_add_subpath(paths, zh1, subpath[m.end(0):])
-                return
-
-    paths.append(_get_archive_path_tidy(subpath, True))
-
-
-def get_archive_path(filepath):
-    """Parse archive file path and the sub-archive path.
-
-    - Priority:
-      entry.zip!/entry1.zip!/ = entry.zip!/entry1.zip! >
-      entry.zip!/entry1.zip >
-      entry.zip!/ = entry.zip! >
-      entry.zip
-
-    Returns:
-        a list [path-to-directory-or-file]
-        or [path-to-zip-file, subpath1, subpath2, ...]
-    """
-    paths = []
-    for m in reversed(list(re.finditer(r'!/', filepath, flags=re.I))):
-        archivepath = _get_archive_path_tidy(filepath[:m.start(0)])
-        archivefile = get_localpath(archivepath)
-        conflicting = archivefile + '!'
-        if os.path.lexists(conflicting):
-            break
-
-        # if parent directory does not exist, FileNotFoundError is raised on
-        # Windows, while NotADirectoryError is raised on Linux
-        try:
-            zh = zipfile.ZipFile(archivefile, 'r')
-        except (zipfile.BadZipFile, FileNotFoundError, NotADirectoryError):
-            continue
-
-        with zh as zh:
-            paths.append(archivepath)
-            _get_archive_path_add_subpath(paths, zh, filepath[m.end(0):])
-            return paths
-
-    paths.append(_get_archive_path_tidy(filepath))
-    return paths
-
-
-def _open_archive_path_filter(path, filters):
-    for filter in filters:
-        filter = filter.rstrip('/')
-        if path == filter:
-            return True
-        if path.startswith(filter + ('/' if filter else '')):
-            return True
-    return False
-
-
-@contextmanager
-def open_archive_path(localpaths, mode='r', filters=None):
-    """Open the innermost zip handler for reading or writing.
-
-    e.g. reading from localpaths=['/path/to/foo.zip', 'subdir/file.txt']:
-
-        with open_archive_path(localpaths) as zh:
-            with zh.open(localpaths[-1]) as fh:
-                print(fh.read())
-
-    e.g. writing to localpaths=['/path/to/foo.zip', 'subdir/file.txt']:
-
-        with open_archive_path(localpaths, 'w') as zh:
-            zh.writestr(localpaths[-1], 'foo')
-
-    e.g. deleting localpaths=['/path/to/foo.zip', 'subdir/']:
-
-        with open_archive_path(localpaths, 'w', [localpaths[-1]]) as zh:
-            pass
-
-    Args:
-        localpaths: [path-to-zip-file, subpath1, subpath2, ...]
-        mode: 'r' for reading, 'w' for modifying
-        filters: a list of file or folder to remove
-    """
-    last = len(localpaths) - 1
-    if last < 1:
-        raise ValueError('length of paths must > 1')
-
-    filtered = False
-    stack = []
-    try:
-        zh = zipfile.ZipFile(localpaths[0])
-        stack.append(zh)
-        for i in range(1, last):
-            fh = zh.open(localpaths[i])
-            stack.append(fh)
-            zh = zipfile.ZipFile(fh)
-            stack.append(zh)
-
-        if mode == 'r':
-            yield zh
-
-        elif mode == 'w':
-            # create a buffer for writing
-            buffer = io.BytesIO()
-            with zipfile.ZipFile(buffer, 'w') as zh:
-                yield zh
-
-            # copy zip file
-            for i in reversed(range(1, last + 1)):
-                zh0 = stack.pop()
-                with zipfile.ZipFile(buffer, 'a') as zh:
-                    zh.comment = zh0.comment
-                    for info in zh0.infolist():
-                        if filters and i == last:
-                            if _open_archive_path_filter(info.filename, filters):
-                                filtered = True
-                                continue
-
-                        try:
-                            zh.getinfo(info.filename)
-                        except KeyError:
-                            pass
-                        else:
-                            continue
-
-                        zh.writestr(info, zh0.read(info),
-                                    compress_type=info.compress_type,
-                                    compresslevel=None if info.compress_type == zipfile.ZIP_STORED else 9,
-                                    )
-
-                if filters and not any(f == '' for f in filters) and not filtered:
-                    raise KeyError('paths to filter do not exist')
-
-                if i == 1:
-                    break
-
-                # writer to another buffer for the parent zip
-                buffer2 = io.BytesIO()
-                with zipfile.ZipFile(buffer2, 'w') as zh:
-                    zh.writestr(localpaths[i - 1], buffer.getvalue(), compress_type=zipfile.ZIP_STORED)
-                buffer.close()
-                buffer = buffer2
-
-                # pop a file handler
-                stack.pop()
-
-            # write to the outermost zip
-            # use 'r+b' as 'wb' causes PermissionError for hidden file in Windows
-            buffer.seek(0)
-            with open(localpaths[0], 'r+b') as fw, buffer as fr:
-                fw.truncate()
-                for chunk in iter(functools.partial(fr.read, 8192), b''):
-                    fw.write(chunk)
-    finally:
-        for fh in reversed(stack):
-            fh.close()
-
-
-def get_breadcrumbs(paths, base='', topname='.'):
+def get_breadcrumbs(localpaths, base='', topname='.'):
     """Generate (label, subpath, sep, is_last) tuples.
     """
     base = base.rstrip('/') + '/'
-    paths = paths.copy()
+    paths = list(localpaths)
     paths[0] = paths[0].strip('/')
 
     if not paths[0]:
         yield (topname, base, '/', True)
         return
 
     yield (topname, base, '/', False)
@@ -434,28 +265,28 @@
     if perm == 'all':
         return True
 
     if perm == 'read':
         return action not in {
             'token', 'lock', 'unlock',
             'mkdir', 'mkzip', 'save', 'delete', 'move', 'copy',
-            'backup', 'unbackup', 'cache', 'check',
+            'backup', 'unbackup', 'cache', 'check', 'query',
         }
 
     if perm == 'view':
-        return action in {'view', 'info', 'source', 'download', 'static'}
+        return action in {'view', 'info', 'source', 'download', 'static', 'unknown'}
 
     return False
 
 
 def handle_directory_listing(localpaths, zh=None, redirect_slash=True, format=None):
     """List contents in a directory.
 
     Args:
-        localpaths: [path-to-zip-file, subpath1, subpath2, ...]
+        localpaths: a CPath
         zh: an opened zipfile.ZipFile object for faster reading
     """
     # ensure directory has trailing '/'
     if redirect_slash and not request.path.endswith('/'):
         parts = urlsplit(request.url)
         new_url = urlunsplit((
             parts.scheme,
@@ -482,50 +313,37 @@
 
         headers = {
             'Cache-Control': 'no-cache',
             'Last-Modified': last_modified,
             'ETag': etag,
         }
 
-        with nullcontext(zh) if zh else open_archive_path(localpaths) as zh:
-            subentries = util.zip_listdir(zh, localpaths[-1])
+        with nullcontext(zh) if zh else util.fs.open_archive_path(localpaths) as zh:
+            subentries = zip_listdir(zh, localpaths[-1])
 
     else:
         # disallow cache to reflect any content file change
         stats = os.stat(localpaths[0])
         headers = {
             'Cache-Control': 'no-store',
             'Last-Modified': http_date(stats.st_mtime),
         }
 
-        subentries = util.listdir(localpaths[0])
+        subentries = listdir(localpaths[0])
 
     if format == 'sse':
         def gen():
             for entry in subentries:
-                data = {
-                    'name': entry.name,
-                    'type': entry.type,
-                    'size': entry.size,
-                    'last_modified': entry.last_modified,
-                }
-
+                data = entry._asdict()
                 yield json.dumps(data, ensure_ascii=False)
 
         return http_response(gen(), headers=headers, format=format)
 
     if format == 'json':
-        data = []
-        for entry in subentries:
-            data.append({
-                'name': entry.name,
-                'type': entry.type,
-                'size': entry.size,
-                'last_modified': entry.last_modified,
-            })
+        data = [e._asdict() for e in subentries]
         return http_response(data, headers=headers, format=format)
 
     body = render_template('index.html',
                            sitename=host.name,
                            is_local=is_local_access(),
                            base=request.script_root,
                            path=request.path,
@@ -535,15 +353,15 @@
     return http_response(body, headers=headers)
 
 
 def handle_archive_viewing(localpaths, mimetype):
     """Handle direct visit of HTZ/MAFF file.
 
     Args:
-        localpaths: [path-to-zip-file, subpath1, subpath2, ...]
+        localpaths: a CPath
     """
     def list_maff_pages(pages):
         """List available web pages in a MAFF file.
         """
         return render_template('maff_index.html',
                                sitename=host.name,
                                is_local=is_local_access(),
@@ -552,15 +370,15 @@
                                pages=pages,
                                )
 
     if mimetype == 'application/html+zip':
         subpath = 'index.html'
     else:
         if len(localpaths) > 1:
-            with open_archive_path(localpaths) as zh:
+            with util.fs.open_archive_path(localpaths) as zh:
                 with zh.open(localpaths[-1]) as zh1:
                     pages = util.get_maff_pages(zh1)
         else:
             pages = util.get_maff_pages(localpaths[-1])
 
         if len(pages) > 1:
             # multiple index files
@@ -583,30 +401,30 @@
     return redirect(new_url)
 
 
 def handle_markdown_output(localpaths, zh=None):
     """Output processed markdown.
 
     Args:
-        localpaths: [path-to-zip-file, subpath1, subpath2, ...]
+        localpaths: a CPath
         zh: an opened zipfile.ZipFile object for faster reading
     """
     if len(localpaths) > 1:
         if zh:
             context = nullcontext(zh)
         else:
-            context = open_archive_path(localpaths)
+            context = util.fs.open_archive_path(localpaths)
     else:
         context = nullcontext(None)
 
     with context as zh:
         # calculate last-modified time and etag
         if zh:
             info = zh.getinfo(localpaths[-1])
-            lm = util.zip_timestamp(info)
+            lm = util.fs.zip_timestamp(info)
             last_modified = http_date(lm)
 
             etag = '%s-%s-%s' % (
                 lm,
                 info.file_size,
                 adler32(info.filename.encode('utf-8')) & 0xFFFFFFFF,
             )
@@ -652,27 +470,28 @@
 
 class Request(flask.Request):
     """Subclassed Request object for more useful properties.
     """
     @cached_property
     def paths(self):
         """Like request.path, but with ZIP subpaths resolved."""
-        return get_archive_path(self.path)
+        return util.fs.CPath.resolve(self.path, get_localpath)
 
     @cached_property
     def localpath(self):
         """Corresponding filesystem path of the requested path."""
         return get_localpath(self.path)
 
     @cached_property
     def localpaths(self):
         """Like localpath, but with ZIP subpaths resolved."""
-        paths = self.paths.copy()
-        paths[0] = get_localpath(paths[0])
-        return paths
+        return util.fs.CPath(
+            get_localpath(self.paths[0]),
+            *self.paths[1:],
+        )
 
     @cached_property
     def localrealpath(self):
         """Like localpath, but with symlinks resolved."""
         return os.path.realpath(self.localpath)
 
     @cached_property
@@ -682,14 +501,16 @@
         return mimetype
 
     @cached_property
     def action(self):
         """Shortcut of the requested action."""
         rv = request.values.get('a', default='view')
         rv = request.values.get('action', default=rv)
+        if not globals().get(f'action_{rv}'):
+            rv = 'unknown'
         return rv
 
     @cached_property
     def format(self):
         """Shortcut of the requested format."""
         rv = request.values.get('f')
         rv = request.values.get('format', default=rv)
@@ -712,33 +533,33 @@
 
     return wrapper
 
 
 def handle_action_advanced(func):
     """A decorator function that helps handling an advanced command.
 
-    - Verify POST method.
-    - Provide a default return value.
+    - Verify POST method (except for SSE format).
+    - Add 'Cache-Control: no-store' header.
+    - Provide a default 204 response.
     """
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         format = request.format
 
-        if request.method != 'POST':
+        if request.method != 'POST' and format != 'sse':
             abort(405, valid_methods=['POST'])
 
-        rv = func(*args, **kwargs)
+        response = func(*args, **kwargs)
 
-        if rv is not None:
-            return rv
+        if response is None:
+            response = http_response(status=204, format=format)
 
-        if format:
-            return http_response('Command run successfully.', format=format)
+        response.headers.set('Cache-Control', 'no-store')
 
-        return http_response(status=204)
+        return response
 
     return wrapper
 
 
 def handle_action_writing(func):
     """A decorator function that helps handling a writing action.
     """
@@ -748,67 +569,14 @@
             abort(403, 'Unable to operate the root directory.')
 
         return func(*args, **kwargs)
 
     return wrapper
 
 
-def handle_action_renaming(func):
-    """A decorator function that helps handling a move/copy action.
-    """
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        localpaths = request.localpaths
-
-        if len(localpaths) > 1:
-            with open_archive_path(localpaths) as zh:
-                if not util.zip_has(zh, localpaths[-1]):
-                    abort(404, 'Source does not exist.')
-        else:
-            if not os.path.lexists(localpaths[0]):
-                abort(404, 'Source does not exist.')
-
-        target = request.values.get('target')
-
-        if target is None:
-            abort(400, 'Target is not specified.')
-
-        targetpaths = get_archive_path(target)
-        targetpaths[0] = get_localpath(targetpaths[0])
-
-        if len(targetpaths) > 1:
-            with open_archive_path(targetpaths) as zh:
-                # target is a file
-                if util.zip_has(zh, targetpaths[-1], type='file'):
-                    abort(400, 'Found something at target.')
-
-                # target is a directory, treat as to target/<basename>
-                if util.zip_has(zh, targetpaths[-1], type='dir'):
-                    targetpaths[-1] = targetpaths[-1] + ('/' if targetpaths[-1] else '') + os.path.basename(localpaths[-1])
-
-                    # recheck if target exists
-                    if util.zip_has(zh, targetpaths[-1], type='any'):
-                        abort(400, 'Found identical entry under the target directory.')
-        else:
-            if os.path.lexists(targetpaths[0]):
-                if os.path.isdir(targetpaths[0]):
-                    # target is an existing directory, treat as to target/<basename>
-                    targetpaths[0] = os.path.join(targetpaths[0], os.path.basename(localpaths[-1]))
-
-                    # recheck if target exists
-                    if os.path.lexists(targetpaths[0]):
-                        abort(400, 'Found identical entry under the target directory.')
-                else:
-                    abort(400, 'Found something at target.')
-
-        return func(*args, sourcepaths=localpaths, targetpaths=targetpaths, **kwargs)
-
-    return wrapper
-
-
 def action_unknown():
     """Default handler for an undefined action"""
     abort(400, 'Action not supported.')
 
 
 def action_view():
     """Show the content of a file or list a directory.
@@ -819,22 +587,22 @@
     if request.format:
         return action_info()
 
     localpaths = request.localpaths
     mimetype = request.localmimetype
 
     if len(localpaths) > 1:
-        with open_archive_path(localpaths) as zh:
+        with util.fs.open_archive_path(localpaths) as zh:
             # List directory only when URL suffixed with "/", as it's not a
             # common operation, and it's costy to check for directory existence
             # in a ZIP.
             if request.path.endswith('/'):
                 try:
                     return handle_directory_listing(localpaths, zh, redirect_slash=False)
-                except util.ZipDirNotFoundError:
+                except ZipDirNotFoundError:
                     abort(404)
 
             try:
                 info = zh.getinfo(localpaths[-1])
             except KeyError:
                 # File does not exist.
                 abort(404)
@@ -922,15 +690,15 @@
     """Show file content as plain text."""
     if request.format:
         abort(400, 'Action not supported.')
 
     localpaths = request.localpaths
 
     if len(localpaths) > 1:
-        with open_archive_path(localpaths) as zh:
+        with util.fs.open_archive_path(localpaths) as zh:
             response = zip_static_file(zh, localpaths[-1])
     else:
         response = static_file(localpaths[0])
 
     # show as inline plain text
     # @TODO: Chromium (80) seems to ignore header mimetype for certain types
     #        like image and zip
@@ -947,114 +715,39 @@
     if request.format:
         abort(400, 'Action not supported.')
 
     localpaths = request.localpaths
     filter = request.values.getlist('i')
 
     if len(localpaths) > 1:
-        streaming = False
-        with open_archive_path(localpaths) as zh:
-            try:
-                zh.getinfo(localpaths[-1])
-            except KeyError:
-                base = localpaths[-1] + '/' if localpaths[-1] else ''
-                infos = [i for i in zh.infolist() if i.filename.startswith(base)]
-
-                # not exist
-                if base and not len(infos):
-                    abort(404)
-
-                # directory (explicit or implicit): stream as ZIP
-                streaming = True
-                filename = (localpaths[-1] or os.path.basename(localpaths[-2])) + '.zip'
+        with util.fs.open_archive_path(localpaths) as zh:
+            cur = util.fs.zip_check_subpath(zh, localpaths[-1], allow_invalid=True)
+            if cur in (ZIP_SUBPATH_DIR, ZIP_SUBPATH_DIR_IMPLICIT, ZIP_SUBPATH_DIR_ROOT):
+                filename = (os.path.basename(localpaths[-1]) or os.path.basename(localpaths[-2])) + '.zip'
                 mimetype, _ = mimetypes.guess_type(filename)
-                cut = len(base)
-
-                # prepare paths to output
-                filter = set(filter)
-                filter_d = {f + '/' for f in filter}
-                paths = []
-                for info in infos:
-                    arcname = info.filename
-                    subpath = info.filename[cut:]
-
-                    # exclude the directory itself
-                    if not arcname:
-                        continue
-
-                    # apply the filter
-                    if filter:
-                        if subpath not in filter:
-                            if not any(subpath.startswith(f) for f in filter_d):
-                                continue
-
-                    paths.append((arcname, subpath))
-            else:
+                response = None
+            elif cur == ZIP_SUBPATH_FILE:
                 filename = os.path.basename(request.localrealpath)
                 response = zip_static_file(zh, localpaths[-1], mimetype=request.localmimetype)
+            else:
+                abort(404)
 
-        if streaming:
+        if not response:
             def gen():
-                zs = util.ZipStream()
-                with open_archive_path(localpaths) as zh,\
-                     zipfile.ZipFile(zs, 'w') as zf:
-                    for arcname, subpath in paths:
-                        info = zh.getinfo(arcname)
-                        with zh.open(info) as ih:
-                            info.filename = subpath
-                            with zf.open(info, 'w') as oh:
-                                for chunk in iter(lambda: ih.read(8192), b''):
-                                    oh.write(chunk)
-                                    yield zs.get()
-                yield zs.get()
+                with util.fs.open_archive_path(localpaths) as zh:
+                    yield from util.fs.zip_copy(zh, localpaths[-1], None, '', filter)
 
             response = Response(gen(), mimetype=mimetype)
             response.headers.set('Cache-Control', 'no-store')
     else:
         if os.path.isdir(localpaths[0]):
             filename = os.path.basename(request.localrealpath) + '.zip'
             mimetype, _ = mimetypes.guess_type(filename)
-
-            # prepare paths to output
-            filter = {os.path.normcase(os.path.join(localpaths[0], f)) for f in filter}
-            filter_d = {os.path.join(f, '') for f in filter}
-            cut = len(os.path.join(localpaths[0], ''))
-            paths = []
-            for root, dirs, files in os.walk(localpaths[0]):
-                for file in dirs + files:
-                    file = os.path.join(root, file)
-
-                    # apply the filter
-                    if filter:
-                        file_nc = os.path.normcase(file)
-                        if file_nc not in filter:
-                            if not any(file_nc.startswith(f) for f in filter_d):
-                                continue
-
-                    subpath = file[cut:]
-                    if os.path.isdir(file):
-                        subpath += '/'
-                    paths.append((file, subpath))
-
-            def gen():
-                zs = util.ZipStream()
-                with zipfile.ZipFile(zs, 'w') as zf:
-                    for file, subpath in paths:
-                        zinfo = zipfile.ZipInfo.from_file(file, subpath)
-                        if zinfo.is_dir():
-                            zf.writestr(zinfo, b'')
-                            yield zs.get()
-                        else:
-                            with open(file, 'rb') as ih, zf.open(zinfo, 'w') as oh:
-                                for chunk in iter(lambda: ih.read(8192), b''):
-                                    oh.write(chunk)
-                                    yield zs.get()
-                yield zs.get()
-
-            response = Response(gen(), mimetype=mimetype)
+            gen = util.fs.zip_compress(None, localpaths[0], '', filter)
+            response = Response(gen, mimetype=mimetype)
             response.headers.set('Cache-Control', 'no-store')
         else:
             filename = os.path.basename(request.localrealpath)
             response = static_file(localpaths[0])
 
     filename = quote_path(filename)
     response.headers.set('Content-Disposition',
@@ -1062,33 +755,28 @@
     return response
 
 
 def action_info():
     """Show information of a path."""
     format = request.format
 
-    if not format:
+    if format != 'json':
         abort(400, 'Action not supported.')
 
     localpaths = request.localpaths
     mimetype = request.localmimetype
 
     if len(localpaths) > 1:
-        with open_archive_path(localpaths) as zh:
-            info = util.zip_file_info(zh, localpaths[-1], check_implicit_dir=True)
+        with util.fs.open_archive_path(localpaths) as zh:
+            info = zip_file_info(zh, localpaths[-1], check_implicit_dir=True)
     else:
-        info = util.file_info(localpaths[0])
+        info = file_info(localpaths[0])
 
-    data = {
-        'name': info.name,
-        'type': info.type,
-        'size': info.size,
-        'last_modified': info.last_modified,
-        'mime': mimetype,
-    }
+    data = info._asdict()
+    data['mime'] = mimetype
     return http_response(data, format=format)
 
 
 def action_list():
     """List entries in a directory."""
     format = request.format
 
@@ -1096,15 +784,15 @@
         abort(400, 'Action not supported.')
 
     localpaths = request.localpaths
 
     if len(localpaths) > 1:
         try:
             return handle_directory_listing(localpaths, redirect_slash=False, format=format)
-        except util.ZipDirNotFoundError:
+        except ZipDirNotFoundError:
             abort(404, 'Directory does not exist.')
 
     if os.path.isdir(localpaths[0]):
         return handle_directory_listing(localpaths, redirect_slash=False, format=format)
 
     abort(404, 'Directory does not exist.')
 
@@ -1134,15 +822,15 @@
     localpaths = request.localpaths
     localpath = localpaths[0]
 
     if os.path.lexists(localpath) and not os.path.isfile(localpath):
         abort(400, 'Found a non-file here.')
 
     if len(localpaths) > 1:
-        with open_archive_path(localpaths) as zh:
+        with util.fs.open_archive_path(localpaths) as zh:
             try:
                 info = zh.getinfo(localpaths[-1])
             except KeyError:
                 body = b''
             else:
                 body = zh.read(info)
     else:
@@ -1186,15 +874,15 @@
     if os.path.lexists(localpath) and not os.path.isfile(localpath):
         abort(400, 'Found a non-file here.')
 
     if request.localmimetype not in ('text/html', 'application/xhtml+xml'):
         abort(400, 'This is not an HTML file.')
 
     if len(localpaths) > 1:
-        with open_archive_path(localpaths) as zh:
+        with util.fs.open_archive_path(localpaths) as zh:
             try:
                 zh.getinfo(localpaths[-1])
             except KeyError:
                 abort(404)
     else:
         if not os.path.lexists(localpath):
             abort(404)
@@ -1217,47 +905,41 @@
         abort(400, 'Command can only run on local device.')
 
     localpath = request.localpath
 
     if not os.path.lexists(localpath):
         abort(404, 'File does not exist.')
 
-    util.launch(localpath)
-
-    if format:
-        return http_response('Command run successfully.', format=format)
+    util.fs.launch(localpath)
 
-    return http_response(status=204)
+    return http_response(status=204, format=format)
 
 
 def action_browse():
     """Open a file or directory in the file browser."""
     format = request.format
 
     if not is_local_access():
         abort(400, 'Command can only run on local device.')
 
     localpath = request.localpath
 
     if not os.path.lexists(localpath):
         abort(404, 'File does not exist.')
 
-    util.view_in_explorer(localpath)
-
-    if format:
-        return http_response('Command run successfully.', format=format)
+    util.fs.view_in_explorer(localpath)
 
-    return http_response(status=204)
+    return http_response(status=204, format=format)
 
 
 def action_config():
     """Show server config."""
     format = request.format
 
-    if not format:
+    if format != 'json':
         abort(400, 'Action not supported.')
 
     data = host.config.dump_object()
 
     # filter values for better security
     data = {k: v for k, v in data.items() if k in ('app', 'book')}
     data['app'] = {k: v for k, v in data['app'].items() if k in ('name', 'theme', 'locale')}
@@ -1281,14 +963,17 @@
     """Acquire a token and return its name."""
     format = request.format
 
     # require POST method
     if request.method != 'POST':
         abort(405, valid_methods=['POST'])
 
+    if format not in (None, 'json'):
+        abort(400, 'Action not supported.')
+
     return http_response(host.token_acquire(), format=format)
 
 
 @handle_action_advanced
 @handle_action_token
 def action_lock():
     """Acquire a lock for the given name.
@@ -1305,35 +990,35 @@
     id = request.values.get('id')
 
     timeout = request.values.get('chkt', 5, type=float)
 
     try:
         lock = host.get_lock(name, persist=id)
     except wsb_host.LockPersistError:
-        abort(400, f'Unable to persist lock "{name}".')
+        abort(400, f'Unable to persist lock {name!r}.')
 
     if id:
         try:
             lock.extend()
         except wsb_host.LockExtendNotFoundError:
             # Lock file gone in this short interval. Try acquire.
             pass
         except wsb_host.LockExtendError:
-            abort(500, f'Unable to extend lock "{name}".')
+            abort(500, f'Unable to extend lock {name!r}.')
         else:
             return http_response(lock.id, format=request.format)
 
     try:
         lock.acquire(timeout=timeout)
     except wsb_host.LockTimeoutError:
-        abort(503, f'Unable to acquire lock "{name}".', retry_after=60)
+        abort(503, f'Unable to acquire lock {name!r}.', retry_after=60)
     except wsb_host.LockRegenerateError:
-        abort(500, f'Unable to regenerate stale lock "{name}".')
+        abort(500, f'Unable to regenerate stale lock {name!r}.')
     except wsb_host.LockGenerateError:
-        abort(500, f'Unable to create lock "{name}".')
+        abort(500, f'Unable to create lock {name!r}.')
 
     return http_response(lock.id, format=request.format)
 
 
 @handle_action_advanced
 @handle_action_token
 def action_unlock():
@@ -1347,525 +1032,350 @@
     id = request.values.get('id')
     if id is None:
         abort(400, 'Lock ID is not specified.')
 
     try:
         lock = host.get_lock(name, persist=id)
     except wsb_host.LockPersistError:
-        abort(400, f'Unable to persist lock "{name}".')
+        abort(400, f'Unable to persist lock {name!r}.')
 
     try:
         lock.release()
     except wsb_host.LockReleaseNotFoundError:
         pass
     except wsb_host.LockReleaseError:
-        abort(500, f'Unable to remove lock "{name}".')
+        abort(500, f'Unable to remove lock {name!r}.')
 
 
 @handle_action_advanced
 @handle_action_token
 @handle_action_writing
 def action_mkdir():
     """Create a directory."""
     localpaths = request.localpaths
 
-    if len(localpaths) > 1:
-        try:
-            zh = None
-            with open_archive_path(localpaths) as zh0:
-                if util.zip_has(zh0, localpaths[-1], type='file'):
-                    abort(400, 'Found a non-directory here.')
-
-                # skip if the folder already exists
-                if util.zip_has(zh0, localpaths[-1], type='dir'):
-                    return
-
-                # append for a non-nested zip
-                if len(localpaths) == 2:
-                    zh = zipfile.ZipFile(localpaths[0], 'a')
-
-            if zh is None:
-                zh = open_archive_path(localpaths, 'w')
-
-            with zh as zh:
-                info = zipfile.ZipInfo(localpaths[-1] + '/', time.localtime())
-                zh.writestr(info, b'', compress_type=zipfile.ZIP_STORED)
-        except HTTPException:
-            raise
-        except Exception:
-            traceback.print_exc()
-            abort(500, 'Unable to create a directory here.')
-
-    else:
-        localpath = localpaths[0]
-
-        if os.path.lexists(localpath) and not os.path.isdir(localpath):
-            abort(400, 'Found a non-directory here.')
-
-        try:
-            os.makedirs(localpath, exist_ok=True)
-        except OSError:
-            traceback.print_exc()
-            abort(500, 'Unable to create a directory here.')
+    try:
+        util.fs.mkdir(localpaths)
+    except util.fs.FSEntryExistsError:
+        abort(400, 'Found something here.')
+    except util.fs.FSBadParentError:
+        abort(400, 'Parent directory is not available.')
+    except Exception:
+        traceback.print_exc()
+        abort(500, 'Unable to create a directory here.')
 
 
 @handle_action_advanced
 @handle_action_token
 @handle_action_writing
 def action_mkzip():
     """Create a zip file."""
     localpaths = request.localpaths
 
-    if len(localpaths) > 1:
-        try:
-            zh = None
-            with open_archive_path(localpaths) as zh0:
-                if util.zip_has(zh0, localpaths[-1], type='dir'):
-                    abort(400, 'Found a non-file here.')
-
-                # append for a nonexistent path in a non-nested zip
-                if len(localpaths) == 2:
-                    if not util.zip_has(zh0, localpaths[-1], type='file'):
-                        zh = zipfile.ZipFile(localpaths[0], 'a')
-
-            if zh is None:
-                zh = open_archive_path(localpaths, 'w')
-
-            with zh as zh:
-                info = zipfile.ZipInfo(localpaths[-1], time.localtime())
-                buf = io.BytesIO()
-                with zipfile.ZipFile(buf, 'w'):
-                    pass
-                zh.writestr(info, buf.getvalue(), compress_type=zipfile.ZIP_STORED)
-        except HTTPException:
-            raise
-        except Exception:
-            traceback.print_exc()
-            abort(500, 'Unable to write to this ZIP file.')
-
-    else:
-        localpath = localpaths[0]
-
-        if os.path.lexists(localpath) and not os.path.isfile(localpath):
-            abort(400, 'Found a non-file here.')
-
-        try:
-            os.makedirs(os.path.dirname(localpath), exist_ok=True)
-        except Exception:
-            traceback.print_exc()
-            abort(500, 'Unable to write to this path.')
-
-        try:
-            with zipfile.ZipFile(localpath, 'w'):
-                pass
-        except Exception:
-            traceback.print_exc()
-            abort(500, 'Unable to write to this file.')
+    try:
+        util.fs.mkzip(localpaths)
+    except util.fs.FSIsADirectoryError:
+        abort(400, 'Found a non-file here.')
+    except util.fs.FSEntryExistsError:
+        abort(400, 'Found something here.')
+    except util.fs.FSBadParentError:
+        abort(400, 'Parent directory is not available.')
+    except Exception:
+        traceback.print_exc()
+        abort(500, 'Unable to write to this ZIP file.')
 
 
 @handle_action_advanced
 @handle_action_token
 @handle_action_writing
 def action_save():
     """Write a file with provided text or uploaded stream."""
     localpaths = request.localpaths
 
-    if len(localpaths) > 1:
-        try:
-            zh = None
-            with open_archive_path(localpaths) as zh0:
-                if util.zip_has(zh0, localpaths[-1], type='dir'):
-                    abort(400, 'Found a non-file here.')
-
-                # append for a nonexistent path in a non-nested zip
-                if len(localpaths) == 2:
-                    if not util.zip_has(zh0, localpaths[-1], type='file'):
-                        zh = zipfile.ZipFile(localpaths[0], 'a')
-
-            if zh is None:
-                zh = open_archive_path(localpaths, 'w')
-
-            with zh as zh:
-                info = zipfile.ZipInfo(localpaths[-1], time.localtime())
-                file = request.files.get('upload')
-                if file is not None:
-                    with zh.open(info, 'w', force_zip64=True) as fh:
-                        stream = file.stream
-                        for chunk in iter(functools.partial(stream.read, 8192), b''):
-                            fh.write(chunk)
-                else:
-                    bytes_ = request.values.get('text', '').encode('ISO-8859-1')
-                    zh.writestr(info, bytes_, compress_type=zipfile.ZIP_DEFLATED, compresslevel=9)
-        except HTTPException:
-            raise
-        except Exception:
-            traceback.print_exc()
-            abort(500, 'Unable to write to this ZIP file.')
-
+    file = request.files.get('upload')
+    if file is not None:
+        src = file.stream
     else:
-        localpath = localpaths[0]
-
-        if os.path.lexists(localpath) and not os.path.isfile(localpath):
-            abort(400, 'Found a non-file here.')
+        src = request.values.get('text', '').encode('ISO-8859-1')
 
-        try:
-            os.makedirs(os.path.dirname(localpath), exist_ok=True)
-        except OSError:
-            traceback.print_exc()
-            abort(500, 'Unable to write to this path.')
-
-        try:
-            file = request.files.get('upload')
-            if file is not None:
-                file.save(localpath)
-            else:
-                bytes_ = request.values.get('text', '').encode('ISO-8859-1')
-                with open(localpath, 'wb') as fh:
-                    fh.write(bytes_)
-        except Exception:
-            traceback.print_exc()
-            abort(500, 'Unable to write to this file.')
+    try:
+        util.fs.save(localpaths, src)
+    except util.fs.FSIsADirectoryError:
+        abort(400, 'Found a non-file here.')
+    except util.fs.FSEntryExistsError:
+        abort(400, 'Found something here.')
+    except util.fs.FSBadParentError:
+        abort(400, 'Parent directory is not available.')
+    except Exception:
+        traceback.print_exc()
+        abort(500, 'Unable to write to this ZIP file.')
 
 
 @handle_action_advanced
 @handle_action_token
 @handle_action_writing
 def action_delete():
     """Delete a file or directory."""
     localpaths = request.localpaths
 
-    if len(localpaths) > 1:
-        try:
-            with open_archive_path(localpaths, 'w', [localpaths[-1]]):
-                pass
-        except KeyError:
-            # fail since nothing is deleted
-            abort(404, 'Entry does not exist in this ZIP file.')
-        except Exception:
-            traceback.print_exc()
-            abort(500, 'Unable to write to this ZIP file.')
-
-    else:
-        localpath = localpaths[0]
-
-        if not os.path.lexists(localpath):
-            abort(404, 'File does not exist.')
-
-        if util.file_is_link(localpath):
-            try:
-                os.remove(localpath)
-            except OSError:
-                traceback.print_exc()
-                abort(500, 'Unable to delete this link.')
-        elif os.path.isfile(localpath):
-            try:
-                os.remove(localpath)
-            except OSError:
-                traceback.print_exc()
-                abort(500, 'Unable to delete this file.')
-        elif os.path.isdir(localpath):
-            try:
-                shutil.rmtree(localpath)
-            except OSError:
-                traceback.print_exc()
-                abort(500, 'Unable to delete this directory.')
-        else:
-            # this should not happen
-            abort(500, 'Unable to handle this path.')
+    try:
+        util.fs.delete(localpaths)
+    except util.fs.FSEntryNotFoundError:
+        abort(404, 'Entry does not exist.')
+    except Exception:
+        traceback.print_exc()
+        abort(500, 'Unable to delete this entry.')
 
 
 @handle_action_advanced
 @handle_action_token
 @handle_action_writing
-@handle_action_renaming
-def action_move(sourcepaths, targetpaths):
+def action_move():
     """Move a file or directory."""
-    try:
-        if len(sourcepaths) == 1:
-            if len(targetpaths) == 1:
-                try:
-                    os.makedirs(os.path.dirname(targetpaths[0]), exist_ok=True)
-                except OSError:
-                    traceback.print_exc()
-                    abort(500, 'Unable to move to this path.')
-
-                shutil.move(sourcepaths[0], targetpaths[0])
-
-            else:
-                # Moving a file into a zip is like moving across disk,
-                # which makes little sense. Additionally, moving a
-                # symlink/junction should rename the entry and cannot be
-                # implemented as copying-deleting. Forbid such operation to
-                # prevent a confusion.
-                abort(400, 'Unable to move across a zip.')
-
-        elif len(sourcepaths) > 1:
-            if len(targetpaths) == 1:
-                # Moving from zip to disk is like moving across disk, which
-                # makes little sense.
-                abort(400, 'Unable to move across a zip.')
-
-            else:
-                with open_archive_path(sourcepaths) as zh:
-                    try:
-                        zh.getinfo(sourcepaths[-1])
-                    except KeyError:
-                        base = sourcepaths[-1] + '/'
-                        entries = [e for e in zh.namelist() if e.startswith(base)]
-                    else:
-                        entries = [sourcepaths[-1]]
-
-                    with open_archive_path(targetpaths, 'w') as zh2:
-                        cut = len(sourcepaths[-1])
-                        for entry in entries:
-                            info = zh.getinfo(entry)
-                            info.filename = targetpaths[-1] + entry[cut:]
-                            zh2.writestr(info, zh.read(entry),
-                                         compress_type=info.compress_type,
-                                         compresslevel=None if info.compress_type == zipfile.ZIP_STORED else 9,
-                                         )
+    localpaths = request.localpaths
 
-                with open_archive_path(sourcepaths, 'w', entries):
-                    pass
+    target = request.values.get('target')
+    if target is None:
+        abort(400, 'Target is not specified.')
+    targetpaths = util.fs.CPath.resolve(target, get_localpath).path
+    targetpaths[0] = get_localpath(targetpaths[0])
 
-    except HTTPException:
-        raise
+    try:
+        util.fs.move(localpaths, targetpaths)
+    except util.fs.FSEntryExistsError:
+        abort(400, 'Target already exists.')
+    except util.fs.FSMoveInsideError:
+        abort(400, 'Unable to move into self.')
+    except util.fs.FSMoveAcrossZipError:
+        abort(400, 'Unable to move across a zip.')
+    except util.fs.FSEntryNotFoundError:
+        abort(404, 'Source does not exist.')
     except Exception:
         traceback.print_exc()
         abort(500, 'Unable to move to the target.')
 
 
 @handle_action_advanced
 @handle_action_token
 @handle_action_writing
-@handle_action_renaming
-def action_copy(sourcepaths, targetpaths):
+def action_copy():
     """Copy a file or directory."""
-    # Copying a symlink/junction means copying the real file/directory.
-    # It makes no sense if the symlink/junction is broken.
-    if not os.path.exists(sourcepaths[0]):
-        abort(404, 'Source does not exist.')
-
-    try:
-        if len(sourcepaths) == 1:
-            if len(targetpaths) == 1:
-                try:
-                    os.makedirs(os.path.dirname(targetpaths[0]), exist_ok=True)
-                except OSError:
-                    traceback.print_exc()
-                    abort(500, 'Unable to copy to this path.')
-
-                try:
-                    shutil.copytree(sourcepaths[0], targetpaths[0])
-                except NotADirectoryError:
-                    shutil.copy2(sourcepaths[0], targetpaths[0])
-                except shutil.Error:
-                    traceback.print_exc()
-                    abort(500, 'Fail to copy some files.')
-
-            else:
-                error = False
-                with open_archive_path(targetpaths, 'w') as zh:
-                    try:
-                        util.zip_compress(zh, sourcepaths[0], targetpaths[-1])
-                    except shutil.Error:
-                        traceback.print_exc()
-                        error = True
-                if error:
-                    abort(500, 'Fail to copy some files.')
-
-        elif len(sourcepaths) > 1:
-            if len(targetpaths) == 1:
-                try:
-                    os.makedirs(os.path.dirname(targetpaths[0]), exist_ok=True)
-                except OSError:
-                    traceback.print_exc()
-                    abort(500, 'Unable to copy to this path.')
-
-                with open_archive_path(sourcepaths) as zh:
-                    util.zip_extract(zh, targetpaths[0], sourcepaths[-1])
+    localpaths = request.localpaths
 
-            else:
-                with open_archive_path(sourcepaths) as zh:
-                    try:
-                        zh.getinfo(sourcepaths[-1])
-                    except KeyError:
-                        entries = [e for e in zh.namelist() if e.startswith(sourcepaths[-1] + '/')]
-                    else:
-                        entries = [sourcepaths[-1]]
-
-                    with open_archive_path(targetpaths, 'w') as zh2:
-                        cut = len(sourcepaths[-1])
-                        for entry in entries:
-                            info = zh.getinfo(entry)
-                            info.filename = targetpaths[-1] + entry[cut:]
-                            zh2.writestr(info, zh.read(entry),
-                                         compress_type=info.compress_type,
-                                         compresslevel=None if info.compress_type == zipfile.ZIP_STORED else 9,
-                                         )
+    target = request.values.get('target')
+    if target is None:
+        abort(400, 'Target is not specified.')
+    targetpaths = util.fs.CPath.resolve(target, get_localpath).path
+    targetpaths[0] = get_localpath(targetpaths[0])
 
-    except HTTPException:
-        raise
+    try:
+        util.fs.copy(localpaths, targetpaths)
+    except util.fs.FSEntryExistsError:
+        abort(400, 'Target already exists.')
+    except util.fs.FSEntryNotFoundError:
+        abort(404, 'Source does not exist.')
+    except util.fs.FSPartialError:
+        abort(500, 'Fail to copy some files.')
     except Exception:
         traceback.print_exc()
         abort(500, 'Unable to copy to the target.')
 
 
 @handle_action_advanced
 @handle_action_token
 def action_backup():
     """Bakup file or directory."""
     format = request.format
 
-    if not format:
+    if format != 'json':
         abort(400, 'Action not supported.')
 
     localpaths = request.localpaths
 
     if len(localpaths) > 1:
         abort(400, 'Unable to backup inside a zip file.')
 
     ts = request.values.get('ts') or util.datetime_to_id()
     note = request.values.get('note')
     move = request.values.get('move', default=False, type=bool)
 
-    host.init_backup(ts, note=note)
-    try:
-        host.auto_backup(localpaths[0], move=move)
-        return http_response(os.path.basename(host._backup_dir), format=request.format)
-    finally:
-        host.init_backup(False)
+    backup_dir = host.get_auto_backup_dir(ts, note=note)
+    host.backup(localpaths[0], backup_dir=backup_dir, move=move)
+    return http_response(os.path.basename(backup_dir), format=request.format)
 
 
 @handle_action_advanced
 @handle_action_token
 def action_unbackup():
     """Remove a backup."""
     format = request.format
 
-    if not format:
+    if format != 'json':
         abort(400, 'Action not supported.')
 
     ts = request.values.get('ts') or util.datetime_to_id()
     note = request.values.get('note')
 
-    host.init_backup(ts, note=note)
-    try:
-        host.unbackup(host._backup_dir)
-        return http_response(os.path.basename(host._backup_dir), format=request.format)
-    finally:
-        host.init_backup(False)
+    backup_dir = host.get_auto_backup_dir(ts, note=note)
+    host.unbackup(backup_dir)
+    return http_response(os.path.basename(backup_dir), format=request.format)
 
 
+@handle_action_advanced
 @handle_action_token
 def action_cache():
     """Invoke the cacher."""
     format = request.format
 
+    book_ids = request.values.getlist('book')
+    item_ids = request.values.getlist('item')
+    book_items = {}
+    for i, book_id in enumerate(book_ids):
+        book_items[book_id] = request.values.getlist(f'item[{i}]') + item_ids
+
     kwargs = {
-        'book_ids': request.values.getlist('book'),
-        'item_ids': request.values.getlist('item'),
-        'no_lock': request.values.get('no_lock', default=False, type=bool),
-        'no_backup': request.values.get('no_backup', default=False, type=bool),
+        'book_items': book_items,
+        'lock': not request.values.get('no_lock', default=False, type=bool),
+        'backup': not request.values.get('no_backup', default=False, type=bool),
         'fulltext': request.values.get('fulltext', default=False, type=bool),
-        'inclusive_frames': request.values.get('inclusive_frames', default=False, type=bool),
         'recreate': request.values.get('recreate', default=False, type=bool),
         'static_site': request.values.get('static_site', default=False, type=bool),
-        'static_index': request.values.get('static_index', default=False, type=bool),
-        'rss_root': request.values.get('rss_root'),
-        'rss_item_count': request.values.get('rss_item_count', default=50, type=int),
-        'locale': request.values.get('locale'),
+        'static_index': request.values.get('static_index', default=None, type=bool),
+        'rss': request.values.get('rss', default=None, type=bool),
     }
 
-    headers = {
-        'Cache-Control': 'no-store',
-    }
-    root = host.root
-    config = host.config
+    gen = wsb_cache.generate((host.root, host.config), **kwargs)
 
     if format == 'sse':
-        def gen():
-            for info in wsb_cache.generate(root, config=config, **kwargs):
-                data = {
+        def wrapper():
+            for info in gen:
+                yield json.dumps({
                     'type': info.type,
                     'msg': info.msg,
-                }
+                }, ensure_ascii=False)
 
-                yield json.dumps(data, ensure_ascii=False)
-
-        return http_response(gen(), headers=headers, format=format)
+        return http_response(wrapper(), format=format)
 
     elif format:
-        abort(400, 'Action not supported.')
-
-    def gen():
-        yield from wsb_cache.generate(root, config=config, **kwargs)
+        for info in gen:
+            if info.type == 'critical':
+                abort(500, info.msg)
+        return None
 
     stream = stream_template('cli.html',
                              title='Indexing...',
-                             messages=gen(),
+                             messages=gen,
                              debug=False,
                              )
 
-    return Response(stream, headers=headers)
+    return Response(stream)
 
 
+@handle_action_advanced
 @handle_action_token
 def action_check():
     """Invoke the checker."""
     format = request.format
 
     kwargs = {
         'book_ids': request.values.getlist('book'),
-        'no_lock': request.values.get('no_lock', default=False, type=bool),
-        'no_backup': request.values.get('no_backup', default=False, type=bool),
+        'lock': not request.values.get('no_lock', default=False, type=bool),
+        'backup': not request.values.get('no_backup', default=False, type=bool),
         'resolve_invalid_id': request.values.get('resolve_invalid_id', default=False, type=bool),
         'resolve_missing_index': request.values.get('resolve_missing_index', default=False, type=bool),
         'resolve_missing_index_file': request.values.get('resolve_missing_index_file', default=False, type=bool),
         'resolve_missing_date': request.values.get('resolve_missing_date', default=False, type=bool),
         'resolve_older_mtime': request.values.get('resolve_older_mtime', default=False, type=bool),
         'resolve_toc_unreachable': request.values.get('resolve_toc_unreachable', default=False, type=bool),
         'resolve_toc_invalid': request.values.get('resolve_toc_invalid', default=False, type=bool),
         'resolve_toc_empty_subtree': request.values.get('resolve_toc_empty_subtree', default=False, type=bool),
         'resolve_unindexed_files': request.values.get('resolve_unindexed_files', default=False, type=bool),
         'resolve_absolute_icon': request.values.get('resolve_absolute_icon', default=False, type=bool),
         'resolve_unused_icon': request.values.get('resolve_unused_icon', default=False, type=bool),
     }
 
-    headers = {
-        'Cache-Control': 'no-store',
-    }
-    root = host.root
-    config = host.config
+    gen = wsb_check.run((host.root, host.config), **kwargs)
 
     if format == 'sse':
-        def gen():
-            for info in wsb_check.run(root, config=config, **kwargs):
-                data = {
+        def wrapper():
+            for info in gen:
+                yield json.dumps({
                     'type': info.type,
                     'msg': info.msg,
-                }
+                }, ensure_ascii=False)
 
-                yield json.dumps(data, ensure_ascii=False)
-
-        return http_response(gen(), headers=headers, format=format)
+        return http_response(wrapper(), format=format)
 
     elif format:
-        abort(400, 'Action not supported.')
-
-    def gen():
-        yield from wsb_check.run(root, config=config, **kwargs)
+        for info in gen:
+            if info.type == 'critical':
+                abort(500, info.msg)
+        return None
 
     stream = stream_template('cli.html',
-                             title='Indexing...',
-                             messages=gen(),
+                             title='Checking...',
+                             messages=gen,
                              debug=False,
                              )
 
-    return Response(stream, headers=headers)
+    return Response(stream)
+
+
+@handle_action_advanced
+@handle_action_token
+def action_query():
+    """Perform queries on the scrapbook(s)."""
+    query = request.values.getlist('q', type=json.loads)
+    auto_cache = request.values.get('auto_cache', type=json.loads)
+    details = request.values.get('details', default=False, type=bool)
+    lock = not request.values.get('no_lock', default=False, type=bool)
+
+    try:
+        rv = wsb_util.HostQuery((host.root, host.config),
+                                query, auto_cache, lock=lock).run()
+    except Exception as exc:
+        traceback.print_exc()
+        abort(500, str(exc))
+
+    if details:
+        return http_response(rv, format=request.format)
+
+
+@handle_action_advanced
+def action_search():
+    """Search in scrapbooks."""
+    format = request.format
+
+    if format != 'json':
+        abort(400, 'Action not supported.')
+
+    kwargs = {
+        'query': request.values.get('q', default=''),
+        'context': {
+            'title': -1,
+            'file': -1,
+            'comment': request.values.get('comment', default=None, type=int),
+            'source': request.values.get('source', default=None, type=int),
+            'fulltext': request.values.get('fulltext', default=None, type=int),
+        },
+        'lock': not request.values.get('no_lock', default=False, type=bool),
+    }
+
+    data = {}
+    try:
+        for item in wsb_search.search((host.root, host.config), **kwargs):
+            data.setdefault(item.book_id, []).append({
+                'id': item.id,
+                'file': item.file,
+                'context': item.context,
+            })
+    except wsb_search.QueryError as exc:
+        abort(400, str(exc))
+
+    return http_response(data, format=format)
 
 
 @bp.before_request
 def handle_before_request():
     # handle authorization
     try:
         auth_config = host.config['auth']
@@ -1882,15 +1392,15 @@
 
 @bp.route('/', methods=['GET', 'HEAD', 'POST'])
 @bp.route('/<path:filepath>', methods=['GET', 'HEAD', 'POST'])
 def handle_request(filepath=''):
     """Handle an HTTP request (HEAD, GET, POST).
     """
     try:
-        handler = globals().get(f'action_{request.action}') or action_unknown
+        handler = globals()[f'action_{request.action}']
         return handler()
     except PermissionError:
         abort(403)
 
 
 @bp.after_request
 def handle_after_request(response):
@@ -1910,18 +1420,26 @@
     if request.format == 'json':
         response = exc.get_response()
         response.data = json.dumps({
             'error': {
                 'status': exc.code,
                 'message': exc.description,
             },
-        })
+        }, ensure_ascii=False)
         response.content_type = 'application/json'
         return response
 
+    if request.format == 'sse':
+        response = exc.get_response()
+        response.data = ''.join(generate_server_sent_events((
+            json.dumps({'type': 'critical', 'msg': exc.description}, ensure_ascii=False),
+        )))
+        response.content_type = 'text/event-stream'
+        return response
+
     return exc
 
 
 class WebHost(wsb_host.Host):
     """Extended Host class that also handles HTTP server related things.
 
     - Token handling: security token validation to avoid CSRF attack.
@@ -2028,14 +1546,202 @@
         app.wsgi_app = ProxyFix(app.wsgi_app, **xheaders)
 
     app.jinja_loader = jinja2.FileSystemLoader(_host.templates)
     app.jinja_env.globals.update({
         'os': os,
         'time': time,
         'get_breadcrumbs': get_breadcrumbs,
-        'format_filesize': util.format_filesize,
+        'format_filesize': functools.partial(util.format_filesize, space='\xA0'),
         'quote_path': quote_path,
         'static_url': static_url,
         'i18n': _host.get_i18n(_host.config['app']['locale']),
     })
 
     return app
+
+
+#########################################################################
+# Filesystem helpers
+#########################################################################
+
+FileInfo = namedtuple('FileInfo', ('name', 'type', 'size', 'last_modified'))
+
+
+def file_info(file, base=None):
+    """Read basic file information.
+
+    Args:
+        file: path of the file
+        base: path that the result filename is based under
+    """
+    if base is None:
+        name = os.path.basename(file)
+    else:
+        base = os.path.join(base, '')
+        if not file.startswith(base):
+            raise ValueError('file not under base')
+
+        name = util.unify_pathsep(file[len(base):])
+
+    try:
+        statinfo = os.lstat(file)
+    except OSError:
+        # unexpected error when getting stat info
+        statinfo = None
+        size = None
+        last_modified = None
+    else:
+        size = statinfo.st_size
+        last_modified = statinfo.st_mtime
+
+    if not os.path.lexists(file):
+        type = None
+    elif os.path.islink(file) or util.fs.isjunction(file):
+        type = 'link'
+    elif os.path.isdir(file):
+        type = 'dir'
+    elif os.path.isfile(file):
+        type = 'file'
+    else:
+        type = 'unknown'
+
+    if type != 'file':
+        size = None
+
+    return FileInfo(name=name, type=type, size=size, last_modified=last_modified)
+
+
+def listdir(base, recursive=False):
+    """Generates FileInfo(s) and omit invalid entries.
+    """
+    if not recursive:
+        with os.scandir(base) as entries:
+            for entry in entries:
+                info = file_info(entry.path)
+                if info.type is None:
+                    continue
+                yield info
+
+    else:
+        for root, dirs, files in os.walk(base):
+            for dir in dirs:
+                file = os.path.join(root, dir)
+                info = file_info(file, base)
+                if info.type is None:
+                    continue
+                yield info
+            for file in files:
+                file = os.path.join(root, file)
+                info = file_info(file, base)
+                if info.type is None:
+                    continue
+                yield info
+
+
+#########################################################################
+# ZIP helpers
+#########################################################################
+
+class ZipDirNotFoundError(Exception):
+    pass
+
+
+def zip_file_info(zip, subpath, base=None, check_implicit_dir=False):
+    """Read basic file information from ZIP.
+
+    Args:
+        zip: path, file-like object, or zipfile.ZipFile
+        subpath: 'dir' and 'dir/' are both supported
+        base: path that the result filename is based under,
+            'dir' and 'dir/' are both supported
+    """
+    subpath = subpath.rstrip('/')
+    if base is None:
+        name = os.path.basename(subpath)
+    else:
+        base = base.rstrip('/')
+        base = base + ('/' if base else '')
+        if not subpath.startswith(base):
+            raise ValueError('subpath not under base')
+
+        name = subpath[len(base):]
+
+    with nullcontext(zip) if isinstance(zip, zipfile.ZipFile) else zipfile.ZipFile(zip) as zh:
+        try:
+            info = zh.getinfo(subpath)
+        except KeyError:
+            pass
+        else:
+            return FileInfo(
+                name=name, type='file',
+                size=info.file_size,
+                last_modified=util.fs.zip_timestamp(info),
+            )
+
+        try:
+            info = zh.getinfo(subpath + '/')
+        except KeyError:
+            pass
+        else:
+            return FileInfo(
+                name=name, type='dir', size=None,
+                last_modified=util.fs.zip_timestamp(info),
+            )
+
+        if check_implicit_dir:
+            base = subpath + ('/' if subpath else '')
+            for entry in zh.namelist():
+                if entry.startswith(base):
+                    return FileInfo(name=name, type='dir', size=None, last_modified=None)
+
+    return FileInfo(name=name, type=None, size=None, last_modified=None)
+
+
+def zip_listdir(zip, subpath, recursive=False):
+    """Generates FileInfo(s) and omit invalid entries.
+
+    Raise ZipDirNotFoundError if subpath does not exist.
+
+    NOTE: It is possible that entry mydir/ does not exist while mydir/foo.bar
+    exists. Check for matching subentries to make sure whether the implicit
+    directory exists.
+
+    Args:
+        zip: path, file-like object, or zipfile.ZipFile
+        subpath: the subpath in the ZIP, with or without trailing slash
+    """
+    base = subpath.rstrip('/')
+    if base:
+        base += '/'
+    base_len = len(base)
+    dir_exist = not base
+    entries = {}
+
+    with nullcontext(zip) if isinstance(zip, zipfile.ZipFile) else zipfile.ZipFile(zip) as zh:
+        for filename in zh.namelist():
+            if not filename.startswith(base):
+                continue
+
+            if filename == base:
+                dir_exist = True
+                continue
+
+            entry = filename[base_len:]
+            if not recursive:
+                entry, _, _ = entry.partition('/')
+                entries.setdefault(entry, True)
+            else:
+                parts = entry.rstrip('/').split('/')
+                for i in range(0, len(parts)):
+                    entry = '/'.join(parts[0:i + 1])
+                    entries.setdefault(entry, True)
+
+        if not entries and not dir_exist:
+            raise ZipDirNotFoundError(f'Directory {base!r} does not exist in the zip.')
+
+        for entry in entries:
+            info = zip_file_info(zh, base + entry, base)
+
+            if info.type is None:
+                yield FileInfo(name=entry, type='dir', size=None, last_modified=None)
+            else:
+                yield info
```

### Comparing `webscrapbook-1.9.0/webscrapbook/cli.py` & `webscrapbook-2.0.0b8/webscrapbook/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 """Command line interface of WebScrapBook toolkit.
 """
 import argparse
 import os
 import shutil
 import sys
+import time
 import traceback
 from getpass import getpass
 from inspect import getdoc
-from time import time_ns
 
-from . import (
-    WSB_CONFIG,
-    WSB_DIR,
-    WSB_USER_CONFIG,
-    __version__,
-    config,
-    server,
-    util,
-)
+from . import WSB_CONFIG, WSB_DIR, WSB_USER_CONFIG, __version__, config, util
+from ._polyfill.argparse import BooleanOptionalAction
 
 
 def log(*args):
     print(*args)
 
 
 def die(*args):
@@ -51,169 +44,192 @@
                 fw.write(line)
 
 
 def cmd_serve(args):
     """Serve the root directory forever. Shutdown via Ctrl+C or another killing
     technique.
 
-    By default the local browser will be launched to view the served (hosted) site.
-    This behavior can be changed using the `server.browse` config.
-
     Note that this built-in server is designed only for local hosting, or remote
     hosting for personal or few people usage. For an opened world wide web hosting,
-    a more specialized server should be used."""
+    a more specialized server should be used.
+    """
+    from . import server
     server.serve(**args)
 
 
 def cmd_config(args):
     """Show, generate, or edit the config.
 
     Display the current config when used with no arguments.
 
     Run `wsb help config` for details about config.
     """
     if args['book']:
         fdst = os.path.normpath(os.path.join(args['root'], WSB_DIR, WSB_CONFIG))
         fsrc = os.path.normpath(os.path.join(__file__, '..', 'resources', 'config.ini'))
         if not os.path.isfile(fdst):
-            log(f'Generating "{fdst}"...')
+            log(f'Generating {fdst!r}...')
             try:
                 fcopy(fsrc, fdst)
             except OSError:
                 die(f'Unable to generate {fdst}.')
 
         if args['edit']:
             try:
-                util.launch(fdst)
+                util.fs.launch(fdst)
             except OSError:
                 pass
 
         if args['all']:
             fdst = os.path.normpath(os.path.join(args['root'], WSB_DIR, 'serve.py'))
             fsrc = os.path.normpath(os.path.join(__file__, '..', 'resources', 'serve.py'))
             if not os.path.isfile(fdst):
-                log(f'Generating "{fdst}"...')
+                log(f'Generating {fdst!r}...')
                 try:
                     fcopy(fsrc, fdst)
                     os.chmod(fdst, os.stat(fdst).st_mode | (0o111 & ~get_umask()))
                 except OSError:
-                    die(f'Unable to generate {fdst}.')
+                    die(f'Unable to generate {fdst!r}.')
 
             fdst = os.path.normpath(os.path.join(args['root'], WSB_DIR, 'app.py'))
             fsrc = os.path.normpath(os.path.join(__file__, '..', 'resources', 'app.py'))
             if not os.path.isfile(fdst):
-                log(f'Generating "{fdst}"...')
+                log(f'Generating {fdst!r}...')
                 try:
                     fcopy(fsrc, fdst)
                     os.chmod(fdst, os.stat(fdst).st_mode | (0o111 & ~get_umask()))
                 except OSError:
                     die(f'Unable to generate {fdst}.')
 
     elif args['user']:
         fdst = WSB_USER_CONFIG
         fsrc = os.path.normpath(os.path.join(__file__, '..', 'resources', 'config.ini'))
         if not os.path.isfile(fdst):
-            log(f'Generating "{fdst}"...')
+            log(f'Generating {fdst!r}...')
             try:
                 fcopy(fsrc, fdst)
             except OSError:
                 die(f'Unable to generate {fdst}.')
 
         if args['edit']:
             try:
-                util.launch(fdst)
+                util.fs.launch(fdst)
             except OSError:
                 pass
 
     elif args['edit']:
         die('Use --edit in combine with --book or --user.')
 
     elif args['all']:
         die('Use --all in combine with --book.')
 
     elif args['name']:
         config.load(args['root'])
         value = config.getname(args['name'])
 
         if value is None:
-            die(f"""Config entry "{args['name']}" does not exist""")
+            die(f"""Config entry {args['name']!r} does not exist""")
 
         print(value)
 
     else:
         config.load(args['root'])
         config.dump(sys.stdout)
 
 
 def cmd_encrypt(args):
     """Generate an encrypted password string.
 
     Primilarly to be used in auth config.
     """
-    if args['password'] is None:
+    pw = args['password']
+    if pw is None:
         pw1 = getpass('Enter a password: ')
         pw2 = getpass('Confirm the password: ')
 
         if pw1 != pw2:
             die('Entered passwords do not match.')
 
-        args['password'] = pw1
+        pw = pw1
 
-    print(util.encrypt(args['password'], salt=args['salt'], method=args['method']))
+    print(util.encrypt(pw, salt=args['salt'], method=args['method']))
 
 
 def cmd_cache(args):
-    """Generate (or update) fulltext cache and/or static site pages.
-    """
+    """Generate (or update) fulltext cache and/or static site pages."""
     kwargs = args.copy()
+    root = kwargs.pop('root')
     debug = kwargs.pop('debug')
 
+    book_ids = kwargs.pop('book_ids')
+    item_ids_list = kwargs.pop('item_ids_list')
+    book_items = {}
+    for i, book_id in enumerate(book_ids):
+        try:
+            item_ids = item_ids_list[i]
+        except (TypeError, IndexError):
+            item_ids = None
+        book_items[book_id] = item_ids
+
     from .scrapbook import cache
-    for info in cache.generate(**kwargs):
+    for info in cache.generate(root, book_items, **kwargs):
         if info.type != 'debug' or debug:
             log(f'{info.type.upper()}: {info.msg}')
 
 
 def cmd_export(args):
     """Export data items into archive files (*.wsba).
+
+    The export/import utilities provide a basic way to backup and restore the
+    data and metadata (i.e. item properties) of specific item(s). To
+    reconstruct the original scrapbook tree the exported archive files should
+    be re-imported together using the original Unicode filename order.
+
+    For a reliable way to backup and restore the scrapbook tree as well as the
+    items, it's generally more recommended to create another scrapbook and copy
+    items between them.
     """
     kwargs = args.copy()
+    root = kwargs.pop('root')
     debug = kwargs.pop('debug')
 
     from .scrapbook import exporter
-    for info in exporter.run(**kwargs):
+    for info in exporter.run(root, **kwargs):
         if info.type != 'debug' or debug:
             log(f'{info.type.upper()}: {info.msg}')
 
 
 def cmd_import(args):
     """Import data items from archive files (*.wsba).
 
-    To faithfully recover original tree structure, import items using the same
-    order as how they have been exported.
+    To faithfully reconstruct the original scrapbook tree, the archive files
+    should be imported together using the same Unicode filename order as how
+    they have been exported.
     """
     kwargs = args.copy()
+    root = kwargs.pop('root')
     debug = kwargs.pop('debug')
 
     from .scrapbook import importer
-    for info in importer.run(**kwargs):
+    for info in importer.run(root, **kwargs):
         if info.type != 'debug' or debug:
             log(f'{info.type.upper()}: {info.msg}')
 
 
 def cmd_check(args):
     """Integrity check and fix for scrapbook data.
 
     (TOC = table of contents)
     """
     kwargs = args.copy()
+    root = kwargs.pop('root')
     debug = kwargs.pop('debug')
 
     from .scrapbook import check
-    for info in check.run(**kwargs):
+    for info in check.run(root, **kwargs):
         if info.type != 'debug' or debug:
             log(f'{info.type.upper()}: {info.msg}')
 
 
 def cmd_convert(args):
     """Convert data between different formats.
 
@@ -223,23 +239,35 @@
     """
     kwargs = args.copy()
     kwargs.pop('root')
     mode = kwargs.pop('mode')
     force = kwargs.pop('force')
     debug = kwargs.pop('debug')
 
+    if mode == 'items':
+        book_ids = kwargs.pop('book_ids')
+        item_ids_list = kwargs.pop('item_ids_list')
+        book_items = {}
+        for i, book_id in enumerate(book_ids or []):
+            try:
+                item_ids = item_ids_list[i]
+            except (TypeError, IndexError):
+                item_ids = None
+            book_items[book_id] = item_ids
+        kwargs['book_items'] = book_items
+
     import importlib
     conv = importlib.import_module(f'.scrapbook.convert.{mode}', __package__)
 
     # validate input and output directory
     input = args['input']
     input = os.path.realpath(input)
 
     if not os.path.isdir(input):
-        die(f'''Input directory not available: "{input}"''')
+        die(f"""Input directory not available: {input!r}""")
 
     output = args['output']
     if output is not None:
         output = os.path.realpath(output)
 
         if os.path.normcase(output) == os.path.normcase(input):
             die("""Unable to output to the input directory""")
@@ -249,41 +277,116 @@
 
         if os.path.normcase(input).startswith(os.path.normcase(os.path.join(output, ''))):
             die("""Unable to output to an ancestor of the input directory""")
 
         if not os.path.lexists(output):
             pass
         elif not os.path.isdir(output):
-            die(f'''Output directory not available: "{output}"''')
+            die(f"""Output directory not available: {output!r}""")
         else:
             if force:
                 # using os.rmtree() frequently cause an error on Windows
                 with os.scandir(output) as dirs:
                     for entry in dirs:
                         try:
                             shutil.rmtree(entry)
                         except NotADirectoryError:
                             os.remove(entry)
             else:
                 with os.scandir(output) as dirs:
                     if next(dirs, None):
-                        die(f'''Output directory not empty: "{output}"''')
+                        die(f"""Output directory not empty: {output!r}""")
 
     for info in conv.run(**kwargs):
         if info.type != 'debug' or debug:
             log(f'{info.type.upper()}: {info.msg}')
 
 
+def cmd_query(args):
+    """Perform queries to the scrapbook(s)."""
+    kwargs = args.copy()
+    root = kwargs.pop('root')
+    input_ = kwargs.pop('input')
+
+    import json
+    from contextlib import nullcontext
+
+    from .scrapbook.util import HostQuery
+
+    if input_ is None:
+        cm = nullcontext(sys.stdin)
+    else:
+        try:
+            cm = open(input_, 'r', encoding='UTF-8-SIG')
+        except OSError:
+            raise RuntimeError('Failed to read the input file') from None
+
+    with cm as fh:
+        try:
+            query = json.loads(fh.read())
+        except Exception as exc:
+            raise RuntimeError(f'Malformed input query: {exc}') from None
+
+    rv = HostQuery(root, query).run()
+    print(json.dumps(rv, ensure_ascii=False))
+
+
+def cmd_search(args):
+    """Search for data items in the scrapbook(s)."""
+    kwargs = args.copy()
+    root = kwargs.pop('root')
+    input_ = kwargs.pop('input')
+    kwargs['context'] = {
+        'title': kwargs.pop('title'),
+        'file': kwargs.pop('file'),
+        'fulltext': kwargs.pop('fulltext'),
+        'comment': kwargs.pop('comment'),
+        'source': kwargs.pop('source'),
+    }
+
+    import json
+    from contextlib import nullcontext
+
+    from .scrapbook import search
+
+    if input_ is None:
+        cm = nullcontext(sys.stdin)
+    else:
+        try:
+            cm = open(input_, 'r', encoding='UTF-8-SIG')
+        except OSError:
+            raise RuntimeError('Failed to read the input file') from None
+
+    with cm as fh:
+        query = fh.read()
+
+    try:
+        for item in search.search(root, query, **kwargs):
+            msg = json.dumps({
+                'book_id': item.book_id,
+                'id': item.id,
+                'file': item.file,
+                'context': item.context,
+            }, ensure_ascii=False)
+            log(msg)
+    except search.QueryError as exc:
+        die(exc)
+    except Exception as exc:
+        traceback.print_exc()
+        die(exc)
+
+
 def cmd_help(args):
-    """Show detailed information about certain topics.
-    """
+    """Show detailed information about certain topics."""
     root = os.path.join(os.path.dirname(__file__), 'resources')
 
     if args['topic'] == 'config':
         file = os.path.join(root, 'config.md')
+    elif args['topic'] == 'themes':
+        file = os.path.join(root, 'themes.md')
     elif args['topic'] == 'mimetypes':
         file = os.path.join(root, 'mimetypes.md')
 
     if file:
         with open(file, 'r', encoding='UTF-8') as fh:
             text = fh.read()
         print(text)
@@ -300,20 +403,20 @@
 
 def view_archive_files(files):
     """View archive file(s) in the browser.
 
     Set default application of MAFF/HTZ archive files to this command to open
     them in the browser directly.
     """
-    import mimetypes
     import tempfile
     import webbrowser
-    import zipfile
     from urllib.request import pathname2url
 
+    from ._polyfill import mimetypes, zipfile
+
     cache_prefix = config['browser']['cache_prefix']
     cache_expire = config['browser']['cache_expire'] * 10 ** 9
     use_jar = config['browser']['use_jar']
     browser = webbrowser.get(config['browser']['command'] or None)
 
     temp_dir = tempfile.gettempdir()
     urls = []
@@ -338,15 +441,15 @@
             for entry in entries:
                 if not entry.name.startswith(dest_prefix):
                     continue
 
                 dest_dir = entry.path
 
                 # update atime
-                atime = time_ns()
+                atime = time.time_ns()
                 stat = os.stat(entry)
                 os.utime(entry, ns=(atime, stat.st_mtime_ns))
                 break
             else:
                 dest_dir = tempfile.mkdtemp(prefix=dest_prefix)
                 with zipfile.ZipFile(file) as zh:
                     zh.extractall(dest_dir)
@@ -360,15 +463,15 @@
 
     # open pages in the browser
     for url in urls:
         browser.open(url)
 
     # remove stale caches
     if not use_jar:
-        t = time_ns()
+        t = time.time_ns()
         with os.scandir(temp_dir) as entries:
             for entry in entries:
                 if not entry.name.startswith(cache_prefix):
                     continue
 
                 atime = os.stat(entry).st_atime_ns
                 if t <= atime + cache_expire:
@@ -384,16 +487,16 @@
 def view():
     """CLI entry point for viewing archive files.
     """
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=getdoc(view_archive_files))
     parser.add_argument(
-        'files', nargs='+',
-        help="""files to view.""")
+        'files', metavar='file', nargs='+',
+        help="""file(s) to view.""")
     args = vars(parser.parse_args())
     view_archive_files(args['files'])
 
 
 def parse_args(argv=None):
     # Improve program name when executed through python -m
     # NOTE: We don't expect a bad command name such as having a space.
@@ -416,19 +519,17 @@
     # subcommand: serve
     parser_serve = subparsers.add_parser(
         'serve', aliases=['s'],
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=getdoc(cmd_serve),
         help="""serve the root directory""")
     parser_serve.add_argument(
-        '--browse', default=None, action='store_true',
-        help="""launch the browser to visit the served directory""")
-    parser_serve.add_argument(
-        '--no-browse', dest='browse', action='store_false',
-        help="""do not launch the browser""")
+        '--browse', default=None, action=BooleanOptionalAction,
+        help="""launch the browser to visit the served directory (default:
+as `server.browse` config)""")
     parser_serve.set_defaults(func=cmd_serve)
 
     # subcommand: config
     parser_config = subparsers.add_parser(
         'config', aliases=['c'],
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=getdoc(cmd_config),
@@ -463,92 +564,66 @@
     parser_encrypt.add_argument(
         '-m', '--method', default='sha1', action='store',
         help="""the encrypt method to use, which is one of: plain, md5, sha1,
 sha224, sha256, sha384, sha512, sha3_224, sha3_256, sha3_384, and sha3_512
 (default: %(default)s)""")
     parser_encrypt.add_argument(
         '-s', '--salt', default='', action='store',
-        help="""the salt to add during encryption.""")
+        help="""the salt to add during encryption""")
 
     # subcommand: cache
     parser_cache = subparsers.add_parser(
         'cache', aliases=['a'],
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=getdoc(cmd_cache),
         help="""update fulltext cache and/or static site pages""")
     parser_cache.set_defaults(func=cmd_cache)
     parser_cache.add_argument(
         'book_ids', metavar='book', nargs='*', action='store',
-        help="""the book ID(s) to generate cache. (default: all books)""")
-    parser_cache.add_argument(
-        '--item', dest='item_ids',
-        metavar='ID', action='store', default=None, nargs='+',
-        help="""the items ID(s) to generate cache (default: all)""")
-    parser_cache.add_argument(
-        '--fulltext', default=True, action='store_true',
-        help="""generate fulltext cache. (default)""")
-    parser_cache.add_argument(
-        '--no-fulltext', dest='fulltext', action='store_false',
-        help="""inverse of --fulltext""")
-    parser_cache.add_argument(
-        '--inclusive-frames', default=True, action='store_true',
-        help="""cache frame content as part of the main page (default). It's
-recommended to recreate fulltext cache when changing this option to prevent
-inconsistency.""")
-    parser_cache.add_argument(
-        '--no-inclusive-frames', dest='inclusive_frames', action='store_false',
-        help="""inverse of --inclusive-frames""")
+        help="""the book ID(s) to generate cache (default: all books)""")
     parser_cache.add_argument(
-        '--recreate', dest='recreate', default=False, action='store_true',
-        help="""ignore current fulltext cache and generate again""")
+        '--item', dest='item_ids_list',
+        metavar='ID', action='append', nargs='*',
+        help="""the items ID(s) to generate cache (specify repeatedly for each
+corresponding book) (default/empty: all items)""")
     parser_cache.add_argument(
-        '--no-recreate', dest='recreate', action='store_false',
-        help="""inverse of --recreate (default)""")
+        '--fulltext', default=True, action=BooleanOptionalAction,
+        help="""generate fulltext cache (default: %(default)s)""")
     parser_cache.add_argument(
-        '--static-site', default=False, action='store_true',
-        help="""generate static site pages""")
-    parser_cache.add_argument(
-        '--no-static-site', dest='static_site', action='store_false',
-        help="""inverse of --static-site (default)""")
-    parser_cache.add_argument(
-        '--static-index', default=False, action='store_true',
-        help="""generate static index.html page""")
-    parser_cache.add_argument(
-        '--no-static-index', dest='static_index', action='store_false',
-        help="""inverse of --static-index (default)""")
-    parser_cache.add_argument(
-        '--rss-root', metavar='ROOT_URL', action='store',
-        help="""generate an RSS feed file for the book, using the specified root URL
-        (usually corresponds to webscrapbook app root)""")
+        '--recreate', dest='recreate', default=False, action=BooleanOptionalAction,
+        help="""ignore current fulltext cache and generate again
+(default: %(default)s)""")
     parser_cache.add_argument(
-        '--rss-item-count', default=50, type=int, action='store',
-        help="""number of items the RSS feed should include (default: %(default)s)""")
+        '--static-site', default=False, action=BooleanOptionalAction,
+        help="""generate static site pages (default: %(default)s)""")
     parser_cache.add_argument(
-        '--locale', action='store',
-        help="""locale for the generated pages (default: system locale)""")
+        '--static-index', default=None, action=BooleanOptionalAction,
+        help="""generate static index.html page  (default: as
+`book.*.static_index` config)""")
     parser_cache.add_argument(
-        '--backup', dest='no_backup', default=True, action='store_false',
-        help="""backup changed files""")
+        '--rss', default=None, action=BooleanOptionalAction,
+        help="""generate an RSS feed file for the book (default: True if
+`--static-site` and `book.*.rss_root` config are set)""")
     parser_cache.add_argument(
-        '--no-backup', action='store_true',
-        help="""do not backup changed files (default)""")
+        '--backup', default=False, action=BooleanOptionalAction,
+        help="""backup changed files (default: %(default)s)""")
     parser_cache.add_argument(
         '--debug', default=False, action='store_true',
         help="""include debug output""")
 
     # subcommand: check
     parser_check = subparsers.add_parser(
         'check', aliases=['k'],
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=getdoc(cmd_check),
         help="""check and fix scrapbook data""")
     parser_check.set_defaults(func=cmd_check)
     parser_check.add_argument(
         'book_ids', metavar='book', nargs='*', action='store',
-        help="""the book ID(s) to check. (default: all books)""")
+        help="""the book ID(s) to check (default: all books)""")
 
     parser_check.add_argument(
         '-r', '--resolve', dest='resolve_all', default=False, action='store_true',
         help="""resolve all found issues (implies all --resolve-*)""")
     parser_check.add_argument(
         '--resolve-invalid-id', default=False, action='store_true',
         help="""remove items with invalid ID from metadata entries""")
@@ -580,16 +655,16 @@
         '--resolve-absolute-icon', default=False, action='store_true',
         help="""cache "icon" property with absolute URL to local favicon directory""")
     parser_check.add_argument(
         '--resolve-unused-icon', default=False, action='store_true',
         help="""remove unused favicon caches""")
 
     parser_check.add_argument(
-        '--no-backup', default=False, action='store_true',
-        help="""do not backup changed files""")
+        '--backup', default=True, action=BooleanOptionalAction,
+        help="""backup changed files (default: %(default)s)""")
     parser_check.add_argument(
         '--debug', default=False, action='store_true',
         help="""include debug output""")
 
     # subcommand: export
     parser_export = subparsers.add_parser(
         'export', aliases=['x'],
@@ -598,17 +673,17 @@
         help="""export data items into archive files (*.wsba)""")
     parser_export.set_defaults(func=cmd_export)
     parser_export.add_argument(
         'output', action='store',
         help="""the output directory""")
     parser_export.add_argument(
         '--book', dest='book_id', metavar='ID', default='', action='store',
-        help="""the book ID to export. (default: "")""")
+        help="""the book ID to export (default: "")""")
     parser_export.add_argument(
-        '--item', dest='item_ids',
+        '--item', dest='items',
         metavar='ID', action='store', default=None, nargs='+',
         help="""the items ID(s) to export (default: all)""")
     parser_export.add_argument(
         '-r', '--recursive', default=False, action='store_true',
         help="""recursively include descendant items of the provided item ID(s)""")
     parser_export.add_argument(
         '-s', '--singleton', default=False, action='store_true',
@@ -657,28 +732,28 @@
     parser_import.set_defaults(func=cmd_import)
     parser_import.add_argument(
         'files', metavar='file', action='store', nargs='+',
         help="""the file(s) to import in order. If a directory is provided, all
 child files are imported in unicode filename order.""")
     parser_import.add_argument(
         '--book', dest='book_id', metavar='ID', default='', action='store',
-        help="""the book ID to import into. (default: "")""")
+        help="""the book ID to import into (default: "")""")
     parser_import.add_argument(
         '--target', dest='target_id', metavar='ID',
         default='root', action='store',
         help="""the target item ID to insert the imported items under (default: "%(default)s")""")
     parser_import.add_argument(
         '--target-index', metavar='INDEX',
         type=int, action='store',
         help="""the index number (starting from 0) the imported items will be
 inserted at (default: last)""")
     parser_import.add_argument(
         '--rebuild-folders', default=False, action='store_true',
         help="""insert imported items under the original parent, and
-auto-generate parent folders if not found. (ignores --target and
+auto-generate parent folders if not found (ignores --target and
 --target-index)""")
     parser_import.add_argument(
         '--resolve-id-used', metavar='MODE',
         default='skip', action='store',
         choices={'skip', 'replace', 'new'},
         help="""what to do if an importing item ID already exists (default: "%(default)s")""")
     parser_import.add_argument(
@@ -726,39 +801,24 @@
         'output', action='store', nargs='?',
         help="""the output directory (default: in-place)""")
     parser_convert_migrate.add_argument(
         '--book', dest='book_ids', metavar='ID',
         nargs='+', action='store',
         help="""ID of the book(s) to convert (default: all books)""")
     parser_convert_migrate.add_argument(
-        '--convert-legacy', default=True,
-        action='store_true',
-        help="""convert data files from legacy ScrapBook (default)""")
-    parser_convert_migrate.add_argument(
-        '--no-convert-legacy', dest='convert_legacy',
-        action='store_false',
-        help="""inverse of --convert-legacy""")
-    parser_convert_migrate.add_argument(
-        '--convert-v1', default=True,
-        action='store_true',
-        help="""convert data to latest WebScrapBook 1.* (default)""")
+        '--convert-legacy', default=True, action=BooleanOptionalAction,
+        help="""convert data files from legacy ScrapBook (default: %(default)s)""")
     parser_convert_migrate.add_argument(
-        '--no-convert-v1', dest='convert_v1',
-        action='store_false',
-        help="""inverse of --convert-convert-v1""")
+        '--convert-v1', default=True, action=BooleanOptionalAction,
+        help="""convert data to latest WebScrapBook 1.* (default: %(default)s)""")
     parser_convert_migrate.add_argument(
-        '--use-native-tags', default=False,
-        action='store_true',
+        '--use-native-tags', default=False, action=BooleanOptionalAction,
         help="""use native HTML tags for converted legacy ScrapBook annotations for better
 compatibility with very old browsers (e.g. IE < 9), with the cost of increased possibility
-to conflict with the web page stylesheets""")
-    parser_convert_migrate.add_argument(
-        '--no-use-native-tags', dest='use_native_tags',
-        action='store_false',
-        help="""inverse of --use-native-tags (default)""")
+to conflict with the web page stylesheets (default: %(default)s)""")
     parser_convert_migrate.add_argument(
         '--force', default=False, action='store_true',
         help="""overwrite everything in the output directory""")
     parser_convert_migrate.add_argument(
         '--debug', default=False, action='store_true',
         help="""include debug output""")
 
@@ -797,17 +857,18 @@
         'output', action='store', nargs='?',
         help="""the output directory (default: in-place)""")
     parser_convert_items.add_argument(
         '--book', dest='book_ids', metavar='ID',
         nargs='+', action='store',
         help="""ID of the book(s) to convert (default: all books)""")
     parser_convert_items.add_argument(
-        '--item', dest='item_ids', metavar='ID',
-        nargs='+', action='store',
-        help="""ID of the item(s) to convert (default: all items)""")
+        '--item', dest='item_ids_list', metavar='ID',
+        nargs='*', action='append',
+        help="""ID of the item(s) to convert (specify repeatedly for each
+corresponding book) (default/empty: all items)""")
     parser_convert_items.add_argument(
         '--format', metavar='FORMAT', action='store',
         choices=['folder', 'htz', 'maff', 'single_file'],
         help="""file format to convert item(s) to (default: no conversion)""")
     parser_convert_items.add_argument(
         '--type', dest='types', metavar='TYPE', action='store', nargs='+',
         default=[''],
@@ -841,20 +902,22 @@
     parser_convert_sb2wsb.add_argument(
         'input', action='store',
         help="""the input directory""")
     parser_convert_sb2wsb.add_argument(
         'output', action='store',
         help="""the output directory""")
     parser_convert_sb2wsb.add_argument(
-        '--no-data-files', default=False, action='store_true',
-        help="""do not convert data files (set this if there's something wrong
-with the conversion, and run "wsb convert migrate" afterwards for advanced options)""")
+        '--data-files', default=True, action=BooleanOptionalAction,
+        help="""convert data files (set this if there's something wrong with
+the conversion, and run "wsb convert migrate" afterwards for advanced options)
+(default: %(default)s)""")
     parser_convert_sb2wsb.add_argument(
-        '--no-backup', default=False, action='store_true',
-        help="""do not copy legacy ScrapBook files not needed by WebScrapBook""")
+        '--backup', default=True, action=BooleanOptionalAction,
+        help="""copy legacy ScrapBook files not needed by WebScrapBook
+(default: %(default)s)""")
     parser_convert_sb2wsb.add_argument(
         '--force', default=False, action='store_true',
         help="""overwrite everything in the output directory""")
     parser_convert_sb2wsb.add_argument(
         '--debug', default=False, action='store_true',
         help="""include debug output""")
 
@@ -886,17 +949,17 @@
         'output', action='store',
         help="""the output directory""")
     parser_convert_wsb2sb.add_argument(
         '--book', dest='book_id', metavar='ID',
         default='', action='store',
         help="""ID of the book to convert (default: "")""")
     parser_convert_wsb2sb.add_argument(
-        '--no-data-files', default=False, action='store_true',
-        help="""do not convert data files (set this if there's something wrong
-for the conversion)""")
+        '--data-files', default=True, action=BooleanOptionalAction,
+        help="""convert data files (set this if there's something wrong for the
+conversion) (default: %(default)s)""")
     parser_convert_wsb2sb.add_argument(
         '--force', default=False, action='store_true',
         help="""overwrite everything in the output directory""")
     parser_convert_wsb2sb.add_argument(
         '--debug', default=False, action='store_true',
         help="""include debug output""")
 
@@ -921,30 +984,33 @@
         'output', action='store',
         help="""the output directory""")
     parser_convert_file2wsb.add_argument(
         '--data-folder-suffix', dest='data_folder_suffixes',
         metavar='SUFFIX', default=None, action='store', nargs='*',
         help="""suffixes of the associated support folder (default: .files _files)""")
     parser_convert_file2wsb.add_argument(
-        '--no-preserve-filename', default=False, action='store_true',
-        help="""allow the converter to rename source files to reduce
-folders and redirections in the output""")
+        '--preserve-filename', default=True, action=BooleanOptionalAction,
+        help="""keep the original filename and generate a wrapping subfolder
+and redirecting index file for non-HTML files (default: %(default)s)""")
     parser_convert_file2wsb.add_argument(
-        '--ignore-ie-meta', default=False, action='store_true',
-        help="""ignore metadata generated by built-in save of Internet
-Explorer or a Chromium-based browser""")
+        '--handle-ie-meta', default=True, action=BooleanOptionalAction,
+        help="""handle metadata generated by built-in save of Internet
+Explorer or a Chromium-based browser (default: %(default)s)""")
     parser_convert_file2wsb.add_argument(
-        '--ignore-singlefile-meta', default=False, action='store_true',
-        help="""ignore metadata generated by SingleFile browser extension""")
+        '--handle-singlefile-meta', default=True, action=BooleanOptionalAction,
+        help="""handle metadata generated by SingleFile browser extension
+(default: %(default)s)""")
     parser_convert_file2wsb.add_argument(
-        '--ignore-savepagewe-meta', default=False, action='store_true',
-        help="""ignore metadata generated by Save Page WE browser extension""")
+        '--handle-savepagewe-meta', default=True, action=BooleanOptionalAction,
+        help="""handle metadata generated by Save Page WE browser extension
+(default: %(default)s)""")
     parser_convert_file2wsb.add_argument(
-        '--ignore-maoxian-meta', default=False, action='store_true',
-        help="""ignore metadata generated by MaoXian web clipper browser extension""")
+        '--handle-maoxian-meta', default=True, action=BooleanOptionalAction,
+        help="""handle metadata generated by MaoXian web clipper browser
+extension (default: %(default)s)""")
     parser_convert_file2wsb.add_argument(
         '--force', default=False, action='store_true',
         help="""overwrite everything in the output directory""")
     parser_convert_file2wsb.add_argument(
         '--debug', default=False, action='store_true',
         help="""include debug output""")
 
@@ -973,56 +1039,113 @@
         'output', action='store',
         help="""the output directory""")
     parser_convert_wsb2file.add_argument(
         '--book', dest='book_id', metavar='ID',
         default='', action='store',
         help="""ID of the book to convert (default: "")""")
     parser_convert_wsb2file.add_argument(
-        '--no-prefix', dest='prefix', default=True, action='store_false',
-        help="""don't prefix output files with position number.""")
+        '--prefix', default=True, action=BooleanOptionalAction,
+        help="""prefix the output files with digits to keep the original tree
+order (default: %(default)s)""")
     parser_convert_wsb2file.add_argument(
         '--force', default=False, action='store_true',
         help="""overwrite everything in the output directory""")
     parser_convert_wsb2file.add_argument(
         '--debug', default=False, action='store_true',
         help="""include debug output""")
 
+    # subcommand: query
+    parser_query = subparsers.add_parser(
+        'query', aliases=['q'],
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        description=getdoc(cmd_query),
+        help="""perform queries on the scrapbook(s)""",
+        epilog="""\
+The input should be a JSON array of objects with following properties:
+  "book": the ID of the book (string)
+  "cmd": the book method to call (string)
+  "args": the positional arguments (array)
+  "kwargs": the keyword arguments (object)
+
+The output is a JSON array with the return values corresponding to each
+command.
+""")
+    parser_query.set_defaults(func=cmd_query)
+    parser_query.add_argument(
+        'input', action='store', nargs='?',
+        help="""the input file with commands to run (default: stdin)""")
+
+    # subcommand: search
+    parser_search = subparsers.add_parser(
+        'search', aliases=['r'],
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        description=getdoc(cmd_search),
+        help="""search for data items in the scrapbook(s)""",
+        epilog="""\
+The output is a line-separated list of JSON objects with following
+properties:
+  "book_id": ID of the book
+  "id": ID of the matched item
+  "file": matched filename of the item
+  "context": context snippets of the match
+""")
+    parser_search.set_defaults(func=cmd_search)
+    parser_search.add_argument(
+        'input', action='store', nargs='?',
+        help="""the input file with search query (default: stdin)""")
+    parser_search.add_argument(
+        '--title', metavar='LEN', type=int, action='store',
+        help="""length of the context title (default: None)""")
+    parser_search.add_argument(
+        '--file', metavar='LEN', type=int, action='store',
+        help="""length of the context filename (default: None)""")
+    parser_search.add_argument(
+        '--fulltext', metavar='LEN', type=int, action='store',
+        help="""length of the context fulltext (default: None)""")
+    parser_search.add_argument(
+        '--comment', metavar='LEN', type=int, action='store',
+        help="""length of the context comment (default: None)""")
+    parser_search.add_argument(
+        '--source', metavar='LEN', type=int, action='store',
+        help="""length of the context source (default: None)""")
+
     # subcommand: help
     parser_help = subparsers.add_parser(
         'help',
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=getdoc(cmd_help),
         help="""show detailed information about certain topics""",
         epilog="""\
 Available TOPICs:
   "config"
+  "themes"
   "mimetypes"
 """)
     parser_help.set_defaults(func=cmd_help)
     parser_help.add_argument(
         'topic', metavar='TOPIC', default=None, action='store',
-        choices=['config', 'mimetypes'],
+        choices=['config', 'themes', 'mimetypes'],
         help="""the topic for details""")
 
     # subcommand: view
     parser_view = subparsers.add_parser(
         'view',
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=getdoc(cmd_view),
         help="""view archive file in the browser""")
     parser_view.set_defaults(func=cmd_view)
     parser_view.add_argument(
-        'files', nargs='+',
-        help="""files to view""")
+        'files', metavar='file', nargs='+',
+        help="""file(s) to view""")
 
     return parser.parse_args(argv)
 
 
-def main():
-    args = vars(parse_args())
+def main(argv=None):
+    args = vars(parse_args(argv))
     try:
         func = args.pop('func')
     except KeyError:
         parse_args(['-h'])
         return
     else:
         if func is cmd_convert and args['mode'] is None:
```

### Comparing `webscrapbook-1.9.0/webscrapbook/locales.py` & `webscrapbook-2.0.0b8/webscrapbook/locales.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     from webscrapbook.locales import I18N
     i18n = I18N(<dirs>, 'en', 'messages')
     i18n('something to translate')
 
 @TODO: Consider using official gettext for i18n.
 """
 import hashlib
-import locale
 import os
 
 from . import util
 
 DEFAULT_LANG = 'en'
 
 PREFIX_LOCALE = '@@ui_locale'
@@ -39,16 +38,14 @@
     """
     def __init__(self, dirs, lang=None, domain=None):
         """Initialize an i18n translator
 
         Loads <dir>/<lang>/<domain>.py where <dir> is listed in dirs.
         """
         if not lang:
-            lang, _ = locale.getdefaultlocale()
-        if not lang:
             lang = DEFAULT_LANG
 
         # normalize lang to lower_snake_case
         lang = lang.replace('-', '_').lower()
 
         if not domain:
             domain = 'messages'
```

### Comparing `webscrapbook-1.9.0/webscrapbook/resources/config.ini` & `webscrapbook-2.0.0b8/webscrapbook/resources/config.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-; Run "webscrapbook help config" for details
+; Run "wsb help config" for details
 
 [app]
 ; name = WebScrapBook
 ; theme = default
 ; locale =
 ; root = .
 ; index =
@@ -17,14 +17,19 @@
 [book ""]
 name = scrapbook
 top_dir = 
 data_dir = data
 tree_dir = tree
 index = tree/map.html
 no_tree = false
+new_at_top = false
+inclusive_frames = true
+static_index = false
+rss_root = 
+rss_item_count = 50
 
 ; [auth "user1"]
 ; user = myuser1
 ; pw = 73337dfdaf99b87be97cb4b4f16645e059da6e5f
 ; pw_salt = mysalt1
 ; pw_type = sha1
 ; permission = all
```

### Comparing `webscrapbook-1.9.0/webscrapbook/resources/config.md` & `webscrapbook-2.0.0b8/webscrapbook/resources/config.md`

 * *Files 5% similar despite different names*

```diff
@@ -71,30 +71,26 @@
 
 (default: `WebScrapBook`)
 
 
 #### `theme`
 
 The theme name of the served website. A custom theme can be defined at
-`<host>/.wsb/themes/<name>`, which contains:
-- a `templates` sub-directory for template files;
-- a `static` sub-directory for static files;
-- a `locales` sub-directory for localizations.
-
-If the custom theme has a same name as the built-in one, the application
-will look up for a resource first from custom one and fallback to the
-default one when not found.
+`<root>/.wsb/themes/<name>`. Run `wsb help themes` for more details.
 
 (default: `default`)
 
 
 #### `locale`
 
-The locale name of web interface of the served website. Use system locale if
-left empty.
+The locale code of web interface of the served website. It should follow
+RFC 1766 format case insensitively and can use `-` or `_` as the tag separator.
+The localized string will be searched from the theme or package in a
+hierarchical way. For example, `zh_TW` will be looked up in `zh_TW`, `zh`, and
+then `en` as the final fallback.
 
 (default: )
 
 
 #### `root`
 
 The chrooted directory to host. Files outside this directory are not directly
@@ -185,16 +181,17 @@
 
 (default: `0`)
 
 
 ### `[book]` section(s)
 
 The book section(s) define scrapbooks of a host. It can be subsected as
-`[book "identifier"]`. The primary scrapbook (`[book]` or `[book ""]`)
-is used by default. Additional scrapbooks can be defined and be switched into.
+`[book "identifier"]` (with an identifier being alphanumeric and starts with an
+alphabet). The primary scrapbook (`[book]` or `[book ""]`) is used by default.
+Additional scrapbooks can be defined and be switched into.
 
 
 #### `name`
 
 Defines the name of the scrapbook.
 
 (default: `scrapbook`)
@@ -241,20 +238,64 @@
 #### `no_tree`
 
 Set true to disable virtual tree and index of the book.
 
 (default: `false`)
 
 
+#### `new_at_top`
+
+Put newly added items at the top of the scrapbook tree rather than at the
+bottom. Multiple items will remain the original order when inserted together.
+(e.g. Moving items `A, B, C` into another item having children `X, Y, Z`
+gets `A, B, C, X, Y, Z`.)
+
+(default: `false`)
+
+
+#### `inclusive_frames`
+
+Cache the content of frame pages as part of the main page. The fulltext cache
+should be recreated if this config is changed, to prevent an inconsistency.
+
+(default: `true`)
+
+
+#### `static_index`
+
+Set true to generate an additional `index.html` page when generating static
+site pages. The page provides a static list of data items, for SEO and for a
+client not supporting JavaScript to browse. However, the page takes more time
+to generate and usually loads slower than the dynamic `map.html`.
+
+(default: `false`)
+
+
+#### `rss_root`
+
+The public absolute root URL of the site, to be used by the generated RSS feed.
+No RSS feed will be generated if left blank.
+
+(default: )
+
+
+#### `rss_item_count`
+
+Items in the generated RSS feed.
+
+(default: `50`)
+
+
 ### `[auth]` section(s)
 
 The `[auth]` section(s) define authorization rules. It can be subsected as
-`[auth "identifier"]`. Authorization requirement is activated when at least one
-`[auth]` section exists. Each section defines a rule, and the user must
-fullfill at least one to be allowed to access.
+`[auth "identifier"]` (with an identifier being alphanumeric and starts with an
+alphabet). Authorization requirement is activated when at least one `[auth]`
+section exists. Each section defines a rule, and the user must fullfill at
+least one to be allowed to access.
 
 An encrypted password can be generated via the `encrypt` sub-command, For
 example:
 
     webscrapbook encrypt -m sha1 -s mysalt
 
 You'll then be promopted to input a password, and then you can use the output
```

### Comparing `webscrapbook-1.9.0/webscrapbook/resources/mimetypes.md` & `webscrapbook-2.0.0b8/webscrapbook/resources/mimetypes.md`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/scrapbook/cache.py` & `webscrapbook-2.0.0b8/webscrapbook/scrapbook/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """Generator of fulltext cache and/or static site pages.
 """
 import copy
 import functools
 import html
 import io
 import itertools
-import mimetypes
 import os
 import re
 import shutil
 import time
 import traceback
-import zipfile
 from collections import UserDict, namedtuple
 from contextlib import nullcontext
 from datetime import datetime, timezone
 from urllib.parse import quote, unquote, urljoin, urlsplit
 
 import jinja2
 from lxml import etree
 
 from .. import util
+from .._polyfill import mimetypes, zipfile
 from ..util import Info
 from .host import Host
 
 
 class MutatingDict(UserDict):
     """Support adding during dict iteration.
     """
@@ -74,31 +73,31 @@
         'folder': 'icon/fclose.png',
         'file': 'icon/file.png',
         'image': 'icon/file.png',
         'note': 'icon/note.png',  # ScrapBook X notex
         'postit': 'icon/postit.png',  # ScrapBook X note
     }
 
-    def __init__(self, book, *, locale=None,
-                 static_index=False, rss=False,
-                 ):
+    def __init__(self, book, *, static_index=None):
         self.host = book.host
         self.book = book
-        self.static_index = static_index
-        self.locale = locale
+        self.locale = self.host.config['app']['locale']
+        self.rss = bool(self.book.config['rss_root'])
 
-        self.rss = rss
+        if static_index is None:
+            static_index = self.book.config['static_index']
+        self.static_index = static_index
 
         self.template_env = jinja2.Environment(
             loader=jinja2.FileSystemLoader(self.host.templates),
             autoescape=jinja2.select_autoescape(['html']),
         )
         self.template_env.globals.update({
             'format_string': util.format_string,
-            'i18n': self.host.get_i18n(locale),
+            'i18n': self.host.get_i18n(self.locale),
             'bookname': book.name,
         })
 
         book.load_meta_files()
         book.load_toc_files()
 
     def run(self):
@@ -131,66 +130,66 @@
         yield from self._generate_page('frame.html', 'static_frame.html')
 
         yield from self._generate_page(
             'search.html', 'static_search.html',
             path=util.get_relative_url(self.book.top_dir, self.book.tree_dir),
             data_dir=util.get_relative_url(self.book.data_dir, self.book.top_dir),
             tree_dir=util.get_relative_url(self.book.tree_dir, self.book.top_dir),
-            index=self.host.config['book'][self.book.id]['index'],
+            index=self.book.config['index'],
         )
 
     def _generate_resource_file(self, src, dst):
-        yield Info('debug', f'Checking resource file "{dst}"')
+        yield Info('debug', f'Checking resource file {dst!r}')
         fsrc = self.host.get_static_file(src)
         fdst = os.path.normpath(os.path.join(self.book.tree_dir, dst))
 
         # check whether writing is required
         if os.path.isfile(fdst):
             if os.stat(fsrc).st_size == os.stat(fdst).st_size:
                 if util.checksum(fsrc) == util.checksum(fdst):
-                    yield Info('debug', f'Skipped resource file "{dst}" (up-to-date)')
+                    yield Info('debug', f'Skipped resource file {dst!r} (up-to-date)')
                     return
 
         # save file
-        yield Info('info', f'Generating resource file "{dst}"')
+        yield Info('info', f'Generating resource file {dst!r}')
         try:
             os.makedirs(os.path.dirname(fdst), exist_ok=True)
             fsrc = self.host.get_static_file(src)
             self.book.backup(fdst)
             shutil.copyfile(fsrc, fdst)
         except OSError as exc:
-            yield Info('error', f'Failed to create resource file "{dst}": {exc.strerror}', exc=exc)
+            yield Info('error', f'Failed to create resource file {dst!r}: {exc.strerror}', exc=exc)
 
     def _generate_page(self, dst, tpl, **kwargs):
-        yield Info('debug', f'Checking page "{dst}"')
+        yield Info('debug', f'Checking page {dst!r}')
         fsrc = io.BytesIO()
         fdst = os.path.normpath(os.path.join(self.book.tree_dir, dst))
 
         template = self.template_env.get_template(tpl)
         content = template.render(**kwargs)
         fsrc.write(content.encode('UTF-8'))
 
         # check whether writing is required
         if os.path.isfile(fdst):
             if fsrc.getbuffer().nbytes == os.stat(fdst).st_size:
                 fsrc.seek(0)
                 if util.checksum(fsrc) == util.checksum(fdst):
-                    yield Info('debug', f'Skipped page "{dst}" (up-to-date)')
+                    yield Info('debug', f'Skipped page {dst!r} (up-to-date)')
                     return
 
         # save file
-        yield Info('info', f'Generating page "{dst}"')
+        yield Info('info', f'Generating page {dst!r}')
         try:
             fsrc.seek(0)
             os.makedirs(os.path.dirname(fdst), exist_ok=True)
             self.book.backup(fdst)
             with open(fdst, 'wb') as fh:
                 shutil.copyfileobj(fsrc, fh)
         except OSError as exc:
-            yield Info('error', f'Failed to create page file "{dst}": {exc.strerror}', exc=exc)
+            yield Info('error', f'Failed to create page file {dst!r}: {exc.strerror}', exc=exc)
 
     def _generate_static_index(self):
         def get_class_text(classes, prefix=' '):
             if not classes:
                 return ''
 
             c = html.escape(' '.join(classes))
@@ -263,47 +262,46 @@
                 yield StaticIndexItem('end', level, id, meta_type, meta_marked, title, href, icon, meta_source, meta_comment)
 
             level -= 1
             yield StaticIndexItem('end-container', level)
 
         book = self.book
         level = 0
-        id_chain = {'root'}
-        yield from add_child_items('root')
+        id_chain = {book.ROOT_ITEM_ID}
+        yield from add_child_items(book.ROOT_ITEM_ID)
 
 
 class RssFeedGenerator():
     """Main class for RSS feed generation.
     """
     NS = 'http://www.w3.org/2005/Atom'
 
-    def __init__(self, book, *, rss_root=None, item_count=50):
+    def __init__(self, book):
         self.book = book
-        self.rss_root = rss_root.rstrip('/') + '/'
-        self.item_count = item_count
-
-        book.load_meta_files()
-        book.load_toc_files()
+        self.rss_root = book.config['rss_root'].rstrip('/') + '/'
+        self.item_count = book.config['rss_item_count']
 
     def run(self):
         yield Info('info', 'Generating RSS feed...')
 
         book = self.book
         rss_root = self.rss_root
 
         # RSS root must be an absolute URL
         u = urlsplit(rss_root)
         if not (u.scheme and u.netloc):
-            yield Info('error', f'Invalid RSS root URL "{rss_root}"')
+            yield Info('error', f'Invalid RSS root URL {rss_root!r}')
             return
 
         id_prefix = re.sub(r'/+$', '', f'urn:webscrapbook:{u.netloc}{u.path}')
         data_url = urljoin(rss_root, util.get_relative_url(book.data_dir, book.root))
         tree_url = urljoin(rss_root, util.get_relative_url(book.tree_dir, book.root))
 
+        book.load_meta_files()
+
         # get latest updated item entries
         entries = []
         for id, meta in book.meta.items():
             # show only items with content,
             # either with index or a bookmark with source
             if meta.get('type') in {'folder', 'separator'}:
                 continue
@@ -383,23 +381,23 @@
             if fsrc.getbuffer().nbytes == os.stat(fdst).st_size:
                 fsrc.seek(0)
                 if util.checksum(fsrc) == util.checksum(fdst):
                     yield Info('debug', 'Skipped RSS feed (up-to-date)')
                     return
 
         # save file
-        yield Info('info', 'Generating RSS feed file "feed.atom"')
+        yield Info('info', "Generating RSS feed file 'feed.atom'")
         try:
             fsrc.seek(0)
             os.makedirs(os.path.dirname(fdst), exist_ok=True)
             self.book.backup(fdst)
             with open(fdst, 'wb') as fh:
                 shutil.copyfileobj(fsrc, fh)
         except OSError as exc:
-            yield Info('error', f'Failed to create RSS feed file "feed.atom": {exc.strerror}', exc=exc)
+            yield Info('error', f"Failed to create RSS feed file 'feed.atom': {exc.strerror}", exc=exc)
 
 
 FulltextCacheItem = namedtuple('FulltextCacheItem', ('id', 'meta', 'index', 'indexfile', 'files_to_update'))
 
 
 class FulltextCacheGenerator():
     """Main class for fulltext cache generation.
@@ -414,17 +412,17 @@
         'canvas',
         'noframes', 'noscript', 'noembed',
         'textarea',
         # 'parsererror',
         'svg', 'math',
     }
 
-    def __init__(self, book, *, inclusive_frames=True, recreate=False):
+    def __init__(self, book, *, recreate=False):
         self.book = book
-        self.inclusive_frames = inclusive_frames
+        self.inclusive_frames = self.book.config['inclusive_frames']
         self.recreate = recreate
         self.cache_last_modified = 0
 
     def run(self, item_ids=None):
         """Update fulltext cache for item_ids
 
         Args:
@@ -467,35 +465,35 @@
         else:
             # no change => touch files to prevent falsely detected as outdated
             yield Info('info', 'Touching fulltext files...')
             for file in book.iter_fulltext_files():
                 os.utime(file)
 
     def _cache_item(self, id):
-        yield Info('debug', f'Checking item "{id}"')
+        yield Info('debug', f'Checking item {id!r}')
         book = self.book
 
         # remove id if no meta
         meta = book.meta.get(id)
         if meta is None:
-            yield Info('debug', f'Purging item "{id}" (missing metadata)')
+            yield Info('debug', f'Purging item {id!r} (missing metadata)')
             yield from self._delete_item(id)
             return
 
         # remove id if no index
         index = meta.get('index')
         if not index:
-            yield Info('debug', f'Purging item "{id}" (no index)')
+            yield Info('debug', f'Purging item {id!r} (no index)')
             yield from self._delete_item(id)
             return
 
         # remove id if no index file
         indexfile = os.path.join(book.data_dir, index)
         if not os.path.exists(indexfile):
-            yield Info('debug', f'Purging item "{id}" (missing index file)')
+            yield Info('debug', f'Purging item {id!r} (missing index file)')
             yield from self._delete_item(id)
             return
 
         # a mapping file path => status
         # status: True for a file to be checked; False for a file (mostly
         # an inclusive iframe) that is not available as inline,
         # (already added to cache or to be removed from cache)
@@ -503,97 +501,97 @@
 
         item = FulltextCacheItem(id, meta, index, indexfile, files_to_update)
         yield from self._collect_files_to_update(item)
         yield from self._handle_files_to_update(item)
 
     def _delete_item(self, id):
         if id in self.book.fulltext:
-            yield Info('info', f'Removing stale cache for "{id}".')
+            yield Info('info', f'Removing stale cache for {id!r}.')
             del self.book.fulltext[id]
 
     def _collect_files_to_update(self, item):
         book = self.book
         id, meta, index, indexfile, files_to_update = item
 
         # create cache for this id if not exist yet
         if book.fulltext.get(id) is None:
             book.fulltext[id] = {}
         else:
             # unless newly created, presume no change if archive file not newer
             # than cache file, for better performance
             if util.is_archive(indexfile):
                 if os.stat(indexfile).st_mtime <= self.cache_last_modified:
-                    yield Info('debug', f'Skipped "{id}" (archive file older than cache)')
+                    yield Info('debug', f'Skipped {id!r} (archive file older than cache)')
                     return
 
         # add index file(s) to update list
         try:
             for path in book.get_index_paths(index):
-                yield Info('debug', f'Adding "{path}" of "{id}" to check list (from index)')
+                yield Info('debug', f'Adding {path!r} of {id!r} to check list (from index)')
                 files_to_update[path] = True
         except zipfile.BadZipFile:
             # MAFF file corrupted.
             # Skip adding index files.
             # Treat as no file exists and remove all indexes later on.
-            yield Info('error', f'Archive file for "{id}" is corrupted')
+            yield Info('error', f'Archive file for {id!r} is corrupted')
 
         # add files in cache to update list
         for path in book.fulltext[id]:
-            yield Info('debug', f'Adding "{path}" of "{id}" to check list (from cache)')
+            yield Info('debug', f'Adding {path!r} of {id!r} to check list (from cache)')
             files_to_update[path] = True
 
     def _handle_files_to_update(self, item):
         def report_update():
             nonlocal has_update
             if has_update:
                 return
             if book.fulltext[id]:
-                yield Info('info', f'Updating cache for "{id}"...')
+                yield Info('info', f'Updating cache for {id!r}...')
             else:
-                yield Info('info', f'Generating cache for "{id}"...')
+                yield Info('info', f'Generating cache for {id!r}...')
             has_update = True
 
         book = self.book
         id, meta, index, indexfile, files_to_update = item
         has_update = False
 
         for path in files_to_update:
-            yield Info('debug', f'Checking "{path}" of "{id}"')
+            yield Info('debug', f'Checking {path!r} of {id!r}')
             # remove from cache if marked False
             if not files_to_update[path]:
-                yield Info('debug', f'Purging "{path}" of "{id}" (inlined)')
+                yield Info('debug', f'Purging {path!r} of {id!r} (inlined)')
                 if path in book.fulltext[id]:
                     yield from report_update()
                     del book.fulltext[id][path]
                 continue
 
             # mark False to prevent added otherwhere
             files_to_update[path] = False
 
             mtime = yield from self._get_mtime(item, path)
             if mtime is None:
                 # path not exist => delete from cache
-                yield Info('debug', f'Purging "{path}" of "{id}" (file not exist)')
+                yield Info('debug', f'Purging {path!r} of {id!r} (file not exist)')
                 if path in book.fulltext[id]:
                     yield from report_update()
                     del book.fulltext[id][path]
                 continue
 
             # skip update if the file is not newer
             # - A file hasn't been cached may be newly refrenced by another
             #   updated file, and thus needs update even if it's mtime is not
             #   newer.
             if path in book.fulltext[id] and mtime <= self.cache_last_modified:
-                yield Info('debug', f'Skipped "{path}" of "{id}" (file older than cache)')
+                yield Info('debug', f'Skipped {path!r} of {id!r} (file older than cache)')
                 continue
 
             yield from report_update()
 
             # set updated fulltext
-            yield Info('debug', f'Generating cache for "{path}" of "{id}"')
+            yield Info('debug', f'Generating cache for {path!r} of {id!r}')
             fulltext = yield from self._get_fulltext_cache(item, path)
 
             if fulltext is not None:
                 book.fulltext[id][path] = {
                     'content': fulltext,
                 }
             else:
@@ -603,96 +601,96 @@
                     pass
 
     def _get_mtime(self, item, path):
         if util.is_archive(item.index):
             try:
                 zh = zipfile.ZipFile(os.path.join(self.book.data_dir, item.index))
             except zipfile.BadZipFile as exc:
-                yield Info('error', f'Failed to open zip file "{item.index}" for "{item.id}": {exc}', exc=exc)
+                yield Info('error', f'Failed to open zip file {item.index!r} for {item.id!r}: {exc}', exc=exc)
                 return None
             except (FileNotFoundError, IsADirectoryError, NotADirectoryError) as exc:
-                yield Info('error', f'Failed to open zip file "{item.index}" for "{item.id}": {exc.strerror}', exc=exc)
+                yield Info('error', f'Failed to open zip file {item.index!r} for {item.id!r}: {exc.strerror}', exc=exc)
                 return None
 
             try:
                 with zh as zh:
                     info = zh.getinfo(path)
-                    return util.zip_timestamp(info)
+                    return util.fs.zip_timestamp(info)
             except KeyError:
                 return None
             except Exception as exc:
-                yield Info('error', f'Failed to access in-zip-file for "{path}" of "{item.id}": {exc}', exc=exc)
+                yield Info('error', f'Failed to access in-zip-file for {path!r} of {item.id!r}: {exc}', exc=exc)
                 return None
 
         file = os.path.join(self.book.data_dir, os.path.dirname(item.index), path)
         try:
             return os.stat(file).st_mtime
         except (FileNotFoundError, IsADirectoryError, NotADirectoryError):
             return None
         except OSError as exc:
-            yield Info('error', f'Failed to access file for "{path}" of "{item.id}": {exc.strerror}', exc=exc)
+            yield Info('error', f'Failed to access file for {path!r} of {item.id!r}: {exc.strerror}', exc=exc)
             return None
 
     def _open_file(self, item, path):
         if util.is_archive(item.index):
             try:
                 zh = zipfile.ZipFile(os.path.join(self.book.data_dir, item.index))
             except zipfile.BadZipFile as exc:
-                yield Info('error', f'Failed to open zip file "{item.index}" for "{item.id}": {exc}', exc=exc)
+                yield Info('error', f'Failed to open zip file {item.index!r} for {item.id!r}: {exc}', exc=exc)
                 return None
             except (FileNotFoundError, IsADirectoryError, NotADirectoryError) as exc:
-                yield Info('error', f'Failed to open zip file "{item.index}" for "{item.id}": {exc.strerror}', exc=exc)
+                yield Info('error', f'Failed to open zip file {item.index!r} for {item.id!r}: {exc.strerror}', exc=exc)
                 return None
 
             try:
                 with zh as zh:
                     return zh.open(path)
             except KeyError:
                 return None
             except Exception as exc:
-                yield Info('error', f'Failed to open in-zip-file for "{path}" of "{item.id}": {exc}', exc=exc)
+                yield Info('error', f'Failed to open in-zip-file for {path!r} of {item.id!r}: {exc}', exc=exc)
                 return None
 
         file = os.path.join(self.book.data_dir, os.path.dirname(item.index), path)
         try:
             return open(file, 'rb')
         except (FileNotFoundError, IsADirectoryError, NotADirectoryError):
             return None
         except OSError as exc:
-            yield Info('error', f'Failed to open file for "{path}" of "{item.id}": {exc.strerror}', exc=exc)
+            yield Info('error', f'Failed to open file for {path!r} of {item.id!r}: {exc.strerror}', exc=exc)
             return None
 
     def _get_fulltext_cache(self, item, path):
         fh = yield from self._open_file(item, path)
         if not fh:
-            yield Info('debug', f'Skipped "{path}" of "{item.id}" (file not exist or accessible)')
+            yield Info('debug', f'Skipped {path!r} of {item.id!r} (file not exist or accessible)')
             return None
 
         try:
             mime, _ = mimetypes.guess_type(path)
             return (yield from self._get_fulltext_cache_for_fh(item, path, fh, mime))
         except Exception as exc:
             traceback.print_exc()
-            yield Info('error', f'Failed to generate cache for "{item.id}" ({path}): {exc}', exc=exc)
+            yield Info('error', f'Failed to generate cache for {item.id!r} ({path!r}): {exc}', exc=exc)
             return ''
         finally:
             fh.close()
 
     def _get_fulltext_cache_for_fh(self, item, path, fh, mime, *, is_srcdoc=False):
         if not mime:
-            yield Info('debug', f'Skipped "{path}" of "{item.id}" (unknown type)')
+            yield Info('debug', f'Skipped {path!r} of {item.id!r} (unknown type)')
             return None
 
         if util.mime_is_html(mime):
             return (yield from self._get_fulltext_cache_html(item, path, fh, is_srcdoc=is_srcdoc))
 
         if mime.startswith('text/'):
             return (yield from self._get_fulltext_cache_txt(item, path, fh))
 
-        yield Info('debug', f'Skipped "{path}" of "{item.id}" ("{mime}" not supported)')
+        yield Info('debug', f'Skipped {path!r} of {item.id!r} ({mime!r} not supported)')
         return None
 
     def _get_fulltext_cache_html(self, item, path, fh, *, is_srcdoc=False):
         def get_relative_file_path(url):
             # skip when inside a data URL page (can't resolve)
             if path is None:
                 return None
@@ -727,25 +725,31 @@
 
             return target
 
         def add_datauri_content(url):
             try:
                 data = util.parse_datauri(url)
             except util.DataUriMalformedError as exc:
-                yield Info('error', f'Skipped malformed data URL "{util.crop(url, 256)}": {exc}', exc=exc)
+                yield Info('error', f'Skipped malformed data URL {util.crop(url, 256)!r}: {exc}', exc=exc)
                 return
             fh = io.BytesIO(data.bytes)
             fulltext = yield from self._get_fulltext_cache_for_fh(item, None, fh, data.mime)
             if fulltext:
                 results.append(fulltext)
 
         if is_srcdoc:
-            yield Info('debug', f'Retrieving HTML content for "{path}" (srcdoc) of "{item.id}"')
+            yield Info('debug', f'Retrieving HTML content for {path!r} (srcdoc) of {item.id!r}')
         else:
-            yield Info('debug', f'Retrieving HTML content for "{path}" of "{item.id}"')
+            yield Info('debug', f'Retrieving HTML content for {path!r} of {item.id!r}')
+
+        # return '' for an empty file to prevent a parsing error
+        fh.seek(0, 2)
+        if fh.tell() == 0:
+            return ''
+        fh.seek(0)
 
         charset = util.get_html_charset(fh, default=item.meta.get('charset') or 'UTF-8')
         fh.seek(0)
 
         results = []
         has_instant_redirect = False
         for time_, url, context in util.iter_meta_refresh(fh, encoding=charset):
@@ -759,15 +763,15 @@
                 continue
 
             if url.startswith('data:'):
                 yield from add_datauri_content(url)
             else:
                 target = get_relative_file_path(url)
                 if target and target not in item.files_to_update:
-                    yield Info('debug', f'Adding "{target}" of "{item.id}" to check list (from <meta>)')
+                    yield Info('debug', f'Adding {target!r} of {item.id!r} to check list (from <meta>)')
                     item.files_to_update[target] = True
 
         # Add data URL content of meta refresh targets to fulltext index if the
         # page has an instant meta refresh.
         if has_instant_redirect:
             return self.FULLTEXT_SPACE_REPLACER(' '.join(results)).strip()
 
@@ -808,15 +812,15 @@
                         pass
                     else:
                         if url.startswith('data:'):
                             yield from add_datauri_content(url)
                         else:
                             target = get_relative_file_path(url)
                             if target and target not in item.files_to_update:
-                                yield Info('debug', f'Adding "{target}" of "{item.id}" to check list (from <{elem.tag}>)')
+                                yield Info('debug', f'Adding {target!r} of {item.id!r} to check list (from <{elem.tag}>)')
                                 item.files_to_update[target] = True
 
                 elif elem.tag in ('iframe', 'frame'):
                     # include frame page in fulltext index
                     try:
                         srcdoc = elem.attrib['srcdoc']
                     except KeyError:
@@ -831,22 +835,22 @@
                                 target = get_relative_file_path(url)
                                 if target:
                                     if self.inclusive_frames:
                                         # Add frame content to the current page
                                         # content if the targeted file hasn't
                                         # been indexed.
                                         if item.files_to_update.get(target) is not False:
-                                            yield Info('debug', f'Caching "{target}" of "{item.id}" as inline (from <{elem.tag}>)')
+                                            yield Info('debug', f'Caching {target!r} of {item.id!r} as inline (from <{elem.tag}>)')
                                             item.files_to_update[target] = False
                                             fulltext = yield from self._get_fulltext_cache(item, target)
                                             if fulltext:
                                                 results.append(fulltext)
                                     else:
                                         if target not in item.files_to_update:
-                                            yield Info('debug', f'Adding "{target}" of "{item.id}" to check list (from <{elem.tag}>)')
+                                            yield Info('debug', f'Adding {target!r} of {item.id!r} to check list (from <{elem.tag}>)')
                                             item.files_to_update[target] = True
                     else:
                         fh = io.BytesIO(srcdoc.encode('UTF-8-SIG'))
                         fulltext = yield from self._get_fulltext_cache_for_fh(item, path, fh, 'text/html', is_srcdoc=True)
                         if fulltext:
                             results.append(fulltext)
 
@@ -891,82 +895,93 @@
                     except TypeError:
                         # broken html may generate extra root elem
                         break
 
         return self.FULLTEXT_SPACE_REPLACER(' '.join(results)).strip()
 
     def _get_fulltext_cache_txt(self, item, path, fh):
-        yield Info('debug', f'Retrieving text content for "{path}" of "{item.id}"')
+        yield Info('debug', f'Retrieving text content for {path!r} of {item.id!r}')
         charset = util.sniff_bom(fh) or util.fix_codec(item.meta.get('charset', '')) or 'UTF-8'
         text = fh.read().decode(charset, errors='replace')
         return self.FULLTEXT_SPACE_REPLACER(text).strip()
 
 
-def generate(root, book_ids=None, item_ids=None, *,
-             config=None, no_lock=False, no_backup=False,
-             fulltext=True, inclusive_frames=True, recreate=False,
-             static_site=False, static_index=False, locale=None,
-             rss_root=None, rss_item_count=50):
+def generate(host, book_items=None, *,
+             lock=True, backup=True,
+             fulltext=True, recreate=False,
+             static_site=False, static_index=None,
+             rss=None):
     start = time.time()
 
-    host = Host(root, config)
-
-    if not no_backup:
-        host.init_backup(note='cache')
-        yield Info('info', f'Prepared backup at "{host.get_subpath(host._backup_dir)}".')
+    if isinstance(host, Host):
+        pass
+    elif isinstance(host, str):
+        host = Host(host)
+    else:
+        host = Host(*host)
+
+    if backup:
+        host.init_auto_backup(note='cache')
+        yield Info('info', f'Prepared backup at {host.get_subpath(host._auto_backup_dir)!r}.')
+        yield Info('info', '----------------------------------------------------------------------')
 
     try:
-        # cache all books if none specified
-        for book_id in book_ids or host.books:
+        first = True
+        for book_id, item_ids in (book_items or dict.fromkeys(host.books)).items():
+            if first:
+                first = False
+            else:
+                yield Info('info', '----------------------------------------------------------------------')
+
             try:
                 book = host.books[book_id]
             except KeyError:
                 # skip invalid book ID
-                yield Info('warn', f'Skipped invalid book "{book_id}".')
+                yield Info('warn', f'Skipped invalid book {book_id!r}.')
                 continue
 
-            yield Info('debug', f'Loading book "{book_id}".')
-            try:
-                if book.no_tree:
-                    yield Info('info', f'Skipped book "{book_id}" ("{book.name}") (no_tree).')
-                    continue
-
-                yield Info('info', f'Caching book "{book_id}" ({book.name}).')
-                lh = nullcontext() if no_lock else book.get_tree_lock().acquire()
-                with lh:
-                    if fulltext:
-                        generator = FulltextCacheGenerator(
-                            book,
-                            inclusive_frames=inclusive_frames,
-                            recreate=recreate,
-                        )
-                        yield from generator.run(item_ids)
-
-                    if static_site:
-                        generator = StaticSiteGenerator(
-                            book,
-                            static_index=static_index,
-                            locale=locale, rss=bool(rss_root),
-                        )
-                        yield from generator.run()
-
-                    if rss_root:
-                        generator = RssFeedGenerator(
-                            book,
-                            rss_root=rss_root,
-                            item_count=rss_item_count,
-                        )
-                        yield from generator.run()
-
-            except Exception as exc:
-                traceback.print_exc()
-                yield Info('critical', str(exc), exc=exc)
-            else:
-                yield Info('info', 'Done.')
+            if book.no_tree:
+                yield Info('info', f'Skipped book {book_id!r} ({book.name!r}) (no_tree).')
+                continue
 
-            yield Info('info', '----------------------------------------------------------------------')
+            yield Info('info', f'Caching book {book_id!r} ({book.name!r}).')
+            lh = book.get_tree_lock().acquire() if lock else nullcontext()
+            with lh:
+                if fulltext:
+                    generator = FulltextCacheGenerator(
+                        book,
+                        recreate=recreate,
+                    )
+                    yield from generator.run(item_ids)
+
+                if static_site:
+                    generator = StaticSiteGenerator(
+                        book,
+                        static_index=static_index,
+                    )
+                    yield from generator.run()
+
+                _rss = static_site if rss is None else rss
+
+                if _rss:
+                    if not book.config['rss_root']:
+                        yield Info('debug', 'Skipped RSS generating: RSS root not configured')
+                        continue
+
+                    generator = RssFeedGenerator(
+                        book,
+                    )
+                    yield from generator.run()
+
+            yield Info('info', 'Done.')
+    except Exception as exc:
+        traceback.print_exc()
+        yield Info('critical', str(exc), exc=exc)
+        return
     finally:
-        if not no_backup:
-            host.init_backup(False)
+        if backup:
+            host.init_auto_backup(False)
+
+    yield Info('info', '----------------------------------------------------------------------')
 
     elapsed = time.time() - start
     yield Info('info', f'Time spent: {elapsed} seconds.')
```

### Comparing `webscrapbook-1.9.0/webscrapbook/scrapbook/check.py` & `webscrapbook-2.0.0b8/webscrapbook/scrapbook/check.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Generator of integrity check for scrapbook data.
 """
 import copy
 import os
 import time
 import traceback
-import zipfile
 from contextlib import nullcontext
 from datetime import datetime
 from urllib.parse import unquote, urlsplit
 
 from .. import WSB_DIR, util
+from .._polyfill import zipfile
 from ..util import Info
 from .book import Book, TreeFileError
 from .host import Host
 from .indexer import (
+    SUPPORT_FOLDER_SUFFIXES,
     FavIconCacher,
     Indexer,
     generate_item_create,
     generate_item_modify,
 )
 
 # threshold (in seconds) to report file mtime newer than item modify property
@@ -111,49 +112,49 @@
 
     def _load_tree(self):
         try:
             self.book.load_meta_files()
         except TreeFileError as exc:
             raise RuntimeError(
                 f'Malformed meta file '
-                f'"{self.book.get_subpath(exc.filename)}": {exc}'
+                f'{self.book.get_subpath(exc.filename)!r}: {exc}'
             ) from exc
         except OSError as exc:
             raise RuntimeError(
                 f'Failed to load meta file '
-                f'"{self.book.get_subpath(exc.filename)}": {exc.strerror}'
+                f'{self.book.get_subpath(exc.filename)!r}: {exc.strerror}'
             ) from exc
 
         try:
             self.book.load_toc_files()
         except TreeFileError as exc:
             raise RuntimeError(
                 f'Malformed TOC file '
-                f'"{self.book.get_subpath(exc.filename)}": {exc}'
+                f'{self.book.get_subpath(exc.filename)!r}: {exc}'
             ) from exc
         except OSError as exc:
-            raise RuntimeError(f'Failed to load TOC file "{self.book.get_subpath(exc.filename)}": {exc.strerror}') from exc
+            raise RuntimeError(f'Failed to load TOC file {self.book.get_subpath(exc.filename)!r}: {exc.strerror}') from exc
 
     def _check_meta(self):
         items_invalid_id = {}
         items_missing_index = {}
         items_missing_index_file = {}
         items_missing_date = {}
         items_older_mtime = {}
         items_absolute_icon = {}
 
         for id, meta in self.book.meta.items():
             if meta is None:
                 continue
 
-            yield Info('debug', f'Checking item meta for "{id}"')
+            yield Info('debug', f'Checking item meta for {id!r}')
 
             # id
             if id in Book.SPECIAL_ITEM_ID:
-                yield Info('error', f'"{id}": invalid ID (special item)')
+                yield Info('error', f'{id!r}: invalid ID (special item)')
                 self.cnt_errors += 1
                 items_invalid_id[id] = True
 
             # type
             type = meta.get('type', '')
 
             # index
@@ -161,72 +162,72 @@
             index_file = None
             if index:
                 file = os.path.join(self.book.data_dir, index)
                 if os.path.isfile(file):
                     index_file = file
                     yield from self._check_index_file(id, index, file)
                 else:
-                    yield Info('error', f'"{id}": missing index file "{self.book.get_subpath(file)}"')
+                    yield Info('error', f'{id!r}: missing index file {self.book.get_subpath(file)!r}')
                     self.cnt_errors += 1
                     items_missing_index_file[id] = True
 
                 if type in {'folder', 'separator'}:
-                    yield Info('warn', f'"{id}": a {type} item should not have an index file.')
+                    yield Info('warn', f'{id!r}: a {type!r} item should not have an index file.')
                     self.cnt_warns += 1
                 elif type == 'bookmark' and not index.lower().endswith('.htm'):
-                    yield Info('warn', f'"{id}": a bookmark item should use "*.htm" as index file.')
+                    yield Info('warn', f"{id!r}: a bookmark item should use '*.htm' as index file.")
                     self.cnt_warns += 1
             else:
                 if type not in Book.ITEM_TYPES_WITH_OPTIONAL_INDEX:
-                    yield Info('error', f'"{id}": missing "index" property.')
+                    yield Info('error', f"{id!r}: missing 'index' property.")
                     self.cnt_errors += 1
                     items_missing_index[id] = True
 
             # icon
             icon = meta.get('icon')
             if icon:
                 icon_parts = urlsplit(icon)
                 if icon_parts.scheme:
-                    yield Info('warn', f'"{id}": icon "{util.crop(icon, 256)}" is an absolute URL')
+                    yield Info('warn', f'{id!r}: icon {util.crop(icon, 256)!r} is an absolute URL')
                     self.cnt_warns += 1
                     items_absolute_icon[id] = True
                 elif icon_parts.netloc:
-                    yield Info('error', f'"{id}": icon "{util.crop(icon, 256)}" is a protocol-relative URL')
+                    yield Info('error', f'{id!r}: icon {util.crop(icon, 256)!r} is a protocol-relative URL')
                     self.cnt_errors += 1
                 elif icon_parts.path.startswith('/'):
-                    yield Info('error', f'"{id}": icon "{util.crop(icon, 256)}" is a root-relative URL')
+                    yield Info('error', f'{id!r}: icon {util.crop(icon, 256)!r} is a root-relative URL')
                     self.cnt_errors += 1
                 else:
                     yield from self._check_favicon_file(id, meta)
 
             # create
             create = meta.get('create')
             if not create:
-                yield Info('error', f'"{id}": missing "create" property.')
+                yield Info('error', f"{id!r}: missing 'create' property.")
                 self.cnt_errors += 1
                 items_missing_date[id] = True
 
             # modify
             modify = meta.get('modify')
             if not modify:
-                yield Info('error', f'"{id}": missing "modify" property.')
+                yield Info('error', f"{id!r}: missing 'modify' property.")
                 self.cnt_errors += 1
                 items_missing_date[id] = True
             elif index_file:
                 try:
                     ts = os.stat(index_file).st_mtime
                 except OSError:
                     pass
                 else:
                     dt = datetime.fromtimestamp(ts - OLDER_MTIME_THRESHOLD)
                     mtime_check = util.datetime_to_id(dt)
                     if mtime_check > modify:
                         dt = datetime.fromtimestamp(ts)
                         mtime = util.datetime_to_id(dt)
-                        yield Info('warn', f'"{id}": "modify" property ({modify}) is older than last modified time of index file ({mtime}).')
+                        yield Info('warn', f"{id!r}: 'modify' property ({modify}) is older than last modified time of index file ({mtime}).")
                         self.cnt_warns += 1
                         items_older_mtime[id] = True
 
         self.cnt_items += len(self.book.meta)
 
         if items_invalid_id and self.resolve_invalid_id:
             yield from self._resolve_invalid_id(items_invalid_id)
@@ -245,61 +246,58 @@
 
         if items_absolute_icon and self.resolve_absolute_icon:
             yield from self._resolve_absolute_icon(items_absolute_icon)
 
     def _check_index_file(self, id, index, file):
         pf = self._get_index_path_key(file)
         if pf in self.find_index_exclude:
-            yield Info('warn', f'"{id}": index file "{self.book.get_subpath(file)}" is used by another item.')
+            yield Info('warn', f'{id!r}: index file {self.book.get_subpath(file)!r} is used by another item.')
             self.cnt_warns += 1
         else:
-            yield Info('debug', f'Excluding "{pf}" from index finding')
+            yield Info('debug', f'Excluding {pf!r} from index finding')
             self.find_index_exclude.add(pf)
 
             if index.endswith('/index.html'):
                 pd = self._get_index_path_key(os.path.dirname(file))
-                yield Info('debug', f'Excluding "{pd}" from index finding')
+                yield Info('debug', f'Excluding {pd!r} from index finding')
                 self.find_index_exclude.add(pd)
             elif util.is_html(index):
                 basename, ext = os.path.splitext(index)
-                p = self._get_index_path_key(os.path.join(os.path.dirname(file), f'{basename}.files'))
-                yield Info('debug', f'Excluding "{p}" from index finding')
-                self.find_index_exclude.add(p)
-
-                p = self._get_index_path_key(os.path.join(os.path.dirname(file), f'{basename}_files'))
-                yield Info('debug', f'Excluding "{p}" from index finding')
-                self.find_index_exclude.add(p)
+                for suffix in SUPPORT_FOLDER_SUFFIXES:
+                    p = self._get_index_path_key(os.path.join(os.path.dirname(file), f'{basename}{suffix}'))
+                    yield Info('debug', f'Excluding {p!r} from index finding')
+                    self.find_index_exclude.add(p)
             elif util.is_archive(index):
                 try:
                     zh = zipfile.ZipFile(file)
                 except zipfile.BadZipFile:
-                    yield Info('error', f'"{id}": corrupted archive file "{self.book.get_subpath(file)}"')
+                    yield Info('error', f'{id!r}: corrupted archive file {self.book.get_subpath(file)!r}')
                     self.cnt_errors += 1
                     return
 
                 with zh as zh:
                     if util.is_htz(index):
                         try:
                             zh.getinfo('index.html')
                         except KeyError:
-                            yield Info('error', f'"{id}": missing "index.html" in archive file "{self.book.get_subpath(file)}"')
+                            yield Info('error', f"{id!r}: missing 'index.html' in archive file {self.book.get_subpath(file)!r}")
                             self.cnt_errors += 1
                     else:
                         if not util.get_maff_pages(zh):
-                            yield Info('error', f'"{id}": no valid page in archive file "{self.book.get_subpath(file)}"')
+                            yield Info('error', f'{id!r}: no valid page in archive file {self.book.get_subpath(file)!r}')
                             self.cnt_errors += 1
 
     def _check_favicon_file(self, id, meta):
         favicon_dir = os.path.join(self.book.tree_dir, 'favicon', '')
         file = self.book.get_icon_file(meta)
         file_ci = os.path.normcase(file)
         is_in_favicon_dir = file_ci.startswith(os.path.normcase(favicon_dir))
 
         if not os.path.isfile(file):
-            yield Info('error', f'"{id}": missing icon file "{self.book.get_subpath(file)}"')
+            yield Info('error', f'{id!r}: missing icon file {self.book.get_subpath(file)!r}')
             self.cnt_errors += 1
             return
 
         if is_in_favicon_dir:
             self.used_favicons.add(file_ci)
 
     def _check_toc(self):
@@ -307,44 +305,44 @@
         items_missing_meta = {}
         ref_items_invalid = {}
 
         for id, ref_ids in self.book.toc.items():
             if ref_ids is None:
                 continue
 
-            yield Info('debug', f'Checking item TOC for "{id}"')
+            yield Info('debug', f'Checking item TOC for {id!r}')
 
             # missing meta
             if not self.book.meta.get(id) and id not in Book.SPECIAL_ITEM_ID:
-                yield Info('error', f'"{id}": invalid ID (missing metadata entry)')
+                yield Info('error', f'{id!r}: invalid ID (missing metadata entry)')
                 self.cnt_errors += 1
                 items_missing_meta[id] = True
 
             # check referenced IDs
             for ref_id in ref_ids:
                 self.seen_in_toc.add(ref_id)
 
                 # special item ID is invalid
                 if ref_id in Book.SPECIAL_ITEM_ID:
-                    yield Info('error', f'"{id}": invalid reference ID "{ref_id}" (special item)')
+                    yield Info('error', f'{id!r}: invalid reference ID {ref_id!r} (special item)')
                     self.cnt_errors += 1
                     ref_items_invalid.setdefault(id, {})[ref_id] = True
                     continue
 
                 # missing meta
                 if not self.book.meta.get(ref_id):
-                    yield Info('error', f'"{id}": invalid reference ID "{ref_id}" (missing metadata entry)')
+                    yield Info('error', f'{id!r}: invalid reference ID {ref_id!r} (missing metadata entry)')
                     self.cnt_errors += 1
                     ref_items_invalid.setdefault(id, {})[ref_id] = True
                     continue
 
         # items not reachable from TOC
         for id in self.book.meta:
             if id not in self.seen_in_toc and id not in Book.SPECIAL_ITEM_ID:
-                yield Info('error', f'"{id}": not recheable from TOC.')
+                yield Info('error', f'{id!r}: not recheable from TOC.')
                 self.cnt_errors += 1
                 items_unreachable[id] = True
 
         if (items_missing_meta or ref_items_invalid) and self.resolve_toc_invalid:
             yield from self._resolve_toc_invalid(items_missing_meta, ref_items_invalid)
 
         if items_unreachable and self.resolve_toc_unreachable:
@@ -352,127 +350,132 @@
 
     def _check_toc_empty_subtree(self):
         # Calculate this after other TOC related issues are resolved,
         # as they might produce more empty lists.
         yield Info('debug', 'Checking empty lists in TOC...')
 
         items_empty_toc = {}
-
         for id, ref_ids in self.book.toc.items():
-            if ref_ids is None:
-                continue
-
-            if not ref_ids and id != 'root':
-                yield Info('warn', f'"{id}": TOC list is empty')
+            if not ref_ids:
+                yield Info('warn', f'{id!r}: TOC list is empty')
                 self.cnt_warns += 1
                 items_empty_toc[id] = True
 
         if items_empty_toc and self.resolve_toc_empty_subtree:
             yield from self._resolve_toc_empty_subtree(items_empty_toc)
 
     def _check_data_dir(self):
         unindexed_files = {}
         yield from self._check_data_dir_internal(self.book.data_dir, unindexed_files, find_index=True)
 
         if unindexed_files and self.resolve_unindexed_files:
             yield from self._resolve_unindexed_files(unindexed_files)
 
     def _check_data_dir_internal(self, data_dir, unindexed_files, find_index=True):
-        yield Info('debug', f'Inspecting folder "{self.book.get_subpath(data_dir)}" (find_index={find_index})')
+        yield Info('debug', f'Inspecting folder {self.book.get_subpath(data_dir)!r} (find_index={find_index!r})')
 
         if find_index:
             index = os.path.join(data_dir, 'index.html')
             if self._get_index_path_key(index) not in self.find_index_exclude and os.path.isfile(index):
-                yield Info('warn', f'File "{self.book.get_subpath(index)}" not used as item index')
+                yield Info('warn', f'File {self.book.get_subpath(index)!r} not used as item index')
                 self.cnt_warns += 1
                 unindexed_files[index] = True
 
-                yield Info('debug', f'Excluding "{self.book.get_subpath(data_dir)}" from index finding')
+                yield Info('debug', f'Excluding {self.book.get_subpath(data_dir)!r} from index finding')
                 find_index = False
 
         try:
             entries = os.scandir(data_dir)
         except FileNotFoundError:
             return
         except OSError as exc:
-            yield Info('error', f'Failed to scan folder "{self.book.get_subpath(exc.filename)}": {exc.strerror}', exc=exc)
+            yield Info('error', f'Failed to scan folder {self.book.get_subpath(exc.filename)!r}: {exc.strerror}', exc=exc)
             self.cnt_errors += 1
             return
 
-        subdirs = {}
+        entries_to_handle = set()
         with entries as entries:
             for entry in entries:
                 try:
                     assert not os.path.samefile(entry, self.wsb_dir)
                 except AssertionError:
-                    yield Info('debug', f'Skipped special "{self.book.get_subpath(entry)}"')
+                    yield Info('debug', f'Skipped special {self.book.get_subpath(entry)!r}')
                     continue
                 except OSError:
                     pass
 
                 try:
                     assert not os.path.samefile(entry, self.book_wsb_dir)
                 except AssertionError:
-                    yield Info('debug', f'Skipped special "{self.book.get_subpath(entry)}"')
+                    yield Info('debug', f'Skipped special {self.book.get_subpath(entry)!r}')
                     continue
                 except OSError:
                     pass
 
                 if entry.is_dir():
                     self.cnt_dirs += 1
-                    subdirs.setdefault(entry, True)
+                    entries_to_handle.add(entry)
 
                 elif entry.is_file():
                     try:
                         self.cnt_bytes += entry.stat().st_size
                     except OSError as exc:
                         # e.g. a broken symlink can cause this
-                        yield Info('error', f'Failed to access file "{self.book.get_subpath(exc.filename)}": {exc.strerror}', exc=exc)
+                        yield Info('error', f'Failed to access file {self.book.get_subpath(exc.filename)!r}: {exc.strerror}', exc=exc)
                         self.cnt_errors += 1
                     else:
                         self.cnt_files += 1
 
-                    if find_index and entry.is_file():
-                        if self._get_index_path_key(entry) not in self.find_index_exclude:
-                            basename, ext = os.path.splitext(entry.name.lower())
-                            if ext in self.book.ITEM_INDEX_ALLOWED_EXT:
-                                yield Info('warn', f'File "{self.book.get_subpath(entry)}" not used as item index')
-                                self.cnt_warns += 1
-                                unindexed_files[entry.path] = True
-
-                                if util.is_html(entry.path):
-                                    p = self._get_index_path_key(os.path.join(data_dir, f'{basename}.files'))
-                                    yield Info('debug', f'Excluding "{p}" from index finding')
-                                    self.find_index_exclude.add(p)
-
-                                    p = self._get_index_path_key(os.path.join(data_dir, f'{basename}_files'))
-                                    yield Info('debug', f'Excluding "{p}" from index finding')
-                                    self.find_index_exclude.add(p)
-
-        for entry in subdirs:
-            p = self._get_index_path_key(entry)
-            chk = find_index and p not in self.find_index_exclude
-            yield from self._check_data_dir_internal(entry, unindexed_files, find_index=chk)
+                    if not find_index:
+                        continue
+
+                    if self._get_index_path_key(entry) in self.find_index_exclude:
+                        continue
+
+                    basename, ext = os.path.splitext(entry.name)
+                    if ext.lower() not in self.book.ITEM_INDEX_ALLOWED_EXT:
+                        continue
+
+                    entries_to_handle.add(entry)
+
+                    if not util.is_html(entry.path):
+                        continue
+
+                    for suffix in SUPPORT_FOLDER_SUFFIXES:
+                        p = self._get_index_path_key(os.path.join(data_dir, f'{basename}{suffix}'))
+                        yield Info('debug', f'Excluding {p!r} from index finding')
+                        self.find_index_exclude.add(p)
+
+        for entry in sorted(entries_to_handle, key=lambda x: x.path):
+            if entry.is_dir():
+                p = self._get_index_path_key(entry)
+                chk = find_index and p not in self.find_index_exclude
+                yield from self._check_data_dir_internal(entry, unindexed_files, find_index=chk)
+
+            elif entry.is_file():
+                yield Info('warn', f'File {self.book.get_subpath(entry)!r} not used as item index')
+                self.cnt_warns += 1
+                unindexed_files[entry.path] = True
 
     def _check_favicon_cache(self):
         unused_icons = {}
 
         try:
             entries = os.scandir(os.path.join(self.book.tree_dir, 'favicon'))
         except FileNotFoundError:
             return
         except OSError as exc:
-            yield Info('error', f'Failed to scan folder "{self.book.get_subpath(exc.filename)}": {exc.strerror}', exc=exc)
+            yield Info('error', f'Failed to scan folder {self.book.get_subpath(exc.filename)!r}: {exc.strerror}', exc=exc)
             self.cnt_errors += 1
             return
 
         with entries as entries:
             for entry in entries:
                 if os.path.normcase(entry.path) not in self.used_favicons:
-                    yield Info('warn', f'Unused favicon file "{self.book.get_subpath(entry)}".')
+                    yield Info('warn', f'Unused favicon file {self.book.get_subpath(entry)!r}.')
                     self.cnt_warns += 1
                     unused_icons[entry.path] = True
 
         if unused_icons and self.resolve_unused_icon:
             yield from self._resolve_unused_icon(unused_icons)
 
     def _get_index_path_key(self, path):
@@ -482,59 +485,59 @@
         yield Info('info', 'Removing items with invalid ID...')
         for id in ids:
             try:
                 del self.book.meta[id]
             except KeyError:
                 pass
             else:
-                yield Info('info', f'Removed "{id}" from meta.')
+                yield Info('info', f'Removed {id!r} from meta.')
                 self.cnt_resolves += 1
 
     def _resolve_missing_index(self, ids):
         yield Info('info', 'Removing items missing index property...')
         for id in ids:
             try:
                 del self.book.meta[id]
             except KeyError:
                 pass
             else:
-                yield Info('info', f'Removed "{id}" from meta.')
+                yield Info('info', f'Removed {id!r} from meta.')
                 self.cnt_resolves += 1
 
     def _resolve_missing_index_file(self, ids):
         yield Info('info', 'Removing items missing index file...')
         for id in ids:
             try:
                 del self.book.meta[id]
             except KeyError:
                 pass
             else:
-                yield Info('info', f'Removed "{id}" from meta.')
+                yield Info('info', f'Removed {id!r} from meta.')
                 self.cnt_resolves += 1
 
     def _resolve_missing_date(self, ids):
         yield Info('info', 'Generating missing create/modify item property...')
         for id in ids:
             try:
                 item = self.book.meta[id]
             except KeyError:
                 continue
 
             if not item.get('create'):
                 create = generate_item_create(self.book, id)
                 if create:
                     item['create'] = create
-                    yield Info('info', f'Added "create" property for "{id}".')
+                    yield Info('info', f"Added 'create' property for {id!r}.")
                     self.cnt_resolves += 1
 
             if not item.get('modify'):
                 modify = generate_item_modify(self.book, id)
                 if modify:
                     item['modify'] = modify
-                    yield Info('info', f'Added "modify" property for "{id}".')
+                    yield Info('info', f"Added 'modify' property for {id!r}.")
                     self.cnt_resolves += 1
 
     def _resolve_older_mtime(self, ids):
         yield Info('info', 'Updating items with older modify property...')
         for id in ids:
             index = self.book.meta[id].get('index')
             if index:
@@ -544,79 +547,82 @@
                 except OSError:
                     pass
                 else:
                     dt = datetime.fromtimestamp(ts)
                     mtime = util.datetime_to_id(dt)
                     if mtime > self.book.meta[id].get('modify'):
                         self.book.meta[id]['modify'] = mtime
-                        yield Info('info', f'Updated "modify" property for "{id}".')
+                        yield Info('info', f"Updated 'modify' property for {id!r}.")
                         self.cnt_resolves += 1
 
     def _resolve_toc_invalid(self, items_missing_meta, ref_items_invalid):
         yield Info('info', 'Removing invalid items from TOC...')
 
         for id in items_missing_meta:
             try:
                 del self.book.toc[id]
             except KeyError:
                 pass
             else:
-                yield Info('info', f'Removed "{id}" from TOC.')
+                yield Info('info', f'Removed {id!r} from TOC.')
                 self.cnt_resolves += 1
 
         for id, ref_ids in ref_items_invalid.items():
             for ref_id in ref_ids:
                 try:
                     self.book.toc[id].remove(ref_id)
                 except (KeyError, ValueError):
                     pass
                 else:
-                    yield Info('info', f'Removed "{ref_id}" from the subtree of "{id}".')
+                    yield Info('info', f'Removed {ref_id!r} from the subtree of {id!r}.')
                     self.cnt_resolves += 1
 
     def _resolve_toc_unreachable(self, ids):
         yield Info('info', 'Adding unreachable items to root TOC...')
-        self.book.toc.setdefault('root', [])
+        toc = self.book.toc.setdefault(self.book.ROOT_ITEM_ID, [])
         for id in ids:
-            self.book.toc['root'].append(id)
-            yield Info('info', f'Added "{id}" to root TOC.')
+            toc.append(id)
+            yield Info('info', f'Added {id!r} to root TOC.')
             self.cnt_resolves += 1
 
     def _resolve_toc_empty_subtree(self, ids):
         yield Info('info', 'Removing empty item lists from TOC...')
         for id in ids:
             try:
                 del self.book.toc[id]
             except KeyError:
                 pass
             else:
-                yield Info('info', f'Removed "{id}" from TOC.')
+                yield Info('info', f'Removed {id!r} from TOC.')
                 self.cnt_resolves += 1
 
     def _resolve_unindexed_files(self, files):
         yield Info('info', 'Indexing unindexed files...')
         indexer = Indexer(self.book)
         indexed = yield from indexer.run(files)
 
         favicon_dir = os.path.join(self.book.tree_dir, 'favicon', '')
 
         for id in indexed:
             # add to TOC if not seen
             if id not in self.seen_in_toc:
-                self.book.toc.setdefault('root', []).append(id)
+                root = self.book.ROOT_ITEM_ID
+                target_index = 0 if self.book.config['new_at_top'] else len(self.book.toc.get(root, ()))
+                self.book.toc.setdefault(root, []).insert(target_index, id)
                 self.seen_in_toc.add(id)
 
             # record added cached favicons
             index = self.book.meta[id].get('index')
             icon = self.book.meta[id].get('icon')
-            file = os.path.normpath(os.path.join(self.book.data_dir, os.path.dirname(index), unquote(icon)))
-            file_ci = os.path.normcase(file)
-            is_in_favicon_dir = file_ci.startswith(os.path.normcase(favicon_dir))
-            if is_in_favicon_dir:
-                self.used_favicons.add(file_ci)
+            if icon:
+                file = os.path.normpath(os.path.join(self.book.data_dir, os.path.dirname(index), unquote(icon)))
+                file_ci = os.path.normcase(file)
+                is_in_favicon_dir = file_ci.startswith(os.path.normcase(favicon_dir))
+                if is_in_favicon_dir:
+                    self.used_favicons.add(file_ci)
 
             self.cnt_resolves += 1
 
     def _resolve_absolute_icon(self, ids):
         yield Info('info', 'Caching favicons with absolute URL...')
         generator = FavIconCacher(self.book)
         cached = yield from generator.run(ids)
@@ -630,54 +636,67 @@
         for file in files:
             try:
                 self.book.backup(file)
                 os.remove(file)
             except FileNotFoundError:
                 pass
             else:
-                yield Info('info', f'Removed "{self.book.get_subpath(file)}".')
+                yield Info('info', f'Removed {self.book.get_subpath(file)!r}.')
                 self.cnt_resolves += 1
 
 
-def run(root, book_ids=None, *, config=None, no_lock=False, no_backup=False, **kwargs):
+def run(host, book_ids=None, *, lock=True, backup=True, **kwargs):
     start = time.time()
 
-    host = Host(root, config)
-
-    if not no_backup:
-        host.init_backup(note='check')
-        yield Info('info', f'Prepared backup at "{host.get_subpath(host._backup_dir)}".')
+    if isinstance(host, Host):
+        pass
+    elif isinstance(host, str):
+        host = Host(host)
+    else:
+        host = Host(*host)
+
+    if backup:
+        host.init_auto_backup(note='check')
+        yield Info('info', f'Prepared backup at {host.get_subpath(host._auto_backup_dir)!r}.')
+        yield Info('info', '----------------------------------------------------------------------')
 
     try:
         # handle all books if none specified
+        first = True
         for book_id in book_ids or host.books:
+            if first:
+                first = False
+            else:
+                yield Info('info', '----------------------------------------------------------------------')
+
             try:
                 book = host.books[book_id]
             except KeyError:
                 # skip invalid book ID
-                yield Info('warn', f'Skipped invalid book "{book_id}".')
+                yield Info('warn', f'Skipped invalid book {book_id!r}.')
                 continue
 
-            yield Info('debug', f'Loading book "{book_id}"...')
-            try:
-                if book.no_tree:
-                    yield Info('info', f'Skipped book "{book_id}" ({book.name}) (no_tree).')
-                    continue
+            yield Info('debug', f'Loading book {book_id!r}...')
 
-                yield Info('info', f'Checking book "{book_id}" ({book.name}).')
-                lh = nullcontext() if no_lock else book.get_tree_lock().acquire()
-                with lh:
-                    generator = BookChecker(book, **kwargs)
-                    yield from generator.run()
-            except Exception as exc:
-                traceback.print_exc()
-                yield Info('critical', str(exc), exc=exc)
-            else:
-                yield Info('info', 'Done.')
+            if book.no_tree:
+                yield Info('info', f'Skipped book {book_id!r} ({book.name}) (no_tree).')
+                continue
 
-            yield Info('info', '----------------------------------------------------------------------')
+            yield Info('info', f'Checking book {book_id!r} ({book.name}).')
+            lh = book.get_tree_lock().acquire() if lock else nullcontext()
+            with lh:
+                generator = BookChecker(book, **kwargs)
+                yield from generator.run()
+
+            yield Info('info', 'Done.')
+    except Exception as exc:
+        traceback.print_exc()
+        yield Info('critical', str(exc), exc=exc)
+        return
     finally:
-        if not no_backup:
-            host.init_backup(False)
+        if backup:
+            host.init_auto_backup(False)
+
+    yield Info('info', '----------------------------------------------------------------------')
 
     elapsed = time.time() - start
     yield Info('info', f'Time spent: {elapsed} seconds.')
```

### Comparing `webscrapbook-1.9.0/webscrapbook/scrapbook/convert/file2wsb.py` & `webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/file2wsb.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import os
 import shutil
 import time
 import traceback
-from datetime import datetime, timedelta, timezone
 from urllib.parse import quote
 
 from ... import WSB_DIR, util
 from ...util import Info
 from ..host import Host
-from ..indexer import Indexer
-
-DEFAULT_DATA_FOLDER_SUFFIXES = ['.files', '_files']
+from ..indexer import SUPPORT_FOLDER_SUFFIXES, Indexer
 
 
 class Converter:
     def __init__(self, input, output, *,
                  data_folder_suffixes=None,
                  preserve_filename=True,
                  handle_ie_meta=True,
@@ -22,15 +19,15 @@
                  handle_savepagewe_meta=True,
                  handle_maoxian_meta=True,
                  ):
         self.input = os.path.abspath(input)
         self.output = os.path.abspath(output)
         self.data_folder_suffixes = (
             [k for k in dict.fromkeys(os.path.normcase(s.strip()) for s in data_folder_suffixes) if k]
-            if data_folder_suffixes is not None else DEFAULT_DATA_FOLDER_SUFFIXES)
+            if data_folder_suffixes is not None else SUPPORT_FOLDER_SUFFIXES)
         self.preserve_filename = preserve_filename
         self.handle_ie_meta = handle_ie_meta
         self.handle_singlefile_meta = handle_singlefile_meta
         self.handle_savepagewe_meta = handle_savepagewe_meta
         self.handle_maoxian_meta = handle_maoxian_meta
         self.wsb_dir = os.path.join(self.input, WSB_DIR)
         self.host = None
@@ -48,77 +45,72 @@
         yield from self._inspect_data_dir(self.input, paths)
 
         yield Info('info', 'Saving tree files...')
         self.book.save_meta_files()
         self.book.save_toc_files()
 
     def _inspect_data_dir(self, data_dir, paths):
-        yield Info('debug', f'Inspecting directory "{data_dir}"')
+        yield Info('debug', f'Inspecting directory {data_dir!r}')
 
         if not os.path.samefile(data_dir, self.input):
             # add data_dir as an item if index.html exists
             index = os.path.join(data_dir, 'index.html')
             if os.path.isfile(index):
                 yield from self._index_entry(data_dir, paths)
                 return
 
             # create folder item
             basename = os.path.basename(data_dir)
             basename, ext = os.path.splitext(basename)
             if ext.lower() == '.htd':
                 ext = ''
 
-            id = self._generate_unique_id()
-            meta = self.book.DEFAULT_META.copy()
-            meta.update({
+            parent_id = paths[-1]
+            new_items = self.book.add_item({
                 'type': 'folder',
                 'title': basename + ext,
-                'create': id,
-                'modify': id,
-            })
-            for key in list(meta):
-                if meta[key] is None:
-                    del meta[key]
-            self.book.meta[id] = meta
-
-            parent_id = paths[-1]
-            self.book.toc.setdefault(parent_id, []).append(id)
-            yield Info('info', f'Generated folder item "{id}" under "{parent_id}"')
+            }, parent_id)
+            id = next(iter(new_items))
+            yield Info('info', f'Generated folder item {id!r} under {parent_id!r}')
         else:
-            id = 'root'
+            id = self.book.ROOT_ITEM_ID
 
         try:
             entries = os.scandir(data_dir)
         except FileNotFoundError:
             return
         except OSError as exc:
-            yield Info('error', f'Failed to scan folder "{self.book.get_subpath(exc.filename)}": {exc.strerror}', exc=exc)
+            yield Info('error', f'Failed to scan folder {self.book.get_subpath(exc.filename)!r}: {exc.strerror}', exc=exc)
             return
 
         entries_to_handle = set()
         entries_to_exclude = set()
         with entries as entries:
             for entry in entries:
                 if os.path.normcase(entry.path) == os.path.normcase(self.wsb_dir):
-                    yield Info('debug', f'Skipped special "{self.book.get_subpath(entry)}"')
+                    yield Info('debug', f'Skipped special {self.book.get_subpath(entry)!r}')
                     continue
 
                 if entry.is_dir():
                     entries_to_handle.add(entry)
 
                 elif entry.is_file():
-                    if self._get_index_path_key(entry) not in entries_to_exclude:
-                        entries_to_handle.add(entry)
+                    if self._get_index_path_key(entry) in entries_to_exclude:
+                        continue
 
-                        if util.is_html(entry.path):
-                            basename, _ = os.path.splitext(entry.name)
-                            for suffix in self.data_folder_suffixes:
-                                p = self._get_index_path_key(os.path.join(data_dir, f'{basename}{suffix}'))
-                                yield Info('debug', f'Excluding "{p}" from index finding')
-                                entries_to_exclude.add(p)
+                    entries_to_handle.add(entry)
+
+                    if not util.is_html(entry.path):
+                        continue
+
+                    basename, _ = os.path.splitext(entry.name)
+                    for suffix in self.data_folder_suffixes:
+                        p = self._get_index_path_key(os.path.join(data_dir, f'{basename}{suffix}'))
+                        yield Info('debug', f'Excluding {p!r} from index finding')
+                        entries_to_exclude.add(p)
 
         paths.append(id)
 
         for entry in sorted(entries_to_handle, key=lambda x: x.path):
             if self._get_index_path_key(entry) in entries_to_exclude:
                 continue
 
@@ -126,57 +118,57 @@
                 yield from self._inspect_data_dir(entry.path, paths)
             elif entry.is_file():
                 yield from self._index_entry(entry.path, paths)
 
         paths.pop()
 
     def _index_entry(self, entry, paths):
-        yield Info('debug', f'Generating item for "{entry}"...')
+        yield Info('debug', f'Generating item for {entry!r}...')
 
         basename = os.path.basename(entry)
         _, ext = os.path.splitext(entry)
         ext = ext.lower()
         if ext == '.htd':
             ext = ''
 
         # generate a unique ID
-        id = self._generate_unique_id(ext)
+        id = self.book.get_unique_id()
 
         # copy data files
         supporting_folder = self._get_supporting_folder(entry)
         if (supporting_folder or (
             self.preserve_filename and os.path.isfile(entry) and not util.is_archive(entry)
         )):
             dst_dir = os.path.join(self.book.data_dir, id)
             os.makedirs(dst_dir, exist_ok=True)
 
             src = entry
             dst = os.path.join(dst_dir, basename)
-            yield Info('info', f'Copying data file: "{src}" => "{dst}"')
+            yield Info('info', f'Copying data file: {src!r} => {dst!r}')
             try:
                 shutil.copy2(src, dst)
             except OSError as exc:
-                yield Info('error', f'Failed to copy data file "{entry}": {exc.strerror}', exc=exc)
+                yield Info('error', f'Failed to copy data file {entry!r}: {exc.strerror}', exc=exc)
 
             index_file = os.path.join(dst_dir, 'index.html')
             if ext in self.book.ITEM_INDEX_ALLOWED_EXT:
                 # copy entry to index.html for the indexer to retrieve original metadata
                 try:
                     shutil.copy2(src, index_file)
                 except OSError as exc:
-                    yield Info('error', f'Failed to copy data file "{entry}": {exc.strerror}', exc=exc)
+                    yield Info('error', f'Failed to copy data file {entry!r}: {exc.strerror}', exc=exc)
 
                 if supporting_folder:
                     src = supporting_folder
                     dst = os.path.join(dst_dir, os.path.basename(supporting_folder))
-                    yield Info('info', f'Copying data folder: "{src}" => "{dst}"')
+                    yield Info('info', f'Copying data folder: {src!r} => {dst!r}')
                     try:
                         shutil.copytree(src, dst)
                     except OSError as exc:
-                        yield Info('error', f'Failed to copy data folder "{entry}": {exc.strerror}', exc=exc)
+                        yield Info('error', f'Failed to copy data folder {entry!r}: {exc.strerror}', exc=exc)
 
                 # generate meta
                 indexer = Indexer(
                     self.book,
                     handle_ie_meta=self.handle_ie_meta,
                     handle_singlefile_meta=self.handle_singlefile_meta,
                     handle_savepagewe_meta=self.handle_savepagewe_meta,
@@ -203,22 +195,22 @@
                     handle_maoxian_meta=self.handle_maoxian_meta,
                 )
                 indexed = yield from indexer.run([index_file])
 
         else:
             src = entry
             dst = os.path.join(self.book.data_dir, id + ext)
-            yield Info('info', f'Copying data files: "{src}" => "{dst}"')
+            yield Info('info', f'Copying data files: {src!r} => {dst!r}')
             try:
                 try:
                     shutil.copytree(src, dst)
                 except NotADirectoryError:
                     shutil.copy2(src, dst)
             except OSError as exc:
-                yield Info('error', f'Failed to copy data files for "{entry}": {exc.strerror}', exc=exc)
+                yield Info('error', f'Failed to copy data files for {entry!r}: {exc.strerror}', exc=exc)
 
             index_file = os.path.join(dst, 'index.html') if os.path.isdir(entry) else dst
 
             # generate meta
             indexer = Indexer(
                 self.book,
                 handle_ie_meta=self.handle_ie_meta,
@@ -236,15 +228,15 @@
 
             if os.path.isfile(entry) and ext not in self.book.ITEM_INDEX_ALLOWED_EXT:
                 meta['type'] = 'file'
 
             # add to parent
             parent_id = paths[-1]
             self.book.toc.setdefault(parent_id, []).append(id)
-            yield Info('info', f'Appended item "{id}" under "{parent_id}"')
+            yield Info('info', f'Appended item {id!r} under {parent_id!r}')
 
     def _get_index_path_key(self, path):
         return self.book.get_subpath(os.path.normcase(path))
 
     def _get_supporting_folder(self, file):
         if os.path.isfile(file) and util.is_html(file):
             base = os.path.splitext(file)[0]
@@ -252,55 +244,48 @@
             for suffix in self.data_folder_suffixes:
                 supporting_folder = f'{base}{suffix}'
                 if os.path.isdir(supporting_folder):
                     return supporting_folder
 
         return None
 
-    def _generate_unique_id(self, ext=''):
-        dt = datetime.now(timezone.utc)
-        id = util.datetime_to_id(dt)
-        while id in self.book.meta or os.path.lexists(os.path.join(self.book.data_dir, id + ext)):
-            dt += timedelta(milliseconds=1)
-            id = util.datetime_to_id(dt)
-        return id
-
 
 def run(input, output, *,
         data_folder_suffixes=None,
-        no_preserve_filename=False,
-        ignore_ie_meta=False,
-        ignore_singlefile_meta=False,
-        ignore_savepagewe_meta=False,
-        ignore_maoxian_meta=False,
+        preserve_filename=True,
+        handle_ie_meta=True,
+        handle_singlefile_meta=True,
+        handle_savepagewe_meta=True,
+        handle_maoxian_meta=True,
         ):
     start = time.time()
     yield Info('info', 'conversion mode: hierarchical files --> WebScrapBook')
     yield Info('info', f'input directory: {os.path.abspath(input)}')
     yield Info('info', f'output directory: {os.path.abspath(output)}')
-    yield Info('info', f'data_folder_suffixes: {DEFAULT_DATA_FOLDER_SUFFIXES if data_folder_suffixes is None else data_folder_suffixes}')
-    yield Info('info', f'no preserve filename: {no_preserve_filename}')
-    yield Info('info', f'ignore IE meta: {ignore_ie_meta}')
-    yield Info('info', f'ignore SingleFile meta: {ignore_singlefile_meta}')
-    yield Info('info', f'ignore Save Page WE meta: {ignore_savepagewe_meta}')
-    yield Info('info', f'ignore MaoXian web clipper meta: {ignore_maoxian_meta}')
+    yield Info('info', f'data_folder_suffixes: {SUPPORT_FOLDER_SUFFIXES if data_folder_suffixes is None else data_folder_suffixes}')
+    yield Info('info', f'preserve filename: {preserve_filename}')
+    yield Info('info', f'handle IE meta: {handle_ie_meta}')
+    yield Info('info', f'handle SingleFile meta: {handle_singlefile_meta}')
+    yield Info('info', f'handle Save Page WE meta: {handle_savepagewe_meta}')
+    yield Info('info', f'handle MaoXian web clipper meta: {handle_maoxian_meta}')
     yield Info('info', '')
 
     try:
         conv = Converter(
             input, output,
             data_folder_suffixes=data_folder_suffixes,
-            preserve_filename=not no_preserve_filename,
-            handle_ie_meta=not ignore_ie_meta,
-            handle_singlefile_meta=not ignore_singlefile_meta,
-            handle_savepagewe_meta=not ignore_savepagewe_meta,
-            handle_maoxian_meta=not ignore_maoxian_meta,
+            preserve_filename=preserve_filename,
+            handle_ie_meta=handle_ie_meta,
+            handle_singlefile_meta=handle_singlefile_meta,
+            handle_savepagewe_meta=handle_savepagewe_meta,
+            handle_maoxian_meta=handle_maoxian_meta,
         )
         yield from conv.run()
     except Exception as exc:
         traceback.print_exc()
         yield Info('critical', str(exc), exc=exc)
+        return
     else:
         yield Info('info', 'Done.')
 
     elapsed = time.time() - start
     yield Info('info', f'Time spent: {elapsed} seconds.')
```

### Comparing `webscrapbook-1.9.0/webscrapbook/scrapbook/convert/items.py` & `webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/items.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,75 @@
 import copy
 import html
 import os
 import shutil
 import time
 import traceback
-import zipfile
 from datetime import datetime, timezone
 from email.utils import format_datetime
 from urllib.parse import quote
 
 from ... import util
+from ..._polyfill import zipfile
 from ...util import Info
 from ..host import Host
 from ..indexer import FavIconCacher, SingleHtmlConverter, UnSingleHtmlConverter
 
 
 class Converter:
-    def __init__(self, input, output, book_ids=None, item_ids=None, types=None, format=None):
+    def __init__(self, input, output, book_items=None, types=None, format=None):
         self.input = input
         self.output = output
-        self.book_ids = book_ids
-        self.item_ids = item_ids
+        self.book_items = book_items
         self.types = set(types) if types else {}
         self.format = format
 
     def run(self):
         if self.input != self.output:
             yield Info('info', 'Copying files...')
             self._copy_files()
 
         yield Info('info', 'Applying conversion...')
         host = Host(self.output)
 
-        # handle all books if none specified
-        for book_id in self.book_ids or host.books:
+        for book_id, item_ids in (self.book_items or dict.fromkeys(host.books)).items():
             try:
                 book = host.books[book_id]
             except KeyError:
                 # skip invalid book ID
-                yield Info('warn', f'Skipped invalid book "{book_id}".')
+                yield Info('warn', f'Skipped invalid book {book_id!r}.')
                 continue
 
-            yield Info('info', f'Handling book "{book_id}"...')
+            yield Info('info', f'Handling book {book_id!r}...')
             book.load_meta_files()
 
             book_meta_orig = copy.deepcopy(book.meta)
 
-            # handle all items if none specified
-            for id in self.item_ids or book.meta:
+            for id in (item_ids or book.meta):
                 if id not in book.meta:
                     # skip invalid item ID
-                    yield Info('debug', f'Skipped invalid item "{id}".')
+                    yield Info('debug', f'Skipped invalid item {id!r}.')
                     continue
 
                 type = book.meta[id].get('type', '')
                 if type not in self.types:
-                    yield Info('debug', f'Skipped item "{id}": type="{type}"')
+                    yield Info('debug', f'Skipped item {id!r}: type={type!r}')
                     continue
 
-                yield Info('debug', f'Checking "{id}"...')
+                yield Info('debug', f'Checking {id!r}...')
 
                 if self.format:
                     try:
                         try:
                             yield from self._convert_item_format(book, id)
                         except OSError as exc:
                             raise RuntimeError(exc.strerror) from exc
                     except Exception as exc:
                         traceback.print_exc()
-                        yield Info('error', f'Failed to convert "{id}": {exc}', exc=exc)
+                        yield Info('error', f'Failed to convert {id!r}: {exc}', exc=exc)
 
             # update files
             if book.meta != book_meta_orig:
                 yield Info('info', 'Saving changed meta files...')
                 book.save_meta_files()
 
     def _copy_files(self):
@@ -85,52 +82,52 @@
                     shutil.copy2(src, dst)
 
     def _convert_item_format(self, book, id):
         meta = book.meta[id]
         index = meta.get('index')
 
         if not index:
-            yield Info('debug', f'Skipped "{id}": no index')
+            yield Info('debug', f'Skipped {id!r}: no index')
             return
 
         if index.endswith('/index.html'):
             format = 'folder'
         elif util.is_htz(index):
             format = 'htz'
         elif util.is_maff(index):
             format = 'maff'
         else:
             format = 'single_file'
 
         if format == self.format:
-            yield Info('debug', f'Skipped "{id}": same format')
+            yield Info('debug', f'Skipped {id!r}: same format')
             return
 
         if format == 'folder':
             indexbase = index[:-11]
             fsrc = os.path.normpath(os.path.join(book.data_dir, indexbase))
             indexdir = os.path.normpath(os.path.join(book.data_dir, indexbase + '.' + util.datetime_to_id()))
             shutil.copytree(fsrc, indexdir)
             yield from self._cache_favicon(book, id)
         elif format == 'htz':
             fsrc = os.path.normpath(os.path.join(book.data_dir, index))
             indexbase = index[:-4]
             indexdir = os.path.normpath(os.path.join(book.data_dir, indexbase + '.' + util.datetime_to_id()))
-            util.zip_extract(fsrc, indexdir)
+            util.fs.zip_extract(fsrc, indexdir)
         elif format == 'maff':
             fsrc = os.path.normpath(os.path.join(book.data_dir, index))
             indexbase = index[:-5]
             indexdir = os.path.normpath(os.path.join(book.data_dir, indexbase + '.' + util.datetime_to_id()))
 
             maff_info = next(iter(util.get_maff_pages(fsrc)), None)
             if not maff_info:
-                yield Info('debug', f'Skipping "{id}": no valid index page in MAFF')
+                yield Info('debug', f'Skipping {id!r}: no valid index page in MAFF')
             subpath, _, _ = maff_info.indexfilename.partition('/')
 
-            util.zip_extract(fsrc, indexdir, subpath)
+            util.fs.zip_extract(fsrc, indexdir, subpath)
 
             rdf_file = os.path.join(indexdir, 'index.rdf')
             try:
                 os.remove(rdf_file)
             except FileNotFoundError:
                 pass
         else:
@@ -157,68 +154,68 @@
                     fh.write(content)
 
             shutil.copystat(fsrc, indexfile)
 
         try:
             if self.format == 'folder':
                 fdst = os.path.normpath(os.path.join(book.data_dir, indexbase))
-                yield Info('info', f'Converting "{id}": "{book.get_subpath(fsrc)}" => "{book.get_subpath(fdst)}" ...')
+                yield Info('info', f'Converting {id!r}: {book.get_subpath(fsrc)!r} => {book.get_subpath(fdst)!r} ...')
 
                 if os.path.lexists(fdst):
-                    yield Info('error', f'Failed to convert "{id}": target "{book.get_subpath(fdst)}" already exists.')
+                    yield Info('error', f'Failed to convert {id!r}: target {book.get_subpath(fdst)!r} already exists.')
                     return
 
                 shutil.move(indexdir, fdst)
 
                 # adjust icon path to fit the new index file
                 iconfile = book.get_icon_file(meta)
                 if iconfile:
                     meta['icon'] = util.get_relative_url(iconfile, fdst, path_is_dir=False, start_is_dir=True)
 
                 meta['index'] = indexbase + '/index.html'
 
             elif self.format == 'htz':
                 fdst = os.path.normpath(os.path.join(book.data_dir, indexbase + '.htz'))
-                yield Info('info', f'Converting "{id}": "{book.get_subpath(fsrc)}" => "{book.get_subpath(fdst)}" ...')
+                yield Info('info', f'Converting {id!r}: {book.get_subpath(fsrc)!r} => {book.get_subpath(fdst)!r} ...')
 
                 if os.path.lexists(fdst):
-                    yield Info('error', f'Failed to convert "{id}": target "{book.get_subpath(fdst)}" already exists.')
+                    yield Info('error', f'Failed to convert {id!r}: target {book.get_subpath(fdst)!r} already exists.')
                     return
 
-                util.zip_compress(fdst, indexdir, '')
+                util.fs.zip_compress(fdst, indexdir, '')
                 shutil.copystat(os.path.join(indexdir, 'index.html'), fdst)
 
                 # adjust icon path to fit the new index file
                 iconfile = book.get_icon_file(meta)
                 if iconfile:
                     meta['icon'] = util.get_relative_url(iconfile, fdst, path_is_dir=False, start_is_dir=False)
 
                 meta['index'] = indexbase + '.htz'
 
             elif self.format == 'maff':
                 fdst = os.path.normpath(os.path.join(book.data_dir, indexbase + '.maff'))
-                yield Info('info', f'Converting "{id}": "{book.get_subpath(fsrc)}" => "{book.get_subpath(fdst)}" ...')
+                yield Info('info', f'Converting {id!r}: {book.get_subpath(fsrc)!r} => {book.get_subpath(fdst)!r} ...')
 
                 rdf_file = os.path.join(indexdir, 'index.rdf')
                 if os.path.lexists(rdf_file):
-                    yield Info('error', f'Failed to convert "{id}": index.rdf file already exists.')
+                    yield Info('error', f'Failed to convert {id!r}: index.rdf file already exists.')
                     return
 
                 if os.path.lexists(fdst):
-                    yield Info('error', f'Failed to convert "{id}": target "{book.get_subpath(fdst)}" already exists.')
+                    yield Info('error', f'Failed to convert {id!r}: target {book.get_subpath(fdst)!r} already exists.')
                     return
 
                 subpath = id if util.id_to_datetime(id) else util.datetime_to_id()
-                util.zip_compress(fdst, indexdir, subpath)
+                util.fs.zip_compress(fdst, indexdir, subpath)
 
                 rdf_content = self._generate_index_rdf(book, id)
                 with zipfile.ZipFile(fdst, 'a') as zh:
                     zh.writestr(
                         f'{subpath}/index.rdf', rdf_content,
-                        **util.zip_compression_params(mimetype='application/rdf+xml')
+                        **util.fs.zip_compression_params(mimetype='application/rdf+xml')
                     )
 
                 shutil.copystat(os.path.join(indexdir, 'index.html'), fdst)
 
                 # adjust icon path to fit the new index file
                 iconfile = book.get_icon_file(meta)
                 if iconfile:
@@ -240,18 +237,18 @@
                     _, ext = os.path.splitext(file)
 
                 # special handling to prevent named "index.html"
                 if indexbase == 'index' and ext == '.html':
                     indexbase = 'index_'
 
                 fdst = os.path.normpath(os.path.join(book.data_dir, indexbase + ext))
-                yield Info('info', f'Converting "{id}": "{book.get_subpath(fsrc)}" => "{book.get_subpath(fdst)}" ...')
+                yield Info('info', f'Converting {id!r}: {book.get_subpath(fsrc)!r} => {book.get_subpath(fdst)!r} ...')
 
                 if os.path.lexists(fdst):
-                    yield Info('error', f'Failed to convert "{id}": target "{book.get_subpath(fdst)}" already exists.')
+                    yield Info('error', f'Failed to convert {id!r}: target {book.get_subpath(fdst)!r} already exists.')
                     return
 
                 if util.is_html(file) or util.is_svg(file):
                     conv = SingleHtmlConverter(file)
                     content = conv.run()
                     with open(fdst, 'w', encoding=conv.encoding, newline='') as fh:
                         fh.write(content)
@@ -294,34 +291,39 @@
   <MAF:indexfilename RDF:resource="index.html"/>
   <MAF:charset RDF:resource="{html.escape(meta.get('charset') or 'UTF-8')}"/>
 </RDF:Description>
 </RDF:RDF>
 """
 
 
-def run(input, output, book_ids=None, item_ids=None, types=None, format=None):
+def run(input, output, book_items=None, types=None, format=None):
     start = time.time()
-    book_ids_text = ', '.join(f'"{id}"' for id in book_ids) if book_ids else 'all'
-    item_ids_text = ', '.join(f'"{id}"' for id in item_ids) if item_ids else 'all'
     yield Info('info', 'converting items:')
     yield Info('info', f'input directory: {os.path.abspath(input)}')
     yield Info('info', f'output directory: {os.path.abspath(output) if output is not None else "(in-place)"}')
-    yield Info('info', f'book(s): {book_ids_text}')
-    yield Info('info', f'item(s): {item_ids_text}')
+
+    if book_items:
+        for book_id, item_ids in book_items.items():
+            item_ids_text = ', '.join(f'{id!r}' for id in item_ids) if item_ids else 'all'
+            yield Info('info', f'book: {book_id!r}, item(s): {item_ids_text}')
+    else:
+        yield Info('info', 'books: all, items: all')
+
     yield Info('info', f'types: {types}')
     yield Info('info', f'format: {format}')
     yield Info('info', '')
 
     if output is None:
         output = input
 
     try:
-        conv = Converter(input, output, book_ids=book_ids, item_ids=item_ids, types=types, format=format)
+        conv = Converter(input, output, book_items=book_items, types=types, format=format)
         yield from conv.run()
     except Exception as exc:
         traceback.print_exc()
         yield Info('critical', str(exc), exc=exc)
+        return
     else:
         yield Info('info', 'Done.')
 
     elapsed = time.time() - start
     yield Info('info', f'Time spent: {elapsed} seconds.')
```

### Comparing `webscrapbook-1.9.0/webscrapbook/scrapbook/convert/migrate.py` & `webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,18 +161,18 @@
 
         # handle all books if none specified
         for book_id in self.book_ids or host.books:
             try:
                 book = host.books[book_id]
             except KeyError:
                 # skip invalid book ID
-                yield Info('warn', f'Skipped invalid book "{book_id}".')
+                yield Info('warn', f'Skipped invalid book {book_id!r}.')
                 continue
 
-            yield Info('info', f'Handling book "{book_id}"...')
+            yield Info('info', f'Handling book {book_id!r}...')
             book.load_meta_files()
             book.load_toc_files()
 
             if self.convert_legacy:
                 yield Info('info', 'Migrating data files from legacy ScrapBook...')
                 converter = ConvertDataFilesLegacy(book, use_native_tags=self.use_native_tags)
                 yield from converter.run()
@@ -206,24 +206,24 @@
         book = self.book
         for id, meta in book.meta.items():
             index = meta.get('index', '')
             if not index.endswith('/index.html'):
                 continue
 
             type = meta.get('type', '')
-            yield Info('debug', f'Converting data files for "{id}" (type="{type}")...')
+            yield Info('debug', f'Converting data files for {id!r} (type={type!r})...')
             if type == 'postit':
                 index_file = os.path.normpath(os.path.join(book.data_dir, index))
                 yield Info('debug', f'Checking: {index_file}...')
                 try:
-                    content = book.load_note_file(index_file)
+                    content = book.load_postit_file(index_file)
                 except OSError as exc:
-                    yield Info('error', f'Failed to convert "{index}" for "{id}": {exc.strerror}', exc=exc)
+                    yield Info('error', f'Failed to convert {index!r} for {id!r}: {exc.strerror}', exc=exc)
                 else:
-                    book.save_note_file(index_file, content)
+                    book.save_postit_file(index_file, content)
             else:
                 index_dir = os.path.normpath(os.path.dirname(os.path.join(book.data_dir, index)))
                 for root, _dirs, files in os.walk(index_dir):
                     for file in files:
                         if HTML_FILE_FILTER.search(file):
                             file = os.path.join(root, file)
                             yield Info('debug', f'Checking: {file}...')
@@ -232,15 +232,15 @@
                                     file,
                                     use_native_tags=self.use_native_tags,
                                     host=self.book.host,
                                 )
                                 conv.run()
                             except Exception as exc:
                                 traceback.print_exc()
-                                yield Info('error', f'Failed to convert "{file}" for "{id}": {exc}', exc=exc)
+                                yield Info('error', f'Failed to convert {file!r} for {id!r}: {exc}', exc=exc)
 
 
 class ConvertHtmlFileLegacy(HtmlRewriter):
     PRE_WRAP_REGEX = re.compile(r'\bwhite-space:\s*pre-wrap\b', re.I)
 
     LEGACY_CLASSES_MAP = {
         'linemarker-marked-line': 'linemarker',
@@ -817,74 +817,74 @@
             if type == 'postit':
                 continue
 
             index = meta.get('index', '')
             if not index:
                 continue
 
-            yield Info('debug', f'Converting data files for "{id}" (type="{type}")...')
+            yield Info('debug', f'Converting data files for {id!r} (type={type!r})...')
 
             # folder
             if index.endswith('/index.html'):
                 index_dir = os.path.normpath(os.path.dirname(os.path.join(book.data_dir, index)))
                 for root, _dirs, files in os.walk(index_dir):
                     for file in files:
                         if HTML_FILE_FILTER.search(file):
                             file = os.path.join(root, file)
-                            yield Info('debug', f'Checking: "{file}"...')
+                            yield Info('debug', f'Checking: {file}...')
                             try:
                                 conv = ConvertHtmlFileV1(file)
                                 conv.run()
                             except Exception as exc:
                                 traceback.print_exc()
-                                yield Info('error', f'Failed to convert "{file}" for "{id}": {exc}', exc=exc)
+                                yield Info('error', f'Failed to convert {file!r} for {id!r}: {exc}', exc=exc)
 
             # htz/maff
             elif util.is_htz(index) or util.is_maff(index):
                 index_file = os.path.normpath(os.path.join(book.data_dir, index))
                 tempdir = tempfile.mkdtemp()
                 tempzipdir = os.path.join(tempdir, 'zip')
                 try:
-                    util.zip_extract(index_file, tempzipdir)
+                    util.fs.zip_extract(index_file, tempzipdir)
 
                     changed = False
                     for root, _dirs, files in os.walk(tempzipdir):
                         for file in files:
                             if HTML_FILE_FILTER.search(file):
                                 file = os.path.join(root, file)
                                 subpath = file[len(tempzipdir) + 1:].replace('\\', '/')
-                                yield Info('debug', f'Checking: "{subpath}" in "{index_file}"...')
+                                yield Info('debug', f'Checking: {subpath!r} in {index_file!r}...')
                                 try:
                                     conv = ConvertHtmlFileV1(file)
                                     conv.run()
                                     if conv.changed:
                                         changed = True
                                 except Exception as exc:
                                     traceback.print_exc()
-                                    yield Info('error', f'Failed to convert "{subpath}" in "{index_file}" for "{id}": {exc}', exc=exc)
+                                    yield Info('error', f'Failed to convert {subpath!r} in {index_file!r} for {id!r}: {exc}', exc=exc)
 
                     # don't recompress (and change mtime) if no content changed
                     if changed:
-                        util.zip_compress(index_file, tempzipdir, '')
+                        util.fs.zip_compress(index_file, tempzipdir, '')
                 finally:
                     try:
                         shutil.rmtree(tempdir)
                     except OSError:
                         pass
 
             # single file
             elif util.is_html(index):
                 file = os.path.normpath(os.path.join(book.data_dir, index))
-                yield Info('debug', f'Checking: "{file}"...')
+                yield Info('debug', f'Checking: {file}...')
                 try:
                     conv = ConvertHtmlFileV1(file)
                     conv.run()
                 except Exception as exc:
                     traceback.print_exc()
-                    yield Info('error', f'Failed to convert "{file}" for "{id}": {exc}', exc=exc)
+                    yield Info('error', f'Failed to convert {file!r} for {id!r}: {exc}', exc=exc)
 
 
 class ConvertHtmlFileV1(HtmlRewriter):
     def run(self):
         self.require_basic_loader = False
         self.require_annotation_loader = False
 
@@ -1092,15 +1092,15 @@
 
 def run(input, output, book_ids=None, *,
         convert_legacy=False,
         convert_v1=False,
         use_native_tags=False,
         ):
     start = time.time()
-    book_ids_text = ', '.join(f'"{id}"' for id in book_ids) if book_ids else 'all'
+    book_ids_text = ', '.join(f'{id!r}' for id in book_ids) if book_ids else 'all'
     yield Info('info', 'migrating:')
     yield Info('info', f'input directory: {os.path.abspath(input)}')
     yield Info('info', f'output directory: {os.path.abspath(output) if output is not None else "(in-place)"}')
     yield Info('info', f'book(s): {book_ids_text}')
     yield Info('info', f'convert legacy: {convert_legacy}')
     yield Info('info', f'convert v1: {convert_v1}')
     yield Info('info', f'use native tags: {use_native_tags}')
@@ -1115,12 +1115,13 @@
                          convert_v1=convert_v1,
                          use_native_tags=use_native_tags,
                          )
         yield from conv.run()
     except Exception as exc:
         traceback.print_exc()
         yield Info('critical', str(exc), exc=exc)
+        return
     else:
         yield Info('info', 'Done.')
 
     elapsed = time.time() - start
     yield Info('info', f'Time spent: {elapsed} seconds.')
```

### Comparing `webscrapbook-1.9.0/webscrapbook/scrapbook/convert/sb2wsb.py` & `webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/sb2wsb.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,29 +55,29 @@
         self.meta = {}
         self.toc = {'root': []}
         self.rdf_mtime = 0
         self.sitemaps = {}
         self.modifies = {}
 
     def load(self):
-        yield Info('info', 'Loading "scrapbook.rdf"...')
+        yield Info('info', "Loading 'scrapbook.rdf'...")
         yield from self._load_rdf()
         yield Info('info', 'Inspecting data directory...')
         yield from self._load_data_dir()
 
     def _load_rdf(self):
         rdf_file = os.path.join(self.root, 'scrapbook.rdf')
         try:
             self.rdf_mtime = os.stat(rdf_file).st_mtime
             with open(rdf_file, 'rb') as fh:
                 yield from self._parse_rdf(fh)
         except OSError as exc:
-            raise RuntimeError(f'Unable to load "scrapbook.rdf": {exc.strerror}') from exc
+            raise RuntimeError(f"Unable to load 'scrapbook.rdf': {exc.strerror}") from exc
         except etree.XMLSyntaxError as exc:
-            raise RuntimeError(f'Malformed "scrapbook.rdf": {exc.args[0]}') from exc
+            raise RuntimeError(f"Malformed 'scrapbook.rdf': {exc.args[0]}") from exc
 
     def _parse_rdf(self, fh):
         for _event, elem in etree.iterparse(
             fh, events=('end',),
             remove_comments=True, encoding='UTF-8',
             tag=(f'{RDF}Description', f'{NC}BookmarkSeparator', f'{RDF}Seq'),
         ):
@@ -129,24 +129,24 @@
         except OSError as exc:
             raise RuntimeError(f'Failed to scan data directory: {exc.strerror}') from exc
 
         with dirs as dirs:
             for dir in dirs:
                 # check name as ID
                 id = dir.name
-                yield Info('debug', f'Inspecting item folder "{id}"')
+                yield Info('debug', f'Inspecting item folder {id!r}')
                 match_id = REGEX_ID.match(id)
                 if not match_id:
-                    yield Info('warn', f'Skipped item folder "{id}" (invalid ID)')
+                    yield Info('warn', f'Skipped item folder {id!r} (invalid ID)')
                     continue
 
                 # check index.html
                 index_file = os.path.join(dir, 'index.html')
                 if not os.path.isfile(index_file):
-                    yield Info('debug', f'Skipped item folder "{id}" (missing "index.html")')
+                    yield Info('debug', f"Skipped item folder {id!r} (missing 'index.html')")
                     continue
 
                 # record mtime of index.html
                 ts = os.stat(index_file).st_mtime
                 mtime = datetime.fromtimestamp(ts)
                 modify = util.datetime_to_id(mtime)
                 self.modifies[id] = modify
@@ -154,46 +154,46 @@
                 # record seen sitemap.xml
                 sitemap_file = os.path.join(dir, 'sitemap.xml')
                 if os.path.isfile(sitemap_file):
                     self.sitemaps[id] = True
 
                 # load index.dat
                 if load_index_dat:
-                    yield Info('debug', f'Checking "index.dat" for "{id}"')
+                    yield Info('debug', f"Checking 'index.dat' for {id!r}")
                     index_dat_file = os.path.join(dir, 'index.dat')
                     try:
                         assert os.stat(index_dat_file).st_mtime > self.rdf_mtime
                     except (FileNotFoundError, IsADirectoryError, NotADirectoryError, AssertionError):
                         continue
                     except OSError as exc:
-                        yield Info('error', f'Failed to read "index.dat" for "{id}": {exc.strerror}', exc=exc)
+                        yield Info('error', f"Failed to read 'index.dat' for {id!r}: {exc.strerror}", exc=exc)
                         continue
 
-                    yield Info('info', f'Reading metadata from newer "index.dat" for "{id}"')
+                    yield Info('info', f"Reading metadata from newer 'index.dat' for {id!r}")
                     try:
                         with open(index_dat_file, encoding='UTF-8') as fh:
                             meta = {}
                             for line in fh:
                                 line = line.rstrip('\n')
                                 key, _, value = line.partition('\t')
                                 if not value:
                                     continue
                                 meta[key] = value
                             self.meta.setdefault(id, {}).update(meta)
                     except OSError as exc:
-                        yield Info('error', f'Failed to read "index.dat" for "{id}": {exc.strerror}', exc=exc)
+                        yield Info('error', f"Failed to read 'index.dat' for {id!r}: {exc.strerror}", exc=exc)
                         continue
 
 
 class Converter:
-    def __init__(self, input, output, *, no_data_files=False, no_backup=False):
+    def __init__(self, input, output, *, data_files=True, backup=True):
         self.input = os.path.realpath(input)
         self.output = os.path.realpath(output)
-        self.no_data_files = no_data_files
-        self.no_backup = no_backup
+        self.data_files = data_files
+        self.backup = backup
 
         self.index_files = {}
 
     def run(self):
         fsrc = os.path.normpath(os.path.join(__file__, '..', '..', '..', 'resources', 'config.ini'))
         fdst = os.path.normpath(os.path.join(self.output, WSB_DIR, WSB_CONFIG))
 
@@ -209,52 +209,44 @@
 
         yield Info('info', 'Setting up new scrapbook...')
         host = Host(self.output)
         book = host.books['']
         book.load_meta_files()
         book.load_toc_files()
 
-        if not self.no_backup:
-            host.init_backup(note='convert-sb2wsb')
+        if self.backup:
+            host.init_auto_backup(note='convert-sb2wsb')
 
         try:
             yield Info('info', 'Loading legacy scrapbook data...')
             book0 = LegacyBook(self.input)
             yield from book0.load()
 
             yield Info('info', 'Calculating tree data...')
             yield from self._merge_meta(book, book0)
             yield from self._merge_toc(book, book0)
 
             yield Info('info', 'Copying data files...')
             yield from self._copy_data_files(book, book0)
 
-            if not self.no_data_files:
+            if self.data_files:
                 yield from self._convert_data_files(book, book0)
 
             yield Info('info', 'Saving tree files...')
             book.save_meta_files()
             book.save_toc_files()
         finally:
-            if not self.no_backup:
-                host.init_backup(False)
+            if self.backup:
+                host.init_auto_backup(False)
 
     def _merge_meta(self, book, book0):
         for id0, meta0 in book0.meta.items():
-            yield Info('debug', f'Inspecting item metadata for "{id0}"')
+            yield Info('debug', f'Inspecting item metadata for {id0!r}')
             id = id0
             meta = meta0.copy()
-            meta_new = book.meta.setdefault(id, book.DEFAULT_META.copy())
-
-            # meta['id']
-            # omit id field in meta
-            try:
-                del meta['id']
-            except KeyError:
-                pass
 
             # meta['type'], meta['marked']
             meta['type'] = LEGACY_TYPE_MAP.get(meta.get('type'), meta.get('type', ''))
             if meta['type'] == 'marked':
                 # if sitemap exists, type should be site
                 meta['type'] = 'site' if id in book0.sitemaps else ''
                 meta['marked'] = True
@@ -263,15 +255,15 @@
             if meta['type'] not in Book.ITEM_TYPES_WITH_OPTIONAL_INDEX:
                 meta['index'] = f'{id}/index.html'
             elif meta.get('icon', '').startswith(f'{RES_PROTOCOL_BASE}data/{id}/'):
                 # Add a dummy index.html to relate the icon file with the item
                 # if it's saved in the item directory. (mainly for ScrapBee)
                 meta['index'] = f'{id}/index.html'
                 self.index_files[os.path.normpath(os.path.join(book.data_dir, id, 'index.html'))] = True
-                yield Info('debug', f'Registering dummy file "{meta["index"]}"')
+                yield Info('debug', f'Registering dummy file {meta["index"]!r}')
 
             # meta['create']
             # fallback to id
             if meta.get('create'):
                 meta['create'] = util.datetime_to_id(util.id_to_datetime_legacy(meta['create']))
             else:
                 meta['create'] = util.datetime_to_id(util.id_to_datetime_legacy(id))
@@ -340,75 +332,73 @@
             # meta['container']
             # this should not appear in scrapbook.rdf normally
             try:
                 del meta['container']
             except KeyError:
                 pass
 
-            # merge and remove None values
-            meta_new.update(meta)
-            for k, v in list(meta_new.items()):
-                if v is None:
-                    del meta_new[k]
+            # add to book
+            book.add_item(meta, None)
 
     def _merge_toc(self, book, book0):
         book.toc.update(book0.toc)
         return
         yield
 
     def _copy_data_files(self, book, book0):
         with os.scandir(self.input) as dirs:
             for src in dirs:
                 if src.name == WSB_DIR:
-                    yield Info('warn', f'Skipped copying special directory "{WSB_DIR}"')
+                    yield Info('warn', f'Skipped copying special directory {WSB_DIR!r}')
                     continue
 
                 if src.name in PRUNE_FILES:
-                    if self.no_backup:
-                        yield Info('debug', f'Skipped legacy scrapbook entry "{src.name}"')
+                    if self.backup:
+                        yield Info('debug', f'Backup legacy scrapbook entry {src.name!r}')
+                        book.backup(src, base=self.input)
                         continue
                     else:
-                        yield Info('debug', f'Backup legacy scrapbook entry "{src.name}"')
-                        book.backup(src, base=self.input)
+                        yield Info('debug', f'Skipped legacy scrapbook entry {src.name!r}')
                         continue
 
                 dst = os.path.join(book.top_dir, src.name)
 
                 try:
                     shutil.copytree(src, dst)
                 except NotADirectoryError:
                     shutil.copy2(src, dst)
 
         # generate registered dummy index files
         for path in self.index_files:
             if not os.path.lexists(path):
-                yield Info('debug', f'Generating registered dummy file "{path}"')
+                yield Info('debug', f'Generating registered dummy file {path!r}')
                 os.makedirs(os.path.dirname(path), exist_ok=True)
                 with open(path, 'wb'):
                     pass
 
     def _convert_data_files(self, book, book0):
         from .migrate import ConvertDataFilesLegacy
         converter = ConvertDataFilesLegacy(book)
         yield from converter.run()
 
 
-def run(input, output, *, no_data_files=False, no_backup=False):
+def run(input, output, *, data_files=True, backup=True):
     start = time.time()
     yield Info('info', 'conversion mode: ScrapBook --> WebScrapBook')
     yield Info('info', f'input directory: {os.path.abspath(input)}')
     yield Info('info', f'output directory: {os.path.abspath(output)}')
-    yield Info('info', f'no-data-files: {no_data_files}')
-    yield Info('info', f'no-backup: {no_backup}')
+    yield Info('info', f'data-files: {data_files}')
+    yield Info('info', f'backup: {backup}')
     yield Info('info', '')
 
     try:
-        conv = Converter(input, output, no_data_files=no_data_files, no_backup=no_backup)
+        conv = Converter(input, output, data_files=data_files, backup=backup)
         yield from conv.run()
     except Exception as exc:
         traceback.print_exc()
         yield Info('critical', str(exc), exc=exc)
+        return
     else:
         yield Info('info', 'Done.')
 
     elapsed = time.time() - start
     yield Info('info', f'Time spent: {elapsed} seconds.')
```

### Comparing `webscrapbook-1.9.0/webscrapbook/scrapbook/convert/wsb2file.py` & `webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/wsb2file.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,74 +22,74 @@
 
     def run(self):
         host = Host(self.input)
 
         try:
             self.book = host.books[self.book_id]
         except KeyError as exc:
-            raise RuntimeError(f'book "{self.book_id}" does not exist') from exc
+            raise RuntimeError(f'book {self.book_id!r} does not exist') from exc
 
         self.book.load_meta_files()
         self.book.load_toc_files()
 
         id_chain = set()
         path_chain = []
-        ref_ids = self.book.toc.get('root', [])
+        ref_ids = self.book.toc.get(self.book.ROOT_ITEM_ID, [])
         idx_len = len(str(len(ref_ids)))
         for idx, ref_id in enumerate(ref_ids):
             yield from self._export_item(ref_id, idx, idx_len, id_chain, path_chain)
 
     def _export_item(self, id, idx, idx_len, id_chain, path_chain):
         if id not in self.book.meta or id in Book.SPECIAL_ITEM_ID:
             return
 
-        yield Info('debug', f'Exporting item "{id}"')
+        yield Info('debug', f'Exporting item {id!r}')
 
         meta = self.book.meta[id]
         type = meta.get('type', '')
         prefix = f'{idx + 1:0{idx_len}d}-' if self.prefix else ''
         basename = self.book.meta[id].get('title') or (id if type != 'separator' else '----')
 
         path = os.path.join(self.output, *path_chain, util.crop(prefix + util.validate_filename(basename), 128))
         path = self._get_unique_path(path)
         self.used_paths.add(path)
 
         if type == 'folder':
             dst = path
             subpath = os.path.relpath(dst, self.output)
-            yield Info('info', f'Exporting "{id}" to "{subpath}"...')
+            yield Info('info', f'Exporting {id!r} to {subpath!r}...')
             try:
                 os.makedirs(dst, exist_ok=True)
             except OSError as exc:
-                yield Info('error', f'Failed to export "{id}" to "{subpath}": {exc}', exc=exc)
+                yield Info('error', f'Failed to export {id!r} to {subpath!r}: {exc}', exc=exc)
 
         elif type == 'separator':
             if self.prefix:
                 dst = path + '.-'
                 subpath = os.path.relpath(dst, self.output)
-                yield Info('info', f'Exporting "{id}" to "{subpath}"...')
+                yield Info('info', f'Exporting {id!r} to {subpath!r}...')
                 try:
                     os.makedirs(os.path.dirname(dst), exist_ok=True)
                     with open(dst, 'wb') as fh:
                         pass
                 except OSError as exc:
-                    yield Info('error', f'Failed to export "{id}" to "{subpath}": {exc}', exc=exc)
+                    yield Info('error', f'Failed to export {id!r} to {subpath!r}: {exc}', exc=exc)
 
         elif type == 'bookmark':
             source = meta.get('source')
             if source:
                 dst = path + '.htm'
                 subpath = os.path.relpath(dst, self.output)
-                yield Info('info', f'Exporting "{id}" to "{subpath}"...')
+                yield Info('info', f'Exporting {id!r} to {subpath!r}...')
                 try:
                     os.makedirs(os.path.dirname(dst), exist_ok=True)
                     with open(dst, 'w', encoding='UTF-8') as fh:
                         fh.write(f'<!DOCTYPE html><meta charset="UTF-8"><meta http-equiv="refresh" content="0; url={html.escape(source)}">')
                 except OSError as exc:
-                    yield Info('error', f'Failed to export "{id}" to "{subpath}": {exc}', exc=exc)
+                    yield Info('error', f'Failed to export {id!r} to {subpath!r}: {exc}', exc=exc)
 
         else:
             index = meta.get('index', '')
             if index:
                 if index.endswith('/index.html'):
                     src = os.path.normpath(os.path.dirname(os.path.join(self.book.data_dir, index)))
                     ext = '.htd'
@@ -99,23 +99,23 @@
 
                     if not ext:
                         # prevent conflict with folder
                         ext = '._'
 
                 dst = path + ext
                 subpath = os.path.relpath(dst, self.output)
-                yield Info('info', f'Exporting "{id}" to "{subpath}"...')
+                yield Info('info', f'Exporting {id!r} to {subpath!r}...')
                 try:
                     os.makedirs(os.path.dirname(dst), exist_ok=True)
                     try:
                         shutil.copytree(src, dst)
                     except NotADirectoryError:
                         shutil.copy2(src, dst)
                 except OSError as exc:
-                    yield Info('error', f'Failed to export "{id}" to "{subpath}": {exc}', exc=exc)
+                    yield Info('error', f'Failed to export {id!r} to {subpath!r}: {exc}', exc=exc)
 
         # do not add descendants for a recursive item
         if id in id_chain:
             return
 
         id_chain.add(id)
         path_chain.append(os.path.basename(path))
@@ -136,22 +136,23 @@
 
 
 def run(input, output, book_id='', prefix=True):
     start = time.time()
     yield Info('info', 'conversion mode: WebScrapBook --> hierarchical files')
     yield Info('info', f'input directory: {os.path.abspath(input)}')
     yield Info('info', f'output directory: {os.path.abspath(output)}')
-    yield Info('info', f'book: "{book_id}"')
+    yield Info('info', f'book: {book_id!r}')
     yield Info('info', f'prefix: {prefix}')
     yield Info('info', '')
 
     try:
         conv = Converter(input, output, book_id=book_id, prefix=prefix)
         yield from conv.run()
     except Exception as exc:
         traceback.print_exc()
         yield Info('critical', str(exc), exc=exc)
+        return
     else:
         yield Info('info', 'Done.')
 
     elapsed = time.time() - start
     yield Info('info', f'Time spent: {elapsed} seconds.')
```

### Comparing `webscrapbook-1.9.0/webscrapbook/scrapbook/convert/wsb2sb.py` & `webscrapbook-2.0.0b8/webscrapbook/scrapbook/convert/wsb2sb.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,32 +25,32 @@
 }
 
 HTML_FILE_FILTER = re.compile(r'^.+\.x?html$', re.I)
 REGEX_LINEFEED = re.compile(r'\r\n?|\n')
 
 
 class Converter:
-    def __init__(self, input, output, book_id='', no_data_files=False):
+    def __init__(self, input, output, book_id='', data_files=False):
         self.input = input
         self.output = output
         self.book_id = book_id
-        self.no_data_files = no_data_files
+        self.data_files = data_files
 
         self.id_to_oid = {}
         self.oid_to_id = {}
         self.path_to_oid = {}
         self.icons_to_cache = {}
 
     def run(self):
         host = Host(self.input)
 
         try:
             book = host.books[self.book_id]
         except KeyError as exc:
-            raise RuntimeError(f'book "{self.book_id}" does not exist') from exc
+            raise RuntimeError(f'book {self.book_id!r} does not exist') from exc
 
         book.load_meta_files()
         book.load_toc_files()
 
         yield Info('info', 'Creating ID mapping...')
         yield from self._generate_id_mapping(book)
 
@@ -86,43 +86,43 @@
                 oid = util.datetime_to_id_legacy(ts)
             return oid
 
         nonconvertable_ids = []
 
         # map convertable IDs
         for id in book.meta:
-            yield Info('debug', f'Createding ID mapping: "{id}"')
+            yield Info('debug', f'Createding ID mapping: {id!r}')
             oid = get_legacy_id(id)
             if oid and oid not in self.oid_to_id:
                 self.id_to_oid[id] = oid
                 self.oid_to_id[oid] = id
-                yield Info('debug', f'Created ID mapping: "{id}" => "{oid}"')
+                yield Info('debug', f'Created ID mapping: {id!r} => {oid!r}')
             else:
                 nonconvertable_ids.append(id)
 
         # generate for non-convertable IDs
         for id in nonconvertable_ids:
             oid = generate_unique_id(id)
             self.id_to_oid[id] = oid
             self.oid_to_id[oid] = id
-            yield Info('debug', f'Created ID mapping: "{id}" => "{oid}" (new)')
+            yield Info('debug', f'Created ID mapping: {id!r} => {oid!r} (new)')
 
     def _generate_directory_mapping(self, book):
         for id, oid in self.id_to_oid.items():
             index = book.meta[id].get('index', '')
             if not index.endswith('/index.html'):
                 continue
 
             dsrc = os.path.join(book.data_dir, os.path.dirname(index), '')
             self.path_to_oid[os.path.normcase(dsrc)] = oid
-            yield Info('debug', f'Created directory mapping "{dsrc}" => "{oid}"')
+            yield Info('debug', f'Created directory mapping {dsrc!r} => {oid!r}')
 
     def _generate_rdf(self, book):
         def make_meta_node(id, meta):
-            yield Info('debug', f'Generating meta node for "{id}"')
+            yield Info('debug', f'Generating meta node for {id!r}')
 
             oid = self.id_to_oid[id]
             type = meta.get('type', '')
             tagname = f'{NC}BookmarkSeparator' if type == 'separator' else f'{RDF}Description'
 
             node = etree.SubElement(root, tagname)
             node.attrib[f'{RDF}about'] = f'urn:scrapbook:item{oid}'
@@ -149,29 +149,29 @@
                 node.attrib[f'{NS1}modify'] = util.datetime_to_id_legacy(util.id_to_datetime(modify))
 
             locked = meta.get('locked')
             if locked is not None:
                 node.attrib[f'{NS1}lock'] = 'true' if locked else ''
 
         def make_toc_node(id):
-            yield Info('debug', f'Generating TOC node for "{id}"')
+            yield Info('debug', f'Generating TOC node for {id!r}')
 
             node = etree.SubElement(root, f'{RDF}Seq')
-            if id == 'root':
+            if id == book.ROOT_ITEM_ID:
                 node.attrib[f'{RDF}about'] = 'urn:scrapbook:root'
             else:
                 oid = self.id_to_oid[id]
                 node.attrib[f'{RDF}about'] = f'urn:scrapbook:item{oid}'
 
             for ref_id in book.toc.get(id, []):
                 if ref_id in seen_in_toc:
-                    yield Info('debug', f'Skipped adding "{ref_id}" under "{id}" (referenced)')
+                    yield Info('debug', f'Skipped adding {ref_id!r} under {id!r} (referenced)')
                     continue
 
-                yield Info('debug', f'Adding "{ref_id}" under "{id}"')
+                yield Info('debug', f'Adding {ref_id!r} under {id!r}')
                 oref_id = self.id_to_oid[ref_id]
                 child = etree.SubElement(node, f'{RDF}li')
                 child.attrib[f'{RDF}resource'] = f'urn:scrapbook:item{oref_id}'
                 seen_in_toc.add(ref_id)
 
                 if ref_id in book.toc:
                     yield from make_toc_node(ref_id)
@@ -183,16 +183,16 @@
          xmlns:RDF="http://www.w3.org/1999/02/22-rdf-syntax-ns#">
 </RDF:RDF>
 """)
 
         for id, meta in book.meta.items():
             yield from make_meta_node(id, meta)
 
-        seen_in_toc = {'root'}
-        yield from make_toc_node('root')
+        seen_in_toc = {book.ROOT_ITEM_ID}
+        yield from make_toc_node(book.ROOT_ITEM_ID)
 
         try:
             etree.indent(root)
         except AttributeError:
             # etree.indent is supported since lxml >= 4.5.0
             # Do simple line separation for first-level children for older
             # versions.
@@ -202,23 +202,23 @@
         tree = root.getroottree()
         file = os.path.join(self.output, 'scrapbook.rdf')
         os.makedirs(os.path.dirname(file), exist_ok=True)
         tree.write(file, encoding='UTF-8', xml_declaration=True, pretty_print=True)
 
     def _copy_data_files(self, book):
         for id, oid in self.id_to_oid.items():
-            yield Info('debug', f'Copying data files for "{id}" => "{oid}"')
+            yield Info('debug', f'Copying data files for {id!r} => {oid!r}')
             type = book.meta[id].get('type', '')
             if type in Book.ITEM_TYPES_WITH_OPTIONAL_INDEX:
-                yield Info('debug', f'Skipped copying data for "{id}": type is "{type}"')
+                yield Info('debug', f'Skipped copying data for {id!r}: type is {type!r}')
                 continue
 
             index = book.meta[id].get('index', '')
             if not index:
-                yield Info('debug', f'Skipped copying data for "{id}": no index')
+                yield Info('debug', f'Skipped copying data for {id!r}: no index')
                 continue
 
             try:
                 if index.endswith('/index.html'):
                     fsrc = os.path.normpath(os.path.dirname(os.path.join(book.data_dir, index)))
                     fdst = os.path.join(self.output, 'data', oid)
                     os.makedirs(os.path.dirname(fdst), exist_ok=True)
@@ -228,90 +228,90 @@
                     fdst = os.path.join(self.output, 'data', oid, 'index.html')
                     os.makedirs(os.path.dirname(fdst), exist_ok=True)
                     shutil.copy2(fsrc, fdst)
                 elif util.is_htz(index):
                     fsrc = os.path.normpath(os.path.join(book.data_dir, index))
                     fdst = os.path.join(self.output, 'data', oid)
                     os.makedirs(os.path.dirname(fdst), exist_ok=True)
-                    util.zip_extract(fsrc, fdst)
+                    util.fs.zip_extract(fsrc, fdst)
                 elif util.is_maff(index):
                     fsrc = os.path.normpath(os.path.join(book.data_dir, index))
                     fdst = os.path.join(self.output, 'data', oid)
                     pages = util.get_maff_pages(fsrc)
                     if len(pages) == 0:
-                        yield Info('error', f'Failed to copy data for "{id}": no page in MAFF archive')
+                        yield Info('error', f'Failed to copy data for {id!r}: no page in MAFF archive')
                         continue
                     else:
                         if len(pages) > 1:
-                            yield Info('warn', f'"{id}": only the first web page in MAFF archive can be copied')
+                            yield Info('warn', f'{id!r}: only the first web page in MAFF archive can be copied')
                         page = pages[0]
                         topdir, _, _ = page.indexfilename.partition('/')
 
                     os.makedirs(os.path.dirname(fdst), exist_ok=True)
-                    util.zip_extract(fsrc, fdst, topdir)
+                    util.fs.zip_extract(fsrc, fdst, topdir)
                 else:
                     basename = os.path.basename(index)
                     fsrc = os.path.normpath(os.path.join(book.data_dir, index))
                     fdst = os.path.join(self.output, 'data', oid, basename)
                     os.makedirs(os.path.dirname(fdst), exist_ok=True)
                     shutil.copy2(fsrc, fdst)
                     with open(os.path.join(self.output, 'data', oid, 'index.html'), 'w', encoding='UTF-8') as fh:
                         fh.write('<html><head><meta charset="UTF-8">'
                                  f'<meta http-equiv="refresh" content="0;URL=./{quote(basename)}">'
                                  '</head><body></body></html>')
             except OSError as exc:
-                yield Info('error', f'Failed to copy data for "{id}": {exc}', exc=exc)
+                yield Info('error', f'Failed to copy data for {id!r}: {exc}', exc=exc)
 
             if type == 'postit':
-                yield Info('debug', f'Converting data file for "{id}" (type={type})')
+                yield Info('debug', f'Converting data file for {id!r} (type={type!r})')
                 file = os.path.join(self.output, 'data', oid, 'index.html')
                 try:
-                    content = book.load_note_file(file)
+                    content = book.load_postit_file(file)
                 except OSError as exc:
-                    yield Info('error', f'Failed to convert "index.html" for "{id}": {exc.strerror}', exc=exc)
+                    yield Info('error', f"Failed to convert 'index.html' for {id!r}: {exc.strerror}", exc=exc)
                 else:
                     with open(file, 'w', encoding='UTF-8') as fh:
                         fh.write(f"""\
 <html><head><meta http-equiv="Content-Type" content="text/html;Charset=UTF-8"></head><body><pre>
 {content}
 </pre></body></html>""")
-            elif not self.no_data_files:
-                yield Info('debug', f'Converting data files for "{id}" (type={type})')
+            elif self.data_files:
+                yield Info('debug', f'Converting data files for {id!r} (type={type!r})')
                 index_dir = os.path.join(self.output, 'data', oid)
                 for root, _dirs, files in os.walk(index_dir):
                     for file in files:
                         if HTML_FILE_FILTER.search(file):
                             file = os.path.join(root, file)
-                            yield Info('debug', f'Checking: {file}...')
+                            yield Info('debug', f'Checking: {file!r}...')
                             try:
                                 conv = ConvertHtmlFile(file)
                                 conv.run()
                             except Exception as exc:
                                 traceback.print_exc()
-                                yield Info('error', f'Failed to convert "{file}" for "{id}": {exc}', exc=exc)
+                                yield Info('error', f'Failed to convert {file!r} for {id!r}: {exc}', exc=exc)
 
     def _handle_item_icon(self, book, id):
-        yield Info('debug', f'Checking icon for "{id}"')
+        yield Info('debug', f'Checking icon for {id!r}')
         icon = book.meta[id].get('icon', '')
 
         if not icon:
             # return moz_icon if defined
             moz_icon_url = book.meta[id].get('icon-moz')
             if moz_icon_url:
-                yield Info('debug', f'Use moz-icon URL from property for "{id}": "{moz_icon_url}"')
+                yield Info('debug', f'Use moz-icon URL from property for {id!r}: {moz_icon_url!r}')
                 return moz_icon_url
 
             # generate moz-icon:// for files
             if book.meta[id].get('type', '') == 'file':
                 index = book.meta[id].get('index', '')
                 indexfile = os.path.normpath(os.path.join(book.data_dir, index))
                 targetfile = util.get_meta_refreshed_file(indexfile)
                 if targetfile:
                     moz_icon_url = f'moz-icon://{quote(os.path.basename(targetfile))}?size=16'
-                    yield Info('debug', f'Generated moz-icon URL for "{id}": "{moz_icon_url}"')
+                    yield Info('debug', f'Generated moz-icon URL for {id!r}: {moz_icon_url!r}')
                     return moz_icon_url
             return ''
 
         file = book.get_icon_file(book.meta[id])
 
         if not file:
             return icon
@@ -319,46 +319,46 @@
         file_ci = os.path.normcase(file)
 
         # favicon cache should go to "icon" folder
         favicon_dir = os.path.join(book.tree_dir, 'favicon', '')
         if file_ci.startswith(os.path.normcase(favicon_dir)):
             subpath = os.path.relpath(file, favicon_dir)
             fdst = os.path.join(self.output, 'icon', subpath)
-            self.icons_to_cache[file_ci] = fdst
-            yield Info('debug', f'Created icon file mapping (cache): "{file}" => "{fdst}"')
+            self.icons_to_cache[file_ci] = (file, fdst)
+            yield Info('debug', f'Created icon file mapping (cache): {file!r} => {fdst!r}')
             return f'resource://scrapbook/icon/{pathname2url(subpath)}'
 
         # if inside data folder
         if file_ci.startswith(os.path.normcase(book.data_dir)):
             # if under an item folder, map to legacy item folder
             for path, oid in self.path_to_oid.items():
                 if file_ci.startswith(path):
                     subpath = os.path.relpath(file, path)
                     fdst = os.path.join(self.output, 'data', oid, subpath)
-                    self.icons_to_cache[file_ci] = fdst
-                    yield Info('debug', f'Created icon file mapping (item): "{file}" => "{fdst}"')
+                    self.icons_to_cache[file_ci] = (file, fdst)
+                    yield Info('debug', f'Created icon file mapping (item): {file!r} => {fdst!r}')
                     return f'resource://scrapbook/data/{oid}/{pathname2url(subpath)}'
 
             # otherwise, map to sub-data-directory path
             subpath = os.path.relpath(file, book.data_dir)
             fdst = os.path.join(self.output, 'data', subpath)
-            self.icons_to_cache[file_ci] = fdst
-            yield Info('debug', f'Created icon file mapping (data): "{file}" => "{fdst}"')
+            self.icons_to_cache[file_ci] = (file, fdst)
+            yield Info('debug', f'Created icon file mapping (data): {file!r} => {fdst!r}')
             return f'resource://scrapbook/data/{pathname2url(subpath)}'
 
         # record icons outside of "data" folder to copy later
         subpath = os.path.relpath(file, book.top_dir)
         fdst = os.path.join(self.output, subpath)
-        self.icons_to_cache[file_ci] = fdst
-        yield Info('debug', f'Created icon file mapping: "{file}" => "{fdst}"')
+        self.icons_to_cache[file_ci] = (file, fdst)
+        yield Info('debug', f'Created icon file mapping: {file!r} => {fdst!r}')
         return f'resource://scrapbook/{pathname2url(subpath)}'
 
     def _copy_icon_files(self):
-        for fsrc, fdst in self.icons_to_cache.items():
-            yield Info('debug', f'Copying icon "{fsrc}" => "{fdst}"')
+        for fsrc, fdst in self.icons_to_cache.values():
+            yield Info('debug', f'Copying icon {fsrc!r} => {fdst!r}')
             if not os.path.exists(fdst):
                 os.makedirs(os.path.dirname(fdst), exist_ok=True)
                 shutil.copy2(fsrc, fdst)
 
 
 class ConvertHtmlFile(HtmlRewriter):
     def rewrite(self, markups):
@@ -596,27 +596,28 @@
 
             rv.append(markup)
             i += 1
 
         return rv, i
 
 
-def run(input, output, book_id='', no_data_files=False):
+def run(input, output, book_id='', data_files=True):
     start = time.time()
     yield Info('info', 'conversion mode: WebScrapBook --> ScrapBook')
     yield Info('info', f'input directory: {os.path.abspath(input)}')
     yield Info('info', f'output directory: {os.path.abspath(output)}')
-    yield Info('info', f'book: "{book_id}"')
-    yield Info('info', f'no-data-files: {no_data_files}')
+    yield Info('info', f'book: {book_id!r}')
+    yield Info('info', f'data-files: {data_files}')
     yield Info('info', '')
 
     try:
-        conv = Converter(input, output, book_id=book_id, no_data_files=no_data_files)
+        conv = Converter(input, output, book_id=book_id, data_files=data_files)
         yield from conv.run()
     except Exception as exc:
         traceback.print_exc()
         yield Info('critical', str(exc), exc=exc)
+        return
     else:
         yield Info('info', 'Done.')
 
     elapsed = time.time() - start
     yield Info('info', f'Time spent: {elapsed} seconds.')
```

### Comparing `webscrapbook-1.9.0/webscrapbook/scrapbook/exporter.py` & `webscrapbook-2.0.0b8/webscrapbook/util/css.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,181 +1,140 @@
-import json
-import os
-import time
-import traceback
-import zipfile
-from contextlib import nullcontext
-from datetime import datetime, timedelta, timezone
-
-from .. import util
-from ..util import Info
-from .host import Host
-
-
-class Exporter():
-    """Main class for generating exports.
-    """
-    def __init__(self, output, book, *, singleton=False):
-        self.output = output
-        self.book = book
-        self.singleton = singleton
-
-        self.recycle = None
-        self.used_ts = None
-        self.map_id_to_eid = None
-
-    def run(self, item_ids=None, recursive=False):
-        book = self.book
-        self.book.load_meta_files()
-        self.book.load_toc_files()
-
-        os.makedirs(self.output, exist_ok=True)
-
-        self.recycle = set(book.toc.get('recycle', []))
-        self.used_ts = set()
-        self.map_id_to_eid = {}
-
-        if item_ids:
-            id_pool = {id for id in item_ids if id in book.meta and id not in self.recycle}
-
-            # add descendant id if recursive mode
-            if recursive:
-                for id in list(id_pool):
-                    for desc_id in self._iter_child_items(id, [id]):
-                        id_pool.add(desc_id)
-                        yield Info('debug', f'Included descendant item of "{id}": "{desc_id}"')
-        else:
-            id_pool = {id for id in book.meta if id not in self.recycle}
-
-        id_chain = ['root']
-        for id in self._iter_child_items('root', id_chain):
-            if id in id_pool:
-                yield from self._export_item(id, id_chain)
-
-        id_chain = ['hidden']
-        for id in self._iter_child_items('hidden', id_chain):
-            if id in id_pool:
-                yield from self._export_item(id, id_chain)
+import re
+from urllib.parse import urljoin
+from urllib.request import pathname2url
+
+from . import util
+
+
+class CssRewriter:
+    """The base class that handles CSS rewriting for a reference path.
+    """  # noqa: N815, F541
+    pCm = f"""(?:/\\*[\\s\\S]*?(?:\\*/|$))"""  # comment  # noqa: N815, F541  # noqa: N815, F541
+    pSp = f"""(?:[ \\t\\r\\n\\v\\f]*)"""  # space equivalents  # noqa: N815, F541
+    pCmSp = f"""(?:(?:{pCm}|{pSp})*)"""  # comment or space  # noqa: N815, F541
+    pCmSp2 = f"""(?:(?:{pCm}|{pSp})+)"""  # comment or space, at least one  # noqa: N815, F541
+    pChar = f"""(?:\\\\.|[^\\\\"'])"""  # a non-quote char or an escaped char sequence  # noqa: N815, F541
+    pStr = f"""(?:{pChar}*?)"""  # string  # noqa: N815, F541
+    pSStr = f"""(?:{pCmSp}{pStr}{pCmSp})"""  # comment-or-space enclosed string  # noqa: N815, F541
+    pDQStr = f"""(?:"[^\\\\"]*(?:\\\\.[^\\\\"]*)*")"""  # double quoted string  # noqa: N815, F541
+    pSQStr = f"""(?:'[^\\\\']*(?:\\\\.[^\\\\']*)*')"""  # single quoted string  # noqa: N815, F541
+    pES = f"""(?:(?:{pCm}|{pDQStr}|{pSQStr}|{pChar})*?)"""  # embeded string  # noqa: N815, F541
+    pUrl = f"""(?:\\burl\\({pSp}(?:{pDQStr}|{pSQStr}|{pStr}){pSp}\\))"""  # URL  # noqa: N815, F541
+    pUrl2 = f"""(\\burl\\({pSp})({pDQStr}|{pSQStr}|{pStr})({pSp}\\))"""  # URL; catch 3  # noqa: N815, F541
+    pRImport = f"""(@import{pCmSp})({pUrl}|{pDQStr}|{pSQStr})"""  # @import; catch 2  # noqa: N815, F541
+    pRFontFace = f"""(@font-face{pCmSp}{{{pES}}})"""  # @font-face; catch 1  # noqa: N815, F541
+    pRNamespace = f"""(@namespace{pCmSp}(?:{pStr}{pCmSp2})?{pUrl})"""  # @namespace; catch 1  # noqa: N815, F541
+
+    REGEX_REWRITE_CSS = re.compile(f"""{pCm}|{pRImport}|{pRFontFace}|{pRNamespace}|({pUrl})""", re.I)
+    REGEX_PARSE_URL = re.compile(pUrl2, re.I)
+    REGEX_UNESCAPE_CSS = re.compile(r"""\\(?:([0-9A-Fa-f]{1,6}) ?|(.))""")
+
+    def __init__(self, file=None, *,
+                 encoding=None,
+                 ref_url=None, url_chain=set()):  # noqa: B006
+        """Initialize the class and bind associated information.
+
+        Args:
+            file: path of the associated file.
+            ref_url: overriding URL path of the reference path.
+            encoding: the encoding for reading a file. None for autodetection
+                (and self.encoding will be auto reset on reading).
+        """
+        self.file = file
+        self.encoding = encoding
+        self.ref_url = ref_url
+        self.url_chain = url_chain.copy()
+
+        if file:
+            if not ref_url:
+                self.ref_url = urljoin('file:///', pathname2url(file))
+
+        if self.ref_url:
+            self.url_chain.add(self.ref_url)
 
-    def _iter_child_items(self, id, id_chain):
-        """Generate descendant items for the item of id.
+    def run(self, *args, **kwargs):
+        """Common rewriting case when an associated file is provided.
         """
-        for ref_id in self.book.toc.get(id, []):
-            yield ref_id
+        if not self.file:
+            raise RuntimeError('Associated file not set.')
+
+        text = self.load(self.file)
+        return self.rewrite(text, *args, **kwargs)
 
-            # do not export children of a circular item
-            if ref_id not in id_chain:
-                id_chain.append(ref_id)
-                yield from self._iter_child_items(ref_id, id_chain)
-                id_chain.pop()
-
-    def _export_item(self, id, id_chain):
-        if id in self.map_id_to_eid:
-            if self.singleton:
-                yield Info('debug', f'Skipped exporting item "{id}" (singleton mode)')
-                return
+    def load(self, file):
+        """Load a CSS file and return content text.
 
-        yield Info('debug', f'Exporting item "{id}"')
+        May reset self.encoding.
+
+        Args:
+            file: str, path-like, or file-like bytes object
+        Raises:
+            OSError: failed to read the file
+        """
         try:
-            yield from self._export_item_internal(id, id_chain)
-        except Exception as exc:
-            # unexpected error
-            traceback.print_exc()
-            yield Info('error', f'Failed to export "{id}": {exc}', exc=exc)
-
-    def _export_item_internal(self, id, id_chain):
-        meta = self.book.meta[id]
-        index = meta.get('index', '')
-
-        # generate a unique timestamp as prefix
-        ts = datetime.now(timezone.utc)
-        ets = util.datetime_to_id(ts)
-        while ets in self.used_ts:
-            ts += timedelta(milliseconds=1)
-            ets = util.datetime_to_id(ts)
-        self.used_ts.add(ets)
-
-        # setup an export id (eid), which is unique and is same among all
-        # occurrences of the same id, to the ets of the first occurrence
-        eid = self.map_id_to_eid.setdefault(id, ets)
-
-        # generate a unique timestamp prefix
-        basename = ets + '-' + meta.get('title', meta.get('id', ''))
-        basename = util.crop(util.validate_filename(basename), 128)
-
-        # generate a unique filename
-        i = 0
-        dst = os.path.join(self.output, f'{basename}.wsba')
-        while os.path.lexists(dst):
-            i += 1
-            dst = os.path.join(self.output, f'{basename}-{i}.wsba')
-
-        yield Info('info', f'Exporting "{id}" to "{os.path.basename(dst)}"')
-        parents = [{'id': id, 'title': self.book.meta.get(id, {}).get('title', '')} for id in id_chain]
-        meta_data = {'id': id, **meta}
-        export_data = {
-            'version': 1,
-            'id': eid,
-            'timestamp': ets,
-            'timezone': datetime.now().astimezone().utcoffset().total_seconds(),
-            'path': parents,
-        }
-        with zipfile.ZipFile(dst, 'w') as zh:
-            zh.writestr('meta.json', json.dumps(meta_data, ensure_ascii=False, indent=2))
-            zh.writestr('export.json', json.dumps(export_data, ensure_ascii=False, indent=2))
-
-            # include data file(s)
-            if index:
-                zh.writestr('data/', '')
-                src = os.path.join(self.book.data_dir, os.path.dirname(index) if index.endswith('/index.html') else index)
-                yield Info('debug', f'Saving data files for "{id}": "{self.book.get_subpath(src)}"')
-                util.zip_compress(zh, src, f'data/{os.path.basename(src)}')
-
-            # include favicon cache
-            iconfile = self.book.get_icon_file(meta)
-            if not iconfile:
-                return
-
-            favicon_dir = os.path.join(self.book.tree_dir, 'favicon', '')
-            if not os.path.normcase(iconfile).startswith(os.path.normcase(favicon_dir)):
-                return
-
-            zh.writestr('favicon/', '')
-            util.zip_compress(zh, iconfile, f'favicon/{os.path.basename(iconfile)}')
-
-
-def run(root, output, book_id='', item_ids=None, *, recursive=False, singleton=False,
-        config=None, no_lock=False):
-    start = time.time()
-
-    host = Host(root, config)
-
-    # Fail for invalid book ID
-    if book_id not in host.books:
-        yield Info('error', f'Invalid book "{book_id}".')
-        return
-
-    yield Info('debug', f'Loading book "{book_id}".')
-
-    try:
-        book = host.books[book_id]
-
-        if book.no_tree:
-            yield Info('error', f'Unable to export book "{book_id}" ("{book.name}") (no_tree).')
-            return
-
-        yield Info('info', f'Exporting from book "{book_id}" ({book.name}).')
-        lh = nullcontext() if no_lock else book.get_tree_lock().acquire()
-        with lh:
-            generator = Exporter(output, book, singleton=singleton)
-            yield from generator.run(item_ids, recursive)
-
-    except Exception as exc:
-        traceback.print_exc()
-        yield Info('critical', str(exc), exc=exc)
-    else:
-        yield Info('info', 'Done.')
+            fh = open(file, 'rb')
+        except TypeError:
+            fh = file
 
-    yield Info('info', '----------------------------------------------------------------------')
+        try:
+            if not self.encoding:
+                # Seek for the correct charset (encoding).
+                # Use ISO-8859-1 if no encoding can be determined, so that
+                # rewriting work independently with encoding.
+                self.encoding = util.sniff_bom(fh) or 'ISO-8859-1'
+
+            return fh.read().decode(self.encoding)
+        finally:
+            if fh != file:
+                fh.close()
+
+    def rewrite(self, text,
+                rewrite_import_url=lambda url: url,
+                rewrite_font_face_url=lambda url: url,
+                rewrite_background_url=lambda url: url,
+                ):
+        def unescape_css(str):
+            return self.REGEX_UNESCAPE_CSS.sub(unescape_css_sub, str)
+
+        def unescape_css_sub(m):
+            u, c = m.groups()
+            if c:
+                return c
+            if u:
+                return chr(int(u, 16))
+
+        def parse_url(text, callback):
+            def parse_url_sub(m):
+                pre, url, post = m.groups()
+                if url.startswith('"') and url.endswith('"'):
+                    rewritten = callback(unescape_css(url[1:-1]))
+                elif url.startswith("'") and url.endswith("'"):
+                    rewritten = callback(unescape_css(url[1:-1]))
+                else:
+                    rewritten = callback(url.strip())
+                return f'{pre}"{rewritten}"{post}'
+
+            if not callback:
+                return text
+
+            return self.REGEX_PARSE_URL.sub(parse_url_sub, text)
+
+        def rewrite_sub(m):
+            im1, im2, ff, ns, u = m.groups()
+            if im2:
+                if im2.startswith('"') and im2.endswith('"'):
+                    rewritten = rewrite_import_url(unescape_css(im2[1:-1]))
+                elif im2.startswith("'") and im2.endswith("'"):
+                    rewritten = rewrite_import_url(unescape_css(im2[1:-1]))
+                else:
+                    rewritten = parse_url(im2, rewrite_import_url)
+                return f'{im1}"{rewritten}"'
+            elif ff:
+                return parse_url(ff, rewrite_font_face_url)
+            elif ns:
+                # do not rewrite @namespace rule
+                return ns
+            elif u:
+                return parse_url(u, rewrite_background_url)
+            return m.group(0)
 
-    elapsed = time.time() - start
-    yield Info('info', f'Time spent: {elapsed} seconds.')
+        return self.REGEX_REWRITE_CSS.sub(rewrite_sub, text)
```

### Comparing `webscrapbook-1.9.0/webscrapbook/scrapbook/host.py` & `webscrapbook-2.0.0b8/webscrapbook/scrapbook/host.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,20 +103,20 @@
 
         if persist:
             try:
                 with open(self.file, encoding='UTF-8') as fh:
                     assert fh.read() == persist
             except OSError as exc:
                 raise LockPersistOSError(
-                    f'unable to access lock file for "{name}"',
+                    f'unable to access lock file for {name!r}',
                     name=self.name, file=self.file, id=persist
                 ) from exc
             except AssertionError as exc:
                 raise LockPersistUnmatchError(
-                    f'unable to persist lock "{name}" with given ID',
+                    f'unable to persist lock {name!r} with given ID',
                     name=self.name, file=self.file, id=persist
                 ) from exc
 
             self.id = persist
             self._lock = True
         else:
             self.id = token_urlsafe()
@@ -166,15 +166,15 @@
 
         try:
             os.makedirs(os.path.dirname(self.file))
         except FileExistsError:
             pass
         except OSError as exc:
             raise LockGenerateError(
-                f'unable to create lock "{self.name}"',
+                f'unable to create lock {self.name!r}',
                 name=self.name, file=self.file
             ) from exc
 
         while True:
             try:
                 with open(self.file, 'x', encoding='UTF-8') as fh:
                     fh.write(self.id)
@@ -184,102 +184,102 @@
                 except FileNotFoundError:
                     # A rare case that lock file has been removed during the
                     # short inverval. Try acquire again.
                     continue
                 except OSError as exc:
                     # error out if self.file cannot be stated
                     raise LockGenerateError(
-                        f'unable to create lock "{self.name}"',
+                        f'unable to create lock {self.name!r}',
                         name=self.name, file=self.file
                     ) from exc
 
                 # error out if self.file is not a regular file in POSIX
                 # (Windows raises PermissionError rather than FileExistsError
                 # in such case)
                 if not stat.S_ISREG(st.st_mode):
                     raise LockGenerateError(
-                        f'unable to create lock "{self.name}"',
+                        f'unable to create lock {self.name!r}',
                         name=self.name, file=self.file
                     ) from exc
 
                 t = time.time()
 
                 if t >= timeout_time:
                     raise LockTimeoutError(
-                        f'timeout when acquiring lock "{self.name}"',
+                        f'timeout when acquiring lock {self.name!r}',
                         name=self.name, file=self.file
                     )
 
                 stale_time = st.st_mtime + self.stale
 
                 if t >= stale_time:
                     # Current lock file is stale. Rewrite with current ID.
                     try:
                         with open(self.file, 'w', encoding='UTF-8') as fh:
                             fh.write(self.id)
                     except OSError as exc:
                         raise LockRegenerateError(
-                            f'unable to regenerate stale lock "{self.name}"',
+                            f'unable to regenerate stale lock {self.name!r}',
                             name=self.name, file=self.file) from exc
                     else:
                         break
 
                 time.sleep(poll_interval)
             except OSError as exc:
                 raise LockGenerateError(
-                    f'unable to create lock "{self.name}"',
+                    f'unable to create lock {self.name!r}',
                     name=self.name, file=self.file
                 ) from exc
             else:
                 break
 
         self._lock = True
         return _FileLockAcquireProxy(self)
 
     def extend(self):
         """Extend duration of the lock.
         """
         if not self._lock:
             raise LockExtendNotAcquiredError(
-                f'lock "{self.name}" has not been acquired',
+                f'lock {self.name!r} has not been acquired',
                 name=self.name, file=self.file
             )
 
         try:
             os.utime(self.file)
         except FileNotFoundError as exc:
             raise LockExtendNotFoundError(
-                f'file for lock "{self.name}" does not exist',
+                f'file for lock {self.name!r} does not exist',
                 name=self.name, file=self.file
             ) from exc
         except OSError as exc:
             raise LockExtendError(
-                f'unable to extend lock "{self.name}"',
+                f'unable to extend lock {self.name!r}',
                 name=self.name, file=self.file
             ) from exc
 
     def release(self):
         """Release the lock.
         """
         if not self._lock:
             raise LockReleaseNotAcquiredError(
-                f'lock "{self.name}" has not been acquired',
+                f'lock {self.name!r} has not been acquired',
                 name=self.name, file=self.file
             )
 
         try:
             os.remove(self.file)
         except FileNotFoundError as exc:
             raise LockReleaseNotFoundError(
-                f'file for lock "{self.name}" does not exist',
+                f'file for lock {self.name!r} does not exist',
                 name=self.name, file=self.file
             ) from exc
         except OSError as exc:
             raise LockReleaseError(
-                f'unable to release lock "{self.name}"',
+                f'unable to release lock {self.name!r}',
                 name=self.name, file=self.file
             ) from exc
         else:
             self._lock = False
 
     def keep(self):
         """Spawn a keeper thread to keep the lock fresh until released.
@@ -362,15 +362,15 @@
         self.templates = [os.path.join(t, 'templates') for t in self.themes]
         self.locales = [os.path.join(t, 'locales') for t in self.themes]
 
         self.locks = os.path.join(root, WSB_DIR, 'locks')
 
         self.books = BooksProxy(self)
 
-        self._backup_dir = None  # directory for auto backup
+        self._auto_backup_dir = None  # directory for auto backup
 
     def __repr__(self):
         repr_str = ', '.join(f'{attr}={repr(getattr(self, attr))}' for attr in self.REPR_ATTRS)
         return f'{self.__class__.__name__}({repr_str})'
 
     def get_i18n(self, lang=None, domain=None):
         return I18N(self.locales, lang, domain)
@@ -395,16 +395,15 @@
         Also canonicalize path separators to "/".
         """
         path = os.path.relpath(file, self.root)
 
         # Convert non-standard path separators to '/'. (Currently this only
         # happens on Windows, which uses '\', and it's safe to do so since
         # Windows does not allow '/' in filename.)
-        if os.sep != '/':
-            path = path.replace(os.sep, '/')
+        path = util.unify_pathsep(path)
 
         return path
 
     def backup(self, file, backup_dir=None, base=None, move=False):
         """Create a backup for the file or directory.
 
         Args:
@@ -426,15 +425,15 @@
         if backup_dir is None:
             ts = util.datetime_to_id()
             backup_dir = os.path.join(self.backup_dir, ts)
 
         if not os.path.exists(file):
             return
 
-        if not os.path.abspath(file).startswith(os.path.join(base, '')):
+        if not os.path.normcase(os.path.abspath(file)).startswith(os.path.normcase(os.path.join(base, ''))):
             return
 
         dst = os.path.join(backup_dir, os.path.relpath(file, base))
         if os.path.lexists(dst):
             try:
                 shutil.rmtree(dst)
             except NotADirectoryError:
@@ -456,33 +455,53 @@
             backup_dir: a path-like for the backup.
         """
         try:
             shutil.rmtree(backup_dir)
         except FileNotFoundError:
             pass
 
-    def init_backup(self, ts=True, note=None):
-        """Setup a backup dir for following auto backups until next set.
+    def get_auto_backup_dir(self, ts=True, note=None):
+        """Get the path of a subdir for backup.
 
         Args:
             ts: a webscrapbook ID as timestamp. True to generate one from
-                the current time. False to disable auto backup.
+                the current time.
             note: a note text for the backup, sanitized to a valid filename
-        """
-        if ts is False:
-            self._backup_dir = None
-            return
 
+        Returns:
+            str: the backup dir path
+        """
         if ts is True:
             ts = util.datetime_to_id()
 
         filename = ts + (f'-{util.validate_filename(note)}' if note else '')
 
-        self._backup_dir = os.path.join(self.backup_dir, filename)
+        return os.path.join(self.backup_dir, filename)
+
+    def init_auto_backup(self, ts=True, note=None):
+        """Setup a backup dir for following auto backups until next set.
+
+        NOTE: This is not thread-safe and should only be used on a thread-specific
+            Host object.
+
+        Args:
+            ts: a webscrapbook ID as timestamp. True to generate one from
+                the current time. False to disable auto backup.
+            note: a note text for the backup, sanitized to a valid filename
+
+        Returns:
+            str: the backup dir path
+        """
+        if ts is False:
+            self._auto_backup_dir = None
+        else:
+            self._auto_backup_dir = self.get_auto_backup_dir(ts, note)
+
+        return self._auto_backup_dir
 
     def auto_backup(self, file, base=None, move=False):
         """Perform an auto backup if inited.
         """
-        if not self._backup_dir:
+        if not self._auto_backup_dir:
             return
 
-        self.backup(file, backup_dir=self._backup_dir, base=base, move=move)
+        self.backup(file, backup_dir=self._auto_backup_dir, base=base, move=move)
```

### Comparing `webscrapbook-1.9.0/webscrapbook/scrapbook/importer.py` & `webscrapbook-2.0.0b8/webscrapbook/scrapbook/importer.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,89 +2,90 @@
 import json
 import os
 import re
 import shutil
 import time
 import traceback
 import uuid
-import zipfile
 from contextlib import nullcontext
-from datetime import datetime, timedelta, timezone
+from urllib.request import pathname2url
 
 from .. import util
+from .._polyfill import zipfile
 from ..util import Info
-from .book import Book
 from .host import Host
 
 REGEX_TARGET_FILENAME_FORMATTER = re.compile(r'%([^%]*)%')
 
 
 class Importer():
-    """Main class for importing.
-    """
+    """Main class for importing."""
     def __init__(self, book, *,
                  target_id=None,
                  target_index=None,
                  target_filename=None,
                  rebuild_folders=False,
                  prune=False,
                  resolve_id_used='skip',  # skip, replace, new
                  ):
         self.book = book
-        self.target_id = target_id or 'root'
-        self.target_index = target_index
+        self.target_id = target_id or book.ROOT_ITEM_ID
+        self.target_index = target_index if (isinstance(target_index, int) and target_index >= 0) else None
         self.target_filename = target_filename or '%ID%'
         self.rebuild_folders = rebuild_folders
         self.prune = prune
         self.resolve_id_used = resolve_id_used
 
-        self.map_eid_to_id = None
-        self.map_id_to_new_id = None
-
     def run(self, files=None):
-        book = self.book
         self.book.load_meta_files()
         self.book.load_toc_files()
 
-        self.map_eid_to_id = {}
+        self.map_eid_to_info = {}
         self.map_id_to_new_id = {}
 
-        book_meta_orig = copy.deepcopy(book.meta)
-        book_toc_orig = copy.deepcopy(book.toc)
+        book_meta_orig = copy.deepcopy(self.book.meta)
+        book_toc_orig = copy.deepcopy(self.book.toc)
+
+        # fix target_id
+        if not self.rebuild_folders:
+            if not (self.target_id in self.book.meta or self.target_id in self.book.SPECIAL_ITEM_ID):
+                yield Info('warn', f'Target ID {self.target_id!r} is invalid. Use {self.book.ROOT_ITEM_ID!r} instead.')
+                self.target_id = self.book.ROOT_ITEM_ID
 
         for file in files:
             if os.path.isdir(file):
                 with os.scandir(file) as entries:
                     srcs = sorted(f.path for f in entries if util.is_wsba(f.path))
             elif os.path.isfile(file):
                 if not util.is_wsba(file):
-                    yield Info('warn', f'Skipped invalid file "{os.path.basename(file)}"')
+                    yield Info('warn', f'Skipped invalid file {os.path.basename(file)!r}')
                     continue
                 srcs = [file]
             else:
-                yield Info('error', f'Failed to import file "{os.path.basename(file)}": unable to access file')
+                yield Info('error', f'Failed to import file {os.path.basename(file)!r}: unable to access file')
                 continue
 
             for src in srcs:
                 try:
-                    yield Info('debug', f'Importing file "{os.path.basename(src)}"')
+                    yield Info('debug', f'Importing file {os.path.basename(src)!r}')
                     id, eid, parent_id = yield from self._import_file(src)
                 except RuntimeError as exc:
                     # intended raise to skip the import
-                    yield Info('error', f'Failed to import file "{os.path.basename(src)}": {exc}', exc=exc)
+                    yield Info('error', f'Failed to import file {os.path.basename(src)!r}: {exc}', exc=exc)
                 except Exception as exc:
                     # unexpected error
                     traceback.print_exc()
-                    yield Info('error', f'Failed to import file "{os.path.basename(src)}": {exc}', exc=exc)
+                    yield Info('error', f'Failed to import file {os.path.basename(src)!r}: {exc}', exc=exc)
                 else:
                     # finalize a successful import
-                    yield Info('info', f'Imported "{id}" (under "{parent_id}")')
-                    self.map_eid_to_id.setdefault(eid, id)
+                    text_parent = '' if parent_id is None else f' (under {parent_id!r})'
+                    yield Info('info', f'Imported {id!r}{text_parent}')
+                    self.map_eid_to_info.setdefault(eid, {}).setdefault('id', id)
                     if self.prune:
-                        yield Info('debug', f'Removing "{os.path.basename(src)}" (prune)')
+                        yield Info('debug', f'Removing {os.path.basename(src)!r} (prune)')
                         os.remove(src)
 
         # update files
         if self.book.meta != book_meta_orig:
             yield Info('info', 'Saving changed meta files...')
             self.book.save_meta_files()
 
@@ -199,28 +200,51 @@
         with zipfile.ZipFile(file) as zh:
             with zh.open('meta.json') as fh:
                 meta = json.load(fh)
 
             with zh.open('export.json') as fh:
                 export_info = json.load(fh)
 
+            if export_info['version'] == 2:
+                try:
+                    assert isinstance(export_info['id'], str)
+                    assert isinstance(export_info['timestamp'], str)
+                    assert isinstance(export_info['timezone'], int)
+                    assert isinstance(export_info['path'], list)
+                    assert isinstance(export_info['index'], int)
+                except (AssertionError, KeyError):
+                    raise RuntimeError('Malformed archive')
+
+            elif export_info['version'] == 1:
+                try:
+                    assert isinstance(export_info['id'], str)
+                    assert isinstance(export_info['timestamp'], str)
+                    assert isinstance(export_info['timezone'], float)
+                    assert isinstance(export_info['path'], list)
+                except (AssertionError, KeyError):
+                    raise RuntimeError('Malformed archive')
+
+            else:
+                raise RuntimeError(f'Unsupported archive version: {export_info["version"]!r}')
+
             id = meta.pop('id')
-            if id in Book.SPECIAL_ITEM_ID:
-                raise RuntimeError(f'invalid ID "{id}"')
+            if id in self.book.SPECIAL_ITEM_ID:
+                raise RuntimeError(f'invalid ID {id!r}')
 
-            # duplicated occurrence of a previously imported id
-            # add to TOC only
-            if self.map_eid_to_id.get(export_info['id']) == id:
-                parent_id = yield from self._insert_to_toc(id, export_info)
-                return (id, export_info['id'], parent_id)
+            # skip importing data for a duplicated occurrence of a previously
+            # imported item
+            imported_id = self.map_eid_to_info.setdefault(export_info['id'], {}).get('id')
+            if imported_id is not None:
+                id = imported_id
+                yield Info('debug', f'Skipped importing data for multi-referenced {id!r}')
+            else:
+                id = yield from self._import_meta_and_data(id, meta, zh, export_info)
 
-            # do the import
-            id = yield from self._import_meta_and_data(id, meta, zh, export_info)
             parent_id = yield from self._insert_to_toc(id, export_info)
-            return (id, export_info['id'], parent_id)
+            return id, export_info['id'], parent_id
 
     def _import_meta_and_data(self, id, meta, zh, export_info):
         """Import meta and data
 
         Returns:
             string: ID of the imported item
         """
@@ -238,27 +262,27 @@
             dst = os.path.normpath(os.path.join(self.book.data_dir, filename))
             meta['index'] = filename + ('/index.html' if index.endswith('/index.html') else '')
 
         # handle resolve cases if id exists
         # may overwrite id, dst, and meta['index']
         if id in self.book.meta:
             if self.resolve_id_used == 'skip':
-                raise RuntimeError(f'ID "{id}" already exists')
+                raise RuntimeError(f'ID {id!r} already exists')
 
             elif self.resolve_id_used == 'replace':
                 index_old = self.book.meta[id].get('index', '')
 
                 # replace only if index type matches
                 if os.path.splitext(index)[1] != os.path.splitext(index_old)[1]:
                     raise RuntimeError('index type not match')
 
                 if index_old.endswith('/index.html') != index.endswith('/index.html'):
                     raise RuntimeError('index type not match')
 
-                yield Info('info', f'Force importing duplicated "{id}"...')
+                yield Info('info', f'Force importing duplicated {id!r}...')
 
                 if index:
                     # use original index
                     meta['index'] = index_old
 
                     # remove current index file or folder
                     if index.endswith('/index.html'):
@@ -270,151 +294,179 @@
                     else:
                         dst = os.path.normpath(os.path.join(self.book.data_dir, index_old))
                         try:
                             os.remove(dst)
                         except FileNotFoundError:
                             pass
 
-            elif self.resolve_id_used == 'new':
-                # generate a new unique id
-                ts = datetime.now(timezone.utc)
-                new_id = util.datetime_to_id(ts)
-                while new_id in self.book.meta:
-                    ts += timedelta(milliseconds=1)
-                    new_id = util.datetime_to_id(ts)
+                self.map_eid_to_info.setdefault(export_info['id'], {}).setdefault('replaced', True)
 
-                yield Info('info', f'Importing duplicated "{id}" as "{new_id}"...')
+            elif self.resolve_id_used == 'new':
+                new_id = self.book.get_unique_id()
+                yield Info('info', f'Importing duplicated {id!r} as {new_id!r}...')
                 self.map_id_to_new_id[id] = new_id
                 id = new_id
 
                 if index:
                     # overwrite dst and index
                     filename = self.generate_imported_filename(id, meta, export_info) + ext
                     dst = os.path.normpath(os.path.join(self.book.data_dir, filename))
                     meta['index'] = filename + ('/index.html' if index.endswith('/index.html') else '')
 
             else:
-                raise RuntimeError(f'unknown resolve mode: "{self.resolve_id_used}"')
+                raise RuntimeError(f'unknown resolve mode: {self.resolve_id_used!r}')
 
         # import data files
         if index:
             if os.path.lexists(dst):
-                raise RuntimeError(f'file "{dst}" already exists')
+                raise RuntimeError(f'file {dst!r} already exists')
 
-            yield Info('debug', f'Extracting data files to "{self.book.get_subpath(dst)}"')
+            yield Info('debug', f'Extracting data files to {self.book.get_subpath(dst)!r}')
             os.makedirs(os.path.dirname(dst), exist_ok=True)
-            util.zip_extract(zh, dst, src, tzoffset=export_info['timezone'])
+            util.fs.zip_extract(zh, dst, src, tzoffset=export_info['timezone'])
 
         # import favicon
         for f in zh.namelist():
             if f.startswith('favicon/') and not f.endswith('/'):
+                basename = os.path.basename(f)
+                iconfile = os.path.join(self.book.tree_dir, 'favicon', basename)
+                os.makedirs(os.path.dirname(iconfile), exist_ok=True)
+
                 try:
-                    basename = os.path.basename(f)
-                    dst = os.path.join(self.book.tree_dir, 'favicon', basename)
-                    os.makedirs(os.path.dirname(dst), exist_ok=True)
-                    util.zip_extract(zh, dst, f, tzoffset=export_info['timezone'])
+                    util.fs.zip_extract(zh, iconfile, f, tzoffset=export_info['timezone'])
                 except FileExistsError:
-                    yield Info('debug', f'Skipped existing favicon cache "{basename}"')
+                    yield Info('debug', f'Skipped existing favicon cache {basename!r}')
                 else:
-                    yield Info('info', f'Added favicon cache "{basename}"')
+                    yield Info('info', f'Added favicon cache {basename!r}')
+
+                # rewrite icon property to be consistent with the importing book
+                try:
+                    base = os.path.dirname(dst)
+                except UnboundLocalError:
+                    base = self.book.data_dir
+                meta['icon'] = pathname2url(os.path.relpath(iconfile, base))
+
+                break
 
         self.book.meta[id] = meta
         return id
 
     def _insert_to_toc(self, id, export_info):
         """Insert the importing item to TOC
 
         Returns:
             string: ID of the parent the item is inserted under
         """
+        if self.map_eid_to_info.setdefault(export_info['id'], {}).get('replaced'):
+            yield Info('debug', f'Skipped inserting replaced {id!r}')
+            return None
+
+        # deduplicate by checking the ref_key
         if self.rebuild_folders:
             export_path = export_info['path']
-            parent_id = export_path[-1]['id']
-            parent_id = self.map_id_to_new_id.get(parent_id, parent_id)
+            if export_info['version'] == 2:
+                ref_key = (export_path[-1]['id'], export_info['index'])
+            elif export_info['version'] == 1:
+                ref_key = export_path[-1]['id']
         else:
-            parent_id = self.target_id
+            if export_info['version'] == 2:
+                ref_key = (self.target_id, None)
+            elif export_info['version'] == 1:
+                ref_key = self.target_id
+
+        if ref_key in self.map_eid_to_info[export_info['id']].setdefault('refs', set()):
+            yield Info('debug', f'Skipped inserting multi-referenced {id!r}')
+            return None
+
+        self.map_eid_to_info[export_info['id']]['refs'].add(ref_key)
 
-        if parent_id in self.book.meta or parent_id in Book.SPECIAL_ITEM_ID:
-            yield from self._insert_to_id(id, parent_id)
+        # perform the insertion
+        if not self.rebuild_folders:
+            parent_id = self.target_id
+            self._insert_to_id(id, parent_id)
             return parent_id
 
-        for i in reversed(range(len(export_path) - 1)):
+        for i in reversed(range(len(export_path))):
             parent_id = export_path[i]['id']
-            if parent_id in self.book.meta or parent_id in Book.SPECIAL_ITEM_ID:
+            parent_id = self.map_id_to_new_id.get(parent_id, parent_id)
+            if parent_id in self.book.meta or parent_id in self.book.SPECIAL_ITEM_ID:
                 break
         else:
             # for a bad path data not starting from 'root'
             i = -1
-            parent_id = 'root'
+            parent_id = self.book.ROOT_ITEM_ID
 
         for j in range(i + 1, len(export_path)):
-            # generate a new unique id
-            ts = datetime.now(timezone.utc)
-            new_id = util.datetime_to_id(ts)
-            while new_id in self.book.meta:
-                ts += timedelta(milliseconds=1)
-                new_id = util.datetime_to_id(ts)
-
-            yield Info('info', f'Generating folder "{new_id}" under "{parent_id}"...')
-            new_meta = {
-                'title': export_path[j]['title'],
-                'type': 'folder',
-                'create': new_id,
-                'modify': new_id,
-            }
-            self.book.meta[new_id] = new_meta
-            self.book.toc.setdefault(parent_id, []).append(new_id)
-            self.map_id_to_new_id[export_path[j]['id']] = new_id
+            folder_id = export_path[j]['id']
+            folder_title = export_path[j]['title']
+            try:
+                new_id = self.map_id_to_new_id[folder_id]
+            except KeyError:
+                new_items = self.book.add_item({
+                    'title': folder_title,
+                    'type': 'folder',
+                }, parent_id)
+                new_id = next(iter(new_items))
+                self.map_id_to_new_id[folder_id] = new_id
+                yield Info('info', f'Generated folder {new_id!r} for missing {folder_id!r} under {parent_id!r}')
+            else:
+                if new_id not in self.book.toc.get(parent_id, ()):
+                    self._insert_to_id(new_id, parent_id, allow_insert=False)
+                    yield Info('info', f'Inserted folder {new_id!r} for missing {folder_id!r} under {parent_id!r}')
             parent_id = new_id
 
-        yield from self._insert_to_id(id, parent_id, allow_insert=False)
+        self._insert_to_id(id, parent_id, allow_insert=False)
         return parent_id
 
     def _insert_to_id(self, id, parent_id, allow_insert=True):
-        if id in self.book.toc.get(parent_id, []):
-            yield Info('debug', f'Skipped appending "{id}" to "{parent_id}": already in')
-            return
-
         parent = self.book.toc.setdefault(parent_id, [])
 
         if allow_insert and self.target_index is not None:
             parent.insert(self.target_index, id)
-            self.target_index += 1
+            if not self.book.config['new_at_top']:
+                self.target_index += 1
         else:
-            parent.append(id)
+            target_index = 0 if self.book.config['new_at_top'] else len(parent)
+            parent.insert(target_index, id)
 
 
-def run(root, files, book_id='', *, config=None, no_lock=False, **kwargs):
+def run(host, files, book_id='', *, lock=True, **kwargs):
     start = time.time()
 
-    host = Host(root, config)
+    if isinstance(host, Host):
+        pass
+    elif isinstance(host, str):
+        host = Host(host)
+    else:
+        host = Host(*host)
 
     # Fail for invalid book ID
     if book_id not in host.books:
-        yield Info('error', f'Invalid book "{book_id}".')
+        yield Info('error', f'Invalid book {book_id!r}.')
         return
 
-    yield Info('debug', f'Loading book "{book_id}".')
+    yield Info('debug', f'Loading book {book_id!r}.')
 
     try:
         book = host.books[book_id]
 
         if book.no_tree:
-            yield Info('error', f'Unable to import to book "{book_id}" ("{book.name}") (no_tree).')
+            yield Info('error', f'Unable to import to book {book_id!r} ({book.name!r}) (no_tree).')
             return
 
-        yield Info('info', f'Impoting to book "{book_id}" ({book.name}).')
-        lh = nullcontext() if no_lock else book.get_tree_lock().acquire()
+        yield Info('info', f'Impoting to book {book_id!r} ({book.name!r}).')
+        lh = book.get_tree_lock().acquire() if lock else nullcontext()
         with lh:
             generator = Importer(book, **kwargs)
             yield from generator.run(files)
 
     except Exception as exc:
         traceback.print_exc()
         yield Info('critical', str(exc), exc=exc)
+        return
     else:
         yield Info('info', 'Done.')
 
     yield Info('info', '----------------------------------------------------------------------')
 
     elapsed = time.time() - start
     yield Info('info', f'Time spent: {elapsed} seconds.')
```

### Comparing `webscrapbook-1.9.0/webscrapbook/scrapbook/indexer.py` & `webscrapbook-2.0.0b8/webscrapbook/scrapbook/indexer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Generator to generate item metadata from files.
 """
 import io
-import mimetypes
 import os
 import re
 import shutil
 import traceback
-import zipfile
 from base64 import b64encode
-from datetime import datetime, timedelta, timezone
+from datetime import datetime
 from functools import partial
 from urllib.error import URLError
 from urllib.parse import quote, unquote, urljoin, urlsplit, urlunsplit
 from urllib.request import pathname2url, url2pathname, urlopen
 
 from lxml import etree
 
 from .. import util
+from .._polyfill import mimetypes, zipfile
 from ..util import Info
 from ..util.css import CssRewriter
 from ..util.html import REGEX_ASCII_WHITESPACES, HtmlRewriter
 
 HTML_TITLE_EXCLUDE_PARENTS = {
     'xmp',
     'svg',
@@ -45,14 +44,16 @@
     'audio/ogg': '.oga',
     'video/mpeg': '.mpeg',
     'video/mp4': '.mp4',
     'video/ogg': '.ogv',
     'application/ogg': '.ogx',
 }
 
+SUPPORT_FOLDER_SUFFIXES = ['.files', '_files']
+
 
 def generate_item_title(book, id):
     # infer from source
     if book.meta[id].get('source'):
         parts = urlsplit(book.meta[id].get('source'))
         if parts.scheme:
             title = os.path.basename(unquote(parts.path))
@@ -158,45 +159,49 @@
     def run(self, files):
         self.book.load_meta_files()
 
         indexed = {}
         for file in files:
             id = yield from self._index_file(file)
             if id:
-                yield Info('info', f'Added item "{id}" for "{self.book.get_subpath(file)}".')
+                yield Info('info', f'Added item {id!r} for {self.book.get_subpath(file)!r}.')
                 indexed[id] = True
 
         return indexed
 
     def _index_file(self, file):
         subpath = self.book.get_subpath(file)
-        yield Info('debug', f'Indexing "{subpath}"...')
+        yield Info('debug', f'Indexing {subpath!r}...')
 
         if not os.path.isfile(file):
-            yield Info('error', f'File "{subpath}" does not exist.')
+            yield Info('error', f'File {subpath!r} does not exist.')
             return None
 
         _, ext = os.path.splitext(file.lower())
         is_webpage = ext in self.book.ITEM_INDEX_ALLOWED_EXT
 
         if is_webpage:
             tree = self.book.get_tree_from_index_file(file)
             if tree is None:
-                yield Info('error', f'Failed to read document from file "{subpath}"')
+                yield Info('error', f'Failed to read document from file {subpath!r}')
                 return None
 
             tree_root = tree.getroot()
             if tree_root is None or tree_root.tag != 'html':
-                yield Info('error', f'No html element in file "{subpath}"')
+                yield Info('error', f'No html element in file {subpath!r}')
                 return None
 
             html_elem = tree_root
 
-        # generate default properties
-        meta = self.book.DEFAULT_META.copy()
+        # prepare meta
+        # use empty create and modify to prevent auto-generated by book.add_item()
+        meta = {
+            'create': '',
+            'modify': '',
+        }
 
         if is_webpage:
             # attempt to load metadata generated by certain applications
             if self.handle_ie_meta:
                 self._handle_ie_meta(meta, tree_root)
 
             if self.handle_singlefile_meta:
@@ -210,96 +215,86 @@
 
             # merge properties from html[data-scrapbook-*] attributes
             for key, value in html_elem.attrib.items():
                 if key.startswith('data-scrapbook-'):
                     meta[key[15:]] = value
 
         # id
-        id = meta.pop('id')
-        if id:
+        id = meta.get('id')
+        if id is not None:
             # if explicitly specified in html attributes, use it or fail out.
             if id in self.book.meta:
-                yield Info('error', f'Specified ID "{id}" is already used.')
+                yield Info('error', f'Specified ID {id!r} is already used.')
                 return None
 
             if id in self.book.SPECIAL_ITEM_ID:
-                yield Info('error', f'Specified ID "{id}" is invalid.')
+                yield Info('error', f'Specified ID {id!r} is invalid.')
                 return None
 
         else:
             # Take base filename as id if it corresponds to standard timestamp
             # format and not used; otherwise generate a new one.
             basepath = os.path.relpath(file, self.book.data_dir)
             basename = os.path.basename(basepath)
             if basename == 'index.html':
                 basename = os.path.basename(os.path.dirname(basepath))
             id, _ = os.path.splitext(basename)
 
-            if not util.id_to_datetime(id) or id in self.book.meta:
-                ts = datetime.now(timezone.utc)
-                id = util.datetime_to_id(ts)
-                while id in self.book.meta:
-                    ts += timedelta(milliseconds=1)
-                    id = util.datetime_to_id(ts)
+            if util.id_to_datetime(id) and id not in self.book.meta:
+                meta['id'] = id
 
-        # add to meta
-        self.book.meta[id] = meta
+        # add to book
+        new_items = self.book.add_item(meta, None)
+        id, meta = next(iter(new_items.items()))
 
         # index
         meta['index'] = os.path.relpath(file, self.book.data_dir).replace('\\', '/')
 
         # type
-        if not meta['type']:
+        if meta.get('type') is None:
             meta['type'] = '' if is_webpage else 'file'
 
         # title
-        if meta['title'] is None:
+        if meta.get('title') is None:
             title = None
             if is_webpage:
                 title_elem = next(iter_title_elems(tree), None)
                 if title_elem is not None:
                     try:
                         title = (
                             (title_elem.text or '')
                             + ''.join(etree.tostring(e, encoding='unicode') for e in title_elem)
                         )
                     except UnicodeDecodeError as exc:
-                        yield Info('error', f'Failed to extract title for "{id}": {exc}', exc=exc)
+                        yield Info('error', f'Failed to extract title for {id!r}: {exc}', exc=exc)
             if not title or not title.strip():
                 title = generate_item_title(self.book, id)
             meta['title'] = title or ''
 
         # create
-        if not meta['create']:
+        if not meta.get('create'):
             meta['create'] = generate_item_create(self.book, id) or ''
 
         # modify
-        if not meta['modify']:
+        if not meta.get('modify'):
             meta['modify'] = generate_item_modify(self.book, id) or ''
 
         # icon
-        if meta['icon'] is None:
+        if meta.get('icon') is None:
             if is_webpage:
-                favicon_elem = next(iter_favicon_elems(tree), None)
-                icon = favicon_elem.attrib.get('href', '') if favicon_elem is not None else ''
-                meta['icon'] = icon
-            else:
-                meta['icon'] = ''
+                try:
+                    favicon_elem = next(iter_favicon_elems(tree))
+                except StopIteration:
+                    pass
+                else:
+                    meta['icon'] = favicon_elem.attrib.get('href', '')
 
         generator = FavIconCacher(self.book, cache_archive=True)
         yield from generator.run([id])
 
-        # source
-        if meta['source'] is None:
-            meta['source'] = ''
-
-        # comment
-        if meta['comment'] is None:
-            meta['comment'] = ''
-
         return id
 
     def _handle_ie_meta(self, meta, root):
         doc_comment = root.getprevious()
 
         if doc_comment is None:
             return
@@ -395,19 +390,19 @@
             cache_file = yield from self._cache_favicon(id)
             if cache_file:
                 cached[id] = cache_file
 
         return cached
 
     def _cache_favicon(self, id):
-        yield Info('debug', f'Caching favicon for "{id}"...')
+        yield Info('debug', f'Caching favicon for {id!r}...')
 
         url = self.book.meta[id].get('icon')
         if not url:
-            yield Info('debug', f'Skipped for "{id}": no favicon to cache.')
+            yield Info('debug', f'Skipped for {id!r}: no favicon to cache.')
             return None
 
         urlparts = urlsplit(url)
 
         index = self.book.meta[id].get('index', '')
 
         # absolute URL
@@ -439,58 +434,50 @@
         return None
 
     def _cache_favicon_absolute_url(self, id, index, url, source_url=None):
         """cache absolute URL (also works for data URL)
         """
         def verify_mime(mime):
             if not mime:
-                yield Info('error', f'Unable to cache favicon "{util.crop(source_url, 256)}" for "{id}": unknown MIME type')
+                yield Info('error', f'Unable to cache favicon {util.crop(source_url, 256)!r} for {id!r}: unknown MIME type')
                 return False
 
             if not (mime.startswith('image/') or mime == 'application/octet-stream'):
-                yield Info('error', f'Unable to cache favicon "{util.crop(source_url, 256)}" for "{id}": invalid image MIME type "{mime}"')
+                yield Info('error', f'Unable to cache favicon {util.crop(source_url, 256)!r} for {id!r}: invalid image MIME type {mime!r}')
                 return False
 
             return True
 
-        def cache_fh(fh):
-            fsrc = io.BytesIO()
-            while True:
-                chunk = fh.read(8192)
-                if not chunk:
-                    break
-                fsrc.write(chunk)
-
-            fsrc.seek(0)
+        def cache_fh(fsrc):
             hash_ = util.checksum(fsrc)
             ext = mime_to_extension(mime)
             fdst = os.path.join(self.book.tree_dir, 'favicon', hash_ + ext)
 
             if os.path.isfile(fdst):
-                yield Info('info', f'Use saved favicon for "{util.crop(source_url, 256)}" for "{id}" at "{self.book.get_subpath(fdst)}".')
+                yield Info('info', f'Use saved favicon for {util.crop(source_url, 256)!r} for {id!r} at {self.book.get_subpath(fdst)!r}.')
                 return fdst
 
-            yield Info('info', f'Saving favicon "{util.crop(source_url, 256)}" for "{id}" at "{self.book.get_subpath(fdst)}".')
+            yield Info('info', f'Saving favicon {util.crop(source_url, 256)!r} for {id!r} at {self.book.get_subpath(fdst)!r}.')
             fsrc.seek(0)
             os.makedirs(os.path.dirname(fdst), exist_ok=True)
             self.book.backup(fdst)
             with open(fdst, 'wb') as fw:
                 shutil.copyfileobj(fsrc, fw)
             return fdst
 
         if source_url is None:
             source_url = url
 
         try:
             r = urlopen(url)
         except URLError as exc:
-            yield Info('error', f'Unable to cache favicon "{util.crop(source_url, 256)}" for "{id}": unable to fetch favicon URL.', exc=exc)
+            yield Info('error', f'Unable to cache favicon {util.crop(source_url, 256)!r} for {id!r}: unable to fetch favicon URL.', exc=exc)
             return None
         except ValueError as exc:
-            yield Info('error', f'Unable to cache favicon "{util.crop(source_url, 256)}" for "{id}": unsupported or malformatted URL: {exc}', exc=exc)
+            yield Info('error', f'Unable to cache favicon {util.crop(source_url, 256)!r} for {id!r}: unsupported or malformatted URL: {exc}', exc=exc)
             return None
 
         with r as r:
             mime, _ = util.parse_content_type(r.info()['content-type'])
             if not (yield from verify_mime(mime)):
                 return None
 
@@ -522,36 +509,36 @@
 
             try:
                 with zipfile.ZipFile(file) as zh:
                     bytes_ = zh.read(subpath)
             except OSError as exc:
                 raise RuntimeError(exc.strerror) from exc
         except Exception as exc:
-            yield Info('error', f'Failed to read archive favicon "{util.crop(url, 256)}" for "{id}": {exc}', exc=exc)
+            yield Info('error', f'Failed to read archive favicon {util.crop(url, 256)!r} for {id!r}: {exc}', exc=exc)
             return None
 
         mime, _ = mimetypes.guess_type(subpath)
         mime = mime or 'application/octet-stream'
         return f'data:{mime};base64,{b64encode(bytes_).decode("ascii")}'
 
     def _get_file_favicon(self, id, index, url, subpath):
         """Convert relative favicon path to data URL.
         """
         file = os.path.normpath(os.path.join(self.book.data_dir, index, '..', subpath))
 
         # skip if already in favicon dir
         if os.path.normcase(file).startswith(self.favicon_dir):
-            yield Info('debug', f'Skipped favicon "{util.crop(url, 256)}" for "{id}": already in favicon folder')
+            yield Info('debug', f'Skipped favicon {util.crop(url, 256)!r} for {id!r}: already in favicon folder')
             return None
 
         try:
             with open(file, 'rb') as fh:
                 bytes_ = fh.read()
         except OSError as exc:
-            yield Info('error', f'Failed to read archive favicon "{util.crop(url, 256)}" for "{id}": {exc.strerror}', exc=exc)
+            yield Info('error', f'Failed to read archive favicon {util.crop(url, 256)!r} for {id!r}: {exc.strerror}', exc=exc)
 
         mime, _ = mimetypes.guess_type(subpath)
         mime = mime or 'application/octet-stream'
         return f'data:{mime};base64,{b64encode(bytes_).decode("ascii")}'
 
 
 class SingleHtmlConverter(HtmlRewriter):
```

### Comparing `webscrapbook-1.9.0/webscrapbook/server.py` & `webscrapbook-2.0.0b8/webscrapbook/server.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/locales/en/messages.py` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/en/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,22 +113,22 @@
   • comment: items whose comment contains the keyword.
   • tc: items whose title or comment contains the keyword.
   • tcc: items whose title, fulltext, or comment contains the keyword.
   • index: items whose index file path contains the keyword.
   • source: items whose source URL contains the keyword.
   • icon: items whose icon URL contains the keyword.
   • charset: items whose charset contains the keyword.
-  • create: items whose create time matches the condition. The time condition is an interval with 0-17 digits, followed by a minus sign optionally, and then followed by 0-17 digits. The two 17-digit numbers means the year (4 digits), month (01-12), day (01-31), hours (00-59), minutes (00-59), seconds (00-59), and milliseconds (000-999) in local datetime. Each omitted digit is assumed to be a “0”, except that “999...” is assumed if the end datetime is totally omitted. For example, “create:2014-2015” means since 2014 until 2015; “create:-201309” means before Sep 2013; and “create:20110825” means after Aug 25, 2011.
-  • modify: items whose modify time matches the condition. Time format is same as create.
+  • create: items whose create time matches the condition. Multiple values are “or”-connected. The time condition is an interval with 0-17 digits, followed by a minus sign optionally, and then followed by 0-17 digits. The two 17-digit numbers means the year (4 digits), month (01-12), day (01-31), hours (00-59), minutes (00-59), seconds (00-59), and milliseconds (000-999) in local datetime. Each omitted digit is assumed to be a “0”, except that “999...” is assumed if the end datetime is totally omitted. For example, “create:2014-2015” means since 2014 until 2015; “create:-201309” means before Sep 2013; and “create:20110825” means after Aug 25, 2011.
+  • modify: items whose modify time matches the condition. Multiple values are “or”-connected. Time format is same as create.
   • marked: marked items.
   • locked: locked items.
   • location: items with geolocation information.
   • file: items whose filename contains the keyword.
   • root: items under the item of ID. Multiple values are “or”-connected.
-  • book: items in the specific scrapbook (by name). Multiple values are “or”-connected.
+  • book: items in the specific scrapbook (by ID). Multiple values are “or”-connected.
   • sort: sort search results using the specific condition, which can be id, title, comment, file, content, source, type, create, or modify. For example, “sort:id -sort:modify” means sorting by ID in acending order and then sorting by modify time in descending order.
   • limit: set a limit on the search result number. For example, “limit:10” means showing the first 10 results, “limit:-20” means removing the last 20 results, and “limit:0” or “-limit:” means unsetting the limit."""
 cache_search_result = 'Found %length% results:'
 cache_search_result_named = '(%name%) Found %length% results:'
 cache_search_sort_last_created = 'Last Created'
 cache_search_sort_last_modified = 'Last Modified'
 cache_search_sort_title = 'Sort by title'
```

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/locales/es/messages.py` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/es/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,22 +113,22 @@
    • comment: elementos cuyo comentario contiene la palabra clave.
    • tc: artículos cuyo título o comentario contiene la palabra clave.
    • tcc: elementos cuyo título, texto completo o comentario contiene la palabra clave.
    • index: elementos cuya ruta de archivo de índice contiene la palabra clave.
    • source: elementos cuya URL fuente contiene la palabra clave.
    • icon: elementos cuyo icono URL contiene la palabra clave.
    • charset: elementos cuyo juego de caracteres contiene la palabra clave.
-   • create: elementos cuyo tiempo de creación coincide con la condición. La condición de tiempo es un intervalo con 0-17 dígitos, seguido de un signo menos opcionalmente, y luego seguido de 0-17 dígitos. Los dos números de 17 dígitos significan el año (4 dígitos), mes (01-12), día (01-31), horas (00-59), minutos (00-59), segundos (00-59) y milisegundos (000-999) en fecha y hora local. Se supone que cada dígito omitido es un "0", excepto que se asume "999..." si se omite totalmente la fecha y hora de finalización. Por ejemplo, “create:2014-2015” significa desde 2014 hasta 2015; “create:-201309” significa antes de septiembre de 2013; y “create:20110825” significa después del 25 de agosto de 2011.
-   • modify: elementos cuyo tiempo de modificación coincide con la condición. El formato de hora es el mismo que crear.
+   • create: elementos cuyo tiempo de creación coincide con la condición. Múltiples valores están conectados “or”. La condición de tiempo es un intervalo con 0-17 dígitos, seguido de un signo menos opcionalmente, y luego seguido de 0-17 dígitos. Los dos números de 17 dígitos significan el año (4 dígitos), mes (01-12), día (01-31), horas (00-59), minutos (00-59), segundos (00-59) y milisegundos (000-999) en fecha y hora local. Se supone que cada dígito omitido es un "0", excepto que se asume "999..." si se omite totalmente la fecha y hora de finalización. Por ejemplo, “create:2014-2015” significa desde 2014 hasta 2015; “create:-201309” significa antes de septiembre de 2013; y “create:20110825” significa después del 25 de agosto de 2011.
+   • modify: elementos cuyo tiempo de modificación coincide con la condición. Múltiples valores están conectados “or”. El formato de hora es el mismo que crear.
    • marked: elementos marcados.
    • locked: elementos bloqueados.
    • location: artículos con información de geolocalización.
    • file: elementos cuyo nombre de archivo contiene la palabra clave.
    • root: elementos bajo el elemento de ID. Múltiples valores están conectados “or”.
-   • book: artículos en el álbum de recortes específico (por nombre). Múltiples valores están conectados “or”.
+   • book: artículos en el álbum de recortes específico (por ID). Múltiples valores están conectados “or”.
    • sort: ordenar los resultados de la búsqueda usando la condición específica, que puede ser id, title, comment, file, content, source, type, create o modify. Por ejemplo, “sort:id -sort:modify” significa ordenar por ID en orden ascendente y luego ordenar por tiempo de modificación en orden descendente.
    • limit: establece un límite en el número de resultados de búsqueda. Por ejemplo, “limit:10” significa mostrar los primeros 10 resultados, “limit:-20” significa eliminar los últimos 20 resultados y “limit:0” o “-limit:” significa anular el límite."""
 cache_search_result = 'Encontrado %length% resultados:'
 cache_search_result_named = '(%name%) Encontrado %length% resultados:'
 cache_search_sort_last_created = 'Última creación'
 cache_search_sort_last_modified = 'Última modificación'
 cache_search_sort_title = 'Ordenar por título'
```

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/locales/zh/messages.py` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/zh/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,22 +113,22 @@
   • comment：搜尋評註含有關鍵詞的項目。
   • tc：搜尋標題或評註含有關鍵詞的項目。
   • tcc：搜尋標題、全文或評註含有關鍵詞的項目。
   • index：搜尋索引檔含有關鍵詞的項目。
   • source：搜尋原始網址含有關鍵詞的項目。
   • icon：搜尋圖示網址含有關鍵詞的項目。
   • charset：搜尋字集含有關鍵詞的項目。
-  • create：搜尋建立時間符合條件的項目。時間格式為 0-17 位數字，後面接負號（可略），再接 0-17 位數字，表示時間範圍的起始與結束。兩個 17 位數字表示本地時間的年（4 位數）、月（01-12）、日（01-31）、時（00-59）、分（00-59）、秒（00-59）、毫秒（000-999），省略的部分視為 0，唯結束時間全省略時視為「999...」。例如「create:2014-2015」表示 2014 年到 2015 年，「create:-201309」表示 2013 年九月以前，「create:20110825」表示 2011 年八月 25 日以後。
-  • modify：搜尋修改時間符合條件的項目。時間格式同 create。
+  • create：搜尋建立時間符合條件的項目。多次指定時以「或」連接。時間格式為 0-17 位數字，後面接負號（可略），再接 0-17 位數字，表示時間範圍的起始與結束。兩個 17 位數字表示本地時間的年（4 位數）、月（01-12）、日（01-31）、時（00-59）、分（00-59）、秒（00-59）、毫秒（000-999），省略的部分視為 0，唯結束時間全省略時視為「999...」。例如「create:2014-2015」表示 2014 年到 2015 年，「create:-201309」表示 2013 年九月以前，「create:20110825」表示 2011 年八月 25 日以後。
+  • modify：搜尋修改時間符合條件的項目。多次指定時以「或」連接。時間格式同 create。
   • marked：搜尋強調標示的項目。
   • locked：搜尋鎖定的項目。
   • location：搜尋含有地理位置資訊的項目。
   • file：搜尋檔名含有關鍵詞的項目。
   • root：搜尋此 ID 項目下的子項目。多次指定時以「或」連接。
-  • book：搜尋指定剪貼簿（依名稱）中的項目。多次指定時以「或」連接。
+  • book：搜尋指定剪貼簿（依 ID）中的項目。多次指定時以「或」連接。
   • sort：將搜尋結果按指定方式排序，負號表示倒序。可填入 id、title、comment、file、content、source、type、create、modify。例如「sort:id -sort:modify」表示先按 ID 遞增排序再按修改時間遞減排序。
   • limit：設定搜尋結果筆數限制。例如「limit:10」表示只呈現前 10 筆搜尋結果，「limit:-20」表示不呈現最後 20 筆搜尋結果，「limit:0」或「-limit:」表示移除之前設定的限制。"""
 cache_search_result = '找到 %length% 筆結果：'
 cache_search_result_named = '(%name%) 找到 %length% 筆結果：'
 cache_search_sort_last_created = '最後建立'
 cache_search_sort_last_modified = '最後修改'
 cache_search_sort_title = '標題排序'
```

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/locales/zh_cn/messages.py` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/locales/zh_cn/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,22 +113,22 @@
   • comment：搜索评注含有关键词的项目。
   • tc：搜索标题或评注含有关键词的项目。
   • tcc：搜索标题、全文或评注含有关键词的项目。
   • index：搜索索引文件含有关键词的项目。
   • source：搜索原始网址含有关键词的项目。
   • icon：搜索图示网址含有关键词的项目。
   • charset：搜索字元集含有关键词的项目。
-  • create：搜索建立时间匹配条件的项目。时间格式为 0-17 位数字，后面接负号（可略），再接 0-17 位数字，表示时间范围的起始与结束。两个 17 位数字表示本地时间的年（4 位数）、月（01-12）、日（01-31）、时（00-59）、分（00-59）、秒（00-59）、毫秒（000-999），省略的部分视为补 0，唯结束时间全省略时视为“999...”。例如“create:2014-2015”表示 2014 年到 2015 年，“create:-201309”表示 2013 年九月以前，“create:20110825”表示 2011 年八月 25 日以后。
-  • modify：搜索修改时间匹配条件的项目。时间格式同 create。
+  • create：搜索建立时间匹配条件的项目。多次指定时以“或”连接。时间格式为 0-17 位数字，后面接负号（可略），再接 0-17 位数字，表示时间范围的起始与结束。两个 17 位数字表示本地时间的年（4 位数）、月（01-12）、日（01-31）、时（00-59）、分（00-59）、秒（00-59）、毫秒（000-999），省略的部分视为补 0，唯结束时间全省略时视为“999...”。例如“create:2014-2015”表示 2014 年到 2015 年，“create:-201309”表示 2013 年九月以前，“create:20110825”表示 2011 年八月 25 日以后。
+  • modify：搜索修改时间匹配条件的项目。多次指定时以“或”连接。时间格式同 create。
   • marked：搜索强调标示的项目。
   • locked：搜索锁定的项目。
   • location：搜索含有地理位置信息的项目。
   • file：搜索文件名含有关键词的项目。
   • root：搜索此 ID 项目下的子项目。多次指定时以“或”连接。
-  • book：搜索指定剪贴簿（依名称）中的项目。多次指定时以“或”连接。
+  • book：搜索指定剪贴簿（依 ID）中的项目。多次指定时以“或”连接。
   • sort：将搜索结果按指定方式排序，负号表示倒序。可填入 id、title、comment、file、content、source、type、create、modify。例如“sort:id -sort:modify”表示先按 ID 递增排序再按修改时间递减排序。
   • limit：设置搜索结果笔数限制。例如“limit:10”表示只呈现前 10 笔搜索结果，“limit:-20”表示不呈现最后 20 笔搜索结果，“limit:0”或“-limit:”表示移除之前设置的限制。"""
 cache_search_result = '找到 %length% 笔结果：'
 cache_search_result_named = '(%name%) 找到 %length% 笔结果：'
 cache_search_sort_last_created = '最后创建'
 cache_search_sort_last_modified = '最后修改'
 cache_search_sort_title = '标题排序'
```

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/comment.png` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/comment.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/common.css` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/common.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/common.js` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/common.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -127,25 +127,15 @@
     getTargetUrl(url) {
         const u = new URL(url || document.location.href);
         u.search = u.hash = '';
         return u.href;
     },
 
     async acquireToken(url) {
-        let xhr;
-        try {
-            xhr = await utils.xhr({
-                url: url + '?a=token&f=json',
-                responseType: 'json',
-                method: "POST",
-            });
-        } catch (ex) {
-            throw new Error('Unable to connect to backend server.');
-        }
-
-        if (!(xhr.response && xhr.response.success)) {
-            throw new Error('Unable to acquire an access token.');
-        }
-
+        const xhr = await this.wsb({
+            url: url + '?a=token&f=json',
+            responseType: 'json',
+            method: "POST",
+        });
         return xhr.response.data;
     },
 };
```

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/edit.css` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/edit.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/edit.js` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/edit.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/editx.js` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/editx.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/external.png` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/external.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/fclose.png` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/fclose.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/fopen.png` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/fopen.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/index-ex.css` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index-ex.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/index-ex.js` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index-ex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1811,14 +1811,31 @@
             let newDir = prompt(utils.lang('command_move_prompt_multi'), dir);
             if (!newDir) {
                 return;
             }
 
             newDir = newDir.replace(/\/+$/, '') + '/';
 
+            // create the target directory
+            try {
+                const target = location.origin + (base + newDir).split('/').map(x => encodeURIComponent(x)).join('/');
+                const formData = new FormData();
+                formData.append('token', await utils.acquireToken(target));
+
+                await utils.wsb({
+                    url: target + '?a=mkdir&f=json',
+                    responseType: 'json',
+                    method: "POST",
+                    formData: formData,
+                });
+            } catch (ex) {
+                alert(`Unable to move to "${newDir}": ${ex.message}`);
+                return;
+            }
+
             const entries = Array.prototype.map.call(selectedEntries, entry => {
                 const oldPath = dir + entry.dataset.path;
                 const newPath = newDir + oldPath.replace(/^.*\//, '');
                 return {
                     oldPath,
                     newPath
                 };
@@ -1826,15 +1843,15 @@
             const errors = [];
             for (const {
                     oldPath,
                     newPath
                 }
                 of entries.sort(onCommandRun.sortEntries).reverse()) {
                 try {
-                    await moveEntry(oldPath, newPath);
+                    await moveEntry(oldPath, newDir);
                 } catch (ex) {
                     errors.push(`"${oldPath}" => "${newPath}": ${ex.message}`);
                 }
             }
             if (errors.length) {
                 const msg = 'Unable to move entries:\n' + errors.reverse().join('\n');
                 alert(msg);
@@ -1880,14 +1897,31 @@
             let newDir = prompt(utils.lang('command_copy_prompt_multi'), dir);
             if (!newDir) {
                 return;
             }
 
             newDir = newDir.replace(/\/+$/, '') + '/';
 
+            // create the target directory
+            try {
+                const target = location.origin + (base + newDir).split('/').map(x => encodeURIComponent(x)).join('/');
+                const formData = new FormData();
+                formData.append('token', await utils.acquireToken(target));
+
+                await utils.wsb({
+                    url: target + '?a=mkdir&f=json',
+                    responseType: 'json',
+                    method: "POST",
+                    formData: formData,
+                });
+            } catch (ex) {
+                alert(`Unable to move to "${newDir}": ${ex.message}`);
+                return;
+            }
+
             const entries = Array.prototype.map.call(selectedEntries, entry => {
                 const oldPath = dir + entry.dataset.path;
                 const newPath = newDir + oldPath.replace(/^.*\//, '');
                 return {
                     oldPath,
                     newPath
                 };
@@ -1895,15 +1929,15 @@
             const errors = [];
             for (const {
                     oldPath,
                     newPath
                 }
                 of entries.sort(onCommandRun.sortEntries).reverse()) {
                 try {
-                    await copyEntry(oldPath, newPath);
+                    await copyEntry(oldPath, newDir);
                 } catch (ex) {
                     errors.push(`"${oldPath}" => "${newPath}": ${ex.message}`);
                 }
             }
             if (errors.length) {
                 const msg = 'Unable to copy entries:\n' + errors.reverse().join('\n');
                 alert(msg);
```

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/index.css` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/index.js` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/index.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/postit.png` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/postit.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/search.png` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/search.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/static/toggle.png` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/static/toggle.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/templates/cli.html` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/cli.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/templates/edit.html` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/edit.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/templates/editx.html` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/editx.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/templates/index.html` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/index.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_frame.html` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_frame.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_index.html` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_index.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_map.html` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_map.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_search.html` & `webscrapbook-2.0.0b8/webscrapbook/themes/default/templates/static_search.html`

 * *Files 0% similar despite different names*

```diff
@@ -136,23 +136,23 @@
 .scrapbook-marked > div > a {
   font-weight: bold;
 }
 </style>
 <link rel="stylesheet" href="search.css">
 <script>
 const conf = {
-  scrapbooks: [
-    {
-      name: "",
+  scrapbooks: {
+    '': {
+      name: {{ bookname | tojson }},
       path: {{ path | tojson }},
       dataDir: {{ data_dir | tojson }},
       treeDir: {{ tree_dir | tojson }},
       indexPage: {{ index | tojson }}
-    }
-  ],
+    },
+  },
   allowHttp: 0,  // whether to load js cache from HTTP(S)? -1: deny, 0: ask; 1: allow
   defaultSearch: "-type:folder -type:separator",  // the constant string to add before the input keyword
   viewInMapTitle: {{ i18n('cache_search_view_in_map') | tojson }},  // title for "view in map"
 };
 
 const scrapbook = {
   books: [],
@@ -178,37 +178,38 @@
     });
  
     document.getElementById('helper').addEventListener('change', (event) => {
       event.preventDefault();
       this.helperFill();
     });
 
-    scrapbook.books = conf.scrapbooks.map(
-      book => Object.assign({}, book, {
+    this.books = Object.entries(conf.scrapbooks).map(
+      ([id, book]) => Object.assign(book, {
+      	id,
         toc: {},
         meta: {},
         fulltext: {},
       })
     );
 
     return this.loadBooks().then(() => {
       document.getElementById('search').disabled = false;
     });
   },
 
   loadBooks() {
     let p = Promise.resolve();
-    scrapbook.books.forEach((book) => {
+    for (const book of this.books) {
       p = p.then(() => {
         return this.loadBook(book);
       }).catch((ex) => {
         console.error(ex);
         this.addMsg("Error: " + ex.message);
       });
-    });
+    }
     return p;
   },
 
   loadBook(book) {
     return Promise.resolve().then(() => {
       let base = this.resolveUrl(book.path, location.href);
 
@@ -341,15 +342,15 @@
   showResults(results, book) {
     const info = {
       "": "%",
       name: book.name,
       length: results.length,
     };
 
-    if (book.name) {
+    if (book.id) {
       this.addMsg(this.formatString({{ i18n('cache_search_result_named') | tojson }}, info));
     } else {
       this.addMsg(this.formatString({{ i18n('cache_search_result') | tojson }}, info));
     }
 
     const wrapper = document.getElementById("result");
     for (const item of results) {
@@ -489,15 +490,15 @@
   },
 
   parseQuery(queryStr) {
     const query = {
       error: [],
       rules: {},
       sorts: [],
-      limit: null,
+      limit: 0,
       books: {
         include: [],
         exclude: [],
       },
       roots: {
         include: [],
         exclude: [],
@@ -518,29 +519,35 @@
       switch (key) {
         case "id": case "file":
           query.sorts.push({key, order});
           break;
         case "content":
           query.sorts.push({key: "fulltext", subkey: key, order});
           break;
-        default:
+        case "title": case "comment": case "source":
+        case "type": case "create": case "modify":
           query.sorts.push({key: "meta", subkey: key, order});
           break;
+        default:
+          addError("Invalid sort: " + key);
+          break;
       }
     };
 
     const setLimit = (value, positive) => {
       if (!positive) {
-        query.limit = null;
+        query.limit = 0;
         return; 
       }
 
-      const newValue = parseInt(value);
-      if (!Number.isNaN(newValue)) {
+      const newValue = parseInt(value, 10);
+      if (Number.isInteger(newValue)) {
         query.limit = newValue;
+      } else {
+        addError("Invalid limit: " + value);
       }
     };
 
     const addError = (msg) => {
       query.error.push(msg);
     };
 
@@ -674,24 +681,24 @@
 
       return "";
     });
     return query;
   },
 
   search(query) {
-    const books = new Set(scrapbook.books);
-    if (query.books.include.length) {
-      for (const book of books) {
-        if (!query.books.include.includes(book.name)) {
-          books.delete(book);
-        }
-      }
-    }
+  	let books = new Set(scrapbook.books);
+  	if (query.books.include.length) {
+  	  books = new Set(
+        query.books.include
+          .map(id => conf.scrapbooks[id])
+          .filter(book => books.has(book))
+      );
+  	}
     for (const book of books) {
-      if (query.books.exclude.includes(book.name)) {
+      if (query.books.exclude.includes(book.id)) {
         books.delete(book);
       }
     }
 
     let p = Promise.resolve();
     books.forEach((book) => {
       p = p.then(() => {
@@ -840,19 +847,19 @@
   },
 
   _match_type(rule, item) {
     return this.matchTextOr(rule, item.meta.type);
   },
 
   _match_create(rule, item) {
-    return this.matchDate(rule, item.meta.create);
+    return this.matchDateOr(rule, item.meta.create);
   },
 
   _match_modify(rule, item) {
-    return this.matchDate(rule, item.meta.modify);
+    return this.matchDateOr(rule, item.meta.modify);
   },
 
   _match_marked(rule, item) {
     return this.matchBool(rule, item.meta.marked);
   },
 
   _match_locked(rule, item) {
@@ -911,30 +918,31 @@
       if (key.test(text)) {
         return true;
       }
     }
     return false;
   },
 
-  matchDate(rule, date) {
+  matchDateOr(rule, date) {
     if (!date) { return false; }
 
     for (const key of rule.exclude) {
       if (key[0] <= date && date <= key[1]) {
         return false;
       }
     }
 
+    if (!rule.include.length) { return true; }
     for (const key of rule.include) {
-      if (!(key[0] <= date && date <= key[1])) {
-        return false;
+      if (key[0] <= date && date <= key[1]) {
+        return true;
       }
     }
 
-    return true;
+    return false;
   },
 
   idLocalToUtc(id) {
     if (/^(\d{4})(\d{2})(\d{2})(\d{2})(\d{2})(\d{2})(\d{3})$/.test(id)) {
       const dd = new Date(
           parseInt(RegExp.$1, 10), Math.max(parseInt(RegExp.$2, 10), 1) - 1, Math.max(parseInt(RegExp.$3, 10), 1),
           parseInt(RegExp.$4, 10), parseInt(RegExp.$5, 10), parseInt(RegExp.$6, 10), parseInt(RegExp.$7, 10)
@@ -995,12 +1003,12 @@
 <details id="help">
 <summary>{{ i18n('cache_search_help_label') }}</summary>
 <div>{{ i18n('cache_search_help_desc') }}</div>
 </details>
 <ul id="result"></ul>
 </div>
 <div id="support">
-Supported browsers: Chromium ≥ 49, Firefox ≥ 41, Edge ≥ 14, Safari ≥ 8, with JavaScript enabled.
+Supported browsers: Firefox ≥ 52、Chrome ≥ 55、Safari ≥ 10.1、Opera ≥ 42、Edge ≥ 15, with JavaScript enabled.
 </div>
 <script>scrapbook.init();</script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -23,9 +23,9 @@
 {{ i18n('cache_search_sort_last_modified') }}
 {{ i18n('cache_search_sort_last_created') }}
 {{ i18n('cache_search_sort_title') }}
 {{ i18n('cache_search_sort_id') }}
  [{{ i18n('cache_search_start') }}]
  {{ i18n('cache_search_help_label') }}
 {{ i18n('cache_search_help_desc') }}
-Supported browsers: Chromium â¥ 49, Firefox â¥ 41, Edge â¥ 14, Safari â¥ 8,
-with JavaScript enabled.
+Supported browsers: Firefox â¥ 52ãChrome â¥ 55ãSafari â¥ 10.1ãOpera
+â¥ 42ãEdge â¥ 15, with JavaScript enabled.
```

### Comparing `webscrapbook-1.9.0/webscrapbook/util/html.py` & `webscrapbook-2.0.0b8/webscrapbook/util/html.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.9.0/webscrapbook/util/util.py` & `webscrapbook-2.0.0b8/webscrapbook/util/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,38 @@
 """Miscellaneous utilities
 """
 import binascii
 import codecs
-import collections
 import hashlib
 import importlib
 import math
-import mimetypes
 import os
 import re
-import shutil
-import stat
-import subprocess
 import sys
-import tempfile
-import time
-import zipfile
 from base64 import b64decode
 from collections import namedtuple
 from contextlib import nullcontext
 from datetime import datetime, timezone
 from ipaddress import AddressValueError, IPv6Address
 from urllib.parse import quote, unquote_to_bytes, urljoin, urlsplit
 from urllib.request import pathname2url, url2pathname
 
 import lxml.html
 from lxml import etree
 
+from .._polyfill import mimetypes, zipfile
+
 #########################################################################
 # Common classes and objects handling
 #########################################################################
 
 # common namedtuple for yielded messages for certain classes
 Info = namedtuple('Info', ('type', 'msg', 'data', 'exc'), defaults=(None, None))
 
 
-class frozendict(collections.abc.Mapping):  # noqa: N801
-    """Implementation of a frozen dict, which is hashable if all values
-       are hashable.
-    """
-    def __init__(self, *args, **kwargs):
-        self._d = dict(*args, **kwargs)
-        self._hash = None
-
-    def __repr__(self):
-        return f'{type(self).__name__}({self._d.__repr__()})'
-
-    def __iter__(self):
-        return iter(self._d)
-
-    def __len__(self):
-        return len(self._d)
-
-    def __getitem__(self, key):
-        return self._d[key]
-
-    def __reversed__(self):
-        try:
-            return reversed(self._d)
-        except TypeError:
-            # reversed(dict) not supported in Python < 3.8
-            # shim via reversing a list
-            return reversed(list(self._d))
-
-    def __hash__(self):
-        if self._hash is None:
-            self._hash = hash(frozenset(self.items()))
-        return self._hash
-
-    def copy(self):
-        return self.__class__(self._d.copy())
-
-
-def make_hashable(obj):
-    if isinstance(obj, collections.abc.Hashable):
-        return obj
-
-    if isinstance(obj, collections.abc.Set):
-        return frozenset(make_hashable(v) for v in obj)
-
-    if isinstance(obj, collections.abc.Sequence):
-        return tuple(make_hashable(v) for v in obj)
-
-    if isinstance(obj, collections.abc.Mapping):
-        return frozendict((k, make_hashable(v)) for k, v in obj.items())
-
-    raise TypeError(f"unable to make '{type(obj).__name__}' hashable")
-
-
 def import_module_file(ns, file):
     try:
         return sys.modules[ns]
     except KeyError:
         pass
 
     spec = importlib.util.spec_from_file_location(ns, file)
@@ -187,14 +128,21 @@
                 int(ms),
             )
         except ValueError:
             pass
     return None
 
 
+def unify_pathsep(text):
+    """Convert non-standard path separators to '/'."""
+    if os.sep != '/':
+        return text.replace(os.sep, '/')
+    return text
+
+
 def validate_filename(filename, force_ascii=False):
     """Transliterates the given string to be a safe filename
 
     See also: scrapbook.validateFilename of WebScrapBook.
     """
     fn = filename
 
@@ -226,18 +174,22 @@
     return fn
 
 
 #########################################################################
 # String handling
 #########################################################################
 
-def crop(text, width=70, ellipsis='...'):
+def cropped(text, width=70, ellipsis='...'):
     if len(text) > width:
-        return text[:max(width - len(ellipsis), 0)] + ellipsis
-    return text
+        return (text[:max(width - len(ellipsis), 0)], ellipsis)
+    return (text, '')
+
+
+def crop(text, width=70, ellipsis='...'):
+    return ''.join(cropped(text, width, ellipsis))
 
 
 REGEX_FORMAT_STRING = re.compile(r'%(\w*)%')
 
 
 def format_string(text, mapping):
     """A very simple implementation for string formatting with placeholders.
@@ -608,48 +560,14 @@
     return pathname2url(rel_path)  # this quotes URL
 
 
 #########################################################################
 # Filesystem related manipulation
 #########################################################################
 
-FileInfo = namedtuple('FileInfo', ('name', 'type', 'size', 'last_modified'))
-
-
-def launch(path):
-    """Launch a file or open a directory in the explorer.
-    """
-    if sys.platform == 'win32':
-        os.startfile(path)
-    elif sys.platform == 'darwin':
-        subprocess.run(['open', path])
-    else:
-        subprocess.run(['xdg-open', path])
-
-
-def view_in_explorer(path):
-    """Open the parent directory of a file or directory
-       in the explorer.
-    """
-    if sys.platform == 'win32':
-        subprocess.run(['explorer', '/select,', path])
-    elif sys.platform == 'darwin':
-        try:
-            subprocess.run(['open', '-R', path])
-        except OSError:
-            # fallback for older OS X
-            launch(os.path.dirname(path))
-    else:
-        try:
-            subprocess.run(['nautilus', '--select', path])
-        except OSError:
-            # fallback if no nautilus
-            launch(os.path.dirname(path))
-
-
 def checksum(file, method='sha1', chunk_size=4096):
     """Calculate the checksum of a file.
 
     Args:
         file: str, path-like, or file-like bytes object
     """
     try:
@@ -667,98 +585,15 @@
 
         return h.hexdigest()
     finally:
         if fh != file:
             fh.close()
 
 
-def file_is_link(path, st=None):
-    """Check if a path is a symlink or Windows directory junction
-
-    Args:
-        st: known stat for the path for better performance
-    """
-    if st is None:
-        try:
-            st = os.lstat(path)
-        except (OSError, ValueError, AttributeError):
-            return False
-
-    if os.name == 'nt':
-        if st.st_file_attributes & stat.FILE_ATTRIBUTE_REPARSE_POINT:
-            # this is True for symlink or directory junction
-            return True
-
-    return stat.S_ISLNK(st.st_mode)
-
-
-def file_info(file, base=None):
-    """Read basic file information.
-    """
-    if base is None:
-        name = os.path.basename(file)
-    else:
-        name = file[len(base) + 1:].replace('\\', '/')
-
-    try:
-        statinfo = os.lstat(file)
-    except OSError:
-        # unexpected error when getting stat info
-        statinfo = None
-        size = None
-        last_modified = None
-    else:
-        size = statinfo.st_size
-        last_modified = statinfo.st_mtime
-
-    if not os.path.lexists(file):
-        type = None
-    elif file_is_link(file, statinfo):
-        type = 'link'
-    elif os.path.isdir(file):
-        type = 'dir'
-    elif os.path.isfile(file):
-        type = 'file'
-    else:
-        type = 'unknown'
-
-    if type != 'file':
-        size = None
-
-    return FileInfo(name=name, type=type, size=size, last_modified=last_modified)
-
-
-def listdir(base, recursive=False):
-    """Generates FileInfo(s) and omit invalid entries.
-    """
-    if not recursive:
-        with os.scandir(base) as entries:
-            for entry in entries:
-                info = file_info(entry.path)
-                if info.type is None:
-                    continue
-                yield info
-
-    else:
-        for root, dirs, files in os.walk(base):
-            for dir in dirs:
-                file = os.path.join(root, dir)
-                info = file_info(file, base)
-                if info.type is None:
-                    continue
-                yield info
-            for file in files:
-                file = os.path.join(root, file)
-                info = file_info(file, base)
-                if info.type is None:
-                    continue
-                yield info
-
-
-def format_filesize(bytes, si=False):
+def format_filesize(bytes, si=False, space=' '):
     """Convert file size from bytes to human readable presentation.
     """
     try:
         bytes = int(bytes)
     except (ValueError, TypeError):
         return ''
 
@@ -768,16 +603,16 @@
     else:
         thresh = 1024
         units = ['B', 'KB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB']
 
     e = math.floor(math.log(max(1, bytes)) / math.log(thresh))
     e = min(e, len(units) - 1)
     n = bytes / thresh ** e
-    tpl = '{:.1f}\xA0{}' if (e >= 1 and n < 10) else '{:.0f}\xA0{}'  # noqa: P103
-    return tpl.format(n, units[e])
+    tpl = '{:.1f}{}{}' if (e >= 1 and n < 10) else '{:.0f}{}{}'  # noqa: P103
+    return tpl.format(n, space, units[e])
 
 
 COMPRESSIBLE_TYPES = {
     'application/xml',
 
     # historical non-text/* javascript types
     # ref: https://mimesniff.spec.whatwg.org/
@@ -882,333 +717,14 @@
 
 def is_wsba(filename):
     mime, _ = mimetypes.guess_type(filename)
     return mime_is_wsba(mime)
 
 
 #########################################################################
-# ZIP handling
-#########################################################################
-
-class ZipDirNotFoundError(Exception):
-    pass
-
-
-def zip_fix_subpath(subpath):
-    """Fix subpath to fit ZIP format specification.
-    """
-    if os.sep != '/' and os.sep in subpath:
-        subpath = subpath.replace(os.sep, '/')
-    return subpath
-
-
-def zip_compression_params(mimetype=None, compress_type=None, compresslevel=None, autodetector=is_compressible):
-    """A helper for determining compress type and level.
-    """
-    if compress_type is None and compresslevel is None and autodetector is not None:
-        compressible = autodetector(mimetype)
-        compress_type = zipfile.ZIP_DEFLATED if compressible else zipfile.ZIP_STORED
-        compresslevel = 9 if compressible else None
-
-    return {
-        'compress_type': compress_type,
-        'compresslevel': compresslevel,
-    }
-
-
-def zip_tuple_timestamp(zipinfodate):
-    """Get timestamp from a ZipInfo.date_time.
-    """
-    return time.mktime(zipinfodate + (0, 0, -1))
-
-
-def zip_timestamp(zipinfo):
-    """Get timestamp from a ZipInfo.
-    """
-    return zip_tuple_timestamp(zipinfo.date_time)
-
-
-def zip_file_info(zip, subpath, base=None, check_implicit_dir=False):
-    """Read basic file information from ZIP.
-
-    Args:
-        zip: path, file-like object, or zipfile.ZipFile
-        subpath: 'dir' and 'dir/' are both supported
-    """
-    subpath = zip_fix_subpath(subpath)
-
-    subpath = subpath.rstrip('/')
-    if base is None:
-        name = os.path.basename(subpath)
-    else:
-        name = subpath[len(base):]
-
-    with nullcontext(zip) if isinstance(zip, zipfile.ZipFile) else zipfile.ZipFile(zip) as zh:
-        try:
-            info = zh.getinfo(subpath)
-        except KeyError:
-            pass
-        else:
-            return FileInfo(name=name, type='file', size=info.file_size, last_modified=zip_timestamp(info))
-
-        try:
-            info = zh.getinfo(subpath + '/')
-        except KeyError:
-            pass
-        else:
-            return FileInfo(name=name, type='dir', size=None, last_modified=zip_timestamp(info))
-
-        if check_implicit_dir:
-            base = subpath + ('/' if subpath else '')
-            for entry in zh.namelist():
-                if entry.startswith(base):
-                    return FileInfo(name=name, type='dir', size=None, last_modified=None)
-
-    return FileInfo(name=name, type=None, size=None, last_modified=None)
-
-
-def zip_listdir(zip, subpath, recursive=False):
-    """Generates FileInfo(s) and omit invalid entries.
-
-    Raise ZipDirNotFoundError if subpath does not exist.
-
-    NOTE: It is possible that entry mydir/ does not exist while mydir/foo.bar
-    exists. Check for matching subentries to make sure whether the implicit
-    directory exists.
-
-    Args:
-        zip: path, file-like object, or zipfile.ZipFile
-        subpath: the subpath in the ZIP, with or without trailing slash
-    """
-    subpath = zip_fix_subpath(subpath)
-
-    base = subpath.rstrip('/')
-    if base:
-        base += '/'
-    base_len = len(base)
-    dir_exist = not base
-    entries = {}
-
-    with nullcontext(zip) if isinstance(zip, zipfile.ZipFile) else zipfile.ZipFile(zip) as zh:
-        for filename in zh.namelist():
-            if not filename.startswith(base):
-                continue
-
-            if filename == base:
-                dir_exist = True
-                continue
-
-            entry = filename[base_len:]
-            if not recursive:
-                entry, _, _ = entry.partition('/')
-                entries.setdefault(entry, True)
-            else:
-                parts = entry.rstrip('/').split('/')
-                for i in range(0, len(parts)):
-                    entry = '/'.join(parts[0:i + 1])
-                    entries.setdefault(entry, True)
-
-        if not entries and not dir_exist:
-            raise ZipDirNotFoundError(f'Directory "{base}/" does not exist in the zip.')
-
-        for entry in entries:
-            info = zip_file_info(zh, base + entry, base)
-
-            if info.type is None:
-                yield FileInfo(name=entry, type='dir', size=None, last_modified=None)
-            else:
-                yield info
-
-
-def zip_has(zip, subpath, type='any'):
-    """Check if a directory or file exists in the ZIP.
-
-    NOTE: It is possible that entry mydir/ does not exist while mydir/foo.bar
-    exists. Check for matching subentries to make sure whether the implicit
-    directory exists.
-
-    Args:
-        zip: path, file-like object, or zipfile.ZipFile
-        subpath: the subpath in the ZIP, with or without trailing slash
-        type: 'dir', 'file', or 'any'
-    """
-    subpath = zip_fix_subpath(subpath)
-
-    if type not in ('dir', 'file', 'any'):
-        raise ValueError(f'Invalid type: "{type}"')
-
-    base = subpath.rstrip('/')
-    if base == '':
-        return True if type != 'file' else False
-
-    with nullcontext(zip) if isinstance(zip, zipfile.ZipFile) else zipfile.ZipFile(zip) as zh:
-        if type in ('file', 'any'):
-            try:
-                zh.getinfo(base)
-            except KeyError:
-                pass
-            else:
-                return True
-
-        base += '/'
-        if type in ('dir', 'any'):
-            try:
-                zh.getinfo(base + '/')
-            except KeyError:
-                pass
-            else:
-                return True
-
-            # check for an implicit directory
-            for path in zh.namelist():
-                if path.startswith(base):
-                    return True
-
-    return False
-
-
-def zip_compress(zip, filename, subpath, filter=None):
-    """Compress src to be the subpath in the zip.
-
-    Args:
-        zip: path, file-like object, or zipfile.ZipFile
-        filename: path of the source file or directory
-        subpath: internal path to a file or folder (without trailing slash)
-        filter: an iterable of permitted subentries if filename is a directory
-            (with normcase'd absolute path)
-
-    Raises:
-        shutil.Error: if any child file cannot be added to the zip
-    """
-    subpath = zip_fix_subpath(subpath)
-
-    filename = os.path.abspath(filename)
-    with nullcontext(zip) if isinstance(zip, zipfile.ZipFile) else zipfile.ZipFile(zip, 'w') as zh:
-        if os.path.isdir(filename):
-            errors = []
-
-            subpath = subpath + '/' if subpath else ''
-            src = filename
-            dst = subpath
-            if dst:
-                try:
-                    ts = time.localtime(os.stat(src).st_mtime)[:-3]
-                    zh.writestr(zipfile.ZipInfo(dst, ts), '')
-                except OSError as why:
-                    errors.append((src, dst, str(why)))
-
-            filter = {os.path.normcase(os.path.join(filename, f)) for f in (filter or [])}
-            filter_d = {os.path.join(f, '') for f in filter}
-
-            base_cut = len(os.path.join(filename, ''))
-            for root, dirs, files in os.walk(filename, followlinks=True):
-                for dir in dirs:
-                    src = os.path.join(root, dir)
-
-                    # apply the filter
-                    if filter:
-                        src_nc = os.path.normcase(src)
-                        if src_nc not in filter:
-                            if not any(src_nc.startswith(f) for f in filter_d):
-                                continue
-
-                    dst = src[base_cut:]
-                    if os.sep != '/':
-                        dst = dst.replace(os.sep, '/')
-                    dst = subpath + dst + '/'
-                    try:
-                        ts = time.localtime(os.stat(src).st_mtime)[:-3]
-                        zh.writestr(zipfile.ZipInfo(dst, ts), '')
-                    except OSError as why:
-                        errors.append((src, dst, str(why)))
-
-                for file in files:
-                    src = os.path.join(root, file)
-
-                    # apply the filter
-                    if filter:
-                        src_nc = os.path.normcase(src)
-                        if src_nc not in filter:
-                            if not any(src_nc.startswith(f) for f in filter_d):
-                                continue
-
-                    dst = src[base_cut:]
-                    if os.sep != '/':
-                        dst = dst.replace(os.sep, '/')
-                    dst = subpath + dst
-                    try:
-                        zh.write(src, dst, **zip_compression_params(mimetype=mimetypes.guess_type(dst)[0]))
-                    except OSError as why:
-                        errors.append((src, dst, str(why)))
-
-            if errors:
-                raise shutil.Error(errors)
-        else:
-            zh.write(filename, subpath, **zip_compression_params(mimetype=mimetypes.guess_type(subpath)[0]))
-
-
-def zip_extract(zip, dst, subpath='', tzoffset=None):
-    """Extract zip subpath to dst and preserve metadata.
-
-    Args:
-        zip: path, file-like object, or zipfile.ZipFile
-        dst: path where the extracted file or directory will be placed at.
-        subpath: internal path to a file or folder (without trailing slash), or
-            '' or None to extract the whole zip
-        tzoffset: known timezone offset (in seconds) the ZIP file has been
-            created at, to adjust mtime of the internal files, which are
-            recorded using local timestamp
-
-    Raises:
-        FileExistsError: if dst already exists
-    """
-    subpath = zip_fix_subpath(subpath)
-
-    if os.path.lexists(dst):
-        # trigger FileExistsError
-        os.mkdir(dst)
-
-    tempdir = tempfile.mkdtemp()
-    try:
-        with nullcontext(zip) if isinstance(zip, zipfile.ZipFile) else zipfile.ZipFile(zip) as zh:
-            if not subpath:
-                entries = zh.namelist()
-            else:
-                try:
-                    zh.getinfo(subpath)
-                except KeyError:
-                    entries = [e for e in zh.namelist() if e.startswith(subpath + '/')]
-                else:
-                    entries = [subpath]
-
-            # extract entries and keep datetime
-            zh.extractall(tempdir, entries)
-            for entry in entries:
-                file = os.path.join(tempdir, entry)
-                ts = zip_timestamp(zh.getinfo(entry))
-
-                if tzoffset is not None:
-                    delta = datetime.now().astimezone().utcoffset().total_seconds()
-                    ts = ts - tzoffset + delta
-
-                os.utime(file, (ts, ts))
-
-        # move to target path
-        if not subpath:
-            shutil.move(tempdir, dst)
-        else:
-            shutil.move(os.path.join(tempdir, subpath), dst)
-    finally:
-        try:
-            shutil.rmtree(tempdir)
-        except OSError:
-            pass
-
-
-#########################################################################
 # HTTP manipulation
 #########################################################################
 
 HEADER_OWS = r'[\t ]*'
 HEADER_TOKEN = r"[!#$%&'*+.0-9A-Z^_`a-z|~-]+"
 HEADER_QUOTED_STRING = r'(?:"[^"]*(?:\.[^"]*)*")'
 
@@ -1747,14 +1263,14 @@
     def plain(self, text, salt=''):
         return text + salt
 
     def encrypt(self, text, salt='', method='plain'):
         fn = getattr(self, method, None)
 
         if not callable(fn):
-            print(f'Encrypt method "{method}" not implemented, fallback to "plain".', file=sys.stderr)
+            print(f"Encrypt method {method!r} not implemented, fallback to 'plain'.", file=sys.stderr)
             fn = self.plain
 
         return fn(text, salt)
 
 
 encrypt = Encrypt().encrypt
```

### Comparing `webscrapbook-1.9.0/webscrapbook.egg-info/PKG-INFO` & `webscrapbook-2.0.0b8/webscrapbook.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: webscrapbook
-Version: 1.9.0
+Version: 2.0.0b8
 Summary: A backend toolkit for management of WebScrapBook collection.
 Home-page: https://github.com/danny0838/PyWebScrapBook
 Author: Danny Lin
 Author-email: danny0838@gmail.com
-License: MIT
+License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
@@ -72,18 +73,21 @@
         check (k)  check and fix scrapbook data
         export (x)
                    export data items into archive files (*.wsba)
         import (i)
                    import data items from archive files (*.wsba)
         convert (v)
                    convert scrapbook data between different formats
+        query (q)  perform queries on the scrapbook(s)
+        search (r)
+                   search for data items in the scrapbook(s)
         help       show detailed information about certain topics
         view       view archive file in the browser
 
-    optional arguments:
+    options:
       -h, --help   show this help message and exit
       --version    show version information and exit
       --root ROOT  root directory to manipulate (default: current working directory)
 
 Run `wsb <command> --help` for help about `<command>`. For example, `wsb config --help` for help about `wsb config`.
 
 ### Host a scrapbook
```

