# Comparing `tmp/polarismesh_specification-1.3.0a6.tar.gz` & `tmp/polarismesh_specification-1.3.0a7.tar.gz`

## Comparing `polarismesh_specification-1.3.0a6.tar` & `polarismesh_specification-1.3.0a7.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
--rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
--rw-r--r--   0        0        0    15838 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
--rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
--rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
--rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/__init__.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/__init__.pyi
--rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/code_pb2.py
--rw-r--r--   0        0        0     4864 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/code_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/model_pb2.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/model_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/namespace_pb2.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/__init__.pyi
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/auth_pb2.py
--rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
--rw-r--r--   0        0        0    13092 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
--rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
--rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
--rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
--rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
--rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
--rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
--rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
--rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/.gitignore
--rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/LICENSE.txt
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/README.md
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/pyproject.toml
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
+-rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
+-rw-r--r--   0        0        0    15838 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
+-rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
+-rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
+-rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/__init__.pyi
+-rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/code_pb2.py
+-rw-r--r--   0        0        0     4864 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/code_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/model_pb2.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/namespace_pb2.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/__init__.pyi
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/auth_pb2.py
+-rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
+-rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
+-rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
+-rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
+-rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
+-rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
+-rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
+-rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
+-rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
+-rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/.gitignore
+-rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/LICENSE.txt
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/README.md
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/pyproject.toml
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/PKG-INFO
```

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/code_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/code_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/code_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/model_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/model_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/model_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/namespace_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/namespace_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/auth_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/auth_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/client_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/client_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 from ..service_manage import client_pb2 as client__pb2
 from ..service_manage import service_pb2 as service__pb2
 from ..service_manage import request_pb2 as request__pb2
 from ..service_manage import response_pb2 as response__pb2
 from ..service_manage import heartbeat_pb2 as heartbeat__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rgrpcapi.proto\x12\x02v1\x1a\x0c\x63lient.proto\x1a\rservice.proto\x1a\rrequest.proto\x1a\x0eresponse.proto\x1a\x0fheartbeat.proto2\xd1\x03\n\x0bPolarisGRPC\x12*\n\x0cReportClient\x12\n.v1.Client\x1a\x0c.v1.Response\"\x00\x12\x30\n\x10RegisterInstance\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12\x32\n\x12\x44\x65registerInstance\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12;\n\x08\x44iscover\x12\x13.v1.DiscoverRequest\x1a\x14.v1.DiscoverResponse\"\x00(\x01\x30\x01\x12)\n\tHeartbeat\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12\x30\n\x0e\x42\x61tchHeartbeat\x12\x0e.v1.Heartbeats\x1a\x0c.v1.Response\"\x00\x12J\n\x11\x42\x61tchGetHeartbeat\x12\x18.v1.GetHeartbeatsRequest\x1a\x19.v1.GetHeartbeatsResponse\"\x00\x12J\n\x11\x42\x61tchDelHeartbeat\x12\x18.v1.DelHeartbeatsRequest\x1a\x19.v1.DelHeartbeatsResponse\"\x00\x42\x93\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\x12PolarisGRPCServiceZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rgrpcapi.proto\x12\x02v1\x1a\x0c\x63lient.proto\x1a\rservice.proto\x1a\rrequest.proto\x1a\x0eresponse.proto\x1a\x0fheartbeat.proto2\xe6\x03\n\x0bPolarisGRPC\x12*\n\x0cReportClient\x12\n.v1.Client\x1a\x0c.v1.Response\"\x00\x12\x30\n\x10RegisterInstance\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12\x32\n\x12\x44\x65registerInstance\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12;\n\x08\x44iscover\x12\x13.v1.DiscoverRequest\x1a\x14.v1.DiscoverResponse\"\x00(\x01\x30\x01\x12)\n\tHeartbeat\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12\x45\n\x0e\x42\x61tchHeartbeat\x12\x15.v1.HeartbeatsRequest\x1a\x16.v1.HeartbeatsResponse\"\x00(\x01\x30\x01\x12J\n\x11\x42\x61tchGetHeartbeat\x12\x18.v1.GetHeartbeatsRequest\x1a\x19.v1.GetHeartbeatsResponse\"\x00\x12J\n\x11\x42\x61tchDelHeartbeat\x12\x18.v1.DelHeartbeatsRequest\x1a\x19.v1.DelHeartbeatsResponse\"\x00\x42\x93\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\x12PolarisGRPCServiceZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpcapi_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageB\022PolarisGRPCServiceZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
   _POLARISGRPC._serialized_start=99
-  _POLARISGRPC._serialized_end=564
+  _POLARISGRPC._serialized_end=585
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,18 +39,18 @@
                 response_deserializer=response__pb2.DiscoverResponse.FromString,
                 )
         self.Heartbeat = channel.unary_unary(
                 '/v1.PolarisGRPC/Heartbeat',
                 request_serializer=service__pb2.Instance.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
                 )
-        self.BatchHeartbeat = channel.unary_unary(
+        self.BatchHeartbeat = channel.stream_stream(
                 '/v1.PolarisGRPC/BatchHeartbeat',
-                request_serializer=heartbeat__pb2.Heartbeats.SerializeToString,
-                response_deserializer=response__pb2.Response.FromString,
+                request_serializer=heartbeat__pb2.HeartbeatsRequest.SerializeToString,
+                response_deserializer=heartbeat__pb2.HeartbeatsResponse.FromString,
                 )
         self.BatchGetHeartbeat = channel.unary_unary(
                 '/v1.PolarisGRPC/BatchGetHeartbeat',
                 request_serializer=heartbeat__pb2.GetHeartbeatsRequest.SerializeToString,
                 response_deserializer=heartbeat__pb2.GetHeartbeatsResponse.FromString,
                 )
         self.BatchDelHeartbeat = channel.unary_unary(
@@ -94,15 +94,15 @@
     def Heartbeat(self, request, context):
         """被调方上报心跳
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def BatchHeartbeat(self, request, context):
+    def BatchHeartbeat(self, request_iterator, context):
         """被调方批量上报心跳
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def BatchGetHeartbeat(self, request, context):
@@ -143,18 +143,18 @@
                     response_serializer=response__pb2.DiscoverResponse.SerializeToString,
             ),
             'Heartbeat': grpc.unary_unary_rpc_method_handler(
                     servicer.Heartbeat,
                     request_deserializer=service__pb2.Instance.FromString,
                     response_serializer=response__pb2.Response.SerializeToString,
             ),
-            'BatchHeartbeat': grpc.unary_unary_rpc_method_handler(
+            'BatchHeartbeat': grpc.stream_stream_rpc_method_handler(
                     servicer.BatchHeartbeat,
-                    request_deserializer=heartbeat__pb2.Heartbeats.FromString,
-                    response_serializer=response__pb2.Response.SerializeToString,
+                    request_deserializer=heartbeat__pb2.HeartbeatsRequest.FromString,
+                    response_serializer=heartbeat__pb2.HeartbeatsResponse.SerializeToString,
             ),
             'BatchGetHeartbeat': grpc.unary_unary_rpc_method_handler(
                     servicer.BatchGetHeartbeat,
                     request_deserializer=heartbeat__pb2.GetHeartbeatsRequest.FromString,
                     response_serializer=heartbeat__pb2.GetHeartbeatsResponse.SerializeToString,
             ),
             'BatchDelHeartbeat': grpc.unary_unary_rpc_method_handler(
@@ -254,27 +254,27 @@
         return grpc.experimental.unary_unary(request, target, '/v1.PolarisGRPC/Heartbeat',
             service__pb2.Instance.SerializeToString,
             response__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def BatchHeartbeat(request,
+    def BatchHeartbeat(request_iterator,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/v1.PolarisGRPC/BatchHeartbeat',
-            heartbeat__pb2.Heartbeats.SerializeToString,
-            response__pb2.Response.FromString,
+        return grpc.experimental.stream_stream(request_iterator, target, '/v1.PolarisGRPC/BatchHeartbeat',
+            heartbeat__pb2.HeartbeatsRequest.SerializeToString,
+            heartbeat__pb2.HeartbeatsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def BatchGetHeartbeat(request,
             target,
             options=(),
```

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,28 +10,32 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from ..service_manage import service_pb2 as service__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fheartbeat.proto\x12\x02v1\x1a\rservice.proto\"\xd6\x01\n\x0fHeartbeatRecord\x12\x1f\n\ninstanceId\x18\x01 \x01(\tR\x0binstance_id\x12\x18\n\x07service\x18\x02 \x01(\tR\x07service\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12\x12\n\x04host\x18\x04 \x01(\tR\x04host\x12\x12\n\x04port\x18\x05 \x01(\rR\x04port\x12,\n\x10lastHeartbeatSec\x18\x06 \x01(\x03R\x12last_heartbeat_sec\x12\x14\n\x05\x65xist\x18\x07 \x01(\x08R\x05\x65xist\":\n\nHeartbeats\x12,\n\nheartbeats\x18\x01 \x03(\x0b\x32\x0c.v1.InstanceR\nheartbeats\"9\n\x14GetHeartbeatsRequest\x12!\n\x0binstanceIds\x18\x01 \x03(\tR\x0cinstance_ids\"F\n\x15GetHeartbeatsResponse\x12-\n\x07records\x18\x01 \x03(\x0b\x32\x13.v1.HeartbeatRecordR\x07records\"9\n\x14\x44\x65lHeartbeatsRequest\x12!\n\x0binstanceIds\x18\x01 \x03(\tR\x0cinstance_ids\"3\n\x15\x44\x65lHeartbeatsResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\r\x12\x0c\n\x04info\x18\x02 \x01(\tB\x7f\n7com.tencent.polaris.specification.api.v1.service.manageZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fheartbeat.proto\x12\x02v1\x1a\rservice.proto\"|\n\x0fHeartbeatRecord\x12\x1f\n\ninstanceId\x18\x01 \x01(\tR\x0binstance_id\x12,\n\x10lastHeartbeatSec\x18\x06 \x01(\x03R\x12last_heartbeat_sec\x12\x14\n\x05\x65xist\x18\x07 \x01(\x08R\x05\x65xistJ\x04\x08\x02\x10\x06\"\x94\x01\n\x11InstanceHeartbeat\x12\x1f\n\ninstanceId\x18\x01 \x01(\tR\x0binstance_id\x12\x18\n\x07service\x18\x02 \x01(\tR\x07service\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12\x12\n\x04host\x18\x04 \x01(\tR\x04host\x12\x12\n\x04port\x18\x05 \x01(\rR\x04port\"J\n\x11HeartbeatsRequest\x12\x35\n\nheartbeats\x18\x01 \x03(\x0b\x32\x15.v1.InstanceHeartbeatR\nheartbeats\"\x14\n\x12HeartbeatsResponse\"9\n\x14GetHeartbeatsRequest\x12!\n\x0binstanceIds\x18\x01 \x03(\tR\x0cinstance_ids\"F\n\x15GetHeartbeatsResponse\x12-\n\x07records\x18\x01 \x03(\x0b\x32\x13.v1.HeartbeatRecordR\x07records\"9\n\x14\x44\x65lHeartbeatsRequest\x12!\n\x0binstanceIds\x18\x01 \x03(\tR\x0cinstance_ids\"3\n\x15\x44\x65lHeartbeatsResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\r\x12\x0c\n\x04info\x18\x02 \x01(\tB\x7f\n7com.tencent.polaris.specification.api.v1.service.manageZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'heartbeat_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
-  _HEARTBEATRECORD._serialized_start=39
-  _HEARTBEATRECORD._serialized_end=253
-  _HEARTBEATS._serialized_start=255
-  _HEARTBEATS._serialized_end=313
-  _GETHEARTBEATSREQUEST._serialized_start=315
-  _GETHEARTBEATSREQUEST._serialized_end=372
-  _GETHEARTBEATSRESPONSE._serialized_start=374
-  _GETHEARTBEATSRESPONSE._serialized_end=444
-  _DELHEARTBEATSREQUEST._serialized_start=446
-  _DELHEARTBEATSREQUEST._serialized_end=503
-  _DELHEARTBEATSRESPONSE._serialized_start=505
-  _DELHEARTBEATSRESPONSE._serialized_end=556
+  _HEARTBEATRECORD._serialized_start=38
+  _HEARTBEATRECORD._serialized_end=162
+  _INSTANCEHEARTBEAT._serialized_start=165
+  _INSTANCEHEARTBEAT._serialized_end=313
+  _HEARTBEATSREQUEST._serialized_start=315
+  _HEARTBEATSREQUEST._serialized_end=389
+  _HEARTBEATSRESPONSE._serialized_start=391
+  _HEARTBEATSRESPONSE._serialized_end=411
+  _GETHEARTBEATSREQUEST._serialized_start=413
+  _GETHEARTBEATSREQUEST._serialized_end=470
+  _GETHEARTBEATSRESPONSE._serialized_start=472
+  _GETHEARTBEATSRESPONSE._serialized_end=542
+  _DELHEARTBEATSREQUEST._serialized_start=544
+  _DELHEARTBEATSREQUEST._serialized_end=601
+  _DELHEARTBEATSRESPONSE._serialized_start=603
+  _DELHEARTBEATSRESPONSE._serialized_end=654
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -29,29 +29,39 @@
 class GetHeartbeatsResponse(_message.Message):
     __slots__ = ["records"]
     RECORDS_FIELD_NUMBER: _ClassVar[int]
     records: _containers.RepeatedCompositeFieldContainer[HeartbeatRecord]
     def __init__(self, records: _Optional[_Iterable[_Union[HeartbeatRecord, _Mapping]]] = ...) -> None: ...
 
 class HeartbeatRecord(_message.Message):
