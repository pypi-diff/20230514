# Comparing `tmp/TDhelper-2.4.8.tar.gz` & `tmp/TDhelper-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDhelper-2.4.8.tar", last modified: Sun May  7 04:02:33 2023, max compression
+gzip compressed data, was "TDhelper-2.4.9.tar", last modified: Sun May 14 13:34:09 2023, max compression
```

## Comparing `TDhelper-2.4.8.tar` & `TDhelper-2.4.9.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11361 2023-04-03 05:53:54.000000 TDhelper-2.4.8/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-05-07 04:02:33.853343 TDhelper-2.4.8/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2573 2023-04-03 05:53:54.000000 TDhelper-2.4.8/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.813343 TDhelper-2.4.8/TDhelper/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.813343 TDhelper-2.4.8/TDhelper/Decorators/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Decorators/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Decorators/log.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Decorators/performance.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.813343 TDhelper-2.4.8/TDhelper/Event/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4150 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Event/Event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Event/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.813343 TDhelper-2.4.8/TDhelper/Event/classEvent/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Event/classEvent/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1273 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Event/classEvent/event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      966 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Event/classEvent/meta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.813343 TDhelper-2.4.8/TDhelper/Event/webEvent/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31736 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Event/webEvent/Events.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Event/webEvent/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.813343 TDhelper-2.4.8/TDhelper/MagicCls/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/MagicCls/FieldsType.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1740 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/MagicCls/MagicMeta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       74 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/MagicCls/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1978 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/MagicCls/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      892 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/MagicCls/test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.823343 TDhelper-2.4.8/TDhelper/Msg/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1165 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Msg/AppPush.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2564 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Msg/Config.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2170 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Msg/Email.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1438 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Msg/InterfaceMsg.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2113 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Msg/SMS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Msg/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.823343 TDhelper-2.4.8/TDhelper/Scheduler/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Scheduler/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      742 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Scheduler/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      750 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Scheduler/example_scheduler.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      828 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Scheduler/interface.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1620 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Scheduler/log_config.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4208 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Scheduler/service.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.823343 TDhelper-2.4.8/TDhelper/Spider/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/cfg.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8292 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/contentExtraction.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.823343 TDhelper-2.4.8/TDhelper/Spider/models/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      976 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/models/BadRequestModel.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2619 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/models/Cache_L1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1332 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/models/Cache_L2.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2137 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/models/Cache_L2_Model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/models/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/models/fingerprint.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      243 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/models/spider_event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1702 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/models/status.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    43496 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/regex.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/spiderFactory.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10838 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/Spider/spiderPools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       73 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5366 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/apiCore.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.823343 TDhelper-2.4.8/TDhelper/bin/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/bin/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      541 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/bin/globalvar.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.823343 TDhelper-2.4.8/TDhelper/cache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/cache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      948 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/cache/memcache.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1130 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/cache/pools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2739 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/cache/ring.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.823343 TDhelper-2.4.8/TDhelper/cache/webCache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/cache/webCache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/cache/webCache/interface.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-04-26 14:20:15.000000 TDhelper-2.4.8/TDhelper/cache/webCache/mongo.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/cache/webCache/redis.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1221 2023-04-26 14:19:38.000000 TDhelper-2.4.8/TDhelper/cache/webCache/webCacheFactory.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.823343 TDhelper-2.4.8/TDhelper/db/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.823343 TDhelper-2.4.8/TDhelper/db/Db/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/db/Db/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1235 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/db/Db/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      238 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/db/Db/helper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/db/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/db/mongodb/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/db/mongodb/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1102 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/db/mongodb/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3718 2023-04-26 14:07:17.000000 TDhelper-2.4.8/TDhelper/db/mongodb/dbhelper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1919 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/db/mongodb/objectId.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       44 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/db/mongodb/setting.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/db/mysql/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/db/mysql/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      510 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/db/mysql/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/db/mysql/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/db/mysql/mysql_x.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      126 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/db/mysql/setting.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/document/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       24 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/document/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/document/excel/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/document/excel/FieldType/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      104 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/document/excel/FieldType/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       36 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/document/excel/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/document/excel/meta/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/document/excel/meta/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/document/excel/meta/modelMeta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      818 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/document/excel/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      622 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/document/file.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/document/ini/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/document/ini/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      123 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/document/ini/fields.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/document/ini/meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      440 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/document/ini/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      314 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/document/ini/test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/generic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2220 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/generic/a/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/a/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       48 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/a/b.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1402 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/classDocCfg.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/generic/crypto/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1404 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/crypto/MD5.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/crypto/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4668 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/dictHelper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/generic/dynamic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/dynamic/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/generic/dynamic/base/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2582 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/dynamic/base/Meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/dynamic/base/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2825 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/dynamic/test.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1417 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/findAttribute.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      144 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/randGetValue.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1146 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/recursion.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5628 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/requier.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3721 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/standard_result.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4808 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/threadPools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3452 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/generic/transformationType.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/network/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.833343 TDhelper-2.4.8/TDhelper/network/http/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7978 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/http/REST_HTTP.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    61039 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/http/RPC.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    34603 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/http/RPC1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/http/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4663 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/http/http_helper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3588 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/http/http_postdataformat.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26267 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/http/m3u8.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26805 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/http/m3u8_backup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.843343 TDhelper-2.4.8/TDhelper/network/http/status/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      165 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/http/status/M3U8_STATUS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/http/status/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.843343 TDhelper-2.4.8/TDhelper/network/rpc/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.843343 TDhelper-2.4.8/TDhelper/network/rpc/Client/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/Client/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4091 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/Client/rpc.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10831 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/Client/service.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.843343 TDhelper-2.4.8/TDhelper/network/rpc/Core/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2141 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/Core/Meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/Core/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    15661 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/Core/struct.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.843343 TDhelper-2.4.8/TDhelper/network/rpc/Generic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6115 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/Generic/Host.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/Generic/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.843343 TDhelper-2.4.8/TDhelper/network/rpc/Server/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/Server/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7837 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/Server/obsolete_Service.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3839 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/Server/server.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.843343 TDhelper-2.4.8/TDhelper/network/rpc/Struct/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2202 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/Struct/Result.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/Struct/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/rpc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.843343 TDhelper-2.4.8/TDhelper/network/socket/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/socket/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/TDhelper/network/socket/cache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/socket/cache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      518 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/socket/cache/queue.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2371 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/socket/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/TDhelper/network/socket/model/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      757 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/socket/model/SOCKET_MODELS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/socket/model/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/TDhelper/network/socket/protocol/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/socket/protocol/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/socket/protocol/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/socket/server.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/TDhelper/network/websocket/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/websocket/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/websocket/protocol.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/network/websocket/server.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/reflect.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/TDhelper/robot/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/TDhelper/robot/control/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/control/D_33890.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/control/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1296 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/control/device.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/TDhelper/robot/people/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1117 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/people/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5622 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/people/leg.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/TDhelper/robot/people/scripts/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/people/scripts/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3111 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/people/scripts/runScript.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/people/scripts/script.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/people/upperLimb.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/people/vertebra.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/TDhelper/robot/struct/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/struct/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      621 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/struct/ankle.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/struct/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      613 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/struct/hip.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      618 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/struct/knee.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      697 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/robot/struct/toe.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/TDhelper/shellScripts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      335 2023-04-06 02:34:35.000000 TDhelper-2.4.8/TDhelper/shellScripts/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3169 2023-05-07 04:02:03.000000 TDhelper-2.4.8/TDhelper/shellScripts/saasHelper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/TDhelper/simulate/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/simulate/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2713 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/simulate/json.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/TDhelper/structs/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/structs/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4359 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/structs/dir.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.853343 TDhelper-2.4.8/TDhelper/web/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/web/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8255 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/web/permission.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-04-03 05:53:54.000000 TDhelper-2.4.8/TDhelper/web/permissionHelper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 04:02:33.813343 TDhelper-2.4.8/TDhelper.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-05-07 04:02:33.000000 TDhelper-2.4.8/TDhelper.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5532 2023-05-07 04:02:33.000000 TDhelper-2.4.8/TDhelper.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-07 04:02:33.000000 TDhelper-2.4.8/TDhelper.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-05-07 04:02:33.000000 TDhelper-2.4.8/TDhelper.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      754 2023-05-07 04:02:33.000000 TDhelper-2.4.8/TDhelper.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-07 04:02:33.000000 TDhelper-2.4.8/TDhelper.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-07 04:02:33.853343 TDhelper-2.4.8/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-05-07 04:02:15.000000 TDhelper-2.4.8/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.224796 TDhelper-2.4.9/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11361 2023-04-03 05:53:54.000000 TDhelper-2.4.9/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-05-14 13:34:09.224796 TDhelper-2.4.9/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2573 2023-04-03 05:53:54.000000 TDhelper-2.4.9/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.184796 TDhelper-2.4.9/TDhelper/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.184796 TDhelper-2.4.9/TDhelper/Decorators/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Decorators/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Decorators/log.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Decorators/performance.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.184796 TDhelper-2.4.9/TDhelper/Event/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4150 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Event/Event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Event/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.184796 TDhelper-2.4.9/TDhelper/Event/classEvent/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Event/classEvent/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1273 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Event/classEvent/event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      966 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Event/classEvent/meta.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.184796 TDhelper-2.4.9/TDhelper/Event/webEvent/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31736 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Event/webEvent/Events.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Event/webEvent/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.184796 TDhelper-2.4.9/TDhelper/MagicCls/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/MagicCls/FieldsType.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1740 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/MagicCls/MagicMeta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       74 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/MagicCls/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1978 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/MagicCls/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      892 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/MagicCls/test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.194796 TDhelper-2.4.9/TDhelper/Msg/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1165 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Msg/AppPush.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2564 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Msg/Config.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2170 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Msg/Email.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1438 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Msg/InterfaceMsg.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2113 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Msg/SMS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Msg/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.194796 TDhelper-2.4.9/TDhelper/Scheduler/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Scheduler/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      742 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Scheduler/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      750 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Scheduler/example_scheduler.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      828 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Scheduler/interface.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1620 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Scheduler/log_config.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4208 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Scheduler/service.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.194796 TDhelper-2.4.9/TDhelper/Spider/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Spider/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Spider/cfg.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8292 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Spider/contentExtraction.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.194796 TDhelper-2.4.9/TDhelper/Spider/models/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      976 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Spider/models/BadRequestModel.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2619 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Spider/models/Cache_L1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1332 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Spider/models/Cache_L2.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2137 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Spider/models/Cache_L2_Model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Spider/models/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Spider/models/fingerprint.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      243 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Spider/models/spider_event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1702 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Spider/models/status.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    43496 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Spider/regex.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/Spider/spiderFactory.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10838 2023-05-14 08:23:04.000000 TDhelper-2.4.9/TDhelper/Spider/spiderPools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       73 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5366 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/apiCore.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.194796 TDhelper-2.4.9/TDhelper/bin/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/bin/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      541 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/bin/globalvar.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.194796 TDhelper-2.4.9/TDhelper/cache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/cache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      948 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/cache/memcache.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1130 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/cache/pools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2739 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/cache/ring.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.194796 TDhelper-2.4.9/TDhelper/cache/webCache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/cache/webCache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/cache/webCache/interface.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-04-26 14:20:15.000000 TDhelper-2.4.9/TDhelper/cache/webCache/mongo.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/cache/webCache/redis.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1221 2023-04-26 14:19:38.000000 TDhelper-2.4.9/TDhelper/cache/webCache/webCacheFactory.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.194796 TDhelper-2.4.9/TDhelper/db/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.194796 TDhelper-2.4.9/TDhelper/db/Db/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/db/Db/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1235 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/db/Db/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      238 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/db/Db/helper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/db/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.194796 TDhelper-2.4.9/TDhelper/db/mongodb/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/db/mongodb/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1102 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/db/mongodb/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3718 2023-04-26 14:07:17.000000 TDhelper-2.4.9/TDhelper/db/mongodb/dbhelper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1919 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/db/mongodb/objectId.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       44 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/db/mongodb/setting.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.194796 TDhelper-2.4.9/TDhelper/db/mysql/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/db/mysql/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      510 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/db/mysql/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/db/mysql/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/db/mysql/mysql_x.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      126 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/db/mysql/setting.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.194796 TDhelper-2.4.9/TDhelper/document/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       24 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/document/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.194796 TDhelper-2.4.9/TDhelper/document/excel/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.204796 TDhelper-2.4.9/TDhelper/document/excel/FieldType/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      104 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/document/excel/FieldType/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       36 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/document/excel/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.204796 TDhelper-2.4.9/TDhelper/document/excel/meta/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/document/excel/meta/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/document/excel/meta/modelMeta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      818 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/document/excel/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      622 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/document/file.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.204796 TDhelper-2.4.9/TDhelper/document/ini/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/document/ini/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      123 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/document/ini/fields.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/document/ini/meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      440 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/document/ini/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      314 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/document/ini/test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.204796 TDhelper-2.4.9/TDhelper/generic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2220 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.204796 TDhelper-2.4.9/TDhelper/generic/a/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/a/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       48 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/a/b.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1402 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/classDocCfg.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.204796 TDhelper-2.4.9/TDhelper/generic/crypto/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1404 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/crypto/MD5.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/crypto/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4668 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/dictHelper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.204796 TDhelper-2.4.9/TDhelper/generic/dynamic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/dynamic/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.204796 TDhelper-2.4.9/TDhelper/generic/dynamic/base/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2582 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/dynamic/base/Meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/dynamic/base/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2825 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/dynamic/test.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1417 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/findAttribute.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      144 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/randGetValue.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1146 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/recursion.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5628 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/requier.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3721 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/standard_result.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4808 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/generic/threadPools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3886 2023-05-14 08:06:04.000000 TDhelper-2.4.9/TDhelper/generic/transformationType.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.204796 TDhelper-2.4.9/TDhelper/network/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.204796 TDhelper-2.4.9/TDhelper/network/http/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7978 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/http/REST_HTTP.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    61039 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/http/RPC.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    34603 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/http/RPC1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/http/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4663 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/http/http_helper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3588 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/http/http_postdataformat.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26267 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/http/m3u8.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26805 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/http/m3u8_backup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.204796 TDhelper-2.4.9/TDhelper/network/http/status/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      165 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/http/status/M3U8_STATUS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/http/status/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.204796 TDhelper-2.4.9/TDhelper/network/rpc/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/network/rpc/Client/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/rpc/Client/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4800 2023-05-14 13:08:38.000000 TDhelper-2.4.9/TDhelper/network/rpc/Client/rpc.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10831 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/rpc/Client/service.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/network/rpc/Core/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2141 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/rpc/Core/Meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/rpc/Core/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    15829 2023-05-14 13:08:22.000000 TDhelper-2.4.9/TDhelper/network/rpc/Core/struct.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/network/rpc/Generic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7381 2023-05-14 10:09:53.000000 TDhelper-2.4.9/TDhelper/network/rpc/Generic/Host.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/rpc/Generic/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/network/rpc/Server/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/rpc/Server/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7837 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/rpc/Server/obsolete_Service.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4207 2023-05-14 12:54:46.000000 TDhelper-2.4.9/TDhelper/network/rpc/Server/server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/network/rpc/Struct/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2202 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/rpc/Struct/Result.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/rpc/Struct/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/rpc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/network/socket/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/socket/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/network/socket/cache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/socket/cache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      518 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/socket/cache/queue.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2371 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/socket/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/network/socket/model/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      757 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/socket/model/SOCKET_MODELS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/socket/model/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/network/socket/protocol/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/socket/protocol/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/socket/protocol/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/socket/server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/network/websocket/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/websocket/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/websocket/protocol.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/network/websocket/server.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/reflect.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/robot/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/robot/control/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/control/D_33890.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/control/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1296 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/control/device.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/robot/people/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1117 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/people/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5622 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/people/leg.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.214796 TDhelper-2.4.9/TDhelper/robot/people/scripts/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/people/scripts/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3111 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/people/scripts/runScript.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/people/scripts/script.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/people/upperLimb.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/people/vertebra.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.224796 TDhelper-2.4.9/TDhelper/robot/struct/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/struct/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      621 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/struct/ankle.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/struct/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      613 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/struct/hip.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      618 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/struct/knee.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      697 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/robot/struct/toe.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.224796 TDhelper-2.4.9/TDhelper/shellScripts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      335 2023-04-06 02:34:35.000000 TDhelper-2.4.9/TDhelper/shellScripts/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3190 2023-05-07 06:20:59.000000 TDhelper-2.4.9/TDhelper/shellScripts/saasHelper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.224796 TDhelper-2.4.9/TDhelper/simulate/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/simulate/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2713 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/simulate/json.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.224796 TDhelper-2.4.9/TDhelper/structs/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/structs/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4359 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/structs/dir.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.224796 TDhelper-2.4.9/TDhelper/web/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/web/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8255 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/web/permission.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-04-03 05:53:54.000000 TDhelper-2.4.9/TDhelper/web/permissionHelper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 13:34:09.184796 TDhelper-2.4.9/TDhelper.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-05-14 13:34:09.000000 TDhelper-2.4.9/TDhelper.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5532 2023-05-14 13:34:09.000000 TDhelper-2.4.9/TDhelper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-14 13:34:09.000000 TDhelper-2.4.9/TDhelper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-05-14 13:34:09.000000 TDhelper-2.4.9/TDhelper.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      754 2023-05-14 13:34:09.000000 TDhelper-2.4.9/TDhelper.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-14 13:34:09.000000 TDhelper-2.4.9/TDhelper.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-14 13:34:09.224796 TDhelper-2.4.9/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-05-14 13:33:54.000000 TDhelper-2.4.9/setup.py
```

### Comparing `TDhelper-2.4.8/LICENSE` & `TDhelper-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/PKG-INFO` & `TDhelper-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDhelper
-Version: 2.4.8
+Version: 2.4.9
 Summary: reconsitution web.permissionHelper cls.
 Home-page: https://gitee.com/TonyDon/pyLib
 Author: TangJing
 Author-email: yeihizhi@163.com
 License: Apache 2.0
 Keywords: pip,TDhelper,featureextraction
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TDhelper Version: 2.4.8 Summary: reconsitution
+Metadata-Version: 2.1 Name: TDhelper Version: 2.4.9 Summary: reconsitution
 web.permissionHelper cls. Home-page: https://gitee.com/TonyDon/pyLib Author:
 TangJing Author-email: yeihizhi@163.com License: Apache 2.0 Keywords:
 pip,TDhelper,featureextraction Description-Content-Type: text/markdown License-
 File: LICENSE # TDhelper LIb helper class lib. # ***Cache*** ## 1. pools ## 2.
 ring cache # ***db*** ## 1. sqllite ## 2. mongodb ## 3. mysql #
 ***Decorators*** ## 1. log # ***document*** ## 1. file ## 2. excel #
 ***Event*** ## 1. Event ## 2. classEvent ## 3. webEvent # ***generic*** #
