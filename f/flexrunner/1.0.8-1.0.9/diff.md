# Comparing `tmp/flexrunner-1.0.8.tar.gz` & `tmp/flexrunner-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexrunner-1.0.8.tar", last modified: Wed Feb 22 08:07:03 2023, max compression
+gzip compressed data, was "flexrunner-1.0.9.tar", last modified: Sun May 14 09:25:08 2023, max compression
```

## Comparing `flexrunner-1.0.8.tar` & `flexrunner-1.0.9.tar`

### file list

```diff
@@ -1,167 +1,236 @@
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.454897 flexrunner-1.0.8/
--rw-rw-rw-   0        0        0     1928 2022-11-14 08:53:53.000000 flexrunner-1.0.8/.gitignore
--rw-rw-rw-   0        0        0     1081 2022-11-14 08:53:53.000000 flexrunner-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      296 2023-02-22 06:42:35.000000 flexrunner-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2184 2023-02-22 08:07:03.455495 flexrunner-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1032 2023-01-18 05:55:56.000000 flexrunner-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.361593 flexrunner-1.0.8/demo/
--rw-rw-rw-   0        0        0     1586 2022-12-23 09:13:54.000000 flexrunner-1.0.8/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.362592 flexrunner-1.0.8/demo/bin/
--rw-rw-rw-   0        0        0      193 2023-02-22 07:43:57.000000 flexrunner-1.0.8/demo/bin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.362592 flexrunner-1.0.8/demo/bin/webdrivers/
--rw-rw-rw-   0        0        0      193 2023-02-22 07:45:28.000000 flexrunner-1.0.8/demo/bin/webdrivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.364712 flexrunner-1.0.8/demo/conf/
--rw-rw-rw-   0        0        0      190 2022-11-14 08:53:53.000000 flexrunner-1.0.8/demo/conf/__init__.py
--rw-rw-rw-   0        0        0      188 2022-11-14 08:53:53.000000 flexrunner-1.0.8/demo/conf/debug.xml
--rw-rw-rw-   0        0        0      188 2022-11-14 08:53:53.000000 flexrunner-1.0.8/demo/conf/demo.xml
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.365713 flexrunner-1.0.8/demo/conf/testbed/
--rw-rw-rw-   0        0        0      190 2022-11-14 08:53:53.000000 flexrunner-1.0.8/demo/conf/testbed/__init__.py
--rw-rw-rw-   0        0        0      778 2023-01-18 03:29:39.000000 flexrunner-1.0.8/demo/conf/testbed/testbed_demo.xml
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.367713 flexrunner-1.0.8/demo/conf/testset/
--rw-rw-rw-   0        0        0      190 2022-11-14 08:53:53.000000 flexrunner-1.0.8/demo/conf/testset/__init__.py
--rw-rw-rw-   0        0        0      459 2023-02-22 07:42:03.000000 flexrunner-1.0.8/demo/conf/testset/testset_demo.xml
--rw-rw-rw-   0        0        0     4583 2023-02-17 08:30:44.000000 flexrunner-1.0.8/demo/conftest.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.368713 flexrunner-1.0.8/demo/page_objects/
--rw-rw-rw-   0        0        0      211 2022-12-23 09:20:21.000000 flexrunner-1.0.8/demo/page_objects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.369713 flexrunner-1.0.8/demo/page_objects/bucket_mgr/
--rw-rw-rw-   0        0        0      212 2023-02-06 02:41:55.000000 flexrunner-1.0.8/demo/page_objects/bucket_mgr/__init__.py
--rw-rw-rw-   0        0        0     1501 2023-02-17 08:30:44.000000 flexrunner-1.0.8/demo/page_objects/bucket_mgr/bucket_list_page.py
--rw-rw-rw-   0        0        0     2214 2023-02-17 08:30:44.000000 flexrunner-1.0.8/demo/page_objects/login_page.py
--rw-rw-rw-   0        0        0      199 2023-02-22 02:03:32.000000 flexrunner-1.0.8/demo/pytest.ini
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.369713 flexrunner-1.0.8/demo/testcase/
--rw-rw-rw-   0        0        0      190 2022-11-14 08:53:53.000000 flexrunner-1.0.8/demo/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.370714 flexrunner-1.0.8/demo/testcase/om/
--rw-rw-rw-   0        0        0      233 2022-12-29 06:58:18.000000 flexrunner-1.0.8/demo/testcase/om/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.371713 flexrunner-1.0.8/demo/testcase/om/home_page/
--rw-rw-rw-   0        0        0      213 2022-12-29 06:59:13.000000 flexrunner-1.0.8/demo/testcase/om/home_page/__init__.py
--rw-rw-rw-   0        0        0      671 2023-02-17 08:30:43.000000 flexrunner-1.0.8/demo/testcase/om/home_page/test_home.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.376018 flexrunner-1.0.8/demo/testcase/om/login/
--rw-rw-rw-   0        0        0      213 2022-12-29 06:58:44.000000 flexrunner-1.0.8/demo/testcase/om/login/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.378020 flexrunner-1.0.8/demo/testcase/om/login/steps/
--rw-rw-rw-   0        0        0      221 2022-12-23 08:50:20.000000 flexrunner-1.0.8/demo/testcase/om/login/steps/__init__.py
--rw-rw-rw-   0        0        0      819 2023-02-17 08:30:44.000000 flexrunner-1.0.8/demo/testcase/om/login/steps/api.py
--rw-rw-rw-   0        0        0      187 2022-12-26 10:08:24.000000 flexrunner-1.0.8/demo/testcase/om/login/steps/ui.py
--rw-rw-rw-   0        0        0     1130 2023-02-17 08:30:43.000000 flexrunner-1.0.8/demo/testcase/om/login/test_login.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.379020 flexrunner-1.0.8/demo/testcase/protocol/
--rw-rw-rw-   0        0        0      276 2023-01-18 06:05:51.000000 flexrunner-1.0.8/demo/testcase/protocol/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.379020 flexrunner-1.0.8/demo/testcase/protocol/file_store/
--rw-rw-rw-   0        0        0      194 2022-12-29 05:42:14.000000 flexrunner-1.0.8/demo/testcase/protocol/file_store/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.380020 flexrunner-1.0.8/demo/testcase/protocol/file_store/file_directory/
--rw-rw-rw-   0        0        0      206 2022-12-29 05:43:52.000000 flexrunner-1.0.8/demo/testcase/protocol/file_store/file_directory/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.380020 flexrunner-1.0.8/demo/testcase/protocol/file_store/file_share/
--rw-rw-rw-   0        0        0      206 2022-12-29 05:44:21.000000 flexrunner-1.0.8/demo/testcase/protocol/file_store/file_share/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.382020 flexrunner-1.0.8/demo/testcase/protocol/file_store/file_user/
--rw-rw-rw-   0        0        0      206 2022-12-29 05:43:58.000000 flexrunner-1.0.8/demo/testcase/protocol/file_store/file_user/__init__.py
--rw-rw-rw-   0        0        0      764 2023-02-17 08:30:44.000000 flexrunner-1.0.8/demo/testcase/protocol/file_store/file_user/test_file_user_create.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.382020 flexrunner-1.0.8/demo/testcase/protocol/object_store/
--rw-rw-rw-   0        0        0      218 2022-12-29 05:40:55.000000 flexrunner-1.0.8/demo/testcase/protocol/object_store/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.383020 flexrunner-1.0.8/demo/testcase/protocol/object_store/mc/
--rw-rw-rw-   0        0        0      210 2023-01-18 06:04:10.000000 flexrunner-1.0.8/demo/testcase/protocol/object_store/mc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.383020 flexrunner-1.0.8/demo/testcase/protocol/object_store/web/
--rw-rw-rw-   0        0        0      193 2023-01-18 06:00:12.000000 flexrunner-1.0.8/demo/testcase/protocol/object_store/web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.385019 flexrunner-1.0.8/demo/testcase/protocol/object_store/web/bucket/
--rw-rw-rw-   0        0        0      197 2022-12-29 00:53:39.000000 flexrunner-1.0.8/demo/testcase/protocol/object_store/web/bucket/__init__.py
--rw-rw-rw-   0        0        0     1113 2023-02-17 08:30:44.000000 flexrunner-1.0.8/demo/testcase/protocol/object_store/web/bucket/test_bucket_create.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.386020 flexrunner-1.0.8/demo/testcase/protocol/object_store/web/object/
--rw-rw-rw-   0        0        0      200 2022-12-29 05:26:21.000000 flexrunner-1.0.8/demo/testcase/protocol/object_store/web/object/__init__.py
--rw-rw-rw-   0        0        0     1114 2023-02-17 08:30:43.000000 flexrunner-1.0.8/demo/testcase/protocol/object_store/web/object/test_object_upload.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.386020 flexrunner-1.0.8/demo/testdata/
--rw-rw-rw-   0        0        0      190 2022-11-14 08:53:53.000000 flexrunner-1.0.8/demo/testdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.388020 flexrunner-1.0.8/flexrunner/
--rw-rw-rw-   0        0        0      762 2023-02-22 07:02:47.000000 flexrunner-1.0.8/flexrunner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.409115 flexrunner-1.0.8/flexrunner/base/
--rw-rw-rw-   0        0        0      190 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/base/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-02-22 07:15:24.000000 flexrunner-1.0.8/flexrunner/base/db.py
--rw-rw-rw-   0        0        0     4199 2023-02-17 08:30:43.000000 flexrunner-1.0.8/flexrunner/base/log.py
--rw-rw-rw-   0        0        0     4078 2023-02-22 08:00:57.000000 flexrunner-1.0.8/flexrunner/base/models.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.411117 flexrunner-1.0.8/flexrunner/cli/
--rw-rw-rw-   0        0        0      200 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/cli/__init__.py
--rw-rw-rw-   0        0        0     5947 2023-02-22 07:05:09.000000 flexrunner-1.0.8/flexrunner/cli/main.py
--rw-rw-rw-   0        0        0     4521 2023-02-22 08:06:30.000000 flexrunner-1.0.8/flexrunner/cli/manage.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.415117 flexrunner-1.0.8/flexrunner/config/
--rw-rw-rw-   0        0        0      996 2023-02-22 07:23:02.000000 flexrunner-1.0.8/flexrunner/config/__init__.py
--rw-rw-rw-   0        0        0     3362 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/config/cf_ini.py
--rw-rw-rw-   0        0        0     4403 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/config/cf_xml.py
--rw-rw-rw-   0        0        0      518 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/config/cf_yaml.py
--rw-rw-rw-   0        0        0      499 2022-12-27 04:58:01.000000 flexrunner-1.0.8/flexrunner/config/global_cf.ini
--rw-rw-rw-   0        0        0     3108 2023-02-22 07:14:21.000000 flexrunner-1.0.8/flexrunner/config/globals.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.415117 flexrunner-1.0.8/flexrunner/core/
--rw-rw-rw-   0        0        0      228 2022-12-23 08:57:23.000000 flexrunner-1.0.8/flexrunner/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.417117 flexrunner-1.0.8/flexrunner/core/data_factory/
--rw-rw-rw-   0        0        0      194 2022-12-20 04:49:40.000000 flexrunner-1.0.8/flexrunner/core/data_factory/__init__.py
--rw-rw-rw-   0        0        0      544 2022-12-20 04:51:29.000000 flexrunner-1.0.8/flexrunner/core/data_factory/random_func.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.418184 flexrunner-1.0.8/flexrunner/core/extend/
--rw-rw-rw-   0        0        0        0 2022-11-14 08:51:28.000000 flexrunner-1.0.8/flexrunner/core/extend/__init__.py
--rw-rw-rw-   0        0        0      843 2023-02-17 08:30:43.000000 flexrunner-1.0.8/flexrunner/core/extend/step.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.423184 flexrunner-1.0.8/flexrunner/core/runners/
--rw-rw-rw-   0        0        0      404 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.429183 flexrunner-1.0.8/flexrunner/core/runners/api/
--rw-rw-rw-   0        0        0      281 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.431183 flexrunner-1.0.8/flexrunner/core/runners/api/builtin/
--rw-rw-rw-   0        0        0      294 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/api/builtin/__init__.py
--rw-rw-rw-   0        0        0     7990 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/core/runners/api/builtin/comparators.py
--rw-rw-rw-   0        0        0     5513 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/api/builtin/functions.py
--rw-rw-rw-   0        0        0     8424 2023-02-17 08:30:43.000000 flexrunner-1.0.8/flexrunner/core/runners/api/builtin_loader.py
--rw-rw-rw-   0        0        0     7562 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/api/client.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.434348 flexrunner-1.0.8/flexrunner/core/runners/api/data_loader/
--rw-rw-rw-   0        0        0      430 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/core/runners/api/data_loader/__init__.py
--rw-rw-rw-   0        0        0     4441 2023-02-22 07:27:14.000000 flexrunner-1.0.8/flexrunner/core/runners/api/data_loader/case_loader.py
--rw-rw-rw-   0        0        0      501 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/core/runners/api/data_loader/csv_case_loader.py
--rw-rw-rw-   0        0        0     9605 2023-02-17 08:30:43.000000 flexrunner-1.0.8/flexrunner/core/runners/api/data_loader/xmind_case_loader.py
--rw-rw-rw-   0        0        0      195 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/core/runners/api/data_loader/yaml_case_loader.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.435349 flexrunner-1.0.8/flexrunner/core/runners/api/ext/
--rw-rw-rw-   0        0        0      190 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/core/runners/api/ext/__init__.py
--rw-rw-rw-   0        0        0     3477 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/api/ext/uploader.py
--rw-rw-rw-   0        0        0     6542 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/api/models.py
--rw-rw-rw-   0        0        0    22429 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/api/parser.py
--rw-rw-rw-   0        0        0    13779 2023-02-17 08:30:43.000000 flexrunner-1.0.8/flexrunner/core/runners/api/response.py
--rw-rw-rw-   0        0        0    29015 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/api/runner.py
--rw-rw-rw-   0        0        0    16951 2023-02-17 08:30:43.000000 flexrunner-1.0.8/flexrunner/core/runners/api/step.py
--rw-rw-rw-   0        0        0     1318 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/api/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.439348 flexrunner-1.0.8/flexrunner/core/runners/command/
--rw-rw-rw-   0        0        0      283 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/command/__init__.py
--rw-rw-rw-   0        0        0      281 2022-12-20 05:24:32.000000 flexrunner-1.0.8/flexrunner/core/runners/command/runner.py
--rw-rw-rw-   0        0        0      930 2022-12-29 02:02:27.000000 flexrunner-1.0.8/flexrunner/core/runners/decorator_class.py
--rw-rw-rw-   0        0        0     2280 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/core/runners/exceptions.py
--rw-rw-rw-   0        0        0     1323 2022-12-26 09:59:28.000000 flexrunner-1.0.8/flexrunner/core/runners/interface.py
--rw-rw-rw-   0        0        0     7442 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/meta_class.py
--rw-rw-rw-   0        0        0     1109 2023-02-17 08:30:43.000000 flexrunner-1.0.8/flexrunner/core/runners/test_decorator_class.py
--rw-rw-rw-   0        0        0     1241 2023-02-17 08:30:43.000000 flexrunner-1.0.8/flexrunner/core/runners/test_meta_class.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.443349 flexrunner-1.0.8/flexrunner/core/runners/web/
--rw-rw-rw-   0        0        0      398 2023-02-17 08:30:43.000000 flexrunner-1.0.8/flexrunner/core/runners/web/__init__.py
--rw-rw-rw-   0        0        0     1144 2022-12-20 08:19:20.000000 flexrunner-1.0.8/flexrunner/core/runners/web/exceptions.py
--rw-rw-rw-   0        0        0     7923 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/web/runner.py
--rw-rw-rw-   0        0        0    30868 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/core/runners/web/webdriver.py
--rw-rw-rw-   0        0        0     1671 2022-12-20 04:47:01.000000 flexrunner-1.0.8/flexrunner/core/runners/web/webdriver_manager_extend.py
--rw-rw-rw-   0        0        0     6710 2023-02-22 07:48:12.000000 flexrunner-1.0.8/flexrunner/global_context.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.446349 flexrunner-1.0.8/flexrunner/libs/
--rw-rw-rw-   0        0        0      190 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/libs/__init__.py
--rw-rw-rw-   0        0        0     2574 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/libs/jenkins_opt.py
--rw-rw-rw-   0        0        0     7528 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/libs/mysql_opt.py
--rw-rw-rw-   0        0        0     3494 2023-02-17 08:30:43.000000 flexrunner-1.0.8/flexrunner/libs/sqlalchemy_opt.py
--rw-rw-rw-   0        0        0     5760 2023-02-17 08:30:43.000000 flexrunner-1.0.8/flexrunner/libs/sqlite_opt.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.447764 flexrunner-1.0.8/flexrunner/notification/
--rw-rw-rw-   0        0        0      190 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/notification/__init__.py
--rw-rw-rw-   0        0        0      183 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/notification/mail.py
--rw-rw-rw-   0        0        0     2750 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/notification/qw_chat.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.453899 flexrunner-1.0.8/flexrunner/utils/
--rw-rw-rw-   0        0        0      190 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/utils/__init__.py
--rw-rw-rw-   0        0        0     6520 2023-02-17 08:30:44.000000 flexrunner-1.0.8/flexrunner/utils/dsl_helper.py
--rw-rw-rw-   0        0        0     5618 2022-11-15 01:06:31.000000 flexrunner-1.0.8/flexrunner/utils/file_helper.py
--rw-rw-rw-   0        0        0     2281 2022-11-15 01:06:39.000000 flexrunner-1.0.8/flexrunner/utils/pkg_helper.py
--rw-rw-rw-   0        0        0     6995 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/utils/retry.py
--rw-rw-rw-   0        0        0      565 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/utils/singleton.py
--rw-rw-rw-   0        0        0    10199 2022-11-14 08:53:53.000000 flexrunner-1.0.8/flexrunner/utils/util.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.402372 flexrunner-1.0.8/flexrunner.egg-info/
--rw-rw-rw-   0        0        0     2184 2023-02-22 08:07:03.000000 flexrunner-1.0.8/flexrunner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4354 2023-02-22 08:07:03.000000 flexrunner-1.0.8/flexrunner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-22 08:07:03.000000 flexrunner-1.0.8/flexrunner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-02-22 08:07:03.000000 flexrunner-1.0.8/flexrunner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-22 08:07:03.000000 flexrunner-1.0.8/flexrunner.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      541 2023-02-22 08:07:03.000000 flexrunner-1.0.8/flexrunner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-02-22 08:07:03.000000 flexrunner-1.0.8/flexrunner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1146 2023-02-21 11:32:40.000000 flexrunner-1.0.8/requirements.txt
--rw-rw-rw-   0        0        0      142 2023-02-22 08:07:03.457497 flexrunner-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3207 2023-02-22 07:32:20.000000 flexrunner-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:07:03.453899 flexrunner-1.0.8/tests/
--rw-rw-rw-   0        0        0      190 2022-11-14 08:53:53.000000 flexrunner-1.0.8/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.982070 flexrunner-1.0.9/
+-rw-rw-rw-   0        0        0     1928 2022-08-06 09:35:43.000000 flexrunner-1.0.9/.gitignore
+-rw-rw-rw-   0        0        0     1081 2022-08-06 09:35:43.000000 flexrunner-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      296 2023-02-22 13:57:15.000000 flexrunner-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2223 2023-05-14 09:25:08.983073 flexrunner-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1032 2023-01-24 13:47:52.000000 flexrunner-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.905978 flexrunner-1.0.9/demo/
+-rw-rw-rw-   0        0        0     1672 2023-04-16 06:24:22.000000 flexrunner-1.0.9/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.906978 flexrunner-1.0.9/demo/bin/
+-rw-rw-rw-   0        0        0      193 2023-02-22 13:57:15.000000 flexrunner-1.0.9/demo/bin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.906978 flexrunner-1.0.9/demo/bin/webdrivers/
+-rw-rw-rw-   0        0        0      193 2023-02-22 13:57:15.000000 flexrunner-1.0.9/demo/bin/webdrivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.906978 flexrunner-1.0.9/demo/conf/
+-rw-rw-rw-   0        0        0      190 2023-01-24 13:47:52.000000 flexrunner-1.0.9/demo/conf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.907978 flexrunner-1.0.9/demo/conf/testbed/
+-rw-rw-rw-   0        0        0      190 2023-01-24 13:47:52.000000 flexrunner-1.0.9/demo/conf/testbed/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.909410 flexrunner-1.0.9/demo/conf/testset/
+-rw-rw-rw-   0        0        0      190 2023-01-24 13:47:52.000000 flexrunner-1.0.9/demo/conf/testset/__init__.py
+-rw-rw-rw-   0        0        0     7029 2023-04-16 06:35:20.000000 flexrunner-1.0.9/demo/conftest.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.910598 flexrunner-1.0.9/demo/features/
+-rw-rw-rw-   0        0        0      193 2023-02-22 13:57:15.000000 flexrunner-1.0.9/demo/features/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.912605 flexrunner-1.0.9/demo/features/om/
+-rw-rw-rw-   0        0        0      211 2023-02-22 13:57:15.000000 flexrunner-1.0.9/demo/features/om/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.912605 flexrunner-1.0.9/demo/features/om/file_store/
+-rw-rw-rw-   0        0        0      190 2023-03-06 03:02:23.000000 flexrunner-1.0.9/demo/features/om/file_store/__init__.py
+-rw-rw-rw-   0        0        0     2337 2023-04-05 13:08:32.000000 flexrunner-1.0.9/demo/features/om/login_page.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.912605 flexrunner-1.0.9/demo/features/om/object_store/
+-rw-rw-rw-   0        0        0      190 2023-03-06 03:02:23.000000 flexrunner-1.0.9/demo/features/om/object_store/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.913606 flexrunner-1.0.9/demo/features/om/object_store/bucket_mgr/
+-rw-rw-rw-   0        0        0      212 2023-02-22 13:57:15.000000 flexrunner-1.0.9/demo/features/om/object_store/bucket_mgr/__init__.py
+-rw-rw-rw-   0        0        0     1793 2023-04-05 13:26:22.000000 flexrunner-1.0.9/demo/features/om/object_store/bucket_mgr/bucket_list_page.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.914606 flexrunner-1.0.9/demo/features/om/object_store/obj_mgr/
+-rw-rw-rw-   0        0        0      190 2023-04-05 13:32:47.000000 flexrunner-1.0.9/demo/features/om/object_store/obj_mgr/__init__.py
+-rw-rw-rw-   0        0        0      185 2023-04-05 13:32:47.000000 flexrunner-1.0.9/demo/features/om/object_store/obj_mgr/upload.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.915605 flexrunner-1.0.9/demo/features/toolkit/
+-rw-rw-rw-   0        0        0      190 2023-04-05 08:36:16.000000 flexrunner-1.0.9/demo/features/toolkit/__init__.py
+-rw-rw-rw-   0        0        0      968 2023-04-05 11:24:38.000000 flexrunner-1.0.9/demo/features/toolkit/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.916603 flexrunner-1.0.9/demo/testcase/
+-rw-rw-rw-   0        0        0      203 2023-02-25 07:48:33.000000 flexrunner-1.0.9/demo/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.916603 flexrunner-1.0.9/demo/testcase/om/
+-rw-rw-rw-   0        0        0      245 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/om/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.916603 flexrunner-1.0.9/demo/testcase/om/file_store/
+-rw-rw-rw-   0        0        0      228 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/om/file_store/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.917604 flexrunner-1.0.9/demo/testcase/om/file_store/file_directory/
+-rw-rw-rw-   0        0        0      242 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/om/file_store/file_directory/__init__.py
+-rw-rw-rw-   0        0        0      488 2023-02-25 13:44:33.000000 flexrunner-1.0.9/demo/testcase/om/file_store/file_directory/test_create_file_dir.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.918605 flexrunner-1.0.9/demo/testcase/om/file_store/file_share/
+-rw-rw-rw-   0        0        0      240 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/om/file_store/file_share/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-02-25 13:44:36.000000 flexrunner-1.0.9/demo/testcase/om/file_store/file_share/test_create_file_share.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.919604 flexrunner-1.0.9/demo/testcase/om/file_store/file_user/
+-rw-rw-rw-   0        0        0      240 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/om/file_store/file_user/__init__.py
+-rw-rw-rw-   0        0        0      640 2023-03-06 13:20:42.000000 flexrunner-1.0.9/demo/testcase/om/file_store/file_user/test_create_file_user.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.920604 flexrunner-1.0.9/demo/testcase/om/home_page/
+-rw-rw-rw-   0        0        0      225 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/om/home_page/__init__.py
+-rw-rw-rw-   0        0        0      564 2023-03-06 13:20:42.000000 flexrunner-1.0.9/demo/testcase/om/home_page/test_home.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.920604 flexrunner-1.0.9/demo/testcase/om/login/
+-rw-rw-rw-   0        0        0      227 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/om/login/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.921603 flexrunner-1.0.9/demo/testcase/om/login/steps/
+-rw-rw-rw-   0        0        0      221 2023-02-22 13:57:15.000000 flexrunner-1.0.9/demo/testcase/om/login/steps/__init__.py
+-rw-rw-rw-   0        0        0      819 2023-02-22 13:57:15.000000 flexrunner-1.0.9/demo/testcase/om/login/steps/api.py
+-rw-rw-rw-   0        0        0      187 2023-02-22 13:57:15.000000 flexrunner-1.0.9/demo/testcase/om/login/steps/ui.py
+-rw-rw-rw-   0        0        0     1327 2023-04-05 13:10:05.000000 flexrunner-1.0.9/demo/testcase/om/login/test_login.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.922603 flexrunner-1.0.9/demo/testcase/om/object_store/
+-rw-rw-rw-   0        0        0      226 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/om/object_store/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.923603 flexrunner-1.0.9/demo/testcase/om/object_store/bucket/
+-rw-rw-rw-   0        0        0      222 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/om/object_store/bucket/__init__.py
+-rw-rw-rw-   0        0        0     1030 2023-04-05 13:15:37.000000 flexrunner-1.0.9/demo/testcase/om/object_store/bucket/test_bucket_create.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.924605 flexrunner-1.0.9/demo/testcase/om/object_store/object/
+-rw-rw-rw-   0        0        0      228 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/om/object_store/object/__init__.py
+-rw-rw-rw-   0        0        0     1050 2023-04-05 13:32:48.000000 flexrunner-1.0.9/demo/testcase/om/object_store/object/test_object_upload.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.924605 flexrunner-1.0.9/demo/testcase/performance/
+-rw-rw-rw-   0        0        0      225 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/performance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.924605 flexrunner-1.0.9/demo/testcase/performance/object_store/
+-rw-rw-rw-   0        0        0      224 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/performance/object_store/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.925604 flexrunner-1.0.9/demo/testcase/protocol/
+-rw-rw-rw-   0        0        0      290 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/protocol/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.925604 flexrunner-1.0.9/demo/testcase/protocol/file_store/
+-rw-rw-rw-   0        0        0      235 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/protocol/file_store/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.925604 flexrunner-1.0.9/demo/testcase/protocol/file_store/cifs/
+-rw-rw-rw-   0        0        0      245 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/protocol/file_store/cifs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.926605 flexrunner-1.0.9/demo/testcase/protocol/file_store/nfs/
+-rw-rw-rw-   0        0        0      241 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/protocol/file_store/nfs/__init__.py
+-rw-rw-rw-   0        0        0      436 2023-02-25 13:45:21.000000 flexrunner-1.0.9/demo/testcase/protocol/file_store/nfs/test_mount.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.927605 flexrunner-1.0.9/demo/testcase/protocol/object_store/
+-rw-rw-rw-   0        0        0      242 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/protocol/object_store/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.928605 flexrunner-1.0.9/demo/testcase/protocol/object_store/mc/
+-rw-rw-rw-   0        0        0      228 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/protocol/object_store/mc/__init__.py
+-rw-rw-rw-   0        0        0      855 2023-03-12 02:06:51.000000 flexrunner-1.0.9/demo/testcase/protocol/object_store/mc/test_mc_admin.py
+-rw-rw-rw-   0        0        0      426 2023-02-25 13:45:34.000000 flexrunner-1.0.9/demo/testcase/protocol/object_store/mc/test_mc_cp.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.928605 flexrunner-1.0.9/demo/testcase/protocol/object_store/mc_admin/
+-rw-rw-rw-   0        0        0      235 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/protocol/object_store/mc_admin/__init__.py
+-rw-rw-rw-   0        0        0      463 2023-02-25 13:45:34.000000 flexrunner-1.0.9/demo/testcase/protocol/object_store/mc_admin/test_mc_admin_bucket.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.929604 flexrunner-1.0.9/demo/testcase/protocol/object_store/sdkgo/
+-rw-rw-rw-   0        0        0      263 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/protocol/object_store/sdkgo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.929604 flexrunner-1.0.9/demo/testcase/reliability/
+-rw-rw-rw-   0        0        0      229 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/reliability/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.930604 flexrunner-1.0.9/demo/testcase/reliability/network/
+-rw-rw-rw-   0        0        0      225 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/reliability/network/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-02-25 13:45:41.000000 flexrunner-1.0.9/demo/testcase/reliability/network/test_net_flashover.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.930604 flexrunner-1.0.9/demo/testcase/restapi/
+-rw-rw-rw-   0        0        0      245 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/restapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.930604 flexrunner-1.0.9/demo/testcase/toolkit/
+-rw-rw-rw-   0        0        0      225 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/toolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.931604 flexrunner-1.0.9/demo/testcase/toolkit/cleanup/
+-rw-rw-rw-   0        0        0      237 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/toolkit/cleanup/__init__.py
+-rw-rw-rw-   0        0        0      634 2023-04-05 11:25:21.000000 flexrunner-1.0.9/demo/testcase/toolkit/cleanup/test_cleanup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.932604 flexrunner-1.0.9/demo/testcase/toolkit/deploy/
+-rw-rw-rw-   0        0        0      235 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/toolkit/deploy/__init__.py
+-rw-rw-rw-   0        0        0      624 2023-04-05 08:36:16.000000 flexrunner-1.0.9/demo/testcase/toolkit/deploy/test_deploy.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.932604 flexrunner-1.0.9/demo/testcase/toolkit/upgrade/
+-rw-rw-rw-   0        0        0      223 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/toolkit/upgrade/__init__.py
+-rw-rw-rw-   0        0        0      437 2023-02-25 13:46:01.000000 flexrunner-1.0.9/demo/testcase/toolkit/upgrade/test_upgrade.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.933604 flexrunner-1.0.9/demo/testcase/value_added/
+-rw-rw-rw-   0        0        0      239 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/value_added/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.933604 flexrunner-1.0.9/demo/testcase/value_added/ilm/
+-rw-rw-rw-   0        0        0      241 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/value_added/ilm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.933604 flexrunner-1.0.9/demo/testcase/value_added/tier/
+-rw-rw-rw-   0        0        0      231 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/value_added/tier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.934605 flexrunner-1.0.9/demo/testcase/value_added/worm/
+-rw-rw-rw-   0        0        0      227 2023-02-25 09:04:26.000000 flexrunner-1.0.9/demo/testcase/value_added/worm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.934605 flexrunner-1.0.9/demo/testdata/
+-rw-rw-rw-   0        0        0      190 2023-02-22 13:57:15.000000 flexrunner-1.0.9/demo/testdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.935604 flexrunner-1.0.9/flexrunner/
+-rw-rw-rw-   0        0        0      944 2023-05-14 09:20:56.000000 flexrunner-1.0.9/flexrunner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.946387 flexrunner-1.0.9/flexrunner/base/
+-rw-rw-rw-   0        0        0      190 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/base/__init__.py
+-rw-rw-rw-   0        0        0     8905 2023-04-16 06:34:53.000000 flexrunner-1.0.9/flexrunner/base/db.py
+-rw-rw-rw-   0        0        0     5432 2023-04-14 23:52:53.000000 flexrunner-1.0.9/flexrunner/base/log.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.949766 flexrunner-1.0.9/flexrunner/base/models/
+-rw-rw-rw-   0        0        0      462 2023-04-14 23:52:53.000000 flexrunner-1.0.9/flexrunner/base/models/__init__.py
+-rw-rw-rw-   0        0        0     1189 2023-04-14 23:52:53.000000 flexrunner-1.0.9/flexrunner/base/models/log_icon_models.py
+-rw-rw-rw-   0        0        0     1387 2023-03-06 12:42:14.000000 flexrunner-1.0.9/flexrunner/base/models/platform_models.py
+-rw-rw-rw-   0        0        0     1818 2023-02-26 05:32:16.000000 flexrunner-1.0.9/flexrunner/base/models/result_models.py
+-rw-rw-rw-   0        0        0     2119 2023-04-16 06:30:34.000000 flexrunner-1.0.9/flexrunner/base/models/testcase_models.py
+-rw-rw-rw-   0        0        0     1478 2023-02-25 09:16:06.000000 flexrunner-1.0.9/flexrunner/base/models/xml_conf_models.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.950770 flexrunner-1.0.9/flexrunner/cli/
+-rw-rw-rw-   0        0        0      200 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/cli/__init__.py
+-rw-rw-rw-   0        0        0     6958 2023-04-15 06:06:21.000000 flexrunner-1.0.9/flexrunner/cli/main.py
+-rw-rw-rw-   0        0        0     5214 2023-05-14 09:07:19.000000 flexrunner-1.0.9/flexrunner/cli/manage.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.952769 flexrunner-1.0.9/flexrunner/config/
+-rw-rw-rw-   0        0        0      850 2023-03-06 02:53:55.000000 flexrunner-1.0.9/flexrunner/config/__init__.py
+-rw-rw-rw-   0        0        0     3362 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/config/cf_ini.py
+-rw-rw-rw-   0        0        0     4403 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/config/cf_xml.py
+-rw-rw-rw-   0        0        0      518 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/config/cf_yaml.py
+-rw-rw-rw-   0        0        0     3132 2023-05-14 09:24:24.000000 flexrunner-1.0.9/flexrunner/config/globals.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.952769 flexrunner-1.0.9/flexrunner/core/
+-rw-rw-rw-   0        0        0      228 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.953770 flexrunner-1.0.9/flexrunner/core/data_factory/
+-rw-rw-rw-   0        0        0      194 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/data_factory/__init__.py
+-rw-rw-rw-   0        0        0      544 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/data_factory/random_func.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.953770 flexrunner-1.0.9/flexrunner/core/extend/
+-rw-rw-rw-   0        0        0        0 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/extend/__init__.py
+-rw-rw-rw-   0        0        0      843 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/extend/step.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.954769 flexrunner-1.0.9/flexrunner/core/report/
+-rw-rw-rw-   0        0        0      327 2023-04-15 05:53:09.000000 flexrunner-1.0.9/flexrunner/core/report/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.955769 flexrunner-1.0.9/flexrunner/core/report/log_to_html/
+-rw-rw-rw-   0        0        0      190 2023-04-15 05:51:53.000000 flexrunner-1.0.9/flexrunner/core/report/log_to_html/__init__.py
+-rw-rw-rw-   0        0        0    19062 2023-04-16 06:03:56.000000 flexrunner-1.0.9/flexrunner/core/report/log_to_html/report.py
+-rw-rw-rw-   0        0        0     5112 2023-04-14 23:52:53.000000 flexrunner-1.0.9/flexrunner/core/report/log_to_html/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.960769 flexrunner-1.0.9/flexrunner/core/runners/
+-rw-rw-rw-   0        0        0      523 2023-03-06 02:53:55.000000 flexrunner-1.0.9/flexrunner/core/runners/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.964769 flexrunner-1.0.9/flexrunner/core/runners/api/
+-rw-rw-rw-   0        0        0      281 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.965768 flexrunner-1.0.9/flexrunner/core/runners/api/builtin/
+-rw-rw-rw-   0        0        0      294 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/builtin/__init__.py
+-rw-rw-rw-   0        0        0     7990 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/builtin/comparators.py
+-rw-rw-rw-   0        0        0     5513 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/builtin/functions.py
+-rw-rw-rw-   0        0        0     8424 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/builtin_loader.py
+-rw-rw-rw-   0        0        0     7562 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/client.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.967768 flexrunner-1.0.9/flexrunner/core/runners/api/data_loader/
+-rw-rw-rw-   0        0        0      430 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/data_loader/__init__.py
+-rw-rw-rw-   0        0        0     4441 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/data_loader/case_loader.py
+-rw-rw-rw-   0        0        0      501 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/data_loader/csv_case_loader.py
+-rw-rw-rw-   0        0        0     9605 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/data_loader/xmind_case_loader.py
+-rw-rw-rw-   0        0        0      195 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/data_loader/yaml_case_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.967768 flexrunner-1.0.9/flexrunner/core/runners/api/ext/
+-rw-rw-rw-   0        0        0      190 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/ext/__init__.py
+-rw-rw-rw-   0        0        0     3477 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/ext/uploader.py
+-rw-rw-rw-   0        0        0     6554 2023-02-25 09:24:21.000000 flexrunner-1.0.9/flexrunner/core/runners/api/models.py
+-rw-rw-rw-   0        0        0    22429 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/parser.py
+-rw-rw-rw-   0        0        0    13779 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/response.py
+-rw-rw-rw-   0        0        0    29015 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/runner.py
+-rw-rw-rw-   0        0        0    16959 2023-02-25 09:24:21.000000 flexrunner-1.0.9/flexrunner/core/runners/api/step.py
+-rw-rw-rw-   0        0        0     1318 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/api/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.968769 flexrunner-1.0.9/flexrunner/core/runners/command/
+-rw-rw-rw-   0        0        0      283 2023-03-06 02:53:55.000000 flexrunner-1.0.9/flexrunner/core/runners/command/__init__.py
+-rw-rw-rw-   0        0        0     2740 2023-04-05 11:32:21.000000 flexrunner-1.0.9/flexrunner/core/runners/command/runner.py
+-rw-rw-rw-   0        0        0      625 2023-04-14 23:52:53.000000 flexrunner-1.0.9/flexrunner/core/runners/custom_testcase.py
+-rw-rw-rw-   0        0        0      930 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/decorator_class.py
+-rw-rw-rw-   0        0        0     2280 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/exceptions.py
+-rw-rw-rw-   0        0        0     1789 2023-04-14 23:52:53.000000 flexrunner-1.0.9/flexrunner/core/runners/icon_msg.py
+-rw-rw-rw-   0        0        0     1323 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/interface.py
+-rw-rw-rw-   0        0        0    13403 2023-04-14 23:52:53.000000 flexrunner-1.0.9/flexrunner/core/runners/meta_class.py
+-rw-rw-rw-   0        0        0     1109 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/test_decorator_class.py
+-rw-rw-rw-   0        0        0     1241 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/test_meta_class.py
+-rw-rw-rw-   0        0        0      526 2023-02-25 12:04:42.000000 flexrunner-1.0.9/flexrunner/core/runners/util.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.973790 flexrunner-1.0.9/flexrunner/core/runners/web/
+-rw-rw-rw-   0        0        0      398 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/web/__init__.py
+-rw-rw-rw-   0        0        0     1144 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/web/exceptions.py
+-rw-rw-rw-   0        0        0     9074 2023-04-14 23:52:53.000000 flexrunner-1.0.9/flexrunner/core/runners/web/runner.py
+-rw-rw-rw-   0        0        0    31426 2023-04-14 23:52:53.000000 flexrunner-1.0.9/flexrunner/core/runners/web/webdriver.py
+-rw-rw-rw-   0        0        0     1671 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/core/runners/web/webdriver_manager_extend.py
+-rw-rw-rw-   0        0        0     9792 2023-04-15 06:06:03.000000 flexrunner-1.0.9/flexrunner/global_context.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.974789 flexrunner-1.0.9/flexrunner/notification/
+-rw-rw-rw-   0        0        0      190 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/notification/__init__.py
+-rw-rw-rw-   0        0        0    12218 2023-04-05 08:36:16.000000 flexrunner-1.0.9/flexrunner/notification/mail.py
+-rw-rw-rw-   0        0        0     2750 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/notification/qw_chat.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.979271 flexrunner-1.0.9/flexrunner/pkgs/
+-rw-rw-rw-   0        0        0      190 2023-03-06 02:53:55.000000 flexrunner-1.0.9/flexrunner/pkgs/__init__.py
+-rw-rw-rw-   0        0        0     2574 2023-03-06 02:53:55.000000 flexrunner-1.0.9/flexrunner/pkgs/jenkins_opt.py
+-rw-rw-rw-   0        0        0     7528 2023-03-06 02:53:55.000000 flexrunner-1.0.9/flexrunner/pkgs/mysql_opt.py
+-rw-rw-rw-   0        0        0     7262 2023-03-06 02:53:55.000000 flexrunner-1.0.9/flexrunner/pkgs/retry.py
+-rw-rw-rw-   0        0        0     3684 2023-03-06 02:53:55.000000 flexrunner-1.0.9/flexrunner/pkgs/sqlalchemy_opt.py
+-rw-rw-rw-   0        0        0     5760 2023-03-06 02:53:55.000000 flexrunner-1.0.9/flexrunner/pkgs/sqlite_opt.py
+-rw-rw-rw-   0        0        0    11238 2023-03-06 02:53:55.000000 flexrunner-1.0.9/flexrunner/pkgs/ssh_mgr.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.982070 flexrunner-1.0.9/flexrunner/utils/
+-rw-rw-rw-   0        0        0      190 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/utils/__init__.py
+-rw-rw-rw-   0        0        0     6520 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/utils/dsl_helper.py
+-rw-rw-rw-   0        0        0     5618 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/utils/file_helper.py
+-rw-rw-rw-   0        0        0     2281 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/utils/pkg_helper.py
+-rw-rw-rw-   0        0        0     6995 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/utils/retry.py
+-rw-rw-rw-   0        0        0      565 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/utils/singleton.py
+-rw-rw-rw-   0        0        0    10199 2023-02-22 13:57:15.000000 flexrunner-1.0.9/flexrunner/utils/util.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.945387 flexrunner-1.0.9/flexrunner.egg-info/
+-rw-rw-rw-   0        0        0     2223 2023-05-14 09:25:08.000000 flexrunner-1.0.9/flexrunner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6303 2023-05-14 09:25:08.000000 flexrunner-1.0.9/flexrunner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 09:25:08.000000 flexrunner-1.0.9/flexrunner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-05-14 09:25:08.000000 flexrunner-1.0.9/flexrunner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-14 09:23:18.000000 flexrunner-1.0.9/flexrunner.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      667 2023-05-14 09:25:08.000000 flexrunner-1.0.9/flexrunner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-14 09:25:08.000000 flexrunner-1.0.9/flexrunner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1412 2023-05-14 09:23:13.000000 flexrunner-1.0.9/requirements.txt
+-rw-rw-rw-   0        0        0      142 2023-05-14 09:25:08.984089 flexrunner-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3209 2023-05-14 09:20:37.000000 flexrunner-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 09:25:08.982070 flexrunner-1.0.9/tests/
+-rw-rw-rw-   0        0        0      190 2022-08-06 08:59:49.000000 flexrunner-1.0.9/tests/__init__.py
```

### Comparing `flexrunner-1.0.8/.gitignore` & `flexrunner-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/LICENSE` & `flexrunner-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/PKG-INFO` & `flexrunner-1.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: flexrunner
-Version: 1.0.8
+Version: 1.0.9
+Summary: UNKNOWN
 Home-page: https://github.com/txu2k8/test-runner-flex
 Author: TXU
 Author-email: tao.xu2008@outlook.com
 Maintainer: TXU
 Maintainer-email: tao.xu2008@outlook.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
