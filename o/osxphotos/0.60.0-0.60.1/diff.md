# Comparing `tmp/osxphotos-0.60.0.tar.gz` & `tmp/osxphotos-0.60.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osxphotos-0.60.0.tar", last modified: Sun May  7 14:48:43 2023, max compression
+gzip compressed data, was "osxphotos-0.60.1.tar", last modified: Sun May 14 15:28:30 2023, max compression
```

## Comparing `osxphotos-0.60.0.tar` & `osxphotos-0.60.1.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.569779 osxphotos-0.60.0/
--rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.0/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.0/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-05-07 14:48:43.569088 osxphotos-0.60.0/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)   224064 2023-05-07 14:48:33.000000 osxphotos-0.60.0/README.md
--rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.0/README.rst
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.507659 osxphotos-0.60.0/osxphotos/
--rw-r--r--   0 rhet       (501) staff       (20)     1952 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.0/osxphotos/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15945 2023-05-07 14:44:48.000000 osxphotos-0.60.0/osxphotos/_constants.py
--rw-r--r--   0 rhet       (501) staff       (20)       45 2023-05-07 14:38:45.000000 osxphotos-0.60.0/osxphotos/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.0/osxphotos/adjustmentsinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.0/osxphotos/albuminfo.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.527845 osxphotos-0.60.0/osxphotos/cli/
--rw-r--r--   0 rhet       (501) staff       (20)     3565 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.0/osxphotos/cli/about.py
--rw-r--r--   0 rhet       (501) staff       (20)     6869 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/albums.py
--rw-r--r--   0 rhet       (501) staff       (20)     9933 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3802 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/cli_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)    26594 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/cli_params.py
--rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/click_rich_echo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.0/osxphotos/cli/color_themes.py
--rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/common.py
--rw-r--r--   0 rhet       (501) staff       (20)      713 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/darkmode.py
--rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/debug_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/docs.py
--rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/dump.py
--rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/exiftool_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)   106908 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/export.py
--rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/grep.py
--rw-r--r--   0 rhet       (501) staff       (20)    22101 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/help.py
--rw-r--r--   0 rhet       (501) staff       (20)    61649 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/import_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/info.py
--rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/install_uninstall_run.py
--rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/keywords.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/kvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/labels.py
--rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/list.py
--rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.0/osxphotos/cli/orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/persons.py
--rw-r--r--   0 rhet       (501) staff       (20)    20564 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/photo_inspect.py
--rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/places.py
--rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/print_photo_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     5674 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/query.py
--rw-r--r--   0 rhet       (501) staff       (20)     7833 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/repl.py
--rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/report_writer.py
--rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.0/osxphotos/cli/rich_progress.py
--rw-r--r--   0 rhet       (501) staff       (20)     3355 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/show_command.py
--rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/snap_diff.py
--rw-r--r--   0 rhet       (501) staff       (20)    26935 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/cli/sync.py
--rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/sync_results.py
--rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.0/osxphotos/cli/theme.py
--rw-r--r--   0 rhet       (501) staff       (20)    28044 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.0/osxphotos/cli/tutorial.py
--rw-r--r--   0 rhet       (501) staff       (20)      692 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/cli/uuid.py
--rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/cli/verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-02-03 04:08:06.000000 osxphotos-0.60.0/osxphotos/cli/version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5089 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/compare_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/crash_reporter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.0/osxphotos/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/debug.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.528403 osxphotos-0.60.0/osxphotos/docs/
--rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.0/osxphotos/docs/README.md
--rw-r--r--   0 rhet       (501) staff       (20)  1459529 2023-05-07 14:48:39.000000 osxphotos-0.60.0/osxphotos/docs/docs.zip
--rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/exif_datetime_updater.py
--rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.0/osxphotos/exifinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.0/osxphotos/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.0/osxphotos/exiftool_filetypes.json
--rw-r--r--   0 rhet       (501) staff       (20)    51732 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/export_db_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    10742 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/frozen_photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5121 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/imageconverter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.0/osxphotos/momentinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     3787 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/photodates.py
--rw-r--r--   0 rhet       (501) staff       (20)    89066 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/photoexporter.py
--rw-r--r--   0 rhet       (501) staff       (20)    80700 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    46258 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     5542 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/photosalbum.py
--rw-r--r--   0 rhet       (501) staff       (20)     5332 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/photoscript_utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.535350 osxphotos-0.60.0/osxphotos/photosdb/
--rw-r--r--   0 rhet       (501) staff       (20)      215 2020-08-09 15:12:11.000000 osxphotos-0.60.0/osxphotos/photosdb/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)    10393 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7615 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)   149146 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/photosdb/photosdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/photosdb/photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.0/osxphotos/phototables.py
--rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.0/osxphotos/phototemplate.cog.md
--rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-05-07 14:48:32.000000 osxphotos-0.60.0/osxphotos/phototemplate.md
--rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/phototemplate.py
--rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.0/osxphotos/phototemplate.tx
--rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/phototz.py
--rw-r--r--   0 rhet       (501) staff       (20)    21858 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.0/osxphotos/pyrepl.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.537111 osxphotos-0.60.0/osxphotos/queries/
--rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.0/osxphotos/queries/README.md
--rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.0/osxphotos/queries/cloud_album_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.0/osxphotos/queries/shared_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.0/osxphotos/queries/title.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.0/osxphotos/query_builder.py
--rw-r--r--   0 rhet       (501) staff       (20)    13457 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/queryoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.0/osxphotos/rich_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/sqlgrep.py
--rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.0/osxphotos/sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/template_counter.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.538126 osxphotos-0.60.0/osxphotos/templates/
--rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.0/osxphotos/templates/DESCRIPTION.txt
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/templates/xmp_sidecar.mako
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/templates/xmp_sidecar_beta.mako
--rw-r--r--   0 rhet       (501) staff       (20)     3242 2023-05-07 13:56:16.000000 osxphotos-0.60.0/osxphotos/text_detection.py
--rw-r--r--   0 rhet       (501) staff       (20)     2282 2022-05-05 03:55:31.000000 osxphotos-0.60.0/osxphotos/timeutils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3442 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/timezones.py
--rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.0/osxphotos/tutorial.md
--rw-r--r--   0 rhet       (501) staff       (20)    27213 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)    18621 2023-05-07 14:33:19.000000 osxphotos-0.60.0/osxphotos/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.510165 osxphotos-0.60.0/osxphotos.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-05-07 14:48:43.000000 osxphotos-0.60.0/osxphotos.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     6344 2023-05-07 14:48:43.000000 osxphotos-0.60.0/osxphotos.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2023-05-07 14:48:43.000000 osxphotos-0.60.0/osxphotos.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       58 2023-05-07 14:48:43.000000 osxphotos-0.60.0/osxphotos.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      888 2023-05-07 14:48:43.000000 osxphotos-0.60.0/osxphotos.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)       16 2023-05-07 14:48:43.000000 osxphotos-0.60.0/osxphotos.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2023-05-07 14:48:43.569822 osxphotos-0.60.0/setup.cfg
--rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.0/setup.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.567919 osxphotos-0.60.0/tests/
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-07 14:48:43.568686 osxphotos-0.60.0/tests/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.0/tests/plugins/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.0/tests/plugins/env_vars.py
--rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_10_12_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    11012 2022-02-07 05:54:47.000000 osxphotos-0.60.0/tests/test_albums_folders_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     4849 2021-06-12 05:33:53.000000 osxphotos-0.60.0/tests/test_albums_folders_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     5334 2021-06-12 05:33:48.000000 osxphotos-0.60.0/tests/test_albums_folders_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_bigsur_10_16_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    54731 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)   273142 2023-05-07 14:25:27.000000 osxphotos-0.60.0/tests/test_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     1798 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_cli_add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     4571 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_cli_add_to_album.py
--rw-r--r--   0 rhet       (501) staff       (20)     2218 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_cli_all_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)     6798 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_cli_batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.0/tests/test_cli_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_export_cloud.py
--rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.0/tests/test_cli_export_projects.py
--rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)    29996 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_cli_import.py
--rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     6397 2022-05-05 04:33:28.000000 osxphotos-0.60.0/tests/test_cli_param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     3450 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_cli_sync.py
--rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_cli_verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.0/tests/test_cloud_owner_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.0/tests/test_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.0/tests/test_concurrent_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.0/tests/test_configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     1946 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2748 2022-05-06 13:53:04.000000 osxphotos-0.60.0/tests/test_datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_debug.py
--rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-01-21 18:04:00.000000 osxphotos-0.60.0/tests/test_empty_library_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.0/tests/test_exif_info.py
--rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     9781 2021-04-26 00:13:29.000000 osxphotos-0.60.0/tests/test_exiftool_caching.py
--rw-r--r--   0 rhet       (501) staff       (20)    18308 2022-05-21 05:13:12.000000 osxphotos-0.60.0/tests/test_export_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     5910 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_export_catalina_10_15_7_use_photos_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.0/tests/test_export_convert_to_jpeg.py
--rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    10301 2022-05-21 05:13:12.000000 osxphotos-0.60.0/tests/test_export_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3892 2021-03-14 19:20:10.000000 osxphotos-0.60.0/tests/test_export_raw_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_exportresults.py
--rw-r--r--   0 rhet       (501) staff       (20)   155137 2022-06-17 17:31:26.000000 osxphotos-0.60.0/tests/test_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_highsierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     4022 2022-01-01 04:28:52.000000 osxphotos-0.60.0/tests/test_image_converter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_incloud_big_sur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.0/tests/test_incloud_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_incloud_catalina_10_15_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1270 2021-06-12 05:43:32.000000 osxphotos-0.60.0/tests/test_incloud_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.0/tests/test_live_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)      859 2021-06-12 05:45:42.000000 osxphotos-0.60.0/tests/test_modified_date_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)      930 2021-06-12 05:46:24.000000 osxphotos-0.60.0/tests/test_modified_date_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.0/tests/test_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1205 2020-01-12 08:00:41.000000 osxphotos-0.60.0/tests/test_mojave_10_14_6_path_edited.py
--rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_monterey_12_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    50393 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_monterey_dev_beta_12_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4731 2020-06-27 19:46:37.000000 osxphotos-0.60.0/tests/test_movies_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4870 2020-06-27 19:50:41.000000 osxphotos-0.60.0/tests/test_movies_5_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    13430 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5796 2020-10-27 13:37:01.000000 osxphotos-0.60.0/tests/test_places_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.0/tests/test_places_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.0/tests/test_places_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.0/tests/test_projects_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.0/tests/test_projects_sierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     3376 2022-01-02 07:10:11.000000 osxphotos-0.60.0/tests/test_score_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2020-05-11 01:55:25.000000 osxphotos-0.60.0/tests/test_search_info_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     7530 2020-12-25 19:00:06.000000 osxphotos-0.60.0/tests/test_search_info_10_15_4.py
--rw-r--r--   0 rhet       (501) staff       (20)    10047 2022-01-18 16:08:28.000000 osxphotos-0.60.0/tests/test_search_info_10_15_5.py
--rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_search_info_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_shared_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1744 2020-10-05 13:13:43.000000 osxphotos-0.60.0/tests/test_shared_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_shared_ventura_13_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.0/tests/test_sidecar_xmp.py
--rw-r--r--   0 rhet       (501) staff       (20)     3017 2020-08-23 23:26:56.000000 osxphotos-0.60.0/tests/test_specials_bigsur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.0/tests/test_specials_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.0/tests/test_specials_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.0/tests/test_specials_sierra_10_12.py
--rw-r--r--   0 rhet       (501) staff       (20)      489 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)    50016 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_template.py
--rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_template_counter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_template_today.py
--rw-r--r--   0 rhet       (501) staff       (20)     2032 2023-05-07 13:56:16.000000 osxphotos-0.60.0/tests/test_uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.0/tests/test_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.0/tests/test_ventura_13_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-03-09 14:25:57.000000 osxphotos-0.60.0/tests/test_ventura_dev_preview_13_0_0.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.485674 osxphotos-0.60.1/
+-rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.1/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.1/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-05-14 15:28:30.485482 osxphotos-0.60.1/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)   224064 2023-05-14 15:28:19.000000 osxphotos-0.60.1/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.1/README.rst
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.424011 osxphotos-0.60.1/osxphotos/
+-rw-r--r--   0 rhet       (501) staff       (20)     1952 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.1/osxphotos/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15945 2023-05-07 15:00:00.000000 osxphotos-0.60.1/osxphotos/_constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2023-05-14 15:28:16.000000 osxphotos-0.60.1/osxphotos/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.1/osxphotos/adjustmentsinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.1/osxphotos/albuminfo.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.435499 osxphotos-0.60.1/osxphotos/cli/
+-rw-r--r--   0 rhet       (501) staff       (20)     3565 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.1/osxphotos/cli/about.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6869 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/albums.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9933 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3802 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/cli_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26594 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/cli_params.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/click_rich_echo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.1/osxphotos/cli/color_themes.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/common.py
+-rw-r--r--   0 rhet       (501) staff       (20)      713 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/darkmode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/debug_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/docs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/exiftool_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)   106908 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/export.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/grep.py
+-rw-r--r--   0 rhet       (501) staff       (20)    22101 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/help.py
+-rw-r--r--   0 rhet       (501) staff       (20)    61649 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/import_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/install_uninstall_run.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/keywords.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/kvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/labels.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/list.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.1/osxphotos/cli/orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/persons.py
+-rw-r--r--   0 rhet       (501) staff       (20)    20564 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/photo_inspect.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/places.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/print_photo_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5674 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/query.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7833 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/repl.py
+-rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/report_writer.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.1/osxphotos/cli/rich_progress.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3355 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/show_command.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/snap_diff.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26935 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/cli/sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/sync_results.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.1/osxphotos/cli/theme.py
+-rw-r--r--   0 rhet       (501) staff       (20)    28044 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.1/osxphotos/cli/tutorial.py
+-rw-r--r--   0 rhet       (501) staff       (20)      692 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/cli/uuid.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/cli/verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-02-03 04:08:06.000000 osxphotos-0.60.1/osxphotos/cli/version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5089 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/compare_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/crash_reporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.1/osxphotos/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/debug.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.436446 osxphotos-0.60.1/osxphotos/docs/
+-rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.1/osxphotos/docs/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)  1467005 2023-05-14 15:28:27.000000 osxphotos-0.60.1/osxphotos/docs/docs.zip
+-rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/exif_datetime_updater.py
+-rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.1/osxphotos/exifinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.1/osxphotos/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.1/osxphotos/exiftool_filetypes.json
+-rw-r--r--   0 rhet       (501) staff       (20)    51790 2023-05-14 15:28:03.000000 osxphotos-0.60.1/osxphotos/export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/export_db_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10742 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/frozen_photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5121 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/imageconverter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.1/osxphotos/momentinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3787 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/photodates.py
+-rw-r--r--   0 rhet       (501) staff       (20)    89066 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/photoexporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)    80700 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    46258 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5542 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/photosalbum.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5332 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/photoscript_utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.439611 osxphotos-0.60.1/osxphotos/photosdb/
+-rw-r--r--   0 rhet       (501) staff       (20)      215 2020-08-09 15:12:11.000000 osxphotos-0.60.1/osxphotos/photosdb/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10393 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7615 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)   149146 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/photosdb/photosdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/photosdb/photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.1/osxphotos/phototables.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.1/osxphotos/phototemplate.cog.md
+-rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-05-14 15:28:19.000000 osxphotos-0.60.1/osxphotos/phototemplate.md
+-rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/phototemplate.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.1/osxphotos/phototemplate.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/phototz.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21858 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.1/osxphotos/pyrepl.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.440980 osxphotos-0.60.1/osxphotos/queries/
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.1/osxphotos/queries/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.1/osxphotos/queries/cloud_album_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.1/osxphotos/queries/shared_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.1/osxphotos/queries/title.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.1/osxphotos/query_builder.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13457 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/queryoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.1/osxphotos/rich_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/sqlgrep.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.1/osxphotos/sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/template_counter.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.442050 osxphotos-0.60.1/osxphotos/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.1/osxphotos/templates/DESCRIPTION.txt
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/templates/xmp_sidecar.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/templates/xmp_sidecar_beta.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     3242 2023-05-07 13:56:16.000000 osxphotos-0.60.1/osxphotos/text_detection.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2282 2022-05-05 03:55:31.000000 osxphotos-0.60.1/osxphotos/timeutils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3442 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/timezones.py
+-rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.1/osxphotos/tutorial.md
+-rw-r--r--   0 rhet       (501) staff       (20)    27213 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18621 2023-05-07 14:33:19.000000 osxphotos-0.60.1/osxphotos/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.424732 osxphotos-0.60.1/osxphotos.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-05-14 15:28:30.000000 osxphotos-0.60.1/osxphotos.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     6344 2023-05-14 15:28:30.000000 osxphotos-0.60.1/osxphotos.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2023-05-14 15:28:30.000000 osxphotos-0.60.1/osxphotos.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       58 2023-05-14 15:28:30.000000 osxphotos-0.60.1/osxphotos.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      888 2023-05-14 15:28:30.000000 osxphotos-0.60.1/osxphotos.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       16 2023-05-14 15:28:30.000000 osxphotos-0.60.1/osxphotos.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2023-05-14 15:28:30.485709 osxphotos-0.60.1/setup.cfg
+-rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.1/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.484725 osxphotos-0.60.1/tests/
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-05-14 15:28:30.485158 osxphotos-0.60.1/tests/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.1/tests/plugins/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.1/tests/plugins/env_vars.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_10_12_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11012 2022-02-07 05:54:47.000000 osxphotos-0.60.1/tests/test_albums_folders_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4849 2021-06-12 05:33:53.000000 osxphotos-0.60.1/tests/test_albums_folders_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5334 2021-06-12 05:33:48.000000 osxphotos-0.60.1/tests/test_albums_folders_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_bigsur_10_16_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    54731 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)   273142 2023-05-07 14:25:27.000000 osxphotos-0.60.1/tests/test_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1798 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_cli_add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4571 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_cli_add_to_album.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2218 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_cli_all_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6798 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_cli_batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.1/tests/test_cli_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_export_cloud.py
+-rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.1/tests/test_cli_export_projects.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)    29996 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_cli_import.py
+-rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6397 2022-05-05 04:33:28.000000 osxphotos-0.60.1/tests/test_cli_param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3450 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_cli_sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_cli_verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.1/tests/test_cloud_owner_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.1/tests/test_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.1/tests/test_concurrent_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.1/tests/test_configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1946 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2748 2022-05-06 13:53:04.000000 osxphotos-0.60.1/tests/test_datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_debug.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-01-21 18:04:00.000000 osxphotos-0.60.1/tests/test_empty_library_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.1/tests/test_exif_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9781 2021-04-26 00:13:29.000000 osxphotos-0.60.1/tests/test_exiftool_caching.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18308 2022-05-21 05:13:12.000000 osxphotos-0.60.1/tests/test_export_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5910 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_export_catalina_10_15_7_use_photos_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.1/tests/test_export_convert_to_jpeg.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10301 2022-05-21 05:13:12.000000 osxphotos-0.60.1/tests/test_export_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3892 2021-03-14 19:20:10.000000 osxphotos-0.60.1/tests/test_export_raw_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_exportresults.py
+-rw-r--r--   0 rhet       (501) staff       (20)   155137 2022-06-17 17:31:26.000000 osxphotos-0.60.1/tests/test_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_highsierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4022 2022-01-01 04:28:52.000000 osxphotos-0.60.1/tests/test_image_converter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_incloud_big_sur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.1/tests/test_incloud_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_incloud_catalina_10_15_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1270 2021-06-12 05:43:32.000000 osxphotos-0.60.1/tests/test_incloud_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.1/tests/test_live_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)      859 2021-06-12 05:45:42.000000 osxphotos-0.60.1/tests/test_modified_date_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)      930 2021-06-12 05:46:24.000000 osxphotos-0.60.1/tests/test_modified_date_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.1/tests/test_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1205 2020-01-12 08:00:41.000000 osxphotos-0.60.1/tests/test_mojave_10_14_6_path_edited.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_monterey_12_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50393 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_monterey_dev_beta_12_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4731 2020-06-27 19:46:37.000000 osxphotos-0.60.1/tests/test_movies_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4870 2020-06-27 19:50:41.000000 osxphotos-0.60.1/tests/test_movies_5_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13430 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5796 2020-10-27 13:37:01.000000 osxphotos-0.60.1/tests/test_places_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.1/tests/test_places_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.1/tests/test_places_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.1/tests/test_projects_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.1/tests/test_projects_sierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3376 2022-01-02 07:10:11.000000 osxphotos-0.60.1/tests/test_score_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2020-05-11 01:55:25.000000 osxphotos-0.60.1/tests/test_search_info_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7530 2020-12-25 19:00:06.000000 osxphotos-0.60.1/tests/test_search_info_10_15_4.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10047 2022-01-18 16:08:28.000000 osxphotos-0.60.1/tests/test_search_info_10_15_5.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_search_info_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_shared_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1744 2020-10-05 13:13:43.000000 osxphotos-0.60.1/tests/test_shared_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_shared_ventura_13_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.1/tests/test_sidecar_xmp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3017 2020-08-23 23:26:56.000000 osxphotos-0.60.1/tests/test_specials_bigsur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.1/tests/test_specials_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.1/tests/test_specials_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.1/tests/test_specials_sierra_10_12.py
+-rw-r--r--   0 rhet       (501) staff       (20)      489 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50016 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_template_counter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_template_today.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2032 2023-05-07 13:56:16.000000 osxphotos-0.60.1/tests/test_uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.1/tests/test_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.1/tests/test_ventura_13_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-03-09 14:25:57.000000 osxphotos-0.60.1/tests/test_ventura_dev_preview_13_0_0.py
```

### Comparing `osxphotos-0.60.0/LICENSE` & `osxphotos-0.60.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/PKG-INFO` & `osxphotos-0.60.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.0
+Version: 0.60.1
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.0/README.md` & `osxphotos-0.60.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2095,15 +2095,15 @@
 {openbracket}                   An open bracket: '['
 {closebracket}                  A close bracket: ']'
 {newline}                       A newline: '\n'
 {lf}                            A line feed: '\n', alias for {newline}
 {cr}                            A carriage return: '\r'
 {crlf}                          A carriage return + line feed: '\r\n'
 {tab}                           :A tab: '\t'