```

### Comparing `TDhelper-2.4.8/README.md` & `TDhelper-2.4.9/README.md`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Decorators/log.py` & `TDhelper-2.4.9/TDhelper/Decorators/log.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Decorators/performance.py` & `TDhelper-2.4.9/TDhelper/Decorators/performance.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Event/Event.py` & `TDhelper-2.4.9/TDhelper/Event/Event.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Event/classEvent/event.py` & `TDhelper-2.4.9/TDhelper/Event/classEvent/event.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Event/classEvent/meta.py` & `TDhelper-2.4.9/TDhelper/Event/classEvent/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Event/webEvent/Events.py` & `TDhelper-2.4.9/TDhelper/Event/webEvent/Events.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/MagicCls/MagicMeta.py` & `TDhelper-2.4.9/TDhelper/MagicCls/MagicMeta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/MagicCls/model.py` & `TDhelper-2.4.9/TDhelper/MagicCls/model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/MagicCls/test.py` & `TDhelper-2.4.9/TDhelper/MagicCls/test.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Msg/AppPush.py` & `TDhelper-2.4.9/TDhelper/Msg/AppPush.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Msg/Config.py` & `TDhelper-2.4.9/TDhelper/Msg/Config.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Msg/Email.py` & `TDhelper-2.4.9/TDhelper/Msg/Email.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Msg/InterfaceMsg.py` & `TDhelper-2.4.9/TDhelper/Msg/InterfaceMsg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Msg/SMS.py` & `TDhelper-2.4.9/TDhelper/Msg/SMS.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Scheduler/base.py` & `TDhelper-2.4.9/TDhelper/Scheduler/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Scheduler/example_scheduler.py` & `TDhelper-2.4.9/TDhelper/Scheduler/example_scheduler.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Scheduler/interface.py` & `TDhelper-2.4.9/TDhelper/Scheduler/interface.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Scheduler/log_config.py` & `TDhelper-2.4.9/TDhelper/Scheduler/log_config.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Scheduler/service.py` & `TDhelper-2.4.9/TDhelper/Scheduler/service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Spider/contentExtraction.py` & `TDhelper-2.4.9/TDhelper/Spider/contentExtraction.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Spider/models/BadRequestModel.py` & `TDhelper-2.4.9/TDhelper/Spider/models/BadRequestModel.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Spider/models/Cache_L1.py` & `TDhelper-2.4.9/TDhelper/Spider/models/Cache_L1.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Spider/models/Cache_L2.py` & `TDhelper-2.4.9/TDhelper/Spider/models/Cache_L2.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Spider/models/Cache_L2_Model.py` & `TDhelper-2.4.9/TDhelper/Spider/models/Cache_L2_Model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Spider/models/fingerprint.py` & `TDhelper-2.4.9/TDhelper/Spider/models/fingerprint.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Spider/models/status.py` & `TDhelper-2.4.9/TDhelper/Spider/models/status.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Spider/regex.py` & `TDhelper-2.4.9/TDhelper/Spider/regex.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/Spider/spiderPools.py` & `TDhelper-2.4.9/TDhelper/Spider/spiderPools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 from enum import Enum
 from TDhelper.Event.Event import Event
 from TDhelper.Spider.regex import Analysis
 from TDhelper.Spider.models.spider_event import event as Analysis_Event
 from TDhelper.Spider.models.status import STATUS as SPIDER_STATUS
 from TDhelper.Spider.models.fingerprint import fingerprint
-from TDhelper.Cache.pools import pools
+from TDhelper.cache.pools import pools
 from TDhelper.Spider.models.Cache_L1 import L1, event as L1_EVENT, L2
 from TDhelper.Spider.models.BadRequestModel import BadRequest
 from threading import Thread
 
 import copy
```

