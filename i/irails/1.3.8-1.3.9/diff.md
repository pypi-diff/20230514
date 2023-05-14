# Comparing `tmp/irails-1.3.8.tar.gz` & `tmp/irails-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.8.tar", last modified: Sat May 13 09:28:25 2023, max compression
+gzip compressed data, was "irails-1.3.9.tar", last modified: Sat May 13 15:05:32 2023, max compression
```

## Comparing `irails-1.3.8.tar` & `irails-1.3.9.tar`

### file list

```diff
@@ -1,88 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.886745 irails-1.3.8/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5315 2023-05-13 09:28:25.885760 irails-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     4532 2023-05-13 06:11:01.000000 irails-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.803318 irails-1.3.8/irails/
--rw-rw-rw-   0        0        0      306 2023-05-13 09:27:55.000000 irails-1.3.8/irails/__init__.py
--rw-rw-rw-   0        0        0     3409 2023-05-13 06:08:26.000000 irails-1.3.8/irails/_i18n.py
--rw-rw-rw-   0        0        0     2445 2023-05-11 15:39:57.000000 irails-1.3.8/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.3.8/irails/_utils.py
--rw-rw-rw-   0        0        0    11722 2023-05-11 15:21:25.000000 irails-1.3.8/irails/auth.py
--rw-rw-rw-   0        0        0    12426 2023-05-13 05:30:29.000000 irails-1.3.8/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.815967 irails-1.3.8/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.816964 irails-1.3.8/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.8/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.8/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.8/irails/cbv.py
--rw-rw-rw-   0        0        0     6065 2023-05-11 15:19:41.000000 irails-1.3.8/irails/config.py
--rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.8/irails/controller_utils.py
--rw-rw-rw-   0        0        0    32314 2023-05-13 09:22:45.000000 irails-1.3.8/irails/core.py
--rw-rw-rw-   0        0        0     6409 2023-05-11 15:21:34.000000 irails-1.3.8/irails/database.py
--rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.8/irails/log.py
--rw-rw-rw-   0        0        0     8673 2023-05-11 15:20:30.000000 irails-1.3.8/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.8/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9341 2023-05-11 15:20:39.000000 irails-1.3.8/irails/midware_session.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.3.8/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.829931 irails-1.3.8/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.8/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7811 2023-05-11 15:34:41.000000 irails-1.3.8/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.3.8/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7755 2023-05-13 05:57:18.000000 irails-1.3.8/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.8/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.8/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.8/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     1855 2023-05-11 12:33:17.000000 irails-1.3.8/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.757444 irails-1.3.8/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.843898 irails-1.3.8/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.8/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.8/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.8/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.8/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.3.8/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.3.8/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.3.8/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.8/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.846885 irails-1.3.8/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.8/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.847882 irails-1.3.8/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.8/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.861812 irails-1.3.8/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.8/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.8/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.8/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.8/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.8/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.8/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.8/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.8/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.8/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.760436 irails-1.3.8/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.865801 irails-1.3.8/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.8/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.8/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.8/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.8/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.869789 irails-1.3.8/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.8/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.8/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.872783 irails-1.3.8/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.765420 irails-1.3.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.876772 irails-1.3.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.881758 irails-1.3.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.8/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.8/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.767415 irails-1.3.8/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.882756 irails-1.3.8/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.8/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2887 2023-05-12 05:35:40.000000 irails-1.3.8/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-13 09:28:25.812975 irails-1.3.8/irails.egg-info/
--rw-rw-rw-   0        0        0     5315 2023-05-13 09:28:25.000000 irails-1.3.8/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2326 2023-05-13 09:28:25.000000 irails-1.3.8/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 09:28:25.000000 irails-1.3.8/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-13 09:28:25.000000 irails-1.3.8/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      777 2023-05-13 09:28:25.000000 irails-1.3.8/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-13 09:28:25.000000 irails-1.3.8/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 09:28:25.886745 irails-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.595268 irails-1.3.9/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5315 2023-05-13 15:05:32.593577 irails-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4532 2023-05-13 06:11:01.000000 irails-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.529375 irails-1.3.9/irails/
+-rw-rw-rw-   0        0        0      306 2023-05-13 15:05:29.000000 irails-1.3.9/irails/__init__.py
+-rw-rw-rw-   0        0        0     3409 2023-05-13 06:08:26.000000 irails-1.3.9/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2576 2023-05-13 14:48:27.000000 irails-1.3.9/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.3.9/irails/_utils.py
+-rw-rw-rw-   0        0        0    11802 2023-05-13 14:57:32.000000 irails-1.3.9/irails/auth.py
+-rw-rw-rw-   0        0        0    12679 2023-05-13 15:01:43.000000 irails-1.3.9/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.539350 irails-1.3.9/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.540345 irails-1.3.9/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.9/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.9/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.9/irails/cbv.py
+-rw-rw-rw-   0        0        0     6097 2023-05-13 14:54:50.000000 irails-1.3.9/irails/config.py
+-rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.9/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    32428 2023-05-13 14:55:43.000000 irails-1.3.9/irails/core.py
+-rw-rw-rw-   0        0        0     6409 2023-05-11 15:21:34.000000 irails-1.3.9/irails/database.py
+-rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.9/irails/log.py
+-rw-rw-rw-   0        0        0     8673 2023-05-11 15:20:30.000000 irails-1.3.9/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.9/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9341 2023-05-11 15:20:39.000000 irails-1.3.9/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.3.9/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.548324 irails-1.3.9/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.9/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.9/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7723 2023-05-13 13:51:38.000000 irails-1.3.9/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7755 2023-05-13 05:57:18.000000 irails-1.3.9/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.9/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.9/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.9/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     1333 2023-05-13 14:32:06.000000 irails-1.3.9/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2361 2023-05-13 14:26:41.000000 irails-1.3.9/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.495989 irails-1.3.9/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.559296 irails-1.3.9/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.9/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.9/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.9/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.9/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.3.9/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.3.9/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.9/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.9/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.561290 irails-1.3.9/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.9/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.562288 irails-1.3.9/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.9/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.574626 irails-1.3.9/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.9/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.9/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.9/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.9/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.9/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.9/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.9/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.9/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.9/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.498987 irails-1.3.9/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.577620 irails-1.3.9/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.9/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.9/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.9/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.9/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.579615 irails-1.3.9/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.9/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.9/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.581611 irails-1.3.9/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.502979 irails-1.3.9/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.585606 irails-1.3.9/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.9/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.589588 irails-1.3.9/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.9/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.9/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.9/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.504984 irails-1.3.9/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.591583 irails-1.3.9/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.9/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0      661 2023-05-13 14:34:53.000000 irails-1.3.9/irails/unit_test.py
+-rw-rw-rw-   0        0        0     2887 2023-05-12 05:35:40.000000 irails-1.3.9/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-13 15:05:32.536357 irails-1.3.9/irails.egg-info/
+-rw-rw-rw-   0        0        0     5315 2023-05-13 15:05:32.000000 irails-1.3.9/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2383 2023-05-13 15:05:32.000000 irails-1.3.9/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-13 15:05:32.000000 irails-1.3.9/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-13 15:05:32.000000 irails-1.3.9/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      777 2023-05-13 15:05:32.000000 irails-1.3.9/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-13 15:05:32.000000 irails-1.3.9/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-13 15:05:32.595268 irails-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.9/setup.py
```

### Comparing `irails-1.3.8/PKG-INFO` & `irails-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.8
+Version: 1.3.9
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.8/README.md` & `irails-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/_i18n.py` & `irails-1.3.9/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/_loader.py` & `irails-1.3.9/irails/_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import importlib
 import sys,os
 from .config import config,ROOT_PATH 
 from ._i18n import load_app_translations
 from gettext import gettext as _