@@ -51,7 +53,8 @@
 
 ```
 
 ## 测试demo环境搭建
 ```
 .\minio.exe server D:\minio\data\ --console-address 127.0.0.1:9001
 ```
+
```

### Comparing `flexrunner-1.0.8/README.md` & `flexrunner-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/demo/__init__.py` & `flexrunner-1.0.9/demo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 @email:tao.xu2008@outlook.com
 @description: 此处demo使用MINIO项目UI测试作为示例
 
 MINIO Windows本地临时部署：
 # 1、下载minio二进制文件
     https://min.io/docs/minio/windows/index.html
 # 2、本地准备数据存储路径，如：
-    D:\minio\data\
+    D:\\minio\\data\\
 # 3、cmd终端中启动服务
-    PS D:\minio> .\minio.exe server D:\minio\data\
+    PS D:\\minio> .\\minio.exe server D:\\minio\\data\
     MinIO Object Storage Server
     Copyright: 2015-2022 MinIO, Inc.
     License: GNU AGPLv3 <https://www.gnu.org/licenses/agpl-3.0.html>
     Version: RELEASE.2022-08-26T19-53-15Z (go1.18.5 windows/amd64)
 
     Status:         1 Online, 0 Offline.
     API: http://10.1.2.12:9000  http://192.168.153.1:9000  http://192.168.204.1:9000  http://127.0.0.1:9000