-{osxphotos_version}             The osxphotos version, e.g. '0.60.0'
+{osxphotos_version}             The osxphotos version, e.g. '0.60.1'
 {osxphotos_cmd_line}            The full command line used to run osxphotos
 
 The following substitutions may result in multiple values. Thus if specified
 for --directory these could result in multiple copies of a photo being being
 exported, one to each directory.  For example: --directory
 '{created.year}/{album}' could result in the same photo being exported to each
 of the following directories if the photos were created in 2019 and were in
@@ -2582,15 +2582,15 @@
 |{openbracket}|An open bracket: '['|
 |{closebracket}|A close bracket: ']'|
 |{newline}|A newline: '\n'|
 |{lf}|A line feed: '\n', alias for {newline}|
 |{cr}|A carriage return: '\r'|
 |{crlf}|A carriage return + line feed: '\r\n'|
 |{tab}|:A tab: '\t'|
-|{osxphotos_version}|The osxphotos version, e.g. '0.60.0'|
+|{osxphotos_version}|The osxphotos version, e.g. '0.60.1'|
 |{osxphotos_cmd_line}|The full command line used to run osxphotos|
 |{album}|Album(s) photo is contained in|
 |{folder_album}|Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{project}|Project(s) photo is contained in (such as greeting cards, calendars, slideshows)|
 |{album_project}|Album(s) and project(s) photo is contained in; treats projects as regular albums|
 |{folder_album_project}|Folder path + album (includes projects as albums) photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{keyword}|Keyword(s) assigned to photo|
```

### Comparing `osxphotos-0.60.0/README.rst` & `osxphotos-0.60.1/README.rst`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/__init__.py` & `osxphotos-0.60.1/osxphotos/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/_constants.py` & `osxphotos-0.60.1/osxphotos/_constants.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/adjustmentsinfo.py` & `osxphotos-0.60.1/osxphotos/adjustmentsinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/albuminfo.py` & `osxphotos-0.60.1/osxphotos/albuminfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/__init__.py` & `osxphotos-0.60.1/osxphotos/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/about.py` & `osxphotos-0.60.1/osxphotos/cli/about.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/add_locations.py` & `osxphotos-0.60.1/osxphotos/cli/add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/albums.py` & `osxphotos-0.60.1/osxphotos/cli/albums.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/batch_edit.py` & `osxphotos-0.60.1/osxphotos/cli/batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/cli.py` & `osxphotos-0.60.1/osxphotos/cli/cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/cli_commands.py` & `osxphotos-0.60.1/osxphotos/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/cli_params.py` & `osxphotos-0.60.1/osxphotos/cli/cli_params.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/click_rich_echo.py` & `osxphotos-0.60.1/osxphotos/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/color_themes.py` & `osxphotos-0.60.1/osxphotos/cli/color_themes.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/common.py` & `osxphotos-0.60.1/osxphotos/cli/common.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/darkmode.py` & `osxphotos-0.60.1/osxphotos/cli/darkmode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/debug_dump.py` & `osxphotos-0.60.1/osxphotos/cli/debug_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/docs.py` & `osxphotos-0.60.1/osxphotos/cli/docs.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/dump.py` & `osxphotos-0.60.1/osxphotos/cli/dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/exiftool_cli.py` & `osxphotos-0.60.1/osxphotos/cli/exiftool_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/export.py` & `osxphotos-0.60.1/osxphotos/cli/export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/exportdb.py` & `osxphotos-0.60.1/osxphotos/cli/exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/grep.py` & `osxphotos-0.60.1/osxphotos/cli/grep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/help.py` & `osxphotos-0.60.1/osxphotos/cli/help.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/import_cli.py` & `osxphotos-0.60.1/osxphotos/cli/import_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/info.py` & `osxphotos-0.60.1/osxphotos/cli/info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/install_uninstall_run.py` & `osxphotos-0.60.1/osxphotos/cli/install_uninstall_run.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/keywords.py` & `osxphotos-0.60.1/osxphotos/cli/keywords.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/kvstore.py` & `osxphotos-0.60.1/osxphotos/cli/kvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/labels.py` & `osxphotos-0.60.1/osxphotos/cli/labels.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/list.py` & `osxphotos-0.60.1/osxphotos/cli/list.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/orphans.py` & `osxphotos-0.60.1/osxphotos/cli/orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/param_types.py` & `osxphotos-0.60.1/osxphotos/cli/param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/persons.py` & `osxphotos-0.60.1/osxphotos/cli/persons.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/photo_inspect.py` & `osxphotos-0.60.1/osxphotos/cli/photo_inspect.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/places.py` & `osxphotos-0.60.1/osxphotos/cli/places.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/print_photo_info.py` & `osxphotos-0.60.1/osxphotos/cli/print_photo_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/query.py` & `osxphotos-0.60.1/osxphotos/cli/query.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/repl.py` & `osxphotos-0.60.1/osxphotos/cli/repl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/report_writer.py` & `osxphotos-0.60.1/osxphotos/cli/report_writer.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/rich_progress.py` & `osxphotos-0.60.1/osxphotos/cli/rich_progress.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/show_command.py` & `osxphotos-0.60.1/osxphotos/cli/show_command.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/snap_diff.py` & `osxphotos-0.60.1/osxphotos/cli/snap_diff.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/sync.py` & `osxphotos-0.60.1/osxphotos/cli/sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/sync_results.py` & `osxphotos-0.60.1/osxphotos/cli/sync_results.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/theme.py` & `osxphotos-0.60.1/osxphotos/cli/theme.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/timewarp.py` & `osxphotos-0.60.1/osxphotos/cli/timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/tutorial.py` & `osxphotos-0.60.1/osxphotos/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/uuid.py` & `osxphotos-0.60.1/osxphotos/cli/uuid.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/verbose.py` & `osxphotos-0.60.1/osxphotos/cli/verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/cli/version.py` & `osxphotos-0.60.1/osxphotos/cli/version.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/compare_exif.py` & `osxphotos-0.60.1/osxphotos/compare_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/configoptions.py` & `osxphotos-0.60.1/osxphotos/configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/crash_reporter.py` & `osxphotos-0.60.1/osxphotos/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/datetime_formatter.py` & `osxphotos-0.60.1/osxphotos/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/datetime_utils.py` & `osxphotos-0.60.1/osxphotos/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/debug.py` & `osxphotos-0.60.1/osxphotos/debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/docs/docs.zip` & `osxphotos-0.60.1/osxphotos/docs/docs.zip`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 1459529 bytes, number of entries: 99
+Zip file size: 1467005 bytes, number of entries: 99
 -rw-r--r--  3.0 unx   331458 tx defN 23-Feb-12 16:23 docs/API_README.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_modules/
--rw-r--r--  3.0 unx    11779 tx defN 23-May-07 14:48 docs/_modules/index.html
+-rw-r--r--  3.0 unx    11779 tx defN 23-May-14 15:28 docs/_modules/index.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:15 docs/_modules/osxphotos/
 -rw-r--r--  3.0 unx   317579 tx defN 23-May-07 14:38 docs/_modules/osxphotos/photoexporter.html
 -rw-r--r--  3.0 unx   296439 tx defN 23-May-07 14:38 docs/_modules/osxphotos/phototemplate.html
--rw-r--r--  3.0 unx   200939 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/export_db.html
+-rw-r--r--  3.0 unx   201027 tx defN 23-May-14 15:28 docs/_modules/osxphotos/export_db.html
 -rw-r--r--  3.0 unx    14791 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/scoreinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:55 docs/_modules/osxphotos/photoinfo/
 -rw-r--r--  3.0 unx    14017 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
 -rw-r--r--  3.0 unx   284197 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/_photoinfo_export.html
 -rw-r--r--  3.0 unx   195566 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/photoinfo.html
 -rw-r--r--  3.0 unx    33978 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_searchinfo.html
 -rw-r--r--  3.0 unx    17959 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_scoreinfo.html
@@ -24,78 +24,78 @@
 -rw-r--r--  3.0 unx    92802 tx defN 23-May-07 14:38 docs/_modules/osxphotos/placeinfo.html
 -rw-r--r--  3.0 unx    21299 tx defN 22-May-06 00:24 docs/_modules/osxphotos/momentinfo.html
 -rw-r--r--  3.0 unx    82289 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/albuminfo.html
 -rw-r--r--  3.0 unx    78750 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/exiftool.html
 -rw-r--r--  3.0 unx    26012 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/debug.html
 -rw-r--r--  3.0 unx    59723 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/queryoptions.html
 -rw-r--r--  3.0 unx    80476 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/personinfo.html
--rw-r--r--  3.0 unx    61850 tx defN 23-May-07 14:48 docs/_modules/osxphotos/_constants.html
+-rw-r--r--  3.0 unx    61850 tx defN 23-May-14 15:28 docs/_modules/osxphotos/_constants.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-12 16:20 docs/_sources/
 -rw-r--r--  3.0 unx      198 tx defN 22-Apr-23 14:44 docs/_sources/cli.rst.txt
--rw-r--r--  3.0 unx    31854 tx defN 23-May-07 14:38 docs/_sources/template_help.rst.txt
+-rw-r--r--  3.0 unx    31854 tx defN 23-May-14 15:28 docs/_sources/template_help.rst.txt
 -rw-r--r--  3.0 unx    31240 tx defN 21-Apr-26 18:30 docs/_sources/tutorial.md.txt
 -rw-r--r--  3.0 unx       52 tx defN 21-Jan-24 17:13 docs/_sources/modules.rst.txt
 -rw-r--r--  3.0 unx    41238 tx defN 22-Aug-27 16:24 docs/_sources/tutorial.rst.txt
 -rw-r--r--  3.0 unx       93 tx defN 23-Feb-12 16:23 docs/_sources/reference.rst.txt
 -rw-r--r--  3.0 unx     7548 tx defN 22-Apr-23 18:28 docs/_sources/package_overview.rst.txt
 -rw-r--r--  3.0 unx      149 tx defN 22-Apr-21 04:29 docs/_sources/cli_export.rst.txt
 -rw-r--r--  3.0 unx   147706 tx defN 23-Feb-12 16:20 docs/_sources/API_README.rst.txt
 -rw-r--r--  3.0 unx      502 tx defN 23-Feb-12 16:24 docs/_sources/index.rst.txt
 -rw-r--r--  3.0 unx     4241 tx defN 22-May-01 15:46 docs/_sources/overview.rst.txt
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_static/
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/plus.png
 -rw-r--r--  3.0 unx     4712 tx defN 22-Nov-13 03:13 docs/_static/sphinx_highlight.js
 -rw-r--r--  3.0 unx    19530 tx defN 21-Jun-05 18:07 docs/_static/underscore.js
 -rw-r--r--  3.0 unx    11185 tx defN 21-Mar-22 05:50 docs/_static/alabaster.css
--rw-r--r--  3.0 unx      421 tx defN 23-May-07 14:48 docs/_static/documentation_options.js
+-rw-r--r--  3.0 unx      421 tx defN 23-May-14 15:28 docs/_static/documentation_options.js
 -rw-r--r--  3.0 unx    18215 tx defN 22-Nov-13 03:13 docs/_static/searchtools.js
 -rw-r--r--  3.0 unx     1266 tx defN 22-Nov-13 03:13 docs/_static/debug.css
 -rw-r--r--  3.0 unx      313 tx defN 22-Apr-21 05:12 docs/_static/check-solid.svg
 -rw-r--r--  3.0 unx     9031 tx defN 22-Apr-21 05:12 docs/_static/clipboard.min.js
 -rw-r--r--  3.0 unx      286 bx stor 21-Mar-14 19:14 docs/_static/file.png
 -rw-r--r--  3.0 unx     4418 tx defN 22-Nov-13 03:13 docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     8472 tx defN 23-May-07 14:48 docs/_static/copybutton.js
+-rw-r--r--  3.0 unx     8472 tx defN 23-May-14 15:28 docs/_static/copybutton.js
 -rw-r--r--  3.0 unx   287630 tx defN 21-Mar-14 19:14 docs/_static/jquery-3.5.1.js
 -rw-r--r--  3.0 unx       42 tx stor 21-Mar-14 19:14 docs/_static/custom.css
--rw-r--r--  3.0 unx     4758 tx defN 23-May-07 14:48 docs/_static/language_data.js
+-rw-r--r--  3.0 unx     4758 tx defN 23-May-14 15:28 docs/_static/language_data.js
 -rw-r--r--  3.0 unx      411 tx defN 22-Apr-21 05:12 docs/_static/copy-button.svg
 -rw-r--r--  3.0 unx     2698 tx defN 22-Dec-03 06:57 docs/_static/copybutton_funcs.js
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/minus.png
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-24 15:32 docs/_static/styles/
 -rw-r--r--  3.0 unx    72647 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css.map
 -rw-r--r--  3.0 unx     5529 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css
 -rw-r--r--  3.0 unx    48032 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css
 -rw-r--r--  3.0 unx     7809 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css.map
 -rw-r--r--  3.0 unx     6034 tx defN 22-Nov-13 03:13 docs/_static/skeleton.css
 -rw-r--r--  3.0 unx   288580 tx defN 22-Nov-13 03:13 docs/_static/jquery-3.6.0.js
--rw-r--r--  3.0 unx    14810 tx defN 23-May-07 14:48 docs/_static/basic.css
+-rw-r--r--  3.0 unx    14810 tx defN 23-May-14 15:28 docs/_static/basic.css
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:21 docs/_static/scripts/
 -rw-r--r--  3.0 unx      187 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js.LICENSE.txt
 -rw-r--r--  3.0 unx    28242 tx defN 22-Nov-13 03:13 docs/_static/scripts/furo.js.map
 -rw-r--r--  3.0 unx        0 bx stor 22-Apr-21 04:34 docs/_static/scripts/furo-extensions.js
 -rw-r--r--  3.0 unx     5265 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js
--rw-r--r--  3.0 unx    21072 tx defN 23-May-07 14:48 docs/_static/pygments.css
+-rw-r--r--  3.0 unx    21072 tx defN 23-May-14 15:28 docs/_static/pygments.css
 -rw-r--r--  3.0 unx     2060 tx defN 22-Dec-03 06:57 docs/_static/copybutton.css
 -rw-r--r--  3.0 unx     4472 tx defN 22-Nov-13 03:13 docs/_static/doctools.js
 -rw-r--r--  3.0 unx    67692 tx defN 21-Mar-14 19:14 docs/_static/underscore-1.12.0.js
 -rw-r--r--  3.0 unx    89501 tx defN 22-Nov-13 03:13 docs/_static/jquery.js
 -rw-r--r--  3.0 unx    68420 tx defN 21-Jun-05 18:07 docs/_static/underscore-1.13.1.js
--rw-r--r--  3.0 unx   414459 tx defN 23-May-07 14:38 docs/cli.html
+-rw-r--r--  3.0 unx   414459 tx defN 23-May-14 15:28 docs/cli.html
 -rw-r--r--  3.0 unx    85854 tx defN 22-Apr-21 04:30 docs/cli_export.html
--rw-r--r--  3.0 unx   243869 tx defN 23-May-07 14:48 docs/genindex.html
--rw-r--r--  3.0 unx   103976 tx defN 23-May-07 14:48 docs/index.html
+-rw-r--r--  3.0 unx   243869 tx defN 23-May-14 15:28 docs/genindex.html
+-rw-r--r--  3.0 unx   103976 tx defN 23-May-14 15:28 docs/index.html
 -rw-r--r--  3.0 unx     2984 tx defN 22-Apr-20 14:01 docs/modules.html
--rw-r--r--  3.0 unx     9396 bx stor 23-May-07 14:48 docs/objects.inv
+-rw-r--r--  3.0 unx     9396 bx stor 23-May-14 15:28 docs/objects.inv
 -rw-r--r--  3.0 unx   267506 bx defN 21-May-10 00:50 docs/osxphotos.pdf
--rw-r--r--  3.0 unx    26446 tx defN 23-May-07 14:38 docs/overview.html
--rw-r--r--  3.0 unx    32469 tx defN 23-May-07 14:38 docs/package_overview.html
--rw-r--r--  3.0 unx    10831 tx defN 23-May-07 14:48 docs/py-modindex.html
--rw-r--r--  3.0 unx   438606 tx defN 23-May-07 14:48 docs/reference.html
+-rw-r--r--  3.0 unx    26446 tx defN 23-May-14 15:28 docs/overview.html
+-rw-r--r--  3.0 unx    32469 tx defN 23-May-14 15:28 docs/package_overview.html
+-rw-r--r--  3.0 unx    10831 tx defN 23-May-14 15:28 docs/py-modindex.html
+-rw-r--r--  3.0 unx   438606 tx defN 23-May-14 15:28 docs/reference.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:53 docs/screencast/
 -rw-r--r--  3.0 unx     8007 tx defN 21-Jan-24 17:13 docs/screencast/terminalizer-demo.yml
 -rw-r--r--  3.0 unx    77927 bx defN 21-Jan-24 17:13 docs/screencast/osx-screenshot.png
 -rw-r--r--  3.0 unx   224316 bx defN 21-Jan-24 17:13 docs/screencast/demo.gif