-app_cfg=config.get('app')
-if app_cfg:
-    app_dirs = app_cfg.get("appdir")
-    app_enabled = app_cfg.get("enabled")
+
+app_dirs = []
+app_enabled = []
+
 
 def __list_directories(dir):
     """
     return all subdirectory under :dir
     """
     dirs_list = [] 
+
     for name in os.listdir(dir):
        
         path = os.path.join(dir,name)
         if os.path.isdir(path) and name!='__pycache__': 
             dirs_list.append(name)
     return dirs_list
 
@@ -48,23 +49,28 @@
                 _log.error(_("load app %s failed")%app_dir)
                 _log.error(e.args)
                 cnt -= 1
             else:
                 pass
     return cnt
 def _load_apps(debug=False):
-    
+    global app_dirs,app_enabled
+    app_cfg=config.get('app')
+    if app_cfg:
+        app_dirs = app_cfg.get("appdir")
+        app_enabled = app_cfg.get("enabled")
     unloaded = 0
     loaded = 0
     for app_dir in app_dirs:
-        app_list =  __list_directories(app_dir)
+        abs_app_dir=os.path.abspath(os.path.join(ROOT_PATH,app_dir))
+        app_list =  __list_directories(abs_app_dir)
         for app in app_list:
             if __check_if_enabled(app):  