@@ -34,11 +34,14 @@
 
     +-----------------------------------------------------------------+
     | You are running an older version of MinIO released 3 months ago |
     | Update: Run `mc admin update`                                   |
     +-----------------------------------------------------------------+
 
 """
+# 产品ID、Name，用于关联平台
+PRODUCT_ID = 1
+PRODUCT_NAME = 'demo'
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `flexrunner-1.0.8/demo/page_objects/bucket_mgr/bucket_list_page.py` & `flexrunner-1.0.9/demo/features/om/object_store/bucket_mgr/bucket_list_page.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,35 +11,44 @@
 from flexrunner.global_context import GlobalContext
 from flexrunner import StepMetaClass
 
 
 class BucketListPage(WebRunner, metaclass=StepMetaClass):
     """桶页面"""
     env = GlobalContext.env
-    bucket_url = env.web_url + "/buckets"
+    buckets_url = env.web_url + "/buckets"
 
-    def refresh_bucket(self):
+    def refresh_bucket_list(self):
         """刷新桶列表"""
-        self.open(self.bucket_url)
+        self.open(self.buckets_url)
         self.click(xpath='//*[@id="root"]/div/main/div[3]/div/div/div[1]/div[2]/span[4]')
 
-    def _enter_create_bucket(self):
+    def search_bucket_list(self, bucket_name):
+        """搜索桶列表"""
+        self.open(self.buckets_url)
+        self.type_enter(bucket_name, clear=True, xpath='//*[@id="search-resource"]')
+
+    def assert_bucket_exist(self, bucket_name):
+        self.search_bucket_list(bucket_name)
+        self.assertElement(xpath=f'//*[@id="manageBucket-{bucket_name}"]')
+
+    def _enter_create_bucket_page(self):
         """进入”创建桶“页面"""
-        self.open(self.bucket_url)
+        self.open(self.buckets_url)
         self.click(xpath='//*[@id="root"]/div/main/div[3]/div/div/div[1]/div[2]/span[5]')
         self.assertInUrl("add-bucket")
 
     def _create_bucket_input(self, bucket_name):
         """创建桶输入信息"""
-        self.type(xpath='//*[@id="root"]/div/main/div[3]/div/div/div/div[1]/form/div[1]/div[1]/div/div/div/div',
+        self.type(xpath='//*[@id="bucket-name"]',
                   text=bucket_name, enter=False)
-        self.click(xpath='//*[@id="root"]/div/main/div[3]/div/div/div/div[1]/form/div[2]/button[2]')
+        self.click(xpath='//*[@id="create-bucket"]')
 
     def create_bucket(self, bucket_name):
         """创建一个桶"""
-        self._enter_create_bucket()
+        self._enter_create_bucket_page()
         self._create_bucket_input(bucket_name)
-        self.assertInUrl(bucket_name)
+        self.assert_bucket_exist(bucket_name)
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `flexrunner-1.0.8/demo/page_objects/login_page.py` & `flexrunner-1.0.9/demo/features/om/login_page.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,67 +4,69 @@
 @author:TXU
 @file:login_page
 @time:2022/12/23
 @email:tao.xu2008@outlook.com
 @description: 登录页面 操作步骤
 """
 import pytest