### Comparing `TDhelper-2.4.8/TDhelper/apiCore.py` & `TDhelper-2.4.9/TDhelper/apiCore.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/bin/globalvar.py` & `TDhelper-2.4.9/TDhelper/bin/globalvar.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/cache/memcache.py` & `TDhelper-2.4.9/TDhelper/cache/memcache.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/cache/pools.py` & `TDhelper-2.4.9/TDhelper/cache/pools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/cache/ring.py` & `TDhelper-2.4.9/TDhelper/cache/ring.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/cache/webCache/interface.py` & `TDhelper-2.4.9/TDhelper/cache/webCache/interface.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/cache/webCache/mongo.py` & `TDhelper-2.4.9/TDhelper/cache/webCache/mongo.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/cache/webCache/webCacheFactory.py` & `TDhelper-2.4.9/TDhelper/cache/webCache/webCacheFactory.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/db/Db/base.py` & `TDhelper-2.4.9/TDhelper/db/Db/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/db/mongodb/base.py` & `TDhelper-2.4.9/TDhelper/db/mongodb/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/db/mongodb/dbhelper.py` & `TDhelper-2.4.9/TDhelper/db/mongodb/dbhelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/db/mongodb/objectId.py` & `TDhelper-2.4.9/TDhelper/db/mongodb/objectId.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/db/mysql/mysql_x.py` & `TDhelper-2.4.9/TDhelper/db/mysql/mysql_x.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/document/excel/meta/modelMeta.py` & `TDhelper-2.4.9/TDhelper/document/excel/meta/modelMeta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/document/excel/model.py` & `TDhelper-2.4.9/TDhelper/document/excel/model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/document/file.py` & `TDhelper-2.4.9/TDhelper/document/file.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/document/ini/meta.py` & `TDhelper-2.4.9/TDhelper/document/ini/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/generic/__init__.py` & `TDhelper-2.4.9/TDhelper/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/generic/classDocCfg.py` & `TDhelper-2.4.9/TDhelper/generic/classDocCfg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/generic/crypto/MD5.py` & `TDhelper-2.4.9/TDhelper/generic/crypto/MD5.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/generic/dictHelper.py` & `TDhelper-2.4.9/TDhelper/generic/dictHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/generic/dynamic/base/Meta.py` & `TDhelper-2.4.9/TDhelper/generic/dynamic/base/Meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/generic/dynamic/test.py` & `TDhelper-2.4.9/TDhelper/generic/dynamic/test.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/generic/findAttribute.py` & `TDhelper-2.4.9/TDhelper/generic/findAttribute.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/generic/recursion.py` & `TDhelper-2.4.9/TDhelper/generic/recursion.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/generic/requier.py` & `TDhelper-2.4.9/TDhelper/generic/requier.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/generic/standard_result.py` & `TDhelper-2.4.9/TDhelper/generic/standard_result.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/generic/threadPools.py` & `TDhelper-2.4.9/TDhelper/generic/threadPools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/generic/transformationType.py` & `TDhelper-2.4.9/TDhelper/generic/transformationType.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 # here put the import lib
 import datetime
 from pickle import TRUE
 
 # code start
 
 