--rw-r--r--  3.0 unx    10567 tx defN 23-May-07 14:48 docs/search.html
--rw-r--r--  3.0 unx   146510 tx defN 23-May-07 14:48 docs/searchindex.js
--rw-r--r--  3.0 unx    64566 tx defN 23-May-07 14:48 docs/template_help.html
--rw-r--r--  3.0 unx    84995 tx defN 23-May-07 14:48 docs/tutorial.html
-99 files, 6833436 bytes uncompressed, 1440797 bytes compressed:  78.9%
+-rw-r--r--  3.0 unx    10567 tx defN 23-May-14 15:28 docs/search.html
+-rw-r--r--  3.0 unx   215976 tx defN 23-May-14 15:28 docs/searchindex.js
+-rw-r--r--  3.0 unx    64566 tx defN 23-May-14 15:28 docs/template_help.html
+-rw-r--r--  3.0 unx    84995 tx defN 23-May-14 15:28 docs/tutorial.html
+99 files, 6902990 bytes uncompressed, 1448273 bytes compressed:  79.0%
```

#### docs/_modules/index.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>Overview: module code - osxphotos 0.60.0 documentation</title>
+        <title>Overview: module code - osxphotos 0.60.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="../index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/export_db.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.export_db - osxphotos 0.59.2 documentation</title>
+        <title>osxphotos.export_db - osxphotos 0.60.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1114,40 +1114,43 @@
 
     <span class="nd">@retry</span><span class="p">(</span><span class="n">stop</span><span class="o">=</span><span class="n">stop_after_attempt</span><span class="p">(</span><span class="n">MAX_RETRY_ATTEMPTS</span><span class="p">))</span>
     <span class="k">def</span> <span class="nf">_open_export_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">dbfile</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>  <span class="c1"># sourcery skip: raise-specific-error</span>
         <span class="sd">&quot;&quot;&quot;open export database and return a db connection</span>
 <span class="sd">        returns: connection to the database</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">dbfile</span><span class="p">):</span>
-            <span class="n">conn</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_db_connection</span><span class="p">()</span>
-            <span class="k">if</span> <span class="ow">not</span> <span class="n">conn</span><span class="p">:</span>
+            <span class="c1"># database doesn&#39;t exist so create it in-memory</span>
+            <span class="n">src</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_db_connection</span><span class="p">()</span>
+            <span class="k">if</span> <span class="ow">not</span> <span class="n">src</span><span class="p">:</span>
                 <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="s2">&quot;Error getting connection to in-memory database&quot;</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_create_or_migrate_db_tables</span><span class="p">(</span><span class="n">conn</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_create_or_migrate_db_tables</span><span class="p">(</span><span class="n">src</span><span class="p">)</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">was_created</span> <span class="o">=</span> <span class="kc">True</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">was_upgraded</span> <span class="o">=</span> <span class="p">()</span>
-        <span class="k">else</span><span class="p">:</span>
-            <span class="n">conn</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span><span class="n">dbfile</span><span class="p">,</span> <span class="n">check_same_thread</span><span class="o">=</span><span class="n">SQLITE_CHECK_SAME_THREAD</span><span class="p">)</span>
-            <span class="n">dbdump</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dump_db</span><span class="p">(</span><span class="n">conn</span><span class="p">)</span>
-            <span class="n">conn</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">version</span> <span class="o">=</span> <span class="n">OSXPHOTOS_EXPORTDB_VERSION</span>
+            <span class="k">return</span> <span class="n">src</span>
 
-            <span class="c1"># Create a database in memory and import from the dump</span>
-            <span class="n">conn</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span>
-                <span class="s2">&quot;:memory:&quot;</span><span class="p">,</span> <span class="n">check_same_thread</span><span class="o">=</span><span class="n">SQLITE_CHECK_SAME_THREAD</span>
-            <span class="p">)</span>
-            <span class="n">conn</span><span class="o">.</span><span class="n">cursor</span><span class="p">()</span><span class="o">.</span><span class="n">executescript</span><span class="p">(</span><span class="n">dbdump</span><span class="o">.</span><span class="n">read</span><span class="p">())</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">was_created</span> <span class="o">=</span> <span class="kc">False</span>
-            <span class="n">version_info</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_database_version</span><span class="p">(</span><span class="n">conn</span><span class="p">)</span>
-            <span class="k">if</span> <span class="n">version_info</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">&lt;</span> <span class="n">OSXPHOTOS_EXPORTDB_VERSION</span><span class="p">:</span>
-                <span class="bp">self</span><span class="o">.</span><span class="n">_create_or_migrate_db_tables</span><span class="p">(</span><span class="n">conn</span><span class="p">)</span>
-                <span class="bp">self</span><span class="o">.</span><span class="n">was_upgraded</span> <span class="o">=</span> <span class="p">(</span><span class="n">version_info</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">OSXPHOTOS_EXPORTDB_VERSION</span><span class="p">)</span>
-            <span class="k">else</span><span class="p">:</span>
-                <span class="bp">self</span><span class="o">.</span><span class="n">was_upgraded</span> <span class="o">=</span> <span class="p">()</span>
+        <span class="c1"># database exists so copy it to memory</span>
+        <span class="n">src</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span><span class="n">dbfile</span><span class="p">,</span> <span class="n">check_same_thread</span><span class="o">=</span><span class="n">SQLITE_CHECK_SAME_THREAD</span><span class="p">)</span>
+
+        <span class="c1"># Create a database in memory by backing up the on-disk database</span>
+        <span class="n">dst</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span><span class="s2">&quot;:memory:&quot;</span><span class="p">,</span> <span class="n">check_same_thread</span><span class="o">=</span><span class="n">SQLITE_CHECK_SAME_THREAD</span><span class="p">)</span>
+        <span class="k">with</span> <span class="n">dst</span><span class="p">:</span>
+            <span class="n">src</span><span class="o">.</span><span class="n">backup</span><span class="p">(</span><span class="n">dst</span><span class="p">,</span> <span class="n">pages</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>
+        <span class="n">src</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+
+        <span class="bp">self</span><span class="o">.</span><span class="n">was_created</span> <span class="o">=</span> <span class="kc">False</span>
+        <span class="n">version_info</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_database_version</span><span class="p">(</span><span class="n">dst</span><span class="p">)</span>
+        <span class="k">if</span> <span class="n">version_info</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">&lt;</span> <span class="n">OSXPHOTOS_EXPORTDB_VERSION</span><span class="p">:</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_create_or_migrate_db_tables</span><span class="p">(</span><span class="n">dst</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">was_upgraded</span> <span class="o">=</span> <span class="p">(</span><span class="n">version_info</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">OSXPHOTOS_EXPORTDB_VERSION</span><span class="p">)</span>
+        <span class="k">else</span><span class="p">:</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">was_upgraded</span> <span class="o">=</span> <span class="p">()</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">version</span> <span class="o">=</span> <span class="n">OSXPHOTOS_EXPORTDB_VERSION</span>
 
-        <span class="k">return</span> <span class="n">conn</span>
+        <span class="k">return</span> <span class="n">dst</span>
 
     <span class="k">def</span> <span class="nf">_get_db_connection</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;return db connection to in memory database&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span><span class="s2">&quot;:memory:&quot;</span><span class="p">,</span> <span class="n">check_same_thread</span><span class="o">=</span><span class="n">SQLITE_CHECK_SAME_THREAD</span><span class="p">)</span>
 
     <span class="k">def</span> <span class="nf">_dump_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">conn</span><span class="p">:</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">Connection</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">StringIO</span><span class="p">:</span>
         <span class="sd">&quot;&quot;&quot;dump sqlite db to a string buffer&quot;&quot;&quot;</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.1_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.60.1_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -1037,43 +1037,46 @@
     @retry(stop=stop_after_attempt(MAX_RETRY_ATTEMPTS))
     def _open_export_db(self, dbfile: str):  # sourcery skip: raise-specific-
 error
         """open export database and return a db connection
         returns: connection to the database
         """
         if not os.path.isfile(dbfile):
-            conn = self._get_db_connection()
-            if not conn:
+            # database doesn't exist so create it in-memory
+            src = self._get_db_connection()
+            if not src:
                 raise Exception("Error getting connection to in-memory
 database")
-            self._create_or_migrate_db_tables(conn)
+            self._create_or_migrate_db_tables(src)
             self.was_created = True
             self.was_upgraded = ()
-        else:
-            conn = sqlite3.connect(dbfile,
+            self.version = OSXPHOTOS_EXPORTDB_VERSION
+            return src
+
+        # database exists so copy it to memory
+        src = sqlite3.connect(dbfile,
 check_same_thread=SQLITE_CHECK_SAME_THREAD)
-            dbdump = self._dump_db(conn)
-            conn.close()
 
-            # Create a database in memory and import from the dump
-            conn = sqlite3.connect(
-                ":memory:", check_same_thread=SQLITE_CHECK_SAME_THREAD
-            )
-            conn.cursor().executescript(dbdump.read())
-            self.was_created = False
-            version_info = self._get_database_version(conn)
-            if version_info[1] < OSXPHOTOS_EXPORTDB_VERSION:
-                self._create_or_migrate_db_tables(conn)
-                self.was_upgraded = (version_info[1],
-OSXPHOTOS_EXPORTDB_VERSION)
-            else:
-                self.was_upgraded = ()
+        # Create a database in memory by backing up the on-disk database
+        dst = sqlite3.connect(":memory:",
+check_same_thread=SQLITE_CHECK_SAME_THREAD)
+        with dst:
+            src.backup(dst, pages=1)
+        src.close()
+
+        self.was_created = False
+        version_info = self._get_database_version(dst)
+        if version_info[1] < OSXPHOTOS_EXPORTDB_VERSION:
+            self._create_or_migrate_db_tables(dst)
+            self.was_upgraded = (version_info[1], OSXPHOTOS_EXPORTDB_VERSION)
+        else:
+            self.was_upgraded = ()
         self.version = OSXPHOTOS_EXPORTDB_VERSION
 
-        return conn
+        return dst
 
     def _get_db_connection(self):
         """return db connection to in memory database"""
         return sqlite3.connect(":memory:",
 check_same_thread=SQLITE_CHECK_SAME_THREAD)
 
     def _dump_db(self, conn: sqlite3.Connection) -> StringIO:
```

#### docs/_modules/osxphotos/_constants.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos._constants - osxphotos 0.60.0 documentation</title>
+        <title>osxphotos._constants - osxphotos 0.60.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_sources/template_help.rst.txt

```diff
@@ -357,15 +357,15 @@
    * - {cr}
      - A carriage return: '\r'
    * - {crlf}
      - A carriage return + line feed: '\r\n'
    * - {tab}
      - :A tab: '\t'
    * - {osxphotos_version}
-     - The osxphotos version, e.g. '0.60.0'
+     - The osxphotos version, e.g. '0.60.1'
    * - {osxphotos_cmd_line}
      - The full command line used to run osxphotos
    * - {album}
      - Album(s) photo is contained in
    * - {folder_album}
      - Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder
    * - {project}
```

#### docs/_static/documentation_options.js

##### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 var DOCUMENTATION_OPTIONS = {
     URL_ROOT: document.getElementById("documentation_options").getAttribute('data-url_root'),
-    VERSION: '0.60.0',
+    VERSION: '0.60.1',
     LANGUAGE: 'en',
     COLLAPSE_INDEX: false,
     BUILDER: 'html',
     FILE_SUFFIX: '.html',
     LINK_SUFFIX: '.html',
     HAS_SOURCE: true,
     SOURCELINK_SUFFIX: '.txt',