-from loguru import logger
 
 from flexrunner import WebRunner
 from flexrunner.global_context import GlobalContext
 from flexrunner import StepMetaClass
 
 
 class LoginPage(WebRunner, metaclass=StepMetaClass):
     """登录页面"""
     env = GlobalContext.env
 
-    def _login_input(self, user=None, password=None):
+    def login_input(self, user=None, password=None):
         """登录页面输入"""
         self.open(self.env.web_url + '/login')
         self.type(id_="accessKey", text=user or self.env.web_user, enter=False)
         self.type(id_="secretKey", text=password or self.env.web_pass, enter=False)
         self.click(id_="do-login")
 
-    def _assert_login_success(self):
+    def assert_login_success(self):
         """验证登录成功"""
-        self.assertInUrl("buckets")
+        self.assertInUrl("browser")
         self.assertInTitle("MinIO Console")
 
-    def _assert_login_failed(self):
+    def assert_login_failed(self):
         """验证登录失败"""
         self.assertInElement(xpath='/html/body/div[2]/div[1]', text="Invalid Login.")
+        # self.assertInElement(xpath='/html/body/div[2]/div[1]', text="ErrorResponse")
+
+    def assert_logout_success(self):
+        """验证退出登录成功"""
+        self.assertInUrl("/login")
 
     def login_success(self):
         """正常登录 -> 成功"""
-        self._login_input()
-        self._assert_login_success()
+        self.login_input()
+        self.assert_login_success()
 
     def login_with_err_user(self):
         """使用错误用户名登录 -> 失败"""
-        self._login_input(user='err_user')
-        self._assert_login_failed()
+        self.login_input(user='err_user')
+        self.assert_login_failed()
 
     def login_with_err_pass(self):
         """使用错误用户名密码登录 -> 失败"""
-        self._login_input(password='err_password')
-        self._assert_login_failed()
+        self.login_input(password='err_password')
+        self.assert_login_failed()
 
     def login_with_err_user_pass(self):
         """使用错误用户名+密码登录 -> 失败"""
-        self._login_input(user='err_user', password='err_password')
-        self._assert_login_failed()
+        self.login_input(user='err_user', password='err_password')
+        self.assert_login_failed()
 
     def logout(self):
         """退出登录"""
-        try:
-            self.click(xpath='//*[@id="app-menu"]/div/div[2]/ul[2]/div')
-        except Exception as e:
-            logger.error(e)
+        self.click(xpath='//*[@id="app-menu"]/div/div[2]/ul[2]/a')
+        self.assert_logout_success()
 
 
 @pytest.fixture()
 def teardown_logout():
     yield
     # 在执行测试方法之后要执行的代码, 退出登录
     LoginPage().logout()
```

### Comparing `flexrunner-1.0.8/demo/testcase/om/home_page/test_home.py` & `flexrunner-1.0.9/demo/testcase/om/home_page/test_home.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,25 +6,22 @@
 @time:2022/12/29
 @email:tao.xu2008@outlook.com
 @description: 首页显示验证
 """
 import pytest
 import allure
 from flexrunner import CaseMetaClass
-from demo.page_objects.login_page import LoginPage, teardown_logout
+from demo.features.om.login_page import LoginPage
 
 
-@allure.epic("OM")
-@allure.feature("首页")
-@allure.story("首页")
 @allure.suite("首页")
 class TestCaseHome(metaclass=CaseMetaClass):
     login_page = LoginPage()
 
     @pytest.mark.CI
-    def test_home_001(self, teardown_logout):
+    def test_home_005(self):
         """正常登录成功"""
         self.login_page.login_success()
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `flexrunner-1.0.8/demo/testcase/om/login/steps/api.py` & `flexrunner-1.0.9/demo/testcase/om/login/steps/api.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/demo/testcase/protocol/file_store/file_user/test_file_user_create.py` & `flexrunner-1.0.9/demo/testcase/om/file_store/file_user/test_create_file_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
 @author:TXU
-@file:test_file_user_create
+@file:test_create_file_user
 @time:2022/12/29
 @email:tao.xu2008@outlook.com
 @description: 文件用户 - 创建
 """
 import pytest
 import allure
 from flexrunner import CaseMetaClass
-from demo.page_objects.login_page import LoginPage, teardown_logout
+from demo.features.om.login_page import LoginPage
 
 
-@allure.epic("协议")
-@allure.feature("文件存储")
-@allure.story("文件用户")
-@allure.suite("本地用户/创建")
+@allure.suite("创建本地用户")
 class TestCaseCreateLocalUser(metaclass=CaseMetaClass):
     login_page = LoginPage()
 
     @pytest.mark.CI
-    def test_create_loacl_user_001(self, teardown_logout):
+    def test_create_loacl_user_008(self):
         """文件存储-正常创建本地用户成功"""
         self.login_page.login_success()
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `flexrunner-1.0.8/demo/testcase/protocol/object_store/web/bucket/test_bucket_create.py` & `flexrunner-1.0.9/demo/testcase/om/object_store/object/test_object_upload.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
 @author:TXU
-@file:test_bucket_create
-@time:2022/12/28
+@file:object
+@time:2022/12/29
 @email:tao.xu2008@outlook.com
-@description:
+@description: 对象上传
 """
 import pytest
 import allure
 from flexrunner import CaseMetaClass
 from flexrunner.global_context import GlobalContext
-from demo.page_objects.login_page import LoginPage
-from demo.page_objects.bucket_mgr.bucket_list_page import BucketListPage
+from demo.features.om.login_page import LoginPage
+from demo.features.om.object_store.bucket_mgr.bucket_list_page import BucketListPage
 
 
-@allure.epic("协议（Web）")
-@allure.feature("对象存储")
-@allure.story("桶管理")
-@allure.suite("创建桶")
-class TestCaseCreateBucket(metaclass=CaseMetaClass):
+@allure.suite("上传对象")
+class TestCaseUploadObject(metaclass=CaseMetaClass):
     time_str = GlobalContext.get_time_str()
+    bucket_name = f'auto-{time_str}'
     login_page = LoginPage()
     bucket_list_page = BucketListPage()
 
     @classmethod
     def setup_class(cls):
         cls.login_page.login_success()
+        cls.bucket_list_page.create_bucket(cls.bucket_name)
 
     @classmethod
     def teardown_class(cls):
         cls.login_page.logout()
 
     @pytest.mark.P0
-    def test_create_bucket_001(self):
-        """创建桶成功"""
-        bucket_name = f'auto_{self.time_str}'
-        self.bucket_list_page.create_bucket(bucket_name)
+    def test_upload_object_010(self):
+        """上传对象成功 TODO"""
+        pass
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `flexrunner-1.0.8/flexrunner/__init__.py` & `flexrunner-1.0.9/flexrunner/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 @author:TXU
 @file:__init__.py
 @time:2022/08/24
 @email:tao.xu2008@outlook.com
 @description:
 """
 # from flexrunner.global_context import GlobalContext
+from flexrunner.core.runners.util import get_testcase_id_by_func_name
 from flexrunner.core.runners.meta_class import StepMetaClass, CaseMetaClass, step_decorator, case_decorator
 from flexrunner.core.runners.api.step import ApiStep, RunRequest
 from flexrunner.core.runners.web import WebRunner, WebDriver, WebElement
+from flexrunner.core.runners.command import CmdRunner
 
-__version__ = '1.0.8'
 __all__ = [
     # "GlobalContext",
+    "get_testcase_id_by_func_name",
     "StepMetaClass", "CaseMetaClass", "step_decorator", "case_decorator",  # 元编程，实现批量装饰
     "ApiStep", "RunRequest",
     "WebRunner", "WebDriver", "WebElement",  # WEB UI 测试
+    "CmdRunner"  # CMD命令执行测试
 ]
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `flexrunner-1.0.8/flexrunner/cli/main.py` & `flexrunner-1.0.9/flexrunner/cli/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,79 +5,97 @@
 @file:main
 @time:2022/08/21
 @email:tao.xu2008@outlook.com
 @description:
 """
 import os
 import json