-                _dir = os.path.join(app_dir,app)
-                _abs_app_path = os.path.dirname(os.path.abspath(_dir))
+                #_dir = os.path.join(app_dir,app)
+                _abs_app_path =  abs_app_dir
                 if _abs_app_path not in sys.path:
                     sys.path.insert(-1,_abs_app_path)
                 debug and print('load app:'+app)
                 n = _load_app(app)
                 if n:
                     loaded = loaded + 1
                 else:
```

### Comparing `irails-1.3.8/irails/_utils.py` & `irails-1.3.9/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/auth.py` & `irails-1.3.9/irails/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from starlette.authentication import AuthenticationBackend, AuthenticationError, SimpleUser, AuthCredentials,BaseUser
 from starlette.middleware.authentication import AuthenticationMiddleware
 from starlette.authentication import BaseUser,SimpleUser,UnauthenticatedUser
 from casbin.persist.adapters import FileAdapter
 from casbin.persist.adapter import Adapter
 # from .midware_casbin import CasbinMiddleware
  
-from .config import config
+from .config import config,ROOT_PATH
 from .log import _log
 import jwt
 from datetime import datetime, timedelta
 from typing import Optional, Tuple, Type, Union,Dict
 from ._utils import iJSONEncoder,is_datetime_format
 
 AUTH_EXPIRED='[EXPIRED]!'
@@ -247,15 +247,16 @@
         kwargs:secret_key=KEY
     """
     __session_name = config.get("auth").get("session_name",'user')
     global _casbin_auth
     cfg = config.get("auth")
     adapter_uri = kwagrs.get('adapter_uri',None)
     del kwagrs['adapter_uri']
-    model_file = cfg.get("auth_model",'./configs/casbin-model.conf')    
+    model_file = cfg.get("auth_model",'./configs/casbin-model.conf') 
+    model_file = os.path.abspath(os.path.join(ROOT_PATH,model_file))   
     adapter = adapter_class(adapter_uri)
     enforcer = casbin.Enforcer(model_file, adapter)
    
     _casbin_auth = CasbinAuth(enforcer=enforcer,session_name=__session_name)
     
     return backend(**kwagrs) 
 def reload_adapter(app:FastAPI,adapter:Adapter=None):
```

### Comparing `irails-1.3.8/irails/base_controller.py` & `irails-1.3.9/irails/base_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
  
 import re
 from fastapi import FastAPI,UploadFile,File,Header, Depends,HTTPException,Request,Response, status as StateCodes
 from fastapi.responses import RedirectResponse,HTMLResponse,PlainTextResponse
 from .view import _View
- 
+from ._utils import get_controller_name,get_snaked_name
 from .config import config,ROOT_PATH
 from .log import _log
 import os,uuid
 from hashlib import md5
 from typing import Dict
 from logging import Logger
 import inspect
@@ -33,15 +33,18 @@
 i18n_cfg = config.get('i18n')
 if i18n_cfg:
     url_lang_key = i18n_cfg.get('url_lang_key','lang')
 else:
     url_lang_key = 'lang'
 
  
-
+def get_controller_path_from_class_name(class_name):
+    class_name = re.sub(r"Controller$", "", class_name) 
+    class_name = get_snaked_name(class_name)
+    return class_name
 def url_for(url:str="",**kws): 
     url = url.strip()
     if url and url.startswith("/"):
         return url
     url_path = ""
     if kws:
         
@@ -166,15 +169,15 @@
                 return HTMLResponse(content,**kwargs)
             elif format=='text':
                 return PlainTextResponse(content,**kwargs)
             else:
                 return Response(content=content,**kwargs)
         if not view_path and hasattr(self.request.state,'action'):
             func = self.request.state.action.replace(self.__class__.__name__+'.','')
-            vpath = re.sub(r"Controller$", "", self.__class__.__name__).lower()
+            vpath = re.sub(r"Controller$", "", get_controller_path_from_class_name(self.__class__.__name__)).lower()
              
             if self.__version__:
                 vpath += f'/{self.__version__}'
 
             view_path = f"{vpath}/{func}.{format}" 
         
         if not view_path or local2context:    
@@ -188,17 +191,16 @@
                 frame_info = inspect.getframeinfo(caller_frame)
                 if not frame_info[2]=='actions_decorator' and not frame_info[0].endswith('controller_utils.py'):
                     action_frame = caller_frame
             caller_function_name = action_frame.f_code.co_name
             caller_locals = action_frame.f_locals
             # caller_class = caller_locals.get("self", None).__class__
             caller_classname:str = self.__class__.__name__
+            caller_classname = get_controller_path_from_class_name(caller_classname)
             
-            caller_classname = re.sub(r"Controller$", "", caller_classname).lower()
-                
             #caller_file = os.path.basename(caller.filename) 
             if local2context:
                 del caller_locals['self']
                 context.update(caller_locals)
             if not view_path:
                 if self.__version__:
                     version_path = f"{self.__version__}/"
```

### Comparing `irails-1.3.8/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.9/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.9/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/cbv.py` & `irails-1.3.9/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/config.py` & `irails-1.3.9/irails/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,63 +3,57 @@
 import yaml
 import logging
 from hashlib import md5
 from typing import Dict
 import os.path
 import re
 
+def is_cli_mode():
+    executeble = sys.argv[0]
+    executeble = os.path.basename(executeble)
+    # print(f"current executeble:" + executeble)
+    return (executeble.lower().startswith('irails'))
 
 def is_in_app(directory):
     """
     check exists controllers , views dir in :directory
     """
 
     controller_dir = os.path.join(directory, 'controllers')
     views_dir = os.path.join(directory, 'views')
     if not os.path.exists(controller_dir):
         print(f"can't location `controller` dir")
         return False
     if not os.path.exists(views_dir):
         print(f"can't location `views` dir")
         return False
-    # initfile = os.path.join(controller_dir, '__init__.py')
-    # if not os.path.exists(initfile):
-    #     return False
-
+ 
     return True
 
 
 def is_in_irails(directory):
     """
     check exists configs dir,   main.py and configs/general.yaml 
