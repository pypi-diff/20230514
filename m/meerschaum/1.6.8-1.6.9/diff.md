# Comparing `tmp/meerschaum-1.6.8.tar.gz` & `tmp/meerschaum-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerschaum-1.6.8.tar", last modified: Fri May 12 06:36:15 2023, max compression
+gzip compressed data, was "meerschaum-1.6.9.tar", last modified: Fri May 12 17:43:14 2023, max compression
```

## Comparing `meerschaum-1.6.8.tar` & `meerschaum-1.6.9.tar`

### file list

```diff
@@ -1,279 +1,279 @@
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.390143 meerschaum-1.6.8/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-1.6.8/LICENSE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-1.6.8/NOTICE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-05-12 06:36:15.389143 meerschaum-1.6.8/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9248 2022-07-13 02:48:08.000000 meerschaum-1.6.8/README.md
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.374143 meerschaum-1.6.8/meerschaum/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1236 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2774 2022-10-22 06:28:47.000000 meerschaum-1.6.8/meerschaum/__main__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.375143 meerschaum-1.6.8/meerschaum/_internal/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-1.6.8/meerschaum/_internal/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.375143 meerschaum-1.6.8/meerschaum/_internal/arguments/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-1.6.8/meerschaum/_internal/arguments/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9741 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/_internal/arguments/_parse_arguments.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12375 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/_internal/arguments/_parser.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.375143 meerschaum-1.6.8/meerschaum/_internal/docs/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/_internal/docs/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7719 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/docs/index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4625 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/_internal/entry.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.375143 meerschaum-1.6.8/meerschaum/_internal/gui/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1332 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/gui/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.376143 meerschaum-1.6.8/meerschaum/_internal/gui/app/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/gui/app/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-1.6.8/meerschaum/_internal/gui/app/_windows.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1016 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/gui/app/actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1678 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/gui/app/pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.376143 meerschaum-1.6.8/meerschaum/_internal/shell/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31489 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/_internal/shell/Shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2981 2022-10-22 06:28:01.000000 meerschaum-1.6.8/meerschaum/_internal/shell/ShellCompleter.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-1.6.8/meerschaum/_internal/shell/ValidAutoSuggest.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/shell/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.376143 meerschaum-1.6.8/meerschaum/_internal/shell/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/shell/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.376143 meerschaum-1.6.8/meerschaum/_internal/term/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2021-12-09 07:32:03.000000 meerschaum-1.6.8/meerschaum/_internal/term/TermPageHandler.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1495 2021-12-09 07:32:03.000000 meerschaum-1.6.8/meerschaum/_internal/term/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      788 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/_internal/term/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.378143 meerschaum-1.6.8/meerschaum/actions/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8129 2022-10-26 04:20:20.000000 meerschaum-1.6.8/meerschaum/actions/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10996 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/actions/api.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14529 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/actions/bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4857 2022-08-23 06:14:42.000000 meerschaum-1.6.8/meerschaum/actions/clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6095 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/actions/copy.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15245 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/actions/delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2701 2022-06-27 01:07:31.000000 meerschaum-1.6.8/meerschaum/actions/drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9492 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/actions/edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7380 2022-10-18 06:13:35.000000 meerschaum-1.6.8/meerschaum/actions/install.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/actions/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-1.6.8/meerschaum/actions/os.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/actions/python.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11219 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/actions/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      605 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/actions/reload.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3211 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/actions/setup.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-1.6.8/meerschaum/actions/sh.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23468 2023-01-11 06:27:06.000000 meerschaum-1.6.8/meerschaum/actions/show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4224 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/actions/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5501 2022-10-25 06:38:00.000000 meerschaum-1.6.8/meerschaum/actions/stack.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18247 2022-11-22 01:55:36.000000 meerschaum-1.6.8/meerschaum/actions/start.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3948 2023-01-16 21:21:28.000000 meerschaum-1.6.8/meerschaum/actions/stop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15339 2022-12-15 02:09:06.000000 meerschaum-1.6.8/meerschaum/actions/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6073 2022-08-19 04:59:44.000000 meerschaum-1.6.8/meerschaum/actions/uninstall.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6307 2022-08-19 04:59:44.000000 meerschaum-1.6.8/meerschaum/actions/upgrade.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3348 2022-10-26 04:20:20.000000 meerschaum-1.6.8/meerschaum/actions/verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.378143 meerschaum-1.6.8/meerschaum/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7638 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/api/_chain.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      966 2022-08-19 04:59:44.000000 meerschaum-1.6.8/meerschaum/api/_events.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-08-19 04:59:44.000000 meerschaum-1.6.8/meerschaum/api/_oauth2.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1226 2022-11-05 03:38:45.000000 meerschaum-1.6.8/meerschaum/api/_websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.379143 meerschaum-1.6.8/meerschaum/api/dash/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2238 2023-01-09 08:57:26.000000 meerschaum-1.6.8/meerschaum/api/dash/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9600 2022-10-31 13:18:31.000000 meerschaum-1.6.8/meerschaum/api/dash/actions.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.380143 meerschaum-1.6.8/meerschaum/api/dash/assets/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/assets/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/assets/ansi_up.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/assets/banner_1920x320.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/assets/favicon.ico
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/assets/logo_48x48.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/assets/logo_500x500.png
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.381143 meerschaum-1.6.8/meerschaum/api/dash/callbacks/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      283 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/callbacks/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24874 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/api/dash/callbacks/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2529 2023-01-09 09:04:18.000000 meerschaum-1.6.8/meerschaum/api/dash/callbacks/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/callbacks/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3446 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/api/dash/callbacks/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6771 2022-10-31 13:18:31.000000 meerschaum-1.6.8/meerschaum/api/dash/components.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/graphs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3544 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13682 2022-10-31 13:18:31.000000 meerschaum-1.6.8/meerschaum/api/dash/keys.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.381143 meerschaum-1.6.8/meerschaum/api/dash/pages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/api/dash/pages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3838 2022-10-31 13:18:31.000000 meerschaum-1.6.8/meerschaum/api/dash/pages/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      598 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/pages/error.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4601 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/pages/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1425 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/pages/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2398 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/pages/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15039 2022-10-31 14:15:34.000000 meerschaum-1.6.8/meerschaum/api/dash/pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3054 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      886 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-1.6.8/meerschaum/api/dash/websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.381143 meerschaum-1.6.8/meerschaum/api/models/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/models/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/models/_interfaces.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/models/_locations.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/models/_metrics.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-1.6.8/meerschaum/api/models/_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.381143 meerschaum-1.6.8/meerschaum/api/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.381143 meerschaum-1.6.8/meerschaum/api/resources/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.382143 meerschaum-1.6.8/meerschaum/api/resources/static/css/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/css/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/css/bootstrap.min.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1592 2022-10-31 13:18:31.000000 meerschaum-1.6.8/meerschaum/api/resources/static/css/dash.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/css/dbc_dark.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/css/styles.css
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.382143 meerschaum-1.6.8/meerschaum/api/resources/static/ico/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/ico/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/ico/logo.ico
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.382143 meerschaum-1.6.8/meerschaum/api/resources/static/js/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/js/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/js/action_button.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/js/main.js
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.383143 meerschaum-1.6.8/meerschaum/api/resources/static/png/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/png/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.383143 meerschaum-1.6.8/meerschaum/api/resources/templates/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/templates/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/templates/index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/templates/old_index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/templates/secret.html
--rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     2082 2021-12-09 07:32:03.000000 meerschaum-1.6.8/meerschaum/api/resources/templates/termpage.html
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.383143 meerschaum-1.6.8/meerschaum/api/routes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      734 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/routes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-1.6.8/meerschaum/api/routes/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1803 2022-06-27 01:07:31.000000 meerschaum-1.6.8/meerschaum/api/routes/_connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/api/routes/_index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1882 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/api/routes/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1702 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/api/routes/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21169 2023-01-21 08:00:50.000000 meerschaum-1.6.8/meerschaum/api/routes/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6152 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/api/routes/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7239 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/api/routes/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-1.6.8/meerschaum/api/routes/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.383143 meerschaum-1.6.8/meerschaum/api/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      615 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/api/tables/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.384142 meerschaum-1.6.8/meerschaum/config/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11629 2023-01-11 04:28:52.000000 meerschaum-1.6.8/meerschaum/config/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5135 2023-05-05 04:35:54.000000 meerschaum-1.6.8/meerschaum/config/_default.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8807 2022-07-13 02:48:16.000000 meerschaum-1.6.8/meerschaum/config/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4507 2022-10-22 07:29:33.000000 meerschaum-1.6.8/meerschaum/config/_environment.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5556 2022-05-02 19:58:56.000000 meerschaum-1.6.8/meerschaum/config/_formatting.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      647 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/config/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1508 2023-01-11 05:57:34.000000 meerschaum-1.6.8/meerschaum/config/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6648 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/config/_paths.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/config/_preprocess.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14567 2022-10-14 04:34:51.000000 meerschaum-1.6.8/meerschaum/config/_read_config.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3589 2021-11-21 05:32:46.000000 meerschaum-1.6.8/meerschaum/config/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4968 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/config/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       71 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/config/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.384142 meerschaum-1.6.8/meerschaum/config/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/config/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.384142 meerschaum-1.6.8/meerschaum/config/stack/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8233 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/config/stack/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.384142 meerschaum-1.6.8/meerschaum/config/stack/grafana/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-1.6.8/meerschaum/config/stack/grafana/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.384142 meerschaum-1.6.8/meerschaum/config/stack/mosquitto/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/config/stack/mosquitto/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.384142 meerschaum-1.6.8/meerschaum/config/stack/mosquitto/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/config/stack/mosquitto/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.385143 meerschaum-1.6.8/meerschaum/config/stack/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/config/stack/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.385143 meerschaum-1.6.8/meerschaum/config/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3679 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/config/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.385143 meerschaum-1.6.8/meerschaum/connectors/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/Connector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12064 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.386143 meerschaum-1.6.8/meerschaum/connectors/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4022 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/api/APIConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/connectors/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2759 2022-10-22 06:21:34.000000 meerschaum-1.6.8/meerschaum/connectors/api/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/connectors/api/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2056 2022-11-01 03:12:07.000000 meerschaum-1.6.8/meerschaum/connectors/api/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1572 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/connectors/api/_get.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2054 2022-11-18 03:44:05.000000 meerschaum-1.6.8/meerschaum/connectors/api/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1185 2022-06-27 01:07:31.000000 meerschaum-1.6.8/meerschaum/connectors/api/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      933 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/connectors/api/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19986 2023-04-26 08:12:59.000000 meerschaum-1.6.8/meerschaum/connectors/api/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5227 2022-06-27 01:07:31.000000 meerschaum-1.6.8/meerschaum/connectors/api/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      922 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/connectors/api/_post.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-1.6.8/meerschaum/connectors/api/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5303 2022-08-19 04:59:44.000000 meerschaum-1.6.8/meerschaum/connectors/api/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4048 2022-10-18 06:13:35.000000 meerschaum-1.6.8/meerschaum/connectors/parse.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.386143 meerschaum-1.6.8/meerschaum/connectors/plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-1.6.8/meerschaum/connectors/plugin/PluginConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/connectors/plugin/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7215 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/poll.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.386143 meerschaum-1.6.8/meerschaum/connectors/sql/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8592 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/sql/SQLConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/connectors/sql/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3495 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_cli.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10197 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_create_engine.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12650 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    88433 2023-05-09 02:50:23.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7921 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26869 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3312 2022-10-18 01:38:49.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9972 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_users.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.387143 meerschaum-1.6.8/meerschaum/connectors/sql/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6482 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/sql/tables/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/connectors/sql/tables/types.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/connectors/sql/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.387143 meerschaum-1.6.8/meerschaum/core/
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.387143 meerschaum-1.6.8/meerschaum/core/Pipe/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15032 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/core/Pipe/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_attributes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2112 2022-11-13 04:57:20.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10716 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_data.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1854 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3146 2023-05-08 21:38:02.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2877 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    25706 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_sync.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.387143 meerschaum-1.6.8/meerschaum/core/Plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/core/Plugin/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.387143 meerschaum-1.6.8/meerschaum/core/User/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/core/User/_User.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/core/User/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/core/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.388142 meerschaum-1.6.8/meerschaum/plugins/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33813 2023-01-21 08:00:50.000000 meerschaum-1.6.8/meerschaum/plugins/_Plugin.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18398 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/plugins/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.388142 meerschaum-1.6.8/meerschaum/utils/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      444 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/utils/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.389143 meerschaum-1.6.8/meerschaum/utils/daemon/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24801 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/utils/daemon/Daemon.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3170 2023-01-09 03:01:33.000000 meerschaum-1.6.8/meerschaum/utils/daemon/Log.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5355 2023-01-09 09:50:51.000000 meerschaum-1.6.8/meerschaum/utils/daemon/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4302 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/utils/daemon/_names.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/utils/debug.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.389143 meerschaum-1.6.8/meerschaum/utils/formatting/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9387 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/utils/formatting/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2939 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/utils/formatting/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12729 2022-10-25 06:38:00.000000 meerschaum-1.6.8/meerschaum/utils/formatting/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3032 2022-10-18 06:13:35.000000 meerschaum-1.6.8/meerschaum/utils/formatting/_pprint.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3844 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/utils/formatting/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11791 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/utils/get_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3419 2022-10-18 06:13:35.000000 meerschaum-1.6.8/meerschaum/utils/interactive.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    61453 2023-05-08 21:38:02.000000 meerschaum-1.6.8/meerschaum/utils/misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/utils/networking.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.389143 meerschaum-1.6.8/meerschaum/utils/packages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    53718 2023-05-08 21:38:02.000000 meerschaum-1.6.8/meerschaum/utils/packages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8054 2023-05-12 06:36:03.000000 meerschaum-1.6.8/meerschaum/utils/packages/_packages.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-1.6.8/meerschaum/utils/packages/lazy_loader.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2781 2022-08-23 06:14:42.000000 meerschaum-1.6.8/meerschaum/utils/pool.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/utils/process.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16060 2022-05-02 19:58:56.000000 meerschaum-1.6.8/meerschaum/utils/prompt.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1635 2022-08-29 21:54:10.000000 meerschaum-1.6.8/meerschaum/utils/schedule.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34702 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/utils/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2152 2022-10-25 06:38:00.000000 meerschaum-1.6.8/meerschaum/utils/threading.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2517 2023-05-05 21:42:47.000000 meerschaum-1.6.8/meerschaum/utils/typing.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.389143 meerschaum-1.6.8/meerschaum/utils/venv/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3479 2022-10-25 06:38:00.000000 meerschaum-1.6.8/meerschaum/utils/venv/_Venv.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    22150 2023-04-26 08:12:59.000000 meerschaum-1.6.8/meerschaum/utils/venv/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6610 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/utils/warnings.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/utils/yaml.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.375143 meerschaum-1.6.8/meerschaum.egg-info/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7834 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/SOURCES.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/dependency_links.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/entry_points.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4703 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/requires.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/top_level.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/zip-safe
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2023-05-12 06:36:15.390143 meerschaum-1.6.8/setup.cfg
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3056 2023-05-12 06:36:03.000000 meerschaum-1.6.8/setup.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.914779 meerschaum-1.6.9/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-1.6.9/LICENSE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-1.6.9/NOTICE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-05-12 17:43:14.913779 meerschaum-1.6.9/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9248 2022-07-13 02:48:08.000000 meerschaum-1.6.9/README.md
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.890779 meerschaum-1.6.9/meerschaum/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1236 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2774 2022-10-22 06:28:47.000000 meerschaum-1.6.9/meerschaum/__main__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.891779 meerschaum-1.6.9/meerschaum/_internal/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-1.6.9/meerschaum/_internal/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.891779 meerschaum-1.6.9/meerschaum/_internal/arguments/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-1.6.9/meerschaum/_internal/arguments/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9741 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/_internal/arguments/_parse_arguments.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12375 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/_internal/arguments/_parser.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.892779 meerschaum-1.6.9/meerschaum/_internal/docs/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/_internal/docs/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7719 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/docs/index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4625 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/_internal/entry.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.892779 meerschaum-1.6.9/meerschaum/_internal/gui/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1332 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/gui/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.892779 meerschaum-1.6.9/meerschaum/_internal/gui/app/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/gui/app/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-1.6.9/meerschaum/_internal/gui/app/_windows.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1016 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/gui/app/actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1678 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/gui/app/pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.892779 meerschaum-1.6.9/meerschaum/_internal/shell/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31489 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/_internal/shell/Shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2981 2022-10-22 06:28:01.000000 meerschaum-1.6.9/meerschaum/_internal/shell/ShellCompleter.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-1.6.9/meerschaum/_internal/shell/ValidAutoSuggest.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/shell/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.893779 meerschaum-1.6.9/meerschaum/_internal/shell/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/shell/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.893779 meerschaum-1.6.9/meerschaum/_internal/term/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2021-12-09 07:32:03.000000 meerschaum-1.6.9/meerschaum/_internal/term/TermPageHandler.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1495 2021-12-09 07:32:03.000000 meerschaum-1.6.9/meerschaum/_internal/term/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      788 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/_internal/term/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.895779 meerschaum-1.6.9/meerschaum/actions/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8129 2022-10-26 04:20:20.000000 meerschaum-1.6.9/meerschaum/actions/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10996 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/actions/api.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14529 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/actions/bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4857 2022-08-23 06:14:42.000000 meerschaum-1.6.9/meerschaum/actions/clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6095 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/actions/copy.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15245 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/actions/delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2701 2022-06-27 01:07:31.000000 meerschaum-1.6.9/meerschaum/actions/drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9492 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/actions/edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7380 2022-10-18 06:13:35.000000 meerschaum-1.6.9/meerschaum/actions/install.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/actions/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-1.6.9/meerschaum/actions/os.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/actions/python.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11219 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/actions/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      605 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/actions/reload.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3211 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/actions/setup.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-1.6.9/meerschaum/actions/sh.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23468 2023-01-11 06:27:06.000000 meerschaum-1.6.9/meerschaum/actions/show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4224 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/actions/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5501 2022-10-25 06:38:00.000000 meerschaum-1.6.9/meerschaum/actions/stack.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18247 2022-11-22 01:55:36.000000 meerschaum-1.6.9/meerschaum/actions/start.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3948 2023-01-16 21:21:28.000000 meerschaum-1.6.9/meerschaum/actions/stop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15339 2022-12-15 02:09:06.000000 meerschaum-1.6.9/meerschaum/actions/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6073 2022-08-19 04:59:44.000000 meerschaum-1.6.9/meerschaum/actions/uninstall.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6307 2022-08-19 04:59:44.000000 meerschaum-1.6.9/meerschaum/actions/upgrade.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3348 2022-10-26 04:20:20.000000 meerschaum-1.6.9/meerschaum/actions/verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.896779 meerschaum-1.6.9/meerschaum/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7638 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/api/_chain.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      966 2022-08-19 04:59:44.000000 meerschaum-1.6.9/meerschaum/api/_events.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-08-19 04:59:44.000000 meerschaum-1.6.9/meerschaum/api/_oauth2.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1226 2022-11-05 03:38:45.000000 meerschaum-1.6.9/meerschaum/api/_websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.897779 meerschaum-1.6.9/meerschaum/api/dash/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2238 2023-01-09 08:57:26.000000 meerschaum-1.6.9/meerschaum/api/dash/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9600 2022-10-31 13:18:31.000000 meerschaum-1.6.9/meerschaum/api/dash/actions.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.898779 meerschaum-1.6.9/meerschaum/api/dash/assets/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/assets/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/assets/ansi_up.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/assets/banner_1920x320.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/assets/favicon.ico
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/assets/logo_48x48.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/assets/logo_500x500.png
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.899779 meerschaum-1.6.9/meerschaum/api/dash/callbacks/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      283 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/callbacks/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24874 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/api/dash/callbacks/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2529 2023-01-09 09:04:18.000000 meerschaum-1.6.9/meerschaum/api/dash/callbacks/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/callbacks/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3446 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/api/dash/callbacks/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6771 2022-10-31 13:18:31.000000 meerschaum-1.6.9/meerschaum/api/dash/components.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/graphs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3544 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13682 2022-10-31 13:18:31.000000 meerschaum-1.6.9/meerschaum/api/dash/keys.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.899779 meerschaum-1.6.9/meerschaum/api/dash/pages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/api/dash/pages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3838 2022-10-31 13:18:31.000000 meerschaum-1.6.9/meerschaum/api/dash/pages/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      598 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/pages/error.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4601 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/pages/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1425 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/pages/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2398 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/pages/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15039 2022-10-31 14:15:34.000000 meerschaum-1.6.9/meerschaum/api/dash/pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3054 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      886 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-1.6.9/meerschaum/api/dash/websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.900779 meerschaum-1.6.9/meerschaum/api/models/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/models/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/models/_interfaces.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/models/_locations.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/models/_metrics.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-1.6.9/meerschaum/api/models/_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.900779 meerschaum-1.6.9/meerschaum/api/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.900779 meerschaum-1.6.9/meerschaum/api/resources/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.901779 meerschaum-1.6.9/meerschaum/api/resources/static/css/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/css/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/css/bootstrap.min.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1592 2022-10-31 13:18:31.000000 meerschaum-1.6.9/meerschaum/api/resources/static/css/dash.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/css/dbc_dark.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/css/styles.css
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.901779 meerschaum-1.6.9/meerschaum/api/resources/static/ico/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/ico/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/ico/logo.ico
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.901779 meerschaum-1.6.9/meerschaum/api/resources/static/js/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/js/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/js/action_button.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/js/main.js
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.901779 meerschaum-1.6.9/meerschaum/api/resources/static/png/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/png/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.901779 meerschaum-1.6.9/meerschaum/api/resources/templates/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/templates/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/templates/index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/templates/old_index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/templates/secret.html
+-rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     2082 2021-12-09 07:32:03.000000 meerschaum-1.6.9/meerschaum/api/resources/templates/termpage.html
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.903779 meerschaum-1.6.9/meerschaum/api/routes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      734 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/routes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-1.6.9/meerschaum/api/routes/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1803 2022-06-27 01:07:31.000000 meerschaum-1.6.9/meerschaum/api/routes/_connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/api/routes/_index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1882 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/api/routes/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1702 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/api/routes/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21169 2023-01-21 08:00:50.000000 meerschaum-1.6.9/meerschaum/api/routes/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6152 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/api/routes/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7239 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/api/routes/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-1.6.9/meerschaum/api/routes/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.903779 meerschaum-1.6.9/meerschaum/api/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      615 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/api/tables/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.904779 meerschaum-1.6.9/meerschaum/config/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11629 2023-01-11 04:28:52.000000 meerschaum-1.6.9/meerschaum/config/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5135 2023-05-05 04:35:54.000000 meerschaum-1.6.9/meerschaum/config/_default.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8807 2022-07-13 02:48:16.000000 meerschaum-1.6.9/meerschaum/config/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4507 2022-10-22 07:29:33.000000 meerschaum-1.6.9/meerschaum/config/_environment.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5556 2022-05-02 19:58:56.000000 meerschaum-1.6.9/meerschaum/config/_formatting.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      647 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/config/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1508 2023-01-11 05:57:34.000000 meerschaum-1.6.9/meerschaum/config/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6648 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/config/_paths.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/config/_preprocess.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14567 2022-10-14 04:34:51.000000 meerschaum-1.6.9/meerschaum/config/_read_config.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3589 2021-11-21 05:32:46.000000 meerschaum-1.6.9/meerschaum/config/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4968 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/config/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       71 2023-05-12 17:42:26.000000 meerschaum-1.6.9/meerschaum/config/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.904779 meerschaum-1.6.9/meerschaum/config/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/config/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.904779 meerschaum-1.6.9/meerschaum/config/stack/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8233 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/config/stack/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.904779 meerschaum-1.6.9/meerschaum/config/stack/grafana/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-1.6.9/meerschaum/config/stack/grafana/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.904779 meerschaum-1.6.9/meerschaum/config/stack/mosquitto/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/config/stack/mosquitto/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.904779 meerschaum-1.6.9/meerschaum/config/stack/mosquitto/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/config/stack/mosquitto/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.905779 meerschaum-1.6.9/meerschaum/config/stack/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/config/stack/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.905779 meerschaum-1.6.9/meerschaum/config/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3679 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/config/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.905779 meerschaum-1.6.9/meerschaum/connectors/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/Connector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12064 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.906779 meerschaum-1.6.9/meerschaum/connectors/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4022 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/api/APIConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/connectors/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2759 2022-10-22 06:21:34.000000 meerschaum-1.6.9/meerschaum/connectors/api/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/connectors/api/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2056 2022-11-01 03:12:07.000000 meerschaum-1.6.9/meerschaum/connectors/api/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1572 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/connectors/api/_get.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2054 2022-11-18 03:44:05.000000 meerschaum-1.6.9/meerschaum/connectors/api/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1185 2022-06-27 01:07:31.000000 meerschaum-1.6.9/meerschaum/connectors/api/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      933 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/connectors/api/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19986 2023-04-26 08:12:59.000000 meerschaum-1.6.9/meerschaum/connectors/api/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5227 2022-06-27 01:07:31.000000 meerschaum-1.6.9/meerschaum/connectors/api/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      922 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/connectors/api/_post.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-1.6.9/meerschaum/connectors/api/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5303 2022-08-19 04:59:44.000000 meerschaum-1.6.9/meerschaum/connectors/api/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4048 2022-10-18 06:13:35.000000 meerschaum-1.6.9/meerschaum/connectors/parse.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.907779 meerschaum-1.6.9/meerschaum/connectors/plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-1.6.9/meerschaum/connectors/plugin/PluginConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/connectors/plugin/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7215 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/poll.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.908779 meerschaum-1.6.9/meerschaum/connectors/sql/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8592 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/sql/SQLConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/connectors/sql/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3495 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_cli.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10197 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_create_engine.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12650 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    88433 2023-05-09 02:50:23.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7921 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26869 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3312 2022-10-18 01:38:49.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9972 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_users.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.908779 meerschaum-1.6.9/meerschaum/connectors/sql/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6482 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/sql/tables/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/connectors/sql/tables/types.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/connectors/sql/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.908779 meerschaum-1.6.9/meerschaum/core/
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.909779 meerschaum-1.6.9/meerschaum/core/Pipe/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15032 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/core/Pipe/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_attributes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2112 2022-11-13 04:57:20.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10716 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_data.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1854 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3146 2023-05-08 21:38:02.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3005 2023-05-12 17:42:26.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    25706 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_sync.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.909779 meerschaum-1.6.9/meerschaum/core/Plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/core/Plugin/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.910779 meerschaum-1.6.9/meerschaum/core/User/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/core/User/_User.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/core/User/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/core/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.910779 meerschaum-1.6.9/meerschaum/plugins/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33813 2023-01-21 08:00:50.000000 meerschaum-1.6.9/meerschaum/plugins/_Plugin.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18398 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/plugins/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.912779 meerschaum-1.6.9/meerschaum/utils/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      444 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/utils/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.912779 meerschaum-1.6.9/meerschaum/utils/daemon/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24801 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/utils/daemon/Daemon.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3170 2023-01-09 03:01:33.000000 meerschaum-1.6.9/meerschaum/utils/daemon/Log.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5355 2023-01-09 09:50:51.000000 meerschaum-1.6.9/meerschaum/utils/daemon/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4302 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/utils/daemon/_names.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/utils/debug.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.912779 meerschaum-1.6.9/meerschaum/utils/formatting/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9387 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/utils/formatting/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2939 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/utils/formatting/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12729 2022-10-25 06:38:00.000000 meerschaum-1.6.9/meerschaum/utils/formatting/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3032 2022-10-18 06:13:35.000000 meerschaum-1.6.9/meerschaum/utils/formatting/_pprint.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3844 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/utils/formatting/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11791 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/utils/get_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3419 2022-10-18 06:13:35.000000 meerschaum-1.6.9/meerschaum/utils/interactive.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    61453 2023-05-08 21:38:02.000000 meerschaum-1.6.9/meerschaum/utils/misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/utils/networking.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.913779 meerschaum-1.6.9/meerschaum/utils/packages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    53718 2023-05-08 21:38:02.000000 meerschaum-1.6.9/meerschaum/utils/packages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8054 2023-05-12 17:39:43.000000 meerschaum-1.6.9/meerschaum/utils/packages/_packages.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-1.6.9/meerschaum/utils/packages/lazy_loader.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2781 2022-08-23 06:14:42.000000 meerschaum-1.6.9/meerschaum/utils/pool.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/utils/process.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16060 2022-05-02 19:58:56.000000 meerschaum-1.6.9/meerschaum/utils/prompt.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1635 2022-08-29 21:54:10.000000 meerschaum-1.6.9/meerschaum/utils/schedule.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34702 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/utils/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2152 2022-10-25 06:38:00.000000 meerschaum-1.6.9/meerschaum/utils/threading.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2517 2023-05-05 21:42:47.000000 meerschaum-1.6.9/meerschaum/utils/typing.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.913779 meerschaum-1.6.9/meerschaum/utils/venv/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3479 2022-10-25 06:38:00.000000 meerschaum-1.6.9/meerschaum/utils/venv/_Venv.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    22150 2023-04-26 08:12:59.000000 meerschaum-1.6.9/meerschaum/utils/venv/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6610 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/utils/warnings.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/utils/yaml.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.891779 meerschaum-1.6.9/meerschaum.egg-info/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7834 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/SOURCES.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/dependency_links.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/entry_points.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4703 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/requires.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/top_level.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/zip-safe
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2023-05-12 17:43:14.914779 meerschaum-1.6.9/setup.cfg
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3056 2023-05-12 17:39:43.000000 meerschaum-1.6.9/setup.py
```

### Comparing `meerschaum-1.6.8/LICENSE` & `meerschaum-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/PKG-INFO` & `meerschaum-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 1.6.8
+Version: 1.6.9
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
```

### Comparing `meerschaum-1.6.8/README.md` & `meerschaum-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/__init__.py` & `meerschaum-1.6.9/meerschaum/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/__main__.py` & `meerschaum-1.6.9/meerschaum/__main__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/arguments/__init__.py` & `meerschaum-1.6.9/meerschaum/_internal/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/arguments/_parse_arguments.py` & `meerschaum-1.6.9/meerschaum/_internal/arguments/_parse_arguments.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/arguments/_parser.py` & `meerschaum-1.6.9/meerschaum/_internal/arguments/_parser.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/docs/index.py` & `meerschaum-1.6.9/meerschaum/_internal/docs/index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/entry.py` & `meerschaum-1.6.9/meerschaum/_internal/entry.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/gui/__init__.py` & `meerschaum-1.6.9/meerschaum/_internal/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/gui/app/__init__.py` & `meerschaum-1.6.9/meerschaum/_internal/gui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/gui/app/_windows.py` & `meerschaum-1.6.9/meerschaum/_internal/gui/app/_windows.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/gui/app/actions.py` & `meerschaum-1.6.9/meerschaum/_internal/gui/app/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/gui/app/pipes.py` & `meerschaum-1.6.9/meerschaum/_internal/gui/app/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/shell/Shell.py` & `meerschaum-1.6.9/meerschaum/_internal/shell/Shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/shell/ShellCompleter.py` & `meerschaum-1.6.9/meerschaum/_internal/shell/ShellCompleter.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/shell/ValidAutoSuggest.py` & `meerschaum-1.6.9/meerschaum/_internal/shell/ValidAutoSuggest.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/term/TermPageHandler.py` & `meerschaum-1.6.9/meerschaum/_internal/term/TermPageHandler.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/term/__init__.py` & `meerschaum-1.6.9/meerschaum/_internal/term/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/_internal/term/tools.py` & `meerschaum-1.6.9/meerschaum/_internal/term/tools.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/__init__.py` & `meerschaum-1.6.9/meerschaum/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/api.py` & `meerschaum-1.6.9/meerschaum/actions/api.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/bootstrap.py` & `meerschaum-1.6.9/meerschaum/actions/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/clear.py` & `meerschaum-1.6.9/meerschaum/actions/clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/copy.py` & `meerschaum-1.6.9/meerschaum/actions/copy.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/delete.py` & `meerschaum-1.6.9/meerschaum/actions/delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/drop.py` & `meerschaum-1.6.9/meerschaum/actions/drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/edit.py` & `meerschaum-1.6.9/meerschaum/actions/edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/install.py` & `meerschaum-1.6.9/meerschaum/actions/install.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/login.py` & `meerschaum-1.6.9/meerschaum/actions/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/os.py` & `meerschaum-1.6.9/meerschaum/actions/os.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/python.py` & `meerschaum-1.6.9/meerschaum/actions/python.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/register.py` & `meerschaum-1.6.9/meerschaum/actions/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/reload.py` & `meerschaum-1.6.9/meerschaum/actions/reload.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/setup.py` & `meerschaum-1.6.9/meerschaum/actions/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/sh.py` & `meerschaum-1.6.9/meerschaum/actions/sh.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/show.py` & `meerschaum-1.6.9/meerschaum/actions/show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/sql.py` & `meerschaum-1.6.9/meerschaum/actions/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/stack.py` & `meerschaum-1.6.9/meerschaum/actions/stack.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/start.py` & `meerschaum-1.6.9/meerschaum/actions/start.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/stop.py` & `meerschaum-1.6.9/meerschaum/actions/stop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/sync.py` & `meerschaum-1.6.9/meerschaum/actions/sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/uninstall.py` & `meerschaum-1.6.9/meerschaum/actions/uninstall.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/upgrade.py` & `meerschaum-1.6.9/meerschaum/actions/upgrade.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/actions/verify.py` & `meerschaum-1.6.9/meerschaum/actions/verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/__init__.py` & `meerschaum-1.6.9/meerschaum/api/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/_chain.py` & `meerschaum-1.6.9/meerschaum/api/_chain.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/_events.py` & `meerschaum-1.6.9/meerschaum/api/_events.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/_oauth2.py` & `meerschaum-1.6.9/meerschaum/api/_oauth2.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/_websockets.py` & `meerschaum-1.6.9/meerschaum/api/_websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/__init__.py` & `meerschaum-1.6.9/meerschaum/api/dash/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/actions.py` & `meerschaum-1.6.9/meerschaum/api/dash/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/assets/ansi_up.js` & `meerschaum-1.6.9/meerschaum/api/dash/assets/ansi_up.js`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/assets/banner_1920x320.png` & `meerschaum-1.6.9/meerschaum/api/dash/assets/banner_1920x320.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/assets/favicon.ico` & `meerschaum-1.6.9/meerschaum/api/dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/assets/logo_48x48.png` & `meerschaum-1.6.9/meerschaum/api/dash/assets/logo_48x48.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/assets/logo_500x500.png` & `meerschaum-1.6.9/meerschaum/api/dash/assets/logo_500x500.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/callbacks/dashboard.py` & `meerschaum-1.6.9/meerschaum/api/dash/callbacks/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/callbacks/login.py` & `meerschaum-1.6.9/meerschaum/api/dash/callbacks/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/callbacks/plugins.py` & `meerschaum-1.6.9/meerschaum/api/dash/callbacks/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/callbacks/register.py` & `meerschaum-1.6.9/meerschaum/api/dash/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/components.py` & `meerschaum-1.6.9/meerschaum/api/dash/components.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/connectors.py` & `meerschaum-1.6.9/meerschaum/api/dash/connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/graphs.py` & `meerschaum-1.6.9/meerschaum/api/dash/graphs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/jobs.py` & `meerschaum-1.6.9/meerschaum/api/dash/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/keys.py` & `meerschaum-1.6.9/meerschaum/api/dash/keys.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/pages/dashboard.py` & `meerschaum-1.6.9/meerschaum/api/dash/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/pages/error.py` & `meerschaum-1.6.9/meerschaum/api/dash/pages/error.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/pages/login.py` & `meerschaum-1.6.9/meerschaum/api/dash/pages/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/pages/plugins.py` & `meerschaum-1.6.9/meerschaum/api/dash/pages/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/pages/register.py` & `meerschaum-1.6.9/meerschaum/api/dash/pages/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/pipes.py` & `meerschaum-1.6.9/meerschaum/api/dash/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/plugins.py` & `meerschaum-1.6.9/meerschaum/api/dash/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/users.py` & `meerschaum-1.6.9/meerschaum/api/dash/users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/dash/websockets.py` & `meerschaum-1.6.9/meerschaum/api/dash/websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/resources/static/css/bootstrap.min.css` & `meerschaum-1.6.9/meerschaum/api/resources/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/resources/static/css/dash.css` & `meerschaum-1.6.9/meerschaum/api/resources/static/css/dash.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/resources/static/css/dbc_dark.css` & `meerschaum-1.6.9/meerschaum/api/resources/static/css/dbc_dark.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/resources/static/ico/logo.ico` & `meerschaum-1.6.9/meerschaum/api/resources/static/ico/logo.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/resources/static/js/action_button.js` & `meerschaum-1.6.9/meerschaum/api/resources/static/js/action_button.js`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/resources/templates/index.html` & `meerschaum-1.6.9/meerschaum/api/resources/templates/index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/resources/templates/old_index.html` & `meerschaum-1.6.9/meerschaum/api/resources/templates/old_index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/resources/templates/termpage.html` & `meerschaum-1.6.9/meerschaum/api/resources/templates/termpage.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/routes/__init__.py` & `meerschaum-1.6.9/meerschaum/api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/routes/_actions.py` & `meerschaum-1.6.9/meerschaum/api/routes/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/routes/_connectors.py` & `meerschaum-1.6.9/meerschaum/api/routes/_connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/routes/_index.py` & `meerschaum-1.6.9/meerschaum/api/routes/_index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/routes/_login.py` & `meerschaum-1.6.9/meerschaum/api/routes/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/routes/_misc.py` & `meerschaum-1.6.9/meerschaum/api/routes/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/routes/_pipes.py` & `meerschaum-1.6.9/meerschaum/api/routes/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/routes/_plugins.py` & `meerschaum-1.6.9/meerschaum/api/routes/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/routes/_users.py` & `meerschaum-1.6.9/meerschaum/api/routes/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/routes/_version.py` & `meerschaum-1.6.9/meerschaum/api/routes/_version.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/api/tables/__init__.py` & `meerschaum-1.6.9/meerschaum/api/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/__init__.py` & `meerschaum-1.6.9/meerschaum/config/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/_default.py` & `meerschaum-1.6.9/meerschaum/config/_default.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/_edit.py` & `meerschaum-1.6.9/meerschaum/config/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/_environment.py` & `meerschaum-1.6.9/meerschaum/config/_environment.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/_formatting.py` & `meerschaum-1.6.9/meerschaum/config/_formatting.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/_jobs.py` & `meerschaum-1.6.9/meerschaum/config/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/_patch.py` & `meerschaum-1.6.9/meerschaum/config/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/_paths.py` & `meerschaum-1.6.9/meerschaum/config/_paths.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/_preprocess.py` & `meerschaum-1.6.9/meerschaum/config/_preprocess.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/_read_config.py` & `meerschaum-1.6.9/meerschaum/config/_read_config.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/_shell.py` & `meerschaum-1.6.9/meerschaum/config/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/_sync.py` & `meerschaum-1.6.9/meerschaum/config/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/stack/__init__.py` & `meerschaum-1.6.9/meerschaum/config/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/stack/grafana/__init__.py` & `meerschaum-1.6.9/meerschaum/config/stack/grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/config/static/__init__.py` & `meerschaum-1.6.9/meerschaum/config/static/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/Connector.py` & `meerschaum-1.6.9/meerschaum/connectors/Connector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/__init__.py` & `meerschaum-1.6.9/meerschaum/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/api/APIConnector.py` & `meerschaum-1.6.9/meerschaum/connectors/api/APIConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/api/_actions.py` & `meerschaum-1.6.9/meerschaum/connectors/api/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/api/_delete.py` & `meerschaum-1.6.9/meerschaum/connectors/api/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/api/_fetch.py` & `meerschaum-1.6.9/meerschaum/connectors/api/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/api/_get.py` & `meerschaum-1.6.9/meerschaum/connectors/api/_get.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/api/_login.py` & `meerschaum-1.6.9/meerschaum/connectors/api/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/api/_misc.py` & `meerschaum-1.6.9/meerschaum/connectors/api/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/api/_patch.py` & `meerschaum-1.6.9/meerschaum/connectors/api/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/api/_pipes.py` & `meerschaum-1.6.9/meerschaum/connectors/api/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/api/_plugins.py` & `meerschaum-1.6.9/meerschaum/connectors/api/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/api/_post.py` & `meerschaum-1.6.9/meerschaum/connectors/api/_post.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/api/_uri.py` & `meerschaum-1.6.9/meerschaum/connectors/api/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/api/_users.py` & `meerschaum-1.6.9/meerschaum/connectors/api/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/parse.py` & `meerschaum-1.6.9/meerschaum/connectors/parse.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/plugin/PluginConnector.py` & `meerschaum-1.6.9/meerschaum/connectors/plugin/PluginConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/poll.py` & `meerschaum-1.6.9/meerschaum/connectors/poll.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/sql/SQLConnector.py` & `meerschaum-1.6.9/meerschaum/connectors/sql/SQLConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/sql/_cli.py` & `meerschaum-1.6.9/meerschaum/connectors/sql/_cli.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/sql/_create_engine.py` & `meerschaum-1.6.9/meerschaum/connectors/sql/_create_engine.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/sql/_fetch.py` & `meerschaum-1.6.9/meerschaum/connectors/sql/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/sql/_pipes.py` & `meerschaum-1.6.9/meerschaum/connectors/sql/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/sql/_plugins.py` & `meerschaum-1.6.9/meerschaum/connectors/sql/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/sql/_sql.py` & `meerschaum-1.6.9/meerschaum/connectors/sql/_sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/sql/_uri.py` & `meerschaum-1.6.9/meerschaum/connectors/sql/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/sql/_users.py` & `meerschaum-1.6.9/meerschaum/connectors/sql/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/sql/tables/__init__.py` & `meerschaum-1.6.9/meerschaum/connectors/sql/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/connectors/sql/tables/types.py` & `meerschaum-1.6.9/meerschaum/connectors/sql/tables/types.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/core/Pipe/__init__.py` & `meerschaum-1.6.9/meerschaum/core/Pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/core/Pipe/_attributes.py` & `meerschaum-1.6.9/meerschaum/core/Pipe/_attributes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/core/Pipe/_bootstrap.py` & `meerschaum-1.6.9/meerschaum/core/Pipe/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/core/Pipe/_clear.py` & `meerschaum-1.6.9/meerschaum/core/Pipe/_clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/core/Pipe/_data.py` & `meerschaum-1.6.9/meerschaum/core/Pipe/_data.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/core/Pipe/_delete.py` & `meerschaum-1.6.9/meerschaum/core/Pipe/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/core/Pipe/_drop.py` & `meerschaum-1.6.9/meerschaum/core/Pipe/_drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/core/Pipe/_dtypes.py` & `meerschaum-1.6.9/meerschaum/core/Pipe/_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/core/Pipe/_edit.py` & `meerschaum-1.6.9/meerschaum/core/Pipe/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/core/Pipe/_fetch.py` & `meerschaum-1.6.9/meerschaum/core/Pipe/_fetch.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,19 +61,21 @@
         )
         connector_plugin = Plugin(plugin_name)
         connector_plugin.activate_venv(debug=debug)
     
     _chunk_hook = kw.pop('chunk_hook', None)
     if sync_chunks and _chunk_hook is None:
 