+import shutil
+
+import pytest
 import typer
 import subprocess
+import urllib3
 from loguru import logger
 
 from flexrunner.base.db import TestDB
 from flexrunner.base.log import LogLevelEnum, init_logger
-from flexrunner import config
 from flexrunner.global_context import GlobalContext
 from flexrunner.utils.util import seconds_to_hms, json_dumps
 
 
-def run_pytest(context):
+urllib3.disable_warnings()
+urllib3.add_stderr_logger(LogLevelEnum.INFO.value)
+
+
+def run_pytest(context, collect_only=False):
     """
     执行pytest
+    :param collect_only:
     :param context:
     :return:
     """
     # 解析pytest 文件
     test_conf = context.test_conf
     pytest_files_set = []
     for ts in test_conf.test_set_list:
         for case in ts.case_list:
             pytest_files_set.append(os.path.join(test_conf.base_path, case['location']))
     logger.info("\n{}".format(json.dumps(pytest_files_set, indent=2)))
 
-    db_info = config.DB_INFO
+    db_info = GlobalContext.db_info
     if db_info.get('ENGINE') == 'django.db.backends.sqlite3':
         db_info["DB_PATH"] = str(db_info.get('NAME'))
     elif db_info.get('ENGINE') == 'django.db.backends.mysql':
         db_info["USER"] = db_info.get('USER')
         db_info["PASSWORD"] = db_info.get('PASSWORD')
         db_info["HOST"] = db_info.get('HOST')
         db_info["PORT"] = db_info.get('PORT')
         db_info["NAME"] = db_info.get('NAME')
     # - 构建pytest 参数
     logger.info("构建pytest 参数...")
     argv = pytest_files_set + [
-        '--log_path={}'.format(context.report_summary.log_path),
-        '--log_level={}'.format(context.log_level),
+        '--case_log_path={}'.format(context().case_log_path),
+        '--case_log_level={}'.format(context.log_level),
         '-v', '-s',
         # '--show-capture=no',  # 不显示捕获日志
         '--ignore-unknown-dependency',
         '-W', 'ignore:Module already imported:pytest.PytestWarning',
 
+        # '--capture=sys',
+        '--allure-no-capture',  # 取消添加程序中捕获到控制台或者终端的log日志或者print输出到allure测试报告的Test Body中
+        '--alluredir={}'.format(context().allure_results_path), '--clean-alluredir',  # 生成allure xml结果
+
         # pytest-html
-        # '--html={}'.format(context().html_report_path),
+        # '--html={}'.format(context().html_report_full_path),
         # '--self-contained-html',
 
         # pytest-flexreport
+        '--template=3',
         '--report={}'.format(context().html_report_full_path),
         '--history_dir={}'.format(context().project_reports_path),
         '--title=测试报告：{}（ID={}）'.format(test_conf.project, context.report_summary.id),
-        '--template=2',
-
-        # '--capture=sys',
-        '--allure-no-capture',  # 取消添加程序中捕获到控制台或者终端的log日志或者print输出到allure测试报告的Test Body中
-        '--alluredir={}'.format(context().xml_report_path), '--clean-alluredir',  # 生成allure xml结果
+        '--log_path={}'.format(context().log_full_path),
+        '--report_path={}'.format(context.jenkins_workspace or "http://127.0.0.1:65329/index.html"),
+        '--testcase_basename=testcase',
+
+        # pytest-json-report
+        '--json-report',
+        '--json-report-file={}'.format(context().json_report_full_path),
     ]
+    if collect_only:
+        argv.append('--collect-only')  # 只收集用例不执行，可用于统计用例数
+
     # -q test_01.py
     logger.info("pytest 命令：{}\n".format(json.dumps(argv, indent=2)))
 
     # - 执行pytest
 
     # 执行方式一
-    import pytest
+    # import pytest
     pytest.main(argv)
     # err_msg = ''
     # exit_code = 0
 
     # 执行方式二
     # p = subprocess.Popen(['pytest'] + argv)
     # p.wait()
@@ -142,33 +160,38 @@
 def main(
     test_conf_path: str = typer.Option(
             "./demo/conf/demo.xml",
             "--test_conf_path",
             "-f",
             help="配置文件路径，对应目录：./{$project}/conf/{$test_conf}",
         ),
+    report_allure: bool = typer.Option(False, help="本地生成allure报告"),
+    jenkins_workspace: str = typer.Option("", help="jenkins workspace路径"),
+    collect_only: bool = typer.Option(False, help="只收集用例不执行，用于统计用例数"),
     loglevel: LogLevelEnum = typer.Option(LogLevelEnum.INFO, help="日志等级"),
     desc: str = typer.Option('', help="测试描述"),
 ):
     """FlexRunner 命令行 CLI"""
     # 参数解析
     test_conf_path = os.path.abspath(os.path.join(os.getcwd(), test_conf_path))
     logger.info("执行 {}".format(test_conf_path))
     GlobalContext.test_conf_path = test_conf_path
+    GlobalContext.jenkins_workspace = jenkins_workspace
     GlobalContext().init_data()
 
     # 初始化日志
-    init_logger(log_path=GlobalContext().log_path, suffix=desc.strip(), loglevel=loglevel)
+    init_logger(log_path=GlobalContext().log_full_path, suffix=desc.strip(), loglevel=loglevel)
 
     # - 执行 pytest
     try:
-        return run_pytest(GlobalContext)
+        return run_pytest(GlobalContext, collect_only)
     except Exception as e:
         raise e
     finally:
         logger.info("test log: {}".format(GlobalContext.report_summary.log_path))
         logger.info("result data: {}".format(GlobalContext.report_summary.report_allure_path))
-        generate_allure_report(GlobalContext)
+        if report_allure and not collect_only:
+            generate_allure_report(GlobalContext)
 
 
 if __name__ == '__main__':
     typer.run(main)
```

### Comparing `flexrunner-1.0.8/flexrunner/cli/manage.py` & `flexrunner-1.0.9/flexrunner/cli/manage.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,26 +4,47 @@
 @author:TXU
 @file:manage
 @time:2023/2/21
 @email:tao.xu2008@outlook.com
 @description: 项目管理相关命令
 """
 import os
-import typer
 import shutil
+import typer
+from typing import Optional
 from loguru import logger
 
+from flexrunner.config import VERSION, AUTHOR
 from webdriver_manager.firefox import GeckoDriverManager
 from webdriver_manager.microsoft import IEDriverManager
 from webdriver_manager.microsoft import EdgeChromiumDriverManager
 from flexrunner import config
 from flexrunner.base.models import WebDriverTypeEnum
 from flexrunner.core.runners.web.webdriver_manager_extend import ChromeDriverManager
 
 
+def version_callback(value: bool):
+    if value:
+        print(f"Version: {VERSION}")
+        print(f"Written by: {VERSION}")
+        raise typer.Exit()
+
+
+def public(
+        version: Optional[bool] = typer.Option(
+            None, "--version", callback=version_callback, help='Show the tool version'
+        ),
+):
+    """公共参数"""
+    pass
+
+
+app = typer.Typer(name="FlexRunner", callback=public, add_completion=False, help="FlexRunner 命令行 CLI.")
+
+
 def create_folder(folder_path):
     if not os.path.exists(folder_path):
         os.makedirs(folder_path)
         logger.info(f"created folder: {folder_path}")
 
 
 def create_file(path, file_content=""):
@@ -65,14 +86,15 @@
 
     # project/conf
     create_folder(os.path.join(project_path, "conf"))
 
     # project/conf
     create_folder(os.path.join(project_path, "conf"))
     create_file(os.path.join(project_path, "conf", "debug.xml"))
+    create_file(os.path.join(project_path, "conf", "global_conf.ini"))
     create_folder(os.path.join(project_path, "conf", "testbed"))
     create_file(os.path.join(project_path, "conf",  "testbed", "testbed_debug.xml"))
     create_folder(os.path.join(project_path, "conf", "testset"))
     create_file(os.path.join(project_path, "conf", "testset", "testset_debug.xml"))
 
     # project/testdata
     data_sample = '''{
@@ -113,22 +135,24 @@
     elif browser == "edge":
         driver_path = EdgeChromiumDriverManager().install()
         logger.info(f"Edge Driver[==>] {driver_path}")
     else:
         raise NameError(f"Not found '{browser}' browser driver.")
 
 
+@app.command(help='CLI初始化测试项目')
 def startapp(
     project: str = typer.Option("demo", "--project", "-p", help="Create a new automation test project"),
-    install: WebDriverTypeEnum = typer.Option('', "--install", "-i", help="install with Web driver type?"),
+    install: WebDriverTypeEnum = typer.Option(..., "--install", "-i", help="install with Web driver type?"),
 ):
     """FlexRunner startapp 命令行 CLI"""
-    create_scaffold(project)
     if install:
         install_driver(install.value)
+        return
+    create_scaffold(project)
 
 
 def main():
     typer.run(startapp)
 
 
 if __name__ == '__main__':
```

### Comparing `flexrunner-1.0.8/flexrunner/config/__init__.py` & `flexrunner-1.0.9/flexrunner/config/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,16 +18,13 @@
     "read_yaml", "ConfigIni", "ConfigXml",
     # 全局内存变量-读写
     "set_global_value", "get_global_value", "get_global_dict",
     # 环境变量-读写
     "set_os_environ", "unset_os_environ", "get_os_environment",
     # 全局常量
     "CWD", "BASE_DIR", "LOG_DIR", "REPORT_DIR",  # 全局路径 dir
-    "global_cf",
-    "DB_INFO",  # 数据库配置
     "TIME_STR",  # 时间戳
-    "FILE_LOG_LEVEL", "CONSOLE_LOG_LEVEL", "MAX_ROTATION", "MAX_RETENTION",  # 日志配置
 ]
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `flexrunner-1.0.8/flexrunner/config/cf_ini.py` & `flexrunner-1.0.9/flexrunner/config/cf_ini.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/config/cf_xml.py` & `flexrunner-1.0.9/flexrunner/config/cf_xml.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/config/cf_yaml.py` & `flexrunner-1.0.9/flexrunner/config/cf_yaml.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/config/globals.py` & `flexrunner-1.0.9/flexrunner/config/globals.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,42 +13,44 @@
 from loguru import logger
 
 from flexrunner.core.runners.exceptions import EnvNotFound, VariableNotFound
 from flexrunner.config.cf_ini import ConfigIni
 
 
 # 版本号
-VERSION = "1.0.1 - 2022-12-26"
-AUTHOR = "tao.xu"
+VERSION = "1.0.9"
+AUTHOR = "tao.xu@outlook.com - 2023-05-14"
 
 # 时间字符串
 TIME_STR = datetime.now().strftime("%Y-%m-%d-%H-%M-%S")  # 时间字符串
 TIME_STR_F = datetime.now().strftime("%Y-%m-%d-%H-%M-%S-%f")  # 时间字符串
 
 # 项目root目录
 CWD = os.getcwd()
 BASE_DIR = Path(__file__).resolve().parent.parent.parent if __file__.endswith('py') else os.getcwd()
-global_cf_path = os.path.join(BASE_DIR, "flexrunner", "config", "global_cf.ini")
 
 # 日志、报告目录路径
 LOG_DIR = os.path.join(CWD, "log")
 REPORT_DIR = os.path.join(CWD, 'reports')
 
+"""
 # global_cf.ini 配置项
 # 创建配置对象为全局变量
+global_cf_path = os.path.join(BASE_DIR, "flexrunner", "config", "global_conf.ini")
 global_cf = ConfigIni(global_cf_path)
 FILE_LOG_LEVEL = global_cf.get_str("LOGGER", "file_level")
 CONSOLE_LOG_LEVEL = global_cf.get_str("LOGGER", "console_level")
 MAX_ROTATION = global_cf.get_str("LOGGER", "max_rotation")
 MAX_RETENTION = global_cf.get_str("LOGGER", "max_retention")
 
 DB_INFO = {
     "ENGINE": global_cf.get_str("DATABASES", "ENGINE"),
     "NAME": global_cf.get_str("DATABASES", "NAME"),
 }