-def transformation(value: any, transformationType):
+def transformation(value: any, transformationType, split_str=" "):
     """
     类型转换(目前仅只支持int,str,datetime,bool转换)
     - Params:
         - value: 需要转换的内容.
         - transformationType: 转换后的类型.
+        - split_str: 字符转数组分割字符，默认一个空格, 如字符串内不包含分割字符则会直接把字符串按每个字符分割；
     """
     try:
         if not isinstance(value, transformationType):
             if transformationType == int:
                 value = int(value)
             if transformationType == str:
                 if isinstance(value, datetime.datetime):
@@ -87,10 +88,16 @@
                         value = False
                     elif v == "true":
                         value = True
                     else:
                         value = True
                 else:
                     value = bool(value)
+            if transformationType == list:
+                if isinstance(value, str):
+                    if value.__contains__(split_str):
+                        value= value.split(split_str)
+                    else:
+                        value= list(value)
     except Exception as e:
         raise e
     return value
```

### Comparing `TDhelper-2.4.8/TDhelper/network/http/REST_HTTP.py` & `TDhelper-2.4.9/TDhelper/network/http/REST_HTTP.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/http/RPC.py` & `TDhelper-2.4.9/TDhelper/network/http/RPC.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/http/RPC1.py` & `TDhelper-2.4.9/TDhelper/network/http/RPC1.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/http/http_helper.py` & `TDhelper-2.4.9/TDhelper/network/http/http_helper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/http/http_postdataformat.py` & `TDhelper-2.4.9/TDhelper/network/http/http_postdataformat.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/http/m3u8.py` & `TDhelper-2.4.9/TDhelper/network/http/m3u8.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/http/m3u8_backup.py` & `TDhelper-2.4.9/TDhelper/network/http/m3u8_backup.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/rpc/Client/rpc.py` & `TDhelper-2.4.9/TDhelper/network/rpc/Client/rpc.py`

 * *Files 19% similar despite different names*

```diff
@@ -47,16 +47,18 @@
                 for k, v in self.__context__["msg"].items():
                     self.__dict__["__srv_struct__"][k] = type(
                         k, (RPC_SERVICE,), {}).create_by_cnf(v, self.__TOKEN_KEY__)
                     methods = [kv for kv in v['methods'].keys()]
                     self.__dict__[k] = type(k, (dynamic_creator,), {
                                             "__dynamic_methods__": methods, "__hook_method__": self.__call__})()
             else:
-                self.__LOGGER__.error("not found rpc method.")
-                raise Exception("not found rpc method.")
+                self.__LOGGER__.error("not found rpc method.%s"%self.__context__["msg"])
+                s="not found rpc method.%s"%self.__context__["msg"]
+                print(s)
+                raise Exception(s)
         else:
             raise Exception("not found rpc instance config.")
         super(client, self).__init__()
 
     @performance.performance_testing
     def __call__(self, service_name, fun_name, *args, **kwargs):
         remote_func_name = ("".join([service_name, '.', fun_name]))
@@ -88,7 +90,30 @@
         if state == 200:
             body = json.loads(body)
             if body["state"] == 200:
                 return body
             else:
                 return {}
         return {}
+    
+    def reload(self):
+        pass
+    
+    def monitor(self,speed=None):
+        '''
+            start monitor service health.
+            
+            Args:
+            
+                speed: <cls,int>, monitor speed. seconds.
+        '''
+        if self.__srv_struct__:
+            for o in self.__srv_struct__:
+                self.__srv_struct__[o].monitor(speed)
+                
+    def stop_monitor(self):
+        '''
+            stop monitor service health.
+        '''
+        if self.__srv_struct__:
+            for o in self.__srv_struct__:
+                self.__srv_struct__[o].stop_monitor()
```

### Comparing `TDhelper-2.4.8/TDhelper/network/rpc/Client/service.py` & `TDhelper-2.4.9/TDhelper/network/rpc/Client/service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/rpc/Core/Meta.py` & `TDhelper-2.4.9/TDhelper/network/rpc/Core/Meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/rpc/Core/struct.py` & `TDhelper-2.4.9/TDhelper/network/rpc/Core/struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,14 +239,20 @@
             "name": self.name,
             "description": self.description,
             "key": self.key.upper(),
             "accessSecret": self.secret,
             "protocol": self.protocol
         })
 