```

#### docs/cli.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Template System" href="template_help.html" /><link rel="prev" title="OSXPhotos Tutorial" href="tutorial.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.0 documentation</title>
+        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/genindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.0 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.1 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/index.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos 0.60.0 documentation</title>
+        <title>osxphotos 0.60.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="#"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="#"><div class="brand">osxphotos 0.60.1 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="#">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Tutorial" href="tutorial.html" /><link rel="prev" title="Welcome to OSXPhotos’s documentation!" href="index.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos - osxphotos 0.60.0 documentation</title>
+        <title>OSXPhotos - osxphotos 0.60.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/package_overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Reference" href="reference.html" /><link rel="prev" title="OSXPhotos Template System" href="template_help.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Package Overview - osxphotos 0.60.0 documentation</title>
+        <title>OSXPhotos Python Package Overview - osxphotos 0.60.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/py-modindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.0 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.1 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/reference.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="OSXPhotos Python Package Overview" href="package_overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Reference - osxphotos 0.60.0 documentation</title>
+        <title>OSXPhotos Python Reference - osxphotos 0.60.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/search.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.0 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.1 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
 
@@ -117,15 +117,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -140,15 +140,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="#" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/searchindex.js

##### js-beautify {}

```diff
@@ -4082,14 +4082,2028 @@
             [6, "color-themes"]
         ],
         "Conclusion": [
             [6, "conclusion"]
         ]
     },
     "indexentries": {
+        "--add-exported-to-album": [
+            [0, "cmdoption-osxphotos-export-add-exported-to-album"]
+        ],
+        "--add-missing-to-album": [
+            [0, "cmdoption-osxphotos-export-add-missing-to-album"]
+        ],
+        "--add-skipped-to-album": [
+            [0, "cmdoption-osxphotos-export-add-skipped-to-album"]
+        ],
+        "--add-to-album": [
+            [0, "cmdoption-osxphotos-query-add-to-album"],
+            [0, "cmdoption-osxphotos-timewarp-a"]
+        ],
+        "--added-after": [
+            [0, "cmdoption-osxphotos-add-locations-added-after"],
+            [0, "cmdoption-osxphotos-export-added-after"],
+            [0, "cmdoption-osxphotos-query-added-after"],
+            [0, "cmdoption-osxphotos-repl-added-after"],
+            [0, "cmdoption-osxphotos-sync-added-after"]
+        ],
+        "--added-before": [
+            [0, "cmdoption-osxphotos-add-locations-added-before"],
+            [0, "cmdoption-osxphotos-export-added-before"],
+            [0, "cmdoption-osxphotos-query-added-before"],
+            [0, "cmdoption-osxphotos-repl-added-before"],
+            [0, "cmdoption-osxphotos-sync-added-before"]
+        ],
+        "--added-in-last": [
+            [0, "cmdoption-osxphotos-add-locations-added-in-last"],
+            [0, "cmdoption-osxphotos-export-added-in-last"],
+            [0, "cmdoption-osxphotos-query-added-in-last"],
+            [0, "cmdoption-osxphotos-repl-added-in-last"],
+            [0, "cmdoption-osxphotos-sync-added-in-last"]
+        ],
+        "--album": [
+            [0, "cmdoption-osxphotos-add-locations-album"],
+            [0, "cmdoption-osxphotos-export-album"],
+            [0, "cmdoption-osxphotos-import-a"],
+            [0, "cmdoption-osxphotos-query-album"],
+            [0, "cmdoption-osxphotos-repl-album"],
+            [0, "cmdoption-osxphotos-sync-album"]
+        ],
+        "--album-keyword": [
+            [0, "cmdoption-osxphotos-exiftool-album-keyword"],
+            [0, "cmdoption-osxphotos-export-album-keyword"]
+        ],
+        "--alt-copy": [
+            [0, "cmdoption-osxphotos-export-alt-copy"]
+        ],
+        "--append": [
+            [0, "cmdoption-osxphotos-exiftool-append"],
+            [0, "cmdoption-osxphotos-export-append"],
+            [0, "cmdoption-osxphotos-exportdb-append"],
+            [0, "cmdoption-osxphotos-import-append"],
+            [0, "cmdoption-osxphotos-sync-A"]
+        ],
+        "--burst": [
+            [0, "cmdoption-osxphotos-add-locations-burst"],
+            [0, "cmdoption-osxphotos-export-burst"],
+            [0, "cmdoption-osxphotos-query-burst"],
+            [0, "cmdoption-osxphotos-repl-burst"],
+            [0, "cmdoption-osxphotos-sync-burst"]
+        ],
+        "--check-signatures": [
+            [0, "cmdoption-osxphotos-exportdb-check-signatures"]
+        ],
+        "--check-templates": [
+            [0, "cmdoption-osxphotos-import-check-templates"]
+        ],
+        "--cleanup": [
+            [0, "cmdoption-osxphotos-export-cleanup"]
+        ],
+        "--clear-location": [
+            [0, "cmdoption-osxphotos-import-L"]
+        ],
+        "--clear-metadata": [
+            [0, "cmdoption-osxphotos-import-C"]
+        ],
+        "--clone": [
+            [0, "cmdoption-osxphotos-theme-clone"]
+        ],
+        "--cloudasset": [
+            [0, "cmdoption-osxphotos-add-locations-cloudasset"],
+            [0, "cmdoption-osxphotos-export-cloudasset"],
+            [0, "cmdoption-osxphotos-query-cloudasset"],
+            [0, "cmdoption-osxphotos-repl-cloudasset"],
+            [0, "cmdoption-osxphotos-sync-cloudasset"]
+        ],
+        "--compare-exif": [
+            [0, "cmdoption-osxphotos-timewarp-c"]
+        ],
+        "--config": [
+            [0, "cmdoption-osxphotos-theme-config"]
+        ],
+        "--config-only": [
+            [0, "cmdoption-osxphotos-export-config-only"]
+        ],
+        "--convert-to-jpeg": [
+            [0, "cmdoption-osxphotos-export-convert-to-jpeg"]
+        ],
+        "--current-name": [
+            [0, "cmdoption-osxphotos-export-current-name"]
+        ],
+        "--date": [
+            [0, "cmdoption-osxphotos-timewarp-d"]
+        ],
+        "--date-added": [
+            [0, "cmdoption-osxphotos-timewarp-date-added"]
+        ],
+        "--date-added-from-photo": [
+            [0, "cmdoption-osxphotos-timewarp-date-added-from-photo"]
+        ],
+        "--date-delta": [
+            [0, "cmdoption-osxphotos-timewarp-D"]
+        ],
+        "--db": [
+            [0, "cmdoption-osxphotos-albums-library"],
+            [0, "cmdoption-osxphotos-batch-edit-library"],
+            [0, "cmdoption-osxphotos-diff-library"],
+            [0, "cmdoption-osxphotos-dump-library"],
+            [0, "cmdoption-osxphotos-exiftool-library"],
+            [0, "cmdoption-osxphotos-export-library"],
+            [0, "cmdoption-osxphotos-info-library"],
+            [0, "cmdoption-osxphotos-inspect-library"],
+            [0, "cmdoption-osxphotos-keywords-library"],
+            [0, "cmdoption-osxphotos-labels-library"],
+            [0, "cmdoption-osxphotos-library"],
+            [0, "cmdoption-osxphotos-orphans-library"],
+            [0, "cmdoption-osxphotos-persons-library"],
+            [0, "cmdoption-osxphotos-places-library"],
+            [0, "cmdoption-osxphotos-query-library"],
+            [0, "cmdoption-osxphotos-repl-library"],
+            [0, "cmdoption-osxphotos-show-library"],
+            [0, "cmdoption-osxphotos-snap-library"],
+            [0, "cmdoption-osxphotos-sync-library"]
+        ],
+        "--db-config": [
+            [0, "cmdoption-osxphotos-exiftool-db-config"]
+        ],
+        "--default": [
+            [0, "cmdoption-osxphotos-theme-default"]
+        ],
+        "--delete": [
+            [0, "cmdoption-osxphotos-theme-delete"]
+        ],
+        "--delete-file": [
+            [0, "cmdoption-osxphotos-exportdb-delete-file"]
+        ],
+        "--delete-uuid": [
+            [0, "cmdoption-osxphotos-exportdb-delete-uuid"]
+        ],
+        "--deleted": [
+            [0, "cmdoption-osxphotos-dump-deleted"],
+            [0, "cmdoption-osxphotos-export-deleted"],
+            [0, "cmdoption-osxphotos-query-deleted"],
+            [0, "cmdoption-osxphotos-repl-deleted"]
+        ],
+        "--deleted-only": [
+            [0, "cmdoption-osxphotos-dump-deleted-only"],
+            [0, "cmdoption-osxphotos-export-deleted-only"],
+            [0, "cmdoption-osxphotos-query-deleted-only"],
+            [0, "cmdoption-osxphotos-repl-deleted-only"]
+        ],
+        "--description": [
+            [0, "cmdoption-osxphotos-add-locations-description"],
+            [0, "cmdoption-osxphotos-batch-edit-description"],
+            [0, "cmdoption-osxphotos-export-description"],
+            [0, "cmdoption-osxphotos-import-d"],
+            [0, "cmdoption-osxphotos-query-description"],
+            [0, "cmdoption-osxphotos-repl-description"],
+            [0, "cmdoption-osxphotos-sync-description"]
+        ],
+        "--description-template": [
+            [0, "cmdoption-osxphotos-exiftool-description-template"],
+            [0, "cmdoption-osxphotos-export-description-template"]
+        ],
+        "--detect-text": [
+            [0, "cmdoption-osxphotos-inspect-t"]
+        ],
+        "--directory": [
+            [0, "cmdoption-osxphotos-export-directory"]
+        ],
+        "--download-missing": [
+            [0, "cmdoption-osxphotos-export-download-missing"]
+        ],
+        "--dry-run": [
+            [0, "cmdoption-osxphotos-add-locations-dry-run"],
+            [0, "cmdoption-osxphotos-batch-edit-dry-run"],
+            [0, "cmdoption-osxphotos-exiftool-dry-run"],
+            [0, "cmdoption-osxphotos-export-dry-run"],
+            [0, "cmdoption-osxphotos-exportdb-dry-run"],
+            [0, "cmdoption-osxphotos-sync-dry-run"]
+        ],
+        "--dup-check": [
+            [0, "cmdoption-osxphotos-import-D"]
+        ],
+        "--duplicate": [
+            [0, "cmdoption-osxphotos-add-locations-duplicate"],
+            [0, "cmdoption-osxphotos-export-duplicate"],
+            [0, "cmdoption-osxphotos-query-duplicate"],
+            [0, "cmdoption-osxphotos-repl-duplicate"],
+            [0, "cmdoption-osxphotos-sync-duplicate"]
+        ],
+        "--edit": [
+            [0, "cmdoption-osxphotos-theme-edit"]
+        ],
+        "--edited": [
+            [0, "cmdoption-osxphotos-add-locations-edited"],
+            [0, "cmdoption-osxphotos-export-edited"],
+            [0, "cmdoption-osxphotos-query-edited"],
+            [0, "cmdoption-osxphotos-repl-edited"],
+            [0, "cmdoption-osxphotos-sync-edited"]
+        ],
+        "--edited-suffix": [
+            [0, "cmdoption-osxphotos-export-edited-suffix"]
+        ],
+        "--emacs": [
+            [0, "cmdoption-osxphotos-repl-emacs"]
+        ],
+        "--errors": [
+            [0, "cmdoption-osxphotos-exportdb-errors"]
+        ],
+        "--exif": [
+            [0, "cmdoption-osxphotos-add-locations-exif"],
+            [0, "cmdoption-osxphotos-export-exif"],
+            [0, "cmdoption-osxphotos-query-exif"],
+            [0, "cmdoption-osxphotos-repl-exif"],
+            [0, "cmdoption-osxphotos-sync-exif"]
+        ],
+        "--exiftool": [
+            [0, "cmdoption-osxphotos-export-exiftool"],
+            [0, "cmdoption-osxphotos-import-e"]
+        ],
+        "--exiftool-merge-keywords": [
+            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-keywords"],
+            [0, "cmdoption-osxphotos-export-exiftool-merge-keywords"]
+        ],
+        "--exiftool-merge-persons": [
+            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-persons"],
+            [0, "cmdoption-osxphotos-export-exiftool-merge-persons"]
+        ],
+        "--exiftool-option": [
+            [0, "cmdoption-osxphotos-exiftool-exiftool-option"],
+            [0, "cmdoption-osxphotos-export-exiftool-option"]
+        ],
+        "--exiftool-path": [
+            [0, "cmdoption-osxphotos-exiftool-exiftool-path"],
+            [0, "cmdoption-osxphotos-export-exiftool-path"],
+            [0, "cmdoption-osxphotos-import-0"],
+            [0, "cmdoption-osxphotos-timewarp-e"]
+        ],
+        "--export": [
+            [0, "cmdoption-osxphotos-orphans-export"],
+            [0, "cmdoption-osxphotos-sync-e"]
+        ],
+        "--export-as-hardlink": [
+            [0, "cmdoption-osxphotos-export-export-as-hardlink"]
+        ],
+        "--export-by-date": [
+            [0, "cmdoption-osxphotos-export-export-by-date"]
+        ],
+        "--export-dir": [
+            [0, "cmdoption-osxphotos-exportdb-export-dir"]
+        ],
+        "--exportdb": [
+            [0, "cmdoption-osxphotos-exiftool-exportdb"],
+            [0, "cmdoption-osxphotos-export-exportdb"]
+        ],
+        "--external-edit": [
+            [0, "cmdoption-osxphotos-add-locations-external-edit"],
+            [0, "cmdoption-osxphotos-export-external-edit"],
+            [0, "cmdoption-osxphotos-query-external-edit"],
+            [0, "cmdoption-osxphotos-repl-external-edit"],
+            [0, "cmdoption-osxphotos-sync-external-edit"]
+        ],
+        "--favorite": [
+            [0, "cmdoption-osxphotos-add-locations-favorite"],
+            [0, "cmdoption-osxphotos-export-favorite"],
+            [0, "cmdoption-osxphotos-query-favorite"],
+            [0, "cmdoption-osxphotos-repl-favorite"],
+            [0, "cmdoption-osxphotos-sync-favorite"]
+        ],
+        "--favorite-rating": [
+            [0, "cmdoption-osxphotos-export-favorite-rating"]
+        ],
+        "--field": [
+            [0, "cmdoption-osxphotos-dump-f"],
+            [0, "cmdoption-osxphotos-query-f"]
+        ],
+        "--filename": [
+            [0, "cmdoption-osxphotos-export-filename"],
+            [0, "cmdoption-osxphotos-uuid-f"]
+        ],
+        "--finder-tag-keywords": [
+            [0, "cmdoption-osxphotos-export-finder-tag-keywords"]
+        ],
+        "--finder-tag-template": [
+            [0, "cmdoption-osxphotos-export-finder-tag-template"]
+        ],
+        "--folder": [
+            [0, "cmdoption-osxphotos-add-locations-folder"],
+            [0, "cmdoption-osxphotos-export-folder"],
+            [0, "cmdoption-osxphotos-query-folder"],
+            [0, "cmdoption-osxphotos-repl-folder"],
+            [0, "cmdoption-osxphotos-sync-folder"]
+        ],
+        "--force": [
+            [0, "cmdoption-osxphotos-timewarp-force"]
+        ],
+        "--force-update": [
+            [0, "cmdoption-osxphotos-export-force-update"]
+        ],
+        "--from-date": [
+            [0, "cmdoption-osxphotos-add-locations-from-date"],
+            [0, "cmdoption-osxphotos-export-from-date"],
+            [0, "cmdoption-osxphotos-query-from-date"],
+            [0, "cmdoption-osxphotos-repl-from-date"],
+            [0, "cmdoption-osxphotos-sync-from-date"]
+        ],
+        "--from-time": [
+            [0, "cmdoption-osxphotos-add-locations-from-time"],
+            [0, "cmdoption-osxphotos-export-from-time"],
+            [0, "cmdoption-osxphotos-query-from-time"],
+            [0, "cmdoption-osxphotos-repl-from-time"],
+            [0, "cmdoption-osxphotos-sync-from-time"]
+        ],
+        "--function": [
+            [0, "cmdoption-osxphotos-timewarp-F"]
+        ],
+        "--glob": [
+            [0, "cmdoption-osxphotos-import-g"]
+        ],
+        "--has-comment": [
+            [0, "cmdoption-osxphotos-add-locations-has-comment"],
+            [0, "cmdoption-osxphotos-export-has-comment"],
+            [0, "cmdoption-osxphotos-query-has-comment"],
+            [0, "cmdoption-osxphotos-repl-has-comment"],
+            [0, "cmdoption-osxphotos-sync-has-comment"]
+        ],
+        "--has-likes": [
+            [0, "cmdoption-osxphotos-add-locations-has-likes"],
+            [0, "cmdoption-osxphotos-export-has-likes"],
+            [0, "cmdoption-osxphotos-query-has-likes"],
+            [0, "cmdoption-osxphotos-repl-has-likes"],
+            [0, "cmdoption-osxphotos-sync-has-likes"]
+        ],
+        "--has-raw": [
+            [0, "cmdoption-osxphotos-add-locations-has-raw"],
+            [0, "cmdoption-osxphotos-export-has-raw"],
+            [0, "cmdoption-osxphotos-query-has-raw"],
+            [0, "cmdoption-osxphotos-repl-has-raw"],
+            [0, "cmdoption-osxphotos-sync-has-raw"]
+        ],
+        "--hdr": [
+            [0, "cmdoption-osxphotos-add-locations-hdr"],
+            [0, "cmdoption-osxphotos-export-hdr"],
+            [0, "cmdoption-osxphotos-query-hdr"],
+            [0, "cmdoption-osxphotos-repl-hdr"],
+            [0, "cmdoption-osxphotos-sync-hdr"]
+        ],
+        "--help": [
+            [0, "cmdoption-osxphotos-run-h"]
+        ],
+        "--hidden": [
+            [0, "cmdoption-osxphotos-add-locations-hidden"],
+            [0, "cmdoption-osxphotos-export-hidden"],
+            [0, "cmdoption-osxphotos-query-hidden"],
+            [0, "cmdoption-osxphotos-repl-hidden"],
+            [0, "cmdoption-osxphotos-sync-hidden"]
+        ],
+        "--ignore-case": [
+            [0, "cmdoption-osxphotos-add-locations-i"],
+            [0, "cmdoption-osxphotos-export-i"],
+            [0, "cmdoption-osxphotos-query-i"],
+            [0, "cmdoption-osxphotos-repl-i"],
+            [0, "cmdoption-osxphotos-sync-0"]
+        ],
+        "--ignore-date-modified": [
+            [0, "cmdoption-osxphotos-exiftool-ignore-date-modified"],
+            [0, "cmdoption-osxphotos-export-ignore-date-modified"]
+        ],
+        "--ignore-signature": [
+            [0, "cmdoption-osxphotos-export-ignore-signature"]
+        ],
+        "--import": [
+            [0, "cmdoption-osxphotos-sync-i"]
+        ],
+        "--in-album": [
+            [0, "cmdoption-osxphotos-add-locations-in-album"],
+            [0, "cmdoption-osxphotos-export-in-album"],
+            [0, "cmdoption-osxphotos-query-in-album"],
+            [0, "cmdoption-osxphotos-repl-in-album"],
+            [0, "cmdoption-osxphotos-sync-in-album"]
+        ],
+        "--incloud": [
+            [0, "cmdoption-osxphotos-add-locations-incloud"],
+            [0, "cmdoption-osxphotos-export-incloud"],
+            [0, "cmdoption-osxphotos-query-incloud"],
+            [0, "cmdoption-osxphotos-repl-incloud"],
+            [0, "cmdoption-osxphotos-sync-incloud"]
+        ],
+        "--info": [
+            [0, "cmdoption-osxphotos-exportdb-info"]
+        ],
+        "--inspect": [
+            [0, "cmdoption-osxphotos-timewarp-i"]
+        ],
+        "--is-reference": [
+            [0, "cmdoption-osxphotos-add-locations-is-reference"],
+            [0, "cmdoption-osxphotos-export-is-reference"],
+            [0, "cmdoption-osxphotos-query-is-reference"],
+            [0, "cmdoption-osxphotos-repl-is-reference"],
+            [0, "cmdoption-osxphotos-sync-is-reference"]
+        ],
+        "--jpeg-ext": [
+            [0, "cmdoption-osxphotos-export-jpeg-ext"]
+        ],
+        "--jpeg-quality": [
+            [0, "cmdoption-osxphotos-export-jpeg-quality"]
+        ],
+        "--json": [
+            [0, "cmdoption-osxphotos-albums-json"],
+            [0, "cmdoption-osxphotos-dump-json"],
+            [0, "cmdoption-osxphotos-info-json"],
+            [0, "cmdoption-osxphotos-json"],
+            [0, "cmdoption-osxphotos-keywords-json"],
+            [0, "cmdoption-osxphotos-labels-json"],
+            [0, "cmdoption-osxphotos-list-json"],
+            [0, "cmdoption-osxphotos-persons-json"],
+            [0, "cmdoption-osxphotos-places-json"],
+            [0, "cmdoption-osxphotos-query-json"]
+        ],
+        "--keep": [
+            [0, "cmdoption-osxphotos-export-keep"]
+        ],
+        "--keyword": [
+            [0, "cmdoption-osxphotos-add-locations-keyword"],
+            [0, "cmdoption-osxphotos-batch-edit-keyword"],
+            [0, "cmdoption-osxphotos-export-keyword"],
+            [0, "cmdoption-osxphotos-import-k"],
+            [0, "cmdoption-osxphotos-query-keyword"],
+            [0, "cmdoption-osxphotos-repl-keyword"],
+            [0, "cmdoption-osxphotos-sync-keyword"]
+        ],
+        "--keyword-template": [
+            [0, "cmdoption-osxphotos-exiftool-keyword-template"],
+            [0, "cmdoption-osxphotos-export-keyword-template"]
+        ],
+        "--label": [
+            [0, "cmdoption-osxphotos-add-locations-label"],
+            [0, "cmdoption-osxphotos-export-label"],
+            [0, "cmdoption-osxphotos-query-label"],
+            [0, "cmdoption-osxphotos-repl-label"],
+            [0, "cmdoption-osxphotos-sync-label"]
+        ],
+        "--last-errors": [
+            [0, "cmdoption-osxphotos-exportdb-last-errors"]
+        ],
+        "--last-run": [
+            [0, "cmdoption-osxphotos-exportdb-last-run"]
+        ],
+        "--library": [
+            [0, "cmdoption-osxphotos-albums-library"],
+            [0, "cmdoption-osxphotos-batch-edit-library"],
+            [0, "cmdoption-osxphotos-diff-library"],
+            [0, "cmdoption-osxphotos-dump-library"],
+            [0, "cmdoption-osxphotos-exiftool-library"],
+            [0, "cmdoption-osxphotos-export-library"],
+            [0, "cmdoption-osxphotos-info-library"],
+            [0, "cmdoption-osxphotos-inspect-library"],
+            [0, "cmdoption-osxphotos-keywords-library"],
+            [0, "cmdoption-osxphotos-labels-library"],
+            [0, "cmdoption-osxphotos-library"],
+            [0, "cmdoption-osxphotos-orphans-library"],
+            [0, "cmdoption-osxphotos-persons-library"],
+            [0, "cmdoption-osxphotos-places-library"],
+            [0, "cmdoption-osxphotos-query-library"],
+            [0, "cmdoption-osxphotos-repl-library"],
+            [0, "cmdoption-osxphotos-show-library"],
+            [0, "cmdoption-osxphotos-snap-library"],
+            [0, "cmdoption-osxphotos-sync-library"],
+            [0, "cmdoption-osxphotos-timewarp-L"]
+        ],
+        "--limit": [
+            [0, "cmdoption-osxphotos-export-limit"]
+        ],
+        "--list": [
+            [0, "cmdoption-osxphotos-theme-list"]
+        ],
+        "--live": [
+            [0, "cmdoption-osxphotos-add-locations-live"],
+            [0, "cmdoption-osxphotos-export-live"],
+            [0, "cmdoption-osxphotos-query-live"],
+            [0, "cmdoption-osxphotos-repl-live"],
+            [0, "cmdoption-osxphotos-sync-live"]
+        ],
+        "--load-config": [
+            [0, "cmdoption-osxphotos-exiftool-load-config"],
+            [0, "cmdoption-osxphotos-export-load-config"]
+        ],
+        "--location": [
+            [0, "cmdoption-osxphotos-add-locations-location"],
+            [0, "cmdoption-osxphotos-batch-edit-location"],
+            [0, "cmdoption-osxphotos-export-location"],
+            [0, "cmdoption-osxphotos-import-l"],
+            [0, "cmdoption-osxphotos-query-location"],
+            [0, "cmdoption-osxphotos-repl-location"],
+            [0, "cmdoption-osxphotos-sync-location"]
+        ],
+        "--match-time": [
+            [0, "cmdoption-osxphotos-timewarp-0"]
+        ],
+        "--max-size": [
+            [0, "cmdoption-osxphotos-add-locations-max-size"],
+            [0, "cmdoption-osxphotos-export-max-size"],
+            [0, "cmdoption-osxphotos-query-max-size"],
+            [0, "cmdoption-osxphotos-repl-max-size"],
+            [0, "cmdoption-osxphotos-sync-max-size"]
+        ],
+        "--merge": [
+            [0, "cmdoption-osxphotos-sync-m"]
+        ],
+        "--merge-keywords": [
+            [0, "cmdoption-osxphotos-import-m"]
+        ],
+        "--migrate": [
+            [0, "cmdoption-osxphotos-exportdb-migrate"]
+        ],
+        "--migrate-photos-library": [
+            [0, "cmdoption-osxphotos-exportdb-migrate-photos-library"]
+        ],
+        "--min-size": [
+            [0, "cmdoption-osxphotos-add-locations-min-size"],
+            [0, "cmdoption-osxphotos-export-min-size"],
+            [0, "cmdoption-osxphotos-query-min-size"],
+            [0, "cmdoption-osxphotos-repl-min-size"],
+            [0, "cmdoption-osxphotos-sync-min-size"]
+        ],
+        "--missing": [
+            [0, "cmdoption-osxphotos-add-locations-missing"],
+            [0, "cmdoption-osxphotos-export-missing"],
+            [0, "cmdoption-osxphotos-query-missing"],
+            [0, "cmdoption-osxphotos-repl-missing"],
+            [0, "cmdoption-osxphotos-sync-missing"]
+        ],
+        "--name": [
+            [0, "cmdoption-osxphotos-add-locations-name"],
+            [0, "cmdoption-osxphotos-export-name"],
+            [0, "cmdoption-osxphotos-query-name"],
+            [0, "cmdoption-osxphotos-repl-name"],
+            [0, "cmdoption-osxphotos-sync-name"]
+        ],
+        "--no-comment": [
+            [0, "cmdoption-osxphotos-add-locations-no-comment"],
+            [0, "cmdoption-osxphotos-export-no-comment"],
+            [0, "cmdoption-osxphotos-query-no-comment"],
+            [0, "cmdoption-osxphotos-repl-no-comment"],
+            [0, "cmdoption-osxphotos-sync-no-comment"]
+        ],
+        "--no-description": [
+            [0, "cmdoption-osxphotos-add-locations-no-description"],
+            [0, "cmdoption-osxphotos-export-no-description"],
+            [0, "cmdoption-osxphotos-query-no-description"],
+            [0, "cmdoption-osxphotos-repl-no-description"],
+            [0, "cmdoption-osxphotos-sync-no-description"]
+        ],
+        "--no-keyword": [
+            [0, "cmdoption-osxphotos-add-locations-no-keyword"],
+            [0, "cmdoption-osxphotos-export-no-keyword"],
+            [0, "cmdoption-osxphotos-query-no-keyword"],
+            [0, "cmdoption-osxphotos-repl-no-keyword"],
+            [0, "cmdoption-osxphotos-sync-no-keyword"]
+        ],
+        "--no-likes": [
+            [0, "cmdoption-osxphotos-add-locations-no-likes"],
+            [0, "cmdoption-osxphotos-export-no-likes"],
+            [0, "cmdoption-osxphotos-query-no-likes"],
+            [0, "cmdoption-osxphotos-repl-no-likes"],
+            [0, "cmdoption-osxphotos-sync-no-likes"]
+        ],
+        "--no-location": [
+            [0, "cmdoption-osxphotos-add-locations-no-location"],
+            [0, "cmdoption-osxphotos-export-no-location"],
+            [0, "cmdoption-osxphotos-query-no-location"],
+            [0, "cmdoption-osxphotos-repl-no-location"],
+            [0, "cmdoption-osxphotos-sync-no-location"]
+        ],
+        "--no-place": [
+            [0, "cmdoption-osxphotos-add-locations-no-place"],
+            [0, "cmdoption-osxphotos-export-no-place"],
+            [0, "cmdoption-osxphotos-query-no-place"],
+            [0, "cmdoption-osxphotos-repl-no-place"],
+            [0, "cmdoption-osxphotos-sync-no-place"]
+        ],
+        "--no-progress": [
+            [0, "cmdoption-osxphotos-export-no-progress"],
+            [0, "cmdoption-osxphotos-import-no-progress"]
+        ],
+        "--no-title": [
+            [0, "cmdoption-osxphotos-add-locations-no-title"],
+            [0, "cmdoption-osxphotos-export-no-title"],
+            [0, "cmdoption-osxphotos-query-no-title"],
+            [0, "cmdoption-osxphotos-repl-no-title"],
+            [0, "cmdoption-osxphotos-sync-no-title"]
+        ],
+        "--not-burst": [
+            [0, "cmdoption-osxphotos-add-locations-not-burst"],
+            [0, "cmdoption-osxphotos-export-not-burst"],
+            [0, "cmdoption-osxphotos-query-not-burst"],
+            [0, "cmdoption-osxphotos-repl-not-burst"],
+            [0, "cmdoption-osxphotos-sync-not-burst"]
+        ],
+        "--not-cloudasset": [
+            [0, "cmdoption-osxphotos-add-locations-not-cloudasset"],
+            [0, "cmdoption-osxphotos-export-not-cloudasset"],
+            [0, "cmdoption-osxphotos-query-not-cloudasset"],
+            [0, "cmdoption-osxphotos-repl-not-cloudasset"],
+            [0, "cmdoption-osxphotos-sync-not-cloudasset"]
+        ],
+        "--not-edited": [
+            [0, "cmdoption-osxphotos-add-locations-not-edited"],
+            [0, "cmdoption-osxphotos-export-not-edited"],
+            [0, "cmdoption-osxphotos-query-not-edited"],
+            [0, "cmdoption-osxphotos-repl-not-edited"],
+            [0, "cmdoption-osxphotos-sync-not-edited"]
+        ],
+        "--not-favorite": [
+            [0, "cmdoption-osxphotos-add-locations-not-favorite"],
+            [0, "cmdoption-osxphotos-export-not-favorite"],
+            [0, "cmdoption-osxphotos-query-not-favorite"],
+            [0, "cmdoption-osxphotos-repl-not-favorite"],
+            [0, "cmdoption-osxphotos-sync-not-favorite"]
+        ],
+        "--not-hdr": [
+            [0, "cmdoption-osxphotos-add-locations-not-hdr"],
+            [0, "cmdoption-osxphotos-export-not-hdr"],
+            [0, "cmdoption-osxphotos-query-not-hdr"],
+            [0, "cmdoption-osxphotos-repl-not-hdr"],
+            [0, "cmdoption-osxphotos-sync-not-hdr"]
+        ],
+        "--not-hidden": [
+            [0, "cmdoption-osxphotos-add-locations-not-hidden"],
+            [0, "cmdoption-osxphotos-export-not-hidden"],
+            [0, "cmdoption-osxphotos-query-not-hidden"],
+            [0, "cmdoption-osxphotos-repl-not-hidden"],
+            [0, "cmdoption-osxphotos-sync-not-hidden"]
+        ],
+        "--not-in-album": [
+            [0, "cmdoption-osxphotos-add-locations-not-in-album"],
+            [0, "cmdoption-osxphotos-export-not-in-album"],
+            [0, "cmdoption-osxphotos-query-not-in-album"],
+            [0, "cmdoption-osxphotos-repl-not-in-album"],
+            [0, "cmdoption-osxphotos-sync-not-in-album"]
+        ],
+        "--not-incloud": [
+            [0, "cmdoption-osxphotos-add-locations-not-incloud"],
+            [0, "cmdoption-osxphotos-export-not-incloud"],
+            [0, "cmdoption-osxphotos-query-not-incloud"],
+            [0, "cmdoption-osxphotos-repl-not-incloud"],
+            [0, "cmdoption-osxphotos-sync-not-incloud"]
+        ],
+        "--not-live": [
+            [0, "cmdoption-osxphotos-add-locations-not-live"],
+            [0, "cmdoption-osxphotos-export-not-live"],
+            [0, "cmdoption-osxphotos-query-not-live"],
+            [0, "cmdoption-osxphotos-repl-not-live"],
+            [0, "cmdoption-osxphotos-sync-not-live"]
+        ],
+        "--not-missing": [
+            [0, "cmdoption-osxphotos-add-locations-not-missing"],
+            [0, "cmdoption-osxphotos-export-not-missing"],
+            [0, "cmdoption-osxphotos-query-not-missing"],
+            [0, "cmdoption-osxphotos-repl-not-missing"],
+            [0, "cmdoption-osxphotos-sync-not-missing"]
+        ],
+        "--not-panorama": [
+            [0, "cmdoption-osxphotos-add-locations-not-panorama"],
+            [0, "cmdoption-osxphotos-export-not-panorama"],
+            [0, "cmdoption-osxphotos-query-not-panorama"],
+            [0, "cmdoption-osxphotos-repl-not-panorama"],
+            [0, "cmdoption-osxphotos-sync-not-panorama"]
+        ],
+        "--not-portrait": [
+            [0, "cmdoption-osxphotos-add-locations-not-portrait"],
+            [0, "cmdoption-osxphotos-export-not-portrait"],
+            [0, "cmdoption-osxphotos-query-not-portrait"],
+            [0, "cmdoption-osxphotos-repl-not-portrait"],
+            [0, "cmdoption-osxphotos-sync-not-portrait"]
+        ],
+        "--not-reference": [
+            [0, "cmdoption-osxphotos-add-locations-not-reference"],
+            [0, "cmdoption-osxphotos-export-not-reference"],
+            [0, "cmdoption-osxphotos-query-not-reference"],
+            [0, "cmdoption-osxphotos-repl-not-reference"],
+            [0, "cmdoption-osxphotos-sync-not-reference"]
+        ],
+        "--not-screenshot": [
+            [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
+            [0, "cmdoption-osxphotos-export-not-screenshot"],
+            [0, "cmdoption-osxphotos-query-not-screenshot"],
+            [0, "cmdoption-osxphotos-repl-not-screenshot"],
+            [0, "cmdoption-osxphotos-sync-not-screenshot"]
+        ],
+        "--not-selfie": [
+            [0, "cmdoption-osxphotos-add-locations-not-selfie"],
+            [0, "cmdoption-osxphotos-export-not-selfie"],
+            [0, "cmdoption-osxphotos-query-not-selfie"],
+            [0, "cmdoption-osxphotos-repl-not-selfie"],
+            [0, "cmdoption-osxphotos-sync-not-selfie"]
+        ],
+        "--not-shared": [
+            [0, "cmdoption-osxphotos-add-locations-not-shared"],
+            [0, "cmdoption-osxphotos-export-not-shared"],
+            [0, "cmdoption-osxphotos-query-not-shared"],
+            [0, "cmdoption-osxphotos-repl-not-shared"]
+        ],
+        "--not-slow-mo": [
+            [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
+            [0, "cmdoption-osxphotos-export-not-slow-mo"],
+            [0, "cmdoption-osxphotos-query-not-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-not-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-not-slow-mo"]
+        ],
+        "--not-time-lapse": [
+            [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
+            [0, "cmdoption-osxphotos-export-not-time-lapse"],
+            [0, "cmdoption-osxphotos-query-not-time-lapse"],
+            [0, "cmdoption-osxphotos-repl-not-time-lapse"],
+            [0, "cmdoption-osxphotos-sync-not-time-lapse"]
+        ],
+        "--only-movies": [
+            [0, "cmdoption-osxphotos-add-locations-only-movies"],
+            [0, "cmdoption-osxphotos-export-only-movies"],
+            [0, "cmdoption-osxphotos-query-only-movies"],
+            [0, "cmdoption-osxphotos-repl-only-movies"],
+            [0, "cmdoption-osxphotos-sync-only-movies"]
+        ],
+        "--only-new": [
+            [0, "cmdoption-osxphotos-export-only-new"]
+        ],
+        "--only-photos": [
+            [0, "cmdoption-osxphotos-add-locations-only-photos"],
+            [0, "cmdoption-osxphotos-export-only-photos"],
+            [0, "cmdoption-osxphotos-query-only-photos"],
+            [0, "cmdoption-osxphotos-repl-only-photos"],
+            [0, "cmdoption-osxphotos-sync-only-photos"]
+        ],
+        "--original-suffix": [
+            [0, "cmdoption-osxphotos-export-original-suffix"]
+        ],
+        "--overwrite": [
+            [0, "cmdoption-osxphotos-export-overwrite"]
+        ],
+        "--panorama": [
+            [0, "cmdoption-osxphotos-add-locations-panorama"],
+            [0, "cmdoption-osxphotos-export-panorama"],
+            [0, "cmdoption-osxphotos-query-panorama"],
+            [0, "cmdoption-osxphotos-repl-panorama"],
+            [0, "cmdoption-osxphotos-sync-panorama"]
+        ],
+        "--parse-date": [
+            [0, "cmdoption-osxphotos-import-P"],
+            [0, "cmdoption-osxphotos-timewarp-M"]
+        ],
+        "--person": [
+            [0, "cmdoption-osxphotos-add-locations-person"],
+            [0, "cmdoption-osxphotos-export-person"],
+            [0, "cmdoption-osxphotos-query-person"],
+            [0, "cmdoption-osxphotos-repl-person"],
+            [0, "cmdoption-osxphotos-sync-person"]
+        ],
+        "--person-keyword": [
+            [0, "cmdoption-osxphotos-exiftool-person-keyword"],
+            [0, "cmdoption-osxphotos-export-person-keyword"]
+        ],
+        "--place": [
+            [0, "cmdoption-osxphotos-add-locations-place"],
+            [0, "cmdoption-osxphotos-export-place"],
+            [0, "cmdoption-osxphotos-query-place"],
+            [0, "cmdoption-osxphotos-repl-place"],
+            [0, "cmdoption-osxphotos-sync-place"]
+        ],
+        "--plain": [
+            [0, "cmdoption-osxphotos-timewarp-plain"]
+        ],
+        "--portrait": [
+            [0, "cmdoption-osxphotos-add-locations-portrait"],
+            [0, "cmdoption-osxphotos-export-portrait"],
+            [0, "cmdoption-osxphotos-query-portrait"],
+            [0, "cmdoption-osxphotos-repl-portrait"],
+            [0, "cmdoption-osxphotos-sync-portrait"]
+        ],
+        "--post-command": [
+            [0, "cmdoption-osxphotos-export-post-command"]
+        ],
+        "--post-function": [
+            [0, "cmdoption-osxphotos-export-post-function"],
+            [0, "cmdoption-osxphotos-import-post-function"]
+        ],
+        "--preview": [
+            [0, "cmdoption-osxphotos-export-preview"],
+            [0, "cmdoption-osxphotos-theme-preview"]
+        ],
+        "--preview-if-missing": [
+            [0, "cmdoption-osxphotos-export-preview-if-missing"]
+        ],
+        "--preview-suffix": [
+            [0, "cmdoption-osxphotos-export-preview-suffix"]
+        ],
+        "--print": [
+            [0, "cmdoption-osxphotos-dump-print"],
+            [0, "cmdoption-osxphotos-export-print"],
+            [0, "cmdoption-osxphotos-query-print"]
+        ],
+        "--pull-exif": [
+            [0, "cmdoption-osxphotos-timewarp-P"]
+        ],
+        "--push-exif": [
+            [0, "cmdoption-osxphotos-timewarp-p"]
+        ],
+        "--query-eval": [
+            [0, "cmdoption-osxphotos-add-locations-query-eval"],
+            [0, "cmdoption-osxphotos-export-query-eval"],
+            [0, "cmdoption-osxphotos-query-query-eval"],
+            [0, "cmdoption-osxphotos-repl-query-eval"],
+            [0, "cmdoption-osxphotos-sync-query-eval"]
+        ],
+        "--query-function": [
+            [0, "cmdoption-osxphotos-add-locations-query-function"],
+            [0, "cmdoption-osxphotos-export-query-function"],
+            [0, "cmdoption-osxphotos-query-query-function"],
+            [0, "cmdoption-osxphotos-repl-query-function"],
+            [0, "cmdoption-osxphotos-sync-query-function"]
+        ],
+        "--quiet": [
+            [0, "cmdoption-osxphotos-query-quiet"]
+        ],
+        "--ramdb": [
+            [0, "cmdoption-osxphotos-export-ramdb"]
+        ],
+        "--raw-output": [
+            [0, "cmdoption-osxphotos-diff-r"]
+        ],
+        "--regex": [
+            [0, "cmdoption-osxphotos-add-locations-regex"],
+            [0, "cmdoption-osxphotos-export-regex"],
+            [0, "cmdoption-osxphotos-query-regex"],
+            [0, "cmdoption-osxphotos-repl-regex"],
+            [0, "cmdoption-osxphotos-sync-regex"]
+        ],
+        "--relative-to": [
+            [0, "cmdoption-osxphotos-import-r"]
+        ],
+        "--replace-keywords": [
+            [0, "cmdoption-osxphotos-batch-edit-replace-keywords"],
+            [0, "cmdoption-osxphotos-exiftool-replace-keywords"],
+            [0, "cmdoption-osxphotos-export-replace-keywords"]
+        ],
+        "--report": [
+            [0, "cmdoption-osxphotos-exiftool-report"],
+            [0, "cmdoption-osxphotos-export-report"],
+            [0, "cmdoption-osxphotos-exportdb-report"],
+            [0, "cmdoption-osxphotos-import-report"],
+            [0, "cmdoption-osxphotos-sync-R"]
+        ],
+        "--resume": [
+            [0, "cmdoption-osxphotos-import-R"]
+        ],
+        "--retry": [
+            [0, "cmdoption-osxphotos-export-retry"]
+        ],
+        "--run": [
+            [0, "cmdoption-osxphotos-version-run"]
+        ],
+        "--save-config": [
+            [0, "cmdoption-osxphotos-exiftool-save-config"],
+            [0, "cmdoption-osxphotos-export-save-config"],
+            [0, "cmdoption-osxphotos-exportdb-save-config"]
+        ],
+        "--screenshot": [
+            [0, "cmdoption-osxphotos-add-locations-screenshot"],
+            [0, "cmdoption-osxphotos-export-screenshot"],
+            [0, "cmdoption-osxphotos-query-screenshot"],
+            [0, "cmdoption-osxphotos-repl-screenshot"],
+            [0, "cmdoption-osxphotos-sync-screenshot"]
+        ],
+        "--selected": [
+            [0, "cmdoption-osxphotos-add-locations-selected"],
+            [0, "cmdoption-osxphotos-export-selected"],
+            [0, "cmdoption-osxphotos-query-selected"],
+            [0, "cmdoption-osxphotos-repl-selected"],
+            [0, "cmdoption-osxphotos-sync-selected"]
+        ],
+        "--selfie": [
+            [0, "cmdoption-osxphotos-add-locations-selfie"],
+            [0, "cmdoption-osxphotos-export-selfie"],
+            [0, "cmdoption-osxphotos-query-selfie"],
+            [0, "cmdoption-osxphotos-repl-selfie"],
+            [0, "cmdoption-osxphotos-sync-selfie"]
+        ],
+        "--set": [
+            [0, "cmdoption-osxphotos-sync-s"]
+        ],
+        "--shared": [
+            [0, "cmdoption-osxphotos-add-locations-shared"],
+            [0, "cmdoption-osxphotos-export-shared"],
+            [0, "cmdoption-osxphotos-query-shared"],
+            [0, "cmdoption-osxphotos-repl-shared"]
+        ],
+        "--sidecar": [
+            [0, "cmdoption-osxphotos-export-sidecar"]
+        ],
+        "--sidecar-drop-ext": [
+            [0, "cmdoption-osxphotos-export-sidecar-drop-ext"]
+        ],
+        "--skip-bursts": [
+            [0, "cmdoption-osxphotos-export-skip-bursts"]
+        ],
+        "--skip-edited": [
+            [0, "cmdoption-osxphotos-export-skip-edited"]
+        ],
+        "--skip-live": [
+            [0, "cmdoption-osxphotos-export-skip-live"]
+        ],
+        "--skip-original-if-edited": [
+            [0, "cmdoption-osxphotos-export-skip-original-if-edited"]
+        ],
+        "--skip-raw": [
+            [0, "cmdoption-osxphotos-export-skip-raw"]
+        ],
+        "--skip-uuid": [
+            [0, "cmdoption-osxphotos-export-skip-uuid"]
+        ],
+        "--skip-uuid-from-file": [
+            [0, "cmdoption-osxphotos-export-skip-uuid-from-file"]
+        ],
+        "--slow-mo": [
+            [0, "cmdoption-osxphotos-add-locations-slow-mo"],
+            [0, "cmdoption-osxphotos-export-slow-mo"],
+            [0, "cmdoption-osxphotos-query-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-slow-mo"]
+        ],
+        "--split-folder": [
+            [0, "cmdoption-osxphotos-import-f"]
+        ],
+        "--sql": [
+            [0, "cmdoption-osxphotos-exportdb-sql"]
+        ],
+        "--strip": [
+            [0, "cmdoption-osxphotos-export-strip"]
+        ],
+        "--style": [
+            [0, "cmdoption-osxphotos-diff-s"]
+        ],
+        "--template": [
+            [0, "cmdoption-osxphotos-inspect-T"]
+        ],
+        "--theme": [
+            [0, "cmdoption-osxphotos-add-locations-theme"],
+            [0, "cmdoption-osxphotos-batch-edit-theme"],
+            [0, "cmdoption-osxphotos-exiftool-theme"],
+            [0, "cmdoption-osxphotos-export-theme"],
+            [0, "cmdoption-osxphotos-exportdb-theme"],
+            [0, "cmdoption-osxphotos-import-theme"],
+            [0, "cmdoption-osxphotos-inspect-theme"],
+            [0, "cmdoption-osxphotos-orphans-theme"],
+            [0, "cmdoption-osxphotos-sync-theme"],
+            [0, "cmdoption-osxphotos-timewarp-theme"]
+        ],
+        "--time": [
+            [0, "cmdoption-osxphotos-timewarp-t"]
+        ],
+        "--time-delta": [
+            [0, "cmdoption-osxphotos-timewarp-T"]
+        ],
+        "--time-lapse": [
+            [0, "cmdoption-osxphotos-add-locations-time-lapse"],
+            [0, "cmdoption-osxphotos-export-time-lapse"],
+            [0, "cmdoption-osxphotos-query-time-lapse"],
+            [0, "cmdoption-osxphotos-repl-time-lapse"],
+            [0, "cmdoption-osxphotos-sync-time-lapse"]
+        ],
+        "--timestamp": [
+            [0, "cmdoption-osxphotos-add-locations-timestamp"],
+            [0, "cmdoption-osxphotos-batch-edit-timestamp"],
+            [0, "cmdoption-osxphotos-diff-timestamp"],
+            [0, "cmdoption-osxphotos-exiftool-timestamp"],
+            [0, "cmdoption-osxphotos-export-timestamp"],
+            [0, "cmdoption-osxphotos-exportdb-timestamp"],
+            [0, "cmdoption-osxphotos-import-timestamp"],
+            [0, "cmdoption-osxphotos-orphans-timestamp"],
+            [0, "cmdoption-osxphotos-sync-timestamp"],
+            [0, "cmdoption-osxphotos-timewarp-2"],
+            [0, "cmdoption-osxphotos-timewarp-timestamp"]
+        ],
+        "--timezone": [
+            [0, "cmdoption-osxphotos-timewarp-z"]
+        ],
+        "--title": [
+            [0, "cmdoption-osxphotos-add-locations-title"],
+            [0, "cmdoption-osxphotos-batch-edit-title"],
+            [0, "cmdoption-osxphotos-export-title"],
+            [0, "cmdoption-osxphotos-import-t"],
+            [0, "cmdoption-osxphotos-query-title"],
+            [0, "cmdoption-osxphotos-repl-title"],
+            [0, "cmdoption-osxphotos-sync-title"]
+        ],
+        "--tmpdir": [
+            [0, "cmdoption-osxphotos-export-tmpdir"]
+        ],
+        "--to-date": [
+            [0, "cmdoption-osxphotos-add-locations-to-date"],
+            [0, "cmdoption-osxphotos-export-to-date"],
+            [0, "cmdoption-osxphotos-query-to-date"],
+            [0, "cmdoption-osxphotos-repl-to-date"],
+            [0, "cmdoption-osxphotos-sync-to-date"]
+        ],
+        "--to-time": [
+            [0, "cmdoption-osxphotos-add-locations-to-time"],
+            [0, "cmdoption-osxphotos-export-to-time"],
+            [0, "cmdoption-osxphotos-query-to-time"],
+            [0, "cmdoption-osxphotos-repl-to-time"],
+            [0, "cmdoption-osxphotos-sync-to-time"]
+        ],
+        "--touch-file": [
+            [0, "cmdoption-osxphotos-export-touch-file"],
+            [0, "cmdoption-osxphotos-exportdb-touch-file"]
+        ],
+        "--undo": [
+            [0, "cmdoption-osxphotos-batch-edit-undo"]
+        ],
+        "--unmatched": [
+            [0, "cmdoption-osxphotos-sync-U"]
+        ],
+        "--update": [
+            [0, "cmdoption-osxphotos-export-update"]
+        ],
+        "--update-errors": [
+            [0, "cmdoption-osxphotos-export-update-errors"]
+        ],
+        "--update-signatures": [
+            [0, "cmdoption-osxphotos-exportdb-update-signatures"]
+        ],
+        "--upgrade": [
+            [0, "cmdoption-osxphotos-install-U"]
+        ],
+        "--use-file-time": [
+            [0, "cmdoption-osxphotos-timewarp-1"]
+        ],
+        "--use-photokit": [
+            [0, "cmdoption-osxphotos-export-use-photokit"]
+        ],
+        "--use-photos-export": [
+            [0, "cmdoption-osxphotos-export-use-photos-export"]
+        ],
+        "--uti": [
+            [0, "cmdoption-osxphotos-add-locations-uti"],
+            [0, "cmdoption-osxphotos-export-uti"],
+            [0, "cmdoption-osxphotos-query-uti"],
+            [0, "cmdoption-osxphotos-repl-uti"],
+            [0, "cmdoption-osxphotos-sync-uti"]
+        ],
+        "--uuid": [
+            [0, "cmdoption-osxphotos-add-locations-uuid"],
+            [0, "cmdoption-osxphotos-export-uuid"],
+            [0, "cmdoption-osxphotos-query-uuid"],
+            [0, "cmdoption-osxphotos-repl-uuid"],
+            [0, "cmdoption-osxphotos-sync-uuid"]
+        ],
+        "--uuid-files": [
+            [0, "cmdoption-osxphotos-exportdb-uuid-files"]
+        ],
+        "--uuid-from-file": [
+            [0, "cmdoption-osxphotos-add-locations-uuid-from-file"],
+            [0, "cmdoption-osxphotos-export-uuid-from-file"],
+            [0, "cmdoption-osxphotos-query-uuid-from-file"],
+            [0, "cmdoption-osxphotos-repl-uuid-from-file"],
+            [0, "cmdoption-osxphotos-sync-uuid-from-file"]
+        ],
+        "--uuid-info": [
+            [0, "cmdoption-osxphotos-exportdb-uuid-info"]
+        ],
+        "--vacuum": [
+            [0, "cmdoption-osxphotos-exportdb-vacuum"]
+        ],
+        "--verbose": [
+            [0, "cmdoption-osxphotos-add-locations-V"],
+            [0, "cmdoption-osxphotos-batch-edit-V"],
+            [0, "cmdoption-osxphotos-diff-V"],
+            [0, "cmdoption-osxphotos-exiftool-V"],
+            [0, "cmdoption-osxphotos-export-V"],
+            [0, "cmdoption-osxphotos-exportdb-V"],
+            [0, "cmdoption-osxphotos-import-V"],
+            [0, "cmdoption-osxphotos-orphans-V"],
+            [0, "cmdoption-osxphotos-sync-V"],
+            [0, "cmdoption-osxphotos-timewarp-V"]
+        ],
+        "--version": [
+            [0, "cmdoption-osxphotos-exportdb-version"],
+            [0, "cmdoption-osxphotos-v"]
+        ],
+        "--walk": [
+            [0, "cmdoption-osxphotos-import-w"]
+        ],
+        "--window": [
+            [0, "cmdoption-osxphotos-add-locations-w"]
+        ],
+        "--xattr-template": [
+            [0, "cmdoption-osxphotos-export-xattr-template"]
+        ],
+        "--year": [
+            [0, "cmdoption-osxphotos-add-locations-year"],
+            [0, "cmdoption-osxphotos-export-year"],
+            [0, "cmdoption-osxphotos-query-year"],
+            [0, "cmdoption-osxphotos-repl-year"],
+            [0, "cmdoption-osxphotos-sync-year"]
+        ],
+        "--yes": [
+            [0, "cmdoption-osxphotos-uninstall-y"]
+        ],
+        "-a": [
+            [0, "cmdoption-osxphotos-sync-A"],
+            [0, "cmdoption-osxphotos-import-a"],
+            [0, "cmdoption-osxphotos-timewarp-a"]
+        ],
+        "-c": [
+            [0, "cmdoption-osxphotos-import-C"],
+            [0, "cmdoption-osxphotos-timewarp-c"]
+        ],
+        "-d": [
+            [0, "cmdoption-osxphotos-import-D"],
+            [0, "cmdoption-osxphotos-timewarp-D"],
+            [0, "cmdoption-osxphotos-import-d"],
+            [0, "cmdoption-osxphotos-timewarp-d"]
+        ],
+        "-f": [
+            [0, "cmdoption-osxphotos-timewarp-F"],
+            [0, "cmdoption-osxphotos-dump-f"],
+            [0, "cmdoption-osxphotos-import-f"],
+            [0, "cmdoption-osxphotos-query-f"],
+            [0, "cmdoption-osxphotos-timewarp-1"],
+            [0, "cmdoption-osxphotos-uuid-f"]
+        ],
+        "-l": [
+            [0, "cmdoption-osxphotos-import-L"],
+            [0, "cmdoption-osxphotos-timewarp-L"],
+            [0, "cmdoption-osxphotos-import-l"]
+        ],
+        "-m": [
+            [0, "cmdoption-osxphotos-timewarp-M"],
+            [0, "cmdoption-osxphotos-import-m"],
+            [0, "cmdoption-osxphotos-sync-m"],
+            [0, "cmdoption-osxphotos-timewarp-0"]
+        ],
+        "-p": [
+            [0, "cmdoption-osxphotos-import-P"],
+            [0, "cmdoption-osxphotos-timewarp-P"],
+            [0, "cmdoption-osxphotos-import-0"],
+            [0, "cmdoption-osxphotos-timewarp-p"]
+        ],
+        "-r": [
+            [0, "cmdoption-osxphotos-import-R"],
+            [0, "cmdoption-osxphotos-sync-R"],
+            [0, "cmdoption-osxphotos-diff-r"],
+            [0, "cmdoption-osxphotos-import-r"]
+        ],
+        "-t": [
+            [0, "cmdoption-osxphotos-inspect-T"],
+            [0, "cmdoption-osxphotos-timewarp-T"],
+            [0, "cmdoption-osxphotos-import-t"],
+            [0, "cmdoption-osxphotos-inspect-t"],
+            [0, "cmdoption-osxphotos-timewarp-t"]
+        ],
+        "-u": [
+            [0, "cmdoption-osxphotos-install-U"],
+            [0, "cmdoption-osxphotos-sync-U"]
+        ],
+        "-v": [
+            [0, "cmdoption-osxphotos-add-locations-V"],
+            [0, "cmdoption-osxphotos-batch-edit-V"],
+            [0, "cmdoption-osxphotos-diff-V"],
+            [0, "cmdoption-osxphotos-exiftool-V"],
+            [0, "cmdoption-osxphotos-export-V"],
+            [0, "cmdoption-osxphotos-exportdb-V"],
+            [0, "cmdoption-osxphotos-import-V"],
+            [0, "cmdoption-osxphotos-orphans-V"],
+            [0, "cmdoption-osxphotos-sync-V"],
+            [0, "cmdoption-osxphotos-timewarp-V"],
+            [0, "cmdoption-osxphotos-v"]
+        ],
+        "-e": [
+            [0, "cmdoption-osxphotos-import-e"],
+            [0, "cmdoption-osxphotos-sync-e"],
+            [0, "cmdoption-osxphotos-timewarp-e"]
+        ],
+        "-g": [
+            [0, "cmdoption-osxphotos-import-g"]
+        ],
+        "-h": [
+            [0, "cmdoption-osxphotos-run-h"]
+        ],
+        "-i": [
+            [0, "cmdoption-osxphotos-add-locations-i"],
+            [0, "cmdoption-osxphotos-export-i"],
+            [0, "cmdoption-osxphotos-query-i"],
+            [0, "cmdoption-osxphotos-repl-i"],
+            [0, "cmdoption-osxphotos-sync-0"],
+            [0, "cmdoption-osxphotos-sync-i"],
+            [0, "cmdoption-osxphotos-timewarp-i"]
+        ],
+        "-k": [
+            [0, "cmdoption-osxphotos-import-k"]
+        ],
+        "-s": [
+            [0, "cmdoption-osxphotos-diff-s"],
+            [0, "cmdoption-osxphotos-sync-s"]
+        ],
+        "-w": [
+            [0, "cmdoption-osxphotos-add-locations-w"],
+            [0, "cmdoption-osxphotos-import-w"]
+        ],
+        "-y": [
+            [0, "cmdoption-osxphotos-uninstall-y"]
+        ],
+        "-z": [
+            [0, "cmdoption-osxphotos-timewarp-z"]
+        ],
+        "args": [
+            [0, "cmdoption-osxphotos-run-arg-ARGS"]
+        ],
+        "db2": [
+            [0, "cmdoption-osxphotos-diff-arg-DB2"]
+        ],
+        "dest": [
+            [0, "cmdoption-osxphotos-export-arg-DEST"]
+        ],
+        "export_database": [
+            [0, "cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE"]
+        ],
+        "export_directory": [
+            [0, "cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY"]
+        ],
+        "files": [
+            [0, "cmdoption-osxphotos-import-arg-FILES"]
+        ],
+        "packages": [
+            [0, "cmdoption-osxphotos-install-arg-PACKAGES"],
+            [0, "cmdoption-osxphotos-uninstall-arg-PACKAGES"]
+        ],
+        "photos_library": [
+            [0, "cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY"]
+        ],
+        "python_file": [
+            [0, "cmdoption-osxphotos-run-arg-PYTHON_FILE"]
+        ],
+        "subtopic": [
+            [0, "cmdoption-osxphotos-help-arg-SUBTOPIC"]
+        ],
+        "topic": [
+            [0, "cmdoption-osxphotos-help-arg-TOPIC"]
+        ],
+        "uuid_or_name": [
+            [0, "cmdoption-osxphotos-show-arg-UUID_OR_NAME"]
+        ],
+        "width": [
+            [0, "cmdoption-osxphotos-tutorial-arg-WIDTH"]
+        ],
+        "osxphotos command line option": [
+            [0, "cmdoption-osxphotos-json"],
+            [0, "cmdoption-osxphotos-library"],
+            [0, "cmdoption-osxphotos-v"]
+        ],
+        "osxphotos-add-locations command line option": [
+            [0, "cmdoption-osxphotos-add-locations-V"],
+            [0, "cmdoption-osxphotos-add-locations-added-after"],
+            [0, "cmdoption-osxphotos-add-locations-added-before"],
+            [0, "cmdoption-osxphotos-add-locations-added-in-last"],
+            [0, "cmdoption-osxphotos-add-locations-album"],
+            [0, "cmdoption-osxphotos-add-locations-burst"],
+            [0, "cmdoption-osxphotos-add-locations-cloudasset"],
+            [0, "cmdoption-osxphotos-add-locations-description"],
+            [0, "cmdoption-osxphotos-add-locations-dry-run"],
+            [0, "cmdoption-osxphotos-add-locations-duplicate"],
+            [0, "cmdoption-osxphotos-add-locations-edited"],
+            [0, "cmdoption-osxphotos-add-locations-exif"],
+            [0, "cmdoption-osxphotos-add-locations-external-edit"],
+            [0, "cmdoption-osxphotos-add-locations-favorite"],
+            [0, "cmdoption-osxphotos-add-locations-folder"],
+            [0, "cmdoption-osxphotos-add-locations-from-date"],
+            [0, "cmdoption-osxphotos-add-locations-from-time"],
+            [0, "cmdoption-osxphotos-add-locations-has-comment"],
+            [0, "cmdoption-osxphotos-add-locations-has-likes"],
+            [0, "cmdoption-osxphotos-add-locations-has-raw"],
+            [0, "cmdoption-osxphotos-add-locations-hdr"],
+            [0, "cmdoption-osxphotos-add-locations-hidden"],
+            [0, "cmdoption-osxphotos-add-locations-i"],
+            [0, "cmdoption-osxphotos-add-locations-in-album"],
+            [0, "cmdoption-osxphotos-add-locations-incloud"],
+            [0, "cmdoption-osxphotos-add-locations-is-reference"],
+            [0, "cmdoption-osxphotos-add-locations-keyword"],
+            [0, "cmdoption-osxphotos-add-locations-label"],
+            [0, "cmdoption-osxphotos-add-locations-live"],
+            [0, "cmdoption-osxphotos-add-locations-location"],
+            [0, "cmdoption-osxphotos-add-locations-max-size"],
+            [0, "cmdoption-osxphotos-add-locations-min-size"],
+            [0, "cmdoption-osxphotos-add-locations-missing"],
+            [0, "cmdoption-osxphotos-add-locations-name"],
+            [0, "cmdoption-osxphotos-add-locations-no-comment"],
+            [0, "cmdoption-osxphotos-add-locations-no-description"],
+            [0, "cmdoption-osxphotos-add-locations-no-keyword"],
+            [0, "cmdoption-osxphotos-add-locations-no-likes"],
+            [0, "cmdoption-osxphotos-add-locations-no-location"],
+            [0, "cmdoption-osxphotos-add-locations-no-place"],
+            [0, "cmdoption-osxphotos-add-locations-no-title"],
+            [0, "cmdoption-osxphotos-add-locations-not-burst"],
+            [0, "cmdoption-osxphotos-add-locations-not-cloudasset"],
+            [0, "cmdoption-osxphotos-add-locations-not-edited"],
+            [0, "cmdoption-osxphotos-add-locations-not-favorite"],
+            [0, "cmdoption-osxphotos-add-locations-not-hdr"],
+            [0, "cmdoption-osxphotos-add-locations-not-hidden"],
+            [0, "cmdoption-osxphotos-add-locations-not-in-album"],
+            [0, "cmdoption-osxphotos-add-locations-not-incloud"],
+            [0, "cmdoption-osxphotos-add-locations-not-live"],
+            [0, "cmdoption-osxphotos-add-locations-not-missing"],
+            [0, "cmdoption-osxphotos-add-locations-not-panorama"],
+            [0, "cmdoption-osxphotos-add-locations-not-portrait"],
+            [0, "cmdoption-osxphotos-add-locations-not-reference"],
+            [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
+            [0, "cmdoption-osxphotos-add-locations-not-selfie"],
+            [0, "cmdoption-osxphotos-add-locations-not-shared"],
+            [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
+            [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
+            [0, "cmdoption-osxphotos-add-locations-only-movies"],
+            [0, "cmdoption-osxphotos-add-locations-only-photos"],
+            [0, "cmdoption-osxphotos-add-locations-panorama"],
+            [0, "cmdoption-osxphotos-add-locations-person"],
+            [0, "cmdoption-osxphotos-add-locations-place"],
+            [0, "cmdoption-osxphotos-add-locations-portrait"],
+            [0, "cmdoption-osxphotos-add-locations-query-eval"],
+            [0, "cmdoption-osxphotos-add-locations-query-function"],
+            [0, "cmdoption-osxphotos-add-locations-regex"],
+            [0, "cmdoption-osxphotos-add-locations-screenshot"],
+            [0, "cmdoption-osxphotos-add-locations-selected"],
+            [0, "cmdoption-osxphotos-add-locations-selfie"],
+            [0, "cmdoption-osxphotos-add-locations-shared"],
+            [0, "cmdoption-osxphotos-add-locations-slow-mo"],
+            [0, "cmdoption-osxphotos-add-locations-theme"],
+            [0, "cmdoption-osxphotos-add-locations-time-lapse"],
+            [0, "cmdoption-osxphotos-add-locations-timestamp"],
+            [0, "cmdoption-osxphotos-add-locations-title"],
+            [0, "cmdoption-osxphotos-add-locations-to-date"],
+            [0, "cmdoption-osxphotos-add-locations-to-time"],
+            [0, "cmdoption-osxphotos-add-locations-uti"],
+            [0, "cmdoption-osxphotos-add-locations-uuid"],
+            [0, "cmdoption-osxphotos-add-locations-uuid-from-file"],
+            [0, "cmdoption-osxphotos-add-locations-w"],
+            [0, "cmdoption-osxphotos-add-locations-year"]
+        ],
+        "osxphotos-albums command line option": [
+            [0, "cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-albums-json"],
+            [0, "cmdoption-osxphotos-albums-library"]
+        ],
+        "osxphotos-batch-edit command line option": [
+            [0, "cmdoption-osxphotos-batch-edit-V"],
+            [0, "cmdoption-osxphotos-batch-edit-description"],
+            [0, "cmdoption-osxphotos-batch-edit-dry-run"],
+            [0, "cmdoption-osxphotos-batch-edit-keyword"],
+            [0, "cmdoption-osxphotos-batch-edit-library"],
+            [0, "cmdoption-osxphotos-batch-edit-location"],
+            [0, "cmdoption-osxphotos-batch-edit-replace-keywords"],
+            [0, "cmdoption-osxphotos-batch-edit-theme"],
+            [0, "cmdoption-osxphotos-batch-edit-timestamp"],
+            [0, "cmdoption-osxphotos-batch-edit-title"],
+            [0, "cmdoption-osxphotos-batch-edit-undo"]
+        ],
+        "osxphotos-diff command line option": [
+            [0, "cmdoption-osxphotos-diff-V"],
+            [0, "cmdoption-osxphotos-diff-arg-DB2"],
+            [0, "cmdoption-osxphotos-diff-library"],
+            [0, "cmdoption-osxphotos-diff-r"],
+            [0, "cmdoption-osxphotos-diff-s"],
+            [0, "cmdoption-osxphotos-diff-timestamp"]
+        ],
+        "osxphotos-dump command line option": [
+            [0, "cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-dump-deleted"],
+            [0, "cmdoption-osxphotos-dump-deleted-only"],
+            [0, "cmdoption-osxphotos-dump-f"],
+            [0, "cmdoption-osxphotos-dump-json"],
+            [0, "cmdoption-osxphotos-dump-library"],
+            [0, "cmdoption-osxphotos-dump-print"]
+        ],
+        "osxphotos-exiftool command line option": [
+            [0, "cmdoption-osxphotos-exiftool-V"],
+            [0, "cmdoption-osxphotos-exiftool-album-keyword"],
+            [0, "cmdoption-osxphotos-exiftool-append"],
+            [0, "cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY"],
+            [0, "cmdoption-osxphotos-exiftool-db-config"],
+            [0, "cmdoption-osxphotos-exiftool-description-template"],
+            [0, "cmdoption-osxphotos-exiftool-dry-run"],
+            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-keywords"],
+            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-persons"],
+            [0, "cmdoption-osxphotos-exiftool-exiftool-option"],
+            [0, "cmdoption-osxphotos-exiftool-exiftool-path"],
+            [0, "cmdoption-osxphotos-exiftool-exportdb"],
+            [0, "cmdoption-osxphotos-exiftool-ignore-date-modified"],
+            [0, "cmdoption-osxphotos-exiftool-keyword-template"],
+            [0, "cmdoption-osxphotos-exiftool-library"],
+            [0, "cmdoption-osxphotos-exiftool-load-config"],
+            [0, "cmdoption-osxphotos-exiftool-person-keyword"],
+            [0, "cmdoption-osxphotos-exiftool-replace-keywords"],
+            [0, "cmdoption-osxphotos-exiftool-report"],
+            [0, "cmdoption-osxphotos-exiftool-save-config"],
+            [0, "cmdoption-osxphotos-exiftool-theme"],
+            [0, "cmdoption-osxphotos-exiftool-timestamp"]
+        ],
+        "osxphotos-export command line option": [
+            [0, "cmdoption-osxphotos-export-V"],
+            [0, "cmdoption-osxphotos-export-add-exported-to-album"],
+            [0, "cmdoption-osxphotos-export-add-missing-to-album"],
+            [0, "cmdoption-osxphotos-export-add-skipped-to-album"],
+            [0, "cmdoption-osxphotos-export-added-after"],
+            [0, "cmdoption-osxphotos-export-added-before"],
+            [0, "cmdoption-osxphotos-export-added-in-last"],
+            [0, "cmdoption-osxphotos-export-album"],
+            [0, "cmdoption-osxphotos-export-album-keyword"],
+            [0, "cmdoption-osxphotos-export-alt-copy"],
+            [0, "cmdoption-osxphotos-export-append"],
+            [0, "cmdoption-osxphotos-export-arg-DEST"],
+            [0, "cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-export-burst"],
+            [0, "cmdoption-osxphotos-export-cleanup"],
+            [0, "cmdoption-osxphotos-export-cloudasset"],
+            [0, "cmdoption-osxphotos-export-config-only"],
+            [0, "cmdoption-osxphotos-export-convert-to-jpeg"],
+            [0, "cmdoption-osxphotos-export-current-name"],
+            [0, "cmdoption-osxphotos-export-deleted"],
+            [0, "cmdoption-osxphotos-export-deleted-only"],
+            [0, "cmdoption-osxphotos-export-description"],
+            [0, "cmdoption-osxphotos-export-description-template"],
+            [0, "cmdoption-osxphotos-export-directory"],
+            [0, "cmdoption-osxphotos-export-download-missing"],
+            [0, "cmdoption-osxphotos-export-dry-run"],
+            [0, "cmdoption-osxphotos-export-duplicate"],
+            [0, "cmdoption-osxphotos-export-edited"],
+            [0, "cmdoption-osxphotos-export-edited-suffix"],
+            [0, "cmdoption-osxphotos-export-exif"],
+            [0, "cmdoption-osxphotos-export-exiftool"],
+            [0, "cmdoption-osxphotos-export-exiftool-merge-keywords"],
+            [0, "cmdoption-osxphotos-export-exiftool-merge-persons"],
+            [0, "cmdoption-osxphotos-export-exiftool-option"],
+            [0, "cmdoption-osxphotos-export-exiftool-path"],
+            [0, "cmdoption-osxphotos-export-export-as-hardlink"],
+            [0, "cmdoption-osxphotos-export-export-by-date"],
+            [0, "cmdoption-osxphotos-export-exportdb"],
+            [0, "cmdoption-osxphotos-export-external-edit"],
+            [0, "cmdoption-osxphotos-export-favorite"],
+            [0, "cmdoption-osxphotos-export-favorite-rating"],
+            [0, "cmdoption-osxphotos-export-filename"],
+            [0, "cmdoption-osxphotos-export-finder-tag-keywords"],
+            [0, "cmdoption-osxphotos-export-finder-tag-template"],
+            [0, "cmdoption-osxphotos-export-folder"],
+            [0, "cmdoption-osxphotos-export-force-update"],
+            [0, "cmdoption-osxphotos-export-from-date"],
+            [0, "cmdoption-osxphotos-export-from-time"],
+            [0, "cmdoption-osxphotos-export-has-comment"],
+            [0, "cmdoption-osxphotos-export-has-likes"],
+            [0, "cmdoption-osxphotos-export-has-raw"],
+            [0, "cmdoption-osxphotos-export-hdr"],
+            [0, "cmdoption-osxphotos-export-hidden"],
+            [0, "cmdoption-osxphotos-export-i"],
+            [0, "cmdoption-osxphotos-export-ignore-date-modified"],
+            [0, "cmdoption-osxphotos-export-ignore-signature"],
+            [0, "cmdoption-osxphotos-export-in-album"],
+            [0, "cmdoption-osxphotos-export-incloud"],
+            [0, "cmdoption-osxphotos-export-is-reference"],
+            [0, "cmdoption-osxphotos-export-jpeg-ext"],
+            [0, "cmdoption-osxphotos-export-jpeg-quality"],
+            [0, "cmdoption-osxphotos-export-keep"],
+            [0, "cmdoption-osxphotos-export-keyword"],
+            [0, "cmdoption-osxphotos-export-keyword-template"],
+            [0, "cmdoption-osxphotos-export-label"],
+            [0, "cmdoption-osxphotos-export-library"],
+            [0, "cmdoption-osxphotos-export-limit"],
+            [0, "cmdoption-osxphotos-export-live"],
+            [0, "cmdoption-osxphotos-export-load-config"],
+            [0, "cmdoption-osxphotos-export-location"],
+            [0, "cmdoption-osxphotos-export-max-size"],
+            [0, "cmdoption-osxphotos-export-min-size"],
+            [0, "cmdoption-osxphotos-export-missing"],
+            [0, "cmdoption-osxphotos-export-name"],
+            [0, "cmdoption-osxphotos-export-no-comment"],
+            [0, "cmdoption-osxphotos-export-no-description"],
+            [0, "cmdoption-osxphotos-export-no-keyword"],
+            [0, "cmdoption-osxphotos-export-no-likes"],
+            [0, "cmdoption-osxphotos-export-no-location"],
+            [0, "cmdoption-osxphotos-export-no-place"],
+            [0, "cmdoption-osxphotos-export-no-progress"],
+            [0, "cmdoption-osxphotos-export-no-title"],
+            [0, "cmdoption-osxphotos-export-not-burst"],
+            [0, "cmdoption-osxphotos-export-not-cloudasset"],
+            [0, "cmdoption-osxphotos-export-not-edited"],
+            [0, "cmdoption-osxphotos-export-not-favorite"],
+            [0, "cmdoption-osxphotos-export-not-hdr"],
+            [0, "cmdoption-osxphotos-export-not-hidden"],
+            [0, "cmdoption-osxphotos-export-not-in-album"],
+            [0, "cmdoption-osxphotos-export-not-incloud"],
+            [0, "cmdoption-osxphotos-export-not-live"],
+            [0, "cmdoption-osxphotos-export-not-missing"],
+            [0, "cmdoption-osxphotos-export-not-panorama"],
+            [0, "cmdoption-osxphotos-export-not-portrait"],
+            [0, "cmdoption-osxphotos-export-not-reference"],
+            [0, "cmdoption-osxphotos-export-not-screenshot"],
+            [0, "cmdoption-osxphotos-export-not-selfie"],
+            [0, "cmdoption-osxphotos-export-not-shared"],
+            [0, "cmdoption-osxphotos-export-not-slow-mo"],
+            [0, "cmdoption-osxphotos-export-not-time-lapse"],
+            [0, "cmdoption-osxphotos-export-only-movies"],
+            [0, "cmdoption-osxphotos-export-only-new"],
+            [0, "cmdoption-osxphotos-export-only-photos"],
+            [0, "cmdoption-osxphotos-export-original-suffix"],
+            [0, "cmdoption-osxphotos-export-overwrite"],
+            [0, "cmdoption-osxphotos-export-panorama"],
+            [0, "cmdoption-osxphotos-export-person"],
+            [0, "cmdoption-osxphotos-export-person-keyword"],
+            [0, "cmdoption-osxphotos-export-place"],
+            [0, "cmdoption-osxphotos-export-portrait"],
+            [0, "cmdoption-osxphotos-export-post-command"],
+            [0, "cmdoption-osxphotos-export-post-function"],
+            [0, "cmdoption-osxphotos-export-preview"],
+            [0, "cmdoption-osxphotos-export-preview-if-missing"],
+            [0, "cmdoption-osxphotos-export-preview-suffix"],
+            [0, "cmdoption-osxphotos-export-print"],
+            [0, "cmdoption-osxphotos-export-query-eval"],
+            [0, "cmdoption-osxphotos-export-query-function"],
+            [0, "cmdoption-osxphotos-export-ramdb"],
+            [0, "cmdoption-osxphotos-export-regex"],
+            [0, "cmdoption-osxphotos-export-replace-keywords"],
+            [0, "cmdoption-osxphotos-export-report"],
+            [0, "cmdoption-osxphotos-export-retry"],
+            [0, "cmdoption-osxphotos-export-save-config"],
+            [0, "cmdoption-osxphotos-export-screenshot"],
+            [0, "cmdoption-osxphotos-export-selected"],
+            [0, "cmdoption-osxphotos-export-selfie"],
+            [0, "cmdoption-osxphotos-export-shared"],
+            [0, "cmdoption-osxphotos-export-sidecar"],
+            [0, "cmdoption-osxphotos-export-sidecar-drop-ext"],
+            [0, "cmdoption-osxphotos-export-skip-bursts"],
+            [0, "cmdoption-osxphotos-export-skip-edited"],
+            [0, "cmdoption-osxphotos-export-skip-live"],
+            [0, "cmdoption-osxphotos-export-skip-original-if-edited"],
+            [0, "cmdoption-osxphotos-export-skip-raw"],
+            [0, "cmdoption-osxphotos-export-skip-uuid"],
+            [0, "cmdoption-osxphotos-export-skip-uuid-from-file"],
+            [0, "cmdoption-osxphotos-export-slow-mo"],
+            [0, "cmdoption-osxphotos-export-strip"],
+            [0, "cmdoption-osxphotos-export-theme"],
+            [0, "cmdoption-osxphotos-export-time-lapse"],
+            [0, "cmdoption-osxphotos-export-timestamp"],
+            [0, "cmdoption-osxphotos-export-title"],
+            [0, "cmdoption-osxphotos-export-tmpdir"],
+            [0, "cmdoption-osxphotos-export-to-date"],
+            [0, "cmdoption-osxphotos-export-to-time"],
+            [0, "cmdoption-osxphotos-export-touch-file"],
+            [0, "cmdoption-osxphotos-export-update"],
+            [0, "cmdoption-osxphotos-export-update-errors"],
+            [0, "cmdoption-osxphotos-export-use-photokit"],
+            [0, "cmdoption-osxphotos-export-use-photos-export"],
+            [0, "cmdoption-osxphotos-export-uti"],
+            [0, "cmdoption-osxphotos-export-uuid"],
+            [0, "cmdoption-osxphotos-export-uuid-from-file"],
+            [0, "cmdoption-osxphotos-export-xattr-template"],
+            [0, "cmdoption-osxphotos-export-year"]
+        ],
+        "osxphotos-exportdb command line option": [
+            [0, "cmdoption-osxphotos-exportdb-V"],
+            [0, "cmdoption-osxphotos-exportdb-append"],
+            [0, "cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE"],
+            [0, "cmdoption-osxphotos-exportdb-check-signatures"],
+            [0, "cmdoption-osxphotos-exportdb-delete-file"],
+            [0, "cmdoption-osxphotos-exportdb-delete-uuid"],
+            [0, "cmdoption-osxphotos-exportdb-dry-run"],
+            [0, "cmdoption-osxphotos-exportdb-errors"],
+            [0, "cmdoption-osxphotos-exportdb-export-dir"],
+            [0, "cmdoption-osxphotos-exportdb-info"],
+            [0, "cmdoption-osxphotos-exportdb-last-errors"],
+            [0, "cmdoption-osxphotos-exportdb-last-run"],
+            [0, "cmdoption-osxphotos-exportdb-migrate"],
+            [0, "cmdoption-osxphotos-exportdb-migrate-photos-library"],
+            [0, "cmdoption-osxphotos-exportdb-report"],
+            [0, "cmdoption-osxphotos-exportdb-save-config"],
+            [0, "cmdoption-osxphotos-exportdb-sql"],
+            [0, "cmdoption-osxphotos-exportdb-theme"],
+            [0, "cmdoption-osxphotos-exportdb-timestamp"],
+            [0, "cmdoption-osxphotos-exportdb-touch-file"],
+            [0, "cmdoption-osxphotos-exportdb-update-signatures"],
+            [0, "cmdoption-osxphotos-exportdb-uuid-files"],
+            [0, "cmdoption-osxphotos-exportdb-uuid-info"],
+            [0, "cmdoption-osxphotos-exportdb-vacuum"],
+            [0, "cmdoption-osxphotos-exportdb-version"]
+        ],
+        "osxphotos-help command line option": [
+            [0, "cmdoption-osxphotos-help-arg-SUBTOPIC"],
+            [0, "cmdoption-osxphotos-help-arg-TOPIC"]
+        ],
+        "osxphotos-import command line option": [
+            [0, "cmdoption-osxphotos-import-0"],
+            [0, "cmdoption-osxphotos-import-C"],
+            [0, "cmdoption-osxphotos-import-D"],
+            [0, "cmdoption-osxphotos-import-L"],
+            [0, "cmdoption-osxphotos-import-P"],
+            [0, "cmdoption-osxphotos-import-R"],
+            [0, "cmdoption-osxphotos-import-V"],
+            [0, "cmdoption-osxphotos-import-a"],
+            [0, "cmdoption-osxphotos-import-append"],
+            [0, "cmdoption-osxphotos-import-arg-FILES"],
+            [0, "cmdoption-osxphotos-import-check-templates"],
+            [0, "cmdoption-osxphotos-import-d"],
+            [0, "cmdoption-osxphotos-import-e"],
+            [0, "cmdoption-osxphotos-import-f"],
+            [0, "cmdoption-osxphotos-import-g"],
+            [0, "cmdoption-osxphotos-import-k"],
+            [0, "cmdoption-osxphotos-import-l"],
+            [0, "cmdoption-osxphotos-import-m"],
+            [0, "cmdoption-osxphotos-import-no-progress"],
+            [0, "cmdoption-osxphotos-import-post-function"],
+            [0, "cmdoption-osxphotos-import-r"],
+            [0, "cmdoption-osxphotos-import-report"],
+            [0, "cmdoption-osxphotos-import-t"],
+            [0, "cmdoption-osxphotos-import-theme"],
+            [0, "cmdoption-osxphotos-import-timestamp"],
+            [0, "cmdoption-osxphotos-import-w"]
+        ],
+        "osxphotos-info command line option": [
+            [0, "cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-info-json"],
+            [0, "cmdoption-osxphotos-info-library"]
+        ],
+        "osxphotos-inspect command line option": [
+            [0, "cmdoption-osxphotos-inspect-T"],
+            [0, "cmdoption-osxphotos-inspect-library"],
+            [0, "cmdoption-osxphotos-inspect-t"],
+            [0, "cmdoption-osxphotos-inspect-theme"]
+        ],
+        "osxphotos-install command line option": [
+            [0, "cmdoption-osxphotos-install-U"],
+            [0, "cmdoption-osxphotos-install-arg-PACKAGES"]
+        ],
+        "osxphotos-keywords command line option": [
+            [0, "cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-keywords-json"],
+            [0, "cmdoption-osxphotos-keywords-library"]
+        ],
+        "osxphotos-labels command line option": [
+            [0, "cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-labels-json"],
+            [0, "cmdoption-osxphotos-labels-library"]
+        ],
+        "osxphotos-list command line option": [
+            [0, "cmdoption-osxphotos-list-json"]
+        ],
+        "osxphotos-orphans command line option": [
+            [0, "cmdoption-osxphotos-orphans-V"],
+            [0, "cmdoption-osxphotos-orphans-export"],
+            [0, "cmdoption-osxphotos-orphans-library"],
+            [0, "cmdoption-osxphotos-orphans-theme"],
+            [0, "cmdoption-osxphotos-orphans-timestamp"]
+        ],
+        "osxphotos-persons command line option": [
+            [0, "cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-persons-json"],
+            [0, "cmdoption-osxphotos-persons-library"]
+        ],
+        "osxphotos-places command line option": [
+            [0, "cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-places-json"],
+            [0, "cmdoption-osxphotos-places-library"]
+        ],
+        "osxphotos-query command line option": [
+            [0, "cmdoption-osxphotos-query-add-to-album"],
+            [0, "cmdoption-osxphotos-query-added-after"],
+            [0, "cmdoption-osxphotos-query-added-before"],
+            [0, "cmdoption-osxphotos-query-added-in-last"],
+            [0, "cmdoption-osxphotos-query-album"],
+            [0, "cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-query-burst"],
+            [0, "cmdoption-osxphotos-query-cloudasset"],
+            [0, "cmdoption-osxphotos-query-deleted"],
+            [0, "cmdoption-osxphotos-query-deleted-only"],
+            [0, "cmdoption-osxphotos-query-description"],
+            [0, "cmdoption-osxphotos-query-duplicate"],
+            [0, "cmdoption-osxphotos-query-edited"],
+            [0, "cmdoption-osxphotos-query-exif"],
+            [0, "cmdoption-osxphotos-query-external-edit"],
+            [0, "cmdoption-osxphotos-query-f"],
+            [0, "cmdoption-osxphotos-query-favorite"],
+            [0, "cmdoption-osxphotos-query-folder"],
+            [0, "cmdoption-osxphotos-query-from-date"],
+            [0, "cmdoption-osxphotos-query-from-time"],
+            [0, "cmdoption-osxphotos-query-has-comment"],
+            [0, "cmdoption-osxphotos-query-has-likes"],
+            [0, "cmdoption-osxphotos-query-has-raw"],
+            [0, "cmdoption-osxphotos-query-hdr"],
+            [0, "cmdoption-osxphotos-query-hidden"],
+            [0, "cmdoption-osxphotos-query-i"],
+            [0, "cmdoption-osxphotos-query-in-album"],
+            [0, "cmdoption-osxphotos-query-incloud"],
+            [0, "cmdoption-osxphotos-query-is-reference"],
+            [0, "cmdoption-osxphotos-query-json"],
+            [0, "cmdoption-osxphotos-query-keyword"],
+            [0, "cmdoption-osxphotos-query-label"],
+            [0, "cmdoption-osxphotos-query-library"],
+            [0, "cmdoption-osxphotos-query-live"],
+            [0, "cmdoption-osxphotos-query-location"],
+            [0, "cmdoption-osxphotos-query-max-size"],
+            [0, "cmdoption-osxphotos-query-min-size"],
+            [0, "cmdoption-osxphotos-query-missing"],
+            [0, "cmdoption-osxphotos-query-name"],
+            [0, "cmdoption-osxphotos-query-no-comment"],
+            [0, "cmdoption-osxphotos-query-no-description"],
+            [0, "cmdoption-osxphotos-query-no-keyword"],
+            [0, "cmdoption-osxphotos-query-no-likes"],
+            [0, "cmdoption-osxphotos-query-no-location"],
+            [0, "cmdoption-osxphotos-query-no-place"],
+            [0, "cmdoption-osxphotos-query-no-title"],
+            [0, "cmdoption-osxphotos-query-not-burst"],
+            [0, "cmdoption-osxphotos-query-not-cloudasset"],
+            [0, "cmdoption-osxphotos-query-not-edited"],
+            [0, "cmdoption-osxphotos-query-not-favorite"],
+            [0, "cmdoption-osxphotos-query-not-hdr"],
+            [0, "cmdoption-osxphotos-query-not-hidden"],
+            [0, "cmdoption-osxphotos-query-not-in-album"],
+            [0, "cmdoption-osxphotos-query-not-incloud"],
+            [0, "cmdoption-osxphotos-query-not-live"],
+            [0, "cmdoption-osxphotos-query-not-missing"],
+            [0, "cmdoption-osxphotos-query-not-panorama"],
+            [0, "cmdoption-osxphotos-query-not-portrait"],
+            [0, "cmdoption-osxphotos-query-not-reference"],
+            [0, "cmdoption-osxphotos-query-not-screenshot"],
+            [0, "cmdoption-osxphotos-query-not-selfie"],
+            [0, "cmdoption-osxphotos-query-not-shared"],
+            [0, "cmdoption-osxphotos-query-not-slow-mo"],
+            [0, "cmdoption-osxphotos-query-not-time-lapse"],
+            [0, "cmdoption-osxphotos-query-only-movies"],
+            [0, "cmdoption-osxphotos-query-only-photos"],
+            [0, "cmdoption-osxphotos-query-panorama"],
+            [0, "cmdoption-osxphotos-query-person"],
+            [0, "cmdoption-osxphotos-query-place"],
+            [0, "cmdoption-osxphotos-query-portrait"],
+            [0, "cmdoption-osxphotos-query-print"],
+            [0, "cmdoption-osxphotos-query-query-eval"],
+            [0, "cmdoption-osxphotos-query-query-function"],
+            [0, "cmdoption-osxphotos-query-quiet"],
+            [0, "cmdoption-osxphotos-query-regex"],
+            [0, "cmdoption-osxphotos-query-screenshot"],
+            [0, "cmdoption-osxphotos-query-selected"],
+            [0, "cmdoption-osxphotos-query-selfie"],
+            [0, "cmdoption-osxphotos-query-shared"],
+            [0, "cmdoption-osxphotos-query-slow-mo"],
+            [0, "cmdoption-osxphotos-query-time-lapse"],
+            [0, "cmdoption-osxphotos-query-title"],
+            [0, "cmdoption-osxphotos-query-to-date"],
+            [0, "cmdoption-osxphotos-query-to-time"],
+            [0, "cmdoption-osxphotos-query-uti"],
+            [0, "cmdoption-osxphotos-query-uuid"],
+            [0, "cmdoption-osxphotos-query-uuid-from-file"],
+            [0, "cmdoption-osxphotos-query-year"]
+        ],
+        "osxphotos-repl command line option": [
+            [0, "cmdoption-osxphotos-repl-added-after"],
+            [0, "cmdoption-osxphotos-repl-added-before"],
+            [0, "cmdoption-osxphotos-repl-added-in-last"],
+            [0, "cmdoption-osxphotos-repl-album"],
+            [0, "cmdoption-osxphotos-repl-burst"],
+            [0, "cmdoption-osxphotos-repl-cloudasset"],
+            [0, "cmdoption-osxphotos-repl-deleted"],
+            [0, "cmdoption-osxphotos-repl-deleted-only"],
+            [0, "cmdoption-osxphotos-repl-description"],
+            [0, "cmdoption-osxphotos-repl-duplicate"],
+            [0, "cmdoption-osxphotos-repl-edited"],
+            [0, "cmdoption-osxphotos-repl-emacs"],
+            [0, "cmdoption-osxphotos-repl-exif"],
+            [0, "cmdoption-osxphotos-repl-external-edit"],
+            [0, "cmdoption-osxphotos-repl-favorite"],
+            [0, "cmdoption-osxphotos-repl-folder"],
+            [0, "cmdoption-osxphotos-repl-from-date"],
+            [0, "cmdoption-osxphotos-repl-from-time"],
+            [0, "cmdoption-osxphotos-repl-has-comment"],
+            [0, "cmdoption-osxphotos-repl-has-likes"],
+            [0, "cmdoption-osxphotos-repl-has-raw"],
+            [0, "cmdoption-osxphotos-repl-hdr"],
+            [0, "cmdoption-osxphotos-repl-hidden"],
+            [0, "cmdoption-osxphotos-repl-i"],
+            [0, "cmdoption-osxphotos-repl-in-album"],
+            [0, "cmdoption-osxphotos-repl-incloud"],
+            [0, "cmdoption-osxphotos-repl-is-reference"],
+            [0, "cmdoption-osxphotos-repl-keyword"],
+            [0, "cmdoption-osxphotos-repl-label"],
+            [0, "cmdoption-osxphotos-repl-library"],
+            [0, "cmdoption-osxphotos-repl-live"],
+            [0, "cmdoption-osxphotos-repl-location"],
+            [0, "cmdoption-osxphotos-repl-max-size"],
+            [0, "cmdoption-osxphotos-repl-min-size"],
+            [0, "cmdoption-osxphotos-repl-missing"],
+            [0, "cmdoption-osxphotos-repl-name"],
+            [0, "cmdoption-osxphotos-repl-no-comment"],
+            [0, "cmdoption-osxphotos-repl-no-description"],
+            [0, "cmdoption-osxphotos-repl-no-keyword"],
+            [0, "cmdoption-osxphotos-repl-no-likes"],
+            [0, "cmdoption-osxphotos-repl-no-location"],
+            [0, "cmdoption-osxphotos-repl-no-place"],
+            [0, "cmdoption-osxphotos-repl-no-title"],
+            [0, "cmdoption-osxphotos-repl-not-burst"],
+            [0, "cmdoption-osxphotos-repl-not-cloudasset"],
+            [0, "cmdoption-osxphotos-repl-not-edited"],
+            [0, "cmdoption-osxphotos-repl-not-favorite"],
+            [0, "cmdoption-osxphotos-repl-not-hdr"],
+            [0, "cmdoption-osxphotos-repl-not-hidden"],
+            [0, "cmdoption-osxphotos-repl-not-in-album"],
+            [0, "cmdoption-osxphotos-repl-not-incloud"],
+            [0, "cmdoption-osxphotos-repl-not-live"],
+            [0, "cmdoption-osxphotos-repl-not-missing"],
+            [0, "cmdoption-osxphotos-repl-not-panorama"],
+            [0, "cmdoption-osxphotos-repl-not-portrait"],
+            [0, "cmdoption-osxphotos-repl-not-reference"],
+            [0, "cmdoption-osxphotos-repl-not-screenshot"],
+            [0, "cmdoption-osxphotos-repl-not-selfie"],
+            [0, "cmdoption-osxphotos-repl-not-shared"],
+            [0, "cmdoption-osxphotos-repl-not-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-not-time-lapse"],
+            [0, "cmdoption-osxphotos-repl-only-movies"],
+            [0, "cmdoption-osxphotos-repl-only-photos"],
+            [0, "cmdoption-osxphotos-repl-panorama"],
+            [0, "cmdoption-osxphotos-repl-person"],
+            [0, "cmdoption-osxphotos-repl-place"],
+            [0, "cmdoption-osxphotos-repl-portrait"],
+            [0, "cmdoption-osxphotos-repl-query-eval"],
+            [0, "cmdoption-osxphotos-repl-query-function"],
+            [0, "cmdoption-osxphotos-repl-regex"],
+            [0, "cmdoption-osxphotos-repl-screenshot"],
+            [0, "cmdoption-osxphotos-repl-selected"],
+            [0, "cmdoption-osxphotos-repl-selfie"],
+            [0, "cmdoption-osxphotos-repl-shared"],
+            [0, "cmdoption-osxphotos-repl-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-time-lapse"],
+            [0, "cmdoption-osxphotos-repl-title"],
+            [0, "cmdoption-osxphotos-repl-to-date"],
+            [0, "cmdoption-osxphotos-repl-to-time"],
+            [0, "cmdoption-osxphotos-repl-uti"],
+            [0, "cmdoption-osxphotos-repl-uuid"],
+            [0, "cmdoption-osxphotos-repl-uuid-from-file"],
+            [0, "cmdoption-osxphotos-repl-year"]
+        ],
+        "osxphotos-run command line option": [
+            [0, "cmdoption-osxphotos-run-arg-ARGS"],
+            [0, "cmdoption-osxphotos-run-arg-PYTHON_FILE"],
+            [0, "cmdoption-osxphotos-run-h"]
+        ],
+        "osxphotos-show command line option": [
+            [0, "cmdoption-osxphotos-show-arg-UUID_OR_NAME"],
+            [0, "cmdoption-osxphotos-show-library"]
+        ],
+        "osxphotos-snap command line option": [
+            [0, "cmdoption-osxphotos-snap-library"]
+        ],
+        "osxphotos-sync command line option": [
+            [0, "cmdoption-osxphotos-sync-0"],
+            [0, "cmdoption-osxphotos-sync-A"],
+            [0, "cmdoption-osxphotos-sync-R"],
+            [0, "cmdoption-osxphotos-sync-U"],
+            [0, "cmdoption-osxphotos-sync-V"],
+            [0, "cmdoption-osxphotos-sync-added-after"],
+            [0, "cmdoption-osxphotos-sync-added-before"],
+            [0, "cmdoption-osxphotos-sync-added-in-last"],
+            [0, "cmdoption-osxphotos-sync-album"],
+            [0, "cmdoption-osxphotos-sync-burst"],
+            [0, "cmdoption-osxphotos-sync-cloudasset"],
+            [0, "cmdoption-osxphotos-sync-description"],
+            [0, "cmdoption-osxphotos-sync-dry-run"],
+            [0, "cmdoption-osxphotos-sync-duplicate"],
+            [0, "cmdoption-osxphotos-sync-e"],
+            [0, "cmdoption-osxphotos-sync-edited"],
+            [0, "cmdoption-osxphotos-sync-exif"],
+            [0, "cmdoption-osxphotos-sync-external-edit"],
+            [0, "cmdoption-osxphotos-sync-favorite"],
+            [0, "cmdoption-osxphotos-sync-folder"],
+            [0, "cmdoption-osxphotos-sync-from-date"],
+            [0, "cmdoption-osxphotos-sync-from-time"],
+            [0, "cmdoption-osxphotos-sync-has-comment"],
+            [0, "cmdoption-osxphotos-sync-has-likes"],
+            [0, "cmdoption-osxphotos-sync-has-raw"],
+            [0, "cmdoption-osxphotos-sync-hdr"],
+            [0, "cmdoption-osxphotos-sync-hidden"],
+            [0, "cmdoption-osxphotos-sync-i"],
+            [0, "cmdoption-osxphotos-sync-in-album"],
+            [0, "cmdoption-osxphotos-sync-incloud"],
+            [0, "cmdoption-osxphotos-sync-is-reference"],
+            [0, "cmdoption-osxphotos-sync-keyword"],
+            [0, "cmdoption-osxphotos-sync-label"],
+            [0, "cmdoption-osxphotos-sync-library"],
+            [0, "cmdoption-osxphotos-sync-live"],
+            [0, "cmdoption-osxphotos-sync-location"],
+            [0, "cmdoption-osxphotos-sync-m"],
+            [0, "cmdoption-osxphotos-sync-max-size"],
+            [0, "cmdoption-osxphotos-sync-min-size"],
+            [0, "cmdoption-osxphotos-sync-missing"],
+            [0, "cmdoption-osxphotos-sync-name"],
+            [0, "cmdoption-osxphotos-sync-no-comment"],
+            [0, "cmdoption-osxphotos-sync-no-description"],
+            [0, "cmdoption-osxphotos-sync-no-keyword"],
+            [0, "cmdoption-osxphotos-sync-no-likes"],
+            [0, "cmdoption-osxphotos-sync-no-location"],
+            [0, "cmdoption-osxphotos-sync-no-place"],
+            [0, "cmdoption-osxphotos-sync-no-title"],
+            [0, "cmdoption-osxphotos-sync-not-burst"],
+            [0, "cmdoption-osxphotos-sync-not-cloudasset"],
+            [0, "cmdoption-osxphotos-sync-not-edited"],
+            [0, "cmdoption-osxphotos-sync-not-favorite"],
+            [0, "cmdoption-osxphotos-sync-not-hdr"],
+            [0, "cmdoption-osxphotos-sync-not-hidden"],
+            [0, "cmdoption-osxphotos-sync-not-in-album"],
+            [0, "cmdoption-osxphotos-sync-not-incloud"],
+            [0, "cmdoption-osxphotos-sync-not-live"],
+            [0, "cmdoption-osxphotos-sync-not-missing"],
+            [0, "cmdoption-osxphotos-sync-not-panorama"],
+            [0, "cmdoption-osxphotos-sync-not-portrait"],
+            [0, "cmdoption-osxphotos-sync-not-reference"],
+            [0, "cmdoption-osxphotos-sync-not-screenshot"],
+            [0, "cmdoption-osxphotos-sync-not-selfie"],
+            [0, "cmdoption-osxphotos-sync-not-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-not-time-lapse"],
+            [0, "cmdoption-osxphotos-sync-only-movies"],
+            [0, "cmdoption-osxphotos-sync-only-photos"],
+            [0, "cmdoption-osxphotos-sync-panorama"],
+            [0, "cmdoption-osxphotos-sync-person"],
+            [0, "cmdoption-osxphotos-sync-place"],
+            [0, "cmdoption-osxphotos-sync-portrait"],
+            [0, "cmdoption-osxphotos-sync-query-eval"],
+            [0, "cmdoption-osxphotos-sync-query-function"],
+            [0, "cmdoption-osxphotos-sync-regex"],
+            [0, "cmdoption-osxphotos-sync-s"],
+            [0, "cmdoption-osxphotos-sync-screenshot"],
+            [0, "cmdoption-osxphotos-sync-selected"],
+            [0, "cmdoption-osxphotos-sync-selfie"],
+            [0, "cmdoption-osxphotos-sync-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-theme"],
+            [0, "cmdoption-osxphotos-sync-time-lapse"],
+            [0, "cmdoption-osxphotos-sync-timestamp"],
+            [0, "cmdoption-osxphotos-sync-title"],
+            [0, "cmdoption-osxphotos-sync-to-date"],
+            [0, "cmdoption-osxphotos-sync-to-time"],
+            [0, "cmdoption-osxphotos-sync-uti"],
+            [0, "cmdoption-osxphotos-sync-uuid"],
+            [0, "cmdoption-osxphotos-sync-uuid-from-file"],
+            [0, "cmdoption-osxphotos-sync-year"]
+        ],
+        "osxphotos-theme command line option": [
+            [0, "cmdoption-osxphotos-theme-clone"],
+            [0, "cmdoption-osxphotos-theme-config"],
+            [0, "cmdoption-osxphotos-theme-default"],
+            [0, "cmdoption-osxphotos-theme-delete"],
+            [0, "cmdoption-osxphotos-theme-edit"],
+            [0, "cmdoption-osxphotos-theme-list"],
+            [0, "cmdoption-osxphotos-theme-preview"]
+        ],
+        "osxphotos-timewarp command line option": [
+            [0, "cmdoption-osxphotos-timewarp-0"],
+            [0, "cmdoption-osxphotos-timewarp-1"],
+            [0, "cmdoption-osxphotos-timewarp-2"],
+            [0, "cmdoption-osxphotos-timewarp-D"],
+            [0, "cmdoption-osxphotos-timewarp-F"],
+            [0, "cmdoption-osxphotos-timewarp-L"],
+            [0, "cmdoption-osxphotos-timewarp-M"],
+            [0, "cmdoption-osxphotos-timewarp-P"],
+            [0, "cmdoption-osxphotos-timewarp-T"],
+            [0, "cmdoption-osxphotos-timewarp-V"],
+            [0, "cmdoption-osxphotos-timewarp-a"],
+            [0, "cmdoption-osxphotos-timewarp-c"],
+            [0, "cmdoption-osxphotos-timewarp-d"],
+            [0, "cmdoption-osxphotos-timewarp-date-added"],
+            [0, "cmdoption-osxphotos-timewarp-date-added-from-photo"],
+            [0, "cmdoption-osxphotos-timewarp-e"],
+            [0, "cmdoption-osxphotos-timewarp-force"],
+            [0, "cmdoption-osxphotos-timewarp-i"],
+            [0, "cmdoption-osxphotos-timewarp-p"],
+            [0, "cmdoption-osxphotos-timewarp-plain"],
+            [0, "cmdoption-osxphotos-timewarp-t"],
+            [0, "cmdoption-osxphotos-timewarp-theme"],
+            [0, "cmdoption-osxphotos-timewarp-timestamp"],
+            [0, "cmdoption-osxphotos-timewarp-z"]
+        ],
+        "osxphotos-tutorial command line option": [
+            [0, "cmdoption-osxphotos-tutorial-arg-WIDTH"]
+        ],
+        "osxphotos-uninstall command line option": [
+            [0, "cmdoption-osxphotos-uninstall-arg-PACKAGES"],
+            [0, "cmdoption-osxphotos-uninstall-y"]
+        ],
+        "osxphotos-uuid command line option": [
+            [0, "cmdoption-osxphotos-uuid-f"]
+        ],
+        "osxphotos-version command line option": [
+            [0, "cmdoption-osxphotos-version-run"]
+        ],
         "albuminfo (class in osxphotos)": [
             [4, "osxphotos.AlbumInfo"]
         ],
         "albumsortorder (class in osxphotos)": [
             [4, "osxphotos.AlbumSortOrder"]
         ],
         "commentinfo (class in osxphotos)": [
```

#### docs/template_help.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Package Overview" href="package_overview.html" /><link rel="prev" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Template System - osxphotos 0.60.0 documentation</title>
+        <title>OSXPhotos Template System - osxphotos 0.60.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -609,15 +609,15 @@
 <dt class="field-odd">A tab<span class="colon">:</span></dt>
 <dd class="field-odd"><p>‘t’</p>
 </dd>
 </dl>
 </td>
 </tr>
 <tr class="row-odd"><td><p>{osxphotos_version}</p></td>
-<td><p>The osxphotos version, e.g. ‘0.60.0’</p></td>
+<td><p>The osxphotos version, e.g. ‘0.60.1’</p></td>
 </tr>
 <tr class="row-even"><td><p>{osxphotos_cmd_line}</p></td>
 <td><p>The full command line used to run osxphotos</p></td>
 </tr>
 <tr class="row-odd"><td><p>{album}</p></td>
 <td><p>Album(s) photo is contained in</p></td>
 </tr>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -428,15 +428,15 @@
 {closebracket}                 A close bracket: â]â
 {newline}                      A newline: ânâ
 {lf}                           A line feed: ânâ, alias for {newline}
 {cr}                           A carriage return: ârâ
 {crlf}                         A carriage return + line feed: ârnâ
 {tab}                            A tab:
                                      âtâ
-{osxphotos_version}            The osxphotos version, e.g. â0.60.0â
+{osxphotos_version}            The osxphotos version, e.g. â0.60.1â
 {osxphotos_cmd_line}           The full command line used to run osxphotos
 {album}                        Album(s) photo is contained in
 {folder_album}                 Folder path + album photo is contained in. e.g. âFolder/Subfolder/Albumâ or just âAlbumâ if
                                no enclosing folder
 {project}                      Project(s) photo is contained in (such as greeting cards, calendars, slideshows)
 {album_project}                Album(s) and project(s) photo is contained in; treats projects as regular albums
 {folder_album_project}         Folder path + album (includes projects as albums) photo is contained in. e.g. âFolder/Subfolder/
```

#### docs/tutorial.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" /><link rel="prev" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Tutorial - osxphotos 0.60.0 documentation</title>
+        <title>OSXPhotos Tutorial - osxphotos 0.60.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.1_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

### Comparing `osxphotos-0.60.0/osxphotos/exif_datetime_updater.py` & `osxphotos-0.60.1/osxphotos/exif_datetime_updater.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/exifinfo.py` & `osxphotos-0.60.1/osxphotos/exifinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/exiftool.py` & `osxphotos-0.60.1/osxphotos/exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/exiftool_filetypes.json` & `osxphotos-0.60.1/osxphotos/exiftool_filetypes.json`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/export_db.py` & `osxphotos-0.60.1/osxphotos/export_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -917,40 +917,43 @@
 
     @retry(stop=stop_after_attempt(MAX_RETRY_ATTEMPTS))
     def _open_export_db(self, dbfile: str):  # sourcery skip: raise-specific-error
         """open export database and return a db connection
         returns: connection to the database
         """
         if not os.path.isfile(dbfile):
-            conn = self._get_db_connection()
-            if not conn:
+            # database doesn't exist so create it in-memory
+            src = self._get_db_connection()
+            if not src:
                 raise Exception("Error getting connection to in-memory database")
-            self._create_or_migrate_db_tables(conn)
+            self._create_or_migrate_db_tables(src)
             self.was_created = True
             self.was_upgraded = ()
+            self.version = OSXPHOTOS_EXPORTDB_VERSION
+            return src
+
+        # database exists so copy it to memory
+        src = sqlite3.connect(dbfile, check_same_thread=SQLITE_CHECK_SAME_THREAD)
+
+        # Create a database in memory by backing up the on-disk database
+        dst = sqlite3.connect(":memory:", check_same_thread=SQLITE_CHECK_SAME_THREAD)
+        with dst:
+            src.backup(dst, pages=1)
+        src.close()
+
+        self.was_created = False
+        version_info = self._get_database_version(dst)
+        if version_info[1] < OSXPHOTOS_EXPORTDB_VERSION:
+            self._create_or_migrate_db_tables(dst)
+            self.was_upgraded = (version_info[1], OSXPHOTOS_EXPORTDB_VERSION)
         else:
-            conn = sqlite3.connect(dbfile, check_same_thread=SQLITE_CHECK_SAME_THREAD)
-            dbdump = self._dump_db(conn)
-            conn.close()
-
-            # Create a database in memory and import from the dump
-            conn = sqlite3.connect(
-                ":memory:", check_same_thread=SQLITE_CHECK_SAME_THREAD
-            )
-            conn.cursor().executescript(dbdump.read())
-            self.was_created = False
-            version_info = self._get_database_version(conn)
-            if version_info[1] < OSXPHOTOS_EXPORTDB_VERSION:
-                self._create_or_migrate_db_tables(conn)
-                self.was_upgraded = (version_info[1], OSXPHOTOS_EXPORTDB_VERSION)
-            else:
-                self.was_upgraded = ()
+            self.was_upgraded = ()
         self.version = OSXPHOTOS_EXPORTDB_VERSION
 
-        return conn
+        return dst
 
     def _get_db_connection(self):
         """return db connection to in memory database"""
         return sqlite3.connect(":memory:", check_same_thread=SQLITE_CHECK_SAME_THREAD)
 
     def _dump_db(self, conn: sqlite3.Connection) -> StringIO:
         """dump sqlite db to a string buffer"""
```

### Comparing `osxphotos-0.60.0/osxphotos/export_db_utils.py` & `osxphotos-0.60.1/osxphotos/export_db_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/fileutil.py` & `osxphotos-0.60.1/osxphotos/fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/frozen_photoinfo.py` & `osxphotos-0.60.1/osxphotos/frozen_photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/imageconverter.py` & `osxphotos-0.60.1/osxphotos/imageconverter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/momentinfo.py` & `osxphotos-0.60.1/osxphotos/momentinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/path_utils.py` & `osxphotos-0.60.1/osxphotos/path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/personinfo.py` & `osxphotos-0.60.1/osxphotos/personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/photodates.py` & `osxphotos-0.60.1/osxphotos/photodates.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/photoexporter.py` & `osxphotos-0.60.1/osxphotos/photoexporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/photoinfo.py` & `osxphotos-0.60.1/osxphotos/photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/photokit.py` & `osxphotos-0.60.1/osxphotos/photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/photosalbum.py` & `osxphotos-0.60.1/osxphotos/photosalbum.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/photoscript_utils.py` & `osxphotos-0.60.1/osxphotos/photoscript_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_comments.py` & `osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_exif.py` & `osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_faceinfo.py` & `osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_scoreinfo.py` & `osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/photosdb/_photosdb_process_searchinfo.py` & `osxphotos-0.60.1/osxphotos/photosdb/_photosdb_process_searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/photosdb/photosdb.py` & `osxphotos-0.60.1/osxphotos/photosdb/photosdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/photosdb/photosdb_utils.py` & `osxphotos-0.60.1/osxphotos/photosdb/photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/phototables.py` & `osxphotos-0.60.1/osxphotos/phototables.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/phototemplate.cog.md` & `osxphotos-0.60.1/osxphotos/phototemplate.cog.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/phototemplate.md` & `osxphotos-0.60.1/osxphotos/phototemplate.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/phototemplate.py` & `osxphotos-0.60.1/osxphotos/phototemplate.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/phototemplate.tx` & `osxphotos-0.60.1/osxphotos/phototemplate.tx`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/phototz.py` & `osxphotos-0.60.1/osxphotos/phototz.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/placeinfo.py` & `osxphotos-0.60.1/osxphotos/placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/pyrepl.py` & `osxphotos-0.60.1/osxphotos/pyrepl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/queries/shared_owner.sql.mako` & `osxphotos-0.60.1/osxphotos/queries/shared_owner.sql.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/query_builder.py` & `osxphotos-0.60.1/osxphotos/query_builder.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/queryoptions.py` & `osxphotos-0.60.1/osxphotos/queryoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/scoreinfo.py` & `osxphotos-0.60.1/osxphotos/scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/searchinfo.py` & `osxphotos-0.60.1/osxphotos/searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/sqlgrep.py` & `osxphotos-0.60.1/osxphotos/sqlgrep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/sqlite_utils.py` & `osxphotos-0.60.1/osxphotos/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/sqlitekvstore.py` & `osxphotos-0.60.1/osxphotos/sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/template_counter.py` & `osxphotos-0.60.1/osxphotos/template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/templates/xmp_sidecar.mako` & `osxphotos-0.60.1/osxphotos/templates/xmp_sidecar.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/templates/xmp_sidecar_beta.mako` & `osxphotos-0.60.1/osxphotos/templates/xmp_sidecar_beta.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/text_detection.py` & `osxphotos-0.60.1/osxphotos/text_detection.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/timeutils.py` & `osxphotos-0.60.1/osxphotos/timeutils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/timezones.py` & `osxphotos-0.60.1/osxphotos/timezones.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/tutorial.md` & `osxphotos-0.60.1/osxphotos/tutorial.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/uti.py` & `osxphotos-0.60.1/osxphotos/uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos/utils.py` & `osxphotos-0.60.1/osxphotos/utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos.egg-info/PKG-INFO` & `osxphotos-0.60.1/osxphotos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.0
+Version: 0.60.1
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.0/osxphotos.egg-info/SOURCES.txt` & `osxphotos-0.60.1/osxphotos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/osxphotos.egg-info/requires.txt` & `osxphotos-0.60.1/osxphotos.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/setup.py` & `osxphotos-0.60.1/setup.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_10_12_6.py` & `osxphotos-0.60.1/tests/test_10_12_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_albums_folders_catalina_10_15_7.py` & `osxphotos-0.60.1/tests/test_albums_folders_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_albums_folders_high_sierra_10_13_6.py` & `osxphotos-0.60.1/tests/test_albums_folders_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_albums_folders_mojave_10_14_6.py` & `osxphotos-0.60.1/tests/test_albums_folders_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_bigsur_10_16_0_1.py` & `osxphotos-0.60.1/tests/test_bigsur_10_16_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_catalina_10_15_7.py` & `osxphotos-0.60.1/tests/test_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli.py` & `osxphotos-0.60.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_add_locations.py` & `osxphotos-0.60.1/tests/test_cli_add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_add_to_album.py` & `osxphotos-0.60.1/tests/test_cli_add_to_album.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_all_commands.py` & `osxphotos-0.60.1/tests/test_cli_all_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_batch_edit.py` & `osxphotos-0.60.1/tests/test_cli_batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_dump.py` & `osxphotos-0.60.1/tests/test_cli_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_exiftool.py` & `osxphotos-0.60.1/tests/test_cli_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_export_cloud.py` & `osxphotos-0.60.1/tests/test_cli_export_cloud.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_export_projects.py` & `osxphotos-0.60.1/tests/test_cli_export_projects.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_exportdb.py` & `osxphotos-0.60.1/tests/test_cli_exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_import.py` & `osxphotos-0.60.1/tests/test_cli_import.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_orphans.py` & `osxphotos-0.60.1/tests/test_cli_orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_param_types.py` & `osxphotos-0.60.1/tests/test_cli_param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_sync.py` & `osxphotos-0.60.1/tests/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_timewarp.py` & `osxphotos-0.60.1/tests/test_cli_timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_utils.py` & `osxphotos-0.60.1/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cli_verbose.py` & `osxphotos-0.60.1/tests/test_cli_verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_cloud_owner_catalina.py` & `osxphotos-0.60.1/tests/test_cloud_owner_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_comments.py` & `osxphotos-0.60.1/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_concurrent_export.py` & `osxphotos-0.60.1/tests/test_concurrent_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_configoptions.py` & `osxphotos-0.60.1/tests/test_configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_datetime_formatter.py` & `osxphotos-0.60.1/tests/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_datetime_utils.py` & `osxphotos-0.60.1/tests/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_debug.py` & `osxphotos-0.60.1/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_empty_library_4_0.py` & `osxphotos-0.60.1/tests/test_empty_library_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_exif_info.py` & `osxphotos-0.60.1/tests/test_exif_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_exiftool.py` & `osxphotos-0.60.1/tests/test_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_exiftool_caching.py` & `osxphotos-0.60.1/tests/test_exiftool_caching.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_export_catalina_10_15_7.py` & `osxphotos-0.60.1/tests/test_export_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_export_catalina_10_15_7_use_photos_export.py` & `osxphotos-0.60.1/tests/test_export_catalina_10_15_7_use_photos_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_export_convert_to_jpeg.py` & `osxphotos-0.60.1/tests/test_export_convert_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_export_db.py` & `osxphotos-0.60.1/tests/test_export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_export_mojave_10_14_6.py` & `osxphotos-0.60.1/tests/test_export_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_export_raw_catalina_10_15_1.py` & `osxphotos-0.60.1/tests/test_export_raw_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_exportresults.py` & `osxphotos-0.60.1/tests/test_exportresults.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_faceinfo.py` & `osxphotos-0.60.1/tests/test_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_fileutil.py` & `osxphotos-0.60.1/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_highsierra.py` & `osxphotos-0.60.1/tests/test_highsierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_image_converter.py` & `osxphotos-0.60.1/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_incloud_big_sur_10_16_0.py` & `osxphotos-0.60.1/tests/test_incloud_big_sur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_incloud_catalina_10_15_1.py` & `osxphotos-0.60.1/tests/test_incloud_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_incloud_catalina_10_15_6.py` & `osxphotos-0.60.1/tests/test_incloud_catalina_10_15_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_incloud_mojave_10_14_6.py` & `osxphotos-0.60.1/tests/test_incloud_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_live_catalina_10_15_1.py` & `osxphotos-0.60.1/tests/test_live_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_modified_date_catalina_10_15_7.py` & `osxphotos-0.60.1/tests/test_modified_date_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_modified_date_mojave_10_14_6.py` & `osxphotos-0.60.1/tests/test_modified_date_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_mojave_10_14_6.py` & `osxphotos-0.60.1/tests/test_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_mojave_10_14_6_path_edited.py` & `osxphotos-0.60.1/tests/test_mojave_10_14_6_path_edited.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_monterey_12_0_1.py` & `osxphotos-0.60.1/tests/test_monterey_12_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_monterey_dev_beta_12_0_0.py` & `osxphotos-0.60.1/tests/test_monterey_dev_beta_12_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_movies_4_0.py` & `osxphotos-0.60.1/tests/test_movies_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_movies_5_0.py` & `osxphotos-0.60.1/tests/test_movies_5_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_path_utils.py` & `osxphotos-0.60.1/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_personinfo.py` & `osxphotos-0.60.1/tests/test_personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_photokit.py` & `osxphotos-0.60.1/tests/test_photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_photosdb_utils.py` & `osxphotos-0.60.1/tests/test_photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_placeinfo.py` & `osxphotos-0.60.1/tests/test_placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_places_catalina_10_15_1.py` & `osxphotos-0.60.1/tests/test_places_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_places_high_sierra_10_13_6.py` & `osxphotos-0.60.1/tests/test_places_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_places_mojave_10_14_6.py` & `osxphotos-0.60.1/tests/test_places_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_projects_catalina.py` & `osxphotos-0.60.1/tests/test_projects_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_projects_sierra.py` & `osxphotos-0.60.1/tests/test_projects_sierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_score_info.py` & `osxphotos-0.60.1/tests/test_score_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_search_info_10_14_6.py` & `osxphotos-0.60.1/tests/test_search_info_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_search_info_10_15_4.py` & `osxphotos-0.60.1/tests/test_search_info_10_15_4.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_search_info_10_15_5.py` & `osxphotos-0.60.1/tests/test_search_info_10_15_5.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_search_info_10_15_7.py` & `osxphotos-0.60.1/tests/test_search_info_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_shared_catalina_10_15_1.py` & `osxphotos-0.60.1/tests/test_shared_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_shared_mojave_10_14_6.py` & `osxphotos-0.60.1/tests/test_shared_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_sidecar_xmp.py` & `osxphotos-0.60.1/tests/test_sidecar_xmp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_specials_bigsur_10_16_0.py` & `osxphotos-0.60.1/tests/test_specials_bigsur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_specials_catalina_10_15_1.py` & `osxphotos-0.60.1/tests/test_specials_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_specials_mojave_10_14_6.py` & `osxphotos-0.60.1/tests/test_specials_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_specials_sierra_10_12.py` & `osxphotos-0.60.1/tests/test_specials_sierra_10_12.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_sqlitekvstore.py` & `osxphotos-0.60.1/tests/test_sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_template.py` & `osxphotos-0.60.1/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_template_counter.py` & `osxphotos-0.60.1/tests/test_template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_template_today.py` & `osxphotos-0.60.1/tests/test_template_today.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_uti.py` & `osxphotos-0.60.1/tests/test_uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_utils.py` & `osxphotos-0.60.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_ventura_13_0_0.py` & `osxphotos-0.60.1/tests/test_ventura_13_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.0/tests/test_ventura_dev_preview_13_0_0.py` & `osxphotos-0.60.1/tests/test_ventura_dev_preview_13_0_0.py`

 * *Files identical despite different names*