-    """
-
-    configs_dir = os.path.join(directory, 'configs')
-    # main_file = os.path.join(directory, 'main.py')
+    """ 
+    configs_dir = os.path.join(directory, 'configs') 
 
     if not os.path.exists(configs_dir):  # or not os.path.exists(main_file):
         return False
-    general_file = os.path.join(configs_dir, 'general.yaml')
-
+    general_file = os.path.join(configs_dir, 'general.yaml') 
     if not os.path.exists(general_file):
         return False
 
     return True
 
 
 ROOT_PATH = os.path.realpath(os.curdir)
 
 IS_IN_irails = is_in_irails(ROOT_PATH)
 
 
-def is_cli_mode():
-    executeble = sys.argv[0]
-    executeble = os.path.basename(executeble)
-    # print(f"current executeble:" + executeble)
-    return (executeble.lower().startswith('irails'))
 
 
 def _extract_name(string):
     match = re.search(r'{([^}]*)}', string)
     if match:
         return match.group(1)
     else:
@@ -174,15 +168,20 @@
                             sub_value = sub_value.get(sub_key, {})
                         value = value.replace("{" + name + "}", str(sub_value))
             else:
                 value = value.replace(
                     "{" + name + "}", self.config.get(name, ""))
         return value
 
-
-config = YamlConfig(os.path.join(ROOT_PATH, "configs"))
+if is_in_app(ROOT_PATH):
+    ROOT_PATH = os.path.join(ROOT_PATH,"../..")
+    config = YamlConfig( os.path.join(ROOT_PATH,"configs"))
+elif IS_IN_irails:
+    config = YamlConfig(os.path.join(ROOT_PATH, "configs"))
+else:
+    print(f"configs dir not found anywhere!")
 _project_name = os.path.basename(ROOT_PATH)
 debug = False
```

### Comparing `irails-1.3.8/irails/controller_utils.py` & `irails-1.3.9/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/core.py` & `irails-1.3.9/irails/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,22 +299,22 @@
 
         # setattr(puppetController,"__controler_url__",controller_name)  
         #for generate url_for function
         url_path = path
        
         _view_url_path:str = url_path.replace("{controller}",controller_name).replace("{version}",version)  
         
-        controller_current_view_path = abs_path + '/views/' + controller_name.lower()  
+        controller_current_view_path = abs_path + '/views/' + get_snaked_name(controller_name)
         if version:
             controller_current_view_path += '/' + version
         setattr(puppetController,"__view_url__",_view_url_path) 
 
         #add app dir sub views to StaticFiles
         if not controller_current_view_path in application._app_views_dirs: #ensure  load it once