+"""
 
 
 # 设置全局 key/value
 _global_dict = {}
 
 
 def set_global_value(key, value):
```

### Comparing `flexrunner-1.0.8/flexrunner/core/data_factory/random_func.py` & `flexrunner-1.0.9/flexrunner/core/data_factory/random_func.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/extend/step.py` & `flexrunner-1.0.9/flexrunner/core/extend/step.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/api/builtin/comparators.py` & `flexrunner-1.0.9/flexrunner/core/runners/api/builtin/comparators.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/api/builtin/functions.py` & `flexrunner-1.0.9/flexrunner/core/runners/api/builtin/functions.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/api/builtin_loader.py` & `flexrunner-1.0.9/flexrunner/core/runners/api/builtin_loader.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/api/client.py` & `flexrunner-1.0.9/flexrunner/core/runners/api/client.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/api/data_loader/case_loader.py` & `flexrunner-1.0.9/flexrunner/core/runners/api/data_loader/case_loader.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/api/data_loader/xmind_case_loader.py` & `flexrunner-1.0.9/flexrunner/core/runners/api/data_loader/xmind_case_loader.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/api/ext/uploader.py` & `flexrunner-1.0.9/flexrunner/core/runners/api/ext/uploader.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/api/models.py` & `flexrunner-1.0.9/flexrunner/core/runners/api/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import Any
 from typing import Dict, Text, Union, Callable
 from typing import List
 
 from pydantic import BaseModel, Field
 from pydantic import HttpUrl
 
-from flexrunner.base.models import TestStatusEnum, StepType, TestTime
+from flexrunner.base.models import TestStatusEnum, StepTypeEnum, TestTime
 
 Name = Text
 Desc = Text
 Url = Text
 BaseUrl = Union[HttpUrl, Text]
 VariablesMapping = Dict[Text, Any]
 FunctionsMapping = Dict[Text, Callable]
@@ -98,15 +98,15 @@
 
 
 class TStep(BaseModel):
     """测试步骤模型"""
     id: int = 0
     sid: Text = ''
     step_name: Name
-    step_type: StepType = StepType.API  # 测试类型 - API
+    step_type: StepTypeEnum = StepTypeEnum.API  # 测试类型 - API
     description: Desc = ''  # 步骤描述
     is_skip: bool = False  # 是否跳过改测试步骤
     skipif: Union[Text, None] = None  # 条件表达式，是否跳过当前步骤
     depends: List[int] = []  # 依赖的测试步骤id，如果依赖步骤失败，跳过当前步骤
     sleep: int = 0  # 执行当前步骤前sleep seconds
     base_url: BaseUrl = ""  # 指定 base_url，如未指定则使用TConfig里的base_url
     request: Union[TRequest, None] = None
```

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/api/parser.py` & `flexrunner-1.0.9/flexrunner/core/runners/api/parser.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/api/response.py` & `flexrunner-1.0.9/flexrunner/core/runners/api/response.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/api/runner.py` & `flexrunner-1.0.9/flexrunner/core/runners/api/runner.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/api/step.py` & `flexrunner-1.0.9/flexrunner/core/runners/api/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 @email:tao.xu2008@outlook.com
 @description:
 """
 import inspect
 from typing import Text, Any, Union
 from loguru import logger
 
-from flexrunner.base.models import StepType
+from flexrunner.base.models import StepTypeEnum
 from flexrunner.core.runners.api.models import (
     TConfig,
     TStep,
     TRequest,
     MethodEnum,
 )
 
@@ -372,15 +372,15 @@
     def validate(self) -> StepRequestValidation:
         return StepRequestValidation(self.__step_context)
 
 
 class RunRequest(object):
     def __init__(self, step_name: Text):
         self.__step_context = TStep(step_name=step_name)
-        self.step_type = StepType.API
+        self.step_type = StepTypeEnum.API
 
     def with_id(self, step_id) -> "RunRequest":
         self.__step_context.id = step_id
         return self
 
     def with_sid(self, step_sid) -> "RunRequest":
         self.__step_context.sid = step_sid
```

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/api/utils.py` & `flexrunner-1.0.9/flexrunner/core/runners/api/utils.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/decorator_class.py` & `flexrunner-1.0.9/flexrunner/core/runners/decorator_class.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/exceptions.py` & `flexrunner-1.0.9/flexrunner/core/runners/exceptions.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/interface.py` & `flexrunner-1.0.9/flexrunner/core/runners/interface.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/test_decorator_class.py` & `flexrunner-1.0.9/flexrunner/core/runners/test_decorator_class.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/test_meta_class.py` & `flexrunner-1.0.9/flexrunner/core/runners/test_meta_class.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/web/exceptions.py` & `flexrunner-1.0.9/flexrunner/core/runners/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/web/runner.py` & `flexrunner-1.0.9/flexrunner/core/runners/web/runner.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,45 +4,46 @@
 @author:TXU
 @file:runner
 @time:2022/12/26
 @email:tao.xu2008@outlook.com
 @description: 
 """
 import time
-from unittest import TestCase
 from urllib.parse import unquote
 
 from loguru import logger
-from prettytable import PrettyTable
 from selenium.webdriver.common.by import By
 
-from flexrunner.base.models import StepType
+from flexrunner.base.models import StepTypeEnum
 from flexrunner.global_context import GlobalContext
+from flexrunner.core.runners.icon_msg import IconMsg
+from flexrunner.core.runners.custom_testcase import CustomTestCase
 from flexrunner.core.runners.web.exceptions import NotFindElementError
 from flexrunner.core.runners.web.webdriver import WebDriver
 
 
-class WebRunner(TestCase, WebDriver):
+class WebRunner(CustomTestCase, WebDriver):
     """Web测试执行引擎入口"""
-    step_type = StepType.WEB.value  # 约定：指定测试类型，meta_class.py step需要使用
+    step_type = StepTypeEnum.WEB.value  # 约定：指定测试类型，meta_class.py step需要使用
 
     def assertTitle(self, title: str = None, msg: str = None) -> None:
         """断言：当前页面title为指定字符串
         Asserts whether the current title is in line with expectations.
 
         Usage:
         self.assertTitle("title")
         """
         if title is None:
             raise AssertionError("The assertion title cannot be empty.")
 
-        logger.info(f"👀 assertTitle -> {title}.")
-        for _ in range(GlobalContext.timeout + 1):
+        logger.info(IconMsg.check(f"assertTitle -> {title}."))
+        for _ in range(1, GlobalContext.timeout + 1):
             try:
-                self.assertEqual(title, GlobalContext.driver.title)
+                self.assertEqual(title, GlobalContext.driver.title, msg=f'第{_}/{GlobalContext.timeout}次检查')
+                logger.info(IconMsg.opt_success(f"assert: PASS"))
                 break
             except AssertionError:
                 time.sleep(1)
         else:
             self.assertEqual(title, GlobalContext.driver.title, msg=msg)
 
     def assertInTitle(self, title: str = None, msg: str = None) -> None:
@@ -51,18 +52,19 @@
 
         Usage:
         self.assertInTitle("title")
         """
         if title is None:
             raise AssertionError("The assertion title cannot be empty.")
 
-        logger.info(f"👀 assertInTitle -> {title}.")
-        for _ in range(GlobalContext.timeout + 1):
+        logger.info(IconMsg.check(f"assertInTitle -> {title}."))
+        for _ in range(1, GlobalContext.timeout + 1):
             try:
-                self.assertIn(title, GlobalContext.driver.title)
+                self.assertIn(title, GlobalContext.driver.title, msg=f'第{_}/{GlobalContext.timeout}次检查')
+                logger.info(IconMsg.opt_success(f"assert: PASS"))
                 break
             except AssertionError:
                 time.sleep(1)
         else:
             self.assertIn(title, GlobalContext.driver.title, msg=msg)
 
     def assertUrl(self, url: str = None, msg: str = None) -> None:
@@ -71,58 +73,62 @@
 
         Usage:
         self.assertUrl("url")
         """
         if url is None:
             raise AssertionError("The assertion URL cannot be empty.")
 
-        logger.info(f"👀 assertUrl -> {url}.")
-        for _ in range(GlobalContext.timeout + 1):
+        logger.info(IconMsg.check(f"assertUrl -> {url}."))
+        for _ in range(1, GlobalContext.timeout + 1):
             current_url = unquote(GlobalContext.driver.current_url)
             try:
-                self.assertEqual(url, current_url)
+                self.assertEqual(url, current_url, msg=f'第{_}/{GlobalContext.timeout}次检查')
+                logger.info(IconMsg.opt_success(f"assert: PASS"))
                 break
             except AssertionError:
                 time.sleep(1)
         else:
             self.assertEqual(url, GlobalContext.driver.current_url, msg=msg)
 
     def assertInUrl(self, url: str = None, msg: str = None) -> None:
         """断言：当前URL包含指定url字符"""
         if url is None:
             raise AssertionError("The assertion URL cannot be empty.")
 
-        logger.info(f"👀 assertInUrl -> {url}.")
-        for _ in range(GlobalContext.timeout + 1):
+        logger.info(IconMsg.check(f"assertInUrl -> {url}."))
+        for _ in range(1, GlobalContext.timeout + 1):
             current_url = unquote(GlobalContext.driver.current_url)
             try:
-                self.assertIn(url, current_url)
-
+                self.assertIn(url, current_url, msg=f'第{_}/{GlobalContext.timeout}次检查')
+                logger.info(IconMsg.opt_success(f"assert: PASS"))
                 break
             except AssertionError:
                 time.sleep(1)
         else:
-            self.assertIn(url, GlobalContext.driver.current_url, msg=msg)
+            current_url = GlobalContext.driver.current_url
+            logger.info(IconMsg.check(f"retry assertInUrl -> {url}: {current_url}"))
+            self.assertIn(url, current_url, msg=msg)
 
     def assertText(self, text: str = None, msg: str = None) -> None:
         """
         Asserts whether the text of the current page conforms to expectations.
 
         Usage:
         self.assertText("text")
         """
         if text is None:
             raise AssertionError("The assertion text cannot be empty.")
 
         elem = GlobalContext.driver.find_element(By.TAG_NAME, "html")
-        logger.info(f"👀 assertText -> {text}.")
-        for _ in range(GlobalContext.timeout + 1):
+        logger.info(IconMsg.check(f"assertText -> {text}."))
+        for _ in range(1, GlobalContext.timeout + 1):
             if elem.is_displayed():
                 try:
-                    self.assertIn(text, elem.text)
+                    self.assertIn(text, elem.text, msg=f'第{_}/{GlobalContext.timeout}次检查')
+                    logger.info(IconMsg.opt_success(f"assert: PASS"))
                     break
                 except AssertionError:
                     time.sleep(1)
         else:
             self.assertIn(text, elem.text, msg=msg)
 
     def assertNotText(self, text: str = None, msg: str = None) -> None:
@@ -133,54 +139,56 @@
         self.assertNotText("text")
         """
         if text is None:
             raise AssertionError("The assertion text cannot be empty.")
 
         elem = GlobalContext.driver.find_element(By.TAG_NAME, "html")
 
-        logger.info(f"👀 assertNotText -> {text}.")
-        for _ in range(GlobalContext.timeout + 1):
+        logger.info(IconMsg.check(f"assertNotText -> {text}."))
+        for _ in range(1, GlobalContext.timeout + 1):
             if elem.is_displayed():
                 try:
-                    self.assertNotIn(text, elem.text)
+                    self.assertNotIn(text, elem.text, msg=f'第{_}/{GlobalContext.timeout}次检查')
+                    logger.info(IconMsg.opt_success(f"assert: PASS"))
                     break
                 except AssertionError:
                     time.sleep(1)
         else:
             self.assertNotIn(text, elem.text, msg=msg)
 
     def assertAlertText(self, text: str = None, msg: str = None) -> None:
         """断言：警告提示文本中包含指定字符串"""
         if text is None:
             raise NameError("Alert text cannot be empty.")
 
-        logger.info(f"👀 assertAlertText -> {text}.")
+        logger.info(IconMsg.check(f"assertAlertText -> {text}."))
         alert_text = GlobalContext.driver.switch_to.alert.text
-        for _ in range(GlobalContext.timeout + 1):
+        for _ in range(1, GlobalContext.timeout + 1):
             try:
-                self.assertEqual(alert_text, text, msg=msg)
+                self.assertEqual(alert_text, text, msg=f'{msg}，第{_}/{GlobalContext.timeout}次检查')
+                logger.info(IconMsg.opt_success(f"assert: PASS"))
                 break
             except AssertionError:
                 time.sleep(1)
         else:
             self.assertEqual(alert_text, text, msg=msg)
 
     def assertElement(self, index: int = 0, msg: str = None, **kwargs) -> None:
         """
         Asserts whether the element exists.
 
         Usage:
         self.assertElement(css="#id")
         """
-        logger.info("👀 assertElement.")
+        logger.info(IconMsg.check(f"assertElement -> {index}."))
         if msg is None:
             msg = "No element found"
 
         elem = True
-        for _ in range(GlobalContext.timeout + 1):
+        for _ in range(1, GlobalContext.timeout + 1):
             try:
                 self.get_element(index=index, **kwargs)
                 elem = True
                 break
             except NotFindElementError:
                 elem = False
                 time.sleep(1)
@@ -190,15 +198,15 @@
     def assertNotElement(self, index: int = 0, msg: str = None, **kwargs) -> None:
         """
         Asserts if the element does not exist.
 
         Usage:
         self.assertNotElement(css="#id")
         """
-        logger.info("👀 assertNotElement.")
+        logger.info(IconMsg.check(f"assertNotElement -> {index}."))
         if msg is None:
             msg = "Find the element"
 
         timeout_backups = GlobalContext.timeout
         GlobalContext.timeout = 2
         try:
             self.get_element(index=index, **kwargs)
@@ -211,15 +219,15 @@
         self.assertFalse(elem, msg=msg)
 
     def assertInElement(self, index: int = 0, text: str = None, msg: str = None, **kwargs) -> None:
         """断言element存在且text包含指定字符串"""
         if text is None:
             raise AssertionError("The assertion text cannot be empty.")
 
-        logger.info(f"👀 assertInElement -> {text}.")
+        logger.info(IconMsg.check(f"assertInElement -> {text}."))
         if msg is None:
             msg = "No element found"
         elem = None
         for _ in range(GlobalContext.timeout + 1):
             try:
                 elem = self.get_element(index=index, **kwargs)
                 break
```

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/web/webdriver.py` & `flexrunner-1.0.9/flexrunner/core/runners/web/webdriver.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from selenium.webdriver.support.select import Select
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.chrome.service import Service as cService
 from selenium.webdriver.remote.remote_connection import LOGGER as S_LOGGER
 from loguru import logger
 
 from flexrunner.global_context import GlobalContext
+from flexrunner.core.runners.icon_msg import IconMsg
 from flexrunner.core.runners.web.exceptions import NotFindElementError
 from flexrunner.core.runners.web.webdriver_manager_extend import ChromeDriverManager
 from flexrunner.core.data_factory.random_func import get_timestamp
 
 
 __all__ = ["WebDriver", "WebElement"]
 