-        def _chunk_hook(chunk, **kw) -> SuccessTuple:
+        def _chunk_hook(chunk, **_kw) -> SuccessTuple:
             """
             Wrap `Pipe.sync()` with a custom chunk label prepended to the message.
             """
-            chunk_success, chunk_message = self.sync(chunk, **kw)
+            from meerschaum.config._patch import apply_patch_to_config
+            kwargs = apply_patch_to_config(kw, _kw)
+            chunk_success, chunk_message = self.sync(chunk, **kwargs)
             chunk_label = self._get_chunk_label(chunk, self.columns.get('datetime', None))
             if chunk_label:
                 chunk_message = '\n' + chunk_label + '\n' + chunk_message
             return chunk_success, chunk_message
 
     df = self.connector.fetch(
         self,
```

### Comparing `meerschaum-1.6.8/meerschaum/core/Pipe/_register.py` & `meerschaum-1.6.9/meerschaum/core/Pipe/_register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/core/Pipe/_show.py` & `meerschaum-1.6.9/meerschaum/core/Pipe/_show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/core/Pipe/_sync.py` & `meerschaum-1.6.9/meerschaum/core/Pipe/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/core/User/_User.py` & `meerschaum-1.6.9/meerschaum/core/User/_User.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/plugins/_Plugin.py` & `meerschaum-1.6.9/meerschaum/plugins/_Plugin.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/plugins/__init__.py` & `meerschaum-1.6.9/meerschaum/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/daemon/Daemon.py` & `meerschaum-1.6.9/meerschaum/utils/daemon/Daemon.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/daemon/Log.py` & `meerschaum-1.6.9/meerschaum/utils/daemon/Log.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/daemon/__init__.py` & `meerschaum-1.6.9/meerschaum/utils/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/daemon/_names.py` & `meerschaum-1.6.9/meerschaum/utils/daemon/_names.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/debug.py` & `meerschaum-1.6.9/meerschaum/utils/debug.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/formatting/__init__.py` & `meerschaum-1.6.9/meerschaum/utils/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/formatting/_jobs.py` & `meerschaum-1.6.9/meerschaum/utils/formatting/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/formatting/_pipes.py` & `meerschaum-1.6.9/meerschaum/utils/formatting/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/formatting/_pprint.py` & `meerschaum-1.6.9/meerschaum/utils/formatting/_pprint.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/formatting/_shell.py` & `meerschaum-1.6.9/meerschaum/utils/formatting/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/get_pipes.py` & `meerschaum-1.6.9/meerschaum/utils/get_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/interactive.py` & `meerschaum-1.6.9/meerschaum/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/misc.py` & `meerschaum-1.6.9/meerschaum/utils/misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/networking.py` & `meerschaum-1.6.9/meerschaum/utils/networking.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/packages/__init__.py` & `meerschaum-1.6.9/meerschaum/utils/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/packages/_packages.py` & `meerschaum-1.6.9/meerschaum/utils/packages/_packages.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/packages/lazy_loader.py` & `meerschaum-1.6.9/meerschaum/utils/packages/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/pool.py` & `meerschaum-1.6.9/meerschaum/utils/pool.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/process.py` & `meerschaum-1.6.9/meerschaum/utils/process.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/prompt.py` & `meerschaum-1.6.9/meerschaum/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/schedule.py` & `meerschaum-1.6.9/meerschaum/utils/schedule.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/sql.py` & `meerschaum-1.6.9/meerschaum/utils/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/threading.py` & `meerschaum-1.6.9/meerschaum/utils/threading.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/typing.py` & `meerschaum-1.6.9/meerschaum/utils/typing.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/venv/_Venv.py` & `meerschaum-1.6.9/meerschaum/utils/venv/_Venv.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/venv/__init__.py` & `meerschaum-1.6.9/meerschaum/utils/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/warnings.py` & `meerschaum-1.6.9/meerschaum/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum/utils/yaml.py` & `meerschaum-1.6.9/meerschaum/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum.egg-info/PKG-INFO` & `meerschaum-1.6.9/meerschaum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 1.6.8
+Version: 1.6.9
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
```

### Comparing `meerschaum-1.6.8/meerschaum.egg-info/SOURCES.txt` & `meerschaum-1.6.9/meerschaum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/meerschaum.egg-info/requires.txt` & `meerschaum-1.6.9/meerschaum.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.8/setup.py` & `meerschaum-1.6.9/setup.py`

 * *Files identical despite different names*

