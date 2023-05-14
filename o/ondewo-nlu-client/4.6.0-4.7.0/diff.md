# Comparing `tmp/ondewo-nlu-client-4.6.0.tar.gz` & `tmp/ondewo-nlu-client-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-nlu-client-4.6.0.tar", last modified: Fri Mar 31 07:18:33 2023, max compression
+gzip compressed data, was "ondewo-nlu-client-4.7.0.tar", last modified: Sun May 14 10:07:13 2023, max compression
```

## Comparing `ondewo-nlu-client-4.6.0.tar` & `ondewo-nlu-client-4.7.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 07:18:33.131834 ondewo-nlu-client-4.6.0/
--rw-rw-r--   0 root         (0) root         (0)    10257 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      126 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7652 2023-03-31 07:18:33.131834 ondewo-nlu-client-4.6.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     7059 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 07:18:33.125834 ondewo-nlu-client-4.6.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 07:18:33.129834 ondewo-nlu-client-4.6.0/ondewo/nlu/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    72645 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/agent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)   111576 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/agent_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)    78517 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/agent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    28369 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/aiservices_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    45837 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/aiservices_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)    15091 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/aiservices_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     2892 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/client.py
--rw-rw-r--   0 root         (0) root         (0)     1654 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/client_config.py
--rw-rw-r--   0 root         (0) root         (0)     3618 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/client_pool.py
--rw-rw-r--   0 root         (0) root         (0)     1582 2023-03-31 07:18:11.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/common_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1515 2023-03-31 07:18:11.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/common_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)      158 2023-03-31 07:18:17.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/common_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    10226 2023-03-31 07:18:11.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/context_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    10666 2023-03-31 07:18:11.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/context_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)    13772 2023-03-31 07:18:11.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/context_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 07:18:33.129834 ondewo-nlu-client-4.6.0/ondewo/nlu/convenience/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/convenience/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8090 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/convenience/shared_request_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 07:18:33.129834 ondewo-nlu-client-4.6.0/ondewo/nlu/core/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1720 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/core/services_container.py
--rw-rw-r--   0 root         (0) root         (0)     1231 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/core/services_interface.py
--rw-rw-r--   0 root         (0) root         (0)    29558 2023-03-31 07:18:11.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/entity_type_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    45588 2023-03-31 07:18:11.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/entity_type_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)    32974 2023-03-31 07:18:11.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/entity_type_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    70722 2023-03-31 07:18:12.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/intent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)   125579 2023-03-31 07:18:12.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/intent_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)    53420 2023-03-31 07:18:12.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/intent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3341 2023-03-31 07:18:11.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/operation_metadata_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     9999 2023-03-31 07:18:11.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/operation_metadata_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)      158 2023-03-31 07:18:17.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/operation_metadata_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7815 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/operations_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    11137 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/operations_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)    10661 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/operations_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     9440 2023-03-31 07:18:12.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/project_role_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    12293 2023-03-31 07:18:12.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/project_role_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)     9487 2023-03-31 07:18:12.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/project_role_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7391 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/project_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     3786 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/project_statistics_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)    14908 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/project_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 07:18:33.129834 ondewo-nlu-client-4.6.0/ondewo/nlu/scripts/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/scripts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6115 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/scripts/client_example_script.py
--rw-rw-r--   0 root         (0) root         (0)     2980 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/server_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      805 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/server_statistics_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)     6064 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/server_statistics_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 07:18:33.130834 ondewo-nlu-client-4.6.0/ondewo/nlu/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11680 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/services/agents.py
--rw-rw-r--   0 root         (0) root         (0)     3561 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/services/aiservices.py
--rw-rw-r--   0 root         (0) root         (0)     2412 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/services/contexts.py
--rw-rw-r--   0 root         (0) root         (0)     4165 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/services/entity_types.py
--rw-rw-r--   0 root         (0) root         (0)     8894 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/services/intents.py
--rw-rw-r--   0 root         (0) root         (0)     2038 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/services/operations.py
--rw-rw-r--   0 root         (0) root         (0)     2301 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/services/project_roles.py
--rw-rw-r--   0 root         (0) root         (0)     2934 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/services/project_statistics.py
--rw-rw-r--   0 root         (0) root         (0)     1771 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/services/server_statistics.py
--rw-rw-r--   0 root         (0) root         (0)     4639 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/services/sessions.py
--rw-rw-r--   0 root         (0) root         (0)     4254 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/services/users.py
--rw-rw-r--   0 root         (0) root         (0)     3389 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/services/utilities.py
--rw-rw-r--   0 root         (0) root         (0)    65016 2023-03-31 07:18:12.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/session_pb2.py
--rw-rw-r--   0 root         (0) root         (0)   126851 2023-03-31 07:18:12.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/session_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)    51990 2023-03-31 07:18:12.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/session_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    19393 2023-03-31 07:18:09.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/user_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    21163 2023-03-31 07:18:09.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/user_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)    24694 2023-03-31 07:18:09.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/user_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    19985 2023-03-31 07:18:11.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/utility_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    38012 2023-03-31 07:18:11.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/utility_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)    15248 2023-03-31 07:18:11.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/utility_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 07:18:33.130834 ondewo-nlu-client-4.6.0/ondewo/nlu/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1302 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/utils/login.py
--rw-rw-r--   0 root         (0) root         (0)     6298 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/webhook_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     8524 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/webhook_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)     6055 2023-03-31 07:18:10.000000 ondewo-nlu-client-4.6.0/ondewo/nlu/webhook_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 07:18:33.130834 ondewo-nlu-client-4.6.0/ondewo/qa/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/qa/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1908 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/qa/client.py
--rw-rw-r--   0 root         (0) root         (0)      912 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/qa/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 07:18:33.131834 ondewo-nlu-client-4.6.0/ondewo/qa/core/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/qa/core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      791 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/qa/core/services_container.py
--rw-rw-r--   0 root         (0) root         (0)      733 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/qa/core/services_interface.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/qa/py.typed
--rw-rw-r--   0 root         (0) root         (0)    11286 2023-03-31 07:18:12.000000 ondewo-nlu-client-4.6.0/ondewo/qa/qa_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    11087 2023-03-31 07:18:12.000000 ondewo-nlu-client-4.6.0/ondewo/qa/qa_pb2.pyi
--rw-rw-r--   0 root         (0) root         (0)    12229 2023-03-31 07:18:12.000000 ondewo-nlu-client-4.6.0/ondewo/qa/qa_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 07:18:33.131834 ondewo-nlu-client-4.6.0/ondewo/qa/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/qa/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1533 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/ondewo/qa/services/qa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 07:18:33.131834 ondewo-nlu-client-4.6.0/ondewo_nlu_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7652 2023-03-31 07:18:33.000000 ondewo-nlu-client-4.6.0/ondewo_nlu_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2855 2023-03-31 07:18:33.000000 ondewo-nlu-client-4.6.0/ondewo_nlu_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 07:18:33.000000 ondewo-nlu-client-4.6.0/ondewo_nlu_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      219 2023-03-31 07:18:33.000000 ondewo-nlu-client-4.6.0/ondewo_nlu_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-31 07:18:33.000000 ondewo-nlu-client-4.6.0/ondewo_nlu_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      220 2023-03-31 07:17:59.000000 ondewo-nlu-client-4.6.0/requirements.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2023-03-31 07:18:33.131834 ondewo-nlu-client-4.6.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1151 2023-03-31 07:18:18.000000 ondewo-nlu-client-4.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 10:07:13.896959 ondewo-nlu-client-4.7.0/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      126 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-05-14 10:07:13.896959 ondewo-nlu-client-4.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     7059 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 10:07:13.887959 ondewo-nlu-client-4.7.0/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 10:07:13.893959 ondewo-nlu-client-4.7.0/ondewo/nlu/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    72645 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/agent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)   111576 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/agent_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    78517 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/agent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    28369 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/aiservices_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    45837 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/aiservices_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    15091 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/aiservices_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     2892 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/client.py
+-rw-rw-r--   0 root         (0) root         (0)     1654 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/client_config.py
+-rw-rw-r--   0 root         (0) root         (0)     3618 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/client_pool.py
+-rw-rw-r--   0 root         (0) root         (0)     1582 2023-05-14 10:06:51.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/common_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1515 2023-05-14 10:06:51.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/common_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-05-14 10:06:58.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/common_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    10226 2023-05-14 10:06:51.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/context_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    10666 2023-05-14 10:06:51.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/context_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    13772 2023-05-14 10:06:51.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/context_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 10:07:13.893959 ondewo-nlu-client-4.7.0/ondewo/nlu/convenience/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/convenience/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8090 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/convenience/shared_request_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 10:07:13.893959 ondewo-nlu-client-4.7.0/ondewo/nlu/core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1720 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/core/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)     1231 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/core/services_interface.py
+-rw-rw-r--   0 root         (0) root         (0)    29558 2023-05-14 10:06:51.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/entity_type_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    45588 2023-05-14 10:06:51.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/entity_type_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    32974 2023-05-14 10:06:51.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/entity_type_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    70722 2023-05-14 10:06:52.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/intent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)   125579 2023-05-14 10:06:52.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/intent_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    53420 2023-05-14 10:06:52.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/intent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3341 2023-05-14 10:06:51.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/operation_metadata_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     9999 2023-05-14 10:06:51.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/operation_metadata_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-05-14 10:06:58.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/operation_metadata_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7815 2023-05-14 10:06:51.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/operations_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    11137 2023-05-14 10:06:51.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/operations_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    10661 2023-05-14 10:06:51.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/operations_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     9440 2023-05-14 10:06:52.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/project_role_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    12293 2023-05-14 10:06:52.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/project_role_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)     9487 2023-05-14 10:06:52.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/project_role_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7391 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/project_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     3786 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/project_statistics_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    14908 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/project_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 10:07:13.893959 ondewo-nlu-client-4.7.0/ondewo/nlu/scripts/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/scripts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6115 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/scripts/client_example_script.py
+-rw-rw-r--   0 root         (0) root         (0)     2980 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/server_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      805 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/server_statistics_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)     6064 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/server_statistics_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 10:07:13.894959 ondewo-nlu-client-4.7.0/ondewo/nlu/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11680 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/services/agents.py
+-rw-rw-r--   0 root         (0) root         (0)     3561 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/services/aiservices.py
+-rw-rw-r--   0 root         (0) root         (0)     2412 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/services/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)     4165 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/services/entity_types.py
+-rw-rw-r--   0 root         (0) root         (0)     8894 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/services/intents.py
+-rw-rw-r--   0 root         (0) root         (0)     2038 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/services/operations.py
+-rw-rw-r--   0 root         (0) root         (0)     2301 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/services/project_roles.py
+-rw-rw-r--   0 root         (0) root         (0)     2934 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/services/project_statistics.py
+-rw-rw-r--   0 root         (0) root         (0)     1771 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/services/server_statistics.py
+-rw-rw-r--   0 root         (0) root         (0)     4639 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/services/sessions.py
+-rw-rw-r--   0 root         (0) root         (0)     4254 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/services/users.py
+-rw-rw-r--   0 root         (0) root         (0)     3389 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/services/utilities.py
+-rw-rw-r--   0 root         (0) root         (0)    65281 2023-05-14 10:06:52.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/session_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)   127556 2023-05-14 10:06:52.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/session_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    51990 2023-05-14 10:06:52.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/session_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    19393 2023-05-14 10:06:49.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/user_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    21163 2023-05-14 10:06:49.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/user_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    24694 2023-05-14 10:06:49.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/user_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    19985 2023-05-14 10:06:52.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/utility_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    38012 2023-05-14 10:06:52.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/utility_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    15248 2023-05-14 10:06:52.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/utility_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 10:07:13.895959 ondewo-nlu-client-4.7.0/ondewo/nlu/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1302 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/utils/login.py
+-rw-rw-r--   0 root         (0) root         (0)     6298 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/webhook_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     8524 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/webhook_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)     6055 2023-05-14 10:06:50.000000 ondewo-nlu-client-4.7.0/ondewo/nlu/webhook_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 10:07:13.895959 ondewo-nlu-client-4.7.0/ondewo/qa/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/qa/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1908 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/qa/client.py
+-rw-rw-r--   0 root         (0) root         (0)      912 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/qa/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 10:07:13.895959 ondewo-nlu-client-4.7.0/ondewo/qa/core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/qa/core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      791 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/qa/core/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)      733 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/qa/core/services_interface.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/qa/py.typed
+-rw-rw-r--   0 root         (0) root         (0)    11286 2023-05-14 10:06:53.000000 ondewo-nlu-client-4.7.0/ondewo/qa/qa_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    11087 2023-05-14 10:06:53.000000 ondewo-nlu-client-4.7.0/ondewo/qa/qa_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    12229 2023-05-14 10:06:53.000000 ondewo-nlu-client-4.7.0/ondewo/qa/qa_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 10:07:13.895959 ondewo-nlu-client-4.7.0/ondewo/qa/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/qa/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1533 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/ondewo/qa/services/qa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 10:07:13.896959 ondewo-nlu-client-4.7.0/ondewo_nlu_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-05-14 10:07:13.000000 ondewo-nlu-client-4.7.0/ondewo_nlu_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2855 2023-05-14 10:07:13.000000 ondewo-nlu-client-4.7.0/ondewo_nlu_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 10:07:13.000000 ondewo-nlu-client-4.7.0/ondewo_nlu_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      219 2023-05-14 10:07:13.000000 ondewo-nlu-client-4.7.0/ondewo_nlu_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-14 10:07:13.000000 ondewo-nlu-client-4.7.0/ondewo_nlu_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      220 2023-05-14 10:06:04.000000 ondewo-nlu-client-4.7.0/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-05-14 10:07:13.896959 ondewo-nlu-client-4.7.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1151 2023-05-14 10:07:00.000000 ondewo-nlu-client-4.7.0/setup.py
```

### Comparing `ondewo-nlu-client-4.6.0/LICENSE` & `ondewo-nlu-client-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/PKG-INFO` & `ondewo-nlu-client-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-nlu-client
-Version: 4.6.0
+Version: 4.7.0
 Summary: This library facilitates the interaction between a user and his/her CAI server.
 Home-page: https://github.com/ondewo/ondewo-nlu-client-python
 Author: Ondewo GmbH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-nlu-client Version: 4.6.0 Summary: This