+    def monitor(self,speed=None):
+        self.host.__start_state_monitor__(speed)
+        
+    def stop_monitor(self):
+        self.host.__stop_state_monitor__()
+    
     def __hit_method__(self, key):
         if key in self.methods:
             return self.methods[key]
         else:
             raise Exception("can not found method(%s)." % key)
 
     def __remote_call__(self, func_name, *args, **kwargs):
```

### Comparing `TDhelper-2.4.8/TDhelper/network/rpc/Generic/Host.py` & `TDhelper-2.4.9/TDhelper/network/rpc/Generic/Host.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from copy import deepcopy
 import random
+import time
+import logging
 from TDhelper.network.http.REST_HTTP import GET
-
+from threading import Thread
 
 class HostManager:
     def __init__(self) -> None:
         self.__host_cnf_backup__ = {}
         self.__host_cnf__ = {}
         self.__host__ = []
         self.__host_len__ = 0
+        self.__monitor_speed__= 10
+        
         # self.__health_sniffer__ = ""
-
+        self.__monitor_state__= True
     def __backup_host__(self):
         self.__host_cnf_backup__ = deepcopy(self.__host_cnf__)
 
     def get_per_http_host(self):
         try:
             return self.__generateHost__(self.getHost())
         except Exception as e:
@@ -60,14 +64,15 @@
         Returns:
             None
         Raises:
             10000 - key already exists.
         """
         serverId = str(serverId)
         proto = self.__checken_proto__(proto)
+        sniffer= sniffer if sniffer else "/api/sniffer"
         if serverId not in self.__host_cnf__:
             self.__host_cnf__[serverId] = {
                 "proto": proto,
                 "host": host,
                 "port": port,
                 "status": status,
                 "sniffer": sniffer
@@ -136,45 +141,59 @@
                     health - checked it's success count.
                     unhealthy - checked it's fail count.
                 health - <class, list>, health serverId list.
                 unhealthy - <class, list>, unhealthy serverId list.
         Raises:
             None.
         """
