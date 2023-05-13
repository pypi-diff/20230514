# Comparing `tmp/Tailbone-0.9.8.tar.gz` & `tmp/Tailbone-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/lance/src/tailbone/dist/tmpbkg6q3jt/Tailbone-0.9.8.tar", last modified: Tue Feb 21 03:51:05 2023, max compression
+gzip compressed data, was "/home/lance/src/tailbone/dist/tmpqyoluhzt/Tailbone-0.9.9.tar", last modified: Wed Feb 22 01:14:55 2023, max compression
```

## Comparing `Tailbone-0.9.8.tar` & `Tailbone-0.9.9.tar`

### file list

```diff
@@ -1,502 +1,502 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:05.000000 Tailbone-0.9.8/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/
--rw-r--r--   0 lance     (1000) lance     (1000)    10342 2023-02-12 03:10:54.000000 Tailbone-0.9.8/tailbone/subscribers.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/reports/
--rw-r--r--   0 lance     (1000) lance     (1000)     3577 2023-02-03 22:10:08.000000 Tailbone-0.9.8/tailbone/reports/ordering_worksheet.mako
--rw-rw-r--   0 lance     (1000) lance     (1000)     2481 2016-12-17 08:48:19.000000 Tailbone-0.9.8/tailbone/reports/inventory_worksheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1632 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/scaffolds.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/grids/
--rw-r--r--   0 lance     (1000) lance     (1000)    39197 2023-02-14 23:30:56.000000 Tailbone-0.9.8/tailbone/grids/filters.py
--rw-r--r--   0 lance     (1000) lance     (1000)    62419 2023-02-14 23:31:26.000000 Tailbone-0.9.8/tailbone/grids/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1077 2021-01-30 20:30:05.000000 Tailbone-0.9.8/tailbone/grids/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    28553 2023-02-04 01:48:39.000000 Tailbone-0.9.8/tailbone/menus.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2691 2022-12-24 05:29:45.000000 Tailbone-0.9.8/tailbone/cleanup.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8274 2023-02-07 18:19:37.000000 Tailbone-0.9.8/tailbone/db.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/
--rw-r--r--   0 lance     (1000) lance     (1000)     2518 2023-02-02 22:24:46.000000 Tailbone-0.9.8/tailbone/templates/feedback_dialog_buefy.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/reports/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/reports/generated/
--rw-r--r--   0 lance     (1000) lance     (1000)      691 2023-02-03 05:22:09.000000 Tailbone-0.9.8/tailbone/templates/reports/generated/generate.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1082 2022-11-28 23:53:29.000000 Tailbone-0.9.8/tailbone/templates/reports/generated/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      346 2021-12-15 01:04:51.000000 Tailbone-0.9.8/tailbone/templates/reports/generated/delete.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1817 2023-02-03 05:22:38.000000 Tailbone-0.9.8/tailbone/templates/reports/generated/choose.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      635 2022-01-08 19:00:03.000000 Tailbone-0.9.8/tailbone/templates/reports/generated/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/reports/problems/
--rw-r--r--   0 lance     (1000) lance     (1000)     2397 2022-11-19 18:52:15.000000 Tailbone-0.9.8/tailbone/templates/reports/problems/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3202 2023-02-03 22:10:08.000000 Tailbone-0.9.8/tailbone/templates/reports/ordering.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1365 2023-02-03 22:10:08.000000 Tailbone-0.9.8/tailbone/templates/reports/inventory.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/principal/
--rw-r--r--   0 lance     (1000) lance     (1000)     3926 2023-02-03 05:23:45.000000 Tailbone-0.9.8/tailbone/templates/principal/find_by_perm.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      369 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/principal/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/grids/
--rw-r--r--   0 lance     (1000) lance     (1000)      755 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/grids/nav.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    21371 2023-02-10 19:06:04.000000 Tailbone-0.9.8/tailbone/templates/grids/buefy.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1584 2022-12-25 20:38:13.000000 Tailbone-0.9.8/tailbone/templates/grids/filters_buefy.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1573 2019-05-06 23:17:43.000000 Tailbone-0.9.8/tailbone/templates/grids/filters.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      910 2018-09-23 00:20:31.000000 Tailbone-0.9.8/tailbone/templates/grids/grid.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3024 2023-02-02 00:24:21.000000 Tailbone-0.9.8/tailbone/templates/grids/b-table.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      795 2019-04-15 23:05:35.000000 Tailbone-0.9.8/tailbone/templates/grids/complete.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/tables/
--rw-r--r--   0 lance     (1000) lance     (1000)    30330 2023-02-02 00:25:12.000000 Tailbone-0.9.8/tailbone/templates/tables/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1518 2023-02-02 22:24:46.000000 Tailbone-0.9.8/tailbone/templates/feedback.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1509 2023-01-29 17:00:34.000000 Tailbone-0.9.8/tailbone/templates/multi_file_upload.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1686 2023-02-02 22:24:46.000000 Tailbone-0.9.8/tailbone/templates/menu.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/vendors/
--rw-r--r--   0 lance     (1000) lance     (1000)     1850 2022-05-15 21:04:06.000000 Tailbone-0.9.8/tailbone/templates/vendors/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/users/
--rw-r--r--   0 lance     (1000) lance     (1000)      481 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/users/find_by_perm.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1314 2022-02-15 02:30:15.000000 Tailbone-0.9.8/tailbone/templates/users/preferences.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      655 2022-02-14 23:08:35.000000 Tailbone-0.9.8/tailbone/templates/users/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/labels/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/labels/profiles/
--rw-r--r--   0 lance     (1000) lance     (1000)      432 2019-05-23 22:57:42.000000 Tailbone-0.9.8/tailbone/templates/labels/profiles/printer.mako
--rw-rw-r--   0 lance     (1000) lance     (1000)      314 2016-12-17 08:48:19.000000 Tailbone-0.9.8/tailbone/templates/labels/profiles/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1232 2023-02-09 02:19:12.000000 Tailbone-0.9.8/tailbone/templates/labels/profiles/view.mako
--rw-rw-r--   0 lance     (1000) lance     (1000)      620 2016-12-17 08:48:19.000000 Tailbone-0.9.8/tailbone/templates/labels/profiles/edit.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/master/
--rw-r--r--   0 lance     (1000) lance     (1000)      879 2021-12-13 19:43:47.000000 Tailbone-0.9.8/tailbone/templates/master/edit_row.mako
--rw-rw-r--   0 lance     (1000) lance     (1000)      248 2016-12-17 08:48:19.000000 Tailbone-0.9.8/tailbone/templates/master/create_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      174 2019-05-22 20:24:53.000000 Tailbone-0.9.8/tailbone/templates/master/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     5610 2023-02-03 05:24:29.000000 Tailbone-0.9.8/tailbone/templates/master/merge.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      584 2023-02-03 18:10:14.000000 Tailbone-0.9.8/tailbone/templates/master/form.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3266 2021-05-14 17:13:11.000000 Tailbone-0.9.8/tailbone/templates/master/view_version.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1033 2023-02-03 22:16:07.000000 Tailbone-0.9.8/tailbone/templates/master/versions.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3058 2023-02-03 18:11:06.000000 Tailbone-0.9.8/tailbone/templates/master/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      170 2018-11-23 00:24:59.000000 Tailbone-0.9.8/tailbone/templates/master/import_file.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1401 2023-02-03 05:26:22.000000 Tailbone-0.9.8/tailbone/templates/master/delete.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      709 2023-02-03 05:26:29.000000 Tailbone-0.9.8/tailbone/templates/master/view_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    23855 2023-02-03 05:29:08.000000 Tailbone-0.9.8/tailbone/templates/master/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      136 2023-02-03 18:11:06.000000 Tailbone-0.9.8/tailbone/templates/master/edit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      893 2021-12-14 03:26:58.000000 Tailbone-0.9.8/tailbone/templates/master/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1376 2023-02-03 05:30:32.000000 Tailbone-0.9.8/tailbone/templates/master/clone.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1681 2023-02-03 03:16:55.000000 Tailbone-0.9.8/tailbone/templates/page.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/purchases/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/purchases/batches/
--rw-r--r--   0 lance     (1000) lance     (1000)      117 2023-02-03 22:16:48.000000 Tailbone-0.9.8/tailbone/templates/purchases/batches/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      278 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/purchases/batches/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/purchases/credits/
--rw-r--r--   0 lance     (1000) lance     (1000)     2469 2023-02-03 23:08:13.000000 Tailbone-0.9.8/tailbone/templates/purchases/credits/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      555 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/purchases/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2630 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/purchases/receiving_worksheet.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/roles/
--rw-r--r--   0 lance     (1000) lance     (1000)      407 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/roles/find_by_perm.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      536 2020-07-17 00:43:21.000000 Tailbone-0.9.8/tailbone/templates/roles/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      867 2023-02-03 05:30:47.000000 Tailbone-0.9.8/tailbone/templates/roles/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      330 2020-06-22 20:36:16.000000 Tailbone-0.9.8/tailbone/templates/roles/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      541 2020-06-22 19:53:23.000000 Tailbone-0.9.8/tailbone/templates/roles/edit.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/custorders/
--rw-r--r--   0 lance     (1000) lance     (1000)    88160 2023-02-03 05:31:02.000000 Tailbone-0.9.8/tailbone/templates/custorders/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     5225 2023-01-11 21:38:41.000000 Tailbone-0.9.8/tailbone/templates/custorders/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/custorders/items/
--rw-r--r--   0 lance     (1000) lance     (1000)    14412 2023-02-02 00:28:24.000000 Tailbone-0.9.8/tailbone/templates/custorders/items/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/departments/
--rw-rw-r--   0 lance     (1000) lance     (1000)      294 2023-02-03 05:31:15.000000 Tailbone-0.9.8/tailbone/templates/departments/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/receiving/
--rw-r--r--   0 lance     (1000) lance     (1000)     1495 2023-02-03 05:31:39.000000 Tailbone-0.9.8/tailbone/templates/receiving/declare_credit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      117 2023-02-03 05:32:11.000000 Tailbone-0.9.8/tailbone/templates/receiving/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1400 2023-02-03 05:32:35.000000 Tailbone-0.9.8/tailbone/templates/receiving/receive_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      305 2018-10-24 22:53:24.000000 Tailbone-0.9.8/tailbone/templates/receiving/transform_unit_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    10589 2023-02-10 19:06:04.000000 Tailbone-0.9.8/tailbone/templates/receiving/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    21656 2023-02-03 05:33:59.000000 Tailbone-0.9.8/tailbone/templates/receiving/view_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     7274 2023-01-08 17:38:39.000000 Tailbone-0.9.8/tailbone/templates/receiving/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/messages/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/messages/archive/
--rw-r--r--   0 lance     (1000) lance     (1000)      353 2023-02-03 05:34:09.000000 Tailbone-0.9.8/tailbone/templates/messages/archive/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1364 2023-02-03 05:34:56.000000 Tailbone-0.9.8/tailbone/templates/messages/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3206 2023-02-03 05:35:31.000000 Tailbone-0.9.8/tailbone/templates/messages/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/messages/sent/
--rw-rw-r--   0 lance     (1000) lance     (1000)      354 2016-12-17 08:48:19.000000 Tailbone-0.9.8/tailbone/templates/messages/sent/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1101 2019-11-05 01:03:51.000000 Tailbone-0.9.8/tailbone/templates/messages/recipients.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1761 2023-02-03 05:35:48.000000 Tailbone-0.9.8/tailbone/templates/messages/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/messages/inbox/
--rw-r--r--   0 lance     (1000) lance     (1000)      355 2023-02-03 05:35:57.000000 Tailbone-0.9.8/tailbone/templates/messages/inbox/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/forms/
--rw-r--r--   0 lance     (1000) lance     (1000)       67 2023-02-03 05:36:08.000000 Tailbone-0.9.8/tailbone/templates/forms/form.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     6607 2023-01-29 16:59:34.000000 Tailbone-0.9.8/tailbone/templates/forms/deform_buefy.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      265 2022-08-09 03:19:59.000000 Tailbone-0.9.8/tailbone/templates/forms/util.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1603 2023-02-03 05:36:20.000000 Tailbone-0.9.8/tailbone/templates/form.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/customers/
--rw-r--r--   0 lance     (1000) lance     (1000)     1056 2023-02-03 22:36:48.000000 Tailbone-0.9.8/tailbone/templates/customers/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/customers/pending/
--rw-r--r--   0 lance     (1000) lance     (1000)     5021 2021-12-24 01:59:01.000000 Tailbone-0.9.8/tailbone/templates/customers/pending/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1075 2022-08-09 04:37:20.000000 Tailbone-0.9.8/tailbone/templates/customers/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/employees/
--rw-r--r--   0 lance     (1000) lance     (1000)      259 2019-04-12 19:47:07.000000 Tailbone-0.9.8/tailbone/templates/employees/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      899 2023-02-03 22:40:11.000000 Tailbone-0.9.8/tailbone/templates/autocomplete.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1170 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/exception.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/luigi/
--rw-r--r--   0 lance     (1000) lance     (1000)    12842 2023-02-02 00:29:33.000000 Tailbone-0.9.8/tailbone/templates/luigi/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    14033 2023-02-02 00:30:45.000000 Tailbone-0.9.8/tailbone/templates/luigi/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/appinfo/
--rw-r--r--   0 lance     (1000) lance     (1000)     3235 2023-02-02 00:31:07.000000 Tailbone-0.9.8/tailbone/templates/appinfo/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     7318 2023-02-02 00:31:53.000000 Tailbone-0.9.8/tailbone/templates/appinfo/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/ordering/
--rw-r--r--   0 lance     (1000) lance     (1000)      112 2023-02-03 05:36:48.000000 Tailbone-0.9.8/tailbone/templates/ordering/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    16377 2021-02-01 03:51:46.000000 Tailbone-0.9.8/tailbone/templates/ordering/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    11560 2023-02-03 05:37:47.000000 Tailbone-0.9.8/tailbone/templates/ordering/worksheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1649 2023-02-07 22:11:44.000000 Tailbone-0.9.8/tailbone/templates/login.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/shifts/
--rw-r--r--   0 lance     (1000) lance     (1000)     1463 2023-02-03 22:42:48.000000 Tailbone-0.9.8/tailbone/templates/shifts/timesheet_edit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      900 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/shifts/schedule_print.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2538 2023-02-03 22:44:07.000000 Tailbone-0.9.8/tailbone/templates/shifts/schedule_edit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      813 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/shifts/schedule_print_employee.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     6116 2023-02-03 22:43:25.000000 Tailbone-0.9.8/tailbone/templates/shifts/base.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1025 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/shifts/schedule.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      833 2023-02-03 22:45:27.000000 Tailbone-0.9.8/tailbone/templates/shifts/timesheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    13008 2023-01-17 03:55:16.000000 Tailbone-0.9.8/tailbone/templates/configure-menus.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      471 2019-08-03 00:53:47.000000 Tailbone-0.9.8/tailbone/templates/about.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/upgrades/
--rw-r--r--   0 lance     (1000) lance     (1000)     9414 2023-02-03 22:10:08.000000 Tailbone-0.9.8/tailbone/templates/upgrades/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     5196 2023-02-02 00:32:20.000000 Tailbone-0.9.8/tailbone/templates/upgrades/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/views/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/views/model/
--rw-r--r--   0 lance     (1000) lance     (1000)     9427 2023-01-16 19:50:05.000000 Tailbone-0.9.8/tailbone/templates/views/model/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    32847 2023-02-04 00:05:40.000000 Tailbone-0.9.8/tailbone/templates/base.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      797 2023-02-03 05:38:48.000000 Tailbone-0.9.8/tailbone/templates/util.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1066 2023-02-02 22:24:46.000000 Tailbone-0.9.8/tailbone/templates/feedback_dialog.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/email-bounces/
--rw-r--r--   0 lance     (1000) lance     (1000)     1667 2023-02-03 23:03:42.000000 Tailbone-0.9.8/tailbone/templates/email-bounces/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/workorders/
--rw-r--r--   0 lance     (1000) lance     (1000)     7838 2022-08-10 02:05:11.000000 Tailbone-0.9.8/tailbone/templates/workorders/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2776 2023-01-19 03:56:10.000000 Tailbone-0.9.8/tailbone/templates/formposter.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/people/
--rw-r--r--   0 lance     (1000) lance     (1000)    58478 2023-02-02 00:34:18.000000 Tailbone-0.9.8/tailbone/templates/people/view_profile_buefy.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1106 2023-02-03 05:39:41.000000 Tailbone-0.9.8/tailbone/templates/people/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/people/merge-requests/
--rw-r--r--   0 lance     (1000) lance     (1000)     1183 2023-02-03 05:39:54.000000 Tailbone-0.9.8/tailbone/templates/people/merge-requests/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3654 2023-02-03 05:40:07.000000 Tailbone-0.9.8/tailbone/templates/people/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/ifps-plu-codes/
--rw-r--r--   0 lance     (1000) lance     (1000)      281 2020-12-07 01:28:53.000000 Tailbone-0.9.8/tailbone/templates/ifps-plu-codes/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      672 2019-08-24 02:39:03.000000 Tailbone-0.9.8/tailbone/templates/home.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/tempmon/
--rw-r--r--   0 lance     (1000) lance     (1000)     3718 2023-02-03 05:40:48.000000 Tailbone-0.9.8/tailbone/templates/tempmon/dashboard.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/tempmon/readings/
--rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:17:35.000000 Tailbone-0.9.8/tailbone/templates/tempmon/readings/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/tempmon/probes/
--rw-r--r--   0 lance     (1000) lance     (1000)     3298 2023-02-03 05:41:19.000000 Tailbone-0.9.8/tailbone/templates/tempmon/probes/graph.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3149 2023-02-03 05:41:51.000000 Tailbone-0.9.8/tailbone/templates/tempmon/probes/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:18:44.000000 Tailbone-0.9.8/tailbone/templates/tempmon/probes/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/tempmon/appliances/
--rw-r--r--   0 lance     (1000) lance     (1000)      510 2023-01-14 00:38:46.000000 Tailbone-0.9.8/tailbone/templates/tempmon/appliances/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      736 2020-04-05 00:31:41.000000 Tailbone-0.9.8/tailbone/templates/tempmon/appliances/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/tempmon/clients/
--rw-r--r--   0 lance     (1000) lance     (1000)     1044 2023-02-03 05:42:03.000000 Tailbone-0.9.8/tailbone/templates/tempmon/clients/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:17:35.000000 Tailbone-0.9.8/tailbone/templates/tempmon/clients/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/batch/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/batch/vendorcatalog/
--rw-r--r--   0 lance     (1000) lance     (1000)     1288 2023-02-03 05:42:10.000000 Tailbone-0.9.8/tailbone/templates/batch/vendorcatalog/create.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      247 2022-01-06 20:44:32.000000 Tailbone-0.9.8/tailbone/templates/batch/vendorcatalog/view_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      309 2022-01-06 18:52:39.000000 Tailbone-0.9.8/tailbone/templates/batch/vendorcatalog/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1388 2022-01-08 19:35:47.000000 Tailbone-0.9.8/tailbone/templates/batch/vendorcatalog/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/batch/inventory/
--rw-r--r--   0 lance     (1000) lance     (1000)     8881 2023-02-03 05:42:38.000000 Tailbone-0.9.8/tailbone/templates/batch/inventory/desktop_form.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/batch/newproduct/
--rw-r--r--   0 lance     (1000) lance     (1000)      160 2022-08-30 15:56:25.000000 Tailbone-0.9.8/tailbone/templates/batch/newproduct/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/batch/pricing/
--rw-r--r--   0 lance     (1000) lance     (1000)      536 2022-06-14 18:18:31.000000 Tailbone-0.9.8/tailbone/templates/batch/pricing/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       84 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/batch/create.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/batch/importer/
--rw-r--r--   0 lance     (1000) lance     (1000)     2387 2023-02-03 05:42:46.000000 Tailbone-0.9.8/tailbone/templates/batch/importer/view_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    11873 2023-02-03 05:50:11.000000 Tailbone-0.9.8/tailbone/templates/batch/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      509 2023-02-03 05:50:25.000000 Tailbone-0.9.8/tailbone/templates/batch/worksheet.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     4716 2023-02-03 05:51:09.000000 Tailbone-0.9.8/tailbone/templates/batch/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       81 2019-06-08 19:26:19.000000 Tailbone-0.9.8/tailbone/templates/batch/edit.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      121 2020-03-24 00:26:09.000000 Tailbone-0.9.8/tailbone/templates/change_password.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/deform/
--rw-r--r--   0 lance     (1000) lance     (1000)     1213 2023-02-03 05:51:23.000000 Tailbone-0.9.8/tailbone/templates/deform/checked_password.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     2164 2023-02-03 05:51:49.000000 Tailbone-0.9.8/tailbone/templates/deform/select.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      710 2023-02-03 05:52:00.000000 Tailbone-0.9.8/tailbone/templates/deform/percentinput.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      257 2023-01-29 16:59:23.000000 Tailbone-0.9.8/tailbone/templates/deform/multi_file_upload.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      918 2023-02-03 05:52:17.000000 Tailbone-0.9.8/tailbone/templates/deform/autocomplete_jquery.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     1979 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/deform/select_jquery.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      509 2019-06-28 17:09:23.000000 Tailbone-0.9.8/tailbone/templates/deform/numericinput.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      758 2023-02-03 05:52:34.000000 Tailbone-0.9.8/tailbone/templates/deform/file_upload.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      545 2021-01-06 00:19:12.000000 Tailbone-0.9.8/tailbone/templates/deform/checkbox_dynamic.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      894 2023-02-04 01:42:19.000000 Tailbone-0.9.8/tailbone/templates/deform/textinput.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      943 2023-02-03 05:53:06.000000 Tailbone-0.9.8/tailbone/templates/deform/cases_units.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      616 2023-02-07 22:10:56.000000 Tailbone-0.9.8/tailbone/templates/deform/password.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      963 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/templates/deform/numberinput.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      655 2023-02-03 05:53:32.000000 Tailbone-0.9.8/tailbone/templates/deform/time_jquery.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      601 2019-11-04 23:21:16.000000 Tailbone-0.9.8/tailbone/templates/deform/message_recipients_buefy.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      597 2023-02-03 05:53:42.000000 Tailbone-0.9.8/tailbone/templates/deform/date_jquery.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      481 2023-02-03 05:53:52.000000 Tailbone-0.9.8/tailbone/templates/deform/textarea.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      581 2019-02-23 02:44:18.000000 Tailbone-0.9.8/tailbone/templates/deform/date_plain.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     2102 2023-02-03 05:54:03.000000 Tailbone-0.9.8/tailbone/templates/deform/permissions.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     1160 2022-07-21 02:27:26.000000 Tailbone-0.9.8/tailbone/templates/deform/select_dynamic.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      492 2023-02-03 05:54:15.000000 Tailbone-0.9.8/tailbone/templates/deform/checkbox.pt
--rw-r--r--   0 lance     (1000) lance     (1000)      875 2022-11-19 23:40:01.000000 Tailbone-0.9.8/tailbone/templates/deform/problem_report_days.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     1718 2019-09-06 22:13:34.000000 Tailbone-0.9.8/tailbone/templates/deform/select_plain.pt
--rw-r--r--   0 lance     (1000) lance     (1000)     7512 2022-12-28 04:29:27.000000 Tailbone-0.9.8/tailbone/templates/page_help.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      772 2021-11-04 22:56:35.000000 Tailbone-0.9.8/tailbone/templates/base_meta.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/datasync/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/datasync/changes/
--rw-r--r--   0 lance     (1000) lance     (1000)     2125 2023-02-03 05:54:34.000000 Tailbone-0.9.8/tailbone/templates/datasync/changes/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     5964 2023-02-02 00:35:51.000000 Tailbone-0.9.8/tailbone/templates/datasync/status.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    31019 2023-02-02 00:43:40.000000 Tailbone-0.9.8/tailbone/templates/datasync/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/members/
--rw-r--r--   0 lance     (1000) lance     (1000)      527 2020-03-18 18:02:17.000000 Tailbone-0.9.8/tailbone/templates/members/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      541 2019-06-15 23:03:40.000000 Tailbone-0.9.8/tailbone/templates/diff.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     6314 2023-02-03 05:54:56.000000 Tailbone-0.9.8/tailbone/templates/appsettings.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    12583 2023-02-02 00:37:54.000000 Tailbone-0.9.8/tailbone/templates/generate_feature.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     9425 2023-01-16 17:56:04.000000 Tailbone-0.9.8/tailbone/templates/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/poser/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/poser/reports/
--rw-r--r--   0 lance     (1000) lance     (1000)     2382 2022-03-04 00:35:18.000000 Tailbone-0.9.8/tailbone/templates/poser/reports/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3917 2022-03-21 22:32:51.000000 Tailbone-0.9.8/tailbone/templates/poser/setup.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/poser/views/
--rw-r--r--   0 lance     (1000) lance     (1000)     1120 2022-03-21 22:32:51.000000 Tailbone-0.9.8/tailbone/templates/poser/views/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1736 2023-02-03 22:10:08.000000 Tailbone-0.9.8/tailbone/templates/upgrade.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)      671 2021-12-07 03:21:19.000000 Tailbone-0.9.8/tailbone/templates/importing/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2643 2021-12-07 03:29:19.000000 Tailbone-0.9.8/tailbone/templates/importing/runjob.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      294 2021-12-06 18:34:10.000000 Tailbone-0.9.8/tailbone/templates/importing/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     6187 2023-02-02 00:43:01.000000 Tailbone-0.9.8/tailbone/templates/importing/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/settings/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/settings/email/
--rw-r--r--   0 lance     (1000) lance     (1000)     3013 2023-02-03 05:55:09.000000 Tailbone-0.9.8/tailbone/templates/settings/email/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1923 2022-08-06 23:37:28.000000 Tailbone-0.9.8/tailbone/templates/settings/email/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2579 2022-08-07 22:50:36.000000 Tailbone-0.9.8/tailbone/templates/settings/email/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    16343 2022-12-24 02:06:19.000000 Tailbone-0.9.8/tailbone/templates/generate_project.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/products/
--rw-r--r--   0 lance     (1000) lance     (1000)     3760 2023-02-03 06:21:59.000000 Tailbone-0.9.8/tailbone/templates/products/batch.mako
--rw-r--r--   0 lance     (1000) lance     (1000)    13299 2023-02-11 03:23:43.000000 Tailbone-0.9.8/tailbone/templates/products/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     8743 2023-02-02 00:39:33.000000 Tailbone-0.9.8/tailbone/templates/products/lookup.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/products/pending/
--rw-r--r--   0 lance     (1000) lance     (1000)     4435 2021-12-24 01:58:50.000000 Tailbone-0.9.8/tailbone/templates/products/pending/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2929 2023-02-03 05:58:51.000000 Tailbone-0.9.8/tailbone/templates/products/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     4184 2023-02-10 18:21:07.000000 Tailbone-0.9.8/tailbone/templates/products/configure.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/themes/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/themes/falafel/
--rw-r--r--   0 lance     (1000) lance     (1000)       93 2023-02-03 22:10:08.000000 Tailbone-0.9.8/tailbone/templates/themes/falafel/base.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       96 2023-02-03 22:10:08.000000 Tailbone-0.9.8/tailbone/templates/themes/falafel/upgrade.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       97 2023-02-03 22:10:08.000000 Tailbone-0.9.8/tailbone/templates/themes/falafel/progress.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/units-of-measure/
--rw-r--r--   0 lance     (1000) lance     (1000)     1899 2021-01-27 14:56:25.000000 Tailbone-0.9.8/tailbone/templates/units-of-measure/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/trainwreck/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/templates/trainwreck/transactions/
--rw-r--r--   0 lance     (1000) lance     (1000)     1625 2023-02-02 00:39:56.000000 Tailbone-0.9.8/tailbone/templates/trainwreck/transactions/rollover.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      389 2022-03-17 21:59:40.000000 Tailbone-0.9.8/tailbone/templates/trainwreck/transactions/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      357 2022-02-19 22:34:34.000000 Tailbone-0.9.8/tailbone/templates/trainwreck/transactions/view_row.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      295 2022-01-01 22:14:16.000000 Tailbone-0.9.8/tailbone/templates/trainwreck/transactions/index.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1862 2023-01-02 18:38:43.000000 Tailbone-0.9.8/tailbone/templates/trainwreck/transactions/configure.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     6614 2023-02-03 22:10:08.000000 Tailbone-0.9.8/tailbone/templates/progress.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2730 2023-01-16 18:44:24.000000 Tailbone-0.9.8/tailbone/handler.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/forms/
--rw-r--r--   0 lance     (1000) lance     (1000)     2315 2023-02-12 04:03:31.000000 Tailbone-0.9.8/tailbone/forms/receiving.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1995 2023-02-12 04:03:46.000000 Tailbone-0.9.8/tailbone/forms/common.py
--rw-r--r--   0 lance     (1000) lance     (1000)    16102 2023-02-12 03:11:23.000000 Tailbone-0.9.8/tailbone/forms/widgets.py
--rw-r--r--   0 lance     (1000) lance     (1000)    46925 2023-02-03 07:12:49.000000 Tailbone-0.9.8/tailbone/forms/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4920 2023-02-12 04:03:15.000000 Tailbone-0.9.8/tailbone/forms/types.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1099 2018-11-23 00:06:07.000000 Tailbone-0.9.8/tailbone/forms/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12442 2023-02-03 23:32:18.000000 Tailbone-0.9.8/tailbone/util.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3466 2022-08-20 22:12:54.000000 Tailbone-0.9.8/tailbone/progress.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5062 2023-02-12 04:03:57.000000 Tailbone-0.9.8/tailbone/auth.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5418 2022-12-07 20:00:13.000000 Tailbone-0.9.8/tailbone/beaker.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11188 2023-02-04 00:06:12.000000 Tailbone-0.9.8/tailbone/app.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:05.000000 Tailbone-0.9.8/tailbone/views/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:05.000000 Tailbone-0.9.8/tailbone/views/purchasing/
--rw-r--r--   0 lance     (1000) lance     (1000)    36721 2023-02-12 03:12:23.000000 Tailbone-0.9.8/tailbone/views/purchasing/batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)    89248 2023-02-12 03:13:09.000000 Tailbone-0.9.8/tailbone/views/purchasing/receiving.py
--rw-r--r--   0 lance     (1000) lance     (1000)    19691 2023-02-12 03:13:39.000000 Tailbone-0.9.8/tailbone/views/purchasing/ordering.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12753 2023-02-12 03:13:48.000000 Tailbone-0.9.8/tailbone/views/purchasing/costing.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1266 2021-09-29 15:13:18.000000 Tailbone-0.9.8/tailbone/views/purchasing/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:05.000000 Tailbone-0.9.8/tailbone/views/asgi/
--rw-r--r--   0 lance     (1000) lance     (1000)     7840 2022-08-21 03:39:57.000000 Tailbone-0.9.8/tailbone/views/asgi/upgrades.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2654 2022-08-20 22:38:06.000000 Tailbone-0.9.8/tailbone/views/asgi/datasync.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4315 2023-02-12 04:02:32.000000 Tailbone-0.9.8/tailbone/views/asgi/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    96304 2023-02-12 03:14:36.000000 Tailbone-0.9.8/tailbone/views/products.py
--rw-r--r--   0 lance     (1000) lance     (1000)    24557 2023-02-12 03:14:59.000000 Tailbone-0.9.8/tailbone/views/customers.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3197 2022-11-23 18:17:10.000000 Tailbone-0.9.8/tailbone/views/reportcodes.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1958 2022-12-10 05:04:58.000000 Tailbone-0.9.8/tailbone/views/taxes.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6801 2023-02-03 06:44:00.000000 Tailbone-0.9.8/tailbone/views/menus.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:05.000000 Tailbone-0.9.8/tailbone/views/vendors/
--rw-r--r--   0 lance     (1000) lance     (1000)     1407 2019-10-09 18:53:24.000000 Tailbone-0.9.8/tailbone/views/vendors/catalogs.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1407 2019-10-09 20:37:31.000000 Tailbone-0.9.8/tailbone/views/vendors/invoices.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7745 2022-12-21 23:46:17.000000 Tailbone-0.9.8/tailbone/views/vendors/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1237 2022-03-04 18:31:55.000000 Tailbone-0.9.8/tailbone/views/vendors/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2566 2022-11-23 18:18:26.000000 Tailbone-0.9.8/tailbone/views/inventory.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:05.000000 Tailbone-0.9.8/tailbone/views/labels/
--rw-r--r--   0 lance     (1000) lance     (1000)     1370 2019-10-09 16:08:43.000000 Tailbone-0.9.8/tailbone/views/labels/batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6330 2023-02-09 02:19:03.000000 Tailbone-0.9.8/tailbone/views/labels/profiles.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1155 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/views/labels/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:05.000000 Tailbone-0.9.8/tailbone/views/purchases/
--rw-r--r--   0 lance     (1000) lance     (1000)     6851 2023-02-12 03:15:03.000000 Tailbone-0.9.8/tailbone/views/purchases/credits.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13768 2022-11-23 18:06:10.000000 Tailbone-0.9.8/tailbone/views/purchases/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1159 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/views/purchases/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2010 2023-01-19 02:11:37.000000 Tailbone-0.9.8/tailbone/views/essentials.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12394 2023-02-12 03:15:13.000000 Tailbone-0.9.8/tailbone/views/employees.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1816 2022-11-23 18:18:05.000000 Tailbone-0.9.8/tailbone/views/permissions.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:05.000000 Tailbone-0.9.8/tailbone/views/custorders/
--rw-r--r--   0 lance     (1000) lance     (1000)     7676 2023-02-12 15:33:23.000000 Tailbone-0.9.8/tailbone/views/custorders/batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)    40125 2023-02-12 04:00:36.000000 Tailbone-0.9.8/tailbone/views/custorders/orders.py
--rw-r--r--   0 lance     (1000) lance     (1000)    20943 2023-02-12 03:15:57.000000 Tailbone-0.9.8/tailbone/views/custorders/items.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1948 2022-11-23 18:19:21.000000 Tailbone-0.9.8/tailbone/views/custorders/creating.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1213 2020-08-02 04:53:28.000000 Tailbone-0.9.8/tailbone/views/custorders/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)   210164 2023-02-14 01:54:00.000000 Tailbone-0.9.8/tailbone/views/master.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6541 2022-11-23 18:27:00.000000 Tailbone-0.9.8/tailbone/views/members.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3726 2022-11-23 18:16:15.000000 Tailbone-0.9.8/tailbone/views/stores.py
--rw-r--r--   0 lance     (1000) lance     (1000)    17512 2022-08-21 03:59:27.000000 Tailbone-0.9.8/tailbone/views/email.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11286 2023-02-03 06:49:24.000000 Tailbone-0.9.8/tailbone/views/luigi.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7542 2023-02-03 06:37:12.000000 Tailbone-0.9.8/tailbone/views/projects.py
--rw-r--r--   0 lance     (1000) lance     (1000)    29862 2023-02-12 03:17:08.000000 Tailbone-0.9.8/tailbone/views/reports.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2483 2022-11-23 18:18:45.000000 Tailbone-0.9.8/tailbone/views/filemon.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2502 2022-11-23 18:19:27.000000 Tailbone-0.9.8/tailbone/views/customergroups.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7810 2022-11-23 18:19:41.000000 Tailbone-0.9.8/tailbone/views/bouncer.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3712 2022-11-23 17:57:17.000000 Tailbone-0.9.8/tailbone/views/categories.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:05.000000 Tailbone-0.9.8/tailbone/views/shifts/
--rw-r--r--   0 lance     (1000) lance     (1000)     5387 2023-02-12 03:56:32.000000 Tailbone-0.9.8/tailbone/views/shifts/timesheet.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6825 2022-11-23 18:16:41.000000 Tailbone-0.9.8/tailbone/views/shifts/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)    21911 2023-02-12 03:57:10.000000 Tailbone-0.9.8/tailbone/views/shifts/lib.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1207 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/views/shifts/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9975 2023-02-12 03:56:46.000000 Tailbone-0.9.8/tailbone/views/shifts/schedule.py
--rw-r--r--   0 lance     (1000) lance     (1000)    24944 2023-02-03 22:10:08.000000 Tailbone-0.9.8/tailbone/views/upgrades.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2491 2022-11-23 18:17:55.000000 Tailbone-0.9.8/tailbone/views/progress.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7062 2023-01-17 02:23:29.000000 Tailbone-0.9.8/tailbone/views/views.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12308 2023-02-12 03:17:37.000000 Tailbone-0.9.8/tailbone/views/common.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9572 2023-02-07 22:11:28.000000 Tailbone-0.9.8/tailbone/views/auth.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4026 2023-02-03 06:50:35.000000 Tailbone-0.9.8/tailbone/views/features.py
--rw-r--r--   0 lance     (1000) lance     (1000)    16596 2022-08-25 01:06:23.000000 Tailbone-0.9.8/tailbone/views/datasync.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2778 2022-11-23 18:18:37.000000 Tailbone-0.9.8/tailbone/views/ifps.py
--rw-r--r--   0 lance     (1000) lance     (1000)    55250 2023-02-12 03:18:47.000000 Tailbone-0.9.8/tailbone/views/people.py
--rw-r--r--   0 lance     (1000) lance     (1000)    20040 2023-02-03 06:30:15.000000 Tailbone-0.9.8/tailbone/views/roles.py
--rw-r--r--   0 lance     (1000) lance     (1000)    23650 2023-02-12 03:55:46.000000 Tailbone-0.9.8/tailbone/views/users.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5677 2023-02-03 22:10:08.000000 Tailbone-0.9.8/tailbone/views/subdepartments.py
--rw-r--r--   0 lance     (1000) lance     (1000)    15212 2023-01-17 06:00:06.000000 Tailbone-0.9.8/tailbone/views/tables.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3974 2022-07-19 19:48:52.000000 Tailbone-0.9.8/tailbone/views/brands.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6469 2023-02-03 06:39:47.000000 Tailbone-0.9.8/tailbone/views/principal.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6101 2023-02-12 03:19:03.000000 Tailbone-0.9.8/tailbone/views/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)    21164 2023-02-03 06:50:07.000000 Tailbone-0.9.8/tailbone/views/importing.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13863 2023-02-03 06:25:44.000000 Tailbone-0.9.8/tailbone/views/workorders.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:05.000000 Tailbone-0.9.8/tailbone/views/tempmon/
--rw-r--r--   0 lance     (1000) lance     (1000)     4207 2022-11-23 18:15:17.000000 Tailbone-0.9.8/tailbone/views/tempmon/readings.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6526 2023-01-14 02:16:48.000000 Tailbone-0.9.8/tailbone/views/tempmon/appliances.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9738 2023-01-14 02:16:41.000000 Tailbone-0.9.8/tailbone/views/tempmon/clients.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3476 2023-02-03 06:28:36.000000 Tailbone-0.9.8/tailbone/views/tempmon/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12249 2023-02-03 06:27:42.000000 Tailbone-0.9.8/tailbone/views/tempmon/probes.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6056 2023-02-12 15:31:40.000000 Tailbone-0.9.8/tailbone/views/tempmon/dashboard.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1344 2020-04-04 20:42:25.000000 Tailbone-0.9.8/tailbone/views/tempmon/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1428 2022-08-16 15:24:10.000000 Tailbone-0.9.8/tailbone/views/handheld.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:05.000000 Tailbone-0.9.8/tailbone/views/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)     3698 2021-10-31 02:25:39.000000 Tailbone-0.9.8/tailbone/views/batch/delproduct.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9424 2020-01-28 23:23:15.000000 Tailbone-0.9.8/tailbone/views/batch/product.py
--rw-r--r--   0 lance     (1000) lance     (1000)    19113 2023-02-12 03:19:20.000000 Tailbone-0.9.8/tailbone/views/batch/inventory.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5646 2022-08-30 18:50:39.000000 Tailbone-0.9.8/tailbone/views/batch/newproduct.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6644 2022-08-14 04:58:46.000000 Tailbone-0.9.8/tailbone/views/batch/vendorinvoice.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7101 2022-01-10 20:54:44.000000 Tailbone-0.9.8/tailbone/views/batch/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)    10066 2023-02-12 03:19:22.000000 Tailbone-0.9.8/tailbone/views/batch/importer.py
--rw-r--r--   0 lance     (1000) lance     (1000)    59451 2023-02-12 04:02:14.000000 Tailbone-0.9.8/tailbone/views/batch/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6273 2022-08-14 04:23:06.000000 Tailbone-0.9.8/tailbone/views/batch/handheld.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1075 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/views/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12439 2022-10-19 21:22:58.000000 Tailbone-0.9.8/tailbone/views/batch/pricing.py
--rw-r--r--   0 lance     (1000) lance     (1000)    14908 2023-02-12 03:19:55.000000 Tailbone-0.9.8/tailbone/views/batch/vendorcatalog.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6163 2022-12-25 18:44:17.000000 Tailbone-0.9.8/tailbone/views/exports.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4350 2022-11-23 18:14:52.000000 Tailbone-0.9.8/tailbone/views/uoms.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7306 2023-02-03 06:52:40.000000 Tailbone-0.9.8/tailbone/views/departments.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:05.000000 Tailbone-0.9.8/tailbone/views/poser/
--rw-r--r--   0 lance     (1000) lance     (1000)     2470 2022-05-11 01:00:46.000000 Tailbone-0.9.8/tailbone/views/poser/master.py
--rw-r--r--   0 lance     (1000) lance     (1000)    10063 2022-05-11 01:00:44.000000 Tailbone-0.9.8/tailbone/views/poser/reports.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11220 2022-07-26 17:01:09.000000 Tailbone-0.9.8/tailbone/views/poser/views.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1138 2022-03-05 00:03:03.000000 Tailbone-0.9.8/tailbone/views/poser/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    16690 2023-02-12 03:19:58.000000 Tailbone-0.9.8/tailbone/views/settings.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2065 2022-11-23 18:19:03.000000 Tailbone-0.9.8/tailbone/views/depositlinks.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2797 2022-12-10 15:46:54.000000 Tailbone-0.9.8/tailbone/views/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3231 2022-11-23 18:00:03.000000 Tailbone-0.9.8/tailbone/views/families.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:05.000000 Tailbone-0.9.8/tailbone/views/trainwreck/
--rw-r--r--   0 lance     (1000) lance     (1000)     1582 2022-11-23 18:15:06.000000 Tailbone-0.9.8/tailbone/views/trainwreck/defaults.py
--rw-r--r--   0 lance     (1000) lance     (1000)    14286 2023-02-03 06:26:52.000000 Tailbone-0.9.8/tailbone/views/trainwreck/base.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1135 2023-01-19 01:57:13.000000 Tailbone-0.9.8/tailbone/views/trainwreck/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2951 2021-11-09 23:17:17.000000 Tailbone-0.9.8/tailbone/views/versions.py
--rw-r--r--   0 lance     (1000) lance     (1000)    20427 2023-02-12 03:20:00.000000 Tailbone-0.9.8/tailbone/views/messages.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1946 2023-01-12 21:03:16.000000 Tailbone-0.9.8/tailbone/helpers.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/api/
--rw-r--r--   0 lance     (1000) lance     (1000)     6539 2023-02-12 04:04:14.000000 Tailbone-0.9.8/tailbone/api/products.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1833 2022-08-14 05:48:19.000000 Tailbone-0.9.8/tailbone/api/customers.py
--rw-r--r--   0 lance     (1000) lance     (1000)    22057 2023-02-12 03:20:10.000000 Tailbone-0.9.8/tailbone/api/master.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1719 2022-08-14 05:51:19.000000 Tailbone-0.9.8/tailbone/api/vendors.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1489 2022-08-14 05:42:00.000000 Tailbone-0.9.8/tailbone/api/master2.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2126 2022-08-14 05:50:11.000000 Tailbone-0.9.8/tailbone/api/upgrades.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4276 2023-02-12 04:04:31.000000 Tailbone-0.9.8/tailbone/api/common.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7804 2022-08-14 05:44:13.000000 Tailbone-0.9.8/tailbone/api/auth.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1547 2023-01-30 00:46:27.000000 Tailbone-0.9.8/tailbone/api/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1802 2022-08-14 05:49:24.000000 Tailbone-0.9.8/tailbone/api/people.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2067 2022-08-14 05:50:38.000000 Tailbone-0.9.8/tailbone/api/users.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4689 2022-12-04 15:22:50.000000 Tailbone-0.9.8/tailbone/api/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     8607 2022-08-31 02:51:40.000000 Tailbone-0.9.8/tailbone/api/workorders.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/api/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)     6799 2022-09-08 01:45:18.000000 Tailbone-0.9.8/tailbone/api/batch/inventory.py
--rw-r--r--   0 lance     (1000) lance     (1000)    19661 2023-02-12 04:04:45.000000 Tailbone-0.9.8/tailbone/api/batch/receiving.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11689 2022-12-08 20:54:28.000000 Tailbone-0.9.8/tailbone/api/batch/ordering.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2688 2022-08-14 05:59:35.000000 Tailbone-0.9.8/tailbone/api/batch/labels.py
--rw-r--r--   0 lance     (1000) lance     (1000)    12913 2023-02-12 04:05:06.000000 Tailbone-0.9.8/tailbone/api/batch/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1097 2019-11-11 20:08:35.000000 Tailbone-0.9.8/tailbone/api/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1389 2022-08-14 05:48:55.000000 Tailbone-0.9.8/tailbone/api/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-02-21 03:50:42.000000 Tailbone-0.9.8/tailbone/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4530 2021-12-15 23:40:27.000000 Tailbone-0.9.8/tailbone/diffs.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1696 2020-02-28 23:40:40.000000 Tailbone-0.9.8/tailbone/exceptions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2637 2019-02-26 03:11:49.000000 Tailbone-0.9.8/tailbone/tweens.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1901 2023-01-15 00:47:07.000000 Tailbone-0.9.8/tailbone/providers.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1161 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3290 2022-08-17 00:32:35.000000 Tailbone-0.9.8/tailbone/asgi.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3067 2021-01-23 03:31:00.000000 Tailbone-0.9.8/tailbone/webapi.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/static/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/static/files/
--rw-r--r--   0 lance     (1000) lance     (1000)     7593 2022-01-06 18:40:01.000000 Tailbone-0.9.8/tailbone/static/files/vendor_catalog_template.xlsx
--rw-r--r--   0 lance     (1000) lance     (1000)     5041 2022-08-30 13:52:10.000000 Tailbone-0.9.8/tailbone/static/files/newproduct_template.xlsx
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/static/css/
--rw-r--r--   0 lance     (1000) lance     (1000)     4880 2021-01-17 02:38:15.000000 Tailbone-0.9.8/tailbone/static/css/codehilite.css
--rw-r--r--   0 lance     (1000) lance     (1000)     5542 2023-02-03 23:02:02.000000 Tailbone-0.9.8/tailbone/static/css/grids.css
--rw-r--r--   0 lance     (1000) lance     (1000)      208 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/static/css/purchases.css
--rw-r--r--   0 lance     (1000) lance     (1000)     1439 2023-02-02 22:24:46.000000 Tailbone-0.9.8/tailbone/static/css/forms.css
--rw-r--r--   0 lance     (1000) lance     (1000)      789 2020-08-02 03:09:36.000000 Tailbone-0.9.8/tailbone/static/css/diffs.css
--rw-r--r--   0 lance     (1000) lance     (1000)      965 2023-02-02 22:24:46.000000 Tailbone-0.9.8/tailbone/static/css/progress.css
--rw-r--r--   0 lance     (1000) lance     (1000)      575 2019-06-05 00:52:33.000000 Tailbone-0.9.8/tailbone/static/css/perms.css
--rw-r--r--   0 lance     (1000) lance     (1000)      390 2023-02-02 22:24:46.000000 Tailbone-0.9.8/tailbone/static/css/filters.css
--rw-r--r--   0 lance     (1000) lance     (1000)     2650 2023-02-02 22:24:46.000000 Tailbone-0.9.8/tailbone/static/css/layout.css
--rw-r--r--   0 lance     (1000) lance     (1000)     7346 2013-09-10 19:45:39.000000 Tailbone-0.9.8/tailbone/static/css/normalize.css
--rw-r--r--   0 lance     (1000) lance     (1000)      440 2021-01-30 19:10:34.000000 Tailbone-0.9.8/tailbone/static/css/base.css
--rw-rw-r--   0 lance     (1000) lance     (1000)     1664 2017-07-18 18:57:10.000000 Tailbone-0.9.8/tailbone/static/css/timesheet.css
--rw-r--r--   0 lance     (1000) lance     (1000)     1173 2023-02-02 22:24:46.000000 Tailbone-0.9.8/tailbone/static/css/grids.rowstatus.css
--rw-rw-r--   0 lance     (1000) lance     (1000)      225 2016-12-17 08:48:19.000000 Tailbone-0.9.8/tailbone/static/css/schedule_print.css
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/static/js/
--rw-r--r--   0 lance     (1000) lance     (1000)     1637 2019-06-24 23:30:10.000000 Tailbone-0.9.8/tailbone/static/js/tailbone.buefy.oncebutton.js
--rw-r--r--   0 lance     (1000) lance     (1000)      813 2021-10-12 18:14:50.000000 Tailbone-0.9.8/tailbone/static/js/debounce.js
--rw-r--r--   0 lance     (1000) lance     (1000)     9498 2022-12-26 21:32:08.000000 Tailbone-0.9.8/tailbone/static/js/tailbone.buefy.autocomplete.js
--rw-r--r--   0 lance     (1000) lance     (1000)     2380 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/static/js/numeric.js
--rw-r--r--   0 lance     (1000) lance     (1000)     1385 2023-02-02 22:24:46.000000 Tailbone-0.9.8/tailbone/static/js/tailbone.feedback.js
--rw-r--r--   0 lance     (1000) lance     (1000)     1514 2022-07-26 20:56:38.000000 Tailbone-0.9.8/tailbone/static/js/tailbone.buefy.numericinput.js
--rw-r--r--   0 lance     (1000) lance     (1000)     1634 2020-11-25 22:42:00.000000 Tailbone-0.9.8/tailbone/static/js/tailbone.buefy.datepicker.js
--rw-r--r--   0 lance     (1000) lance     (1000)     3407 2019-11-05 01:06:58.000000 Tailbone-0.9.8/tailbone/static/js/tailbone.buefy.message_recipients.js
--rw-r--r--   0 lance     (1000) lance     (1000)      437 2019-05-22 20:31:04.000000 Tailbone-0.9.8/tailbone/static/js/tailbone.buefy.timepicker.js
--rw-r--r--   0 lance     (1000) lance     (1000)     4178 2022-11-15 22:21:22.000000 Tailbone-0.9.8/tailbone/static/js/tailbone.buefy.grid.js
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/tailbone/static/img/
--rw-r--r--   0 lance     (1000) lance     (1000)      771 2013-09-10 19:45:39.000000 Tailbone-0.9.8/tailbone/static/img/loading.gif
--rw-r--r--   0 lance     (1000) lance     (1000)      616 2013-09-10 19:45:39.000000 Tailbone-0.9.8/tailbone/static/img/view.png
--rw-r--r--   0 lance     (1000) lance     (1000)      542 2015-03-10 02:10:41.000000 Tailbone-0.9.8/tailbone/static/img/save.png
--rw-rw-r--   0 lance     (1000) lance     (1000)     2077 2016-12-17 08:48:19.000000 Tailbone-0.9.8/tailbone/static/img/product.png
--rw-r--r--   0 lance     (1000) lance     (1000)      533 2013-09-10 19:45:39.000000 Tailbone-0.9.8/tailbone/static/img/edit.png
--rw-r--r--   0 lance     (1000) lance     (1000)      169 2013-09-10 19:45:39.000000 Tailbone-0.9.8/tailbone/static/img/sort_arrow_up.png
--rw-r--r--   0 lance     (1000) lance     (1000)   107339 2013-09-10 19:45:39.000000 Tailbone-0.9.8/tailbone/static/img/Hymenocephalus_italicus.jpg
--rw-r--r--   0 lance     (1000) lance     (1000)    20687 2013-09-10 19:45:39.000000 Tailbone-0.9.8/tailbone/static/img/home_logo.png
--rw-r--r--   0 lance     (1000) lance     (1000)      158 2013-09-10 19:45:39.000000 Tailbone-0.9.8/tailbone/static/img/sort_arrow_down.png
--rw-r--r--   0 lance     (1000) lance     (1000)     5694 2013-09-10 19:45:39.000000 Tailbone-0.9.8/tailbone/static/img/rattail.ico
--rw-rw-r--   0 lance     (1000) lance     (1000)    10375 2022-11-21 03:00:53.000000 Tailbone-0.9.8/tailbone/static/img/testing.png
--rw-r--r--   0 lance     (1000) lance     (1000)      641 2013-09-10 19:45:39.000000 Tailbone-0.9.8/tailbone/static/img/delete.png
--rw-r--r--   0 lance     (1000) lance     (1000)     1152 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/static/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       26 2018-03-01 00:58:49.000000 Tailbone-0.9.8/tailbone/static/robots.txt
--rw-r--r--   0 lance     (1000) lance     (1000)     2984 2023-02-02 00:40:54.000000 Tailbone-0.9.8/tailbone/config.py
--rw-r--r--   0 lance     (1000) lance     (1000)      489 2022-01-13 00:06:52.000000 Tailbone-0.9.8/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     6916 2023-02-11 17:51:28.000000 Tailbone-0.9.8/setup.py
--rw-r--r--   0 lance     (1000) lance     (1000)      146 2023-02-21 03:51:05.000000 Tailbone-0.9.8/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2018-03-01 00:58:49.000000 Tailbone-0.9.8/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)   145205 2023-02-21 03:50:39.000000 Tailbone-0.9.8/CHANGES.rst
--rw-r--r--   0 lance     (1000) lance     (1000)      269 2014-04-22 17:10:45.000000 Tailbone-0.9.8/README.rst
--rw-r--r--   0 lance     (1000) lance     (1000)     1511 2022-08-24 23:26:54.000000 Tailbone-0.9.8/tasks.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1147 2023-02-21 03:51:05.000000 Tailbone-0.9.8/PKG-INFO
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-21 03:51:04.000000 Tailbone-0.9.8/Tailbone.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-02-21 03:51:04.000000 Tailbone-0.9.8/Tailbone.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-02-21 03:51:04.000000 Tailbone-0.9.8/Tailbone.egg-info/not-zip-safe
--rw-r--r--   0 lance     (1000) lance     (1000)    14504 2023-02-21 03:51:04.000000 Tailbone-0.9.8/Tailbone.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      273 2023-02-21 03:51:04.000000 Tailbone-0.9.8/Tailbone.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      446 2023-02-21 03:51:04.000000 Tailbone-0.9.8/Tailbone.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        9 2023-02-21 03:51:04.000000 Tailbone-0.9.8/Tailbone.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)     1147 2023-02-21 03:51:04.000000 Tailbone-0.9.8/Tailbone.egg-info/PKG-INFO
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/
+-rw-r--r--   0 lance     (1000) lance     (1000)    10342 2023-02-12 03:10:54.000000 Tailbone-0.9.9/tailbone/subscribers.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/reports/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3577 2023-02-03 22:10:08.000000 Tailbone-0.9.9/tailbone/reports/ordering_worksheet.mako
+-rw-rw-r--   0 lance     (1000) lance     (1000)     2481 2016-12-17 08:48:19.000000 Tailbone-0.9.9/tailbone/reports/inventory_worksheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1632 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/scaffolds.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/grids/
+-rw-r--r--   0 lance     (1000) lance     (1000)    39197 2023-02-14 23:30:56.000000 Tailbone-0.9.9/tailbone/grids/filters.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    62419 2023-02-14 23:31:26.000000 Tailbone-0.9.9/tailbone/grids/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1077 2021-01-30 20:30:05.000000 Tailbone-0.9.9/tailbone/grids/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    28553 2023-02-04 01:48:39.000000 Tailbone-0.9.9/tailbone/menus.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2691 2022-12-24 05:29:45.000000 Tailbone-0.9.9/tailbone/cleanup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8274 2023-02-07 18:19:37.000000 Tailbone-0.9.9/tailbone/db.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2518 2023-02-02 22:24:46.000000 Tailbone-0.9.9/tailbone/templates/feedback_dialog_buefy.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/reports/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/reports/generated/
+-rw-r--r--   0 lance     (1000) lance     (1000)      691 2023-02-03 05:22:09.000000 Tailbone-0.9.9/tailbone/templates/reports/generated/generate.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1082 2022-11-28 23:53:29.000000 Tailbone-0.9.9/tailbone/templates/reports/generated/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      346 2021-12-15 01:04:51.000000 Tailbone-0.9.9/tailbone/templates/reports/generated/delete.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1817 2023-02-03 05:22:38.000000 Tailbone-0.9.9/tailbone/templates/reports/generated/choose.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      635 2022-01-08 19:00:03.000000 Tailbone-0.9.9/tailbone/templates/reports/generated/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/reports/problems/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2397 2022-11-19 18:52:15.000000 Tailbone-0.9.9/tailbone/templates/reports/problems/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3202 2023-02-03 22:10:08.000000 Tailbone-0.9.9/tailbone/templates/reports/ordering.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1365 2023-02-03 22:10:08.000000 Tailbone-0.9.9/tailbone/templates/reports/inventory.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/principal/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3926 2023-02-03 05:23:45.000000 Tailbone-0.9.9/tailbone/templates/principal/find_by_perm.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      369 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/principal/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/grids/
+-rw-r--r--   0 lance     (1000) lance     (1000)      755 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/grids/nav.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    21371 2023-02-10 19:06:04.000000 Tailbone-0.9.9/tailbone/templates/grids/buefy.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1584 2022-12-25 20:38:13.000000 Tailbone-0.9.9/tailbone/templates/grids/filters_buefy.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1573 2019-05-06 23:17:43.000000 Tailbone-0.9.9/tailbone/templates/grids/filters.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      910 2018-09-23 00:20:31.000000 Tailbone-0.9.9/tailbone/templates/grids/grid.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3024 2023-02-02 00:24:21.000000 Tailbone-0.9.9/tailbone/templates/grids/b-table.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      795 2019-04-15 23:05:35.000000 Tailbone-0.9.9/tailbone/templates/grids/complete.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/tables/
+-rw-r--r--   0 lance     (1000) lance     (1000)    30330 2023-02-02 00:25:12.000000 Tailbone-0.9.9/tailbone/templates/tables/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1518 2023-02-02 22:24:46.000000 Tailbone-0.9.9/tailbone/templates/feedback.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1509 2023-01-29 17:00:34.000000 Tailbone-0.9.9/tailbone/templates/multi_file_upload.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1686 2023-02-02 22:24:46.000000 Tailbone-0.9.9/tailbone/templates/menu.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/vendors/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1850 2022-05-15 21:04:06.000000 Tailbone-0.9.9/tailbone/templates/vendors/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/users/
+-rw-r--r--   0 lance     (1000) lance     (1000)      481 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/users/find_by_perm.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1314 2022-02-15 02:30:15.000000 Tailbone-0.9.9/tailbone/templates/users/preferences.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      655 2022-02-14 23:08:35.000000 Tailbone-0.9.9/tailbone/templates/users/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/labels/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/labels/profiles/
+-rw-r--r--   0 lance     (1000) lance     (1000)      432 2019-05-23 22:57:42.000000 Tailbone-0.9.9/tailbone/templates/labels/profiles/printer.mako
+-rw-rw-r--   0 lance     (1000) lance     (1000)      314 2016-12-17 08:48:19.000000 Tailbone-0.9.9/tailbone/templates/labels/profiles/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1232 2023-02-09 02:19:12.000000 Tailbone-0.9.9/tailbone/templates/labels/profiles/view.mako
+-rw-rw-r--   0 lance     (1000) lance     (1000)      620 2016-12-17 08:48:19.000000 Tailbone-0.9.9/tailbone/templates/labels/profiles/edit.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/master/
+-rw-r--r--   0 lance     (1000) lance     (1000)      879 2021-12-13 19:43:47.000000 Tailbone-0.9.9/tailbone/templates/master/edit_row.mako
+-rw-rw-r--   0 lance     (1000) lance     (1000)      248 2016-12-17 08:48:19.000000 Tailbone-0.9.9/tailbone/templates/master/create_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      174 2019-05-22 20:24:53.000000 Tailbone-0.9.9/tailbone/templates/master/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     5610 2023-02-03 05:24:29.000000 Tailbone-0.9.9/tailbone/templates/master/merge.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      584 2023-02-03 18:10:14.000000 Tailbone-0.9.9/tailbone/templates/master/form.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3266 2021-05-14 17:13:11.000000 Tailbone-0.9.9/tailbone/templates/master/view_version.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1033 2023-02-03 22:16:07.000000 Tailbone-0.9.9/tailbone/templates/master/versions.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3058 2023-02-03 18:11:06.000000 Tailbone-0.9.9/tailbone/templates/master/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      170 2018-11-23 00:24:59.000000 Tailbone-0.9.9/tailbone/templates/master/import_file.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1401 2023-02-03 05:26:22.000000 Tailbone-0.9.9/tailbone/templates/master/delete.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      709 2023-02-03 05:26:29.000000 Tailbone-0.9.9/tailbone/templates/master/view_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    23855 2023-02-03 05:29:08.000000 Tailbone-0.9.9/tailbone/templates/master/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      136 2023-02-03 18:11:06.000000 Tailbone-0.9.9/tailbone/templates/master/edit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      893 2021-12-14 03:26:58.000000 Tailbone-0.9.9/tailbone/templates/master/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1376 2023-02-03 05:30:32.000000 Tailbone-0.9.9/tailbone/templates/master/clone.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1681 2023-02-03 03:16:55.000000 Tailbone-0.9.9/tailbone/templates/page.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/purchases/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/purchases/batches/
+-rw-r--r--   0 lance     (1000) lance     (1000)      117 2023-02-03 22:16:48.000000 Tailbone-0.9.9/tailbone/templates/purchases/batches/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      278 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/purchases/batches/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/purchases/credits/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2469 2023-02-03 23:08:13.000000 Tailbone-0.9.9/tailbone/templates/purchases/credits/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      555 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/purchases/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2630 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/purchases/receiving_worksheet.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/roles/
+-rw-r--r--   0 lance     (1000) lance     (1000)      407 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/roles/find_by_perm.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      536 2020-07-17 00:43:21.000000 Tailbone-0.9.9/tailbone/templates/roles/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      867 2023-02-03 05:30:47.000000 Tailbone-0.9.9/tailbone/templates/roles/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      330 2020-06-22 20:36:16.000000 Tailbone-0.9.9/tailbone/templates/roles/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      541 2020-06-22 19:53:23.000000 Tailbone-0.9.9/tailbone/templates/roles/edit.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/custorders/
+-rw-r--r--   0 lance     (1000) lance     (1000)    88160 2023-02-03 05:31:02.000000 Tailbone-0.9.9/tailbone/templates/custorders/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     5225 2023-01-11 21:38:41.000000 Tailbone-0.9.9/tailbone/templates/custorders/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/custorders/items/
+-rw-r--r--   0 lance     (1000) lance     (1000)    14412 2023-02-02 00:28:24.000000 Tailbone-0.9.9/tailbone/templates/custorders/items/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/departments/
+-rw-rw-r--   0 lance     (1000) lance     (1000)      294 2023-02-03 05:31:15.000000 Tailbone-0.9.9/tailbone/templates/departments/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/receiving/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1495 2023-02-03 05:31:39.000000 Tailbone-0.9.9/tailbone/templates/receiving/declare_credit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      117 2023-02-03 05:32:11.000000 Tailbone-0.9.9/tailbone/templates/receiving/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1400 2023-02-03 05:32:35.000000 Tailbone-0.9.9/tailbone/templates/receiving/receive_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      305 2018-10-24 22:53:24.000000 Tailbone-0.9.9/tailbone/templates/receiving/transform_unit_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    10589 2023-02-10 19:06:04.000000 Tailbone-0.9.9/tailbone/templates/receiving/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    21656 2023-02-03 05:33:59.000000 Tailbone-0.9.9/tailbone/templates/receiving/view_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     7274 2023-01-08 17:38:39.000000 Tailbone-0.9.9/tailbone/templates/receiving/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/messages/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/messages/archive/
+-rw-r--r--   0 lance     (1000) lance     (1000)      353 2023-02-03 05:34:09.000000 Tailbone-0.9.9/tailbone/templates/messages/archive/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1364 2023-02-03 05:34:56.000000 Tailbone-0.9.9/tailbone/templates/messages/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3206 2023-02-03 05:35:31.000000 Tailbone-0.9.9/tailbone/templates/messages/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/messages/sent/
+-rw-rw-r--   0 lance     (1000) lance     (1000)      354 2016-12-17 08:48:19.000000 Tailbone-0.9.9/tailbone/templates/messages/sent/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1101 2019-11-05 01:03:51.000000 Tailbone-0.9.9/tailbone/templates/messages/recipients.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1761 2023-02-03 05:35:48.000000 Tailbone-0.9.9/tailbone/templates/messages/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/messages/inbox/
+-rw-r--r--   0 lance     (1000) lance     (1000)      355 2023-02-03 05:35:57.000000 Tailbone-0.9.9/tailbone/templates/messages/inbox/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/forms/
+-rw-r--r--   0 lance     (1000) lance     (1000)       67 2023-02-03 05:36:08.000000 Tailbone-0.9.9/tailbone/templates/forms/form.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     6607 2023-01-29 16:59:34.000000 Tailbone-0.9.9/tailbone/templates/forms/deform_buefy.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      265 2022-08-09 03:19:59.000000 Tailbone-0.9.9/tailbone/templates/forms/util.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1603 2023-02-03 05:36:20.000000 Tailbone-0.9.9/tailbone/templates/form.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/customers/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1056 2023-02-03 22:36:48.000000 Tailbone-0.9.9/tailbone/templates/customers/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/customers/pending/
+-rw-r--r--   0 lance     (1000) lance     (1000)     5021 2021-12-24 01:59:01.000000 Tailbone-0.9.9/tailbone/templates/customers/pending/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1075 2022-08-09 04:37:20.000000 Tailbone-0.9.9/tailbone/templates/customers/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/employees/
+-rw-r--r--   0 lance     (1000) lance     (1000)      259 2019-04-12 19:47:07.000000 Tailbone-0.9.9/tailbone/templates/employees/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      899 2023-02-03 22:40:11.000000 Tailbone-0.9.9/tailbone/templates/autocomplete.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1170 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/exception.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/luigi/
+-rw-r--r--   0 lance     (1000) lance     (1000)    12842 2023-02-02 00:29:33.000000 Tailbone-0.9.9/tailbone/templates/luigi/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    14033 2023-02-02 00:30:45.000000 Tailbone-0.9.9/tailbone/templates/luigi/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/appinfo/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3235 2023-02-02 00:31:07.000000 Tailbone-0.9.9/tailbone/templates/appinfo/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     7318 2023-02-02 00:31:53.000000 Tailbone-0.9.9/tailbone/templates/appinfo/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/ordering/
+-rw-r--r--   0 lance     (1000) lance     (1000)      112 2023-02-03 05:36:48.000000 Tailbone-0.9.9/tailbone/templates/ordering/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    16377 2021-02-01 03:51:46.000000 Tailbone-0.9.9/tailbone/templates/ordering/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    11560 2023-02-03 05:37:47.000000 Tailbone-0.9.9/tailbone/templates/ordering/worksheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1649 2023-02-07 22:11:44.000000 Tailbone-0.9.9/tailbone/templates/login.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/shifts/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1463 2023-02-03 22:42:48.000000 Tailbone-0.9.9/tailbone/templates/shifts/timesheet_edit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      900 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/shifts/schedule_print.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2538 2023-02-03 22:44:07.000000 Tailbone-0.9.9/tailbone/templates/shifts/schedule_edit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      813 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/shifts/schedule_print_employee.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     6116 2023-02-03 22:43:25.000000 Tailbone-0.9.9/tailbone/templates/shifts/base.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1025 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/shifts/schedule.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      833 2023-02-03 22:45:27.000000 Tailbone-0.9.9/tailbone/templates/shifts/timesheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    13008 2023-01-17 03:55:16.000000 Tailbone-0.9.9/tailbone/templates/configure-menus.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      471 2019-08-03 00:53:47.000000 Tailbone-0.9.9/tailbone/templates/about.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/upgrades/
+-rw-r--r--   0 lance     (1000) lance     (1000)     9414 2023-02-03 22:10:08.000000 Tailbone-0.9.9/tailbone/templates/upgrades/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     5196 2023-02-02 00:32:20.000000 Tailbone-0.9.9/tailbone/templates/upgrades/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/views/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/views/model/
+-rw-r--r--   0 lance     (1000) lance     (1000)     9427 2023-01-16 19:50:05.000000 Tailbone-0.9.9/tailbone/templates/views/model/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    32847 2023-02-04 00:05:40.000000 Tailbone-0.9.9/tailbone/templates/base.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      797 2023-02-03 05:38:48.000000 Tailbone-0.9.9/tailbone/templates/util.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1066 2023-02-02 22:24:46.000000 Tailbone-0.9.9/tailbone/templates/feedback_dialog.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/email-bounces/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1667 2023-02-03 23:03:42.000000 Tailbone-0.9.9/tailbone/templates/email-bounces/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/workorders/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7838 2022-08-10 02:05:11.000000 Tailbone-0.9.9/tailbone/templates/workorders/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2776 2023-01-19 03:56:10.000000 Tailbone-0.9.9/tailbone/templates/formposter.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/people/
+-rw-r--r--   0 lance     (1000) lance     (1000)    58478 2023-02-02 00:34:18.000000 Tailbone-0.9.9/tailbone/templates/people/view_profile_buefy.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1106 2023-02-03 05:39:41.000000 Tailbone-0.9.9/tailbone/templates/people/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/people/merge-requests/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1183 2023-02-03 05:39:54.000000 Tailbone-0.9.9/tailbone/templates/people/merge-requests/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3654 2023-02-03 05:40:07.000000 Tailbone-0.9.9/tailbone/templates/people/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/ifps-plu-codes/
+-rw-r--r--   0 lance     (1000) lance     (1000)      281 2020-12-07 01:28:53.000000 Tailbone-0.9.9/tailbone/templates/ifps-plu-codes/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      672 2019-08-24 02:39:03.000000 Tailbone-0.9.9/tailbone/templates/home.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/tempmon/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3718 2023-02-03 05:40:48.000000 Tailbone-0.9.9/tailbone/templates/tempmon/dashboard.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/tempmon/readings/
+-rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:17:35.000000 Tailbone-0.9.9/tailbone/templates/tempmon/readings/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/tempmon/probes/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3298 2023-02-03 05:41:19.000000 Tailbone-0.9.9/tailbone/templates/tempmon/probes/graph.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3149 2023-02-03 05:41:51.000000 Tailbone-0.9.9/tailbone/templates/tempmon/probes/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:18:44.000000 Tailbone-0.9.9/tailbone/templates/tempmon/probes/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/tempmon/appliances/
+-rw-r--r--   0 lance     (1000) lance     (1000)      510 2023-01-14 00:38:46.000000 Tailbone-0.9.9/tailbone/templates/tempmon/appliances/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      736 2020-04-05 00:31:41.000000 Tailbone-0.9.9/tailbone/templates/tempmon/appliances/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/tempmon/clients/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1044 2023-02-03 05:42:03.000000 Tailbone-0.9.9/tailbone/templates/tempmon/clients/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      305 2020-04-05 00:17:35.000000 Tailbone-0.9.9/tailbone/templates/tempmon/clients/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/batch/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/batch/vendorcatalog/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1288 2023-02-03 05:42:10.000000 Tailbone-0.9.9/tailbone/templates/batch/vendorcatalog/create.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      247 2022-01-06 20:44:32.000000 Tailbone-0.9.9/tailbone/templates/batch/vendorcatalog/view_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      309 2022-01-06 18:52:39.000000 Tailbone-0.9.9/tailbone/templates/batch/vendorcatalog/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1388 2022-01-08 19:35:47.000000 Tailbone-0.9.9/tailbone/templates/batch/vendorcatalog/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/batch/inventory/
+-rw-r--r--   0 lance     (1000) lance     (1000)     8881 2023-02-03 05:42:38.000000 Tailbone-0.9.9/tailbone/templates/batch/inventory/desktop_form.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/batch/newproduct/
+-rw-r--r--   0 lance     (1000) lance     (1000)      160 2022-08-30 15:56:25.000000 Tailbone-0.9.9/tailbone/templates/batch/newproduct/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/batch/pricing/
+-rw-r--r--   0 lance     (1000) lance     (1000)      536 2022-06-14 18:18:31.000000 Tailbone-0.9.9/tailbone/templates/batch/pricing/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       84 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/batch/create.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/batch/importer/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2387 2023-02-03 05:42:46.000000 Tailbone-0.9.9/tailbone/templates/batch/importer/view_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    11873 2023-02-03 05:50:11.000000 Tailbone-0.9.9/tailbone/templates/batch/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      509 2023-02-03 05:50:25.000000 Tailbone-0.9.9/tailbone/templates/batch/worksheet.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     4716 2023-02-03 05:51:09.000000 Tailbone-0.9.9/tailbone/templates/batch/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       81 2019-06-08 19:26:19.000000 Tailbone-0.9.9/tailbone/templates/batch/edit.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      121 2020-03-24 00:26:09.000000 Tailbone-0.9.9/tailbone/templates/change_password.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/deform/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1213 2023-02-03 05:51:23.000000 Tailbone-0.9.9/tailbone/templates/deform/checked_password.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     2164 2023-02-03 05:51:49.000000 Tailbone-0.9.9/tailbone/templates/deform/select.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      710 2023-02-03 05:52:00.000000 Tailbone-0.9.9/tailbone/templates/deform/percentinput.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      257 2023-01-29 16:59:23.000000 Tailbone-0.9.9/tailbone/templates/deform/multi_file_upload.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      918 2023-02-03 05:52:17.000000 Tailbone-0.9.9/tailbone/templates/deform/autocomplete_jquery.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1979 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/deform/select_jquery.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      509 2019-06-28 17:09:23.000000 Tailbone-0.9.9/tailbone/templates/deform/numericinput.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      758 2023-02-03 05:52:34.000000 Tailbone-0.9.9/tailbone/templates/deform/file_upload.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      545 2021-01-06 00:19:12.000000 Tailbone-0.9.9/tailbone/templates/deform/checkbox_dynamic.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      894 2023-02-04 01:42:19.000000 Tailbone-0.9.9/tailbone/templates/deform/textinput.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      943 2023-02-03 05:53:06.000000 Tailbone-0.9.9/tailbone/templates/deform/cases_units.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      616 2023-02-07 22:10:56.000000 Tailbone-0.9.9/tailbone/templates/deform/password.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      963 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/templates/deform/numberinput.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      655 2023-02-03 05:53:32.000000 Tailbone-0.9.9/tailbone/templates/deform/time_jquery.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      601 2019-11-04 23:21:16.000000 Tailbone-0.9.9/tailbone/templates/deform/message_recipients_buefy.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      597 2023-02-03 05:53:42.000000 Tailbone-0.9.9/tailbone/templates/deform/date_jquery.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      481 2023-02-03 05:53:52.000000 Tailbone-0.9.9/tailbone/templates/deform/textarea.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      581 2019-02-23 02:44:18.000000 Tailbone-0.9.9/tailbone/templates/deform/date_plain.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     2102 2023-02-03 05:54:03.000000 Tailbone-0.9.9/tailbone/templates/deform/permissions.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1160 2022-07-21 02:27:26.000000 Tailbone-0.9.9/tailbone/templates/deform/select_dynamic.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      492 2023-02-03 05:54:15.000000 Tailbone-0.9.9/tailbone/templates/deform/checkbox.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)      875 2022-11-19 23:40:01.000000 Tailbone-0.9.9/tailbone/templates/deform/problem_report_days.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1718 2019-09-06 22:13:34.000000 Tailbone-0.9.9/tailbone/templates/deform/select_plain.pt
+-rw-r--r--   0 lance     (1000) lance     (1000)     7512 2022-12-28 04:29:27.000000 Tailbone-0.9.9/tailbone/templates/page_help.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      772 2021-11-04 22:56:35.000000 Tailbone-0.9.9/tailbone/templates/base_meta.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/datasync/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/datasync/changes/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2125 2023-02-03 05:54:34.000000 Tailbone-0.9.9/tailbone/templates/datasync/changes/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     5964 2023-02-02 00:35:51.000000 Tailbone-0.9.9/tailbone/templates/datasync/status.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    31019 2023-02-02 00:43:40.000000 Tailbone-0.9.9/tailbone/templates/datasync/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/members/
+-rw-r--r--   0 lance     (1000) lance     (1000)      527 2020-03-18 18:02:17.000000 Tailbone-0.9.9/tailbone/templates/members/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      541 2019-06-15 23:03:40.000000 Tailbone-0.9.9/tailbone/templates/diff.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     6314 2023-02-03 05:54:56.000000 Tailbone-0.9.9/tailbone/templates/appsettings.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    12583 2023-02-02 00:37:54.000000 Tailbone-0.9.9/tailbone/templates/generate_feature.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     9425 2023-01-16 17:56:04.000000 Tailbone-0.9.9/tailbone/templates/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/poser/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/poser/reports/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2382 2022-03-04 00:35:18.000000 Tailbone-0.9.9/tailbone/templates/poser/reports/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3917 2022-03-21 22:32:51.000000 Tailbone-0.9.9/tailbone/templates/poser/setup.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/poser/views/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1120 2022-03-21 22:32:51.000000 Tailbone-0.9.9/tailbone/templates/poser/views/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1736 2023-02-03 22:10:08.000000 Tailbone-0.9.9/tailbone/templates/upgrade.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)      671 2021-12-07 03:21:19.000000 Tailbone-0.9.9/tailbone/templates/importing/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2643 2021-12-07 03:29:19.000000 Tailbone-0.9.9/tailbone/templates/importing/runjob.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      294 2021-12-06 18:34:10.000000 Tailbone-0.9.9/tailbone/templates/importing/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     6187 2023-02-02 00:43:01.000000 Tailbone-0.9.9/tailbone/templates/importing/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/settings/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/settings/email/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3013 2023-02-03 05:55:09.000000 Tailbone-0.9.9/tailbone/templates/settings/email/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1923 2022-08-06 23:37:28.000000 Tailbone-0.9.9/tailbone/templates/settings/email/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2579 2022-08-07 22:50:36.000000 Tailbone-0.9.9/tailbone/templates/settings/email/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    16343 2022-12-24 02:06:19.000000 Tailbone-0.9.9/tailbone/templates/generate_project.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/products/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3760 2023-02-03 06:21:59.000000 Tailbone-0.9.9/tailbone/templates/products/batch.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)    13299 2023-02-11 03:23:43.000000 Tailbone-0.9.9/tailbone/templates/products/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     8743 2023-02-02 00:39:33.000000 Tailbone-0.9.9/tailbone/templates/products/lookup.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/products/pending/
+-rw-r--r--   0 lance     (1000) lance     (1000)     4435 2021-12-24 01:58:50.000000 Tailbone-0.9.9/tailbone/templates/products/pending/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2929 2023-02-03 05:58:51.000000 Tailbone-0.9.9/tailbone/templates/products/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     4184 2023-02-10 18:21:07.000000 Tailbone-0.9.9/tailbone/templates/products/configure.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/themes/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/themes/falafel/
+-rw-r--r--   0 lance     (1000) lance     (1000)       93 2023-02-03 22:10:08.000000 Tailbone-0.9.9/tailbone/templates/themes/falafel/base.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       96 2023-02-03 22:10:08.000000 Tailbone-0.9.9/tailbone/templates/themes/falafel/upgrade.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       97 2023-02-03 22:10:08.000000 Tailbone-0.9.9/tailbone/templates/themes/falafel/progress.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/units-of-measure/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1899 2021-01-27 14:56:25.000000 Tailbone-0.9.9/tailbone/templates/units-of-measure/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/trainwreck/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/templates/trainwreck/transactions/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1625 2023-02-02 00:39:56.000000 Tailbone-0.9.9/tailbone/templates/trainwreck/transactions/rollover.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      389 2022-03-17 21:59:40.000000 Tailbone-0.9.9/tailbone/templates/trainwreck/transactions/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      357 2022-02-19 22:34:34.000000 Tailbone-0.9.9/tailbone/templates/trainwreck/transactions/view_row.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      295 2022-01-01 22:14:16.000000 Tailbone-0.9.9/tailbone/templates/trainwreck/transactions/index.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1862 2023-01-02 18:38:43.000000 Tailbone-0.9.9/tailbone/templates/trainwreck/transactions/configure.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     6614 2023-02-03 22:10:08.000000 Tailbone-0.9.9/tailbone/templates/progress.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2730 2023-01-16 18:44:24.000000 Tailbone-0.9.9/tailbone/handler.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/forms/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2315 2023-02-12 04:03:31.000000 Tailbone-0.9.9/tailbone/forms/receiving.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1995 2023-02-12 04:03:46.000000 Tailbone-0.9.9/tailbone/forms/common.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    16102 2023-02-12 03:11:23.000000 Tailbone-0.9.9/tailbone/forms/widgets.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    46925 2023-02-03 07:12:49.000000 Tailbone-0.9.9/tailbone/forms/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4920 2023-02-12 04:03:15.000000 Tailbone-0.9.9/tailbone/forms/types.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1099 2018-11-23 00:06:07.000000 Tailbone-0.9.9/tailbone/forms/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12442 2023-02-03 23:32:18.000000 Tailbone-0.9.9/tailbone/util.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3466 2022-08-20 22:12:54.000000 Tailbone-0.9.9/tailbone/progress.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5062 2023-02-12 04:03:57.000000 Tailbone-0.9.9/tailbone/auth.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5418 2022-12-07 20:00:13.000000 Tailbone-0.9.9/tailbone/beaker.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11188 2023-02-04 00:06:12.000000 Tailbone-0.9.9/tailbone/app.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/views/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/views/purchasing/
+-rw-r--r--   0 lance     (1000) lance     (1000)    36721 2023-02-12 03:12:23.000000 Tailbone-0.9.9/tailbone/views/purchasing/batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    89248 2023-02-12 03:13:09.000000 Tailbone-0.9.9/tailbone/views/purchasing/receiving.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    19691 2023-02-12 03:13:39.000000 Tailbone-0.9.9/tailbone/views/purchasing/ordering.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12753 2023-02-12 03:13:48.000000 Tailbone-0.9.9/tailbone/views/purchasing/costing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1266 2021-09-29 15:13:18.000000 Tailbone-0.9.9/tailbone/views/purchasing/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/views/asgi/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7840 2022-08-21 03:39:57.000000 Tailbone-0.9.9/tailbone/views/asgi/upgrades.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2654 2022-08-20 22:38:06.000000 Tailbone-0.9.9/tailbone/views/asgi/datasync.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4315 2023-02-12 04:02:32.000000 Tailbone-0.9.9/tailbone/views/asgi/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    96304 2023-02-12 03:14:36.000000 Tailbone-0.9.9/tailbone/views/products.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    24557 2023-02-12 03:14:59.000000 Tailbone-0.9.9/tailbone/views/customers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3197 2022-11-23 18:17:10.000000 Tailbone-0.9.9/tailbone/views/reportcodes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1958 2022-12-10 05:04:58.000000 Tailbone-0.9.9/tailbone/views/taxes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6801 2023-02-03 06:44:00.000000 Tailbone-0.9.9/tailbone/views/menus.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/views/vendors/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1407 2019-10-09 18:53:24.000000 Tailbone-0.9.9/tailbone/views/vendors/catalogs.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1407 2019-10-09 20:37:31.000000 Tailbone-0.9.9/tailbone/views/vendors/invoices.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7745 2022-12-21 23:46:17.000000 Tailbone-0.9.9/tailbone/views/vendors/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1237 2022-03-04 18:31:55.000000 Tailbone-0.9.9/tailbone/views/vendors/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2566 2022-11-23 18:18:26.000000 Tailbone-0.9.9/tailbone/views/inventory.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/views/labels/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1370 2019-10-09 16:08:43.000000 Tailbone-0.9.9/tailbone/views/labels/batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6330 2023-02-09 02:19:03.000000 Tailbone-0.9.9/tailbone/views/labels/profiles.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1155 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/views/labels/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/views/purchases/
+-rw-r--r--   0 lance     (1000) lance     (1000)     6851 2023-02-12 03:15:03.000000 Tailbone-0.9.9/tailbone/views/purchases/credits.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13768 2022-11-23 18:06:10.000000 Tailbone-0.9.9/tailbone/views/purchases/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1159 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/views/purchases/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2010 2023-01-19 02:11:37.000000 Tailbone-0.9.9/tailbone/views/essentials.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12394 2023-02-12 03:15:13.000000 Tailbone-0.9.9/tailbone/views/employees.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1816 2022-11-23 18:18:05.000000 Tailbone-0.9.9/tailbone/views/permissions.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/views/custorders/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7676 2023-02-12 15:33:23.000000 Tailbone-0.9.9/tailbone/views/custorders/batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    40125 2023-02-12 04:00:36.000000 Tailbone-0.9.9/tailbone/views/custorders/orders.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    20943 2023-02-12 03:15:57.000000 Tailbone-0.9.9/tailbone/views/custorders/items.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1948 2022-11-23 18:19:21.000000 Tailbone-0.9.9/tailbone/views/custorders/creating.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1213 2020-08-02 04:53:28.000000 Tailbone-0.9.9/tailbone/views/custorders/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)   210164 2023-02-21 17:20:01.000000 Tailbone-0.9.9/tailbone/views/master.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6541 2022-11-23 18:27:00.000000 Tailbone-0.9.9/tailbone/views/members.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3726 2022-11-23 18:16:15.000000 Tailbone-0.9.9/tailbone/views/stores.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    17512 2022-08-21 03:59:27.000000 Tailbone-0.9.9/tailbone/views/email.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11286 2023-02-03 06:49:24.000000 Tailbone-0.9.9/tailbone/views/luigi.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7542 2023-02-03 06:37:12.000000 Tailbone-0.9.9/tailbone/views/projects.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    29862 2023-02-12 03:17:08.000000 Tailbone-0.9.9/tailbone/views/reports.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2483 2022-11-23 18:18:45.000000 Tailbone-0.9.9/tailbone/views/filemon.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2502 2022-11-23 18:19:27.000000 Tailbone-0.9.9/tailbone/views/customergroups.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7810 2022-11-23 18:19:41.000000 Tailbone-0.9.9/tailbone/views/bouncer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3712 2022-11-23 17:57:17.000000 Tailbone-0.9.9/tailbone/views/categories.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/views/shifts/
+-rw-r--r--   0 lance     (1000) lance     (1000)     5387 2023-02-12 03:56:32.000000 Tailbone-0.9.9/tailbone/views/shifts/timesheet.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6825 2022-11-23 18:16:41.000000 Tailbone-0.9.9/tailbone/views/shifts/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    21911 2023-02-12 03:57:10.000000 Tailbone-0.9.9/tailbone/views/shifts/lib.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1207 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/views/shifts/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9975 2023-02-12 03:56:46.000000 Tailbone-0.9.9/tailbone/views/shifts/schedule.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    24944 2023-02-03 22:10:08.000000 Tailbone-0.9.9/tailbone/views/upgrades.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2491 2022-11-23 18:17:55.000000 Tailbone-0.9.9/tailbone/views/progress.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7062 2023-01-17 02:23:29.000000 Tailbone-0.9.9/tailbone/views/views.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12308 2023-02-12 03:17:37.000000 Tailbone-0.9.9/tailbone/views/common.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9572 2023-02-07 22:11:28.000000 Tailbone-0.9.9/tailbone/views/auth.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4026 2023-02-03 06:50:35.000000 Tailbone-0.9.9/tailbone/views/features.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    16596 2022-08-25 01:06:23.000000 Tailbone-0.9.9/tailbone/views/datasync.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2778 2022-11-23 18:18:37.000000 Tailbone-0.9.9/tailbone/views/ifps.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    55250 2023-02-12 03:18:47.000000 Tailbone-0.9.9/tailbone/views/people.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    20040 2023-02-03 06:30:15.000000 Tailbone-0.9.9/tailbone/views/roles.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    23650 2023-02-12 03:55:46.000000 Tailbone-0.9.9/tailbone/views/users.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5677 2023-02-03 22:10:08.000000 Tailbone-0.9.9/tailbone/views/subdepartments.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    15212 2023-01-17 06:00:06.000000 Tailbone-0.9.9/tailbone/views/tables.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3974 2022-07-19 19:48:52.000000 Tailbone-0.9.9/tailbone/views/brands.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6469 2023-02-03 06:39:47.000000 Tailbone-0.9.9/tailbone/views/principal.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6101 2023-02-12 03:19:03.000000 Tailbone-0.9.9/tailbone/views/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    21164 2023-02-03 06:50:07.000000 Tailbone-0.9.9/tailbone/views/importing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    13863 2023-02-03 06:25:44.000000 Tailbone-0.9.9/tailbone/views/workorders.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/views/tempmon/
+-rw-r--r--   0 lance     (1000) lance     (1000)     4207 2022-11-23 18:15:17.000000 Tailbone-0.9.9/tailbone/views/tempmon/readings.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6526 2023-01-14 02:16:48.000000 Tailbone-0.9.9/tailbone/views/tempmon/appliances.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9738 2023-01-14 02:16:41.000000 Tailbone-0.9.9/tailbone/views/tempmon/clients.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3476 2023-02-03 06:28:36.000000 Tailbone-0.9.9/tailbone/views/tempmon/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12249 2023-02-03 06:27:42.000000 Tailbone-0.9.9/tailbone/views/tempmon/probes.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6056 2023-02-12 15:31:40.000000 Tailbone-0.9.9/tailbone/views/tempmon/dashboard.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1344 2020-04-04 20:42:25.000000 Tailbone-0.9.9/tailbone/views/tempmon/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1428 2022-08-16 15:24:10.000000 Tailbone-0.9.9/tailbone/views/handheld.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/views/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3698 2021-10-31 02:25:39.000000 Tailbone-0.9.9/tailbone/views/batch/delproduct.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9424 2020-01-28 23:23:15.000000 Tailbone-0.9.9/tailbone/views/batch/product.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    19113 2023-02-12 03:19:20.000000 Tailbone-0.9.9/tailbone/views/batch/inventory.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5646 2022-08-30 18:50:39.000000 Tailbone-0.9.9/tailbone/views/batch/newproduct.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6644 2022-08-14 04:58:46.000000 Tailbone-0.9.9/tailbone/views/batch/vendorinvoice.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7101 2022-01-10 20:54:44.000000 Tailbone-0.9.9/tailbone/views/batch/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    10066 2023-02-12 03:19:22.000000 Tailbone-0.9.9/tailbone/views/batch/importer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    59451 2023-02-12 04:02:14.000000 Tailbone-0.9.9/tailbone/views/batch/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6273 2022-08-14 04:23:06.000000 Tailbone-0.9.9/tailbone/views/batch/handheld.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1075 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/views/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12439 2022-10-19 21:22:58.000000 Tailbone-0.9.9/tailbone/views/batch/pricing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    15260 2023-02-21 23:34:49.000000 Tailbone-0.9.9/tailbone/views/batch/vendorcatalog.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6163 2022-12-25 18:44:17.000000 Tailbone-0.9.9/tailbone/views/exports.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4350 2022-11-23 18:14:52.000000 Tailbone-0.9.9/tailbone/views/uoms.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7306 2023-02-03 06:52:40.000000 Tailbone-0.9.9/tailbone/views/departments.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/views/poser/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2470 2022-05-11 01:00:46.000000 Tailbone-0.9.9/tailbone/views/poser/master.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    10063 2022-05-11 01:00:44.000000 Tailbone-0.9.9/tailbone/views/poser/reports.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11220 2022-07-26 17:01:09.000000 Tailbone-0.9.9/tailbone/views/poser/views.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1138 2022-03-05 00:03:03.000000 Tailbone-0.9.9/tailbone/views/poser/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    16690 2023-02-12 03:19:58.000000 Tailbone-0.9.9/tailbone/views/settings.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2065 2022-11-23 18:19:03.000000 Tailbone-0.9.9/tailbone/views/depositlinks.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2797 2022-12-10 15:46:54.000000 Tailbone-0.9.9/tailbone/views/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3231 2022-11-23 18:00:03.000000 Tailbone-0.9.9/tailbone/views/families.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/views/trainwreck/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1582 2022-11-23 18:15:06.000000 Tailbone-0.9.9/tailbone/views/trainwreck/defaults.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    14286 2023-02-03 06:26:52.000000 Tailbone-0.9.9/tailbone/views/trainwreck/base.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1135 2023-01-19 01:57:13.000000 Tailbone-0.9.9/tailbone/views/trainwreck/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2951 2021-11-09 23:17:17.000000 Tailbone-0.9.9/tailbone/views/versions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    20427 2023-02-12 03:20:00.000000 Tailbone-0.9.9/tailbone/views/messages.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1946 2023-01-12 21:03:16.000000 Tailbone-0.9.9/tailbone/helpers.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/api/
+-rw-r--r--   0 lance     (1000) lance     (1000)     6539 2023-02-12 04:04:14.000000 Tailbone-0.9.9/tailbone/api/products.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1833 2022-08-14 05:48:19.000000 Tailbone-0.9.9/tailbone/api/customers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    22057 2023-02-12 03:20:10.000000 Tailbone-0.9.9/tailbone/api/master.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1719 2022-08-14 05:51:19.000000 Tailbone-0.9.9/tailbone/api/vendors.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1489 2022-08-14 05:42:00.000000 Tailbone-0.9.9/tailbone/api/master2.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2126 2022-08-14 05:50:11.000000 Tailbone-0.9.9/tailbone/api/upgrades.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4276 2023-02-12 04:04:31.000000 Tailbone-0.9.9/tailbone/api/common.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7804 2022-08-14 05:44:13.000000 Tailbone-0.9.9/tailbone/api/auth.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1547 2023-01-30 00:46:27.000000 Tailbone-0.9.9/tailbone/api/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1802 2022-08-14 05:49:24.000000 Tailbone-0.9.9/tailbone/api/people.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2067 2022-08-14 05:50:38.000000 Tailbone-0.9.9/tailbone/api/users.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4689 2022-12-04 15:22:50.000000 Tailbone-0.9.9/tailbone/api/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     8607 2022-08-31 02:51:40.000000 Tailbone-0.9.9/tailbone/api/workorders.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/api/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)     6799 2022-09-08 01:45:18.000000 Tailbone-0.9.9/tailbone/api/batch/inventory.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    19661 2023-02-12 04:04:45.000000 Tailbone-0.9.9/tailbone/api/batch/receiving.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11689 2022-12-08 20:54:28.000000 Tailbone-0.9.9/tailbone/api/batch/ordering.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2688 2022-08-14 05:59:35.000000 Tailbone-0.9.9/tailbone/api/batch/labels.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    12913 2023-02-12 04:05:06.000000 Tailbone-0.9.9/tailbone/api/batch/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1097 2019-11-11 20:08:35.000000 Tailbone-0.9.9/tailbone/api/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1389 2022-08-14 05:48:55.000000 Tailbone-0.9.9/tailbone/api/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-02-22 01:14:17.000000 Tailbone-0.9.9/tailbone/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4530 2021-12-15 23:40:27.000000 Tailbone-0.9.9/tailbone/diffs.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1696 2020-02-28 23:40:40.000000 Tailbone-0.9.9/tailbone/exceptions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2637 2019-02-26 03:11:49.000000 Tailbone-0.9.9/tailbone/tweens.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1901 2023-01-15 00:47:07.000000 Tailbone-0.9.9/tailbone/providers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1161 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3290 2022-08-17 00:32:35.000000 Tailbone-0.9.9/tailbone/asgi.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3067 2021-01-23 03:31:00.000000 Tailbone-0.9.9/tailbone/webapi.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/static/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/static/files/
+-rw-r--r--   0 lance     (1000) lance     (1000)     7593 2022-01-06 18:40:01.000000 Tailbone-0.9.9/tailbone/static/files/vendor_catalog_template.xlsx
+-rw-r--r--   0 lance     (1000) lance     (1000)     5041 2022-08-30 13:52:10.000000 Tailbone-0.9.9/tailbone/static/files/newproduct_template.xlsx
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/static/css/
+-rw-r--r--   0 lance     (1000) lance     (1000)     4880 2021-01-17 02:38:15.000000 Tailbone-0.9.9/tailbone/static/css/codehilite.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     5542 2023-02-03 23:02:02.000000 Tailbone-0.9.9/tailbone/static/css/grids.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      208 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/static/css/purchases.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     1439 2023-02-02 22:24:46.000000 Tailbone-0.9.9/tailbone/static/css/forms.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      789 2020-08-02 03:09:36.000000 Tailbone-0.9.9/tailbone/static/css/diffs.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      965 2023-02-02 22:24:46.000000 Tailbone-0.9.9/tailbone/static/css/progress.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      575 2019-06-05 00:52:33.000000 Tailbone-0.9.9/tailbone/static/css/perms.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      390 2023-02-02 22:24:46.000000 Tailbone-0.9.9/tailbone/static/css/filters.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     2650 2023-02-02 22:24:46.000000 Tailbone-0.9.9/tailbone/static/css/layout.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     7346 2013-09-10 19:45:39.000000 Tailbone-0.9.9/tailbone/static/css/normalize.css
+-rw-r--r--   0 lance     (1000) lance     (1000)      440 2021-01-30 19:10:34.000000 Tailbone-0.9.9/tailbone/static/css/base.css
+-rw-rw-r--   0 lance     (1000) lance     (1000)     1664 2017-07-18 18:57:10.000000 Tailbone-0.9.9/tailbone/static/css/timesheet.css
+-rw-r--r--   0 lance     (1000) lance     (1000)     1173 2023-02-02 22:24:46.000000 Tailbone-0.9.9/tailbone/static/css/grids.rowstatus.css
+-rw-rw-r--   0 lance     (1000) lance     (1000)      225 2016-12-17 08:48:19.000000 Tailbone-0.9.9/tailbone/static/css/schedule_print.css
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/static/js/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1637 2019-06-24 23:30:10.000000 Tailbone-0.9.9/tailbone/static/js/tailbone.buefy.oncebutton.js
+-rw-r--r--   0 lance     (1000) lance     (1000)      813 2021-10-12 18:14:50.000000 Tailbone-0.9.9/tailbone/static/js/debounce.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     9498 2022-12-26 21:32:08.000000 Tailbone-0.9.9/tailbone/static/js/tailbone.buefy.autocomplete.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     2380 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/static/js/numeric.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     1385 2023-02-02 22:24:46.000000 Tailbone-0.9.9/tailbone/static/js/tailbone.feedback.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     1514 2022-07-26 20:56:38.000000 Tailbone-0.9.9/tailbone/static/js/tailbone.buefy.numericinput.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     1634 2020-11-25 22:42:00.000000 Tailbone-0.9.9/tailbone/static/js/tailbone.buefy.datepicker.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     3407 2019-11-05 01:06:58.000000 Tailbone-0.9.9/tailbone/static/js/tailbone.buefy.message_recipients.js
+-rw-r--r--   0 lance     (1000) lance     (1000)      437 2019-05-22 20:31:04.000000 Tailbone-0.9.9/tailbone/static/js/tailbone.buefy.timepicker.js
+-rw-r--r--   0 lance     (1000) lance     (1000)     4178 2022-11-15 22:21:22.000000 Tailbone-0.9.9/tailbone/static/js/tailbone.buefy.grid.js
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/tailbone/static/img/
+-rw-r--r--   0 lance     (1000) lance     (1000)      771 2013-09-10 19:45:39.000000 Tailbone-0.9.9/tailbone/static/img/loading.gif
+-rw-r--r--   0 lance     (1000) lance     (1000)      616 2013-09-10 19:45:39.000000 Tailbone-0.9.9/tailbone/static/img/view.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      542 2015-03-10 02:10:41.000000 Tailbone-0.9.9/tailbone/static/img/save.png
+-rw-rw-r--   0 lance     (1000) lance     (1000)     2077 2016-12-17 08:48:19.000000 Tailbone-0.9.9/tailbone/static/img/product.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      533 2013-09-10 19:45:39.000000 Tailbone-0.9.9/tailbone/static/img/edit.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      169 2013-09-10 19:45:39.000000 Tailbone-0.9.9/tailbone/static/img/sort_arrow_up.png
+-rw-r--r--   0 lance     (1000) lance     (1000)   107339 2013-09-10 19:45:39.000000 Tailbone-0.9.9/tailbone/static/img/Hymenocephalus_italicus.jpg
+-rw-r--r--   0 lance     (1000) lance     (1000)    20687 2013-09-10 19:45:39.000000 Tailbone-0.9.9/tailbone/static/img/home_logo.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      158 2013-09-10 19:45:39.000000 Tailbone-0.9.9/tailbone/static/img/sort_arrow_down.png
+-rw-r--r--   0 lance     (1000) lance     (1000)     5694 2013-09-10 19:45:39.000000 Tailbone-0.9.9/tailbone/static/img/rattail.ico
+-rw-rw-r--   0 lance     (1000) lance     (1000)    10375 2022-11-21 03:00:53.000000 Tailbone-0.9.9/tailbone/static/img/testing.png
+-rw-r--r--   0 lance     (1000) lance     (1000)      641 2013-09-10 19:45:39.000000 Tailbone-0.9.9/tailbone/static/img/delete.png
+-rw-r--r--   0 lance     (1000) lance     (1000)     1152 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/static/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       26 2018-03-01 00:58:49.000000 Tailbone-0.9.9/tailbone/static/robots.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     2984 2023-02-02 00:40:54.000000 Tailbone-0.9.9/tailbone/config.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      489 2022-01-13 00:06:52.000000 Tailbone-0.9.9/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     6916 2023-02-11 17:51:28.000000 Tailbone-0.9.9/setup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      146 2023-02-22 01:14:55.000000 Tailbone-0.9.9/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2018-03-01 00:58:49.000000 Tailbone-0.9.9/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)   145290 2023-02-22 01:14:13.000000 Tailbone-0.9.9/CHANGES.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)      269 2014-04-22 17:10:45.000000 Tailbone-0.9.9/README.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)     1511 2022-08-24 23:26:54.000000 Tailbone-0.9.9/tasks.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1147 2023-02-22 01:14:55.000000 Tailbone-0.9.9/PKG-INFO
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:14:55.000000 Tailbone-0.9.9/Tailbone.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-02-22 01:14:54.000000 Tailbone-0.9.9/Tailbone.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-02-22 01:14:54.000000 Tailbone-0.9.9/Tailbone.egg-info/not-zip-safe
+-rw-r--r--   0 lance     (1000) lance     (1000)    14504 2023-02-22 01:14:55.000000 Tailbone-0.9.9/Tailbone.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      273 2023-02-22 01:14:54.000000 Tailbone-0.9.9/Tailbone.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      446 2023-02-22 01:14:54.000000 Tailbone-0.9.9/Tailbone.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        9 2023-02-22 01:14:54.000000 Tailbone-0.9.9/Tailbone.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1147 2023-02-22 01:14:54.000000 Tailbone-0.9.9/Tailbone.egg-info/PKG-INFO
```

### Comparing `Tailbone-0.9.8/tailbone/subscribers.py` & `Tailbone-0.9.9/tailbone/subscribers.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/reports/ordering_worksheet.mako` & `Tailbone-0.9.9/tailbone/reports/ordering_worksheet.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/reports/inventory_worksheet.mako` & `Tailbone-0.9.9/tailbone/reports/inventory_worksheet.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/scaffolds.py` & `Tailbone-0.9.9/tailbone/scaffolds.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/grids/filters.py` & `Tailbone-0.9.9/tailbone/grids/filters.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/grids/core.py` & `Tailbone-0.9.9/tailbone/grids/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/grids/__init__.py` & `Tailbone-0.9.9/tailbone/grids/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/menus.py` & `Tailbone-0.9.9/tailbone/menus.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/cleanup.py` & `Tailbone-0.9.9/tailbone/cleanup.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/db.py` & `Tailbone-0.9.9/tailbone/db.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/feedback_dialog_buefy.mako` & `Tailbone-0.9.9/tailbone/templates/feedback_dialog_buefy.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/reports/generated/generate.mako` & `Tailbone-0.9.9/tailbone/templates/reports/generated/generate.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/reports/generated/view.mako` & `Tailbone-0.9.9/tailbone/templates/reports/generated/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/reports/generated/choose.mako` & `Tailbone-0.9.9/tailbone/templates/reports/generated/choose.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/reports/generated/configure.mako` & `Tailbone-0.9.9/tailbone/templates/reports/generated/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/reports/problems/view.mako` & `Tailbone-0.9.9/tailbone/templates/reports/problems/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/reports/ordering.mako` & `Tailbone-0.9.9/tailbone/templates/reports/ordering.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/reports/inventory.mako` & `Tailbone-0.9.9/tailbone/templates/reports/inventory.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/principal/find_by_perm.mako` & `Tailbone-0.9.9/tailbone/templates/principal/find_by_perm.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/grids/nav.mako` & `Tailbone-0.9.9/tailbone/templates/grids/nav.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/grids/buefy.mako` & `Tailbone-0.9.9/tailbone/templates/grids/buefy.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/grids/filters_buefy.mako` & `Tailbone-0.9.9/tailbone/templates/grids/filters_buefy.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/grids/filters.mako` & `Tailbone-0.9.9/tailbone/templates/grids/filters.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/grids/grid.mako` & `Tailbone-0.9.9/tailbone/templates/grids/grid.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/grids/b-table.mako` & `Tailbone-0.9.9/tailbone/templates/grids/b-table.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/grids/complete.mako` & `Tailbone-0.9.9/tailbone/templates/grids/complete.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/tables/create.mako` & `Tailbone-0.9.9/tailbone/templates/tables/create.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/feedback.mako` & `Tailbone-0.9.9/tailbone/templates/feedback.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/multi_file_upload.mako` & `Tailbone-0.9.9/tailbone/templates/multi_file_upload.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/menu.mako` & `Tailbone-0.9.9/tailbone/templates/menu.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/vendors/configure.mako` & `Tailbone-0.9.9/tailbone/templates/vendors/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/users/preferences.mako` & `Tailbone-0.9.9/tailbone/templates/users/preferences.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/users/view.mako` & `Tailbone-0.9.9/tailbone/templates/users/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/labels/profiles/view.mako` & `Tailbone-0.9.9/tailbone/templates/labels/profiles/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/labels/profiles/edit.mako` & `Tailbone-0.9.9/tailbone/templates/labels/profiles/edit.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/master/edit_row.mako` & `Tailbone-0.9.9/tailbone/templates/master/edit_row.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/master/merge.mako` & `Tailbone-0.9.9/tailbone/templates/master/merge.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/master/form.mako` & `Tailbone-0.9.9/tailbone/templates/master/form.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/master/view_version.mako` & `Tailbone-0.9.9/tailbone/templates/master/view_version.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/master/versions.mako` & `Tailbone-0.9.9/tailbone/templates/master/versions.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/master/view.mako` & `Tailbone-0.9.9/tailbone/templates/master/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/master/delete.mako` & `Tailbone-0.9.9/tailbone/templates/master/delete.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/master/view_row.mako` & `Tailbone-0.9.9/tailbone/templates/master/view_row.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/master/index.mako` & `Tailbone-0.9.9/tailbone/templates/master/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/master/configure.mako` & `Tailbone-0.9.9/tailbone/templates/master/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/master/clone.mako` & `Tailbone-0.9.9/tailbone/templates/master/clone.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/page.mako` & `Tailbone-0.9.9/tailbone/templates/page.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/purchases/credits/index.mako` & `Tailbone-0.9.9/tailbone/templates/purchases/credits/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/purchases/view.mako` & `Tailbone-0.9.9/tailbone/templates/purchases/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/purchases/receiving_worksheet.mako` & `Tailbone-0.9.9/tailbone/templates/purchases/receiving_worksheet.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/roles/create.mako` & `Tailbone-0.9.9/tailbone/templates/roles/create.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/roles/view.mako` & `Tailbone-0.9.9/tailbone/templates/roles/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/roles/edit.mako` & `Tailbone-0.9.9/tailbone/templates/roles/edit.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/custorders/create.mako` & `Tailbone-0.9.9/tailbone/templates/custorders/create.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/custorders/configure.mako` & `Tailbone-0.9.9/tailbone/templates/custorders/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/custorders/items/view.mako` & `Tailbone-0.9.9/tailbone/templates/custorders/items/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/receiving/declare_credit.mako` & `Tailbone-0.9.9/tailbone/templates/receiving/declare_credit.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/receiving/receive_row.mako` & `Tailbone-0.9.9/tailbone/templates/receiving/receive_row.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/receiving/view.mako` & `Tailbone-0.9.9/tailbone/templates/receiving/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/receiving/view_row.mako` & `Tailbone-0.9.9/tailbone/templates/receiving/view_row.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/receiving/configure.mako` & `Tailbone-0.9.9/tailbone/templates/receiving/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/messages/create.mako` & `Tailbone-0.9.9/tailbone/templates/messages/create.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/messages/view.mako` & `Tailbone-0.9.9/tailbone/templates/messages/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/messages/recipients.mako` & `Tailbone-0.9.9/tailbone/templates/messages/recipients.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/messages/index.mako` & `Tailbone-0.9.9/tailbone/templates/messages/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/forms/deform_buefy.mako` & `Tailbone-0.9.9/tailbone/templates/forms/deform_buefy.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/form.mako` & `Tailbone-0.9.9/tailbone/templates/form.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/customers/view.mako` & `Tailbone-0.9.9/tailbone/templates/customers/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/customers/pending/view.mako` & `Tailbone-0.9.9/tailbone/templates/customers/pending/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/customers/configure.mako` & `Tailbone-0.9.9/tailbone/templates/customers/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/autocomplete.mako` & `Tailbone-0.9.9/tailbone/templates/autocomplete.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/exception.mako` & `Tailbone-0.9.9/tailbone/templates/exception.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/luigi/index.mako` & `Tailbone-0.9.9/tailbone/templates/luigi/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/luigi/configure.mako` & `Tailbone-0.9.9/tailbone/templates/luigi/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/appinfo/index.mako` & `Tailbone-0.9.9/tailbone/templates/appinfo/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/appinfo/configure.mako` & `Tailbone-0.9.9/tailbone/templates/appinfo/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/ordering/view.mako` & `Tailbone-0.9.9/tailbone/templates/ordering/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/ordering/worksheet.mako` & `Tailbone-0.9.9/tailbone/templates/ordering/worksheet.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/login.mako` & `Tailbone-0.9.9/tailbone/templates/login.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/shifts/timesheet_edit.mako` & `Tailbone-0.9.9/tailbone/templates/shifts/timesheet_edit.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/shifts/schedule_print.mako` & `Tailbone-0.9.9/tailbone/templates/shifts/schedule_print.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/shifts/schedule_edit.mako` & `Tailbone-0.9.9/tailbone/templates/shifts/schedule_edit.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/shifts/schedule_print_employee.mako` & `Tailbone-0.9.9/tailbone/templates/shifts/schedule_print_employee.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/shifts/base.mako` & `Tailbone-0.9.9/tailbone/templates/shifts/base.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/shifts/schedule.mako` & `Tailbone-0.9.9/tailbone/templates/shifts/schedule.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/shifts/timesheet.mako` & `Tailbone-0.9.9/tailbone/templates/shifts/timesheet.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/configure-menus.mako` & `Tailbone-0.9.9/tailbone/templates/configure-menus.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/upgrades/view.mako` & `Tailbone-0.9.9/tailbone/templates/upgrades/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/upgrades/configure.mako` & `Tailbone-0.9.9/tailbone/templates/upgrades/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/views/model/create.mako` & `Tailbone-0.9.9/tailbone/templates/views/model/create.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/base.mako` & `Tailbone-0.9.9/tailbone/templates/base.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/util.mako` & `Tailbone-0.9.9/tailbone/templates/util.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/feedback_dialog.mako` & `Tailbone-0.9.9/tailbone/templates/feedback_dialog.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/email-bounces/view.mako` & `Tailbone-0.9.9/tailbone/templates/email-bounces/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/workorders/view.mako` & `Tailbone-0.9.9/tailbone/templates/workorders/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/formposter.mako` & `Tailbone-0.9.9/tailbone/templates/formposter.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/people/view_profile_buefy.mako` & `Tailbone-0.9.9/tailbone/templates/people/view_profile_buefy.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/people/view.mako` & `Tailbone-0.9.9/tailbone/templates/people/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/people/merge-requests/view.mako` & `Tailbone-0.9.9/tailbone/templates/people/merge-requests/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/people/index.mako` & `Tailbone-0.9.9/tailbone/templates/people/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/home.mako` & `Tailbone-0.9.9/tailbone/templates/home.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/tempmon/dashboard.mako` & `Tailbone-0.9.9/tailbone/templates/tempmon/dashboard.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/tempmon/probes/graph.mako` & `Tailbone-0.9.9/tailbone/templates/tempmon/probes/graph.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/tempmon/probes/view.mako` & `Tailbone-0.9.9/tailbone/templates/tempmon/probes/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/tempmon/appliances/index.mako` & `Tailbone-0.9.9/tailbone/templates/tempmon/appliances/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/tempmon/clients/view.mako` & `Tailbone-0.9.9/tailbone/templates/tempmon/clients/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/batch/vendorcatalog/create.mako` & `Tailbone-0.9.9/tailbone/templates/batch/vendorcatalog/create.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/batch/vendorcatalog/configure.mako` & `Tailbone-0.9.9/tailbone/templates/batch/vendorcatalog/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/batch/inventory/desktop_form.mako` & `Tailbone-0.9.9/tailbone/templates/batch/inventory/desktop_form.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/batch/pricing/configure.mako` & `Tailbone-0.9.9/tailbone/templates/batch/pricing/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/batch/importer/view_row.mako` & `Tailbone-0.9.9/tailbone/templates/batch/importer/view_row.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/batch/view.mako` & `Tailbone-0.9.9/tailbone/templates/batch/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/batch/index.mako` & `Tailbone-0.9.9/tailbone/templates/batch/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/checked_password.pt` & `Tailbone-0.9.9/tailbone/templates/deform/checked_password.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/select.pt` & `Tailbone-0.9.9/tailbone/templates/deform/select.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/percentinput.pt` & `Tailbone-0.9.9/tailbone/templates/deform/percentinput.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/autocomplete_jquery.pt` & `Tailbone-0.9.9/tailbone/templates/deform/autocomplete_jquery.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/select_jquery.pt` & `Tailbone-0.9.9/tailbone/templates/deform/select_jquery.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/file_upload.pt` & `Tailbone-0.9.9/tailbone/templates/deform/file_upload.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/checkbox_dynamic.pt` & `Tailbone-0.9.9/tailbone/templates/deform/checkbox_dynamic.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/textinput.pt` & `Tailbone-0.9.9/tailbone/templates/deform/textinput.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/cases_units.pt` & `Tailbone-0.9.9/tailbone/templates/deform/cases_units.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/password.pt` & `Tailbone-0.9.9/tailbone/templates/deform/password.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/numberinput.pt` & `Tailbone-0.9.9/tailbone/templates/deform/numberinput.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/time_jquery.pt` & `Tailbone-0.9.9/tailbone/templates/deform/time_jquery.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/message_recipients_buefy.pt` & `Tailbone-0.9.9/tailbone/templates/deform/message_recipients_buefy.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/date_jquery.pt` & `Tailbone-0.9.9/tailbone/templates/deform/date_jquery.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/date_plain.pt` & `Tailbone-0.9.9/tailbone/templates/deform/date_plain.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/permissions.pt` & `Tailbone-0.9.9/tailbone/templates/deform/permissions.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/select_dynamic.pt` & `Tailbone-0.9.9/tailbone/templates/deform/select_dynamic.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/problem_report_days.pt` & `Tailbone-0.9.9/tailbone/templates/deform/problem_report_days.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/deform/select_plain.pt` & `Tailbone-0.9.9/tailbone/templates/deform/select_plain.pt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/page_help.mako` & `Tailbone-0.9.9/tailbone/templates/page_help.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/base_meta.mako` & `Tailbone-0.9.9/tailbone/templates/base_meta.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/datasync/changes/index.mako` & `Tailbone-0.9.9/tailbone/templates/datasync/changes/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/datasync/status.mako` & `Tailbone-0.9.9/tailbone/templates/datasync/status.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/datasync/configure.mako` & `Tailbone-0.9.9/tailbone/templates/datasync/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/members/view.mako` & `Tailbone-0.9.9/tailbone/templates/members/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/diff.mako` & `Tailbone-0.9.9/tailbone/templates/diff.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/appsettings.mako` & `Tailbone-0.9.9/tailbone/templates/appsettings.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/generate_feature.mako` & `Tailbone-0.9.9/tailbone/templates/generate_feature.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/configure.mako` & `Tailbone-0.9.9/tailbone/templates/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/poser/reports/view.mako` & `Tailbone-0.9.9/tailbone/templates/poser/reports/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/poser/setup.mako` & `Tailbone-0.9.9/tailbone/templates/poser/setup.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/poser/views/configure.mako` & `Tailbone-0.9.9/tailbone/templates/poser/views/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/upgrade.mako` & `Tailbone-0.9.9/tailbone/templates/upgrade.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/importing/view.mako` & `Tailbone-0.9.9/tailbone/templates/importing/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/importing/runjob.mako` & `Tailbone-0.9.9/tailbone/templates/importing/runjob.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/importing/configure.mako` & `Tailbone-0.9.9/tailbone/templates/importing/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/settings/email/view.mako` & `Tailbone-0.9.9/tailbone/templates/settings/email/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/settings/email/index.mako` & `Tailbone-0.9.9/tailbone/templates/settings/email/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/settings/email/configure.mako` & `Tailbone-0.9.9/tailbone/templates/settings/email/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/generate_project.mako` & `Tailbone-0.9.9/tailbone/templates/generate_project.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/products/batch.mako` & `Tailbone-0.9.9/tailbone/templates/products/batch.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/products/view.mako` & `Tailbone-0.9.9/tailbone/templates/products/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/products/lookup.mako` & `Tailbone-0.9.9/tailbone/templates/products/lookup.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/products/pending/view.mako` & `Tailbone-0.9.9/tailbone/templates/products/pending/view.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/products/index.mako` & `Tailbone-0.9.9/tailbone/templates/products/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/products/configure.mako` & `Tailbone-0.9.9/tailbone/templates/products/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/units-of-measure/index.mako` & `Tailbone-0.9.9/tailbone/templates/units-of-measure/index.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/trainwreck/transactions/rollover.mako` & `Tailbone-0.9.9/tailbone/templates/trainwreck/transactions/rollover.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/trainwreck/transactions/configure.mako` & `Tailbone-0.9.9/tailbone/templates/trainwreck/transactions/configure.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/templates/progress.mako` & `Tailbone-0.9.9/tailbone/templates/progress.mako`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/handler.py` & `Tailbone-0.9.9/tailbone/handler.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/forms/receiving.py` & `Tailbone-0.9.9/tailbone/forms/receiving.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/forms/common.py` & `Tailbone-0.9.9/tailbone/forms/common.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/forms/widgets.py` & `Tailbone-0.9.9/tailbone/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/forms/core.py` & `Tailbone-0.9.9/tailbone/forms/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/forms/types.py` & `Tailbone-0.9.9/tailbone/forms/types.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/forms/__init__.py` & `Tailbone-0.9.9/tailbone/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/util.py` & `Tailbone-0.9.9/tailbone/util.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/progress.py` & `Tailbone-0.9.9/tailbone/progress.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/auth.py` & `Tailbone-0.9.9/tailbone/auth.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/beaker.py` & `Tailbone-0.9.9/tailbone/beaker.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/app.py` & `Tailbone-0.9.9/tailbone/app.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/purchasing/batch.py` & `Tailbone-0.9.9/tailbone/views/purchasing/batch.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/purchasing/receiving.py` & `Tailbone-0.9.9/tailbone/views/purchasing/receiving.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/purchasing/ordering.py` & `Tailbone-0.9.9/tailbone/views/purchasing/ordering.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/purchasing/costing.py` & `Tailbone-0.9.9/tailbone/views/purchasing/costing.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/purchasing/__init__.py` & `Tailbone-0.9.9/tailbone/views/purchasing/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/asgi/upgrades.py` & `Tailbone-0.9.9/tailbone/views/asgi/upgrades.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/asgi/datasync.py` & `Tailbone-0.9.9/tailbone/views/asgi/datasync.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/asgi/__init__.py` & `Tailbone-0.9.9/tailbone/views/asgi/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/products.py` & `Tailbone-0.9.9/tailbone/views/products.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/customers.py` & `Tailbone-0.9.9/tailbone/views/customers.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/reportcodes.py` & `Tailbone-0.9.9/tailbone/views/reportcodes.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/taxes.py` & `Tailbone-0.9.9/tailbone/views/taxes.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/menus.py` & `Tailbone-0.9.9/tailbone/views/menus.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/vendors/catalogs.py` & `Tailbone-0.9.9/tailbone/views/vendors/catalogs.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/vendors/invoices.py` & `Tailbone-0.9.9/tailbone/views/vendors/invoices.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/vendors/core.py` & `Tailbone-0.9.9/tailbone/views/vendors/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/vendors/__init__.py` & `Tailbone-0.9.9/tailbone/views/vendors/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/inventory.py` & `Tailbone-0.9.9/tailbone/views/inventory.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/labels/batch.py` & `Tailbone-0.9.9/tailbone/views/labels/batch.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/labels/profiles.py` & `Tailbone-0.9.9/tailbone/views/labels/profiles.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/labels/__init__.py` & `Tailbone-0.9.9/tailbone/views/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/purchases/credits.py` & `Tailbone-0.9.9/tailbone/views/purchases/credits.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/purchases/core.py` & `Tailbone-0.9.9/tailbone/views/purchases/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/purchases/__init__.py` & `Tailbone-0.9.9/tailbone/views/purchases/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/essentials.py` & `Tailbone-0.9.9/tailbone/views/essentials.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/employees.py` & `Tailbone-0.9.9/tailbone/views/employees.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/permissions.py` & `Tailbone-0.9.9/tailbone/views/permissions.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/custorders/batch.py` & `Tailbone-0.9.9/tailbone/views/custorders/batch.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/custorders/orders.py` & `Tailbone-0.9.9/tailbone/views/custorders/orders.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/custorders/items.py` & `Tailbone-0.9.9/tailbone/views/custorders/items.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/custorders/creating.py` & `Tailbone-0.9.9/tailbone/views/custorders/creating.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/custorders/__init__.py` & `Tailbone-0.9.9/tailbone/views/custorders/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/master.py` & `Tailbone-0.9.9/tailbone/views/master.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/members.py` & `Tailbone-0.9.9/tailbone/views/members.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/stores.py` & `Tailbone-0.9.9/tailbone/views/stores.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/email.py` & `Tailbone-0.9.9/tailbone/views/email.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/luigi.py` & `Tailbone-0.9.9/tailbone/views/luigi.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/projects.py` & `Tailbone-0.9.9/tailbone/views/projects.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/reports.py` & `Tailbone-0.9.9/tailbone/views/reports.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/filemon.py` & `Tailbone-0.9.9/tailbone/views/filemon.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/customergroups.py` & `Tailbone-0.9.9/tailbone/views/customergroups.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/bouncer.py` & `Tailbone-0.9.9/tailbone/views/bouncer.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/categories.py` & `Tailbone-0.9.9/tailbone/views/categories.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/shifts/timesheet.py` & `Tailbone-0.9.9/tailbone/views/shifts/timesheet.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/shifts/core.py` & `Tailbone-0.9.9/tailbone/views/shifts/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/shifts/lib.py` & `Tailbone-0.9.9/tailbone/views/shifts/lib.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/shifts/__init__.py` & `Tailbone-0.9.9/tailbone/views/shifts/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/shifts/schedule.py` & `Tailbone-0.9.9/tailbone/views/shifts/schedule.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/upgrades.py` & `Tailbone-0.9.9/tailbone/views/upgrades.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/progress.py` & `Tailbone-0.9.9/tailbone/views/progress.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/views.py` & `Tailbone-0.9.9/tailbone/views/views.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/common.py` & `Tailbone-0.9.9/tailbone/views/common.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/auth.py` & `Tailbone-0.9.9/tailbone/views/auth.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/features.py` & `Tailbone-0.9.9/tailbone/views/features.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/datasync.py` & `Tailbone-0.9.9/tailbone/views/datasync.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/ifps.py` & `Tailbone-0.9.9/tailbone/views/ifps.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/people.py` & `Tailbone-0.9.9/tailbone/views/people.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/roles.py` & `Tailbone-0.9.9/tailbone/views/roles.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/users.py` & `Tailbone-0.9.9/tailbone/views/users.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/subdepartments.py` & `Tailbone-0.9.9/tailbone/views/subdepartments.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/tables.py` & `Tailbone-0.9.9/tailbone/views/tables.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/brands.py` & `Tailbone-0.9.9/tailbone/views/brands.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/principal.py` & `Tailbone-0.9.9/tailbone/views/principal.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/core.py` & `Tailbone-0.9.9/tailbone/views/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/importing.py` & `Tailbone-0.9.9/tailbone/views/importing.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/workorders.py` & `Tailbone-0.9.9/tailbone/views/workorders.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/tempmon/readings.py` & `Tailbone-0.9.9/tailbone/views/tempmon/readings.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/tempmon/appliances.py` & `Tailbone-0.9.9/tailbone/views/tempmon/appliances.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/tempmon/clients.py` & `Tailbone-0.9.9/tailbone/views/tempmon/clients.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/tempmon/core.py` & `Tailbone-0.9.9/tailbone/views/tempmon/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/tempmon/probes.py` & `Tailbone-0.9.9/tailbone/views/tempmon/probes.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/tempmon/dashboard.py` & `Tailbone-0.9.9/tailbone/views/tempmon/dashboard.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/tempmon/__init__.py` & `Tailbone-0.9.9/tailbone/views/tempmon/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/handheld.py` & `Tailbone-0.9.9/tailbone/views/handheld.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/batch/delproduct.py` & `Tailbone-0.9.9/tailbone/views/batch/delproduct.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/batch/product.py` & `Tailbone-0.9.9/tailbone/views/batch/product.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/batch/inventory.py` & `Tailbone-0.9.9/tailbone/views/batch/inventory.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/batch/newproduct.py` & `Tailbone-0.9.9/tailbone/views/batch/newproduct.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/batch/vendorinvoice.py` & `Tailbone-0.9.9/tailbone/views/batch/vendorinvoice.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/batch/labels.py` & `Tailbone-0.9.9/tailbone/views/batch/labels.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/batch/importer.py` & `Tailbone-0.9.9/tailbone/views/batch/importer.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/batch/core.py` & `Tailbone-0.9.9/tailbone/views/batch/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/batch/handheld.py` & `Tailbone-0.9.9/tailbone/views/batch/handheld.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/batch/__init__.py` & `Tailbone-0.9.9/tailbone/views/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/batch/pricing.py` & `Tailbone-0.9.9/tailbone/views/batch/pricing.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/batch/vendorcatalog.py` & `Tailbone-0.9.9/tailbone/views/batch/vendorcatalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,16 @@
             f.set_renderer('parser_key', self.render_parser_key)
 
         # vendor
         f.set_renderer('vendor', self.render_vendor)
         if self.creating and 'vendor' in f:
             f.replace('vendor', 'vendor_uuid')
             f.set_label('vendor_uuid', "Vendor")
+            f.set_required('vendor_uuid')
+            f.set_validator('vendor_uuid', self.valid_vendor_uuid)
 
             # should we use dropdown or autocomplete?  note that if
             # autocomplete is to be used, we also must make sure we
             # have an autocomplete url registered
             use_dropdown = vendor_handler.choice_uses_dropdown()
             if not use_dropdown:
                 try:
@@ -254,14 +256,21 @@
             f.set_type('cache_products', 'boolean')
             f.set_helptext('cache_products',
                            "If set, will pre-cache all products for quicker "
                            "lookups when loading the catalog.")
         else:
             f.remove('cache_products')
 
+    def valid_vendor_uuid(self, node, value):
+        model = self.model
+        if value:
+            vendor = self.Session.get(model.Vendor, value)
+            if not vendor:
+                raise colander.Invalid(node, "Vendor not found")
+
     def render_parser_key(self, batch, field):
         key = getattr(batch, field)
         if not key:
             return
         app = self.get_rattail_app()
         vendor_handler = app.get_vendor_handler()
         parser = vendor_handler.get_catalog_parser(key)
```