+Metadata-Version: 2.1 Name: ondewo-nlu-client Version: 4.7.0 Summary: This
 library facilitates the interaction between a user and his/her CAI server.
 Home-page: https://github.com/ondewo/ondewo-nlu-client-python Author: Ondewo
 GmbH Author-email: office@ondewo.com License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8 Classifier: Operating System
 :: OS Independent Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-nlu-client-4.6.0/README.md` & `ondewo-nlu-client-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/agent_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/agent_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/agent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/agent_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/aiservices_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/aiservices_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/aiservices_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/aiservices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/aiservices_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/aiservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/client.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/client_config.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/client_config.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/client_pool.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/client_pool.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/common_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/common_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/context_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/context_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/context_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/context_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/context_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/context_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/convenience/shared_request_data.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/convenience/shared_request_data.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/core/services_container.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/core/services_container.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/core/services_interface.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/core/services_interface.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/entity_type_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/entity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/entity_type_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/entity_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/entity_type_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/entity_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/intent_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/intent_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/intent_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/intent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/intent_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/intent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/operation_metadata_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/operation_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/operation_metadata_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/operation_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/operations_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/operations_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/operations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/operations_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/project_role_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/project_role_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/project_role_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/project_role_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/project_role_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/project_role_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/project_statistics_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/project_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/project_statistics_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/project_statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/project_statistics_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/project_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/scripts/client_example_script.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/scripts/client_example_script.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/server_statistics_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/server_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/server_statistics_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/server_statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/server_statistics_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/server_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/services/agents.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/services/agents.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/services/aiservices.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/services/aiservices.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/services/contexts.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/services/contexts.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/services/entity_types.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/services/entity_types.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/services/intents.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/services/intents.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/services/operations.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/services/operations.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/services/project_roles.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/services/project_roles.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/services/project_statistics.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/services/project_statistics.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/services/server_statistics.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/services/server_statistics.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/services/sessions.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/services/sessions.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/services/users.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/services/users.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/services/utilities.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/services/utilities.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/session_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/session_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.rpc import status_pb2 as google_dot_rpc_dot_status__pb2
 from google.type import latlng_pb2 as google_dot_type_dot_latlng__pb2
 from ondewo.nlu import context_pb2 as ondewo_dot_nlu_dot_context__pb2
 from ondewo.nlu import intent_pb2 as ondewo_dot_nlu_dot_intent__pb2
 from ondewo.nlu import entity_type_pb2 as ondewo_dot_nlu_dot_entity__type__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18ondewo/nlu/session.proto\x12\nondewo.nlu\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x17google/rpc/status.proto\x1a\x18google/type/latlng.proto\x1a\x18ondewo/nlu/context.proto\x1a\x17ondewo/nlu/intent.proto\x1a\x1condewo/nlu/entity_type.proto\"\x9b\x01\n\x13\x44\x65tectIntentRequest\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x31\n\x0cquery_params\x18\x02 \x01(\x0b\x32\x1b.ondewo.nlu.QueryParameters\x12+\n\x0bquery_input\x18\x03 \x01(\x0b\x32\x16.ondewo.nlu.QueryInput\x12\x13\n\x0binput_audio\x18\x05 \x01(\x0c\"\x86\x01\n\x14\x44\x65tectIntentResponse\x12\x13\n\x0bresponse_id\x18\x01 \x01(\t\x12-\n\x0cquery_result\x18\x02 \x01(\x0b\x32\x17.ondewo.nlu.QueryResult\x12*\n\x0ewebhook_status\x18\x03 \x01(\x0b\x32\x12.google.rpc.Status\"\xef\x02\n\x0fQueryParameters\x12\x11\n\ttime_zone\x18\x01 \x01(\t\x12)\n\x0cgeo_location\x18\x02 \x01(\x0b\x32\x13.google.type.LatLng\x12%\n\x08\x63ontexts\x18\x03 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x16\n\x0ereset_contexts\x18\x04 \x01(\x08\x12(\n\x07payload\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06labels\x18\x07 \x03(\t\x12\x36\n\tplatforms\x18\x08 \x03(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\x12\x12\n\naccount_id\x18\t \x01(\t\x12\x13\n\x0bproperty_id\x18\n \x01(\t\x12\x15\n\rdatastream_id\x18\x0b \x01(\t\x12\x11\n\torigin_id\x18\x0c \x01(\t\x12\x1a\n\x12identified_user_id\x18\r \x01(\t\"\x9b\x01\n\nQueryInput\x12\x34\n\x0c\x61udio_config\x18\x01 \x01(\x0b\x32\x1c.ondewo.nlu.InputAudioConfigH\x00\x12%\n\x04text\x18\x02 \x01(\x0b\x32\x15.ondewo.nlu.TextInputH\x00\x12\'\n\x05\x65vent\x18\x03 \x01(\x0b\x32\x16.ondewo.nlu.EventInputH\x00\x42\x07\n\x05input\"\xa5\x04\n\x0bQueryResult\x12\x12\n\nquery_text\x18\x01 \x01(\t\x12%\n\x1dspeech_recognition_confidence\x18\x02 \x01(\x02\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12+\n\nparameters\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12#\n\x1b\x61ll_required_params_present\x18\x05 \x01(\x08\x12\x18\n\x10\x66ulfillment_text\x18\x06 \x01(\t\x12\x38\n\x14\x66ulfillment_messages\x18\x07 \x03(\x0b\x32\x1a.ondewo.nlu.Intent.Message\x12\x16\n\x0ewebhook_source\x18\x08 \x01(\t\x12\x30\n\x0fwebhook_payload\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\x0foutput_contexts\x18\n \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\"\n\x06intent\x18\x0b \x01(\x0b\x32\x12.ondewo.nlu.Intent\x12#\n\x1bintent_detection_confidence\x18\x0c \x01(\x02\x12\x1b\n\x13query_text_original\x18\r \x01(\t\x12\x30\n\x0f\x64iagnostic_info\x18\x0e \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x15\n\rlanguage_code\x18\x0f \x01(\t\"\xbe\x01\n\x1cStreamingDetectIntentRequest\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x31\n\x0cquery_params\x18\x02 \x01(\x0b\x32\x1b.ondewo.nlu.QueryParameters\x12+\n\x0bquery_input\x18\x03 \x01(\x0b\x32\x16.ondewo.nlu.QueryInput\x12\x18\n\x10single_utterance\x18\x04 \x01(\x08\x12\x13\n\x0binput_audio\x18\x06 \x01(\x0c\"\xd3\x01\n\x1dStreamingDetectIntentResponse\x12\x13\n\x0bresponse_id\x18\x01 \x01(\t\x12\x42\n\x12recognition_result\x18\x02 \x01(\x0b\x32&.ondewo.nlu.StreamingRecognitionResult\x12-\n\x0cquery_result\x18\x03 \x01(\x0b\x32\x17.ondewo.nlu.QueryResult\x12*\n\x0ewebhook_status\x18\x04 \x01(\x0b\x32\x12.google.rpc.Status\"\xfa\x01\n\x1aStreamingRecognitionResult\x12H\n\x0cmessage_type\x18\x01 \x01(\x0e\x32\x32.ondewo.nlu.StreamingRecognitionResult.MessageType\x12\x12\n\ntranscript\x18\x02 \x01(\t\x12\x10\n\x08is_final\x18\x03 \x01(\x08\x12\x12\n\nconfidence\x18\x04 \x01(\x02\"X\n\x0bMessageType\x12\x1c\n\x18MESSAGE_TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTRANSCRIPT\x10\x01\x12\x1b\n\x17\x45ND_OF_SINGLE_UTTERANCE\x10\x02\"\x8d\x01\n\x10InputAudioConfig\x12\x31\n\x0e\x61udio_encoding\x18\x01 \x01(\x0e\x32\x19.ondewo.nlu.AudioEncoding\x12\x19\n\x11sample_rate_hertz\x18\x02 \x01(\x05\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12\x14\n\x0cphrase_hints\x18\x04 \x03(\t\"0\n\tTextInput\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\"^\n\nEventInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\nparameters\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\"\xb4\x01\n\x07Session\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\rsession_steps\x18\x02 \x03(\x0b\x32\x17.ondewo.nlu.SessionStep\x12-\n\x0csession_info\x18\x03 \x01(\x0b\x32\x17.ondewo.nlu.SessionInfo\"<\n\x04View\x12\x14\n\x10VIEW_UNSPECIFIED\x10\x00\x12\r\n\tVIEW_FULL\x10\x01\x12\x0f\n\x0bVIEW_SPARSE\x10\x02\"\xc4\x01\n\x0bSessionStep\x12\x0c\n\x04name\x18\x01 \x01(\t\x12>\n\x15\x64\x65tect_intent_request\x18\x02 \x01(\x0b\x32\x1f.ondewo.nlu.DetectIntentRequest\x12@\n\x16\x64\x65tect_intent_response\x18\x03 \x01(\x0b\x32 .ondewo.nlu.DetectIntentResponse\x12%\n\x08\x63ontexts\x18\x04 \x03(\x0b\x32\x13.ondewo.nlu.Context\"\x8c\x01\n\x17TrackSessionStepRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12-\n\x0csession_step\x18\x02 \x01(\x0b\x32\x17.ondewo.nlu.SessionStep\x12.\n\x0csession_view\x18\x03 \x01(\x0e\x32\x18.ondewo.nlu.Session.View\"\xcc\x01\n\x13ListSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12.\n\x0csession_view\x18\x02 \x01(\x0e\x32\x18.ondewo.nlu.Session.View\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x31\n\x0esession_filter\x18\x05 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\x12.\n\nfield_mask\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"s\n\rContextFilter\x12\x14\n\x0c\x63ontext_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x30\n\x08operator\x18\x04 \x01(\x0e\x32\x1e.ondewo.nlu.ComparisonOperator\"\xd5\r\n\rSessionFilter\x12\x16\n\x0elanguage_codes\x18\x01 \x03(\t\x12+\n\x0fmatched_intents\x18\x02 \x03(\x0b\x32\x12.ondewo.nlu.Intent\x12\x34\n\x14matched_entity_types\x18\x03 \x03(\x0b\x32\x16.ondewo.nlu.EntityType\x12\"\n\x1amin_intents_confidence_min\x18\x04 \x01(\x02\x12\"\n\x1amin_intents_confidence_max\x18\x05 \x01(\x02\x12\'\n\x1fmin_entity_types_confidence_min\x18\x06 \x01(\x02\x12\'\n\x1fmin_entity_types_confidence_max\x18\x07 \x01(\x02\x12\x10\n\x08\x65\x61rliest\x18\x08 \x01(\x01\x12\x0e\n\x06latest\x18\t \x01(\x01\x12\x18\n\x10min_number_turns\x18\n \x01(\x05\x12\x18\n\x10max_number_turns\x18\x0b \x01(\x05\x12\x0e\n\x06labels\x18\x0c \x03(\t\x12\x10\n\x08user_ids\x18\r \x03(\t\x12\x13\n\x0bintent_tags\x18\x0e \x03(\t\x12\x13\n\x0bsession_ids\x18\x0f \x03(\t\x12+\n\x0einput_contexts\x18\x10 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12,\n\x0foutput_contexts\x18\x11 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x19\n\x11\x64uration_in_s_min\x18\x12 \x01(\x02\x12\x19\n\x11\x64uration_in_s_max\x18\x13 \x01(\x02\x12\x19\n\x11\x64uration_in_m_min\x18\x14 \x01(\x02\x12\x19\n\x11\x64uration_in_m_max\x18\x15 \x01(\x02\x12!\n\x19\x64uration_in_m_rounded_min\x18\x16 \x01(\x02\x12!\n\x19\x64uration_in_m_rounded_max\x18\x17 \x01(\x02\x12)\n!duration_interval_15s_rounded_min\x18\x18 \x01(\x02\x12)\n!duration_interval_15s_rounded_max\x18\x19 \x01(\x02\x12)\n!duration_interval_30s_rounded_min\x18\x1a \x01(\x02\x12)\n!duration_interval_30s_rounded_max\x18\x1b \x01(\x02\x12)\n!duration_interval_45s_rounded_min\x18\x1c \x01(\x02\x12)\n!duration_interval_45s_rounded_max\x18\x1d \x01(\x02\x12&\n\x1estarted_time_slot_per_hour_min\x18\x1e \x01(\t\x12&\n\x1estarted_time_slot_per_hour_max\x18\x1f \x01(\t\x12.\n&started_time_slot_per_quarter_hour_min\x18  \x01(\t\x12.\n&started_time_slot_per_quarter_hour_max\x18! \x01(\t\x12+\n#started_time_slot_per_half_hour_min\x18\" \x01(\t\x12+\n#started_time_slot_per_half_hour_max\x18# \x01(\t\x12+\n#started_time_slot_per_day_phase_min\x18$ \x01(\t\x12+\n#started_time_slot_per_day_phase_max\x18% \x01(\t\x12(\n started_time_slot_per_minute_min\x18& \x01(\t\x12(\n started_time_slot_per_minute_max\x18\' \x01(\t\x12!\n\x19\x64uration_in_s_rounded_min\x18( \x01(\x02\x12!\n\x19\x64uration_in_s_rounded_max\x18) \x01(\x02\x12\x36\n\tplatforms\x18* \x03(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\x12\x13\n\x0b\x61\x63\x63ount_ids\x18+ \x03(\t\x12\x14\n\x0cproperty_ids\x18, \x03(\t\x12\x16\n\x0e\x64\x61tastream_ids\x18- \x03(\t\x12\x12\n\norigin_ids\x18. \x03(\t\x12\x1b\n\x13identified_user_ids\x18/ \x03(\t\x12)\n!duration_interval_60s_rounded_min\x18\x30 \x01(\x02\x12)\n!duration_interval_60s_rounded_max\x18\x31 \x01(\x02\"\xf6\x08\n\x0bSessionInfo\x12\x16\n\x0elanguage_codes\x18\x01 \x03(\t\x12+\n\x0fmatched_intents\x18\x02 \x03(\x0b\x32\x12.ondewo.nlu.Intent\x12\x34\n\x14matched_entity_types\x18\x03 \x03(\x0b\x32\x16.ondewo.nlu.EntityType\x12\x1e\n\x16min_intents_confidence\x18\x04 \x01(\x02\x12#\n\x1bmin_entity_types_confidence\x18\x05 \x01(\x02\x12\x10\n\x08\x65\x61rliest\x18\x06 \x01(\x01\x12\x0e\n\x06latest\x18\x07 \x01(\x01\x12\x14\n\x0cnumber_turns\x18\x08 \x01(\x05\x12\x0e\n\x06labels\x18\t \x03(\t\x12\x10\n\x08user_ids\x18\n \x03(\t\x12\x13\n\x0bintent_tags\x18\x0b \x03(\t\x12\x41\n\x13input_context_steps\x18\x0c \x03(\x0b\x32$.ondewo.nlu.SessionInfo.ContextSteps\x12\x42\n\x14output_context_steps\x18\r \x03(\x0b\x32$.ondewo.nlu.SessionInfo.ContextSteps\x12\x15\n\rduration_in_s\x18\x0e \x01(\x02\x12\x15\n\rduration_in_m\x18\x0f \x01(\x02\x12\x1d\n\x15\x64uration_in_m_rounded\x18\x10 \x01(\x02\x12%\n\x1d\x64uration_interval_15s_rounded\x18\x11 \x01(\x02\x12%\n\x1d\x64uration_interval_30s_rounded\x18\x12 \x01(\x02\x12%\n\x1d\x64uration_interval_45s_rounded\x18\x13 \x01(\x02\x12\"\n\x1astarted_time_slot_per_hour\x18\x14 \x01(\t\x12*\n\"started_time_slot_per_quarter_hour\x18\x15 \x01(\t\x12\'\n\x1fstarted_time_slot_per_half_hour\x18\x16 \x01(\t\x12\'\n\x1fstarted_time_slot_per_day_phase\x18\x17 \x01(\t\x12$\n\x1cstarted_time_slot_per_minute\x18\x18 \x01(\t\x12\x1d\n\x15\x64uration_in_s_rounded\x18\x19 \x01(\x02\x12\x36\n\tplatforms\x18\x1a \x03(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\x12\x13\n\x0b\x61\x63\x63ount_ids\x18\x1b \x03(\t\x12\x14\n\x0cproperty_ids\x18\x1c \x03(\t\x12\x16\n\x0e\x64\x61tastream_ids\x18\x1d \x03(\t\x12\x12\n\norigin_ids\x18\x1e \x03(\t\x12\x1b\n\x13identified_user_ids\x18\x1f \x03(\t\x12%\n\x1d\x64uration_interval_60s_rounded\x18  \x01(\x02\x1a\x35\n\x0c\x43ontextSteps\x12%\n\x08\x63ontexts\x18\x01 \x03(\x0b\x32\x13.ondewo.nlu.Context\"V\n\x14ListSessionsResponse\x12%\n\x08sessions\x18\x01 \x03(\x0b\x32\x13.ondewo.nlu.Session\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x87\x01\n\x11GetSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12.\n\x0csession_view\x18\x02 \x01(\x0e\x32\x18.ondewo.nlu.Session.View\x12.\n\nfield_mask\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"s\n\x14\x43reateSessionRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x14\n\x0csession_uuid\x18\x02 \x01(\t\x12\x0e\n\x06labels\x18\x03 \x03(\t\x12%\n\x08\x63ontexts\x18\x04 \x03(\x0b\x32\x13.ondewo.nlu.Context\"*\n\x14\x44\x65leteSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"\xba\x01\n\x1a\x43reateSessionReviewRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x18\n\x10parent_review_id\x18\x02 \x01(\t\x12\x31\n\x0esession_review\x18\x03 \x01(\x0b\x32\x19.ondewo.nlu.SessionReview\x12;\n\x13session_review_view\x18\x04 \x01(\x0e\x32\x1e.ondewo.nlu.SessionReview.View\"\x98\x01\n\rSessionReview\x12\x0c\n\x04name\x18\x01 \x01(\t\x12;\n\x14session_review_steps\x18\x02 \x03(\x0b\x32\x1d.ondewo.nlu.SessionReviewStep\"<\n\x04View\x12\x14\n\x10VIEW_UNSPECIFIED\x10\x00\x12\r\n\tVIEW_FULL\x10\x01\x12\x0f\n\x0bVIEW_SPARSE\x10\x02\"\xd4\x02\n\x11SessionReviewStep\x12\x0c\n\x04name\x18\x01 \x01(\t\x12=\n\x12\x61nnotated_usersays\x18\x02 \x01(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12\x34\n\x10\x64\x65tected_intents\x18\x04 \x03(\x0b\x32\x1a.ondewo.nlu.DetectedIntent\x12%\n\x08\x63ontexts\x18\x05 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12)\n\x0c\x63ontexts_out\x18\x06 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x1b\n\x13query_text_original\x18\x07 \x01(\t\x12\x36\n\tplatforms\x18\x08 \x03(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\"\xb0\x01\n\x0e\x44\x65tectedIntent\x12\"\n\x06intent\x18\x01 \x01(\x0b\x32\x12.ondewo.nlu.Intent\x12\r\n\x05score\x18\x02 \x01(\x02\x12\x11\n\talgorithm\x18\x03 \x01(\t\x12\x38\n\x14\x66ulfillment_messages\x18\x04 \x03(\x0b\x32\x1a.ondewo.nlu.Intent.Message\x12\x1e\n\x16required_param_missing\x18\x05 \x01(\x08\".\n\x18ListSessionLabelsRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"j\n%ListSessionLabelsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"+\n\x19ListSessionLabelsResponse\x12\x0e\n\x06labels\x18\x01 \x03(\t\"j\n%ListLanguageCodesOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"3\n\x19ListLanguageCodesResponse\x12\x16\n\x0elanguage_codes\x18\x01 \x03(\t\"k\n&ListMatchedIntentsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"5\n\x1aListMatchedIntentsResponse\x12\x17\n\x0fmatched_intents\x18\x01 \x03(\t\"o\n*ListMatchedEntityTypesOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\">\n\x1eListMatchedEntityTypesResponse\x12\x1c\n\x14matched_entity_types\x18\x01 \x03(\t\"d\n\x1fListUserIdsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"\'\n\x13ListUserIdsResponse\x12\x10\n\x08user_ids\x18\x01 \x03(\t\"n\n)ListIdentifiedUserIdsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"<\n\x1dListIdentifiedUserIdsResponse\x12\x1b\n\x13identified_user_ids\x18\x01 \x03(\t\"a\n\x1cListTagsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\" \n\x10ListTagsResponse\x12\x0c\n\x04tags\x18\x01 \x03(\t\"j\n%ListInputContextsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"3\n\x19ListInputContextsResponse\x12\x16\n\x0einput_contexts\x18\x01 \x03(\t\"k\n&ListOutputContextsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"5\n\x1aListOutputContextsResponse\x12\x17\n\x0foutput_contexts\x18\x01 \x03(\t\"f\n!ListPlatformsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"*\n\x15ListPlatformsResponse\x12\x11\n\tplatforms\x18\x01 \x03(\t\"g\n\"ListAccountIdsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"-\n\x16ListAccountIdsResponse\x12\x13\n\x0b\x61\x63\x63ount_ids\x18\x01 \x03(\t\"h\n#ListPropertyIdsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"/\n\x17ListPropertyIdsResponse\x12\x14\n\x0cproperty_ids\x18\x01 \x03(\t\"j\n%ListDatastreamIdsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"3\n\x19ListDatastreamIdsResponse\x12\x16\n\x0e\x64\x61tastream_ids\x18\x01 \x03(\t\"f\n!ListOriginIdsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"+\n\x15ListOriginIdsResponse\x12\x12\n\norigin_ids\x18\x01 \x03(\t\"=\n\x17\x41\x64\x64SessionLabelsRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0e\n\x06labels\x18\x02 \x03(\t\"@\n\x1a\x44\x65leteSessionLabelsRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0e\n\x06labels\x18\x02 \x03(\t\"\x80\x01\n\x19ListSessionReviewsRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12;\n\x13session_review_view\x18\x02 \x01(\x0e\x32\x1e.ondewo.nlu.SessionReview.View\x12\x12\n\npage_token\x18\x04 \x01(\t\"i\n\x1aListSessionReviewsResponse\x12\x32\n\x0fsession_reviews\x18\x01 \x03(\x0b\x32\x19.ondewo.nlu.SessionReview\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"q\n\x17GetSessionReviewRequest\x12\x19\n\x11session_review_id\x18\x01 \x01(\t\x12;\n\x13session_review_view\x18\x02 \x01(\x0e\x32\x1e.ondewo.nlu.SessionReview.View\"p\n\x1dGetLatestSessionReviewRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12;\n\x13session_review_view\x18\x02 \x01(\x0e\x32\x1e.ondewo.nlu.SessionReview.View*\xfb\x01\n\rAudioEncoding\x12\x1e\n\x1a\x41UDIO_ENCODING_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x41UDIO_ENCODING_LINEAR_16\x10\x01\x12\x17\n\x13\x41UDIO_ENCODING_FLAC\x10\x02\x12\x18\n\x14\x41UDIO_ENCODING_MULAW\x10\x03\x12\x16\n\x12\x41UDIO_ENCODING_AMR\x10\x04\x12\x19\n\x15\x41UDIO_ENCODING_AMR_WB\x10\x05\x12\x1b\n\x17\x41UDIO_ENCODING_OGG_OPUS\x10\x06\x12)\n%AUDIO_ENCODING_SPEEX_WITH_HEADER_BYTE\x10\x07*\x83\x01\n\x12\x43omparisonOperator\x12\t\n\x05\x45QUAL\x10\x00\x12\x0b\n\x07GREATER\x10\x01\x12\x14\n\x10GREATER_OR_EQUAL\x10\x02\x12\x11\n\rLESS_OR_EQUAL\x10\x03\x12\x0c\n\x08\x43ONTAINS\x10\x04\x12\x0f\n\x0bSTARTS_WITH\x10\x05\x12\r\n\tENDS_WITH\x10\x06\x32\x8d$\n\x08Sessions\x12\x94\x01\n\x0c\x44\x65tectIntent\x12\x1f.ondewo.nlu.DetectIntentRequest\x1a .ondewo.nlu.DetectIntentResponse\"A\x82\xd3\xe4\x93\x02;\"6/v2/{session=projects/*/agent/sessions/*}:detectIntent:\x01*\x12p\n\x15StreamingDetectIntent\x12(.ondewo.nlu.StreamingDetectIntentRequest\x1a).ondewo.nlu.StreamingDetectIntentResponse(\x01\x30\x01\x12\x81\x01\n\x0cListSessions\x12\x1f.ondewo.nlu.ListSessionsRequest\x1a .ondewo.nlu.ListSessionsResponse\".\x82\xd3\xe4\x93\x02(\x12&/v2/{parent=projects/*/agent}/sessions\x12v\n\nGetSession\x12\x1d.ondewo.nlu.GetSessionRequest\x1a\x13.ondewo.nlu.Session\"4\x82\xd3\xe4\x93\x02.\x12,/v2/{session_id=projects/*/agent/sessions/*}\x12y\n\rCreateSession\x12 .ondewo.nlu.CreateSessionRequest\x1a\x13.ondewo.nlu.Session\"1\x82\xd3\xe4\x93\x02+\"&/v2/{parent=projects/*/agent}/sessions:\x01*\x12\x96\x01\n\x10TrackSessionStep\x12#.ondewo.nlu.TrackSessionStepRequest\x1a\x13.ondewo.nlu.Session\"H\x82\xd3\xe4\x93\x02\x42\"=/v2/{session_id=projects/*/agent/sessions/*}:trackSessionStep:\x01*\x12\x7f\n\rDeleteSession\x12 .ondewo.nlu.DeleteSessionRequest\x1a\x16.google.protobuf.Empty\"4\x82\xd3\xe4\x93\x02.*,/v2/{session_id=projects/*/agent/sessions/*}\x12\x9d\x01\n\x11ListSessionLabels\x12$.ondewo.nlu.ListSessionLabelsRequest\x1a%.ondewo.nlu.ListSessionLabelsResponse\";\x82\xd3\xe4\x93\x02\x35\x12\x33/v2/{session_id=projects/*/agent/sessions/*}/labels\x12\xb1\x01\n\x1eListSessionLabelsOfAllSessions\x12\x31.ondewo.nlu.ListSessionLabelsOfAllSessionsRequest\x1a%.ondewo.nlu.ListSessionLabelsResponse\"5\x82\xd3\xe4\x93\x02/\x12-/v2/{parent=projects/*/agent}/sessions/labels\x12\xb9\x01\n\x1eListLanguageCodesOfAllSessions\x12\x31.ondewo.nlu.ListLanguageCodesOfAllSessionsRequest\x1a%.ondewo.nlu.ListLanguageCodesResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/v2/{parent=projects/*/agent}/sessions/language_codes\x12\xbd\x01\n\x1fListMatchedIntentsOfAllSessions\x12\x32.ondewo.nlu.ListMatchedIntentsOfAllSessionsRequest\x1a&.ondewo.nlu.ListMatchedIntentsResponse\">\x82\xd3\xe4\x93\x02\x38\x12\x36/v2/{parent=projects/*/agent}/sessions/matched_intents\x12\xce\x01\n#ListMatchedEntityTypesOfAllSessions\x12\x36.ondewo.nlu.ListMatchedEntityTypesOfAllSessionsRequest\x1a*.ondewo.nlu.ListMatchedEntityTypesResponse\"C\x82\xd3\xe4\x93\x02=\x12;/v2/{parent=projects/*/agent}/sessions/matched_entity_types\x12\xa1\x01\n\x18ListUserIdsOfAllSessions\x12+.ondewo.nlu.ListUserIdsOfAllSessionsRequest\x1a\x1f.ondewo.nlu.ListUserIdsResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//v2/{parent=projects/*/agent}/sessions/user_ids\x12\xca\x01\n\"ListIdentifiedUserIdsOfAllSessions\x12\x35.ondewo.nlu.ListIdentifiedUserIdsOfAllSessionsRequest\x1a).ondewo.nlu.ListIdentifiedUserIdsResponse\"B\x82\xd3\xe4\x93\x02<\x12:/v2/{parent=projects/*/agent}/sessions/identified_user_ids\x12\x94\x01\n\x15ListTagsOfAllSessions\x12(.ondewo.nlu.ListTagsOfAllSessionsRequest\x1a\x1c.ondewo.nlu.ListTagsResponse\"3\x82\xd3\xe4\x93\x02-\x12+/v2/{parent=projects/*/agent}/sessions/tags\x12\xb9\x01\n\x1eListInputContextsOfAllSessions\x12\x31.ondewo.nlu.ListInputContextsOfAllSessionsRequest\x1a%.ondewo.nlu.ListInputContextsResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/v2/{parent=projects/*/agent}/sessions/input_contexts\x12\xbd\x01\n\x1fListOutputContextsOfAllSessions\x12\x32.ondewo.nlu.ListOutputContextsOfAllSessionsRequest\x1a&.ondewo.nlu.ListOutputContextsResponse\">\x82\xd3\xe4\x93\x02\x38\x12\x36/v2/{parent=projects/*/agent}/sessions/output_contexts\x12\xa8\x01\n\x1aListPlatformsOfAllSessions\x12-.ondewo.nlu.ListPlatformsOfAllSessionsRequest\x1a!.ondewo.nlu.ListPlatformsResponse\"8\x82\xd3\xe4\x93\x02\x32\x12\x30/v2/{parent=projects/*/agent}/sessions/platforms\x12\xad\x01\n\x1bListAccountIdsOfAllSessions\x12..ondewo.nlu.ListAccountIdsOfAllSessionsRequest\x1a\".ondewo.nlu.ListAccountIdsResponse\":\x82\xd3\xe4\x93\x02\x34\x12\x32/v2/{parent=projects/*/agent}/sessions/account_ids\x12\xb1\x01\n\x1cListPropertyIdsOfAllSessions\x12/.ondewo.nlu.ListPropertyIdsOfAllSessionsRequest\x1a#.ondewo.nlu.ListPropertyIdsResponse\";\x82\xd3\xe4\x93\x02\x35\x12\x33/v2/{parent=projects/*/agent}/sessions/property_ids\x12\xb9\x01\n\x1eListDatastreamIdsOfAllSessions\x12\x31.ondewo.nlu.ListDatastreamIdsOfAllSessionsRequest\x1a%.ondewo.nlu.ListDatastreamIdsResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/v2/{parent=projects/*/agent}/sessions/datastream_ids\x12\xa9\x01\n\x1aListOriginIdsOfAllSessions\x12-.ondewo.nlu.ListOriginIdsOfAllSessionsRequest\x1a!.ondewo.nlu.ListOriginIdsResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v2/{parent=projects/*/agent}/sessions/origin_ids\x12\x90\x01\n\x10\x41\x64\x64SessionLabels\x12#.ondewo.nlu.AddSessionLabelsRequest\x1a\x13.ondewo.nlu.Session\"B\x82\xd3\xe4\x93\x02<\"7/v2/{session_id=projects/*/agent/sessions/*}/labels:add:\x01*\x12\x99\x01\n\x13\x44\x65leteSessionLabels\x12&.ondewo.nlu.DeleteSessionLabelsRequest\x1a\x13.ondewo.nlu.Session\"E\x82\xd3\xe4\x93\x02?\":/v2/{session_id=projects/*/agent/sessions/*}/labels:delete:\x01*\x12\xa1\x01\n\x12ListSessionReviews\x12%.ondewo.nlu.ListSessionReviewsRequest\x1a&.ondewo.nlu.ListSessionReviewsResponse\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/v2/{session_id=projects/*/agent/sessions/*}/reviews\x12\x99\x01\n\x10GetSessionReview\x12#.ondewo.nlu.GetSessionReviewRequest\x1a\x19.ondewo.nlu.SessionReview\"E\x82\xd3\xe4\x93\x02?\x12=/v2/{session_review_id=projects/*/agent/sessions/*/reviews/*}\x12\xb3\x01\n\x16GetLatestSessionReview\x12).ondewo.nlu.GetLatestSessionReviewRequest\x1a\x19.ondewo.nlu.SessionReview\"S\x82\xd3\xe4\x93\x02M\x12K/v2/{session_id=projects/*/agent/sessions/*}/reviews:getLatestSessionReview\x12\xa5\x01\n\x13\x43reateSessionReview\x12&.ondewo.nlu.CreateSessionReviewRequest\x1a\x19.ondewo.nlu.SessionReview\"K\x82\xd3\xe4\x93\x02\x45\"@/v2/{session_id=projects/*/agent/sessions/*}:createSessionReview:\x01*B\x9b\x01\n\x1e\x63om.google.cloud.dialogflow.v2B\x0cSessionProtoP\x01ZDgoogle.golang.org/genproto/googleapis/cloud/dialogflow/v2;dialogflow\xf8\x01\x01\xa2\x02\x02\x44\x46\xaa\x02\x1aGoogle.Cloud.Dialogflow.V2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18ondewo/nlu/session.proto\x12\nondewo.nlu\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17google/rpc/status.proto\x1a\x18google/type/latlng.proto\x1a\x18ondewo/nlu/context.proto\x1a\x17ondewo/nlu/intent.proto\x1a\x1condewo/nlu/entity_type.proto\"\x9b\x01\n\x13\x44\x65tectIntentRequest\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x31\n\x0cquery_params\x18\x02 \x01(\x0b\x32\x1b.ondewo.nlu.QueryParameters\x12+\n\x0bquery_input\x18\x03 \x01(\x0b\x32\x16.ondewo.nlu.QueryInput\x12\x13\n\x0binput_audio\x18\x05 \x01(\x0c\"\x86\x01\n\x14\x44\x65tectIntentResponse\x12\x13\n\x0bresponse_id\x18\x01 \x01(\t\x12-\n\x0cquery_result\x18\x02 \x01(\x0b\x32\x17.ondewo.nlu.QueryResult\x12*\n\x0ewebhook_status\x18\x03 \x01(\x0b\x32\x12.google.rpc.Status\"\xef\x02\n\x0fQueryParameters\x12\x11\n\ttime_zone\x18\x01 \x01(\t\x12)\n\x0cgeo_location\x18\x02 \x01(\x0b\x32\x13.google.type.LatLng\x12%\n\x08\x63ontexts\x18\x03 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x16\n\x0ereset_contexts\x18\x04 \x01(\x08\x12(\n\x07payload\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06labels\x18\x07 \x03(\t\x12\x36\n\tplatforms\x18\x08 \x03(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\x12\x12\n\naccount_id\x18\t \x01(\t\x12\x13\n\x0bproperty_id\x18\n \x01(\t\x12\x15\n\rdatastream_id\x18\x0b \x01(\t\x12\x11\n\torigin_id\x18\x0c \x01(\t\x12\x1a\n\x12identified_user_id\x18\r \x01(\t\"\x9b\x01\n\nQueryInput\x12\x34\n\x0c\x61udio_config\x18\x01 \x01(\x0b\x32\x1c.ondewo.nlu.InputAudioConfigH\x00\x12%\n\x04text\x18\x02 \x01(\x0b\x32\x15.ondewo.nlu.TextInputH\x00\x12\'\n\x05\x65vent\x18\x03 \x01(\x0b\x32\x16.ondewo.nlu.EventInputH\x00\x42\x07\n\x05input\"\xa5\x04\n\x0bQueryResult\x12\x12\n\nquery_text\x18\x01 \x01(\t\x12%\n\x1dspeech_recognition_confidence\x18\x02 \x01(\x02\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12+\n\nparameters\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12#\n\x1b\x61ll_required_params_present\x18\x05 \x01(\x08\x12\x18\n\x10\x66ulfillment_text\x18\x06 \x01(\t\x12\x38\n\x14\x66ulfillment_messages\x18\x07 \x03(\x0b\x32\x1a.ondewo.nlu.Intent.Message\x12\x16\n\x0ewebhook_source\x18\x08 \x01(\t\x12\x30\n\x0fwebhook_payload\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\x0foutput_contexts\x18\n \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\"\n\x06intent\x18\x0b \x01(\x0b\x32\x12.ondewo.nlu.Intent\x12#\n\x1bintent_detection_confidence\x18\x0c \x01(\x02\x12\x1b\n\x13query_text_original\x18\r \x01(\t\x12\x30\n\x0f\x64iagnostic_info\x18\x0e \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x15\n\rlanguage_code\x18\x0f \x01(\t\"\xbe\x01\n\x1cStreamingDetectIntentRequest\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x31\n\x0cquery_params\x18\x02 \x01(\x0b\x32\x1b.ondewo.nlu.QueryParameters\x12+\n\x0bquery_input\x18\x03 \x01(\x0b\x32\x16.ondewo.nlu.QueryInput\x12\x18\n\x10single_utterance\x18\x04 \x01(\x08\x12\x13\n\x0binput_audio\x18\x06 \x01(\x0c\"\xd3\x01\n\x1dStreamingDetectIntentResponse\x12\x13\n\x0bresponse_id\x18\x01 \x01(\t\x12\x42\n\x12recognition_result\x18\x02 \x01(\x0b\x32&.ondewo.nlu.StreamingRecognitionResult\x12-\n\x0cquery_result\x18\x03 \x01(\x0b\x32\x17.ondewo.nlu.QueryResult\x12*\n\x0ewebhook_status\x18\x04 \x01(\x0b\x32\x12.google.rpc.Status\"\xfa\x01\n\x1aStreamingRecognitionResult\x12H\n\x0cmessage_type\x18\x01 \x01(\x0e\x32\x32.ondewo.nlu.StreamingRecognitionResult.MessageType\x12\x12\n\ntranscript\x18\x02 \x01(\t\x12\x10\n\x08is_final\x18\x03 \x01(\x08\x12\x12\n\nconfidence\x18\x04 \x01(\x02\"X\n\x0bMessageType\x12\x1c\n\x18MESSAGE_TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTRANSCRIPT\x10\x01\x12\x1b\n\x17\x45ND_OF_SINGLE_UTTERANCE\x10\x02\"\x8d\x01\n\x10InputAudioConfig\x12\x31\n\x0e\x61udio_encoding\x18\x01 \x01(\x0e\x32\x19.ondewo.nlu.AudioEncoding\x12\x19\n\x11sample_rate_hertz\x18\x02 \x01(\x05\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12\x14\n\x0cphrase_hints\x18\x04 \x03(\t\"0\n\tTextInput\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\"^\n\nEventInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\nparameters\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\"\xb4\x01\n\x07Session\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\rsession_steps\x18\x02 \x03(\x0b\x32\x17.ondewo.nlu.SessionStep\x12-\n\x0csession_info\x18\x03 \x01(\x0b\x32\x17.ondewo.nlu.SessionInfo\"<\n\x04View\x12\x14\n\x10VIEW_UNSPECIFIED\x10\x00\x12\r\n\tVIEW_FULL\x10\x01\x12\x0f\n\x0bVIEW_SPARSE\x10\x02\"\xf3\x01\n\x0bSessionStep\x12\x0c\n\x04name\x18\x01 \x01(\t\x12>\n\x15\x64\x65tect_intent_request\x18\x02 \x01(\x0b\x32\x1f.ondewo.nlu.DetectIntentRequest\x12@\n\x16\x64\x65tect_intent_response\x18\x03 \x01(\x0b\x32 .ondewo.nlu.DetectIntentResponse\x12%\n\x08\x63ontexts\x18\x04 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12-\n\ttimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8c\x01\n\x17TrackSessionStepRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12-\n\x0csession_step\x18\x02 \x01(\x0b\x32\x17.ondewo.nlu.SessionStep\x12.\n\x0csession_view\x18\x03 \x01(\x0e\x32\x18.ondewo.nlu.Session.View\"\xcc\x01\n\x13ListSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12.\n\x0csession_view\x18\x02 \x01(\x0e\x32\x18.ondewo.nlu.Session.View\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x31\n\x0esession_filter\x18\x05 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\x12.\n\nfield_mask\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"s\n\rContextFilter\x12\x14\n\x0c\x63ontext_name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x30\n\x08operator\x18\x04 \x01(\x0e\x32\x1e.ondewo.nlu.ComparisonOperator\"\xd5\r\n\rSessionFilter\x12\x16\n\x0elanguage_codes\x18\x01 \x03(\t\x12+\n\x0fmatched_intents\x18\x02 \x03(\x0b\x32\x12.ondewo.nlu.Intent\x12\x34\n\x14matched_entity_types\x18\x03 \x03(\x0b\x32\x16.ondewo.nlu.EntityType\x12\"\n\x1amin_intents_confidence_min\x18\x04 \x01(\x02\x12\"\n\x1amin_intents_confidence_max\x18\x05 \x01(\x02\x12\'\n\x1fmin_entity_types_confidence_min\x18\x06 \x01(\x02\x12\'\n\x1fmin_entity_types_confidence_max\x18\x07 \x01(\x02\x12\x10\n\x08\x65\x61rliest\x18\x08 \x01(\x01\x12\x0e\n\x06latest\x18\t \x01(\x01\x12\x18\n\x10min_number_turns\x18\n \x01(\x05\x12\x18\n\x10max_number_turns\x18\x0b \x01(\x05\x12\x0e\n\x06labels\x18\x0c \x03(\t\x12\x10\n\x08user_ids\x18\r \x03(\t\x12\x13\n\x0bintent_tags\x18\x0e \x03(\t\x12\x13\n\x0bsession_ids\x18\x0f \x03(\t\x12+\n\x0einput_contexts\x18\x10 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12,\n\x0foutput_contexts\x18\x11 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x19\n\x11\x64uration_in_s_min\x18\x12 \x01(\x02\x12\x19\n\x11\x64uration_in_s_max\x18\x13 \x01(\x02\x12\x19\n\x11\x64uration_in_m_min\x18\x14 \x01(\x02\x12\x19\n\x11\x64uration_in_m_max\x18\x15 \x01(\x02\x12!\n\x19\x64uration_in_m_rounded_min\x18\x16 \x01(\x02\x12!\n\x19\x64uration_in_m_rounded_max\x18\x17 \x01(\x02\x12)\n!duration_interval_15s_rounded_min\x18\x18 \x01(\x02\x12)\n!duration_interval_15s_rounded_max\x18\x19 \x01(\x02\x12)\n!duration_interval_30s_rounded_min\x18\x1a \x01(\x02\x12)\n!duration_interval_30s_rounded_max\x18\x1b \x01(\x02\x12)\n!duration_interval_45s_rounded_min\x18\x1c \x01(\x02\x12)\n!duration_interval_45s_rounded_max\x18\x1d \x01(\x02\x12&\n\x1estarted_time_slot_per_hour_min\x18\x1e \x01(\t\x12&\n\x1estarted_time_slot_per_hour_max\x18\x1f \x01(\t\x12.\n&started_time_slot_per_quarter_hour_min\x18  \x01(\t\x12.\n&started_time_slot_per_quarter_hour_max\x18! \x01(\t\x12+\n#started_time_slot_per_half_hour_min\x18\" \x01(\t\x12+\n#started_time_slot_per_half_hour_max\x18# \x01(\t\x12+\n#started_time_slot_per_day_phase_min\x18$ \x01(\t\x12+\n#started_time_slot_per_day_phase_max\x18% \x01(\t\x12(\n started_time_slot_per_minute_min\x18& \x01(\t\x12(\n started_time_slot_per_minute_max\x18\' \x01(\t\x12!\n\x19\x64uration_in_s_rounded_min\x18( \x01(\x02\x12!\n\x19\x64uration_in_s_rounded_max\x18) \x01(\x02\x12\x36\n\tplatforms\x18* \x03(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\x12\x13\n\x0b\x61\x63\x63ount_ids\x18+ \x03(\t\x12\x14\n\x0cproperty_ids\x18, \x03(\t\x12\x16\n\x0e\x64\x61tastream_ids\x18- \x03(\t\x12\x12\n\norigin_ids\x18. \x03(\t\x12\x1b\n\x13identified_user_ids\x18/ \x03(\t\x12)\n!duration_interval_60s_rounded_min\x18\x30 \x01(\x02\x12)\n!duration_interval_60s_rounded_max\x18\x31 \x01(\x02\"\xf6\x08\n\x0bSessionInfo\x12\x16\n\x0elanguage_codes\x18\x01 \x03(\t\x12+\n\x0fmatched_intents\x18\x02 \x03(\x0b\x32\x12.ondewo.nlu.Intent\x12\x34\n\x14matched_entity_types\x18\x03 \x03(\x0b\x32\x16.ondewo.nlu.EntityType\x12\x1e\n\x16min_intents_confidence\x18\x04 \x01(\x02\x12#\n\x1bmin_entity_types_confidence\x18\x05 \x01(\x02\x12\x10\n\x08\x65\x61rliest\x18\x06 \x01(\x01\x12\x0e\n\x06latest\x18\x07 \x01(\x01\x12\x14\n\x0cnumber_turns\x18\x08 \x01(\x05\x12\x0e\n\x06labels\x18\t \x03(\t\x12\x10\n\x08user_ids\x18\n \x03(\t\x12\x13\n\x0bintent_tags\x18\x0b \x03(\t\x12\x41\n\x13input_context_steps\x18\x0c \x03(\x0b\x32$.ondewo.nlu.SessionInfo.ContextSteps\x12\x42\n\x14output_context_steps\x18\r \x03(\x0b\x32$.ondewo.nlu.SessionInfo.ContextSteps\x12\x15\n\rduration_in_s\x18\x0e \x01(\x02\x12\x15\n\rduration_in_m\x18\x0f \x01(\x02\x12\x1d\n\x15\x64uration_in_m_rounded\x18\x10 \x01(\x02\x12%\n\x1d\x64uration_interval_15s_rounded\x18\x11 \x01(\x02\x12%\n\x1d\x64uration_interval_30s_rounded\x18\x12 \x01(\x02\x12%\n\x1d\x64uration_interval_45s_rounded\x18\x13 \x01(\x02\x12\"\n\x1astarted_time_slot_per_hour\x18\x14 \x01(\t\x12*\n\"started_time_slot_per_quarter_hour\x18\x15 \x01(\t\x12\'\n\x1fstarted_time_slot_per_half_hour\x18\x16 \x01(\t\x12\'\n\x1fstarted_time_slot_per_day_phase\x18\x17 \x01(\t\x12$\n\x1cstarted_time_slot_per_minute\x18\x18 \x01(\t\x12\x1d\n\x15\x64uration_in_s_rounded\x18\x19 \x01(\x02\x12\x36\n\tplatforms\x18\x1a \x03(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\x12\x13\n\x0b\x61\x63\x63ount_ids\x18\x1b \x03(\t\x12\x14\n\x0cproperty_ids\x18\x1c \x03(\t\x12\x16\n\x0e\x64\x61tastream_ids\x18\x1d \x03(\t\x12\x12\n\norigin_ids\x18\x1e \x03(\t\x12\x1b\n\x13identified_user_ids\x18\x1f \x03(\t\x12%\n\x1d\x64uration_interval_60s_rounded\x18  \x01(\x02\x1a\x35\n\x0c\x43ontextSteps\x12%\n\x08\x63ontexts\x18\x01 \x03(\x0b\x32\x13.ondewo.nlu.Context\"V\n\x14ListSessionsResponse\x12%\n\x08sessions\x18\x01 \x03(\x0b\x32\x13.ondewo.nlu.Session\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x87\x01\n\x11GetSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12.\n\x0csession_view\x18\x02 \x01(\x0e\x32\x18.ondewo.nlu.Session.View\x12.\n\nfield_mask\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"s\n\x14\x43reateSessionRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x14\n\x0csession_uuid\x18\x02 \x01(\t\x12\x0e\n\x06labels\x18\x03 \x03(\t\x12%\n\x08\x63ontexts\x18\x04 \x03(\x0b\x32\x13.ondewo.nlu.Context\"*\n\x14\x44\x65leteSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"\xba\x01\n\x1a\x43reateSessionReviewRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x18\n\x10parent_review_id\x18\x02 \x01(\t\x12\x31\n\x0esession_review\x18\x03 \x01(\x0b\x32\x19.ondewo.nlu.SessionReview\x12;\n\x13session_review_view\x18\x04 \x01(\x0e\x32\x1e.ondewo.nlu.SessionReview.View\"\x98\x01\n\rSessionReview\x12\x0c\n\x04name\x18\x01 \x01(\t\x12;\n\x14session_review_steps\x18\x02 \x03(\x0b\x32\x1d.ondewo.nlu.SessionReviewStep\"<\n\x04View\x12\x14\n\x10VIEW_UNSPECIFIED\x10\x00\x12\r\n\tVIEW_FULL\x10\x01\x12\x0f\n\x0bVIEW_SPARSE\x10\x02\"\x83\x03\n\x11SessionReviewStep\x12\x0c\n\x04name\x18\x01 \x01(\t\x12=\n\x12\x61nnotated_usersays\x18\x02 \x01(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12\x34\n\x10\x64\x65tected_intents\x18\x04 \x03(\x0b\x32\x1a.ondewo.nlu.DetectedIntent\x12%\n\x08\x63ontexts\x18\x05 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12)\n\x0c\x63ontexts_out\x18\x06 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x1b\n\x13query_text_original\x18\x07 \x01(\t\x12\x36\n\tplatforms\x18\x08 \x03(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb0\x01\n\x0e\x44\x65tectedIntent\x12\"\n\x06intent\x18\x01 \x01(\x0b\x32\x12.ondewo.nlu.Intent\x12\r\n\x05score\x18\x02 \x01(\x02\x12\x11\n\talgorithm\x18\x03 \x01(\t\x12\x38\n\x14\x66ulfillment_messages\x18\x04 \x03(\x0b\x32\x1a.ondewo.nlu.Intent.Message\x12\x1e\n\x16required_param_missing\x18\x05 \x01(\x08\".\n\x18ListSessionLabelsRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"j\n%ListSessionLabelsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"+\n\x19ListSessionLabelsResponse\x12\x0e\n\x06labels\x18\x01 \x03(\t\"j\n%ListLanguageCodesOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"3\n\x19ListLanguageCodesResponse\x12\x16\n\x0elanguage_codes\x18\x01 \x03(\t\"k\n&ListMatchedIntentsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"5\n\x1aListMatchedIntentsResponse\x12\x17\n\x0fmatched_intents\x18\x01 \x03(\t\"o\n*ListMatchedEntityTypesOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\">\n\x1eListMatchedEntityTypesResponse\x12\x1c\n\x14matched_entity_types\x18\x01 \x03(\t\"d\n\x1fListUserIdsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"\'\n\x13ListUserIdsResponse\x12\x10\n\x08user_ids\x18\x01 \x03(\t\"n\n)ListIdentifiedUserIdsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"<\n\x1dListIdentifiedUserIdsResponse\x12\x1b\n\x13identified_user_ids\x18\x01 \x03(\t\"a\n\x1cListTagsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\" \n\x10ListTagsResponse\x12\x0c\n\x04tags\x18\x01 \x03(\t\"j\n%ListInputContextsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"3\n\x19ListInputContextsResponse\x12\x16\n\x0einput_contexts\x18\x01 \x03(\t\"k\n&ListOutputContextsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"5\n\x1aListOutputContextsResponse\x12\x17\n\x0foutput_contexts\x18\x01 \x03(\t\"f\n!ListPlatformsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"*\n\x15ListPlatformsResponse\x12\x11\n\tplatforms\x18\x01 \x03(\t\"g\n\"ListAccountIdsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"-\n\x16ListAccountIdsResponse\x12\x13\n\x0b\x61\x63\x63ount_ids\x18\x01 \x03(\t\"h\n#ListPropertyIdsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"/\n\x17ListPropertyIdsResponse\x12\x14\n\x0cproperty_ids\x18\x01 \x03(\t\"j\n%ListDatastreamIdsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"3\n\x19ListDatastreamIdsResponse\x12\x16\n\x0e\x64\x61tastream_ids\x18\x01 \x03(\t\"f\n!ListOriginIdsOfAllSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x31\n\x0esession_filter\x18\x02 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"+\n\x15ListOriginIdsResponse\x12\x12\n\norigin_ids\x18\x01 \x03(\t\"=\n\x17\x41\x64\x64SessionLabelsRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0e\n\x06labels\x18\x02 \x03(\t\"@\n\x1a\x44\x65leteSessionLabelsRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0e\n\x06labels\x18\x02 \x03(\t\"\x80\x01\n\x19ListSessionReviewsRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12;\n\x13session_review_view\x18\x02 \x01(\x0e\x32\x1e.ondewo.nlu.SessionReview.View\x12\x12\n\npage_token\x18\x04 \x01(\t\"i\n\x1aListSessionReviewsResponse\x12\x32\n\x0fsession_reviews\x18\x01 \x03(\x0b\x32\x19.ondewo.nlu.SessionReview\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"q\n\x17GetSessionReviewRequest\x12\x19\n\x11session_review_id\x18\x01 \x01(\t\x12;\n\x13session_review_view\x18\x02 \x01(\x0e\x32\x1e.ondewo.nlu.SessionReview.View\"p\n\x1dGetLatestSessionReviewRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12;\n\x13session_review_view\x18\x02 \x01(\x0e\x32\x1e.ondewo.nlu.SessionReview.View*\xfb\x01\n\rAudioEncoding\x12\x1e\n\x1a\x41UDIO_ENCODING_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x41UDIO_ENCODING_LINEAR_16\x10\x01\x12\x17\n\x13\x41UDIO_ENCODING_FLAC\x10\x02\x12\x18\n\x14\x41UDIO_ENCODING_MULAW\x10\x03\x12\x16\n\x12\x41UDIO_ENCODING_AMR\x10\x04\x12\x19\n\x15\x41UDIO_ENCODING_AMR_WB\x10\x05\x12\x1b\n\x17\x41UDIO_ENCODING_OGG_OPUS\x10\x06\x12)\n%AUDIO_ENCODING_SPEEX_WITH_HEADER_BYTE\x10\x07*\x83\x01\n\x12\x43omparisonOperator\x12\t\n\x05\x45QUAL\x10\x00\x12\x0b\n\x07GREATER\x10\x01\x12\x14\n\x10GREATER_OR_EQUAL\x10\x02\x12\x11\n\rLESS_OR_EQUAL\x10\x03\x12\x0c\n\x08\x43ONTAINS\x10\x04\x12\x0f\n\x0bSTARTS_WITH\x10\x05\x12\r\n\tENDS_WITH\x10\x06\x32\x8d$\n\x08Sessions\x12\x94\x01\n\x0c\x44\x65tectIntent\x12\x1f.ondewo.nlu.DetectIntentRequest\x1a .ondewo.nlu.DetectIntentResponse\"A\x82\xd3\xe4\x93\x02;\"6/v2/{session=projects/*/agent/sessions/*}:detectIntent:\x01*\x12p\n\x15StreamingDetectIntent\x12(.ondewo.nlu.StreamingDetectIntentRequest\x1a).ondewo.nlu.StreamingDetectIntentResponse(\x01\x30\x01\x12\x81\x01\n\x0cListSessions\x12\x1f.ondewo.nlu.ListSessionsRequest\x1a .ondewo.nlu.ListSessionsResponse\".\x82\xd3\xe4\x93\x02(\x12&/v2/{parent=projects/*/agent}/sessions\x12v\n\nGetSession\x12\x1d.ondewo.nlu.GetSessionRequest\x1a\x13.ondewo.nlu.Session\"4\x82\xd3\xe4\x93\x02.\x12,/v2/{session_id=projects/*/agent/sessions/*}\x12y\n\rCreateSession\x12 .ondewo.nlu.CreateSessionRequest\x1a\x13.ondewo.nlu.Session\"1\x82\xd3\xe4\x93\x02+\"&/v2/{parent=projects/*/agent}/sessions:\x01*\x12\x96\x01\n\x10TrackSessionStep\x12#.ondewo.nlu.TrackSessionStepRequest\x1a\x13.ondewo.nlu.Session\"H\x82\xd3\xe4\x93\x02\x42\"=/v2/{session_id=projects/*/agent/sessions/*}:trackSessionStep:\x01*\x12\x7f\n\rDeleteSession\x12 .ondewo.nlu.DeleteSessionRequest\x1a\x16.google.protobuf.Empty\"4\x82\xd3\xe4\x93\x02.*,/v2/{session_id=projects/*/agent/sessions/*}\x12\x9d\x01\n\x11ListSessionLabels\x12$.ondewo.nlu.ListSessionLabelsRequest\x1a%.ondewo.nlu.ListSessionLabelsResponse\";\x82\xd3\xe4\x93\x02\x35\x12\x33/v2/{session_id=projects/*/agent/sessions/*}/labels\x12\xb1\x01\n\x1eListSessionLabelsOfAllSessions\x12\x31.ondewo.nlu.ListSessionLabelsOfAllSessionsRequest\x1a%.ondewo.nlu.ListSessionLabelsResponse\"5\x82\xd3\xe4\x93\x02/\x12-/v2/{parent=projects/*/agent}/sessions/labels\x12\xb9\x01\n\x1eListLanguageCodesOfAllSessions\x12\x31.ondewo.nlu.ListLanguageCodesOfAllSessionsRequest\x1a%.ondewo.nlu.ListLanguageCodesResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/v2/{parent=projects/*/agent}/sessions/language_codes\x12\xbd\x01\n\x1fListMatchedIntentsOfAllSessions\x12\x32.ondewo.nlu.ListMatchedIntentsOfAllSessionsRequest\x1a&.ondewo.nlu.ListMatchedIntentsResponse\">\x82\xd3\xe4\x93\x02\x38\x12\x36/v2/{parent=projects/*/agent}/sessions/matched_intents\x12\xce\x01\n#ListMatchedEntityTypesOfAllSessions\x12\x36.ondewo.nlu.ListMatchedEntityTypesOfAllSessionsRequest\x1a*.ondewo.nlu.ListMatchedEntityTypesResponse\"C\x82\xd3\xe4\x93\x02=\x12;/v2/{parent=projects/*/agent}/sessions/matched_entity_types\x12\xa1\x01\n\x18ListUserIdsOfAllSessions\x12+.ondewo.nlu.ListUserIdsOfAllSessionsRequest\x1a\x1f.ondewo.nlu.ListUserIdsResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//v2/{parent=projects/*/agent}/sessions/user_ids\x12\xca\x01\n\"ListIdentifiedUserIdsOfAllSessions\x12\x35.ondewo.nlu.ListIdentifiedUserIdsOfAllSessionsRequest\x1a).ondewo.nlu.ListIdentifiedUserIdsResponse\"B\x82\xd3\xe4\x93\x02<\x12:/v2/{parent=projects/*/agent}/sessions/identified_user_ids\x12\x94\x01\n\x15ListTagsOfAllSessions\x12(.ondewo.nlu.ListTagsOfAllSessionsRequest\x1a\x1c.ondewo.nlu.ListTagsResponse\"3\x82\xd3\xe4\x93\x02-\x12+/v2/{parent=projects/*/agent}/sessions/tags\x12\xb9\x01\n\x1eListInputContextsOfAllSessions\x12\x31.ondewo.nlu.ListInputContextsOfAllSessionsRequest\x1a%.ondewo.nlu.ListInputContextsResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/v2/{parent=projects/*/agent}/sessions/input_contexts\x12\xbd\x01\n\x1fListOutputContextsOfAllSessions\x12\x32.ondewo.nlu.ListOutputContextsOfAllSessionsRequest\x1a&.ondewo.nlu.ListOutputContextsResponse\">\x82\xd3\xe4\x93\x02\x38\x12\x36/v2/{parent=projects/*/agent}/sessions/output_contexts\x12\xa8\x01\n\x1aListPlatformsOfAllSessions\x12-.ondewo.nlu.ListPlatformsOfAllSessionsRequest\x1a!.ondewo.nlu.ListPlatformsResponse\"8\x82\xd3\xe4\x93\x02\x32\x12\x30/v2/{parent=projects/*/agent}/sessions/platforms\x12\xad\x01\n\x1bListAccountIdsOfAllSessions\x12..ondewo.nlu.ListAccountIdsOfAllSessionsRequest\x1a\".ondewo.nlu.ListAccountIdsResponse\":\x82\xd3\xe4\x93\x02\x34\x12\x32/v2/{parent=projects/*/agent}/sessions/account_ids\x12\xb1\x01\n\x1cListPropertyIdsOfAllSessions\x12/.ondewo.nlu.ListPropertyIdsOfAllSessionsRequest\x1a#.ondewo.nlu.ListPropertyIdsResponse\";\x82\xd3\xe4\x93\x02\x35\x12\x33/v2/{parent=projects/*/agent}/sessions/property_ids\x12\xb9\x01\n\x1eListDatastreamIdsOfAllSessions\x12\x31.ondewo.nlu.ListDatastreamIdsOfAllSessionsRequest\x1a%.ondewo.nlu.ListDatastreamIdsResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/v2/{parent=projects/*/agent}/sessions/datastream_ids\x12\xa9\x01\n\x1aListOriginIdsOfAllSessions\x12-.ondewo.nlu.ListOriginIdsOfAllSessionsRequest\x1a!.ondewo.nlu.ListOriginIdsResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v2/{parent=projects/*/agent}/sessions/origin_ids\x12\x90\x01\n\x10\x41\x64\x64SessionLabels\x12#.ondewo.nlu.AddSessionLabelsRequest\x1a\x13.ondewo.nlu.Session\"B\x82\xd3\xe4\x93\x02<\"7/v2/{session_id=projects/*/agent/sessions/*}/labels:add:\x01*\x12\x99\x01\n\x13\x44\x65leteSessionLabels\x12&.ondewo.nlu.DeleteSessionLabelsRequest\x1a\x13.ondewo.nlu.Session\"E\x82\xd3\xe4\x93\x02?\":/v2/{session_id=projects/*/agent/sessions/*}/labels:delete:\x01*\x12\xa1\x01\n\x12ListSessionReviews\x12%.ondewo.nlu.ListSessionReviewsRequest\x1a&.ondewo.nlu.ListSessionReviewsResponse\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/v2/{session_id=projects/*/agent/sessions/*}/reviews\x12\x99\x01\n\x10GetSessionReview\x12#.ondewo.nlu.GetSessionReviewRequest\x1a\x19.ondewo.nlu.SessionReview\"E\x82\xd3\xe4\x93\x02?\x12=/v2/{session_review_id=projects/*/agent/sessions/*/reviews/*}\x12\xb3\x01\n\x16GetLatestSessionReview\x12).ondewo.nlu.GetLatestSessionReviewRequest\x1a\x19.ondewo.nlu.SessionReview\"S\x82\xd3\xe4\x93\x02M\x12K/v2/{session_id=projects/*/agent/sessions/*}/reviews:getLatestSessionReview\x12\xa5\x01\n\x13\x43reateSessionReview\x12&.ondewo.nlu.CreateSessionReviewRequest\x1a\x19.ondewo.nlu.SessionReview\"K\x82\xd3\xe4\x93\x02\x45\"@/v2/{session_id=projects/*/agent/sessions/*}:createSessionReview:\x01*B\x9b\x01\n\x1e\x63om.google.cloud.dialogflow.v2B\x0cSessionProtoP\x01ZDgoogle.golang.org/genproto/googleapis/cloud/dialogflow/v2;dialogflow\xf8\x01\x01\xa2\x02\x02\x44\x46\xaa\x02\x1aGoogle.Cloud.Dialogflow.V2b\x06proto3')
 
 _AUDIOENCODING = DESCRIPTOR.enum_types_by_name['AudioEncoding']
 AudioEncoding = enum_type_wrapper.EnumTypeWrapper(_AUDIOENCODING)
 _COMPARISONOPERATOR = DESCRIPTOR.enum_types_by_name['ComparisonOperator']
 ComparisonOperator = enum_type_wrapper.EnumTypeWrapper(_COMPARISONOPERATOR)
 AUDIO_ENCODING_UNSPECIFIED = 0
 AUDIO_ENCODING_LINEAR_16 = 1
@@ -602,144 +603,144 @@
   _SESSIONS.methods_by_name['ListSessionReviews']._serialized_options = b'\202\323\344\223\0026\0224/v2/{session_id=projects/*/agent/sessions/*}/reviews'
   _SESSIONS.methods_by_name['GetSessionReview']._options = None
   _SESSIONS.methods_by_name['GetSessionReview']._serialized_options = b'\202\323\344\223\002?\022=/v2/{session_review_id=projects/*/agent/sessions/*/reviews/*}'
   _SESSIONS.methods_by_name['GetLatestSessionReview']._options = None
   _SESSIONS.methods_by_name['GetLatestSessionReview']._serialized_options = b'\202\323\344\223\002M\022K/v2/{session_id=projects/*/agent/sessions/*}/reviews:getLatestSessionReview'
   _SESSIONS.methods_by_name['CreateSessionReview']._options = None
   _SESSIONS.methods_by_name['CreateSessionReview']._serialized_options = b'\202\323\344\223\002E\"@/v2/{session_id=projects/*/agent/sessions/*}:createSessionReview:\001*'
-  _AUDIOENCODING._serialized_start=10459
-  _AUDIOENCODING._serialized_end=10710
-  _COMPARISONOPERATOR._serialized_start=10713
-  _COMPARISONOPERATOR._serialized_end=10844
-  _DETECTINTENTREQUEST._serialized_start=296
-  _DETECTINTENTREQUEST._serialized_end=451
-  _DETECTINTENTRESPONSE._serialized_start=454
-  _DETECTINTENTRESPONSE._serialized_end=588
-  _QUERYPARAMETERS._serialized_start=591
-  _QUERYPARAMETERS._serialized_end=958
-  _QUERYINPUT._serialized_start=961
-  _QUERYINPUT._serialized_end=1116
-  _QUERYRESULT._serialized_start=1119
-  _QUERYRESULT._serialized_end=1668
-  _STREAMINGDETECTINTENTREQUEST._serialized_start=1671
-  _STREAMINGDETECTINTENTREQUEST._serialized_end=1861
-  _STREAMINGDETECTINTENTRESPONSE._serialized_start=1864
-  _STREAMINGDETECTINTENTRESPONSE._serialized_end=2075
-  _STREAMINGRECOGNITIONRESULT._serialized_start=2078
-  _STREAMINGRECOGNITIONRESULT._serialized_end=2328
-  _STREAMINGRECOGNITIONRESULT_MESSAGETYPE._serialized_start=2240
-  _STREAMINGRECOGNITIONRESULT_MESSAGETYPE._serialized_end=2328
-  _INPUTAUDIOCONFIG._serialized_start=2331
-  _INPUTAUDIOCONFIG._serialized_end=2472
-  _TEXTINPUT._serialized_start=2474
-  _TEXTINPUT._serialized_end=2522
-  _EVENTINPUT._serialized_start=2524
-  _EVENTINPUT._serialized_end=2618
-  _SESSION._serialized_start=2621
-  _SESSION._serialized_end=2801
-  _SESSION_VIEW._serialized_start=2741
-  _SESSION_VIEW._serialized_end=2801
-  _SESSIONSTEP._serialized_start=2804
-  _SESSIONSTEP._serialized_end=3000
-  _TRACKSESSIONSTEPREQUEST._serialized_start=3003
-  _TRACKSESSIONSTEPREQUEST._serialized_end=3143
-  _LISTSESSIONSREQUEST._serialized_start=3146
-  _LISTSESSIONSREQUEST._serialized_end=3350
-  _CONTEXTFILTER._serialized_start=3352
-  _CONTEXTFILTER._serialized_end=3467
-  _SESSIONFILTER._serialized_start=3470
-  _SESSIONFILTER._serialized_end=5219
-  _SESSIONINFO._serialized_start=5222
-  _SESSIONINFO._serialized_end=6364
-  _SESSIONINFO_CONTEXTSTEPS._serialized_start=6311
-  _SESSIONINFO_CONTEXTSTEPS._serialized_end=6364
-  _LISTSESSIONSRESPONSE._serialized_start=6366
-  _LISTSESSIONSRESPONSE._serialized_end=6452
-  _GETSESSIONREQUEST._serialized_start=6455
-  _GETSESSIONREQUEST._serialized_end=6590
-  _CREATESESSIONREQUEST._serialized_start=6592
-  _CREATESESSIONREQUEST._serialized_end=6707
-  _DELETESESSIONREQUEST._serialized_start=6709
-  _DELETESESSIONREQUEST._serialized_end=6751
-  _CREATESESSIONREVIEWREQUEST._serialized_start=6754
-  _CREATESESSIONREVIEWREQUEST._serialized_end=6940
-  _SESSIONREVIEW._serialized_start=6943
-  _SESSIONREVIEW._serialized_end=7095
-  _SESSIONREVIEW_VIEW._serialized_start=2741
-  _SESSIONREVIEW_VIEW._serialized_end=2801
-  _SESSIONREVIEWSTEP._serialized_start=7098
-  _SESSIONREVIEWSTEP._serialized_end=7438
-  _DETECTEDINTENT._serialized_start=7441
-  _DETECTEDINTENT._serialized_end=7617
-  _LISTSESSIONLABELSREQUEST._serialized_start=7619
-  _LISTSESSIONLABELSREQUEST._serialized_end=7665
-  _LISTSESSIONLABELSOFALLSESSIONSREQUEST._serialized_start=7667
-  _LISTSESSIONLABELSOFALLSESSIONSREQUEST._serialized_end=7773
-  _LISTSESSIONLABELSRESPONSE._serialized_start=7775
-  _LISTSESSIONLABELSRESPONSE._serialized_end=7818
-  _LISTLANGUAGECODESOFALLSESSIONSREQUEST._serialized_start=7820
-  _LISTLANGUAGECODESOFALLSESSIONSREQUEST._serialized_end=7926
-  _LISTLANGUAGECODESRESPONSE._serialized_start=7928
-  _LISTLANGUAGECODESRESPONSE._serialized_end=7979
-  _LISTMATCHEDINTENTSOFALLSESSIONSREQUEST._serialized_start=7981
-  _LISTMATCHEDINTENTSOFALLSESSIONSREQUEST._serialized_end=8088
-  _LISTMATCHEDINTENTSRESPONSE._serialized_start=8090
-  _LISTMATCHEDINTENTSRESPONSE._serialized_end=8143
-  _LISTMATCHEDENTITYTYPESOFALLSESSIONSREQUEST._serialized_start=8145
-  _LISTMATCHEDENTITYTYPESOFALLSESSIONSREQUEST._serialized_end=8256
-  _LISTMATCHEDENTITYTYPESRESPONSE._serialized_start=8258
-  _LISTMATCHEDENTITYTYPESRESPONSE._serialized_end=8320
-  _LISTUSERIDSOFALLSESSIONSREQUEST._serialized_start=8322
-  _LISTUSERIDSOFALLSESSIONSREQUEST._serialized_end=8422
-  _LISTUSERIDSRESPONSE._serialized_start=8424
-  _LISTUSERIDSRESPONSE._serialized_end=8463
-  _LISTIDENTIFIEDUSERIDSOFALLSESSIONSREQUEST._serialized_start=8465
-  _LISTIDENTIFIEDUSERIDSOFALLSESSIONSREQUEST._serialized_end=8575
-  _LISTIDENTIFIEDUSERIDSRESPONSE._serialized_start=8577
-  _LISTIDENTIFIEDUSERIDSRESPONSE._serialized_end=8637
-  _LISTTAGSOFALLSESSIONSREQUEST._serialized_start=8639
-  _LISTTAGSOFALLSESSIONSREQUEST._serialized_end=8736
-  _LISTTAGSRESPONSE._serialized_start=8738
-  _LISTTAGSRESPONSE._serialized_end=8770
-  _LISTINPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_start=8772
-  _LISTINPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_end=8878
-  _LISTINPUTCONTEXTSRESPONSE._serialized_start=8880
-  _LISTINPUTCONTEXTSRESPONSE._serialized_end=8931
-  _LISTOUTPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_start=8933
-  _LISTOUTPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_end=9040
-  _LISTOUTPUTCONTEXTSRESPONSE._serialized_start=9042
-  _LISTOUTPUTCONTEXTSRESPONSE._serialized_end=9095
-  _LISTPLATFORMSOFALLSESSIONSREQUEST._serialized_start=9097
-  _LISTPLATFORMSOFALLSESSIONSREQUEST._serialized_end=9199
-  _LISTPLATFORMSRESPONSE._serialized_start=9201
-  _LISTPLATFORMSRESPONSE._serialized_end=9243
-  _LISTACCOUNTIDSOFALLSESSIONSREQUEST._serialized_start=9245
-  _LISTACCOUNTIDSOFALLSESSIONSREQUEST._serialized_end=9348
-  _LISTACCOUNTIDSRESPONSE._serialized_start=9350
-  _LISTACCOUNTIDSRESPONSE._serialized_end=9395
-  _LISTPROPERTYIDSOFALLSESSIONSREQUEST._serialized_start=9397
-  _LISTPROPERTYIDSOFALLSESSIONSREQUEST._serialized_end=9501
-  _LISTPROPERTYIDSRESPONSE._serialized_start=9503
-  _LISTPROPERTYIDSRESPONSE._serialized_end=9550
-  _LISTDATASTREAMIDSOFALLSESSIONSREQUEST._serialized_start=9552
-  _LISTDATASTREAMIDSOFALLSESSIONSREQUEST._serialized_end=9658
-  _LISTDATASTREAMIDSRESPONSE._serialized_start=9660
-  _LISTDATASTREAMIDSRESPONSE._serialized_end=9711
-  _LISTORIGINIDSOFALLSESSIONSREQUEST._serialized_start=9713
-  _LISTORIGINIDSOFALLSESSIONSREQUEST._serialized_end=9815
-  _LISTORIGINIDSRESPONSE._serialized_start=9817
-  _LISTORIGINIDSRESPONSE._serialized_end=9860
-  _ADDSESSIONLABELSREQUEST._serialized_start=9862
-  _ADDSESSIONLABELSREQUEST._serialized_end=9923
-  _DELETESESSIONLABELSREQUEST._serialized_start=9925
-  _DELETESESSIONLABELSREQUEST._serialized_end=9989
-  _LISTSESSIONREVIEWSREQUEST._serialized_start=9992
-  _LISTSESSIONREVIEWSREQUEST._serialized_end=10120
-  _LISTSESSIONREVIEWSRESPONSE._serialized_start=10122
-  _LISTSESSIONREVIEWSRESPONSE._serialized_end=10227
-  _GETSESSIONREVIEWREQUEST._serialized_start=10229
-  _GETSESSIONREVIEWREQUEST._serialized_end=10342
-  _GETLATESTSESSIONREVIEWREQUEST._serialized_start=10344
-  _GETLATESTSESSIONREVIEWREQUEST._serialized_end=10456
-  _SESSIONS._serialized_start=10847
-  _SESSIONS._serialized_end=15468
+  _AUDIOENCODING._serialized_start=10586
+  _AUDIOENCODING._serialized_end=10837
+  _COMPARISONOPERATOR._serialized_start=10840
+  _COMPARISONOPERATOR._serialized_end=10971
+  _DETECTINTENTREQUEST._serialized_start=329
+  _DETECTINTENTREQUEST._serialized_end=484
+  _DETECTINTENTRESPONSE._serialized_start=487
+  _DETECTINTENTRESPONSE._serialized_end=621
+  _QUERYPARAMETERS._serialized_start=624
+  _QUERYPARAMETERS._serialized_end=991
+  _QUERYINPUT._serialized_start=994
+  _QUERYINPUT._serialized_end=1149
+  _QUERYRESULT._serialized_start=1152
+  _QUERYRESULT._serialized_end=1701
+  _STREAMINGDETECTINTENTREQUEST._serialized_start=1704
+  _STREAMINGDETECTINTENTREQUEST._serialized_end=1894
+  _STREAMINGDETECTINTENTRESPONSE._serialized_start=1897
+  _STREAMINGDETECTINTENTRESPONSE._serialized_end=2108
+  _STREAMINGRECOGNITIONRESULT._serialized_start=2111
+  _STREAMINGRECOGNITIONRESULT._serialized_end=2361
+  _STREAMINGRECOGNITIONRESULT_MESSAGETYPE._serialized_start=2273
+  _STREAMINGRECOGNITIONRESULT_MESSAGETYPE._serialized_end=2361
+  _INPUTAUDIOCONFIG._serialized_start=2364
+  _INPUTAUDIOCONFIG._serialized_end=2505
+  _TEXTINPUT._serialized_start=2507
+  _TEXTINPUT._serialized_end=2555
+  _EVENTINPUT._serialized_start=2557
+  _EVENTINPUT._serialized_end=2651
+  _SESSION._serialized_start=2654
+  _SESSION._serialized_end=2834
+  _SESSION_VIEW._serialized_start=2774
+  _SESSION_VIEW._serialized_end=2834
+  _SESSIONSTEP._serialized_start=2837
+  _SESSIONSTEP._serialized_end=3080
+  _TRACKSESSIONSTEPREQUEST._serialized_start=3083
+  _TRACKSESSIONSTEPREQUEST._serialized_end=3223
+  _LISTSESSIONSREQUEST._serialized_start=3226
+  _LISTSESSIONSREQUEST._serialized_end=3430
+  _CONTEXTFILTER._serialized_start=3432
+  _CONTEXTFILTER._serialized_end=3547
+  _SESSIONFILTER._serialized_start=3550
+  _SESSIONFILTER._serialized_end=5299
+  _SESSIONINFO._serialized_start=5302
+  _SESSIONINFO._serialized_end=6444
+  _SESSIONINFO_CONTEXTSTEPS._serialized_start=6391
+  _SESSIONINFO_CONTEXTSTEPS._serialized_end=6444
+  _LISTSESSIONSRESPONSE._serialized_start=6446
+  _LISTSESSIONSRESPONSE._serialized_end=6532
+  _GETSESSIONREQUEST._serialized_start=6535
+  _GETSESSIONREQUEST._serialized_end=6670
+  _CREATESESSIONREQUEST._serialized_start=6672
+  _CREATESESSIONREQUEST._serialized_end=6787
+  _DELETESESSIONREQUEST._serialized_start=6789
+  _DELETESESSIONREQUEST._serialized_end=6831
+  _CREATESESSIONREVIEWREQUEST._serialized_start=6834
+  _CREATESESSIONREVIEWREQUEST._serialized_end=7020
+  _SESSIONREVIEW._serialized_start=7023
+  _SESSIONREVIEW._serialized_end=7175
+  _SESSIONREVIEW_VIEW._serialized_start=2774
+  _SESSIONREVIEW_VIEW._serialized_end=2834
+  _SESSIONREVIEWSTEP._serialized_start=7178
+  _SESSIONREVIEWSTEP._serialized_end=7565
+  _DETECTEDINTENT._serialized_start=7568
+  _DETECTEDINTENT._serialized_end=7744
+  _LISTSESSIONLABELSREQUEST._serialized_start=7746
+  _LISTSESSIONLABELSREQUEST._serialized_end=7792
+  _LISTSESSIONLABELSOFALLSESSIONSREQUEST._serialized_start=7794
+  _LISTSESSIONLABELSOFALLSESSIONSREQUEST._serialized_end=7900
+  _LISTSESSIONLABELSRESPONSE._serialized_start=7902
+  _LISTSESSIONLABELSRESPONSE._serialized_end=7945
+  _LISTLANGUAGECODESOFALLSESSIONSREQUEST._serialized_start=7947
+  _LISTLANGUAGECODESOFALLSESSIONSREQUEST._serialized_end=8053
+  _LISTLANGUAGECODESRESPONSE._serialized_start=8055
+  _LISTLANGUAGECODESRESPONSE._serialized_end=8106
+  _LISTMATCHEDINTENTSOFALLSESSIONSREQUEST._serialized_start=8108
+  _LISTMATCHEDINTENTSOFALLSESSIONSREQUEST._serialized_end=8215
+  _LISTMATCHEDINTENTSRESPONSE._serialized_start=8217
+  _LISTMATCHEDINTENTSRESPONSE._serialized_end=8270
+  _LISTMATCHEDENTITYTYPESOFALLSESSIONSREQUEST._serialized_start=8272
+  _LISTMATCHEDENTITYTYPESOFALLSESSIONSREQUEST._serialized_end=8383
+  _LISTMATCHEDENTITYTYPESRESPONSE._serialized_start=8385
+  _LISTMATCHEDENTITYTYPESRESPONSE._serialized_end=8447
+  _LISTUSERIDSOFALLSESSIONSREQUEST._serialized_start=8449
+  _LISTUSERIDSOFALLSESSIONSREQUEST._serialized_end=8549
+  _LISTUSERIDSRESPONSE._serialized_start=8551
+  _LISTUSERIDSRESPONSE._serialized_end=8590
+  _LISTIDENTIFIEDUSERIDSOFALLSESSIONSREQUEST._serialized_start=8592
+  _LISTIDENTIFIEDUSERIDSOFALLSESSIONSREQUEST._serialized_end=8702
+  _LISTIDENTIFIEDUSERIDSRESPONSE._serialized_start=8704
+  _LISTIDENTIFIEDUSERIDSRESPONSE._serialized_end=8764
+  _LISTTAGSOFALLSESSIONSREQUEST._serialized_start=8766
+  _LISTTAGSOFALLSESSIONSREQUEST._serialized_end=8863
+  _LISTTAGSRESPONSE._serialized_start=8865
+  _LISTTAGSRESPONSE._serialized_end=8897
+  _LISTINPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_start=8899
+  _LISTINPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_end=9005
+  _LISTINPUTCONTEXTSRESPONSE._serialized_start=9007
+  _LISTINPUTCONTEXTSRESPONSE._serialized_end=9058
+  _LISTOUTPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_start=9060
+  _LISTOUTPUTCONTEXTSOFALLSESSIONSREQUEST._serialized_end=9167
+  _LISTOUTPUTCONTEXTSRESPONSE._serialized_start=9169
+  _LISTOUTPUTCONTEXTSRESPONSE._serialized_end=9222
+  _LISTPLATFORMSOFALLSESSIONSREQUEST._serialized_start=9224
+  _LISTPLATFORMSOFALLSESSIONSREQUEST._serialized_end=9326
+  _LISTPLATFORMSRESPONSE._serialized_start=9328
+  _LISTPLATFORMSRESPONSE._serialized_end=9370
+  _LISTACCOUNTIDSOFALLSESSIONSREQUEST._serialized_start=9372
+  _LISTACCOUNTIDSOFALLSESSIONSREQUEST._serialized_end=9475
+  _LISTACCOUNTIDSRESPONSE._serialized_start=9477
+  _LISTACCOUNTIDSRESPONSE._serialized_end=9522
+  _LISTPROPERTYIDSOFALLSESSIONSREQUEST._serialized_start=9524
+  _LISTPROPERTYIDSOFALLSESSIONSREQUEST._serialized_end=9628
+  _LISTPROPERTYIDSRESPONSE._serialized_start=9630
+  _LISTPROPERTYIDSRESPONSE._serialized_end=9677
+  _LISTDATASTREAMIDSOFALLSESSIONSREQUEST._serialized_start=9679
+  _LISTDATASTREAMIDSOFALLSESSIONSREQUEST._serialized_end=9785
+  _LISTDATASTREAMIDSRESPONSE._serialized_start=9787
+  _LISTDATASTREAMIDSRESPONSE._serialized_end=9838
+  _LISTORIGINIDSOFALLSESSIONSREQUEST._serialized_start=9840
+  _LISTORIGINIDSOFALLSESSIONSREQUEST._serialized_end=9942
+  _LISTORIGINIDSRESPONSE._serialized_start=9944
+  _LISTORIGINIDSRESPONSE._serialized_end=9987
+  _ADDSESSIONLABELSREQUEST._serialized_start=9989
+  _ADDSESSIONLABELSREQUEST._serialized_end=10050
+  _DELETESESSIONLABELSREQUEST._serialized_start=10052
+  _DELETESESSIONLABELSREQUEST._serialized_end=10116
+  _LISTSESSIONREVIEWSREQUEST._serialized_start=10119
+  _LISTSESSIONREVIEWSREQUEST._serialized_end=10247
+  _LISTSESSIONREVIEWSRESPONSE._serialized_start=10249
+  _LISTSESSIONREVIEWSRESPONSE._serialized_end=10354
+  _GETSESSIONREVIEWREQUEST._serialized_start=10356
+  _GETSESSIONREVIEWREQUEST._serialized_end=10469
+  _GETLATESTSESSIONREVIEWREQUEST._serialized_start=10471
+  _GETLATESTSESSIONREVIEWREQUEST._serialized_end=10583
+  _SESSIONS._serialized_start=10974
+  _SESSIONS._serialized_end=15595
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/session_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/session_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.field_mask_pb2
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import google.protobuf.struct_pb2
+import google.protobuf.timestamp_pb2
 import google.rpc.status_pb2
 import google.type.latlng_pb2
 import ondewo.nlu.context_pb2
 import ondewo.nlu.entity_type_pb2
 import ondewo.nlu.intent_pb2
 import typing
 import typing_extensions
@@ -912,15 +913,17 @@
     """
 
     @property
     def session_steps(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SessionStep]:
         """The list of all the steps of the session"""
         pass
     @property
-    def session_info(self) -> global___SessionInfo: ...
+    def session_info(self) -> global___SessionInfo:
+        """session information"""
+        pass
     def __init__(self,
         *,
         name: typing.Text = ...,
         session_steps: typing.Optional[typing.Iterable[global___SessionStep]] = ...,
         session_info: typing.Optional[global___SessionInfo] = ...,
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["session_info",b"session_info"]) -> builtins.bool: ...
@@ -930,14 +933,15 @@
 class SessionStep(google.protobuf.message.Message):
     """SessionStep is a single user interaction as part of a session"""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     NAME_FIELD_NUMBER: builtins.int
     DETECT_INTENT_REQUEST_FIELD_NUMBER: builtins.int
     DETECT_INTENT_RESPONSE_FIELD_NUMBER: builtins.int
     CONTEXTS_FIELD_NUMBER: builtins.int
+    TIMESTAMP_FIELD_NUMBER: builtins.int
     name: typing.Text
     """The unique identifier for the given review
     Format: <pre><code>projects/&lt;project_uuid&gt;/agent/sessions/&lt;session_uuid&gt;/steps/&lt;session_step_uuid&gt;</code></pre>
     """
 
     @property
     def detect_intent_request(self) -> global___DetectIntentRequest:
@@ -947,23 +951,28 @@
     def detect_intent_response(self) -> global___DetectIntentResponse:
         """The detect intent response  of the session step"""
         pass
     @property
     def contexts(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[ondewo.nlu.context_pb2.Context]:
         """The contexts which were active at the beginning of this step"""
         pass
+    @property
+    def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
+        """Timestamp of session step"""
+        pass
     def __init__(self,
         *,
         name: typing.Text = ...,
         detect_intent_request: typing.Optional[global___DetectIntentRequest] = ...,
         detect_intent_response: typing.Optional[global___DetectIntentResponse] = ...,
         contexts: typing.Optional[typing.Iterable[ondewo.nlu.context_pb2.Context]] = ...,
+        timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["detect_intent_request",b"detect_intent_request","detect_intent_response",b"detect_intent_response"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["contexts",b"contexts","detect_intent_request",b"detect_intent_request","detect_intent_response",b"detect_intent_response","name",b"name"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["detect_intent_request",b"detect_intent_request","detect_intent_response",b"detect_intent_response","timestamp",b"timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["contexts",b"contexts","detect_intent_request",b"detect_intent_request","detect_intent_response",b"detect_intent_response","name",b"name","timestamp",b"timestamp"]) -> None: ...
 global___SessionStep = SessionStep
 
 class TrackSessionStepRequest(google.protobuf.message.Message):
     """TrackSessionStepRequest stores a session step into the session"""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     SESSION_ID_FIELD_NUMBER: builtins.int
     SESSION_STEP_FIELD_NUMBER: builtins.int
@@ -1781,14 +1790,15 @@
     ANNOTATED_USERSAYS_FIELD_NUMBER: builtins.int
     LANGUAGE_CODE_FIELD_NUMBER: builtins.int
     DETECTED_INTENTS_FIELD_NUMBER: builtins.int
     CONTEXTS_FIELD_NUMBER: builtins.int
     CONTEXTS_OUT_FIELD_NUMBER: builtins.int
     QUERY_TEXT_ORIGINAL_FIELD_NUMBER: builtins.int
     PLATFORMS_FIELD_NUMBER: builtins.int
+    TIMESTAMP_FIELD_NUMBER: builtins.int
     name: typing.Text
     """The unique identifier for the given review step
     Format: <pre><code>projects/&lt;project_uuid&gt;/agent/sessions/&lt;session_uuid&gt;/reviews/&lt;review_uuid&gt;/sessionreviewsteps/&lt;session_review_step_uuid&gt;</code></pre>
     """
 
     @property
     def annotated_usersays(self) -> ondewo.nlu.intent_pb2.Intent.TrainingPhrase:
@@ -1816,27 +1826,32 @@
     query_text_original: typing.Text
     """User input without any pre-processing applied"""
 
     @property
     def platforms(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[ondewo.nlu.intent_pb2.Intent.Message.Platform.ValueType]:
         """Messages for each of the Intent.Message.Platform were sent to the user"""
         pass
+    @property
+    def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
+        """Timestamp of session review step"""
+        pass
     def __init__(self,
         *,
         name: typing.Text = ...,
         annotated_usersays: typing.Optional[ondewo.nlu.intent_pb2.Intent.TrainingPhrase] = ...,
         language_code: typing.Text = ...,
         detected_intents: typing.Optional[typing.Iterable[global___DetectedIntent]] = ...,
         contexts: typing.Optional[typing.Iterable[ondewo.nlu.context_pb2.Context]] = ...,
         contexts_out: typing.Optional[typing.Iterable[ondewo.nlu.context_pb2.Context]] = ...,
         query_text_original: typing.Text = ...,
         platforms: typing.Optional[typing.Iterable[ondewo.nlu.intent_pb2.Intent.Message.Platform.ValueType]] = ...,
+        timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["annotated_usersays",b"annotated_usersays"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["annotated_usersays",b"annotated_usersays","contexts",b"contexts","contexts_out",b"contexts_out","detected_intents",b"detected_intents","language_code",b"language_code","name",b"name","platforms",b"platforms","query_text_original",b"query_text_original"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["annotated_usersays",b"annotated_usersays","timestamp",b"timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["annotated_usersays",b"annotated_usersays","contexts",b"contexts","contexts_out",b"contexts_out","detected_intents",b"detected_intents","language_code",b"language_code","name",b"name","platforms",b"platforms","query_text_original",b"query_text_original","timestamp",b"timestamp"]) -> None: ...
 global___SessionReviewStep = SessionReviewStep
 
 class DetectedIntent(google.protobuf.message.Message):
     """This message contains a detected intent"""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     INTENT_FIELD_NUMBER: builtins.int
     SCORE_FIELD_NUMBER: builtins.int
```

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/session_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/user_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/user_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/user_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/user_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/utility_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/utility_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/utility_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/utility_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/utility_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/utility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/utils/login.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/utils/login.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/webhook_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/webhook_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/webhook_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/nlu/webhook_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/nlu/webhook_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/nlu/webhook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/qa/client.py` & `ondewo-nlu-client-4.7.0/ondewo/qa/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/qa/client_config.py` & `ondewo-nlu-client-4.7.0/ondewo/qa/client_config.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/qa/core/services_container.py` & `ondewo-nlu-client-4.7.0/ondewo/qa/core/services_container.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/qa/core/services_interface.py` & `ondewo-nlu-client-4.7.0/ondewo/qa/core/services_interface.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/qa/qa_pb2.py` & `ondewo-nlu-client-4.7.0/ondewo/qa/qa_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/qa/qa_pb2.pyi` & `ondewo-nlu-client-4.7.0/ondewo/qa/qa_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/qa/qa_pb2_grpc.py` & `ondewo-nlu-client-4.7.0/ondewo/qa/qa_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo/qa/services/qa.py` & `ondewo-nlu-client-4.7.0/ondewo/qa/services/qa.py`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/ondewo_nlu_client.egg-info/PKG-INFO` & `ondewo-nlu-client-4.7.0/ondewo_nlu_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-nlu-client
-Version: 4.6.0
+Version: 4.7.0
 Summary: This library facilitates the interaction between a user and his/her CAI server.
 Home-page: https://github.com/ondewo/ondewo-nlu-client-python
 Author: Ondewo GmbH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-nlu-client Version: 4.6.0 Summary: This
+Metadata-Version: 2.1 Name: ondewo-nlu-client Version: 4.7.0 Summary: This
 library facilitates the interaction between a user and his/her CAI server.
 Home-page: https://github.com/ondewo/ondewo-nlu-client-python Author: Ondewo
 GmbH Author-email: office@ondewo.com License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8 Classifier: Operating System
 :: OS Independent Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-nlu-client-4.6.0/ondewo_nlu_client.egg-info/SOURCES.txt` & `ondewo-nlu-client-4.7.0/ondewo_nlu_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ondewo-nlu-client-4.6.0/setup.py` & `ondewo-nlu-client-4.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open('requirements.txt') as f:
     requires = f.read().splitlines()
 
 setuptools.setup(
     name='ondewo-nlu-client',
-    version='4.6.0',
+    version='4.7.0',
     author='Ondewo GmbH',
     author_email='office@ondewo.com',
     description='This library facilitates the interaction between a user and his/her CAI server.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ondewo/ondewo-nlu-client-python',
     packages=[
```