-        result = {
-            "statistics": {
-                "total": self.__host_len__,
-                "health": 0,
-                "unhealthy": 0,
-            },
-            "health": [],
-            "unhealthy": []
-        }
-        for k in self.__host__:
-            m_uri = self.__generateHost__(self.__host_cnf__[k])
-            if m_uri:
-                m_uri += "/" + \
-                    self.__host_cnf__[k]["sniffer"].strip(
-                        '/').replace('\\', "/")
-                status, body = GET(m_uri, time_out=5)
-                if status == 200:
-                    self.__host_cnf__[k]['status'] = True
-                    result["health"].append(k)
+        while self.__monitor_state__:
+            result = {
+                "statistics": {
+                    "total": self.__host_len__,
+                    "health": 0,
+                    "unhealthy": 0,
+                },
+                "health": [],
+                "unhealthy": []
+            }
+            for k in self.__host__:
+                m_uri = self.__generateHost__(self.__host_cnf__[k])
+                if m_uri:
+                    m_uri += "/" + \
+                        self.__host_cnf__[k]["sniffer"].strip(
+                            '/').replace('\\', "/")
+                    status, body = GET(m_uri, time_out=5)
+                    if status == 200:
+                        self.__host_cnf__[k]['status'] = True
+                        logging.info("%s%s:%s%s  success."%(self.__host_cnf__[k]['proto'],self.__host_cnf__[k]['host'],self.__host_cnf__[k]['port'],self.__host_cnf__[k]['sniffer']))
+                        result["health"].append(k)
+                    else:
+                        self.__host_cnf__[k]["status"] = False
+                        logging.info("%s%s:%s%s fail."%(self.__host_cnf__[k]['proto'],self.__host_cnf__[k]['host'],self.__host_cnf__[k]['port'],self.__host_cnf__[k]['sniffer']))
+                        result["unhealthy"].append(k)
                 else:
                     self.__host_cnf__[k]["status"] = False
-                    result["unhealthy"].append(k)
-            else:
-                self.__host_cnf__[k]["status"] = False
-                result['unhealthy'].append(k)
-        for k in result["unhealthy"]:
-            self.delete(k)
-        result["statistics"]["health"] = len(result["health"])
-        result["statistics"]["unhealthy"] = len(result["unhealthy"])
-        return result
-
+                    logging.info("%s%s:%s%s fail."%(self.__host_cnf__[k]['proto'],self.__host_cnf__[k]['host'],self.__host_cnf__[k]['port'],self.__host_cnf__[k]['sniffer']))
+                    result['unhealthy'].append(k)
+            for k in result["unhealthy"]:
+                self.delete(k)
+            result["statistics"]["health"] = len(result["health"])
+            result["statistics"]["unhealthy"] = len(result["unhealthy"])
+            time.sleep(self.__monitor_speed__)
+
+    def __start_state_monitor__(self, speed= None):
+        self.__monitor_state__= True
+        self.__monitor_speed__= speed if speed else self.__monitor_speed__
+        monitor= Thread(target= self.health)
+        monitor.start()
+        
+    def __stop_state_monitor__(self):
+        self.__monitor_state__= False
+        self.__monitor_speed__= 10
+        
     def __generateHost__(self, uri_cnf: dict):
         proto = uri_cnf["proto"]
         host = uri_cnf["host"]
         port = str(uri_cnf["port"])
         if uri_cnf["status"]:
             if port != 80 or port != "80":
                 return proto+host+":"+port
```

### Comparing `TDhelper-2.4.8/TDhelper/network/rpc/Server/obsolete_Service.py` & `TDhelper-2.4.9/TDhelper/network/rpc/Server/obsolete_Service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/rpc/Server/server.py` & `TDhelper-2.4.9/TDhelper/network/rpc/Server/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 import logging
 import html
+from types import FunctionType
 from TDhelper.cache.memcache import cache
 
 class RPC_Server:
     __logger__ = logging
-
-    def __init__(self, logger_handle=None):
+    __logic__= None
+    def __init__(self, logic:FunctionType=None ,logger_handle=None):
         self.__logger__ = logger_handle if logger_handle else self.__logger__
-
+        self.__logic__= logic
+        if self.__logic__:
+            self.__logic__(self)
+        
+    def __reload__(self):
+        cache.__clear__()
+        if self.__logic__:
+            self.__logic__(self)
+        else:
+            self.__logger__.error("logic is none.")
+                
     def __insert__(self, k, v):
         try:
             cache.insert(k, v)
         except Exception as e:
             self.__logger__.error(e)
 
     def __append__(self, k, v):