### Comparing `Tailbone-0.9.8/tailbone/views/exports.py` & `Tailbone-0.9.9/tailbone/views/exports.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/uoms.py` & `Tailbone-0.9.9/tailbone/views/uoms.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/departments.py` & `Tailbone-0.9.9/tailbone/views/departments.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/poser/master.py` & `Tailbone-0.9.9/tailbone/views/poser/master.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/poser/reports.py` & `Tailbone-0.9.9/tailbone/views/poser/reports.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/poser/views.py` & `Tailbone-0.9.9/tailbone/views/poser/views.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/poser/__init__.py` & `Tailbone-0.9.9/tailbone/views/poser/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/settings.py` & `Tailbone-0.9.9/tailbone/views/settings.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/depositlinks.py` & `Tailbone-0.9.9/tailbone/views/depositlinks.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/__init__.py` & `Tailbone-0.9.9/tailbone/views/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/families.py` & `Tailbone-0.9.9/tailbone/views/families.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/trainwreck/defaults.py` & `Tailbone-0.9.9/tailbone/views/trainwreck/defaults.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/trainwreck/base.py` & `Tailbone-0.9.9/tailbone/views/trainwreck/base.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/trainwreck/__init__.py` & `Tailbone-0.9.9/tailbone/views/trainwreck/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/versions.py` & `Tailbone-0.9.9/tailbone/views/versions.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/views/messages.py` & `Tailbone-0.9.9/tailbone/views/messages.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/helpers.py` & `Tailbone-0.9.9/tailbone/helpers.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/products.py` & `Tailbone-0.9.9/tailbone/api/products.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/customers.py` & `Tailbone-0.9.9/tailbone/api/customers.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/master.py` & `Tailbone-0.9.9/tailbone/api/master.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/vendors.py` & `Tailbone-0.9.9/tailbone/api/vendors.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/master2.py` & `Tailbone-0.9.9/tailbone/api/master2.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/upgrades.py` & `Tailbone-0.9.9/tailbone/api/upgrades.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/common.py` & `Tailbone-0.9.9/tailbone/api/common.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/auth.py` & `Tailbone-0.9.9/tailbone/api/auth.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/labels.py` & `Tailbone-0.9.9/tailbone/api/labels.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/people.py` & `Tailbone-0.9.9/tailbone/api/people.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/users.py` & `Tailbone-0.9.9/tailbone/api/users.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/core.py` & `Tailbone-0.9.9/tailbone/api/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/workorders.py` & `Tailbone-0.9.9/tailbone/api/workorders.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/batch/inventory.py` & `Tailbone-0.9.9/tailbone/api/batch/inventory.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/batch/receiving.py` & `Tailbone-0.9.9/tailbone/api/batch/receiving.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/batch/ordering.py` & `Tailbone-0.9.9/tailbone/api/batch/ordering.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/batch/labels.py` & `Tailbone-0.9.9/tailbone/api/batch/labels.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/batch/core.py` & `Tailbone-0.9.9/tailbone/api/batch/core.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/batch/__init__.py` & `Tailbone-0.9.9/tailbone/api/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/api/__init__.py` & `Tailbone-0.9.9/tailbone/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/diffs.py` & `Tailbone-0.9.9/tailbone/diffs.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/exceptions.py` & `Tailbone-0.9.9/tailbone/exceptions.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/tweens.py` & `Tailbone-0.9.9/tailbone/tweens.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/providers.py` & `Tailbone-0.9.9/tailbone/providers.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/__init__.py` & `Tailbone-0.9.9/tailbone/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/asgi.py` & `Tailbone-0.9.9/tailbone/asgi.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/webapi.py` & `Tailbone-0.9.9/tailbone/webapi.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/files/vendor_catalog_template.xlsx` & `Tailbone-0.9.9/tailbone/static/files/vendor_catalog_template.xlsx`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/files/newproduct_template.xlsx` & `Tailbone-0.9.9/tailbone/static/files/newproduct_template.xlsx`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/css/codehilite.css` & `Tailbone-0.9.9/tailbone/static/css/codehilite.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/css/grids.css` & `Tailbone-0.9.9/tailbone/static/css/grids.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/css/forms.css` & `Tailbone-0.9.9/tailbone/static/css/forms.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/css/diffs.css` & `Tailbone-0.9.9/tailbone/static/css/diffs.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/css/progress.css` & `Tailbone-0.9.9/tailbone/static/css/progress.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/css/perms.css` & `Tailbone-0.9.9/tailbone/static/css/perms.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/css/layout.css` & `Tailbone-0.9.9/tailbone/static/css/layout.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/css/normalize.css` & `Tailbone-0.9.9/tailbone/static/css/normalize.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/css/timesheet.css` & `Tailbone-0.9.9/tailbone/static/css/timesheet.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/css/grids.rowstatus.css` & `Tailbone-0.9.9/tailbone/static/css/grids.rowstatus.css`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/js/tailbone.buefy.oncebutton.js` & `Tailbone-0.9.9/tailbone/static/js/tailbone.buefy.oncebutton.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/js/debounce.js` & `Tailbone-0.9.9/tailbone/static/js/debounce.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/js/tailbone.buefy.autocomplete.js` & `Tailbone-0.9.9/tailbone/static/js/tailbone.buefy.autocomplete.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/js/numeric.js` & `Tailbone-0.9.9/tailbone/static/js/numeric.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/js/tailbone.feedback.js` & `Tailbone-0.9.9/tailbone/static/js/tailbone.feedback.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/js/tailbone.buefy.numericinput.js` & `Tailbone-0.9.9/tailbone/static/js/tailbone.buefy.numericinput.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/js/tailbone.buefy.datepicker.js` & `Tailbone-0.9.9/tailbone/static/js/tailbone.buefy.datepicker.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/js/tailbone.buefy.message_recipients.js` & `Tailbone-0.9.9/tailbone/static/js/tailbone.buefy.message_recipients.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/js/tailbone.buefy.grid.js` & `Tailbone-0.9.9/tailbone/static/js/tailbone.buefy.grid.js`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/img/loading.gif` & `Tailbone-0.9.9/tailbone/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/img/view.png` & `Tailbone-0.9.9/tailbone/static/img/view.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/img/save.png` & `Tailbone-0.9.9/tailbone/static/img/save.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/img/product.png` & `Tailbone-0.9.9/tailbone/static/img/product.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/img/edit.png` & `Tailbone-0.9.9/tailbone/static/img/edit.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/img/Hymenocephalus_italicus.jpg` & `Tailbone-0.9.9/tailbone/static/img/Hymenocephalus_italicus.jpg`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/img/home_logo.png` & `Tailbone-0.9.9/tailbone/static/img/home_logo.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/img/rattail.ico` & `Tailbone-0.9.9/tailbone/static/img/rattail.ico`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/img/testing.png` & `Tailbone-0.9.9/tailbone/static/img/testing.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/img/delete.png` & `Tailbone-0.9.9/tailbone/static/img/delete.png`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/static/__init__.py` & `Tailbone-0.9.9/tailbone/static/__init__.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/tailbone/config.py` & `Tailbone-0.9.9/tailbone/config.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/setup.py` & `Tailbone-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/COPYING.txt` & `Tailbone-0.9.9/COPYING.txt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/CHANGES.rst` & `Tailbone-0.9.9/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 
 CHANGELOG
 =========
 
+0.9.9 (2023-02-21)
+------------------
+
+* Validate vendor for catalog batch upload.
+
+
 0.9.8 (2023-02-20)
 ------------------
 
 * Make ``config`` param more explicit, for GridFilter constructor.
 
 
 0.9.7 (2023-02-14)
```

### Comparing `Tailbone-0.9.8/tasks.py` & `Tailbone-0.9.9/tasks.py`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/PKG-INFO` & `Tailbone-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tailbone
-Version: 0.9.8
+Version: 0.9.9
 Summary: Backoffice Web Application for Rattail
 Home-page: http://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Tailbone-0.9.8/Tailbone.egg-info/SOURCES.txt` & `Tailbone-0.9.9/Tailbone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Tailbone-0.9.8/Tailbone.egg-info/PKG-INFO` & `Tailbone-0.9.9/Tailbone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tailbone
-Version: 0.9.8
+Version: 0.9.9
 Summary: Backoffice Web Application for Rattail
 Home-page: http://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