-    __slots__ = ["exist", "host", "instanceId", "lastHeartbeatSec", "namespace", "port", "service"]
+    __slots__ = ["exist", "instanceId", "lastHeartbeatSec"]
     EXIST_FIELD_NUMBER: _ClassVar[int]
-    HOST_FIELD_NUMBER: _ClassVar[int]
     INSTANCEID_FIELD_NUMBER: _ClassVar[int]
     LASTHEARTBEATSEC_FIELD_NUMBER: _ClassVar[int]
+    exist: bool
+    instanceId: str
+    lastHeartbeatSec: int
+    def __init__(self, instanceId: _Optional[str] = ..., lastHeartbeatSec: _Optional[int] = ..., exist: bool = ...) -> None: ...
+
+class HeartbeatsRequest(_message.Message):
+    __slots__ = ["heartbeats"]
+    HEARTBEATS_FIELD_NUMBER: _ClassVar[int]
+    heartbeats: _containers.RepeatedCompositeFieldContainer[InstanceHeartbeat]
+    def __init__(self, heartbeats: _Optional[_Iterable[_Union[InstanceHeartbeat, _Mapping]]] = ...) -> None: ...
+
+class HeartbeatsResponse(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
+class InstanceHeartbeat(_message.Message):
+    __slots__ = ["host", "instanceId", "namespace", "port", "service"]
+    HOST_FIELD_NUMBER: _ClassVar[int]
+    INSTANCEID_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     PORT_FIELD_NUMBER: _ClassVar[int]
     SERVICE_FIELD_NUMBER: _ClassVar[int]
-    exist: bool
     host: str
     instanceId: str
-    lastHeartbeatSec: int
     namespace: str
     port: int
     service: str
-    def __init__(self, instanceId: _Optional[str] = ..., service: _Optional[str] = ..., namespace: _Optional[str] = ..., host: _Optional[str] = ..., port: _Optional[int] = ..., lastHeartbeatSec: _Optional[int] = ..., exist: bool = ...) -> None: ...
-
-class Heartbeats(_message.Message):
-    __slots__ = ["heartbeats"]
-    HEARTBEATS_FIELD_NUMBER: _ClassVar[int]
-    heartbeats: _containers.RepeatedCompositeFieldContainer[_service_pb2.Instance]
-    def __init__(self, heartbeats: _Optional[_Iterable[_Union[_service_pb2.Instance, _Mapping]]] = ...) -> None: ...
+    def __init__(self, instanceId: _Optional[str] = ..., service: _Optional[str] = ..., namespace: _Optional[str] = ..., host: _Optional[str] = ..., port: _Optional[int] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/request_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/request_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/response_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/response_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/service_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/service_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi` & `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/LICENSE.txt` & `polarismesh_specification-1.3.0a7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/README.md` & `polarismesh_specification-1.3.0a7/README.md`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/pyproject.toml` & `polarismesh_specification-1.3.0a7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a6/PKG-INFO` & `polarismesh_specification-1.3.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polarismesh-specification
-Version: 1.3.0a6
+Version: 1.3.0a7
 Project-URL: Documentation, https://github.com/polarismesh/specification#readme
 Project-URL: Issues, https://github.com/polarismesh/specification/issues
 Project-URL: Source, https://github.com/polarismesh/specification
 Author-email: "{authemail@qq.com}" <authemail@qq.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