@@ -70,15 +71,15 @@
         for _ in range(GlobalContext.timeout):
             elems = GlobalContext.driver.find_elements(by=elem[0], value=elem[1])
             if len(elems) >= 1:
                 self.find_elem_info = f"Find {len(elems)} element: {elem[0]}={elem[1]} "
                 break
             time.sleep(1)
         else:
-            self.find_elem_warn = f"❌ Find 0 element through: {elem[0]}={elem[1]}"
+            self.find_elem_warn = IconMsg.opt_fail(f"Find 0 element through: {elem[0]}={elem[1]}")
 
     def get_elements(self, index: int = None):
         """
         Judge element positioning way, and returns the element.
         """
 
         if self.by == "id_":
@@ -163,74 +164,74 @@
 
         def __init__(self, index: int = 0, **kwargs) -> None:
             self.web_elem = WebElement(**kwargs)
             self.elem = self.web_elem.get_elements(index)
             self.web_elem.show_element(self.elem)
 
         def input(self, text="") -> None:
-            logger.info(f"✅ {self.web_elem.info}, input '{text}'.")
+            logger.info(IconMsg.opt(f"{self.web_elem.info}, input '{text}'."))
             self.elem.send_keys(text)
 
         def enter(self) -> None:
-            logger.info(f"✅ {self.web_elem.info}, enter.")
+            logger.info(IconMsg.opt(f"{self.web_elem.info}, enter."))
             self.elem.send_keys(Keys.ENTER)
 
         def select_all(self) -> None:
-            logger.info(f"✅ {self.web_elem.info}, ctrl+a.")
+            logger.info(IconMsg.opt(f"{self.web_elem.info}, ctrl+a."))
             if platform.system().lower() == "darwin":
                 self.elem.send_keys(Keys.COMMAND, "a")
             else:
                 self.elem.send_keys(Keys.CONTROL, "a")
 
         def cut(self) -> None:
-            logger.info(f"✅ {self.web_elem.info}, ctrl+x.")
+            logger.info(IconMsg.opt(f"{self.web_elem.info}, ctrl+x."))
             if platform.system().lower() == "darwin":
                 self.elem.send_keys(Keys.COMMAND, "x")
             else:
                 self.elem.send_keys(Keys.CONTROL, "x")
 
         def copy(self) -> None:
-            logger.info(f"✅ {self.web_elem.info}, ctrl+c.")
+            logger.info(IconMsg.opt(f"{self.web_elem.info}, ctrl+c."))
             if platform.system().lower() == "darwin":
                 self.elem.send_keys(Keys.COMMAND, "c")
             else:
                 self.elem.send_keys(Keys.CONTROL, "c")
 
         def paste(self) -> None:
-            logger.info(f"✅ {self.web_elem.info}, ctrl+v.")
+            logger.info(IconMsg.opt(f"{self.web_elem.info}, ctrl+v."))
             if platform.system().lower() == "darwin":
                 self.elem.send_keys(Keys.COMMAND, "v")
             else:
                 self.elem.send_keys(Keys.CONTROL, "v")
 
         def backspace(self) -> None:
-            logger.info(f"✅ {self.web_elem.info}, backspace.")
+            logger.info(IconMsg.opt(f"{self.web_elem.info}, backspace."))
             self.elem.send_keys(Keys.BACKSPACE)
 
         def delete(self) -> None:
-            logger.info(f"✅ {self.web_elem.info}, delete.")
+            logger.info(IconMsg.opt(f"{self.web_elem.info}, delete."))
             self.elem.send_keys(Keys.DELETE)
 
         def tab(self) -> None:
-            logger.info(f"✅ {self.web_elem.info}, tab.")
+            logger.info(IconMsg.opt(f"{self.web_elem.info}, tab."))
             self.elem.send_keys(Keys.TAB)
 
         def space(self) -> None:
-            logger.info(f"✅ {self.web_elem.info}, space.")
+            logger.info(IconMsg.opt(f"{self.web_elem.info}, space."))
             self.elem.send_keys(Keys.SPACE)
 
     @staticmethod
     def visit(url: str) -> None:
         """
         visit url.
 
         Usage:
             self.visit("https://www.baidu.com")
         """
-        logger.info(f"📖 {url}")
+        logger.info(IconMsg.opt_visit_url(f"{url}"))
         if isinstance(GlobalContext.driver, SeleniumWebDriver) is False:
             GlobalContext.driver = Chrome(service=cService(ChromeDriverManager().install()))
         GlobalContext.driver.get(url)
 
     def open(self, url: str) -> None:
         """
         open url.
@@ -279,17 +280,17 @@
         """
         if clear is True:
             self.clear(index, **kwargs)
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
         if enter is True:
-            logger.info(f"✅ {web_elem.info} -> input '{text}' and enter.")
+            logger.info(IconMsg.opt(f"{web_elem.info} -> input '{text}' and enter."))
         else:
-            logger.info(f"✅ {web_elem.info} -> input '{text}'.")
+            logger.info(IconMsg.opt(f"{web_elem.info} -> input '{text}'."))
         elem.send_keys(text)
         if enter is True:
             elem.send_keys(Keys.ENTER)
 
     def type_enter(self, text: str, clear: bool = False, index: int = 0, **kwargs) -> None:
         """
         Enter text and enter directly.
@@ -306,86 +307,86 @@
 
         Usage:
             self.clear(css="#el")
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
-        logger.info(f"✅ {web_elem.info} -> clear input.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> clear input."))
         elem.clear()
 
     @staticmethod
     def click(index: int = 0, **kwargs) -> None:
         """
         It can click any text / image can be clicked
         Connection, check box, radio buttons, and even drop-down box etc..
 
         Usage:
             self.click(css="#el")
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
-        logger.info(f"✅ {web_elem.info} -> click.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> click."))
         elem.click()
 
     @staticmethod
     def slow_click(index: int = 0, **kwargs) -> None:
         """
         Moving the mouse to the middle of an element. and click element.
 
         Usage:
             self.slow_click(css="#el")
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
-        logger.info(f"✅ {web_elem.info} -> slow click.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> slow click."))
         ActionChains(GlobalContext.driver).move_to_element(elem).click(elem).perform()
 
     @staticmethod
     def right_click(index: int = 0, **kwargs) -> None:
         """
         Right click element.
 
         Usage:
             self.right_click(css="#el")
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
-        logger.info(f"✅ {web_elem.info} -> right click.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> right click."))
         ActionChains(GlobalContext.driver).context_click(elem).perform()
 
     @staticmethod
     def move_to_element(index: int = 0, **kwargs) -> None:
         """
         Mouse over the element.
 
         Usage:
             self.move_to_element(css="#el")
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
-        logger.info(f"✅ {web_elem.info} -> move to element.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> move to element."))
         ActionChains(GlobalContext.driver).move_to_element(elem).perform()
 
     @staticmethod
     def click_and_hold(index: int = 0, **kwargs) -> None:
         """
         Mouse over the element.
 
         Usage:
             self.move_to_element(css="#el")
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
-        logger.info(f"✅ {web_elem.info} -> click and hold.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> click and hold."))
         ActionChains(GlobalContext.driver).click_and_hold(elem).perform()
 
     @staticmethod
     def drag_and_drop_by_offset(index: int = 0, x: int = 0, y: int = 0, **kwargs) -> None:
         """
         Holds down the left mouse button on the source element,
            then moves to the target offset and releases the mouse button.
@@ -395,43 +396,43 @@
          - x: X offset to move to.
          - y: Y offset to move to.
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
         action = ActionChains(GlobalContext.driver)
-        logger.info(f"✅ {web_elem.info} -> drag and drop by offset.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> drag and drop by offset."))
         action.drag_and_drop_by_offset(elem, x, y).perform()
 
     @staticmethod
     def double_click(index: int = 0, **kwargs) -> None:
         """
         Double click element.
 
         Usage:
             self.double_click(css="#el")
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
-        logger.info(f"✅ {web_elem.info} -> double click.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> double click."))
         ActionChains(GlobalContext.driver).double_click(elem).perform()
 
     @staticmethod
     def click_text(text: str, index: int = 0) -> None:
         """
         Click the element by the link text
 
         Usage:
             self.click_text("新闻")
         """
         web_elem = WebElement(link_text=text)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
-        logger.info(f"✅ {web_elem.info} -> click link.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> click link."))
         elem.click()
 
     @staticmethod
     def close() -> None:
         """
         Closes the current window.
 
@@ -459,26 +460,26 @@
 
         Usage:
             driver.submit(css="#el")
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
-        logger.info(f"✅ {web_elem.info} -> submit.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> submit."))
         elem.submit()
 
     @staticmethod
     def refresh() -> None:
         """
         Refresh the current page.
 
         Usage:
             self.refresh()
         """
-        logger.info("🔄️ refresh page.")
+        logger.info(IconMsg.opt_refresh("refresh page."))
         GlobalContext.driver.refresh()
 
     @staticmethod
     def execute_script(script: str, *args):
         """
         Execute JavaScript scripts.
 
@@ -518,177 +519,177 @@
             self.get_attribute(css="#el", attribute="type")
         """
         if attribute is None:
             raise ValueError("attribute is not None")
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
-        logger.info(f"✅ {web_elem.info} -> get attribute：{attribute}.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> get attribute：{attribute}."))
         return elem.get_attribute(attribute)
 
     @staticmethod
     def get_text(index: int = 0, **kwargs) -> str:
         """
         Get element text information.
 
         Usage:
             self.get_text(css="#el")
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
-        logger.info(f"✅ {web_elem.info} -> get text: {elem.text}.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> get text: {elem.text}."))
         return elem.text
 
     @staticmethod
     def get_display(index: int = 0, **kwargs) -> bool:
         """
         Gets the element to display,The return result is true or false.
 
         Usage:
             self.get_display(css="#el")
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
         result = elem.is_displayed()
-        logger.info(f"✅ {web_elem.info} -> element is display: {result}.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> element is display: {result}."))
         return result
 
     @property
     def get_title(self) -> str:
         """
         Get window title.
 
         Usage:
             self.get_title()
         """
-        logger.info(f"✅ get title: {GlobalContext.driver.title}.")
+        logger.info(IconMsg.opt(f"get title: {GlobalContext.driver.title}."))
         return GlobalContext.driver.title
 
     @property
     def get_url(self) -> str:
         """
         Get the URL address of the current page.
 
         Usage:
             self.get_url()
         """
-        logger.info(f"✅ get current url: {GlobalContext.driver.current_url}.")
+        logger.info(IconMsg.opt(f"get current url: {GlobalContext.driver.current_url}."))
         return GlobalContext.driver.current_url
 
     @property
     def get_alert_text(self) -> str:
         """
         Gets the text of the Alert.
 
         Usage:
             self.get_alert_text()
         """
-        logger.info(f"✅ alert text: {GlobalContext.driver.switch_to.alert.text}.")
+        logger.info(IconMsg.opt(f"alert text: {GlobalContext.driver.switch_to.alert.text}."))
         return GlobalContext.driver.switch_to.alert.text
 
     @staticmethod
     def wait(secs: int = 10) -> None:
         """
         Implicitly wait.All elements on the page.
 
         Usage:
             self.wait(10)
         """
-        logger.info(f"⌛️ implicitly wait: {secs}s.")
+        logger.info(IconMsg.opt_wait(f"implicitly wait: {secs}s."))
         GlobalContext.driver.implicitly_wait(secs)
 
     @staticmethod
     def accept_alert() -> None:
         """
         Accept warning box.
 
         Usage:
             self.accept_alert()
         """
-        logger.info("✅ accept alert.")
+        logger.info(IconMsg.opt("accept alert."))
         GlobalContext.driver.switch_to.alert.accept()
 
     @staticmethod
     def dismiss_alert() -> None:
         """
         Dismisses the alert available.
 
         Usage:
             self.dismiss_alert()
         """
-        logger.info("✅ dismiss alert.")
+        logger.info(IconMsg.opt("dismiss alert."))
         GlobalContext.driver.switch_to.alert.dismiss()
 
     @staticmethod
     def switch_to_frame(index: int = 0, **kwargs) -> None:
         """
         Switch to the specified frame.
 
         Usage:
             self.switch_to_frame(css="#el")
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
         web_elem.show_element(elem)
-        logger.info(f"✅ {web_elem.info} -> switch to frame.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> switch to frame."))
         GlobalContext.driver.switch_to.frame(elem)
 
     @staticmethod
     def switch_to_frame_parent() -> None:
         """
         Switches focus to the parent context. If the current context is the top
         level browsing context, the context remains unchanged.
 
         Usage:
             self.switch_to_frame_parent()
         """
-        logger.info("✅ switch to parent frame.")
+        logger.info(IconMsg.opt("switch to parent frame."))
         GlobalContext.driver.switch_to.parent_frame()
 
     @staticmethod
     def switch_to_frame_out() -> None:
         """
         Returns the current form machine form at the next higher level.
         Corresponding relationship with switch_to_frame () method.
 
         Usage:
             self.switch_to_frame_out()
         """
-        logger.info("✅ switch to frame out.")
+        logger.info(IconMsg.opt("switch to frame out."))
         GlobalContext.driver.switch_to.default_content()
 
     @staticmethod
     def switch_to_window(window: int) -> None:
         """
         Switches focus to the specified window.
 
         :Args:
          - window: window index. 1 represents a newly opened window (0 is the first one)
 
         :Usage:
             self.switch_to_window(1)
         """
-        logger.info(f"✅ switch to the {window} window.")
+        logger.info(IconMsg.opt(f"switch to the {window} window."))
         all_handles = GlobalContext.driver.window_handles
         GlobalContext.driver.switch_to.window(all_handles[window])
 
     @staticmethod
     def switch_to_new_window(type_hint=None) -> None:
         """
         Switches to a new top-level browsing context.
 
         The type hint can be one of "tab" or "window". If not specified the
         browser will automatically select it.
 
         :Usage:
             self.switch_to_new_window('tab')
         """
