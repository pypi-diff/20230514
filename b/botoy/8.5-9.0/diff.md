# Comparing `tmp/botoy-8.5.tar.gz` & `tmp/botoy-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/botoy-8.5.tar", last modified: Sat Dec 31 04:14:22 2022, max compression
+gzip compressed data, was "dist/botoy-9.0.tar", last modified: Sun May 14 14:20:14 2023, max compression
```

## Comparing `botoy-8.5.tar` & `botoy-9.0.tar`

### file list

```diff
@@ -1,103 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 04:14:22.000000 botoy-8.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2022-12-31 04:14:22.000000 botoy-8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2022-12-31 04:14:12.000000 botoy-8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 04:14:22.000000 botoy-8.5/botoy/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2022-12-31 04:14:12.000000 botoy-8.5/botoy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-31 04:14:12.000000 botoy-8.5/botoy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2022-12-31 04:14:12.000000 botoy-8.5/botoy/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31623 2022-12-31 04:14:12.000000 botoy-8.5/botoy/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    32324 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 04:14:22.000000 botoy-8.5/botoy/async_decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_common_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_ensure_tempMsg.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_equal_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_from_botself.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_from_phone.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_from_these_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_from_these_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_ignore_botself.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_ignore_tempMsg.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_ignore_these_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_ignore_these_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_in_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_need_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_on_regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_re_findall.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_re_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_startswith.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2022-12-31 04:14:12.000000 botoy-8.5/botoy/async_decorators/_these_msgtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 04:14:22.000000 botoy-8.5/botoy/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2022-12-31 04:14:12.000000 botoy-8.5/botoy/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2022-12-31 04:14:12.000000 botoy-8.5/botoy/cli/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16567 2022-12-31 04:14:12.000000 botoy-8.5/botoy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2022-12-31 04:14:12.000000 botoy-8.5/botoy/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 04:14:22.000000 botoy-8.5/botoy/config/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-31 04:14:12.000000 botoy-8.5/botoy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2022-12-31 04:14:12.000000 botoy-8.5/botoy/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2022-12-31 04:14:12.000000 botoy-8.5/botoy/config/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2022-12-31 04:14:12.000000 botoy-8.5/botoy/config/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11620 2022-12-31 04:14:12.000000 botoy-8.5/botoy/contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 04:14:22.000000 botoy-8.5/botoy/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_common_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_ensure_tempMsg.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_equal_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_from_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_from_botself.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_from_phone.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_from_these_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_from_these_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_ignore_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_ignore_botself.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_ignore_tempMsg.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_ignore_these_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_ignore_these_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_in_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_need_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_on_regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_queued_up.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_re_findall.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_re_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_startswith.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_these_msgtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2022-12-31 04:14:12.000000 botoy-8.5/botoy/decorators/_with_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2022-12-31 04:14:12.000000 botoy-8.5/botoy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2022-12-31 04:14:12.000000 botoy-8.5/botoy/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-12-31 04:14:12.000000 botoy-8.5/botoy/macro.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2022-12-31 04:14:12.000000 botoy-8.5/botoy/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 04:14:22.000000 botoy-8.5/botoy/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 04:14:12.000000 botoy-8.5/botoy/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2022-12-31 04:14:12.000000 botoy-8.5/botoy/parser/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2022-12-31 04:14:12.000000 botoy-8.5/botoy/parser/friend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2022-12-31 04:14:12.000000 botoy-8.5/botoy/parser/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2022-12-31 04:14:12.000000 botoy-8.5/botoy/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2022-12-31 04:14:12.000000 botoy-8.5/botoy/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 04:14:22.000000 botoy-8.5/botoy/refine/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2022-12-31 04:14:12.000000 botoy-8.5/botoy/refine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2022-12-31 04:14:12.000000 botoy-8.5/botoy/refine/_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2022-12-31 04:14:12.000000 botoy-8.5/botoy/refine/_friend_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2022-12-31 04:14:12.000000 botoy-8.5/botoy/refine/_group_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2022-12-31 04:14:12.000000 botoy-8.5/botoy/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2022-12-31 04:14:12.000000 botoy-8.5/botoy/schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 04:14:22.000000 botoy-8.5/botoy/session/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2022-12-31 04:14:12.000000 botoy-8.5/botoy/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2022-12-31 04:14:12.000000 botoy-8.5/botoy/session/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2022-12-31 04:14:12.000000 botoy-8.5/botoy/session/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2022-12-31 04:14:12.000000 botoy-8.5/botoy/session/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2022-12-31 04:14:12.000000 botoy-8.5/botoy/session/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)    18664 2022-12-31 04:14:12.000000 botoy-8.5/botoy/sugar.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2022-12-31 04:14:12.000000 botoy-8.5/botoy/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2022-12-31 04:14:12.000000 botoy-8.5/botoy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2022-12-31 04:14:12.000000 botoy-8.5/botoy/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 04:14:22.000000 botoy-8.5/botoy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2022-12-31 04:14:22.000000 botoy-8.5/botoy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2022-12-31 04:14:22.000000 botoy-8.5/botoy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-31 04:14:22.000000 botoy-8.5/botoy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-31 04:14:22.000000 botoy-8.5/botoy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-31 04:14:22.000000 botoy-8.5/botoy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-31 04:14:22.000000 botoy-8.5/botoy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-31 04:14:12.000000 botoy-8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-31 04:14:22.000000 botoy-8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      969 2022-12-31 04:14:12.000000 botoy-8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:20:14.000000 botoy-9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-14 14:19:59.000000 botoy-9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-14 14:20:14.000000 botoy-9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-14 14:19:59.000000 botoy-9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:20:14.000000 botoy-9.0/botoy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-14 14:19:59.000000 botoy-9.0/botoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 14:19:59.000000 botoy-9.0/botoy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-14 14:19:59.000000 botoy-9.0/botoy/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:20:14.000000 botoy-9.0/botoy/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46439 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:20:14.000000 botoy-9.0/botoy/_internal/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/config/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/contrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/mahiro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:20:14.000000 botoy-9.0/botoy/_internal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/models/friend_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/models/group_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29298 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/sugar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-14 14:19:59.000000 botoy-9.0/botoy/_internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:20:14.000000 botoy-9.0/botoy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-14 14:20:13.000000 botoy-9.0/botoy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-14 14:20:13.000000 botoy-9.0/botoy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:20:13.000000 botoy-9.0/botoy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 14:20:13.000000 botoy-9.0/botoy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-14 14:20:13.000000 botoy-9.0/botoy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 14:20:13.000000 botoy-9.0/botoy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-14 14:19:59.000000 botoy-9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:20:14.000000 botoy-9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-14 14:19:59.000000 botoy-9.0/setup.py
```

### Comparing `botoy-8.5/PKG-INFO` & `botoy-9.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: botoy
-Version: 8.5
+Version: 9.0
 Summary: OPQBot/IOTQQ/IOTBot的Python开发助手
 Home-page: https://github.com/xiyaowong/botoy
 Author: wongxy
 Author-email: xiyao.wong@foxmail.com
 License: MIT
 Description: # botoy
         