-            application._app_views_dirs[controller_current_view_path] = _view_url_path 
+            application._app_views_dirs[controller_current_view_path.lower()] = _view_url_path.lower() 
             #path match static files
             
             
  
         return puppetController 
     return _wapper #: @puppetController 
 
@@ -370,15 +370,15 @@
     global __is_debug
      
     application.title = _project_name
     
     
     
     
-    _log.info(_("\n\init mvc app..."))
+    _log.info(_("loading irails apps..."))
     loaded,unloaded=_load_apps(debug=__is_debug) 
     _log.info(_('Load Apps Completed,%s loaded,%s unloaded') %(loaded,unloaded))  
     if not len(__all_controller__)>0:
         raise RuntimeError(_("not found any controller class"))
     
     _register_controllers()
 
@@ -399,17 +399,18 @@
             if not _casbin_adapter_class:
                 raise RuntimeError(_( "Not support %s ,Adapter config error in auth.casbin_adapter") % __type_casbin_adapter)
             
     
     check_db_migrate()
 
     if _casbin_adapter_class and _adapter_uri:
+        _adapter_uri = os.path.abspath(os.path.join(ROOT_PATH,_adapter_uri))
         _log.info(_("init casbin auth system..."))
         application.authObj = __init_auth(application,auth_type,_casbin_adapter_class,_adapter_uri)
-    _log.info(_("init mvc app end."))
+    _log.info(_("load irails apps finished."))
     return application
 # import subprocess
 # import time
 # # 定义启动和停止进程的方法
 # def start_uvicon():
 #     cmd = 'uvicorn main:app --host 0.0.0.0 --port 8000'
 #     uvicorn_process = subprocess.Popen(cmd.split(), stdout=subprocess.PIPE)
```

### Comparing `irails-1.3.8/irails/database.py` & `irails-1.3.9/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/log.py` & `irails-1.3.9/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/midware.py` & `irails-1.3.9/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/midware_casbin.py` & `irails-1.3.9/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/midware_session.py` & `irails-1.3.9/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/mvc_router.py` & `irails-1.3.9/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/_app.py` & `irails-1.3.9/irails/scripts/_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,15 @@
                 'views',
                 'locales',
                 'tests'
             ]
             context = {'app':app_name}
             for dir in dirs_items:
                 _current_dir = os.path.join(store_dir,dir)
+                print(f"creating {_current_dir}")
                 os.makedirs(_current_dir,exist_ok=True)
                  
             # _init_file = os.path.normpath(os.path.join(store_dir,'__init__.py'))
             # with open(_init_file,'w') as f: #root path of app's dir
             #     f.write(f"from .controllers import *")
             
             # print(f"create {_init_file}")
```

### Comparing `irails-1.3.8/irails/scripts/_controller.py` & `irails-1.3.9/irails/scripts/_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,27 +93,30 @@
             controler_path_name = get_snaked_name(controller_name)
             # store_dir = os.path.join(store_dir,controler_path_name )
             
             # controller_name = self.str_to_upper(name)
             if not self.is_valid_class_name(controller_name):
                 print(f"{controller_name} is a not valided class name,exit...")
                 exit() 
-            
+            acts = []
+            actions = self.args.name
+            if len(actions)==0:actions.append('index')
+
             dirs_items =  {
                 'controllers':{'tpl':'controller.tpl','dest':f'controllers/{controler_path_name}_controller.py','micro':True} , 
                 'models': {'tpl':'model.tpl','dest' : f'models/{controler_path_name}_model.py','micro':True},
                 'services':{'tpl':'service.tpl','dest': f'services/{controler_path_name}_service.py','micro':True },
                 'views': [
                     {'tpl' : 'view.tpl','dest': f'views/{controler_path_name}/index.html','micro':False},
                     {'tpl' : 'css.tpl','dest': f'views/{controler_path_name}/index.css','micro':False}
                     ] ,
                 
-                'tests': {'tpl':'test.tpl','dest': f'tests/test_{controler_path_name}.py','micro':True}
+                'tests': {'tpl':'test_controller.jinja','dest': f'tests/test_{controler_path_name}.py','micro':True}
             }
-            context = {'ctrl_name':controller_name.title(),'ctrl_path':controler_path_name}
+            context = {'ctrl_name':controller_name.title(),'ctrl_path':controler_path_name,'actions':actions}
             for dir in dirs_items:
                 _current_dir = store_dir#os.path.join(store_dir,dir)
                 os.makedirs(_current_dir,exist_ok=True)
                 items = dirs_items[dir]
                 if isinstance(items,list):
                     _item = items
                 else:
@@ -127,17 +130,15 @@
             controller_file = os.path.join(_current_dir,'controllers',f"{controler_path_name}_controller.py")
             __init_file = os.path.join(_current_dir,'controllers','__init__.py')
             self.ensure_line(__init_file,f"from . import {controler_path_name}_controller")
             __init_file = os.path.join(_current_dir,'models','__init__.py')
             self.ensure_line(__init_file,f"from . import {controler_path_name}_model")
             __init_file = os.path.join(_current_dir,'services','__init__.py')
             self.ensure_line(__init_file,f"from . import {controler_path_name}_service")
-            acts = []
-            actions = self.args.name
-            if len(actions)==0:actions.append('index')
+            
             for action in actions:
                 acts.append(f"""
     @api.get('/{action}')
     def {action}(self):
         return self.view()                
 """)
                 _view_file = os.path.join(_current_dir,'views',controler_path_name,f"{action}.html")
```

### Comparing `irails-1.3.8/irails/scripts/_i18n.py` & `irails-1.3.9/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/_project.py` & `irails-1.3.9/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/_run.py` & `irails-1.3.9/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/_shell.py` & `irails-1.3.9/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/main.py` & `irails-1.3.9/irails/scripts/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,27 @@
 import re
 def _ensure_cli():
     executable = os.path.basename(sys.argv[0])
     if not executable.startswith('irails'):
         sys.argv[0] = 'irails'
 _ensure_cli()
 
+def is_dev_mode(path):
+    dev_mode = True
+    irails_srcs = ['__init__.py','_i18n.py','_loader.py','_utils.py','auth.py','base_controller.py','cbv.py']
+    for src in irails_srcs:
+        p = os.path.join(path,src)
+        if not os.path.exists(p):
+            dev_mode = False
+    return dev_mode
+curdir = os.path.abspath(os.curdir)
+project_root = os.path.abspath(os.path.join(curdir,"../.."))
+if is_dev_mode(os.path.join(project_root,'irails')): 
+    sys.path.insert(-1, project_root)
+    
 sys.path.insert(-1,os.path.abspath(os.curdir))
 from irails import __version__
 def collect_features():
     """
     return files in current dir start with '_' no sub dir
     """
```

### Comparing `irails-1.3.8/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.9/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/tpls/app/home.tpl` & `irails-1.3.9/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.9/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.9/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.9/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.9/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.9/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.9/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.9/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.9/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.9/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.9/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.9/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails/view.py` & `irails-1.3.9/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/irails.egg-info/PKG-INFO` & `irails-1.3.9/irails.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.8
+Version: 1.3.9
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.8/irails.egg-info/SOURCES.txt` & `irails-1.3.9/irails.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 irails/core.py
 irails/database.py
 irails/log.py
 irails/midware.py
 irails/midware_casbin.py
 irails/midware_session.py
 irails/mvc_router.py
+irails/unit_test.py
 irails/view.py
 irails.egg-info/PKG-INFO
 irails.egg-info/SOURCES.txt
 irails.egg-info/dependency_links.txt
 irails.egg-info/entry_points.txt
 irails.egg-info/requires.txt
 irails.egg-info/top_level.txt
@@ -30,22 +31,23 @@
 irails/scripts/__init__.py
 irails/scripts/_app.py
 irails/scripts/_controller.py
 irails/scripts/_i18n.py
 irails/scripts/_project.py
 irails/scripts/_run.py
 irails/scripts/_shell.py
+irails/scripts/_test.py
 irails/scripts/main.py
 irails/scripts/tpls/app/controller.tpl
 irails/scripts/tpls/app/css.tpl
 irails/scripts/tpls/app/home.css.tpl
 irails/scripts/tpls/app/home.tpl
 irails/scripts/tpls/app/model.tpl
 irails/scripts/tpls/app/service.tpl
-irails/scripts/tpls/app/test.tpl
+irails/scripts/tpls/app/test_controller.jinja
 irails/scripts/tpls/app/view.tpl
 irails/scripts/tpls/project/.gitignore
 irails/scripts/tpls/project/main.py
 irails/scripts/tpls/project/apps/__init__.py
 irails/scripts/tpls/project/configs/alembic.ini
 irails/scripts/tpls/project/configs/authencation.yaml
 irails/scripts/tpls/project/configs/cache.yaml
```

### Comparing `irails-1.3.8/irails.egg-info/requires.txt` & `irails-1.3.9/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.8/setup.py` & `irails-1.3.9/setup.py`

 * *Files identical despite different names*