-        logger.info("✅ switch to new window.")
+        logger.info(IconMsg.opt("switch to new window."))
         GlobalContext.driver.switch_to.new_window(type_hint=type_hint)
 
     def screenshots(self, file_path: str = None) -> None:
         """
         Saves a screenshots of the current window to a PNG image file.
 
         Usage:
@@ -697,18 +698,18 @@
         """
         if file_path is None:
             img_dir = os.path.join(os.getcwd(), "reports", "images")
             if os.path.exists(img_dir) is False:
                 os.mkdir(img_dir)
             file_path = os.path.join(img_dir, get_timestamp() + ".png")
         if GlobalContext.debug is True:
-            logger.info(f"📷️  screenshot -> ({file_path}).")
+            logger.info(IconMsg.screenshot(f"screenshot -> ({file_path})."))
             GlobalContext.driver.save_screenshot(file_path)
         else:
-            logger.info("📷️  screenshot -> HTML report.")
+            logger.info(IconMsg.screenshot("screenshot -> HTML report."))
             self.images.append(GlobalContext.driver.get_screenshot_as_base64())
 
     def element_screenshot(self, file_path: str = None, index: int = 0, **kwargs) -> None:
         """
         Saves a element screenshot of the element to a PNG image file.
 
         Usage:
@@ -720,18 +721,18 @@
         elem = web_elem.get_elements(index)
         if file_path is None:
             img_dir = os.path.join(os.getcwd(), "reports", "images")
             if os.path.exists(img_dir) is False:
                 os.mkdir(img_dir)
             file_path = os.path.join(img_dir, get_timestamp() + ".png")
         if GlobalContext.debug is True:
-            logger.info(f"📷️ element screenshot -> ({file_path}).")
+            logger.info(IconMsg.screenshot(f"element screenshot -> ({file_path})."))
             elem.screenshot(file_path)
         else:
-            logger.info("📷️ element screenshot -> HTML Report.")
+            logger.info(IconMsg.screenshot("element screenshot -> HTML Report."))
             self.images.append(elem.screenshot_as_base64)
 
     @staticmethod
     def select(value: str = None, text: str = None, index: int = None, **kwargs) -> None:
         """
         Constructor. A check is made that the given element is, indeed, a SELECT tag. If it is not,
         then an UnexpectedTagNameException is thrown.
@@ -750,15 +751,15 @@
             self.select(css="#nr", value='20')
             self.select(css="#nr", text='每页显示20条')
             self.select(css="#nr", index=2)
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(0)
         web_elem.show_element(elem)
-        logger.info(f"✅ {web_elem.info} -> select option.")
+        logger.info(IconMsg.opt(f"{web_elem.info} -> select option."))
         if value is not None:
             Select(elem).select_by_value(value)
         elif text is not None:
             Select(elem).select_by_visible_text(text)
         elif index is not None:
             Select(elem).select_by_index(index)
         else:
@@ -835,29 +836,29 @@
 
     @staticmethod
     def sleep(sec: int) -> None:
         """
         Usage:
             self.sleep(seconds)
         """
-        logger.info(f"💤️ sleep: {sec}s.")
+        logger.info(IconMsg.opt_sleep(f"💤️ sleep: {sec}s."))
         time.sleep(sec)
 
     @staticmethod
     def check_element(css: str = None) -> None:
         """
         Check that the element exists
 
         Usage:
         self.check_element(css="#el")
         """
         if css is None:
             raise NameError("Please enter a CSS selector")
 
-        logger.info("👀 check element.")
+        logger.info(IconMsg.check("check element."))
         js = f'return document.querySelectorAll("{css}")'
         ret = GlobalContext.driver.execute_script(js)
         if len(ret) > 0:
             for i in range(len(ret)):
                 js = f'return document.querySelectorAll("{css}")[{i}].outerHTML;'
                 ret = GlobalContext.driver.execute_script(js)
                 logger.info(f"{i} -> {ret}")
@@ -874,49 +875,49 @@
         print(len(ret))
         """
         web_elem = WebElement(**kwargs)
         elems = web_elem.get_elements()
         if len(elems) == 0:
             logger.warning(f"{web_elem.warn}.")
         else:
-            logger.info(f"✅ {web_elem.info}.")
+            logger.info(IconMsg.opt(f"{web_elem.info}."))
         return elems
 
     @staticmethod
     def get_element(index: int = 0, **kwargs):
         """
         Get a set of elements
 
         Usage:
         elem = self.get_element(index=1, css="#el")
         elem.click()
         """
         web_elem = WebElement(**kwargs)
         elem = web_elem.get_elements(index)
-        logger.info(f"✅ {web_elem.info}.")
+        logger.info(IconMsg.opt(f"{web_elem.info}."))
         return elem
 
     @staticmethod
     def switch_to_app() -> None:
         """
         appium API
         Switch to native app.
         """
-        logger.info("🔀 switch to native app.")
+        logger.info(IconMsg.opt_switch("switch to native app."))
         current_context = GlobalContext.driver.current_context
         if current_context != "NATIVE_APP":
             GlobalContext.driver.switch_to.context('NATIVE_APP')
 
     @staticmethod
     def switch_to_web(context=None) -> None:
         """
         appium API
         Switch to web view.
         """
-        logger.info("🔀 switch to webview.")
+        logger.info(IconMsg.opt("switch to webview."))
         current_context = GlobalContext.driver.current_context
         if context is not None:
             GlobalContext.driver.switch_to.context(context)
         elif "WEBVIEW" in current_context:
             return
         else:
             all_context = GlobalContext.driver.contexts
@@ -929,15 +930,15 @@
 
     @staticmethod
     def switch_to_flutter() -> None:
         """
         appium API
         Switch to flutter app.
         """
-        logger.info("🔀 switch to flutter.")
+        logger.info(IconMsg.opt("switch to flutter."))
         current_context = GlobalContext.driver.current_context
         if current_context != "NATIVE_APP":
             GlobalContext.driver.switch_to.context('FLUTTER')
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `flexrunner-1.0.8/flexrunner/core/runners/web/webdriver_manager_extend.py` & `flexrunner-1.0.9/flexrunner/core/runners/web/webdriver_manager_extend.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/libs/jenkins_opt.py` & `flexrunner-1.0.9/flexrunner/pkgs/jenkins_opt.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/libs/mysql_opt.py` & `flexrunner-1.0.9/flexrunner/pkgs/mysql_opt.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/libs/sqlalchemy_opt.py` & `flexrunner-1.0.9/flexrunner/pkgs/sqlalchemy_opt.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,47 +7,50 @@
 @email:tao.xu2008@outlook.com
 @description:
 """
 import os
 import unittest
 from loguru import logger
 
-from flexrunner.config import root_dir, DB_INFO
+from flexrunner.config import REPORT_DIR
 from sqlalchemy import Column, String, create_engine, Integer
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
 
 # 创建对象的基类:
 Base = declarative_base()
+DEFAULT_DB_INFO = {"ENGINE": 'django.db.backends.sqlite3', "NAME": 'db.sqlite3'}
 
 
 class SqlalchemyOperation(object):
     """sqlalchemy ORM操作"""
-    def __init__(self, db_info):
+    def __init__(self, db_info=None):
+        if db_info is None:
+            db_info = DEFAULT_DB_INFO
         self.db_info = db_info
         self.engine = None
         self.create_engine()
 
         # 创建DBSession类型:
         self.db_session = sessionmaker(bind=self.engine)
         # 创建session对象:
         self.session = self.db_session()
 
     def create_engine(self):
-        if DB_INFO.get('ENGINE') == 'django.db.backends.sqlite3':
-            # db_path = db_info.get('NAME')
-            db_path = os.path.abspath(os.path.join(root_dir, 'test_db.sqlite3'))
+        if self.db_info.get('ENGINE') == 'django.db.backends.sqlite3':
+            # db_path = self.db_info.get('NAME')
+            db_path = os.path.abspath(os.path.join(REPORT_DIR, 'test_db.sqlite3'))
             logger.info(db_path)
             self.engine = create_engine(r'sqlite:///{}'.format(db_path))
-        elif DB_INFO.get('ENGINE') == 'django.db.backends.mysql':
-            user = DB_INFO.get('USER')
-            password = DB_INFO.get('PASSWORD')
-            host = DB_INFO.get('HOST')
-            port = DB_INFO.get('PORT')
-            name = DB_INFO.get('NAME')
+        elif self.db_info.get('ENGINE') == 'django.db.backends.mysql':
+            user = self.db_info.get('USER')
+            password = self.db_info.get('PASSWORD')
+            host = self.db_info.get('HOST')
+            port = self.db_info.get('PORT')
+            name = self.db_info.get('NAME')
             self.engine = create_engine('mysql+pymysql://root:******@localhost:3306/scheduler')
         else:
             logger.critical("错误的数据库类型，将跳过结果写入！")
 
     # 创建所有定义的表到数据库中
     def init_db(self):
         Base.metadata.create_all(self.engine)
```

### Comparing `flexrunner-1.0.8/flexrunner/libs/sqlite_opt.py` & `flexrunner-1.0.9/flexrunner/pkgs/sqlite_opt.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/notification/qw_chat.py` & `flexrunner-1.0.9/flexrunner/notification/qw_chat.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/utils/dsl_helper.py` & `flexrunner-1.0.9/flexrunner/utils/dsl_helper.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/utils/file_helper.py` & `flexrunner-1.0.9/flexrunner/utils/file_helper.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/utils/pkg_helper.py` & `flexrunner-1.0.9/flexrunner/utils/pkg_helper.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/utils/retry.py` & `flexrunner-1.0.9/flexrunner/utils/retry.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/utils/singleton.py` & `flexrunner-1.0.9/flexrunner/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner/utils/util.py` & `flexrunner-1.0.9/flexrunner/utils/util.py`

 * *Files identical despite different names*

### Comparing `flexrunner-1.0.8/flexrunner.egg-info/PKG-INFO` & `flexrunner-1.0.9/flexrunner.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: flexrunner
-Version: 1.0.8
+Version: 1.0.9
+Summary: UNKNOWN
 Home-page: https://github.com/txu2k8/test-runner-flex
 Author: TXU
 Author-email: tao.xu2008@outlook.com
 Maintainer: TXU
 Maintainer-email: tao.xu2008@outlook.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
@@ -51,7 +53,8 @@
 
 ```
 
 ## 测试demo环境搭建
 ```
 .\minio.exe server D:\minio\data\ --console-address 127.0.0.1:9001
 ```
+
```

### Comparing `flexrunner-1.0.8/flexrunner.egg-info/requires.txt` & `flexrunner-1.0.9/flexrunner.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,40 @@
-PyMySQL==1.0.2
+pymysql
 pytz==2022.1
 six==1.16.0
 sqlparse==0.4.2
 tzdata==2022.1
 loguru==0.5.3
-pydantic~=1.9.0
+pydantic~=1.10.4
 prettytable~=3.0.0
 progressbar~=2.5
 Jinja2~=3.0.3
-pytest~=6.2.5
+pytest~=7.2.1
+pytest-ordering==0.6
+pytest-xdist==3.2.1
 pytest-html==3.1.1
 pytest-flexreport
+pytest-json-report
 pytest-dependency==0.5.1
 allure-pytest==2.9.45
 requests~=2.27.1
 urllib3~=1.26.8
 filetype~=1.0.10
+filelock~=3.10.0
 requests-toolbelt~=0.9.1
 PyYAML~=6.0
 jsonpath==0.82
 jmespath==0.10.0
 xmindparser~=1.0.9
 pypinyin~=0.44.0
 arrow~=1.2.1
 Faker~=15.3.4
 python-jenkins==1.7.0
 py~=1.11.0
 selenium~=4.3.0
 APScheduler~=3.9.1
 typer~=0.6.1
-SQLAlchemy
+SQLAlchemy~=1.4.44
 webdriver-manager
+setuptools~=67.0.0
+paramiko~=3.0.0
+scp~=0.14.5
```

### Comparing `flexrunner-1.0.8/requirements.txt` & `flexrunner-1.0.9/requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,40 @@
-﻿PyMySQL==1.0.2
+﻿pymysql
 pytz==2022.1
 six==1.16.0
 sqlparse==0.4.2
 tzdata==2022.1
 loguru==0.5.3
-pydantic~=1.9.0
+pydantic~=1.10.4
 prettytable~=3.0.0
 progressbar~=2.5
 Jinja2~=3.0.3
-pytest~=6.2.5
+pytest~=7.2.1
+pytest-ordering==0.6
+pytest-xdist==3.2.1
 pytest-html==3.1.1
 pytest-flexreport
+pytest-json-report
 pytest-dependency==0.5.1
 allure-pytest==2.9.45
 requests~=2.27.1
 urllib3~=1.26.8
 filetype~=1.0.10
+filelock~=3.10.0
 requests-toolbelt~=0.9.1
 PyYAML~=6.0
 jsonpath==0.82
 jmespath==0.10.0
 xmindparser~=1.0.9
 pypinyin~=0.44.0
 arrow~=1.2.1
 Faker~=15.3.4
 python-jenkins==1.7.0
 py~=1.11.0
 selenium~=4.3.0
 APScheduler~=3.9.1
 typer~=0.6.1
-SQLAlchemy
-webdriver-manager
+SQLAlchemy~=1.4.44
+webdriver-manager
+setuptools~=67.0.0
+paramiko~=3.0.0
+scp~=0.14.5
```

### Comparing `flexrunner-1.0.8/setup.py` & `flexrunner-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import os
 import sys
 import re
 import ast
 from setuptools import setup, find_packages
 
 
-_version_re = re.compile(r'__version__\s+=\s+(.*)')
+_version_re = re.compile(r'VERSION\s+=\s+(.*)')
 
-with open('flexrunner/__init__.py', 'rb') as f:
+with open('flexrunner/config/globals.py', 'rb') as f:
     version = str(ast.literal_eval(_version_re.search(
         f.read().decode('utf-8')).group(1)))
 
 
 # 读取文件内容
 def read_file(filename, encoding='utf-8'):
     cur_dir = os.path.abspath(os.path.dirname(__file__))
```

