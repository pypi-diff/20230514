# Comparing `tmp/chainlit-0.1.0.tar.gz` & `tmp/chainlit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlit-0.1.0.tar", last modified: Fri Mar 31 14:25:33 2023, max compression
+gzip compressed data, was "chainlit-0.1.1.tar", max compression
```

## Comparing `chainlit-0.1.0.tar` & `chainlit-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,34 @@
-drwxr-xr-x   0 danconstantini   (501) staff       (20)        0 2023-03-31 14:25:33.436593 chainlit-0.1.0/
--rw-r--r--   0 danconstantini   (501) staff       (20)      106 2023-03-31 14:25:33.436269 chainlit-0.1.0/PKG-INFO
-drwxr-xr-x   0 danconstantini   (501) staff       (20)        0 2023-03-31 14:25:33.435739 chainlit-0.1.0/chainlit.egg-info/
--rw-r--r--   0 danconstantini   (501) staff       (20)      106 2023-03-31 14:25:33.000000 chainlit-0.1.0/chainlit.egg-info/PKG-INFO
--rw-r--r--   0 danconstantini   (501) staff       (20)      136 2023-03-31 14:25:33.000000 chainlit-0.1.0/chainlit.egg-info/SOURCES.txt
--rw-r--r--   0 danconstantini   (501) staff       (20)        1 2023-03-31 14:25:33.000000 chainlit-0.1.0/chainlit.egg-info/dependency_links.txt
--rw-r--r--   0 danconstantini   (501) staff       (20)        1 2023-03-31 14:25:33.000000 chainlit-0.1.0/chainlit.egg-info/top_level.txt
--rw-r--r--   0 danconstantini   (501) staff       (20)       38 2023-03-31 14:25:33.436700 chainlit-0.1.0/setup.cfg
--rw-r--r--   0 danconstantini   (501) staff       (20)      287 2023-03-31 14:25:01.000000 chainlit-0.1.0/setup.py
+-rw-r--r--   0        0        0     2149 2023-05-14 17:29:40.435617 chainlit-0.1.1/README.md
+-rw-r--r--   0        0        0    13853 2023-05-14 17:28:53.271156 chainlit-0.1.1/chainlit/__init__.py
+-rw-r--r--   0        0        0       87 2023-05-14 17:28:53.271156 chainlit-0.1.1/chainlit/__main__.py
+-rw-r--r--   0        0        0     3471 2023-05-14 17:28:53.271156 chainlit-0.1.1/chainlit/cli/__init__.py
+-rw-r--r--   0        0        0     4093 2023-05-14 17:28:53.271156 chainlit-0.1.1/chainlit/cli/auth.py
+-rw-r--r--   0        0        0     2594 2023-05-14 17:28:53.271156 chainlit-0.1.1/chainlit/cli/deploy.py
+-rw-r--r--   0        0        0      716 2023-05-14 17:28:53.271156 chainlit-0.1.1/chainlit/cli/utils.py
+-rw-r--r--   0        0        0     5150 2023-05-14 17:28:53.271156 chainlit-0.1.1/chainlit/client.py
+-rw-r--r--   0        0        0     6385 2023-05-14 17:28:53.271156 chainlit-0.1.1/chainlit/config.py
+-rw-r--r--   0        0        0  2070264 2023-05-14 17:30:14.051940 chainlit-0.1.1/chainlit/frontend/dist/assets/index-10932891.js
+-rw-r--r--   0        0        0     4317 2023-05-14 17:30:14.051940 chainlit-0.1.1/chainlit/frontend/dist/assets/index-bdffdaa0.css
+-rw-r--r--   0        0        0     8889 2023-05-14 17:30:14.043940 chainlit-0.1.1/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
+-rw-r--r--   0        0        0     8891 2023-05-14 17:30:14.051940 chainlit-0.1.1/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
+-rw-r--r--   0        0        0     6455 2023-05-14 17:30:12.519927 chainlit-0.1.1/chainlit/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0      772 2023-05-14 17:30:14.051940 chainlit-0.1.1/chainlit/frontend/dist/index.html
+-rw-r--r--   0        0        0      344 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/hello.py
+-rw-r--r--   0        0        0        0 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/lc/__init__.py
+-rw-r--r--   0        0        0     8077 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/lc/chainlit_handler.py
+-rw-r--r--   0        0        0      863 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/lc/monkey.py
+-rw-r--r--   0        0        0     5388 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/lc/new_monkey.py
+-rw-r--r--   0        0        0     4129 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/lc/old_monkey.py
+-rw-r--r--   0        0        0     1117 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/lc/utils.py
+-rw-r--r--   0        0        0      398 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/logger.py
+-rw-r--r--   0        0        0     1618 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/markdown.py
+-rw-r--r--   0        0        0     8217 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/sdk.py
+-rw-r--r--   0        0        0     9948 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/server.py
+-rw-r--r--   0        0        0      813 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/session.py
+-rw-r--r--   0        0        0     2017 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/telemetry.py
+-rw-r--r--   0        0        0     1044 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/types.py
+-rw-r--r--   0        0        0     1145 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/user_session.py
+-rw-r--r--   0        0        0      196 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/version.py
+-rw-r--r--   0        0        0     1551 2023-05-14 17:28:53.275156 chainlit-0.1.1/chainlit/watch.py
+-rw-r--r--   0        0        0     1018 2023-05-14 17:28:53.275156 chainlit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3577 1970-01-01 00:00:00.000000 chainlit-0.1.1/PKG-INFO
```