```

### Comparing `TDhelper-2.4.8/TDhelper/network/rpc/Struct/Result.py` & `TDhelper-2.4.9/TDhelper/network/rpc/Struct/Result.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/socket/__init__.py` & `TDhelper-2.4.9/TDhelper/network/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/socket/cache/queue.py` & `TDhelper-2.4.9/TDhelper/network/socket/cache/queue.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/socket/client.py` & `TDhelper-2.4.9/TDhelper/network/socket/client.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/socket/model/SOCKET_MODELS.py` & `TDhelper-2.4.9/TDhelper/network/socket/model/SOCKET_MODELS.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/socket/protocol/base.py` & `TDhelper-2.4.9/TDhelper/network/socket/protocol/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/socket/server.py` & `TDhelper-2.4.9/TDhelper/network/socket/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/websocket/protocol.py` & `TDhelper-2.4.9/TDhelper/network/websocket/protocol.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/network/websocket/server.py` & `TDhelper-2.4.9/TDhelper/network/websocket/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/reflect.py` & `TDhelper-2.4.9/TDhelper/reflect.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/robot/control/D_33890.py` & `TDhelper-2.4.9/TDhelper/robot/control/D_33890.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/robot/control/device.py` & `TDhelper-2.4.9/TDhelper/robot/control/device.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/robot/people/__init__.py` & `TDhelper-2.4.9/TDhelper/robot/people/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/robot/people/leg.py` & `TDhelper-2.4.9/TDhelper/robot/people/leg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/robot/people/scripts/runScript.py` & `TDhelper-2.4.9/TDhelper/robot/people/scripts/runScript.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/robot/people/scripts/script.py` & `TDhelper-2.4.9/TDhelper/robot/people/scripts/script.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/robot/struct/ankle.py` & `TDhelper-2.4.9/TDhelper/robot/struct/ankle.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/robot/struct/base.py` & `TDhelper-2.4.9/TDhelper/robot/struct/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/robot/struct/hip.py` & `TDhelper-2.4.9/TDhelper/robot/struct/hip.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/robot/struct/knee.py` & `TDhelper-2.4.9/TDhelper/robot/struct/knee.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/robot/struct/toe.py` & `TDhelper-2.4.9/TDhelper/robot/struct/toe.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/shellScripts/saasHelper.py` & `TDhelper-2.4.9/TDhelper/shellScripts/saasHelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 if result == 0:
                     result = os.system(
                         "sudo sed -i 's/{project_name}/'"+args['name']+"'/g' "+args['path']+"/"+args['name']+"/settings.py")
                     result = os.system(
                         "sudo sed -i 's/{project_name}/'"+args['name']+"'/g' " + args['path']+"/make/uwsgi.example.ini")
                     result = os.system("sudo rm -rf "+args['path']+"/.git")
         else:
-            pass
+            print('git clone error.')
     except Exception as e:
         print(e)
 
 
 def buildArgs(args):
     result = {
         "name": "project_name",
```

### Comparing `TDhelper-2.4.8/TDhelper/simulate/json.py` & `TDhelper-2.4.9/TDhelper/simulate/json.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/structs/dir.py` & `TDhelper-2.4.9/TDhelper/structs/dir.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/web/permission.py` & `TDhelper-2.4.9/TDhelper/web/permission.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper/web/permissionHelper.py` & `TDhelper-2.4.9/TDhelper/web/permissionHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper.egg-info/PKG-INFO` & `TDhelper-2.4.9/TDhelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDhelper
-Version: 2.4.8
+Version: 2.4.9
 Summary: reconsitution web.permissionHelper cls.
 Home-page: https://gitee.com/TonyDon/pyLib
 Author: TangJing
 Author-email: yeihizhi@163.com
 License: Apache 2.0
 Keywords: pip,TDhelper,featureextraction
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TDhelper Version: 2.4.8 Summary: reconsitution
+Metadata-Version: 2.1 Name: TDhelper Version: 2.4.9 Summary: reconsitution
 web.permissionHelper cls. Home-page: https://gitee.com/TonyDon/pyLib Author:
 TangJing Author-email: yeihizhi@163.com License: Apache 2.0 Keywords:
 pip,TDhelper,featureextraction Description-Content-Type: text/markdown License-
 File: LICENSE # TDhelper LIb helper class lib. # ***Cache*** ## 1. pools ## 2.
 ring cache # ***db*** ## 1. sqllite ## 2. mongodb ## 3. mysql #
 ***Decorators*** ## 1. log # ***document*** ## 1. file ## 2. excel #
 ***Event*** ## 1. Event ## 2. classEvent ## 3. webEvent # ***generic*** #
```

### Comparing `TDhelper-2.4.8/TDhelper.egg-info/SOURCES.txt` & `TDhelper-2.4.9/TDhelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/TDhelper.egg-info/requires.txt` & `TDhelper-2.4.9/TDhelper.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `TDhelper-2.4.8/setup.py` & `TDhelper-2.4.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="TDhelper",
-    version="2.4.8",
+    version="2.4.9",
     keywords=("pip", "TDhelper", "featureextraction"),
     description="reconsitution web.permissionHelper cls.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache 2.0",
     url="https://gitee.com/TonyDon/pyLib",
     author="TangJing",
```