-        <!-- [![QQ群](https://img.shields.io/badge/QQ%E7%BE%A4-757360354-important?style=flat-square&logo=tencentqq)](https://jq.qq.com/?_wv=1027&k=fBx8LvmA) -->
+        [![QQ Group](https://img.shields.io/badge/QQ%E7%BE%A4-856337734-important?style=flat-square&logo=tencentqq)](https://jq.qq.com/?_wv=1027&k=K8iQy7i7)
         
         [![pypi](https://img.shields.io/pypi/v/botoy?style=flat-square 'pypi')](https://pypi.org/project/botoy/)
-        [![python](https://img.shields.io/badge/python-3.7+-blue 'python')](https://pypi.org/project/botoy/)
+        [![python](https://img.shields.io/badge/python-3.8+-blue 'python')](https://pypi.org/project/botoy/)
         [![LICENSE](https://img.shields.io/github/license/opq-osc/botoy?style=flat-square)](https://github.com/opq-osc/botoy/blob/main/LICENSE)
         
         对机器人框架[OPQ](https://github.com/OPQBOT/OPQ/)接口的 Python 封装,
         因为功能模块耦合度低, 所以你可以完全使用该框架开发，也可以选取需要的内容到自己的项目中
         
         ---
         
@@ -23,41 +23,48 @@
         
         ```shell
         pip install botoy -i https://pypi.org/simple --upgrade
         ```
         
         ## 示例
         
-        如果你配置好了 OPQ，并且配置保持默认(bot 连接地址`http://127.0.0.1:8888`)，
-        下面一行代码即可监听消息，并在收到群消息或好友消息内容为 test 时回复 ok
+        如果你配置好了 OPQ，并且配置保持默认(bot 连接地址`http://127.0.0.1:8086`)，
+        下面示例可实现在收到群消息内容为 `test` 时回复 `ok`
         
-        ```python
-        __import__('botoy').Botoy().on_group_msg(lambda ctx: __import__('botoy').Action(ctx.CurrentQQ).sendGroupText(ctx.FromGroupId, 'ok') if ctx.Content == 'test' else None).on_friend_msg(lambda ctx: __import__('botoy').Action(ctx.CurrentQQ).sendFriendText(ctx.FromUin, 'ok') if ctx.Content == 'test' else None).run()
-        ```
-        
-        当然上面的写法明显不常规，要实现和上面相同的功能，一般这样写
+        新建文件 `bot.py`
         
         ```python
-        from botoy import Botoy, S
-        from botoy.decorators import equal_content
+        from botoy import bot, ctx, S
         
+        @bot
+        async def test():
+            if ctx.g and ctx.g.text == 'test':
+                await S.text('ok')
         
-        @equal_content("test")
-        def test(_):
-            S.text("ok")
+        bot.print_receivers()
+        bot.run()
+        ```
         
+        运行 `python bot.py`
         
-        Botoy().on_group_msg(test).on_friend_msg(test).run()
+        ```
+        +------+--------+-------+----------------+
+        | Name | Author | Usage |      Meta      |
+        +------+--------+-------+----------------+
+        | test |        |       | test.py line 4 |
+        +------+--------+-------+----------------+
+        ℹ️ 04-15 19:21:58 INFO 连接中[ws://localhost:8086/ws]...
+        ✔️ 04-15 19:21:58 SUCCESS 连接成功!
         ```
         
         # [文档](https://botoy.readthedocs.io/)
         
-        # [简单例子](https://github.com/opq-osc/botoy-plugins)
+        <!-- # [简单例子](https://github.com/opq-osc/botoy-plugins) -->
         
-        # [插件模板](https://github.com/opq-osc/botoy-plugin-template)
+        <!-- # [插件模板](https://github.com/opq-osc/botoy-plugin-template) -->
         
         # 感谢
         
         [yuban10703](https://github.com/yuban10703)
         [milkice](https://github.com/milkice233)
         
         # LICENSE
@@ -72,11 +79,11 @@
         
         - 修复模块导入错误
         
         ## V0.0.1
         
         初次发布
         
-Keywords: iotbot,iotqq,OPQ,OPQBot
+Keywords: iotbot,iotqq,OPQ,OPQBot,botoy
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `botoy-8.5/README.md` & `botoy-9.0/botoy.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,89 @@
-# botoy
-
-<!-- [![QQ群](https://img.shields.io/badge/QQ%E7%BE%A4-757360354-important?style=flat-square&logo=tencentqq)](https://jq.qq.com/?_wv=1027&k=fBx8LvmA) -->
-
-[![pypi](https://img.shields.io/pypi/v/botoy?style=flat-square 'pypi')](https://pypi.org/project/botoy/)
-[![python](https://img.shields.io/badge/python-3.7+-blue 'python')](https://pypi.org/project/botoy/)
-[![LICENSE](https://img.shields.io/github/license/opq-osc/botoy?style=flat-square)](https://github.com/opq-osc/botoy/blob/main/LICENSE)
-
-对机器人框架[OPQ](https://github.com/OPQBOT/OPQ/)接口的 Python 封装,
-因为功能模块耦合度低, 所以你可以完全使用该框架开发，也可以选取需要的内容到自己的项目中
-
----
-
-## 安装
-
-```shell
-pip install botoy -i https://pypi.org/simple --upgrade
-```
-
-## 示例
-
-如果你配置好了 OPQ，并且配置保持默认(bot 连接地址`http://127.0.0.1:8888`)，
-下面一行代码即可监听消息，并在收到群消息或好友消息内容为 test 时回复 ok
-
-```python
-__import__('botoy').Botoy().on_group_msg(lambda ctx: __import__('botoy').Action(ctx.CurrentQQ).sendGroupText(ctx.FromGroupId, 'ok') if ctx.Content == 'test' else None).on_friend_msg(lambda ctx: __import__('botoy').Action(ctx.CurrentQQ).sendFriendText(ctx.FromUin, 'ok') if ctx.Content == 'test' else None).run()
-```
-
-当然上面的写法明显不常规，要实现和上面相同的功能，一般这样写
-
-```python
-from botoy import Botoy, S
-from botoy.decorators import equal_content
-
-
-@equal_content("test")
-def test(_):
-    S.text("ok")
-
-
-Botoy().on_group_msg(test).on_friend_msg(test).run()
-```
-
-# [文档](https://botoy.readthedocs.io/)
-
-# [简单例子](https://github.com/opq-osc/botoy-plugins)
-
-# [插件模板](https://github.com/opq-osc/botoy-plugin-template)
-
-# 感谢
-
-[yuban10703](https://github.com/yuban10703)
-[milkice](https://github.com/milkice233)
-
-# LICENSE
-
-MIT
+Metadata-Version: 2.1
+Name: botoy
+Version: 9.0
+Summary: OPQBot/IOTQQ/IOTBot的Python开发助手
+Home-page: https://github.com/xiyaowong/botoy
+Author: wongxy
+Author-email: xiyao.wong@foxmail.com
+License: MIT
+Description: # botoy
+        
+        [![QQ Group](https://img.shields.io/badge/QQ%E7%BE%A4-856337734-important?style=flat-square&logo=tencentqq)](https://jq.qq.com/?_wv=1027&k=K8iQy7i7)
+        
+        [![pypi](https://img.shields.io/pypi/v/botoy?style=flat-square 'pypi')](https://pypi.org/project/botoy/)
+        [![python](https://img.shields.io/badge/python-3.8+-blue 'python')](https://pypi.org/project/botoy/)
+        [![LICENSE](https://img.shields.io/github/license/opq-osc/botoy?style=flat-square)](https://github.com/opq-osc/botoy/blob/main/LICENSE)
+        
+        对机器人框架[OPQ](https://github.com/OPQBOT/OPQ/)接口的 Python 封装,
+        因为功能模块耦合度低, 所以你可以完全使用该框架开发，也可以选取需要的内容到自己的项目中
+        
+        ---
+        
+        ## 安装
+        
+        ```shell
+        pip install botoy -i https://pypi.org/simple --upgrade
+        ```
+        
+        ## 示例
+        
+        如果你配置好了 OPQ，并且配置保持默认(bot 连接地址`http://127.0.0.1:8086`)，
+        下面示例可实现在收到群消息内容为 `test` 时回复 `ok`
+        
+        新建文件 `bot.py`
+        
+        ```python
+        from botoy import bot, ctx, S
+        
+        @bot
+        async def test():
+            if ctx.g and ctx.g.text == 'test':
+                await S.text('ok')
+        
+        bot.print_receivers()
+        bot.run()
+        ```
+        
+        运行 `python bot.py`
+        
+        ```
+        +------+--------+-------+----------------+
+        | Name | Author | Usage |      Meta      |
+        +------+--------+-------+----------------+
+        | test |        |       | test.py line 4 |
+        +------+--------+-------+----------------+
+        ℹ️ 04-15 19:21:58 INFO 连接中[ws://localhost:8086/ws]...
+        ✔️ 04-15 19:21:58 SUCCESS 连接成功!
+        ```
+        
+        # [文档](https://botoy.readthedocs.io/)
+        
+        <!-- # [简单例子](https://github.com/opq-osc/botoy-plugins) -->
+        
+        <!-- # [插件模板](https://github.com/opq-osc/botoy-plugin-template) -->
+        
+        # 感谢
+        
+        [yuban10703](https://github.com/yuban10703)
+        [milkice](https://github.com/milkice233)
+        
+        # LICENSE
+        
+        MIT
+        
+        # CHANGE LOG
+        
+        # See [releases](https://github.com/xiyaowong/botoy/releases)
+        
+        ## 0.0.2
+        
+        - 修复模块导入错误
+        
+        ## V0.0.1
+        
+        初次发布
+        
+Keywords: iotbot,iotqq,OPQ,OPQBot,botoy
+Platform: UNKNOWN
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
```

### Comparing `botoy-8.5/botoy/__version__.py` & `botoy-9.0/botoy/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pylint: disable=C0415,C0413
 # type: ignore
-__version__ = "8.5"
+__version__ = "9.0"
 
 
 def check_version(daemon=True):
     def _check_version():
         from distutils.version import LooseVersion as V
         from xml.etree import ElementTree
 
@@ -21,18 +21,16 @@
                 .find("item")
                 .find("title")
                 .text
             )
         except Exception:
             pass
         else:
-
             local_version = V(__version__)
             if local_version < latest_version:
-
                 try:
                     from rich.console import Console
                     from rich.markdown import Markdown
 
                     def mprint(msg):
                         Console().print(Markdown(msg))
```

### Comparing `botoy-8.5/botoy/config/config.py` & `botoy-9.0/botoy/_internal/config/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,21 @@
 import json
 import threading
 from typing import Any, Generic, List, Optional, TypeVar, Union
 
-from .constants import (
-    CONFIG_FILE_PATH,
-    DEFAULT_BLOCKED_USERS,
-    DEFAULT_FRIEND_BLACKLIST,
-    DEFAULT_GROUP_BLACKLIST,
-    DEFAULT_HOST,
-    DEFAULT_PORT,
-    DEFAULT_WEBHOOK,
-    DEFAULT_WEBHOOK_POST_URL,
-    DEFAULT_WEBHOOK_TIMEOUT,
-)
+from .constants import CONFIG_FILE_PATH, DEFAULT_URL
 from .util import dict2tree, lookup
 
 V = TypeVar("V")
 T = TypeVar("T")
 
 lock = threading.RLock()
 
 botoy_config = {
-    "host": DEFAULT_HOST,
-    "port": DEFAULT_PORT,
-    "group_blacklist": DEFAULT_GROUP_BLACKLIST,
-    "friend_blacklist": DEFAULT_FRIEND_BLACKLIST,
-    "blocked_users": DEFAULT_BLOCKED_USERS,
-    "webhook": DEFAULT_WEBHOOK,
-    "webhook_post_url": DEFAULT_WEBHOOK_POST_URL,
-    "webhook_timeout": DEFAULT_WEBHOOK_TIMEOUT,
+    "url": DEFAULT_URL,
 }
 botoy_config_tree = dict2tree(botoy_config)
 
 
 def read_botoy_config():
     global botoy_config, botoy_config_tree
 
@@ -112,22 +95,15 @@
         return "Configuration(tree=%s)" % self._config_tree.__repr__()
 
 
 class Configurations:
     _instance: Optional["Configurations"] = None
 
     # 框架专属配置
-    host: str
-    port: int
-    group_blacklist: List[int]
-    friend_blacklist: List[int]
-    blocked_users: List[int]
-    webhook: bool
-    webhook_post_url: str
-    webhook_timeout: int
+    url: str
 
     def __new__(cls):
         if not cls._instance:
             cls._instance = super().__new__(cls)
         return cls._instance
 
     def get_configuration(self, section: Optional[str] = None) -> Configuration:
@@ -135,22 +111,22 @@
         try:
             config_tree = lookup(botoy_config_tree, section)
         except KeyError:
             config_tree = {}
         return Configuration(config_tree, section)
 
     # 兼容旧版API
-    def get(self, key: str, default=None):
+    def get(self, key: str, default=None) -> Any:
         """配置文件作为字典，此方法等于字典的get方法"""
         return botoy_config.get(key, default)
 
-    def __getitem__(self, key: str):
+    def __getitem__(self, key: str) -> Any:
         return botoy_config.get(key)
 
-    def __getattr__(self, key: str):
+    def __getattr__(self, key: str) -> Any:
         return botoy_config.get(key)
 
     ############
 
     def __repr__(self):
         return "Configurations(\n  data=%s\n  tree=%s\n)" % (
             botoy_config,
```

### Comparing `botoy-8.5/botoy/config/util.py` & `botoy-9.0/botoy/_internal/config/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from typing import Optional
 
-from botoy.exceptions import InvalidConfigError
-
 
 def dict2tree(data: dict) -> dict:
     res = {}
     for key in data.keys():
         if "." not in key:
             res[key] = data[key]
         else:
@@ -18,15 +16,15 @@
                 else:
                     try:
                         pre[part] = pre[part]
                     except KeyError:
                         pre[part] = {}
                     pre = pre[part]
                     if not isinstance(pre, dict):
-                        raise InvalidConfigError(f'"{part}" 不能作为键名, 请查看文档修改你的配置')
+                        raise ValueError(f'"{part}" 不能作为键名, 请查看文档修改你的配置')
     return res
 
 
 def lookup(
     tree: dict,
     key: Optional[str] = None,
 ):
```

### Comparing `botoy-8.5/botoy/log.py` & `botoy-9.0/botoy/_internal/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,38 @@
 import os
 import sys
 
 from loguru import logger as _logger
 
 logger = _logger
 
-CONSOLE_LOG_FORMAT = "{level.icon} {time:MM-DD HH:mm:ss} <lvl>{level}\t{message}</lvl>"
+CONSOLE_LOG_FORMAT = "{level.icon} {time:MM-DD HH:mm:ss} <lvl>{level} {message}</lvl>"
 FILE_LOG_FORMAT = "{time:YYYY-MM-DD HH:mm} {level}\t{message}"
 FILE_LOG_PATH_NAMING = "./logs/{time}.log"
 
 
+class LoguruHandler(logging.Handler):
+    def emit(self, record):
+        # Get corresponding Loguru level if it exists
+        try:
+            level = logger.level(record.levelname).name
+        except ValueError:
+            level = record.levelno
+
+        # Find caller from where originated the logged message
+        frame, depth = logging.currentframe(), 2
+        while frame.f_code.co_filename == logging.__file__:  # type: ignore
+            frame = frame.f_back  # type: ignore
+            depth += 1
+
+        logger.opt(depth=depth, exception=record.exc_info).log(
+            level, record.getMessage()
+        )
+
+
 def logger_init(console_log=True, file_log=False):
     """
     :param console_log: 该参数控制控制台日志等级,为True输出INFO等级日志,为False输出EROOR等级的日志
     :param file_log: 该参数控制日志文件开与关,为True输出INFO等级日志的文件,为False关闭输出日志文件
 
     环境变量``BOTOY_LOG_LEVEL``拥有最高优先级
     """
@@ -42,34 +61,14 @@
             FILE_LOG_PATH_NAMING,
             format=FILE_LOG_FORMAT,
             rotation="1 day",
             encoding="utf-8",
             level=BOTOY_LOG_LEVEL or "INFO",
         )
 
+    ws_logger = logging.getLogger("websockets.client")
+    ws_logger.handlers.clear()
+    ws_logger.addHandler(LoguruHandler())
+    ws_logger.setLevel(level=logging.DEBUG)
 
-class LoguruHandler(logging.Handler):
-    def emit(self, record):
-        # Get corresponding Loguru level if it exists
-        try:
-            level = logger.level(record.levelname).name
-        except ValueError:
-            level = record.levelno
-
-        # Find caller from where originated the logged message
-        frame, depth = logging.currentframe(), 2
-        while frame.f_code.co_filename == logging.__file__:  # type: ignore
-            frame = frame.f_back  # type: ignore
-            depth += 1
-
-        logger.opt(depth=depth, exception=record.exc_info).log(
-            level, record.getMessage()
-        )
-
-
-sio_logger = logging.getLogger("socketio.client")
-sio_logger.handlers.clear()
-sio_logger.addHandler(LoguruHandler())
-if sio_logger.level == logging.NOTSET:
-    sio_logger.setLevel(logging.INFO)
 
 logger_init()
```

### Comparing `botoy-8.5/botoy/pool.py` & `botoy-9.0/botoy/_internal/pool.py`

 * *Files identical despite different names*

### Comparing `botoy-8.5/botoy/runner.py` & `botoy-9.0/botoy/_internal/runner.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,32 +3,29 @@
 import os
 import subprocess
 import sys
 import textwrap
 import time
 from functools import lru_cache
 from pathlib import Path
-from typing import Union
 
 import colorama
 
-from .async_client import AsyncBotoy
-from .client import Botoy
 
-
-@lru_cache(maxsize=2333)
+@lru_cache(maxsize=500)
 def _get_running_args():
     main = sys.modules["__main__"]
     spec = getattr(main, "__spec__", None)
     if spec:
         return [sys.executable, "-m", spec.name] + sys.argv[1:]
     return [sys.executable] + sys.argv
 
 
 def _restart_process():
+    print("")
     return subprocess.Popen(
         _get_running_args(),
         env={
             **os.environ,
             "BOTOY_CHILD": "true",
         },
     )
@@ -41,24 +38,23 @@
         filename = getattr(module, "__file__", None)
         if filename:
             if filename[-4:] in (".pyc", ".pyo"):
                 filename = filename[:-1]
             yield filename
 
 
-def run(bot: Union[Botoy, AsyncBotoy], auto_reload: bool = False):
+def run(bot, auto_reload: bool = False):
     """运行
 
     :param bot: bot实例
     :param auto_reload: 是否自动重载，当plugins目录内有文件或程序依赖的模块文件变动
     时将自动重启，部署时请勿开启该功能
     注意：只有修改操作才会进行重载，添加和删除文件不会
     """
     if auto_reload and os.getenv("BOTOY_CHILD") != "true":
-
         print(
             textwrap.dedent(
                 f"""
               {colorama.Fore.RED}
               ***********************************
               *                                 *
               *  已开启自动重载，部署时请关闭!  *
@@ -103,8 +99,12 @@
             pass
         finally:
             process.terminate()
             process.wait()
 
         return
 
-    return asyncio.run(bot.run()) if isinstance(bot, AsyncBotoy) else bot.run()
+    async def main():
+        await bot.connect()
+        await bot.wait()
+
+    return asyncio.get_event_loop().run_until_complete(main())
```

### Comparing `botoy-8.5/botoy/schedule.py` & `botoy-9.0/botoy/_internal/schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,11 +33,11 @@
                 **(jconfig.apscheduler_config or {}),
             }
         )
         async_scheduler.start()
         logger.info("异步定时任务已启动")
 
 
-if jconfig.apscheduler_autostart is None or jconfig.apscheduler_autostart:
+if jconfig.apscheduler_autostart:
     start_scheduler()
 
 __all__ = ["scheduler", "async_scheduler", "start_scheduler"]
```

### Comparing `botoy-8.5/botoy/utils.py` & `botoy-9.0/botoy/_internal/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 
         def __setitem__(self, index, value):
             contextvar.get()[index] = value
 
         def __delitem__(self, index):
             del contextvar.get()[index]
 
+        def __str__(self):
+            return str(contextvar.get())
+
     return ContextVarBind()
 
 
 def sync_run(func):
     """同步执行异步函数，获取结果(该函数始终新建一个事件循环)
     例如::
```

### Comparing `botoy-8.5/setup.py` & `botoy-9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     long_description=read_files(["README.md", "CHANGELOG.md"]),
     long_description_content_type="text/markdown",
     version=meta["__version__"],
     author="wongxy",
     author_email="xiyao.wong@foxmail.com",
     url="https://github.com/xiyaowong/botoy",
     license="MIT",
-    keywords=["iotbot", "iotqq", "OPQ", "OPQBot"],
+    keywords=["iotbot", "iotqq", "OPQ", "OPQBot", "botoy"],
     packages=find_packages(),
     install_requires=read_files(["requirements.txt"]),
     entry_points="""
         [console_scripts]
-        botoy=botoy.cli:cli
+        botoy=botoy._internal.cli:cli
     """,
     python_requires=">=3.7",
 )
```

