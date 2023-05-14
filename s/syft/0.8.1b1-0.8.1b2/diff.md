# Comparing `tmp/syft-0.8.1b1.tar.gz` & `tmp/syft-0.8.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.1b1.tar", last modified: Sun May  7 12:48:27 2023, max compression
+gzip compressed data, was "syft-0.8.1b2.tar", last modified: Sun May 14 12:45:01 2023, max compression
```

## Comparing `syft-0.8.1b1.tar` & `syft-0.8.1b2.tar`

### file list

```diff
@@ -1,176 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.060686 syft-0.8.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-05-07 12:45:55.000000 syft-0.8.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-07 12:45:55.000000 syft-0.8.1b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-07 12:48:27.060686 syft-0.8.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-07 12:45:54.000000 syft-0.8.1b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-07 12:45:55.000000 syft-0.8.1b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-07 12:48:27.064686 syft-0.8.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-07 12:45:55.000000 syft-0.8.1b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.036685 syft-0.8.1b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.036685 syft-0.8.1b1/src/syft/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-07 12:46:11.000000 syft-0.8.1b1/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-07 12:46:11.000000 syft-0.8.1b1/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.040685 syft-0.8.1b1/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.040685 syft-0.8.1b1/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23296 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21112 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.040685 syft-0.8.1b1/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.044685 syft-0.8.1b1/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.044685 syft-0.8.1b1/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    26952 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.048685 syft-0.8.1b1/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/third_party.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.048685 syft-0.8.1b1/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.048685 syft-0.8.1b1/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    37961 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21160 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.048685 syft-0.8.1b1/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    21157 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.052686 syft-0.8.1b1/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.052686 syft-0.8.1b1/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.052686 syft-0.8.1b1/src/syft/service/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/message/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/message/message_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/message/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.052686 syft-0.8.1b1/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/metadata/metadata_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.052686 syft-0.8.1b1/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/network/network_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.052686 syft-0.8.1b1/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21237 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.056686 syft-0.8.1b1/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.056686 syft-0.8.1b1/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/queue/queue_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.056686 syft-0.8.1b1/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16568 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.056686 syft-0.8.1b1/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.060686 syft-0.8.1b1/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.060686 syft-0.8.1b1/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.060686 syft-0.8.1b1/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.036685 syft-0.8.1b1/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-07 12:48:27.000000 syft-0.8.1b1/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-07 12:48:27.000000 syft-0.8.1b1/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 12:48:27.000000 syft-0.8.1b1/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-07 12:48:27.000000 syft-0.8.1b1/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 12:48:26.000000 syft-0.8.1b1/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-07 12:48:27.000000 syft-0.8.1b1/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 12:48:27.000000 syft-0.8.1b1/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:01.022682 syft-0.8.1b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-05-14 12:42:01.000000 syft-0.8.1b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-14 12:42:01.000000 syft-0.8.1b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-14 12:45:01.022682 syft-0.8.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-14 12:42:01.000000 syft-0.8.1b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-14 12:42:01.000000 syft-0.8.1b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-14 12:45:01.026682 syft-0.8.1b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-14 12:42:01.000000 syft-0.8.1b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.922682 syft-0.8.1b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.938682 syft-0.8.1b2/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-14 12:42:19.000000 syft-0.8.1b2/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-14 12:42:19.000000 syft-0.8.1b2/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.942682 syft-0.8.1b2/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.946682 syft-0.8.1b2/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24303 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.950682 syft-0.8.1b2/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.954682 syft-0.8.1b2/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15930 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.962682 syft-0.8.1b2/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27103 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.970682 syft-0.8.1b2/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/third_party.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.970682 syft-0.8.1b2/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.978682 syft-0.8.1b2/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46598 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27045 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.982682 syft-0.8.1b2/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21458 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.986682 syft-0.8.1b2/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.990682 syft-0.8.1b2/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.990682 syft-0.8.1b2/src/syft/service/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/message/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/message/message_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/message/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.994682 syft-0.8.1b2/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/metadata/metadata_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.994682 syft-0.8.1b2/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (123)    15290 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/network/network_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.994682 syft-0.8.1b2/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.998682 syft-0.8.1b2/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22709 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.998682 syft-0.8.1b2/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/queue/queue_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:01.002682 syft-0.8.1b2/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:01.006682 syft-0.8.1b2/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:01.010682 syft-0.8.1b2/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:01.018682 syft-0.8.1b2/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:01.022682 syft-0.8.1b2/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.942682 syft-0.8.1b2/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.1b1/LICENSE` & `syft-0.8.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/PKG-INFO` & `syft-0.8.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b1
+Version: 0.8.1b2
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b1 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b2 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.1b1/README.md` & `syft-0.8.1b2/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/setup.cfg` & `syft-0.8.1b2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.1-beta.1"
+version = attr: "0.8.1-beta.2"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -38,15 +38,15 @@
 	pandas==1.5.3
 	pyarrow==11.0.0
 	pycapnp==1.3.0
 	pydantic[email]==1.10.7
 	pymongo==4.3.3
 	pynacl==1.5.0
 	redis==4.5.4
-	requests==2.28.2
+	requests==2.29.0
 	RestrictedPython==6.0
 	result==0.9.0
 	tqdm==4.65.0
 	typeguard==2.13.3
 	typing_extensions==4.5.0
 	sherlock[redis,filelock]==0.4.1
 	uvicorn[standard]==0.21.1
@@ -90,15 +90,15 @@
 	python_on_whales
 	pytest-lazy-fixture
 	pytest-rerunfailures
 	coverage
 	joblib
 	faker
 oblv = 
-	pyoblv==0.2.0
+	oblv-ctl==0.3.1
 
 [options.entry_points]
 console_scripts = 
 	syft=syft.node.run:run
 
 [test]
 addopts = --verbose
```

### Comparing `syft-0.8.1b1/src/syft/VERSION` & `syft-0.8.1b2/src/syft/VERSION`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.1-beta.1"
+__version__ = "0.8.1-beta.2"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.1b1/src/syft/__init__.py` & `syft-0.8.1b2/src/syft/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.1-beta.1"
+__version__ = "0.8.1-beta.2"
 
 # stdlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
 
@@ -26,14 +26,16 @@
 from .node.server import serve_node as bind_worker  # noqa: F401
 from .node.worker import Worker  # noqa: F401
 from .serde import NOTHING  # noqa: F401
 from .serde.deserialize import _deserialize as deserialize  # noqa: F401
 from .serde.serializable import serializable  # noqa: F401
 from .serde.serialize import _serialize as serialize  # noqa: F401
 from .service.action.action_object import ActionObject  # noqa: F401
+from .service.action.plan import Plan  # noqa: F401
+from .service.action.plan import planify  # noqa: F401
 from .service.code.user_code import UserCodeStatus  # noqa: F401
 from .service.code.user_code import syft_function  # noqa: F401
 from .service.data_subject import DataSubjectCreate as DataSubject  # noqa: F401
 from .service.dataset.dataset import CreateAsset as Asset  # noqa: F401
 from .service.dataset.dataset import CreateDataset as Dataset  # noqa: F401
 from .service.message.messages import MessageStatus  # noqa: F401
 from .service.policy.policy import CustomInputPolicy  # noqa: F401
@@ -45,20 +47,24 @@
 from .service.project.project import ProjectSubmit as Project  # noqa: F401
 from .service.request.request import SubmitRequest as Request  # noqa: F401
 from .service.response import SyftError  # noqa: F401
 from .service.response import SyftNotReady  # noqa: F401
 from .service.response import SyftSuccess  # noqa: F401
 from .service.user.roles import Roles as roles  # noqa: F401
 from .service.user.user_service import UserService  # noqa: F401
+from .types.twin_object import TwinObject  # noqa: F401
 from .types.uid import UID  # noqa: F401
 from .util import filterwarnings  # noqa: F401
 from .util import jax_settings  # noqa: F401
 from .util import logger  # noqa: F401
+from .util.autoreload import disable_autoreload  # noqa: F401
+from .util.autoreload import enable_autoreload  # noqa: F401
 from .util.telemetry import instrument  # noqa: F401
 from .util.util import autocache  # noqa: F401
+from .util.util import get_root_data_path  # noqa: F401
 from .util.version_compare import make_requires
 
 LATEST_STABLE_SYFT = "0.8"
 requires = make_requires(LATEST_STABLE_SYFT, __version__)
 
 sys.path.append(str(Path(__file__)))
```

### Comparing `syft-0.8.1b1/src/syft/abstract_node.py` & `syft-0.8.1b2/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/client/api.py` & `syft-0.8.1b2/src/syft/client/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from ..service.service import UserLibConfigRegistry
 from ..service.service import UserServiceConfigRegistry
 from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftObject
 from ..types.uid import LineageID
 from ..types.uid import UID
+from ..util.autoreload import autoreload_enabled
 from ..util.telemetry import instrument
 from .connection import NodeConnection
 
 
 class APIRegistry:
     __api_registry__: Dict[str, SyftAPI] = {}
 
@@ -221,14 +222,24 @@
 ):
     if "blocking" in signature.parameters:
         raise Exception(
             f"Signature {signature} can't have 'blocking' kwarg because its reserved"
         )
 
     def wrapper(*args, **kwargs):
+        # relative
+        from ..service.action.action_object import TraceResult
+
+        if TraceResult._client is not None:
+            wrapper_make_call = TraceResult._client.api.make_call
+            wrapper_node_uid = TraceResult._client.api.node_uid
+        else:
+            # somehow this is necessary to prevent shadowing problems
+            wrapper_make_call = make_call
+            wrapper_node_uid = node_uid
         blocking = True
         if "blocking" in kwargs:
             blocking = bool(kwargs["blocking"])
             del kwargs["blocking"]
 
         res = validate_callable_args_and_kwargs(args, kwargs, signature)
 
@@ -237,42 +248,46 @@
         _valid_args, _valid_kwargs = res
 
         if pre_kwargs:
             _valid_kwargs.update(pre_kwargs)
 
         # relative
         from ..service.action.action_object import Action
+        from ..service.action.action_object import ActionType
         from ..service.action.action_object import convert_to_pointers
 
         action_args, action_kwargs = convert_to_pointers(
-            api, node_uid, _valid_args, _valid_kwargs
+            api, wrapper_node_uid, _valid_args, _valid_kwargs
         )
 
         # e.g. numpy.array -> numpy, array
         module, op = module_path.rsplit(".", 1)
-        service_args = [
-            Action(
-                path=module,
-                op=op,
-                remote_self=None,
-                args=[x.syft_lineage_id for x in action_args],
-                kwargs={k: v.syft_lineage_id for k, v in action_kwargs},
-                # TODO: fix
-                result_id=LineageID(UID(), 1),
-            )
-        ]
+        action = Action(
+            path=module,
+            op=op,
+            remote_self=None,
+            args=[x.syft_lineage_id for x in action_args],
+            kwargs={k: v.syft_lineage_id for k, v in action_kwargs},
+            action_type=ActionType.FUNCTION,
+            # TODO: fix
+            result_id=LineageID(UID(), 1),
+        )
+        service_args = [action]
+        # TODO: implement properly
+        TraceResult.result += [action]
 
         api_call = SyftAPICall(
-            node_uid=node_uid,
+            node_uid=wrapper_node_uid,
             path=path,
             args=service_args,
             kwargs=dict(),
             blocking=blocking,
         )
-        result = make_call(api_call=api_call)
+
+        result = wrapper_make_call(api_call=api_call)
         return result
 
     wrapper.__ipython_inspector_signature_override__ = signature
     return wrapper
 
 
 @serializable()
@@ -308,15 +323,15 @@
         if not hasattr(self, "get_all"):
             return NotImplementedError
         results = self.get_all()
         return results._repr_html_()
 
 
 @instrument
-@serializable(attrs=["endpoints", "node_uid", "node_name"])
+@serializable(attrs=["endpoints", "node_uid", "node_name", "lib_endpoints"])
 class SyftAPI(SyftObject):
     # version
     __canonical_name__ = "SyftAPI"
     __version__ = SYFT_OBJECT_VERSION_1
 
     # fields
     connection: Optional[NodeConnection] = None
@@ -682,15 +697,25 @@
                             if issubclass(v, EmailStr):
                                 v = str
                             check_type(param_key, arg, v)  # raises Exception
                             break  # only need one to match
                     else:
                         check_type(param_key, arg, t)  # raises Exception
             except TypeError:
-                _type_str = getattr(t, "__name__", str(t))
-                msg = f"Arg: {arg} must be {_type_str} not {type(arg).__name__}"
+                t_arg = type(arg)
+                if (
+                    autoreload_enabled()
+                    and t.__module__ == t_arg.__module__
+                    and t.__name__ == t_arg.__name__
+                ):
+                    # ignore error when autoreload_enabled()
+                    pass
+                else:
+                    _type_str = getattr(t, "__name__", str(t))
+                    msg = f"Arg: {arg} must be {_type_str} not {type(arg).__name__}"
+
             if msg:
                 return SyftError(message=msg)
 
             _valid_args.append(arg)
 
     return _valid_args, _valid_kwargs
```

### Comparing `syft-0.8.1b1/src/syft/client/client.py` & `syft-0.8.1b2/src/syft/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,16 @@
     url: GridURL
     routes: Type[Routes] = Routes
     session_cache: Optional[Session]
 
     def __init__(
         self, url: Union[GridURL, str], proxy_target_uid: Optional[UID] = None
     ) -> None:
-        url = GridURL.from_url(url)
+        url = GridURL.from_url(url).as_container_host()
+
         proxy_target_uid = proxy_target_uid
         super().__init__(url=url, proxy_target_uid=proxy_target_uid)
 
     def with_proxy(self, proxy_target_uid: UID) -> Self:
         return HTTPConnection(url=self.url, proxy_target_uid=proxy_target_uid)
 
     def get_cache_key(self) -> str:
```

### Comparing `syft-0.8.1b1/src/syft/client/connection.py` & `syft-0.8.1b2/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/client/deploy.py` & `syft-0.8.1b2/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/client/registry.py` & `syft-0.8.1b2/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/client/search.py` & `syft-0.8.1b2/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/client/user_settings.py` & `syft-0.8.1b2/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/external/__init__.py` & `syft-0.8.1b2/src/syft/external/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 # if the external library is not installed, we prompt the user
 # to install it with the pip package name.
 
 OBLV = str_to_bool(os.getenv("ENABLE_OBLV", "false"))
 
 EXTERNAL_LIBS = {
     "oblv": {
-        "pip_package_name": "pyoblv",
-        "module_name": "oblv",
+        "pip_package_name": "oblv-ctl",
+        "module_name": "oblv_ctl",
     }
 }
 
 
 def package_exists(package_name: str) -> bool:
     try:
         importlib.import_module(package_name)
```

### Comparing `syft-0.8.1b1/src/syft/external/oblv/__init__.py` & `syft-0.8.1b2/src/syft/external/oblv/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .oblv_proxy import check_oblv_proxy_installation_status  # noqa: F401
 from .oblv_proxy import create_oblv_key_pair  # noqa: F401
 from .oblv_proxy import get_oblv_public_key  # noqa: F401
 from .oblv_proxy import install_oblv_proxy  # noqa: F401
 
 try:
     # third party
-    from oblv.oblv_client import OblvClient
+    from oblv_ctl.oblv_client import OblvClient
 
     # Oblivious Client serde
     recursive_serde_register(
         OblvClient,
         serialize=lambda x: _serialize([x.token, x.oblivious_user_id], to_bytes=True),
         deserialize=lambda x: OblvClient(*_deserialize(x, from_bytes=True)),
     )
```

### Comparing `syft-0.8.1b1/src/syft/external/oblv/deployment.py` & `syft-0.8.1b2/src/syft/external/oblv/deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # stdlib
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 # third party
-from oblv import OblvClient
-from oblv.models import CreateDeploymentInput
+from oblv_ctl import OblvClient
+from oblv_ctl.models import CreateDeploymentInput
 import yaml
 
 # relative
-from ...util import bcolors
+from ...util.util import bcolors
 from .auth import login
 from .constants import INFRA
 from .constants import REF
 from .constants import REF_TYPE
 from .constants import REGION
 from .constants import REPO_NAME
 from .constants import REPO_OWNER
```

### Comparing `syft-0.8.1b1/src/syft/external/oblv/deployment_client.py` & `syft-0.8.1b2/src/syft/external/oblv/deployment_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,25 @@
 import time
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import TYPE_CHECKING
-from typing import cast
 
 # third party
-from oblv import OblvClient
+from oblv_ctl import OblvClient
 from pydantic import BaseModel
 from pydantic import validator
 import requests
 
 # relative
 from ...client.api import SyftAPI
-from ...client.client import HTTPConnection
-from ...client.client import Routes
-from ...client.client import SyftSigningKey
-from ...serde.deserialize import _deserialize as deserialize
+from ...client.client import SyftClient
+from ...client.client import login
 from ...serde.serializable import serializable
 from ...service.metadata.node_metadata import EnclaveMetadata
 from ...types.uid import UID
 from ...util.util import bcolors
 from .constants import LOCAL_MODE
 from .exceptions import OblvEnclaveError
 from .exceptions import OblvUnAuthorizedError
@@ -72,19 +69,20 @@
             )
         return oblv_client
 
 
 class DeploymentClient:
     deployment_id: str
     key_name: str
-    domain_clients: List[Any] = []  # List of domain client objects
+    domain_clients: List[SyftClient] = []  # List of domain client objects
     oblv_client: OblvClient = None
     __conn_string: str
     __logs: Any
     __process: Any
+    __enclave_client: SyftClient
 
     def __init__(
         self,
         domain_clients: List[Any],
         deployment_id: str,
         oblv_client: Optional[OblvClient] = None,
         key_name: Optional[str] = None,
@@ -98,14 +96,15 @@
         self.key_name = key_name
         self.oblv_client = oblv_client
         self.domain_clients = domain_clients
         self.__conn_string = ""
         self.__process = None
         self.__logs = None
         self._api = api
+        self.__enclave_client = None
 
     def make_request_to_enclave(
         self,
         request_method: Callable,
         connection_string: str,
         params: Optional[Dict] = None,
         files: Optional[Dict] = None,
@@ -238,14 +237,42 @@
                 f"Successfully connected to proxy on port {connection_port}. The logs can be found at {log_file_name}"
             )
         self.__conn_string = f"http://127.0.0.1:{connection_port}"
         self.__logs = log_file_name
         self.__process = process
         return
 
+    def register(
+        self,
+        name: str,
+        email: str,
+        password: str,
+        institution: Optional[str] = None,
+        website: Optional[str] = None,
+    ):
+        self.check_connection_string()
+        guest_client = login(url=self.__conn_string)
+        return guest_client.register(
+            name=name,
+            email=email,
+            password=password,
+            institution=institution,
+            website=website,
+        )
+
+    def login(
+        self,
+        email: str,
+        password: str,
+    ) -> None:
+        self.check_connection_string()
+        self.__enclave_client = login(
+            url=self.__conn_string, email=email, password=password
+        )
+
     def check_connection_string(self) -> None:
         if not self.__conn_string:
             raise Exception(
                 "Either proxy not running or not initiated using syft."
                 + " Run the method initiate_connection to initiate the proxy connection"
             )
 
@@ -283,47 +310,20 @@
         for domain_client in self.domain_clients:
             domain_client.api.services.code.request_code_execution(code=code)
 
         res = self.api.services.code.request_code_execution(code=code)
 
         return res
 
-    def _get_api(self) -> SyftAPI:
-        self.check_connection_string()
-        signing_key = SyftSigningKey.generate()
-
-        params = {"verify_key": str(signing_key.verify_key)}
-        req = self.make_request_to_enclave(
-            requests.get,
-            connection_string=self.__conn_string + Routes.ROUTE_API.value,
-            params=params,
-        )
-        self.sanity_check_oblv_response(req)
-        obj = deserialize(req.content, from_bytes=True)
-        # TODO 🟣 Retrieve of signing key of user after permission  is fully integrated
-        obj.signing_key = signing_key
-        obj.connection = HTTPConnection(self.__conn_string)
-        return cast(SyftAPI, obj)
-
-    # public attributes
-
-    def _set_api(self) -> None:
-        _api = self._get_api()
-        # APIRegistry.set_api_for(node_uid=self.id, api=_api)
-        self._api = _api
-
     @property
     def api(self) -> SyftAPI:
-        if self._api is None:
-            self._set_api()
-
-        return cast(SyftAPI, self._api)
+        if not self.__enclave_client:
+            raise Exception("Kindly login or register with the enclave")
 
-    def refresh(self) -> None:
-        self._set_api()
+        return self.__enclave_client.api
 
     def close_connection(self) -> Optional[str]:
         if self.check_proxy_running():
             os.kill(self.__process.pid, SIGTERM)
             return None
         else:
             return "No Proxy Connection Running"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `syft-0.8.1b1/src/syft/external/oblv/exceptions.py` & `syft-0.8.1b2/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.1b2/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.1b2/src/syft/external/oblv/oblv_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import tarfile
 import zipfile
 
 # third party
 import requests
 
 # relative
-from ...util import bcolors
+from ...util.util import bcolors
 
 
 def check_oblv_proxy_installation_status():
     try:
         result = subprocess.run(["oblv", "-V"], capture_output=True, text=True)  # nosec
         if result.stderr:
             raise subprocess.CalledProcessError(  # nosec
```

### Comparing `syft-0.8.1b1/src/syft/external/oblv/oblv_service.py` & `syft-0.8.1b2/src/syft/external/oblv/oblv_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 from typing import cast
 
 # third party
-from oblv import OblvClient
+from oblv_ctl import OblvClient
 import requests
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
 from ...client.api import NodeView
@@ -382,15 +382,14 @@
         context: AuthedServiceContext,
         user_code_id: UID,
         inputs: Dict,
         node_name: str,
     ) -> Result[Ok, Err]:
         if not context.node or not context.node.signing_key:
             return Err(f"{type(context)} has no node")
-        signing_key = context.node.signing_key
 
         user_code_service = context.node.get_service("usercodeservice")
         action_service = context.node.get_service("actionservice")
         user_code = user_code_service.stash.get_by_uid(
             context.node.signing_key.verify_key, uid=user_code_id
         )
         if user_code.is_err():
@@ -410,28 +409,29 @@
         user_code_service.update_code_state(context=context, code_item=user_code)
 
         if not action_service.exists(context=context, obj_id=user_code_id):
             dict_object = DictObject(id=user_code_id)
             dict_object.base_dict[str(context.credentials)] = inputs
             action_service.store.set(
                 uid=user_code_id,
-                credentials=signing_key.verify_key,
+                credentials=user_code.user_verify_key,
                 syft_object=dict_object,
+                has_result_read_permission=True,
             )
 
         else:
             res = action_service.store.get(
-                uid=user_code_id, credentials=signing_key.verify_key
+                uid=user_code_id, credentials=user_code.user_verify_key
             )
             if res.is_ok():
                 dict_object = res.ok()
                 dict_object.base_dict[str(context.credentials)] = inputs
                 action_service.store.set(
                     uid=user_code_id,
-                    credentials=signing_key.verify_key,
+                    credentials=user_code.user_verify_key,
                     syft_object=dict_object,
                 )
             else:
                 return res
 
         return Ok(Ok(True))
 
@@ -467,11 +467,10 @@
             if action_object.is_err():
                 return action_object
             inputs[var_name] = action_object.ok()
 
         res = api.services.oblv.send_user_code_inputs_to_enclave(
             user_code_id=user_code.id, inputs=inputs, node_name=context.node.name
         )
-
         return res
     else:
         return Ok()
```

### Comparing `syft-0.8.1b1/src/syft/gevent_patch.py` & `syft-0.8.1b2/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/node/credentials.py` & `syft-0.8.1b2/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/node/node.py` & `syft-0.8.1b2/src/syft/node/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 # stdlib
 import contextlib
 from datetime import datetime
 from functools import partial
 import hashlib
+from multiprocessing import current_process
 import os
 import threading
 import traceback
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
@@ -50,14 +51,15 @@
 from ..service.dataset.dataset_service import DatasetService
 from ..service.message.message_service import MessageService
 from ..service.metadata.metadata_service import MetadataService
 from ..service.metadata.metadata_stash import MetadataStash
 from ..service.metadata.node_metadata import NodeMetadata
 from ..service.network.network_service import NetworkService
 from ..service.policy.policy_service import PolicyService
+from ..service.project.project_service import NewProjectService
 from ..service.project.project_service import ProjectService
 from ..service.queue.queue_stash import QueueItem
 from ..service.queue.queue_stash import QueueStash
 from ..service.request.request_service import RequestService
 from ..service.response import SyftError
 from ..service.service import AbstractService
 from ..service.service import ServiceConfigRegistry
@@ -173,14 +175,15 @@
             self.signing_key = signing_key
 
         if self.signing_key is None:
             self.signing_key = SyftSigningKey.generate()
 
         self.processes = processes
         self.is_subprocess = is_subprocess
+
         if name is None:
             name = random_name()
         self.name = name
         services = (
             [
                 UserService,
                 MetadataService,
@@ -190,14 +193,15 @@
                 RequestService,
                 DataSubjectService,
                 NetworkService,
                 PolicyService,
                 MessageService,
                 ProjectService,
                 DataSubjectMemberService,
+                NewProjectService,
             ]
             if services is None
             else services
         )
 
         self.service_config = ServiceConfigRegistry.get_registered_configs()
         self.local_db = local_db
@@ -270,15 +274,15 @@
             signing_key=key,
             processes=processes,
             local_db=local_db,
             sqlite_path=sqlite_path,
         )
 
     def is_root(self, credentials: SyftVerifyKey) -> bool:
-        return credentials == self.signing_key.verify_key
+        return credentials == self.verify_key
 
     @property
     def root_client(self):
         # relative
         from ..client.client import PythonConnection
         from ..client.client import SyftClient
 
@@ -291,33 +295,37 @@
         from ..client.client import PythonConnection
         from ..client.client import SyftClient
 
         connection = PythonConnection(node=self)
         return SyftClient(connection=connection, credentials=SyftSigningKey.generate())
 
     def __repr__(self) -> str:
-        services = []
-        for service in self.services:
-            services.append(service.__name__)
-        service_string = "\n".join(sorted(services))
-        return f"{type(self).__name__}: {self.name} - {self.id} - {self.node_type}\n\nServices:\n{service_string}"
+        service_string = ""
+        if not self.is_subprocess:
+            services = []
+            for service in self.services:
+                services.append(service.__name__)
+            service_string = ", ".join(sorted(services))
+            service_string = f"\n\nServices:\n{service_string}"
+        return f"{type(self).__name__}: {self.name} - {self.id} - {self.node_type}{service_string}"
 
     def post_init(self) -> None:
-        context = AuthedServiceContext(
-            node=self, credentials=self.signing_key.verify_key
-        )
+        context = AuthedServiceContext(node=self, credentials=self.verify_key)
 
         if UserCodeService in self.services:
             user_code_service = self.get_service(UserCodeService)
             user_code_service.load_user_code(context=context)
-        if self.is_subprocess:
+
+        if self.is_subprocess or current_process().name != "MainProcess":
             # print(f"> Starting Subprocess {self}")
             pass
         else:
-            print(f"> {self}")
+            pass
+            # why would we do this?
+            # print(f"> {self}")
 
         def reload_user_code() -> None:
             user_code_service.load_user_code(context=context)
 
         CODE_RELOADER[thread_ident()] = reload_user_code
         # super().post_init()
 
@@ -340,15 +348,15 @@
             print(
                 f"SQLite Store Path:\n!open file://{document_store_config.client_config.file_path}\n"
             )
         document_store = document_store_config.store_type
         self.document_store_config = document_store_config
 
         self.document_store = document_store(
-            root_verify_key=self.signing_key.verify_key,
+            root_verify_key=self.verify_key,
             store_config=document_store_config,
         )
         if action_store_config is None:
             if self.local_db or (self.processes > 0 and not self.is_subprocess):
                 client_config = SQLiteStoreClientConfig(path=self.sqlite_path)
                 action_store_config = SQLiteStoreConfig(client_config=client_config)
             else:
@@ -359,20 +367,18 @@
             and action_store_config.client_config.filename is None
         ):
             action_store_config.client_config.filename = f"{self.id}.sqlite"
 
         if isinstance(action_store_config, SQLiteStoreConfig):
             self.action_store = SQLiteActionStore(
                 store_config=action_store_config,
-                root_verify_key=self.signing_key.verify_key,
+                root_verify_key=self.verify_key,
             )
         else:
-            self.action_store = DictActionStore(
-                root_verify_key=self.signing_key.verify_key
-            )
+            self.action_store = DictActionStore(root_verify_key=self.verify_key)
 
         self.action_store_config = action_store_config
         self.queue_stash = QueueStash(store=self.document_store)
 
     def _construct_services(self):
         self.service_path_map = {}
 
@@ -388,14 +394,15 @@
                 RequestService,
                 DataSubjectService,
                 NetworkService,
                 PolicyService,
                 MessageService,
                 ProjectService,
                 DataSubjectMemberService,
+                NewProjectService,
             ]
 
             if OBLV:
                 # relative
                 from ..external.oblv.oblv_service import OblvService
 
                 store_services += [OblvService]
@@ -431,24 +438,28 @@
         return getattr(service_obj, method_name)
 
     @property
     def metadata(self) -> NodeMetadata:
         return NodeMetadata(
             name=self.name,
             id=self.id,
-            verify_key=self.signing_key.verify_key,
+            verify_key=self.verify_key,
             highest_object_version=HIGHEST_SYFT_OBJECT_VERSION,
             lowest_object_version=LOWEST_SYFT_OBJECT_VERSION,
             syft_version=__version__,
         )
 
     @property
     def icon(self) -> str:
         return "🦾"
 
+    @property
+    def verify_key(self) -> SyftVerifyKey:
+        return self.signing_key.verify_key
+
     def __hash__(self) -> int:
         return hash(self.id)
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, type(self)):
             return False
 
@@ -605,44 +616,39 @@
     ) -> NodeServiceContext:
         return UnauthedServiceContext(node=self, login_credentials=login_credentials)
 
 
 def task_producer(
     pipe: _GIPCDuplexHandle, api_call: SyftAPICall, blocking: bool
 ) -> Any:
-    print("task_producer: Start")
-
     try:
         result = None
         with pipe:
             pipe.put(api_call)
             gevent.sleep(0)
             if blocking:
                 try:
                     result = pipe.get()
                 except EOFError:
                     pass
             pipe.close()
         if blocking:
-            print("task_producer: End")
             return result
     except gipc.gipc.GIPCClosed:
         pass
     except Exception as e:
         print("Exception in task_producer", e)
 
 
 def task_runner(
     pipe: _GIPCDuplexHandle,
     worker_settings: WorkerSettings,
     task_uid: UID,
     blocking: bool,
 ) -> None:
-    print("task_runner: Start")
-
     worker = Node(
         id=worker_settings.id,
         name=worker_settings.name,
         signing_key=worker_settings.signing_key,
         document_store_config=worker_settings.document_store_config,
         action_store_config=worker_settings.action_store_config,
         is_subprocess=True,
@@ -660,25 +666,22 @@
                 )
                 worker.queue_stash.set_result(item)
                 worker.queue_stash.partition.close()
             pipe.close()
     except Exception as e:
         print("Exception in task_runner", e)
         raise e
-    print("task_runner: End")
 
 
 def queue_task(
     api_call: SyftAPICall,
     worker_settings: WorkerSettings,
     task_uid: UID,
     blocking: bool,
 ) -> Optional[Any]:
-    print("queue_task: Start")
-
     with gipc.pipe(encoder=gipc_encoder, decoder=gipc_decoder, duplex=True) as (
         cend,
         pend,
     ):
         process = gipc.start_process(
             task_runner, args=(cend, worker_settings, task_uid, blocking)
         )
@@ -687,17 +690,15 @@
             process.join()
         except KeyboardInterrupt:
             producer.kill(block=True)
             process.terminate()
         process.join()
 
     if blocking:
-        print("queue_task: End")
         return producer.value
-    print("queue_task: End")
     return None
 
 
 def create_worker_metadata(
     worker: AbstractNode,
 ) -> Optional[NodeMetadata]:
     try:
```

### Comparing `syft-0.8.1b1/src/syft/node/routes.py` & `syft-0.8.1b2/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/node/run.py` & `syft-0.8.1b2/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/node/server.py` & `syft-0.8.1b2/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/node/worker_settings.py` & `syft-0.8.1b2/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/serde/array.py` & `syft-0.8.1b2/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/serde/arrow.py` & `syft-0.8.1b2/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/serde/deserialize.py` & `syft-0.8.1b2/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/serde/lib_permissions.py` & `syft-0.8.1b2/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/serde/lib_service_registry.py` & `syft-0.8.1b2/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/serde/recursive.py` & `syft-0.8.1b2/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/serde/recursive_primitives.py` & `syft-0.8.1b2/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/serde/serializable.py` & `syft-0.8.1b2/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/serde/signature.py` & `syft-0.8.1b2/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/serde/third_party.py` & `syft-0.8.1b2/src/syft/serde/third_party.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,9 +156,12 @@
     FrozenDict,
     serialize=lambda x: serialize(flax.serialization.to_state_dict(x), to_bytes=True),
     deserialize=lambda x: FrozenDict(
         flax.serialization.from_state_dict(FrozenDict, deserialize(x, from_bytes=True))
     ),
 )
 
+# unsure why we have to register the object not the type but this works
+recursive_serde_register(np.core._ufunc_config._unspecified())
+
 # how else do you import a relative file to execute it?
 NOTHING = None
```

### Comparing `syft-0.8.1b1/src/syft/service/action/action_object.py` & `syft-0.8.1b2/src/syft/service/action/action_object.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # future
 from __future__ import annotations
 
 # stdlib
+from enum import Enum
 import inspect
 import traceback
 import types
 from typing import Any
 from typing import Callable
 from typing import ClassVar
 from typing import Dict
@@ -23,27 +24,46 @@
 from result import Result
 from typing_extensions import Self
 
 # relative
 from ...client.api import SyftAPI
 from ...client.client import SyftClient
 from ...serde.serializable import serializable
+from ...store.linked_obj import LinkedObject
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftBaseObject
 from ...types.syft_object import SyftObject
 from ...types.uid import LineageID
 from ...types.uid import UID
 from ...util.logger import debug
 from ..response import SyftException
 from .action_data_empty import ActionDataEmpty
+from .action_permissions import ActionPermission
+from .action_types import action_type_for_object
 from .action_types import action_type_for_type
 from .action_types import action_types
 
 
 @serializable()
+class TwinMode(Enum):
+    NONE = 0
+    PRIVATE = 1
+    MOCK = 2
+
+
+@serializable()
+class ActionType(Enum):
+    GETATTRIBUTE = 1
+    METHOD = 2
+    SETATTRIBUTE = 4
+    FUNCTION = 8
+    CREATEOBJECT = 16
+
+
+@serializable()
 class Action(SyftObject):
     """Serializable Action object.
 
     Parameters:
         path: str
             The path of the Type of the remote object.
         op: str
@@ -65,14 +85,16 @@
 
     path: str
     op: str
     remote_self: Optional[LineageID]
     args: List[LineageID]
     kwargs: Dict[str, LineageID]
     result_id: Optional[LineageID]
+    action_type: Optional[ActionType]
+    create_object: Optional[SyftObject] = None
 
     @pydantic.validator("id", pre=True, always=True)
     def make_id(cls, v: Optional[UID]) -> UID:
         """Generate or reuse an UID"""
         return v if isinstance(v, UID) else UID()
 
     @pydantic.validator("result_id", pre=True, always=True)
@@ -100,21 +122,37 @@
         for arg in self.args:
             hashes += hash(arg.syft_history_hash)
         for k, arg in self.kwargs.items():
             hashes += hash(k)
             hashes += hash(arg.syft_history_hash)
         return hashes
 
+    def __repr__(self):
+        def repr_uid(_id):
+            return f"{str(_id)[:3]}..{str(_id)[-1]}"
+
+        arg_repr = ", ".join([repr_uid(x) for x in self.args])
+        kwargs_repr = ", ".join(
+            [f"{key}={repr_uid(value)}" for key, value in self.kwargs.items()]
+        )
+        self_repr = (
+            f"[{repr_uid(self.remote_self)}]" if self.remote_self is not None else ""
+        )
+        return (
+            f"ActionObject {self.path}{self_repr}.{self.op}({arg_repr},{kwargs_repr})"
+        )
+
 
 class ActionObjectPointer:
     pass
 
 
 # Hooks
 HOOK_ALWAYS = "ALWAYS"
+HOOK_ON_POINTERS = "ON_POINTERS"
 
 passthrough_attrs = [
     "__dict__",  # python
     "__class__",  # python
     "__repr_name__",  # python
     "__annotations__",  # python
     "_init_private_attributes",  # pydantic
@@ -180,15 +218,17 @@
             The action generated by the current hook
     """
 
     obj: Any
     op_name: str
     node_uid: Optional[UID]
     result_id: Optional[Union[UID, LineageID]]
+    result_twin_type: Optional[TwinMode]
     action: Optional[Action]
+    action_type: Optional[ActionType]
 
 
 def make_action_side_effect(
     context: PreHookContext, *args: List[Any, ...], **kwargs: Dict[str, Any]
 ) -> Result[Ok[Tuple[PreHookContext, Tuple[Any, ...], Dict[str, Any]]], Err[str]]:
     """Create a new action from context_op_name, and add it to the PreHookContext
 
@@ -199,24 +239,49 @@
             Operation *args
         **kwargs
             Operation *kwargs
     Returns:
         - Ok[[Tuple[PreHookContext, Tuple[Any, ...], Dict[str, Any]]] on success
         - Err[str] on failure
     """
+    # relative
+
     try:
-        action = context.obj.syft_make_method_action(
-            op=context.op_name, args=args, kwargs=kwargs
+        action = context.obj.syft_make_action_with_self(
+            op=context.op_name,
+            args=args,
+            kwargs=kwargs,
+            action_type=context.action_type,
         )
         context.action = action
     except Exception:
+        print(f"make_action_side_effect failed with {traceback.format_exc()}")
         return Err(f"make_action_side_effect failed with {traceback.format_exc()}")
     return Ok((context, args, kwargs))
 
 
+class TraceResult:
+    result = []
+    _client = None
+
+    @classmethod
+    def reset(cls):
+        cls.result = []
+        cls._client = None
+
+
+def trace_action_side_effect(
+    context: PreHookContext, *args: Any, **kwargs: Any
+) -> Result[Ok[Tuple[PreHookContext, Tuple[Any, ...], Dict[str, Any]]], Err[str]]:
+    action = context.action
+    if action is not None:
+        TraceResult.result += [action]
+    return Ok((context, args, kwargs))
+
+
 def convert_to_pointers(
     api: SyftAPI,
     node_uid: Optional[UID] = None,
     args: Optional[List] = None,
     kwargs: Optional[Dict] = None,
 ) -> Tuple[List, Dict]:
     arg_list = []
@@ -241,41 +306,38 @@
                 # arg = action_obj.send(client)
 
             kwarg_dict[k] = arg
 
     return arg_list, kwarg_dict
 
 
-def send_action_side_effect(context: PreHookContext, *args: Any, **kwargs: Any) -> Any:
+def send_action_side_effect(
+    context: PreHookContext, *args: Any, **kwargs: Any
+) -> Result[Ok[Tuple[PreHookContext, Tuple[Any, ...], Dict[str, Any]]], Err[str]]:
+    """Create a new action from the context.op_name, and execute it on the remote node."""
     try:
-        if context.op_name not in dont_make_side_effects and hasattr(
-            context.obj, "syft_node_uid"
-        ):
-            if getattr(context.obj, "syft_node_uid", None):
-                if context.action is not None:
-                    action = context.obj.syft_make_method_action(
-                        op=context.op_name, args=args, kwargs=kwargs
-                    )
-                    context.action = action
-
-        result = make_action_side_effect(context, *args, **kwargs)
-        if result.is_err():
-            raise RuntimeError(result.err())
+        if context.action is None:
+            result = make_action_side_effect(context, *args, **kwargs)
+            if result.is_err():
+                raise RuntimeError(result.err())
 
-        context, _, _ = result.ok()
+            context, _, _ = result.ok()
 
         action_result = context.obj.syft_execute_action(context.action, sync=True)
 
         if not isinstance(action_result, ActionObject):
             raise RuntimeError(f"Got back unexpected response : {action_result}")
         else:
             context.node_uid = action_result.syft_node_uid
-            context.result_id = context.action.result_id
-    except Exception:
-        return Err(f"send_action_side_effect failed with {traceback.format_exc()}")
+            context.result_id = action_result.id
+            context.result_twin_type = action_result.syft_twin_type
+    except Exception as e:
+        return Err(
+            f"send_action_side_effect failed with {e}\n {traceback.format_exc()}"
+        )
     return Ok((context, args, kwargs))
 
 
 def propagate_node_uid(
     context: PreHookContext, op: str, result: Any
 ) -> Result[Ok[Any], Err[str]]:
     """Patch the result to include the syft_node_uid
@@ -326,14 +388,27 @@
         if hasattr(value, "syft_action_data"):
             value = value.syft_action_data
         filtered_kwargs[k] = a
 
     return tuple(filtered_args), filtered_kwargs
 
 
+BASE_PASSTHROUGH_ATTRS = [
+    "is_mock",
+    "is_real",
+    "is_twin",
+    "is_pointer",
+    "request",
+    "__repr__",
+    "_repr_markdown_",
+    "syft_twin_type",
+    "_repr_debug_",
+]
+
+
 class ActionObject(SyftObject):
     """Action object for remote execution."""
 
     __canonical_name__ = "ActionObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     __attr_searchable__: List[str] = []
@@ -346,25 +421,44 @@
     syft_parent_args: Optional[Any]
     syft_parent_kwargs: Optional[Any]
     syft_history_hash: Optional[int]
     syft_internal_type: ClassVar[Type[Any]]
     syft_node_uid: Optional[UID]
     _syft_pre_hooks__: Dict[str, List] = {}
     _syft_post_hooks__: Dict[str, List] = {}
+    syft_twin_type: TwinMode = TwinMode.NONE
+    syft_passthrough_attrs = BASE_PASSTHROUGH_ATTRS
+    # syft_dont_wrap_attrs = ["shape"]
+
+    @property
+    def is_pointer(self) -> bool:
+        return self.syft_node_uid is not None
 
     @property
     def syft_lineage_id(self) -> LineageID:
         """Compute the LineageID of the ActionObject, using the `id` and the `syft_history_hash` memebers"""
         return LineageID(self.id, self.syft_history_hash)
 
     @pydantic.validator("id", pre=True, always=True)
     def make_id(cls, v: Optional[UID]) -> UID:
         """Generate or reuse an UID"""
         return Action.make_id(v)
 
+    @property
+    def is_mock(self):
+        return self.syft_twin_type == TwinMode.MOCK
+
+    @property
+    def is_real(self):
+        return self.syft_twin_type == TwinMode.PRIVATE
+
+    @property
+    def is_twin(self):
+        return self.syft_twin_type != TwinMode.NONE
+
     @pydantic.validator("syft_action_data", pre=True, always=True)
     def check_action_data(
         cls, v: ActionObject.syft_pointer_type
     ) -> ActionObject.syft_pointer_type:
         if cls == AnyActionObject or isinstance(
             v, (cls.syft_internal_type, ActionDataEmpty)
         ):
@@ -416,23 +510,64 @@
 
         kwargs = {"action": action}
         api_call = SyftAPICall(
             node_uid=self.syft_node_uid, path="action.execute", args=[], kwargs=kwargs
         )
         return api.make_call(api_call)
 
+    def request(self, client):
+        # relative
+        from ..request.request import ActionStoreChange
+        from ..request.request import SubmitRequest
+
+        action_object_link = LinkedObject.from_obj(self, node_uid=self.syft_node_uid)
+        permission_change = ActionStoreChange(
+            linked_obj=action_object_link, apply_permission_type=ActionPermission.READ
+        )
+
+        submit_request = SubmitRequest(
+            changes=[permission_change],
+            requesting_user_verify_key=client.credentials.verify_key,
+        )
+        return client.api.services.request.submit(submit_request)
+
     def _syft_try_to_save_to_store(self, obj) -> None:
         if self.syft_node_uid is None:
             return
+        elif obj.syft_node_uid is not None:
+            return
+        # TODO fix: the APIRegistry often gets the wrong client
+        # if you have 2 clients in memory
+        # therefore the following happens if you call a method
+        # with a pointer to a twin (mock version)
+        # 1) it gets the wrong credentials
+        # 2) it uses the mock version to overwrite the real version
+        # 3) it shouldnt send in the first place as it already exists
 
         # relative
         from ...client.api import APIRegistry
 
-        api = APIRegistry.api_for(node_uid=self.syft_node_uid)
-        api.services.action.set(obj)
+        action = Action(
+            path="",
+            op="",
+            remote_self=None,
+            result_id=obj.id,
+            args=[],
+            kwargs=dict(),
+            action_type=ActionType.CREATEOBJECT,
+            create_object=obj,
+        )
+
+        if TraceResult._client is not None:
+            api = TraceResult._client.api
+            TraceResult.result += [action]
+        else:
+            api = APIRegistry.api_for(node_uid=self.syft_node_uid)
+
+        api.services.action.execute(action)
 
     def _syft_prepare_obj_uid(self, obj) -> LineageID:
         # We got the UID
         if isinstance(obj, (UID, LineageID)):
             return LineageID(obj.id)
 
         # We got the ActionObjectPointer
@@ -460,14 +595,15 @@
         remote_self: Optional[Union[UID, LineageID]] = None,
         args: Optional[
             List[Union[UID, LineageID, ActionObjectPointer, ActionObject, Any]]
         ] = [],
         kwargs: Optional[
             Dict[str, Union[UID, LineageID, ActionObjectPointer, ActionObject, Any]]
         ] = {},
+        action_type: Optional[ActionType] = None,
     ) -> Action:
         """Generate new action from the information
 
         Parameters:
             path: str
                 The path of the Type of the remote object.
             op: str
@@ -487,31 +623,33 @@
         """
         arg_ids = []
         kwarg_ids = {}
 
         for obj in args:
             arg_ids.append(self._syft_prepare_obj_uid(obj))
 
-        for k, uid in kwargs.items():
+        for k, obj in kwargs.items():
             kwarg_ids[k] = self._syft_prepare_obj_uid(obj)
 
         action = Action(
             path=path,
             op=op,
             remote_self=LineageID(remote_self),
             args=arg_ids,
             kwargs=kwarg_ids,
+            action_type=action_type,
         )
         return action
 
-    def syft_make_method_action(
+    def syft_make_action_with_self(
         self,
         op: str,
         args: Optional[List[Union[UID, ActionObjectPointer]]] = None,
         kwargs: Optional[Dict[str, Union[UID, ActionObjectPointer]]] = None,
+        action_type: Optional[ActionType] = None,
     ) -> Action:
         """Generate new method action from the current object.
 
         Parameters:
             op: str
                 The method to be executed from the remote object.
             args: List[LineageID]
@@ -523,15 +661,20 @@
 
         Raises:
             ValueError: For invalid args or kwargs
             PydanticValidationError: For args and kwargs
         """
         path = self.syft_get_path()
         return self.syft_make_action(
-            path=path, op=op, remote_self=self.syft_lineage_id, args=args, kwargs=kwargs
+            path=path,
+            op=op,
+            remote_self=self.syft_lineage_id,
+            args=args,
+            kwargs=kwargs,
+            action_type=action_type,
         )
 
     def syft_get_path(self) -> str:
         """Get the type path of the underlying object"""
         if isinstance(self, AnyActionObject) and self.syft_internal_type:
             return f"{type(self.syft_action_data).__name__}"  # avoids AnyActionObject errors
         return f"{type(self).__name__}"
@@ -550,27 +693,30 @@
             A function
         """
 
         def wrapper(
             *args: Optional[List[Union[UID, ActionObjectPointer]]],
             **kwargs: Optional[Dict[str, Union[UID, ActionObjectPointer]]],
         ) -> Action:
-            return self.syft_make_method_action(op=op, args=args, kwargs=kwargs)
+            return self.syft_make_action_with_self(op=op, args=args, kwargs=kwargs)
 
         return wrapper
 
     def send(self, client: SyftClient) -> Self:
         """Send the object to a Syft Client"""
 
         return client.api.services.action.set(self)
 
     def get_from(self, client: SyftClient) -> Any:
         """Get the object from a Syft Client"""
-
-        return client.api.services.action.get(self.id).syft_action_data
+        res = client.api.services.action.get(self.id)
+        if not isinstance(res, ActionObject):
+            return Err(res)
+        else:
+            return res.syft_action_data
 
     @staticmethod
     def from_obj(
         syft_action_data: Any,
         id: Optional[UID] = None,
         syft_lineage_id: Optional[LineageID] = None,
     ) -> ActionObject:
@@ -583,28 +729,39 @@
                 Which ID to use for the ActionObject. Optional
             syft_lineage_id: Optional[LineageID]
                 Which LineageID to use for the ActionObject. Optional
         """
         if id and syft_lineage_id and id != syft_lineage_id.id:
             raise ValueError("UID and LineageID should match")
 
-        action_type = action_type_for_type(syft_action_data)
+        action_type = action_type_for_object(syft_action_data)
         action_object = action_type(syft_action_data=syft_action_data)
 
         if id:
             action_object.id = id
 
         if syft_lineage_id:
             action_object.id = syft_lineage_id.id
             action_object.syft_history_hash = syft_lineage_id.syft_history_hash
         elif id:
             action_object.syft_history_hash = hash(id)
 
         return action_object
 
+    @classmethod
+    def add_trace_hook(cls):
+        return True
+        # if trace_action_side_effect not in self._syft_pre_hooks__[HOOK_ALWAYS]:
+        #     self._syft_pre_hooks__[HOOK_ALWAYS].append(trace_action_side_effect)
+
+    @classmethod
+    def remove_trace_hook(cls):
+        return True
+        # self._syft_pre_hooks__[HOOK_ALWAYS].pop(trace_action_side_effct, None)
+
     @staticmethod
     def empty(
         syft_internal_type: Any = Any,
         id: Optional[UID] = None,
         syft_lineage_id: Optional[LineageID] = None,
     ) -> ActionObject:
         """Create an ActionObject from a type, using a ActionDataEmpty object
@@ -615,31 +772,46 @@
             id: Optional[UID]
                 Which ID to use for the ActionObject. Optional
             syft_lineage_id: Optional[LineageID]
                 Which LineageID to use for the ActionObject. Optional
         """
 
         empty = ActionDataEmpty(syft_internal_type=syft_internal_type)
-        return ActionObject.from_obj(
+        res = ActionObject.from_obj(
             syft_action_data=empty, id=id, syft_lineage_id=syft_lineage_id
         )
+        res.__dict__["syft_internal_type"] = syft_internal_type
+        return res
 
     def __post_init__(self) -> None:
         """Add pre/post hooks."""
         if HOOK_ALWAYS not in self._syft_pre_hooks__:
             self._syft_pre_hooks__[HOOK_ALWAYS] = []
 
+        if HOOK_ON_POINTERS not in self._syft_post_hooks__:
+            self._syft_pre_hooks__[HOOK_ON_POINTERS] = []
+
         # this should be a list as orders matters
-        for side_effect in [make_action_side_effect, send_action_side_effect]:
+        for side_effect in [make_action_side_effect]:
             if side_effect not in self._syft_pre_hooks__[HOOK_ALWAYS]:
                 self._syft_pre_hooks__[HOOK_ALWAYS].append(side_effect)
 
+        for side_effect in [send_action_side_effect]:
+            if side_effect not in self._syft_pre_hooks__[HOOK_ON_POINTERS]:
+                self._syft_pre_hooks__[HOOK_ON_POINTERS].append(side_effect)
+
+        if trace_action_side_effect not in self._syft_pre_hooks__[HOOK_ALWAYS]:
+            self._syft_pre_hooks__[HOOK_ALWAYS].append(trace_action_side_effect)
+
         if HOOK_ALWAYS not in self._syft_post_hooks__:
             self._syft_post_hooks__[HOOK_ALWAYS] = []
 
+        if HOOK_ON_POINTERS not in self._syft_post_hooks__:
+            self._syft_post_hooks__[HOOK_ON_POINTERS] = []
+
         for side_effect in [propagate_node_uid]:
             if side_effect not in self._syft_post_hooks__[HOOK_ALWAYS]:
                 self._syft_post_hooks__[HOOK_ALWAYS].append(side_effect)
 
         if isinstance(self.syft_action_data, ActionObject):
             raise Exception("Nested ActionObjects", self.syft_action_data)
 
@@ -653,23 +825,34 @@
         if name in self._syft_pre_hooks__:
             for hook in self._syft_pre_hooks__[name]:
                 result = hook(context, *result_args, **result_kwargs)
                 if result.is_ok():
                     context, result_args, result_kwargs = result.ok()
                 else:
                     debug(f"Pre-hook failed with {result.err()}")
-
         if name not in self._syft_dont_wrap_attrs():
             if HOOK_ALWAYS in self._syft_pre_hooks__:
                 for hook in self._syft_pre_hooks__[HOOK_ALWAYS]:
                     result = hook(context, *result_args, **result_kwargs)
                     if result.is_ok():
                         context, result_args, result_kwargs = result.ok()
                     else:
-                        debug(f"Pre-hook failed with {result.err()}")
+                        msg = result.err().replace("\\n", "\n")
+                        print(f"Pre-hook failed with {msg}")
+
+        if self.is_pointer:
+            if name not in self._syft_dont_wrap_attrs():
+                if HOOK_ALWAYS in self._syft_pre_hooks__:
+                    for hook in self._syft_pre_hooks__[HOOK_ON_POINTERS]:
+                        result = hook(context, *result_args, **result_kwargs)
+                        if result.is_ok():
+                            context, result_args, result_kwargs = result.ok()
+                        else:
+                            msg = result.err().replace("\\n", "\n")
+                            print(f"Pre-hook failed with {msg}")
 
         return context, result_args, result_kwargs
 
     def _syft_run_post_hooks__(
         self, context: PreHookContext, name: str, result: Any
     ) -> Any:
         """Hooks executed after the actual call"""
@@ -687,26 +870,38 @@
                 for hook in self._syft_post_hooks__[HOOK_ALWAYS]:
                     result = hook(context, name, new_result)
                     if result.is_ok():
                         new_result = result.ok()
                     else:
                         debug(f"Post hook failed with {result.err()}")
 
+        if self.is_pointer:
+            if name not in self._syft_dont_wrap_attrs():
+                if HOOK_ALWAYS in self._syft_post_hooks__:
+                    for hook in self._syft_post_hooks__[HOOK_ON_POINTERS]:
+                        result = hook(context, name, new_result)
+                        if result.is_ok():
+                            new_result = result.ok()
+                        else:
+                            debug(f"Post hook failed with {result.err()}")
+
         return new_result
 
     def _syft_output_action_object(
-        self,
-        result: Any,
+        self, result: Any, context: Optional[PreHookContext] = None
     ) -> Any:
         """Wrap the result in an ActionObject"""
         if issubclass(type(result), ActionObject):
             return result
 
         constructor = action_type_for_type(result)
-        result = constructor(syft_action_data=result)
+        syft_twin_type = TwinMode.NONE
+        if context.result_twin_type is not None:
+            syft_twin_type = context.result_twin_type
+        result = constructor(syft_action_data=result, syft_twin_type=syft_twin_type)
 
         return result
 
     def _syft_passthrough_attrs(self) -> List[str]:
         """These attributes are forwarded to the `object` base class."""
         return passthrough_attrs + getattr(self, "syft_passthrough_attrs", [])
 
@@ -729,15 +924,15 @@
 
     def _syft_attr_propagate_ids(self, context, name: str, result: Any) -> Any:
         """Patch the results with the syft_history_hash, node_uid, and result_id."""
         if name in self._syft_dont_wrap_attrs():
             return result
 
         # Wrap as Syft Object
-        result = self._syft_output_action_object(result)
+        result = self._syft_output_action_object(result, context)
 
         # Propagate History
         if context.action is not None:
             result.syft_history_hash = context.action.syft_history_hash
 
         # Propagate Syft Node UID
         result.syft_node_uid = context.node_uid
@@ -779,15 +974,17 @@
 
         if not self.syft_is_property(context_self, name):
             raise RuntimeError(
                 "[_wrap_attribute_for_properties] Use this only on properties"
             )
         debug(f"[__getattribute__] Handling property {name} ")
 
-        context = PreHookContext(obj=self, op_name=name)
+        context = PreHookContext(
+            obj=self, op_name=name, action_type=ActionType.GETATTRIBUTE
+        )
         context, _, _ = self._syft_run_pre_hooks__(context, name, (), {})
         # no input needs to propagate
         result = self._syft_run_post_hooks__(
             context, name, self.syft_get_property(context_self, name)
         )
 
         return self._syft_attr_propagate_ids(context, name, result)
@@ -807,15 +1004,17 @@
             original_func = fake_func
         else:
             original_func = getattr(self.syft_action_data, name)
 
         debug_original_func(name, original_func)
 
         def _base_wrapper(*args: Any, **kwargs: Any) -> Any:
-            context = PreHookContext(obj=self, op_name=name)
+            context = PreHookContext(
+                obj=self, op_name=name, action_type=ActionType.METHOD
+            )
             context, pre_hook_args, pre_hook_kwargs = self._syft_run_pre_hooks__(
                 context, name, args, kwargs
             )
 
             if has_action_data_empty(args=args, kwargs=kwargs):
                 result = fake_func(*args, **kwargs)
             else:
@@ -852,14 +1051,45 @@
                 original_func
             )
         except Exception:
             debug("name", name, "has no signature")
 
         return wrapper
 
+    def _syft_setattr(self, name, value):
+        args = (name, value)
+        kwargs = dict()
+        op_name = "__setattr__"
+
+        def fake_func(*args: Any, **kwargs: Any) -> Any:
+            return ActionDataEmpty(syft_internal_type=self.syft_internal_type)
+
+        if isinstance(self.syft_action_data, ActionDataEmpty) or has_action_data_empty(
+            args=args, kwargs=kwargs
+        ):
+            local_func = fake_func
+        else:
+            local_func = getattr(self.syft_action_data, op_name)
+
+        context = PreHookContext(
+            obj=self, op_name=op_name, action_type=ActionType.SETATTRIBUTE
+        )
+        context, pre_hook_args, pre_hook_kwargs = self._syft_run_pre_hooks__(
+            context, "__setattr__", args, kwargs
+        )
+
+        original_args, _ = debox_args_and_kwargs(pre_hook_args, pre_hook_kwargs)
+        val = original_args[1]
+        local_func(name, val)
+        local_result = self
+
+        post_result = self._syft_run_post_hooks__(context, op_name, local_result)
+        post_result = self._syft_attr_propagate_ids(context, op_name, post_result)
+        return post_result
+
     def __getattribute__(self, name: str) -> Any:
         """Called unconditionally to implement attribute accesses for instances of the class.
         If the class also defines __getattr__(), the latter will not be called unless __getattribute__()
         either calls it explicitly or raises an AttributeError.
         This method should return the (computed) attribute value or raise an AttributeError exception.
         In order to avoid infinite recursion in this method, its implementation should always:
          * call the base class method with the same name to access any attributes it needs
@@ -871,14 +1101,15 @@
             name: str
                 The name of the attribute to access.
         """
         # bypass certain attrs to prevent recursion issues
         if name.startswith("_syft") or name.startswith("syft"):
             return object.__getattribute__(self, name)
 
+        # third party
         if name in self._syft_passthrough_attrs():
             return object.__getattribute__(self, name)
         context_self = self._syft_get_attr_context(name)
 
         # Handle bool operator on nonbools
         if name == "__bool__" and not hasattr(self.syft_action_data, "__bool__"):
             return self._syft_wrap_attribute_for_bool_on_nonbools(name)
@@ -896,28 +1127,52 @@
         debug(">> ", name, ", defined_on_self = ", defined_on_self)
 
         # use the custom defined version
         if defined_on_self:
             self.__dict__[name] = value
             return value
         else:
+            self._syft_setattr(name, value)
             context_self = self.syft_action_data  # type: ignore
             return context_self.__setattr__(name, value)
 
     def keys(self) -> KeysView[str]:
         return self.syft_action_data.keys()  # type: ignore
 
     ###### __DUNDER_MIFFLIN__
 
     # if we do not implement these boiler plate __method__'s then special infix
     # operations like x + y won't trigger __getattribute__
     # unless there is a super special reason we should write no code in these functions
+    def _repr_markdown_(self) -> str:
+        if self.is_mock:
+            res = "TwinPointer(Mock)"
+        elif self.is_real:
+            res = "TwinPointer(Real)"
+        elif not self.is_twin:
+            res = "Pointer"
+        child_repr = (
+            self.syft_action_data._repr_markdown_()
+            if hasattr(self.syft_action_data, "_repr_markdown_")
+            else self.syft_action_data.__repr__()
+        )
+
+        return f"```python\n{res}\n```\n{child_repr}"
 
     def __repr__(self) -> str:
-        return self.__repr__()
+        if self.is_mock:
+            res = "TwinPointer(Mock)"
+        elif self.is_real:
+            res = "TwinPointer(Real)"
+        if not self.is_twin:
+            res = "Pointer"
+        return f"{res}:\n{str(self.syft_action_data)}"
+
+    def __call__(self, *args: Any, **kwds: Any) -> Any:
+        return self.__call__(*args, **kwds)
 
     def __str__(self) -> str:
         return self.__str__()
 
     def __len__(self) -> int:
         return self.__len__()
 
@@ -1064,15 +1319,15 @@
 
 @serializable()
 class AnyActionObject(ActionObject):
     __canonical_name__ = "AnyActionObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     syft_internal_type: ClassVar[Type[Any]] = Any  # type: ignore
-    syft_passthrough_attrs: List[str] = []
+    # syft_passthrough_attrs: List[str] = []
     syft_dont_wrap_attrs: List[str] = []
 
     def __float__(self) -> float:
         return float(self.syft_action_data)
 
     def __int__(self) -> float:
         return int(self.syft_action_data)
```

### Comparing `syft-0.8.1b1/src/syft/service/action/action_permissions.py` & `syft-0.8.1b2/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/action/action_service.py` & `syft-0.8.1b2/src/syft/service/action/action_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # stdlib
-from enum import Enum
 import importlib
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Union
 
 # third party
@@ -26,30 +25,26 @@
 from ..service import TYPE_TO_SERVICE
 from ..service import UserLibConfigRegistry
 from ..service import service_method
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from .action_object import Action
 from .action_object import ActionObject
 from .action_object import ActionObjectPointer
+from .action_object import ActionType
 from .action_object import AnyActionObject
+from .action_object import TwinMode
+from .action_permissions import ActionObjectREAD
 from .action_store import ActionStore
 from .action_types import action_type_for_type
 from .numpy import NumpyArrayObject
 from .pandas import PandasDataFrameObject  # noqa: F401
 from .pandas import PandasSeriesObject  # noqa: F401
 
 
 @serializable()
-class TwinMode(Enum):
-    NONE = 0
-    PRIVATE = 1
-    MOCK = 2
-
-
-@serializable()
 class ActionService(AbstractService):
     def __init__(self, store: ActionStore) -> None:
         self.store = store
 
     @service_method(path="action.np_array", name="np_array")
     def np_array(self, context: AuthedServiceContext, data: Any) -> Any:
         if not isinstance(data, np.ndarray):
@@ -101,31 +96,43 @@
     def get(
         self,
         context: AuthedServiceContext,
         uid: UID,
         twin_mode: TwinMode = TwinMode.PRIVATE,
     ) -> Result[Ok[ActionObject], Err[str]]:
         """Get an object from the action store"""
+        return self._get(context, uid, twin_mode)
+
+    def _get(
+        self,
+        context: AuthedServiceContext,
+        uid: UID,
+        twin_mode: TwinMode = TwinMode.PRIVATE,
+        has_permission=False,
+    ) -> Result[ActionObject, str]:
         # TODO 🟣 Temporarily added skip permission arguments for enclave
         # until permissions are fully integrated
-        result = self.store.get(uid=uid, credentials=context.credentials)
+        result = self.store.get(
+            uid=uid, credentials=context.credentials, has_permission=has_permission
+        )
         if result.is_ok():
             obj = result.ok()
             if isinstance(obj, TwinObject):
                 if twin_mode == TwinMode.PRIVATE:
                     obj = obj.private
                     obj.syft_point_to(context.node.id)
                 elif twin_mode == TwinMode.MOCK:
                     obj = obj.mock
                     obj.syft_point_to(context.node.id)
                 else:
                     obj.mock.syft_point_to(context.node.id)
                     obj.private.syft_point_to(context.node.id)
             return Ok(obj)
-        return result
+        else:
+            return result
 
     @service_method(
         path="action.get_pointer", name="get_pointer", roles=GUEST_ROLE_LEVEL
     )
     def get_pointer(
         self, context: AuthedServiceContext, uid: UID
     ) -> Result[ActionObjectPointer, str]:
@@ -164,31 +171,29 @@
         try:
             if not has_twin_inputs:
                 # no twins
                 filtered_kwargs = filter_twin_kwargs(
                     real_kwargs, twin_mode=TwinMode.NONE
                 )
                 exec_result = execute_byte_code(code_item, filtered_kwargs)
-                result_action_object = wrap_result(
-                    code_item.id, result_id, exec_result.result
-                )
+                result_action_object = wrap_result(result_id, exec_result.result)
             else:
                 # twins
                 private_kwargs = filter_twin_kwargs(
                     real_kwargs, twin_mode=TwinMode.PRIVATE
                 )
                 private_exec_result = execute_byte_code(code_item, private_kwargs)
                 result_action_object_private = wrap_result(
-                    code_item.id, result_id, private_exec_result.result
+                    result_id, private_exec_result.result
                 )
 
                 mock_kwargs = filter_twin_kwargs(real_kwargs, twin_mode=TwinMode.MOCK)
                 mock_exec_result = execute_byte_code(code_item, mock_kwargs)
                 result_action_object_mock = wrap_result(
-                    code_item.id, result_id, mock_exec_result.result
+                    result_id, mock_exec_result.result
                 )
 
                 result_action_object = TwinObject(
                     id=result_id,
                     private_obj=result_action_object_private,
                     mock_obj=result_action_object_mock,
                 )
@@ -200,131 +205,319 @@
             credentials=context.credentials,
             syft_object=result_action_object,
         )
         if set_result.is_err():
             return set_result.err()
         return Ok(result_action_object)
 
+    def execute_plan(
+        self, plan, context: AuthedServiceContext, plan_kwargs: Dict[str, ActionObject]
+    ):
+        id2inpkey = {v.id: k for k, v in plan.inputs.items()}
+
+        for plan_action in plan.actions:
+            if (
+                hasattr(plan_action.remote_self, "id")
+                and plan_action.remote_self.id in id2inpkey
+            ):
+                plan_action.remote_self = plan_kwargs[
+                    id2inpkey[plan_action.remote_self.id]
+                ]
+            for i, arg in enumerate(plan_action.args):
+                if arg in id2inpkey:
+                    plan_action.args[i] = plan_kwargs[id2inpkey[arg]]
+
+            for k, arg in enumerate(plan_action.kwargs):
+                if arg in id2inpkey:
+                    plan_action.kwargs[k] = plan_kwargs[id2inpkey[arg]]
+
+        for plan_action in plan.actions:
+            action_res = self.execute(context, plan_action)
+            if action_res.is_err():
+                return action_res
+        result_id = plan.outputs[0].id
+        return self._get(context, result_id, TwinMode.MOCK, has_permission=True)
+
+    def call_function(self, context: AuthedServiceContext, action: Action):
+        # run function/class init
+        _user_lib_config_registry = UserLibConfigRegistry.from_user(context.credentials)
+        absolute_path = f"{action.path}.{action.op}"
+        if absolute_path in _user_lib_config_registry:
+            # TODO: implement properly
+            # Now we are assuming its a function/class
+            return execute_callable(self, context, action)
+        else:
+            return Err(
+                f"Failed executing {action}. You have no permission for {absolute_path}"
+            )
+
+    def set_attribute(
+        self,
+        context: AuthedServiceContext,
+        action: Action,
+        resolved_self: Union[ActionObject, TwinObject],
+    ):
+        args, _ = resolve_action_args(action, context, self)
+        if args.is_err():
+            return Err(
+                f"Failed executing action {action}, could not resolve args: {args.err()}"
+            )
+        else:
+            args = args.ok()
+        if not isinstance(args[0], ActionObject):
+            return Err(
+                f"Failed executing action {action} setattribute requires a non-twin string as first argument"
+            )
+        name = args[0].syft_action_data
+        # dont do the whole filtering dance with the name
+        args = [args[1]]
+
+        if isinstance(resolved_self, TwinObject):
+            # todo, create copy?
+            private_args = filter_twin_args(args, twin_mode=TwinMode.PRIVATE)
+            private_val = private_args[0]
+            setattr(resolved_self.private.syft_action_data, name, private_val)
+            # todo: what do we use as data for the mock here?
+            # depending on permisisons?
+            public_args = filter_twin_args(args, twin_mode=TwinMode.MOCK)
+            public_val = public_args[0]
+            setattr(resolved_self.mock.syft_action_data, name, public_val)
+            return Ok(
+                TwinObject(
+                    id=action.result_id,
+                    private_obj=ActionObject.from_obj(
+                        resolved_self.private.syft_action_data
+                    ),
+                    private_obj_id=action.result_id,
+                    mock_obj=ActionObject.from_obj(resolved_self.mock.syft_action_data),
+                    mock_obj_id=action.result_id,
+                )
+            )
+        else:
+            # TODO: Implement for twinobject args
+            args = filter_twin_args(args, twin_mode=TwinMode.NONE)
+            val = args[0]
+            setattr(resolved_self.syft_action_data, name, val)
+            return Ok(
+                ActionObject.from_obj(resolved_self.syft_action_data),
+            )
+            # todo: permissions
+            # setattr(resolved_self.syft_action_data, name, val)
+            # val = resolved_self.syft_action_data
+            # result_action_object = Ok(wrap_result(action.result_id, val))
+
+    def get_attribute(
+        self, action: Action, resolved_self: Union[ActionObject, TwinObject]
+    ):
+        if isinstance(resolved_self, TwinObject):
+            private_result = getattr(resolved_self.private.syft_action_data, action.op)
+            mock_result = getattr(resolved_self.mock.syft_action_data, action.op)
+            return Ok(
+                TwinObject(
+                    id=action.result_id,
+                    private_obj=ActionObject.from_obj(private_result),
+                    private_obj_id=action.result_id,
+                    mock_obj=ActionObject.from_obj(mock_result),
+                    mock_obj_id=action.result_id,
+                )
+            )
+        else:
+            val = getattr(resolved_self.syft_action_data, action.op)
+            return Ok(wrap_result(action.result_id, val))
+
+    def call_method(
+        self,
+        context: AuthedServiceContext,
+        action: Action,
+        resolved_self: Union[ActionObject, TwinObject],
+    ):
+        if isinstance(resolved_self, TwinObject):
+            # method
+            private_result = execute_object(
+                self,
+                context,
+                resolved_self.private,
+                action,
+                twin_mode=TwinMode.PRIVATE,
+            )
+            if private_result.is_err():
+                return Err(
+                    f"Failed executing action {action}, result is an error: {private_result.err()}"
+                )
+            mock_result = execute_object(
+                self, context, resolved_self.mock, action, twin_mode=TwinMode.MOCK
+            )
+            if mock_result.is_err():
+                return Err(
+                    f"Failed executing action {action}, result is an error: {mock_result.err()}"
+                )
+
+            private_result = private_result.ok()
+            mock_result = mock_result.ok()
+
+            return Ok(
+                TwinObject(
+                    id=action.result_id,
+                    private_obj=private_result,
+                    private_obj_id=action.result_id,
+                    mock_obj=mock_result,
+                    mock_obj_id=action.result_id,
+                )
+            )
+        else:
+            return execute_object(self, context, resolved_self, action)
+
     @service_method(path="action.execute", name="execute", roles=GUEST_ROLE_LEVEL)
     def execute(
         self, context: AuthedServiceContext, action: Action
-    ) -> Result[ActionObjectPointer, Err]:
+    ) -> Result[ActionObject, Err]:
         """Execute an operation on objects in the action store"""
+        # relative
+        from .plan import Plan
 
-        if action.remote_self is None:
-            _user_lib_config_registry = UserLibConfigRegistry.from_user(
-                context.credentials
-            )
-            absolute_path = f"{action.path}.{action.op}"
-            if absolute_path in _user_lib_config_registry:
-                # TODO: implement properly
-                # Now we are assuming its a function/class
-                result_action_object = execute_callable(self, context, action)
-            else:
-                return Err(f"You have no permission for {absolute_path}")
+        if action.action_type == ActionType.CREATEOBJECT:
+            result_action_object = Ok(action.create_object)
+        elif action.action_type == ActionType.FUNCTION:
+            result_action_object = self.call_function(context, action)
         else:
-            resolved_self = self.get(
-                context=context, uid=action.remote_self, twin_mode=TwinMode.NONE
+            resolved_self = self._get(
+                context=context,
+                uid=action.remote_self,
+                twin_mode=TwinMode.NONE,
+                has_permission=True,
             )
             if resolved_self.is_err():
-                return resolved_self.err()
-            resolved_self = resolved_self.ok()
-
-            if isinstance(resolved_self, TwinObject):
-                private_result = execute_object(
-                    self,
-                    context,
-                    resolved_self.private,
-                    action,
-                    twin_mode=TwinMode.PRIVATE,
-                )
-                if private_result.is_err():
-                    return private_result.err()
-                mock_result = execute_object(
-                    self, context, resolved_self.mock, action, twin_mode=TwinMode.MOCK
-                )
-                if mock_result.is_err():
-                    return mock_result.err()
-
-                private_result = private_result.ok()
-                mock_result = mock_result.ok()
-
-                result_action_object = Ok(
-                    TwinObject(
-                        id=action.result_id,
-                        private_obj=private_result,
-                        private_obj_id=action.result_id,
-                        mock_obj=mock_result,
-                        mock_obj_id=action.result_id,
-                    )
+                return Err(
+                    f"Failed executing action {action}, could not resolve self: {resolved_self.err()}"
                 )
+            resolved_self = resolved_self.ok()
+            if action.op == "__call__" and isinstance(
+                resolved_self.syft_action_data, Plan
+            ):
+                result_action_object = self.execute_plan(
+                    plan=resolved_self.syft_action_data,
+                    context=context,
+                    plan_kwargs=action.kwargs,
+                )
+                return result_action_object
+            elif action.action_type == ActionType.SETATTRIBUTE:
+                result_action_object = self.set_attribute(
+                    context, action, resolved_self
+                )
+            elif action.action_type == ActionType.GETATTRIBUTE:
+                result_action_object = self.get_attribute(action, resolved_self)
+            elif action.action_type == ActionType.METHOD:
+                result_action_object = self.call_method(context, action, resolved_self)
             else:
-                result_action_object = execute_object(
-                    self, context, resolved_self, action
-                )
+                return Err("Unknown action")
 
         if result_action_object.is_err():
-            return result_action_object.err()
+            return Err(
+                f"Failed executing action {action}, result is an error: {result_action_object.err()}"
+            )
         else:
             result_action_object = result_action_object.ok()
 
+        # check if we have read permissions on the result
+        has_result_read_permission = self.has_read_permission_for_action_result(
+            context, action
+        )
+
         set_result = self.store.set(
             uid=action.result_id,
             credentials=context.credentials,
             syft_object=result_action_object,
+            has_result_read_permission=has_result_read_permission,
         )
         if set_result.is_err():
-            return set_result.err()
+            return Err(
+                f"Failed executing action {action}, set result is an error: {set_result.err()}"
+            )
 
         if isinstance(result_action_object, TwinObject):
             result_action_object = result_action_object.mock
+            # we patch this on the object, because this is the thing we are getting back
+            result_action_object.id = action.result_id
         result_action_object.syft_point_to(context.node.id)
 
         return Ok(result_action_object)
 
+    def has_read_permission_for_action_result(
+        self, context: AuthedServiceContext, action: Action
+    ) -> bool:
+        action_obj_ids = (
+            action.args + list(action.kwargs.values()) + [action.remote_self]
+        )
+        permissions = [
+            ActionObjectREAD(uid=_id, credentials=context.credentials)
+            for _id in action_obj_ids
+        ]
+        return self.store.has_permissions(permissions)
+
     @service_method(path="action.exists", name="exists", roles=GUEST_ROLE_LEVEL)
     def exists(
         self, context: AuthedServiceContext, obj_id: UID
     ) -> Result[SyftSuccess, SyftError]:
         """Checks if the given object id exists in the Action Store"""
         if self.store.exists(obj_id):
             return SyftSuccess(message=f"Object: {obj_id} exists")
         else:
             return SyftError(message=f"Object: {obj_id} does not exist")
 
 
+def resolve_action_args(
+    action: Action, context: AuthedServiceContext, service: ActionService
+):
+    has_twin_inputs = False
+    args = []
+    for arg_id in action.args:
+        arg_value = service._get(
+            context=context, uid=arg_id, twin_mode=TwinMode.NONE, has_permission=True
+        )
+        if arg_value.is_err():
+            return arg_value, False
+        if isinstance(arg_value.ok(), TwinObject):
+            has_twin_inputs = True
+        args.append(arg_value.ok())
+    return Ok(args), has_twin_inputs
+
+
+def resolve_action_kwargs(
+    action: Action, context: AuthedServiceContext, service: ActionService
+):
+    has_twin_inputs = False
+    kwargs = {}
+    for key, arg_id in action.kwargs.items():
+        kwarg_value = service._get(
+            context=context, uid=arg_id, twin_mode=TwinMode.NONE, has_permission=True
+        )
+        if kwarg_value.is_err():
+            return kwarg_value, False
+        if isinstance(kwarg_value.ok(), TwinObject):
+            has_twin_inputs = True
+        kwargs[key] = kwarg_value.ok()
+    return Ok(kwargs), has_twin_inputs
+
+
 def execute_callable(
     service: ActionService,
     context: AuthedServiceContext,
     action: Action,
 ) -> Result[ActionObject, str]:
-    args = []
-
-    if action.args:
-        for arg_id in action.args:
-            arg_value = service.get(
-                context=context, uid=arg_id, twin_mode=TwinMode.NONE
-            )
-            if arg_value.is_err():
-                return arg_value.err()
-            if isinstance(arg_value.ok(), TwinObject):
-                pass
-            args.append(arg_value.ok())
-
-    kwargs = {}
-    if action.kwargs:
-        for key, arg_id in action.kwargs.items():
-            kwarg_value = service.get(
-                context=context, uid=arg_id, twin_mode=TwinMode.NONE
-            )
-            if kwarg_value.is_err():
-                return kwarg_value.err()
-            if isinstance(kwarg_value.ok(), TwinObject):
-                pass
-            kwargs[key] = kwarg_value.ok()
+    args, has_arg_twins = resolve_action_args(action, context, service)
+    kwargs, has_kwargs_twins = resolve_action_kwargs(action, context, service)
+    has_twin_inputs = has_arg_twins or has_kwargs_twins
+    if args.is_err():
+        return args
+    else:
+        args = args.ok()
+    if kwargs.is_err():
+        return kwargs
+    else:
+        kwargs = kwargs.ok()
 
     # 🔵 TODO 10: Get proper code From old RunClassMethodAction to ensure the function
     # is not bound to the original object or mutated
     # stdlib
 
     # TODO: get from CMPTree is probably safer
     def _get_target_callable(path: str, op: str):
@@ -336,63 +529,42 @@
         return res
 
     target_callable = _get_target_callable(action.path, action.op)
 
     result = None
     try:
         if target_callable:
-            # if twin_mode == TwinMode.NONE and not has_twin_inputs:
-            twin_mode = TwinMode.NONE
-            # no twins
-            filtered_args = filter_twin_args(args, twin_mode=twin_mode)
-            filtered_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
-            result = target_callable(*filtered_args, **filtered_kwargs)
-            result_action_object = wrap_result(action.id, action.result_id, result)
-            # elif twin_mode == TwinMode.NONE and has_twin_inputs:
-            #     # self isn't a twin but one of the inputs is
-            #     private_args = filter_twin_args(args, twin_mode=twin_mode)
-            #     private_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
-            #     private_result = target_method(*private_args, **private_kwargs)
-            #     result_action_object_private = wrap_result(
-            #         action.parent_id, action.result_id, private_result
-            #     )
-
-            #     mock_args = filter_twin_args(args, twin_mode=twin_mode)
-            #     mock_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
-            #     mock_result = target_method(*mock_args, **mock_kwargs)
-            #     result_action_object_mock = wrap_result(
-            #         action.parent_id, action.result_id, mock_result
-            #     )
-
-            #     result_action_object = TwinObject(
-            #         id=action.result_id,
-            #         private_obj=result_action_object_private,
-            #         mock_obj=result_action_object_mock,
-            #     )
-            # elif twin_mode == twin_mode.PRIVATE:  # type: ignore
-            #     # twin private path
-            #     private_args = filter_twin_args(args, twin_mode=twin_mode)
-            #     private_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
-            #     result = target_method(*private_args, **private_kwargs)
-            #     result_action_object = wrap_result(
-            #         action.parent_id, action.result_id, result
-            #     )
-            # elif twin_mode == twin_mode.MOCK:  # type: ignore
-            #     # twin mock path
-            #     mock_args = filter_twin_args(args, twin_mode=twin_mode)
-            #     mock_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
-            #     target_method = getattr(unboxed_resolved_self, action.op, None)
-            #     result = target_method(*mock_args, **mock_kwargs)
-            #     result_action_object = wrap_result(
-            #         action.parent_id, action.result_id, result
-            #     )
-            # else:
-            #     raise Exception(
-            #         f"Bad combination of: twin_mode: {twin_mode} and has_twin_inputs: {has_twin_inputs}"
-            #     )
+            if not has_twin_inputs:
+                # if twin_mode == TwinMode.NONE and not has_twin_inputs:
+                twin_mode = TwinMode.NONE
+                # no twins
+                filtered_args = filter_twin_args(args, twin_mode=twin_mode)
+                filtered_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
+                result = target_callable(*filtered_args, **filtered_kwargs)
+                result_action_object = wrap_result(action.result_id, result)
+            else:
+                twin_mode = TwinMode.PRIVATE
+                private_args = filter_twin_args(args, twin_mode=twin_mode)
+                private_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
+                private_result = target_callable(*private_args, **private_kwargs)
+                result_action_object_private = wrap_result(
+                    action.result_id, private_result
+                )
+
+                twin_mode = TwinMode.MOCK
+                mock_args = filter_twin_args(args, twin_mode=twin_mode)
+                mock_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
+                mock_result = target_callable(*mock_args, **mock_kwargs)
+                result_action_object_mock = wrap_result(action.result_id, mock_result)
+
+                result_action_object = TwinObject(
+                    id=action.result_id,
+                    private_obj=result_action_object_private,
+                    mock_obj=result_action_object_mock,
+                )
 
     except Exception as e:
         print("what is this exception", e)
         return Err(e)
     return Ok(result_action_object)
 
 
@@ -400,108 +572,87 @@
     service: ActionService,
     context: AuthedServiceContext,
     resolved_self: ActionObject,
     action: Action,
     twin_mode: TwinMode = TwinMode.NONE,
 ) -> Result[Ok[Union[TwinObject, ActionObject]], Err[str]]:
     unboxed_resolved_self = resolved_self.syft_action_data
-    args = []
-    has_twin_inputs = False
-    if action.args:
-        for arg_id in action.args:
-            arg_value = service.get(
-                context=context, uid=arg_id, twin_mode=TwinMode.NONE
-            )
-            if arg_value.is_err():
-                return arg_value
-            if isinstance(arg_value.ok(), TwinObject):
-                has_twin_inputs = True
-            args.append(arg_value.ok())
-
-    kwargs = {}
-    if action.kwargs:
-        for key, arg_id in action.kwargs.items():
-            kwarg_value = service.get(
-                context=context, uid=arg_id, twin_mode=TwinMode.NONE
-            )
-            if kwarg_value.is_err():
-                return kwarg_value
-            if isinstance(kwarg_value.ok(), TwinObject):
-                has_twin_inputs = True
-            kwargs[key] = kwarg_value.ok()
+    args, has_arg_twins = resolve_action_args(action, context, service)
+    kwargs, has_kwargs_twins = resolve_action_kwargs(action, context, service)
+    if args.is_err():
+        return args
+    else:
+        args = args.ok()
+    if kwargs.is_err():
+        return kwargs
+    else:
+        kwargs = kwargs.ok()
+    has_twin_inputs = has_arg_twins or has_kwargs_twins
 
     # 🔵 TODO 10: Get proper code From old RunClassMethodAction to ensure the function
     # is not bound to the original object or mutated
     target_method = getattr(unboxed_resolved_self, action.op, None)
     result = None
     try:
         if target_method:
             if twin_mode == TwinMode.NONE and not has_twin_inputs:
                 # no twins
                 filtered_args = filter_twin_args(args, twin_mode=twin_mode)
                 filtered_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
                 result = target_method(*filtered_args, **filtered_kwargs)
-                result_action_object = wrap_result(action.id, action.result_id, result)
+                result_action_object = wrap_result(action.result_id, result)
             elif twin_mode == TwinMode.NONE and has_twin_inputs:
                 # self isn't a twin but one of the inputs is
                 private_args = filter_twin_args(args, twin_mode=twin_mode)
                 private_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
                 private_result = target_method(*private_args, **private_kwargs)
                 result_action_object_private = wrap_result(
-                    action.parent_id, action.result_id, private_result
+                    action.result_id, private_result
                 )
 
                 mock_args = filter_twin_args(args, twin_mode=twin_mode)
                 mock_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
                 mock_result = target_method(*mock_args, **mock_kwargs)
-                result_action_object_mock = wrap_result(
-                    action.parent_id, action.result_id, mock_result
-                )
+                result_action_object_mock = wrap_result(action.result_id, mock_result)
 
                 result_action_object = TwinObject(
                     id=action.result_id,
                     private_obj=result_action_object_private,
                     mock_obj=result_action_object_mock,
                 )
             elif twin_mode == twin_mode.PRIVATE:  # type: ignore
                 # twin private path
                 private_args = filter_twin_args(args, twin_mode=twin_mode)
                 private_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
                 result = target_method(*private_args, **private_kwargs)
-                result_action_object = wrap_result(
-                    action.parent_id, action.result_id, result
-                )
+                result_action_object = wrap_result(action.result_id, result)
             elif twin_mode == twin_mode.MOCK:  # type: ignore
                 # twin mock path
                 mock_args = filter_twin_args(args, twin_mode=twin_mode)
                 mock_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
                 target_method = getattr(unboxed_resolved_self, action.op, None)
                 result = target_method(*mock_args, **mock_kwargs)
-                result_action_object = wrap_result(
-                    action.parent_id, action.result_id, result
-                )
+                result_action_object = wrap_result(action.result_id, result)
             else:
                 raise Exception(
                     f"Bad combination of: twin_mode: {twin_mode} and has_twin_inputs: {has_twin_inputs}"
                 )
         else:
             return Err("Missing target method")
 
     except Exception as e:
         return Err(e)
 
     return Ok(result_action_object)
 
 
-def wrap_result(parent_id: UID, result_id: UID, result: Any) -> ActionObject:
+def wrap_result(result_id: UID, result: Any) -> ActionObject:
     # 🟡 TODO 11: Figure out how we want to store action object results
     action_type = action_type_for_type(result)
-    result_action_object = action_type(
-        id=result_id, parent_id=parent_id, syft_action_data=result
-    )
+    result_action_object = action_type(id=result_id, syft_action_data=result)
     return result_action_object
 
 
 def filter_twin_args(args: List[Any], twin_mode: TwinMode) -> Any:
     filtered = []
     for arg in args:
         if isinstance(arg, TwinObject):
```

### Comparing `syft-0.8.1b1/src/syft/service/action/action_store.py` & `syft-0.8.1b2/src/syft/service/action/action_store.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from ...store.document_store import BasePartitionSettings
 from ...store.document_store import StoreConfig
 from ...types.syft_object import SyftObject
 from ...types.twin_object import TwinObject
 from ...types.uid import LineageID
 from ...types.uid import UID
 from ..response import SyftSuccess
+from .action_object import TwinMode
 from .action_permissions import ActionObjectEXECUTE
 from .action_permissions import ActionObjectOWNER
 from .action_permissions import ActionObjectPermission
 from .action_permissions import ActionObjectREAD
 from .action_permissions import ActionObjectWRITE
 from .action_permissions import ActionPermission
 
@@ -56,76 +57,104 @@
         self.permissions = self.store_config.backing_store(
             "permissions", self.settings, self.store_config, ddtype=set
         )
         if root_verify_key is None:
             root_verify_key = SyftSigningKey.generate().verify_key
         self.root_verify_key = root_verify_key
 
-    def get(self, uid: UID, credentials: SyftVerifyKey) -> Result[SyftObject, str]:
+    def get(
+        self, uid: UID, credentials: SyftVerifyKey, has_permission=False
+    ) -> Result[SyftObject, str]:
         uid = uid.id  # We only need the UID from LineageID or UID
 
         # TODO 🟣 Temporarily added skip permission argument for enclave
         # until permissions are fully integrated
         # if you get something you need READ permission
         read_permission = ActionObjectREAD(uid=uid, credentials=credentials)
-        if self.has_permission(read_permission):
-            if isinstance(uid, LineageID):
-                syft_object = self.data[uid.id]
-            elif isinstance(uid, UID):
-                syft_object = self.data[uid]
-            else:
-                raise Exception(f"Unrecognized UID type: {type(uid)}")
-            return Ok(syft_object)
+        if has_permission or self.has_permission(read_permission):
+            try:
+                if isinstance(uid, LineageID):
+                    syft_object = self.data[uid.id]
+                elif isinstance(uid, UID):
+                    syft_object = self.data[uid]
+                else:
+                    raise Exception(f"Unrecognized UID type: {type(uid)}")
+                return Ok(syft_object)
+            except Exception as e:
+                return Err(f"Could not find item with uid {uid}, {e}")
         return Err(f"Permission: {read_permission} denied")
 
     def get_pointer(
         self, uid: UID, credentials: SyftVerifyKey, node_uid: UID
     ) -> Result[SyftObject, str]:
         uid = uid.id  # We only need the UID from LineageID or UID
 
         try:
             # 🟡 TODO 34: do we want pointer read permissions?
             if uid in self.data:
                 obj = self.data[uid]
                 if isinstance(obj, TwinObject):
                     obj = obj.mock
+                    obj.syft_twin_type = TwinMode.MOCK
+                    # we patch the real id on it so we can keep using the twin
+                    obj.id = uid
+                else:
+                    obj.syft_twin_type = TwinMode.NONE
                 obj.syft_point_to(node_uid)
                 return Ok(obj)
+            # third party
             return Err("Permission denied")
         except Exception as e:
             return Err(str(e))
 
     def exists(self, uid: UID) -> bool:
         uid = uid.id  # We only need the UID from LineageID or UID
 
         return uid in self.data
 
     def set(
-        self, uid: UID, credentials: SyftVerifyKey, syft_object: SyftObject
+        self,
+        uid: UID,
+        credentials: SyftVerifyKey,
+        syft_object: SyftObject,
+        has_result_read_permission: bool = False,
     ) -> Result[SyftSuccess, Err]:
         uid = uid.id  # We only need the UID from LineageID or UID
 
         # if you set something you need WRITE permission
         write_permission = ActionObjectWRITE(uid=uid, credentials=credentials)
         can_write = self.has_permission(write_permission)
 
         if not self.exists(uid=uid):
             # attempt to claim it for writing
-            ownership_result = self.take_ownership(uid=uid, credentials=credentials)
-            can_write = True if ownership_result.is_ok() else False
+            if has_result_read_permission:
+                ownership_result = self.take_ownership(uid=uid, credentials=credentials)
+                can_write = True if ownership_result.is_ok() else False
+            else:
+                # root takes owneship, but you can still write
+                ownership_result = self.take_ownership(
+                    uid=uid, credentials=self.root_verify_key
+                )
+                can_write = True if ownership_result.is_ok() else False
 
         if can_write:
             self.data[uid] = syft_object
-            if uid not in self.permissions:
-                # create default permissions
-                self.permissions[uid] = set()
-            permission = f"{credentials.verify}_READ"
-            permissions = self.permissions[uid]
-            permissions.add(permission)
-            self.permissions[uid] = permissions
+            if has_result_read_permission:
+                if uid not in self.permissions:
+                    # create default permissions
+                    self.permissions[uid] = set()
+                self.add_permission(ActionObjectREAD(uid=uid, credentials=credentials))
+            else:
+                self.add_permissions(
+                    [
+                        ActionObjectWRITE(uid=uid, credentials=credentials),
+                        ActionObjectEXECUTE(uid=uid, credentials=credentials),
+                    ]
+                )
+
             return Ok(SyftSuccess(message=f"Set for ID: {uid}"))
         return Err(f"Permission: {write_permission} denied")
 
     def take_ownership(
         self, uid: UID, credentials: SyftVerifyKey
     ) -> Result[SyftSuccess, str]:
         uid = uid.id  # We only need the UID from LineageID or UID
@@ -179,14 +208,17 @@
         elif permission.permission == ActionPermission.WRITE:
             pass
         elif permission.permission == ActionPermission.EXECUTE:
             pass
 
         return False
 
+    def has_permissions(self, permissions: List[ActionObjectPermission]) -> bool:
+        return all([self.has_permission(p) for p in permissions])
+
     def add_permission(self, permission: ActionObjectPermission) -> None:
         permissions = self.permissions[permission.uid]
         permissions.add(permission.permission_string)
         self.permissions[permission.uid] = permissions
 
     def remove_permission(self, permission: ActionObjectPermission):
         permissions = self.permissions[permission.uid]
```

### Comparing `syft-0.8.1b1/src/syft/service/action/numpy.py` & `syft-0.8.1b2/src/syft/service/action/numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # third party
 import numpy as np
 
 # relative
 from ...serde.serializable import serializable
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from .action_object import ActionObject
+from .action_object import BASE_PASSTHROUGH_ATTRS
 from .action_types import action_types
 
 # @serializable(attrs=["id", "node_uid", "parent_id"])
 # class NumpyArrayObjectPointer(ActionObjectPointer):
 #     _inflix_operations = ["__add__", "__sub__", "__eq__", "__mul__"]
 #     __canonical_name__ = "NumpyArrayObjectPointer"
 #     __version__ = SYFT_OBJECT_VERSION_1
@@ -41,15 +42,15 @@
 @serializable()
 class NumpyArrayObject(ActionObject, np.lib.mixins.NDArrayOperatorsMixin):
     __canonical_name__ = "NumpyArrayObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     syft_internal_type: ClassVar[Type[Any]] = np.ndarray
     syft_pointer_type = NumpyArrayObjectPointer
-    syft_passthrough_attrs = []
+    syft_passthrough_attrs = BASE_PASSTHROUGH_ATTRS
     syft_dont_wrap_attrs = ["dtype"]
 
     # def __eq__(self, other: Any) -> bool:
     #     # 🟡 TODO 8: move __eq__ to a Data / Serdeable type interface on ActionObject
     #     if isinstance(other, NumpyArrayObject):
     #         return (
     #             numpy_like_eq(self.syft_action_data, other.syft_action_data)
@@ -82,28 +83,28 @@
 
 @serializable()
 class NumpyScalarObject(ActionObject, np.lib.mixins.NDArrayOperatorsMixin):
     __canonical_name__ = "NumpyScalarObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     syft_internal_type = np.number
-    syft_passthrough_attrs = []
+    syft_passthrough_attrs = BASE_PASSTHROUGH_ATTRS
     syft_dont_wrap_attrs = ["dtype"]
 
     def __float__(self) -> float:
         return float(self.syft_action_data)
 
 
 @serializable()
 class NumpyBoolObject(ActionObject, np.lib.mixins.NDArrayOperatorsMixin):
     __canonical_name__ = "NumpyBoolObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     syft_internal_type = np.bool_
-    syft_passthrough_attrs = []
+    syft_passthrough_attrs = BASE_PASSTHROUGH_ATTRS
     syft_dont_wrap_attrs = ["dtype"]
 
 
 np_array = np.array([1, 2, 3])
 action_types[type(np_array)] = NumpyArrayObject
```

### Comparing `syft-0.8.1b1/src/syft/service/action/pandas.py` & `syft-0.8.1b2/src/syft/service/action/pandas.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 from pandas import DataFrame
 from pandas import Series
 
 # relative
 from ...serde.serializable import serializable
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from .action_object import ActionObject
+from .action_object import BASE_PASSTHROUGH_ATTRS
 from .action_types import action_types
 
 
 @serializable()
 class PandasDataFrameObject(ActionObject):
     __canonical_name__ = "PandasDataframeObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     syft_internal_type: ClassVar[Type[Any]] = DataFrame
-    syft_passthrough_attrs = []
+    syft_passthrough_attrs = BASE_PASSTHROUGH_ATTRS
     # syft_dont_wrap_attrs = ["shape"]
 
     def __dataframe__(self, *args: Any, **kwargs: Any) -> Any:
         return self.__dataframe__(*args, **kwargs)
 
     def __getattribute__(self, name: str) -> Any:
         return super().__getattribute__(name)
@@ -41,15 +42,14 @@
 
 @serializable()
 class PandasSeriesObject(ActionObject):
     __canonical_name__ = "PandasSeriesObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     syft_internal_type = Series
-    syft_passthrough_attrs = []
     # syft_dont_wrap_attrs = ["shape"]
 
     def __getattribute__(self, name: str) -> Any:
         return super().__getattribute__(name)
 
     def syft_get_property(self, obj: Any, method: str) -> Any:
         return getattr(self.syft_action_data, method)
```

### Comparing `syft-0.8.1b1/src/syft/service/action/verification.py` & `syft-0.8.1b2/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/code/unparse.py` & `syft-0.8.1b2/src/syft/service/code/unparse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/code/user_code.py` & `syft-0.8.1b2/src/syft/service/code/user_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,26 +319,33 @@
 
     @property
     def unsafe_function(self) -> Optional[Callable]:
         print("WARNING: This code was submitted by a User and could be UNSAFE.")
 
         # 🟡 TODO: re-use the same infrastructure as the execute_byte_code function
         def wrapper(*args: Any, **kwargs: Any) -> Callable:
-            # remove the decorator
-            inner_function = ast.parse(self.raw_code).body[0]
-            inner_function.decorator_list = []
-            # compile the function
-            raw_byte_code = compile_byte_code(unparse(inner_function))
-            # load it
-            exec(raw_byte_code)  # nosec
-            # execute it
-            evil_string = f"{self.service_func_name}(*args, **kwargs)"
-            result = eval(evil_string, None, locals())  # nosec
-            # return the results
-            return result
+            try:
+                filtered_kwargs = {}
+                for k, v in kwargs.items():
+                    filtered_kwargs[k] = debox_asset(v)
+
+                # remove the decorator
+                inner_function = ast.parse(self.raw_code).body[0]
+                inner_function.decorator_list = []
+                # compile the function
+                raw_byte_code = compile_byte_code(unparse(inner_function))
+                # load it
+                exec(raw_byte_code)  # nosec
+                # execute it
+                evil_string = f"{self.service_func_name}(**filtered_kwargs)"
+                result = eval(evil_string, None, locals())  # nosec
+                # return the results
+                return result
+            except Exception as e:
+                print(f"Failed to run unsafe_function. {e}")
 
         return wrapper
 
     @property
     def code(self) -> str:
         return self.raw_code
```

### Comparing `syft-0.8.1b1/src/syft/service/code/user_code_parse.py` & `syft-0.8.1b2/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/code/user_code_service.py` & `syft-0.8.1b2/src/syft/service/code/user_code_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
             return final_results
         except Exception as e:
             return SyftError(message=f"Failed to run. {e}")
 
 
 def get_outputs(context: AuthedServiceContext, output_history: OutputHistory) -> Any:
     # relative
-    from ...service.action.action_service import TwinMode
+    from ...service.action.action_object import TwinMode
 
     if isinstance(output_history.outputs, list):
         if len(output_history.outputs) == 0:
             return None
         outputs = []
         for output_id in output_history.outputs:
             action_service = context.node.get_service("actionservice")
```

### Comparing `syft-0.8.1b1/src/syft/service/code/user_code_stash.py` & `syft-0.8.1b2/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/context.py` & `syft-0.8.1b2/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/data_subject/data_subject.py` & `syft-0.8.1b2/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.1b2/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.1b2/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.1b2/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/dataset/dataset.py` & `syft-0.8.1b2/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/dataset/dataset_service.py` & `syft-0.8.1b2/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.1b2/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/message/message_service.py` & `syft-0.8.1b2/src/syft/service/message/message_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/message/message_stash.py` & `syft-0.8.1b2/src/syft/service/message/message_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/message/messages.py` & `syft-0.8.1b2/src/syft/service/message/messages.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/metadata/metadata_service.py` & `syft-0.8.1b2/src/syft/service/metadata/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/metadata/metadata_stash.py` & `syft-0.8.1b2/src/syft/service/metadata/metadata_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/metadata/node_metadata.py` & `syft-0.8.1b2/src/syft/service/metadata/node_metadata.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from ...types.syft_object import StorableObjectType
 from ...types.syft_object import SyftObject
 from ...types.transforms import convert_types
 from ...types.transforms import drop
 from ...types.transforms import rename
 from ...types.transforms import transform
 from ...types.uid import UID
+from ...util.util import recursive_hash
 
 
 def check_version(
     client_version: str, server_version: str, server_name: str, silent: bool = False
 ) -> bool:
     client_syft_version = version.parse(client_version)
     node_syft_version = version.parse(server_version)
@@ -77,14 +78,28 @@
     def check_version(self, client_version: str) -> None:
         return check_version(
             client_version=client_version,
             server_version=self.syft_version,
             server_name=self.name,
         )
 
+    def __hash__(self) -> int:
+        hashes = 0
+        hashes += recursive_hash(self.id)
+        hashes += recursive_hash(self.name)
+        hashes += recursive_hash(self.verify_key)
+        hashes += recursive_hash(self.highest_object_version)
+        hashes += recursive_hash(self.lowest_object_version)
+        hashes += recursive_hash(self.node_type)
+        hashes += recursive_hash(self.deployed_on)
+        hashes += recursive_hash(self.organization)
+        hashes += recursive_hash(self.on_board)
+        hashes += recursive_hash(self.description)
+        return hashes
+
 
 @serializable()
 class NodeMetadataJSON(BaseModel, StorableObjectType):
     metadata_version: int
     name: str
     id: str
     verify_key: str
```

### Comparing `syft-0.8.1b1/src/syft/service/network/network_service.py` & `syft-0.8.1b2/src/syft/service/network/network_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,24 +29,26 @@
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import keep
 from ...types.transforms import transform
 from ...types.transforms import transform_method
 from ...types.uid import UID
 from ...util.telemetry import instrument
+from ...util.util import recursive_hash
 from ..context import AuthedServiceContext
 from ..context import NodeServiceContext
 from ..data_subject.data_subject import NamePartitionKey
 from ..metadata.node_metadata import NodeMetadata
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
+from ..user.user_roles import GUEST_ROLE_LEVEL
 
 VerifyKeyPartitionKey = PartitionKey(key="verify_key", type_=SyftVerifyKey)
 
 
 class NodeRoute:
     def client_with_context(self, context: NodeServiceContext) -> SyftClient:
         connection = route_to_connection(route=self, context=context)
@@ -144,14 +146,22 @@
     verify_key: SyftVerifyKey
     node_routes: List[NodeRoute] = []
 
     __attr_searchable__ = ["name"]
     __attr_unique__ = ["verify_key"]
     __attr_repr_cols__ = ["name"]
 
+    def __hash__(self) -> int:
+        hashes = 0
+        hashes += recursive_hash(self.id)
+        hashes += recursive_hash(self.name)
+        hashes += recursive_hash(self.verify_key)
+        hashes += recursive_hash(self.node_routes)
+        return hashes
+
     def update_routes(self, new_routes: List[NodeRoute]) -> None:
         add_routes = []
         existing_routes = set(self.node_routes)
         for new_route in new_routes:
             if new_route not in existing_routes:
                 add_routes.append(new_route)
         self.node_routes += add_routes
@@ -265,19 +275,19 @@
 
     def update_peer(
         self, credentials: SyftVerifyKey, peer: NodePeer
     ) -> Result[NodePeer, str]:
         valid = self.check_type(peer, NodePeer)
         if valid.is_err():
             return SyftError(message=valid.err())
-        existing = self.get_by_uid(peer.id)
+        existing = self.get_by_uid(credentials, peer.id)
         if existing.is_ok() and existing.ok():
             existing = existing.ok()
             existing.update_routes(peer.node_routes)
-            result = self.update(existing)
+            result = self.update(credentials, existing)
             return result
         else:
             result = self.set(credentials, peer)
             return result
 
     def get_for_verify_key(
         self, credentials: SyftVerifyKey, verify_key: SyftVerifyKey
@@ -329,37 +339,37 @@
                 (
                     f"Response from remote peer {remote_peer_metadata} "
                     f"does not match initial peer {remote_peer}"
                 )
             )
 
         # save the remote peer for later
-        result = self.stash.update_peer(remote_peer)
+        result = self.stash.update_peer(context.credentials, remote_peer)
         if result.is_err():
             return SyftError(message=str(result.err()))
 
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="Credentials Exchanged")
 
-    @service_method(path="network.add_peer", name="add_peer")
+    @service_method(path="network.add_peer", name="add_peer", roles=GUEST_ROLE_LEVEL)
     def add_peer(
         self, context: AuthedServiceContext, peer: NodePeer
     ) -> Union[NodeMetadata, SyftError]:
         """Add a Network Node Peer"""
         # save the peer and verify the key matches the message signer
         if peer.verify_key != context.credentials:
             return SyftError(
                 message=(
                     f"The {type(peer)}.verify_key: "
                     f"{peer.verify_key} does not match the signature of the message"
                 )
             )
 
-        result = self.stash.update_peer(peer)
+        result = self.stash.update_peer(context.credentials, peer)
         if result.is_err():
             return SyftError(message=str(result.err()))
         # this way they can match up who we are with who they think we are
         metadata = context.node.metadata
         return metadata
 
     @service_method(path="network.add_route_for", name="add_route_for")
@@ -382,46 +392,50 @@
         client = remote_peer.client_with_context(context=context)
         result = client.api.services.network.verify_route(route)
 
         if not isinstance(result, SyftSuccess):
             return result
         return SyftSuccess(message="Route Verified")
 
-    @service_method(path="network.verify_route", name="verify_route")
+    @service_method(
+        path="network.verify_route", name="verify_route", roles=GUEST_ROLE_LEVEL
+    )
     def verify_route(
         self, context: AuthedServiceContext, route: NodeRoute
     ) -> Union[SyftSuccess, SyftError]:
         """Add a Network Node Route"""
         # get the peer asking for route verification from its verify_key
-        peer = self.stash.get_for_verify_key(context.credentials)
+        peer = self.stash.get_for_verify_key(
+            context.node.verify_key, context.credentials
+        )
         if peer.is_err():
             return SyftError(message=peer.err())
         peer = peer.ok()
 
         client = route.client_with_context(context=context)
         metadata = client.metadata.to(NodeMetadata)
         if peer.verify_key != metadata.verify_key:
             return SyftError(
                 message=(
                     f"verify_key: {metadata.verify_key} at route {route} "
                     f"does not match listed peer: {peer}"
                 )
             )
         peer.update_routes([route])
-        result = self.stash.update_peer(peer)
+        result = self.stash.update_peer(context.credentials, peer)
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="Network Route Verified")
 
     @service_method(path="network.get_all_peers", name="get_all_peers")
     def get_all_peers(
         self, context: AuthedServiceContext
     ) -> Union[List[NodePeer], SyftError]:
         """Get all Peers"""
-        result = self.stash.get_all()
+        result = self.stash.get_all(context.credentials)
         if result.is_ok():
             peers = result.ok()
             return peers
         return SyftError(message=result.err())
 
 
 TYPE_TO_SERVICE[NodePeer] = NetworkService
```

### Comparing `syft-0.8.1b1/src/syft/service/policy/policy.py` & `syft-0.8.1b2/src/syft/service/policy/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         return self.init_kwargs
 
 
 def retrieve_from_db(
     code_item_id: UID, allowed_inputs: Dict[str, UID], context: AuthedServiceContext
 ) -> Dict:
     # relative
-    from ...service.action.action_service import TwinMode
+    from ...service.action.action_object import TwinMode
 
     action_service = context.node.get_service("actionservice")
     code_inputs = {}
 
     if context.node.node_type == NodeType.DOMAIN:
         for var_name, arg_id in allowed_inputs.items():
             kwarg_value = action_service.get(
```

### Comparing `syft-0.8.1b1/src/syft/service/policy/policy_service.py` & `syft-0.8.1b2/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.1b2/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/project/project_stash.py` & `syft-0.8.1b2/src/syft/service/project/project_stash.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,29 +10,45 @@
 from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
 from ...util.telemetry import instrument
 from ..request.request import Request
 from ..response import SyftError
+from .project import NewProject
 from .project import Project
 
-ProjectUserVerifyKeyPartitionKey = PartitionKey(
-    key="user_verify_key", type_=SyftVerifyKey
-)
+VerifyKeyPartitionKey = PartitionKey(key="user_verify_key", type_=SyftVerifyKey)
 
 
 @instrument
 @serializable()
 class ProjectStash(BaseUIDStoreStash):
     object_type = Project
     settings: PartitionSettings = PartitionSettings(
         name=Project.__canonical_name__, object_type=Project
     )
 
     def get_all_for_verify_key(
-        self, credentials: SyftVerifyKey, verify_key: ProjectUserVerifyKeyPartitionKey
+        self, credentials: SyftVerifyKey, verify_key: VerifyKeyPartitionKey
     ) -> Result[List[Request], SyftError]:
         if isinstance(verify_key, str):
             verify_key = SyftVerifyKey.from_string(verify_key)
-        qks = QueryKeys(qks=[ProjectUserVerifyKeyPartitionKey.with_obj(verify_key)])
+        qks = QueryKeys(qks=[VerifyKeyPartitionKey.with_obj(verify_key)])
+        return self.query_all(credentials=credentials, qks=qks)
+
+
+@instrument
+@serializable()
+class NewProjectStash(BaseUIDStoreStash):
+    object_type = NewProject
+    settings: PartitionSettings = PartitionSettings(
+        name=NewProject.__canonical_name__, object_type=NewProject
+    )
+
+    def get_all_for_verify_key(
+        self, credentials: SyftVerifyKey, verify_key: VerifyKeyPartitionKey
+    ) -> Result[List[Request], SyftError]:
+        if isinstance(verify_key, str):
+            verify_key = SyftVerifyKey.from_string(verify_key)
+        qks = QueryKeys(qks=[VerifyKeyPartitionKey.with_obj(verify_key)])
         return self.query_all(credentials=credentials, qks=qks)
```

### Comparing `syft-0.8.1b1/src/syft/service/queue/queue_stash.py` & `syft-0.8.1b2/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/request/request.py` & `syft-0.8.1b2/src/syft/service/request/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import add_node_uid_for_key
 from ...types.transforms import generate_id
 from ...types.transforms import transform
+from ...types.uid import LineageID
 from ...types.uid import UID
 from ..action.action_object import ActionObject
 from ..action.action_service import ActionService
 from ..action.action_store import ActionObjectPermission
 from ..action.action_store import ActionPermission
 from ..code.user_code import UserCode
 from ..code.user_code import UserCodeStatus
@@ -72,22 +73,27 @@
 
     def _run(
         self, context: ChangeContext, apply: bool
     ) -> Result[SyftSuccess, SyftError]:
         try:
             action_service = context.node.get_service(ActionService)
             action_store = action_service.store
+
+            # can we ever have a lineage ID in the store?
+            obj_uid = self.linked_obj.object_uid
+            obj_uid = obj_uid.id if isinstance(obj_uid, LineageID) else obj_uid
+
             owner_permission = ActionObjectPermission(
-                uid=self.linked_obj.object_uid,
+                uid=obj_uid,
                 credentials=context.approving_user_credentials,
                 permission=self.apply_permission_type,
             )
             if action_store.has_permission(permission=owner_permission):
                 requesting_permission = ActionObjectPermission(
-                    uid=self.linked_obj.object_uid,
+                    uid=obj_uid,
                     credentials=context.requesting_user_credentials,
                     permission=self.apply_permission_type,
                 )
                 if apply:
                     action_store.add_permission(requesting_permission)
                 else:
                     action_store.remove_permission(requesting_permission)
@@ -131,14 +137,17 @@
     __attr_unique__ = ["request_hash"]
     __attr_repr_cols__ = ["request_time", "status", "changes"]
 
     def approve(self):
         api = APIRegistry.api_for(self.node_uid)
         return api.services.request.apply(self.id)
 
+    def approve_with_client(self, client):
+        return client.api.services.request.apply(self.id)
+
     def apply(self, context: AuthedServiceContext) -> Result[SyftSuccess, SyftError]:
         change_context = ChangeContext.from_service(context)
         change_context.requesting_user_credentials = self.requesting_user_verify_key
         for change in self.changes:
             result = change.apply(context=change_context)
             if result.is_err():
                 return result
@@ -472,15 +481,15 @@
                     return enclave_res
                 self.linked_obj.update_with_context(context, res)
             else:
                 raise NotImplementedError
             return Ok(SyftSuccess(message=f"{type(self)} Success"))
         except Exception as e:
             print(f"failed to apply {type(self)}. {e}")
-            return Err(SyftError(message=e))
+            return Err(SyftError(message=str(e)))
 
     def apply(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
         return self._run(context=context, apply=True)
 
     def revert(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
         return self._run(context=context, apply=False)
```

### Comparing `syft-0.8.1b1/src/syft/service/request/request_service.py` & `syft-0.8.1b2/src/syft/service/request/request_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from ..message.message_service import MessageService
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
+from ..user.user_roles import GUEST_ROLE_LEVEL
 from ..user.user_service import UserService
 from .request import Request
 from .request import RequestStatus
 from .request import SubmitRequest
 from .request_stash import RequestStash
 
 
@@ -37,15 +38,15 @@
     store: DocumentStore
     stash: RequestStash
 
     def __init__(self, store: DocumentStore) -> None:
         self.store = store
         self.stash = RequestStash(store=store)
 
-    @service_method(path="request.submit", name="submit")
+    @service_method(path="request.submit", name="submit", roles=GUEST_ROLE_LEVEL)
     def submit(
         self,
         context: AuthedServiceContext,
         request: SubmitRequest,
         send_message: bool = True,
     ) -> Union[Request, SyftError]:
         """Submit a Request"""
```

### Comparing `syft-0.8.1b1/src/syft/service/request/request_stash.py` & `syft-0.8.1b2/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/response.py` & `syft-0.8.1b2/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/service.py` & `syft-0.8.1b2/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/user/user.py` & `syft-0.8.1b2/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/user/user_roles.py` & `syft-0.8.1b2/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/user/user_service.py` & `syft-0.8.1b2/src/syft/service/user/user_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/service/user/user_stash.py` & `syft-0.8.1b2/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/store/dict_document_store.py` & `syft-0.8.1b2/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/store/document_store.py` & `syft-0.8.1b2/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/store/kv_document_store.py` & `syft-0.8.1b2/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/store/linked_obj.py` & `syft-0.8.1b2/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/store/locks.py` & `syft-0.8.1b2/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/store/mongo_client.py` & `syft-0.8.1b2/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/store/mongo_codecs.py` & `syft-0.8.1b2/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/store/mongo_document_store.py` & `syft-0.8.1b2/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/store/sqlite_document_store.py` & `syft-0.8.1b2/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/types/datetime.py` & `syft-0.8.1b2/src/syft/types/datetime.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,7 +20,10 @@
     @staticmethod
     def now() -> Self:
         return DateTime(utc_timestamp=datetime.utcnow().timestamp())
 
     def __str__(self) -> str:
         utc_datetime = datetime.utcfromtimestamp(self.utc_timestamp)
         return utc_datetime.strftime("%Y-%m-%d %H:%M:%S")
+
+    def __hash__(self) -> int:
+        return hash(self.utc_timestamp)
```

### Comparing `syft-0.8.1b1/src/syft/types/grid_url.py` & `syft-0.8.1b2/src/syft/types/grid_url.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,25 +77,31 @@
 
     def with_path(self, path: str) -> GridURL:
         dupe = copy.copy(self)
         dupe.path = path
         return dupe
 
     def as_container_host(self, container_host: Optional[str] = None) -> GridURL:
-        if self.host_or_ip not in ["localhost", "docker-host", "host.k3d.internal"]:
+        if self.host_or_ip not in [
+            "localhost",
+            "host.docker.internal",
+            "host.k3d.internal",
+        ]:
             return self
 
         if container_host is None:
             # TODO: we could move config.py to syft and then the Settings singleton
             # could be importable in all parts of the code
             container_host = os.getenv("CONTAINER_HOST", None)
 
         if container_host:
             hostname = (
-                "docker-host" if container_host == "docker" else "host.k3d.internal"
+                "host.docker.internal"
+                if container_host == "docker"
+                else "host.k3d.internal"
             )
         else:
             # convert it back for non container clients
             hostname = "localhost"
 
         return GridURL(
             protocol=self.protocol,
```

### Comparing `syft-0.8.1b1/src/syft/types/syft_metaclass.py` & `syft-0.8.1b2/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/types/syft_object.py` & `syft-0.8.1b2/src/syft/types/syft_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,19 @@
 from typeguard import check_type
 
 # relative
 from ..node.credentials import SyftVerifyKey
 from ..serde.deserialize import _deserialize as deserialize
 from ..serde.recursive_primitives import recursive_serde_register_type
 from ..serde.serialize import _serialize as serialize
+from ..util.autoreload import autoreload_enabled
 from ..util.util import aggressive_set_attr
 from ..util.util import full_name_with_qualname
 from ..util.util import get_qualname_for
+from ..util.util import recursive_hash
 from .syft_metaclass import Empty
 from .syft_metaclass import PartialModelMetaclass
 from .uid import UID
 
 SYFT_OBJECT_VERSION_1 = 1
 SYFT_OBJECT_VERSION_2 = 2
 
@@ -58,15 +60,19 @@
     __object_version_registry__: Dict[str, Type["SyftObject"]] = {}
     __object_transform_registry__: Dict[str, Callable] = {}
 
     def __init_subclass__(cls, **kwargs: Any) -> None:
         super().__init_subclass__(**kwargs)
         if hasattr(cls, "__canonical_name__") and hasattr(cls, "__version__"):
             mapping_string = f"{cls.__canonical_name__}_{cls.__version__}"
-            if mapping_string in cls.__object_version_registry__:
+
+            if (
+                mapping_string in cls.__object_version_registry__
+                and not autoreload_enabled()
+            ):
                 current_cls = cls.__object_version_registry__[mapping_string]
                 if cls == current_cls:
                     # same class so noop
                     return None
 
                 # user code is reinitialized which means it might have a new address
                 # in memory so for that we can just skip
@@ -372,14 +378,25 @@
     def _syft_unique_keys_dict(cls) -> Dict[str, type]:
         return cls._syft_keys_types_dict("__attr_unique__")
 
     @classmethod
     def _syft_searchable_keys_dict(cls) -> Dict[str, type]:
         return cls._syft_keys_types_dict("__attr_searchable__")
 
+    @staticmethod
+    def calculate_hash(obj: Any, keys: List[str]) -> int:
+        hashes = 0
+        for key in keys:
+            if isinstance(obj, dict):
+                value = obj[key]
+            else:
+                value = getattr(obj, key)
+            hashes += recursive_hash(value)
+        return hashes
+
 
 def list_dict_repr_html(self) -> str:
     try:
         max_check = 1
         items_checked = 0
         has_syft = False
         extra_fields = []
```

### Comparing `syft-0.8.1b1/src/syft/types/transforms.py` & `syft-0.8.1b2/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/types/twin_object.py` & `syft-0.8.1b2/src/syft/types/twin_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # stdlib
 from typing import Any
 from typing import Optional
 
 # relative
 from ..serde.serializable import serializable
 from ..service.action.action_object import ActionObject
+from ..service.action.action_object import TwinMode
 from ..service.action.action_types import action_types
 from .syft_object import SyftObject
 from .uid import UID
 
 
 def to_action_object(obj: Any) -> ActionObject:
     if isinstance(obj, ActionObject):
@@ -59,16 +60,18 @@
             id=id,
         )
 
     @property
     def private(self) -> ActionObject:
         twin_id = self.id
         private = self.private_obj
+        private.syft_twin_type = TwinMode.PRIVATE
         private.id = twin_id
         return private
 
     @property
     def mock(self) -> ActionObject:
         twin_id = self.id
         mock = self.mock_obj
+        mock.syft_twin_type = TwinMode.MOCK
         mock.id = twin_id
         return mock
```

### Comparing `syft-0.8.1b1/src/syft/types/uid.py` & `syft-0.8.1b2/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/util/decorators.py` & `syft-0.8.1b2/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/util/experimental_flags.py` & `syft-0.8.1b2/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/util/filterwarnings.py` & `syft-0.8.1b2/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/util/logger.py` & `syft-0.8.1b2/src/syft/util/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,13 +118,18 @@
     return create_log_and_print_function(level="warning")(*args, **kwargs)
 
 
 def info(*args: Any, **kwargs: Any) -> None:
     return create_log_and_print_function(level="info")(*args, **kwargs)
 
 
-def debug(*args: Any, **kwargs: Any) -> None:
+def debug(*args) -> None:
+    debug_msg = " ".join([str(a) for a in args])
+    return logger.debug(debug_msg)
+
+
+def _debug(*args: Any, **kwargs: Any) -> None:
     return create_log_and_print_function(level="debug")(*args, **kwargs)
 
 
 def trace(*args: Any, **kwargs: Any) -> None:
     return create_log_and_print_function(level="trace")(*args, **kwargs)
```

### Comparing `syft-0.8.1b1/src/syft/util/telemetry.py` & `syft-0.8.1b2/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/util/trace_decorator.py` & `syft-0.8.1b2/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft/util/util.py` & `syft-0.8.1b2/src/syft/util/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 # third party
 from forbiddenfruit import curse
 from nacl.signing import SigningKey
 from nacl.signing import VerifyKey
 import requests
 
 # relative
+from ..serde.serialize import _serialize
 from .logger import critical
 from .logger import debug
 from .logger import error
 from .logger import traceback_and_raise
 
 
 def full_name_with_qualname(klass: type) -> str:
@@ -823,7 +824,29 @@
 
 def get_interpreter_module() -> str:
     try:
         shell = get_ipython().__class__.__module__
         return shell
     except NameError:
         return "StandardInterpreter"  # not sure
+
+
+def recursive_hash(obj: Any) -> int:
+    hashes = 0
+    if isinstance(obj, (list, dict, set)):
+        if isinstance(obj, (list, set)):
+            for item in obj:
+                hashes += recursive_hash(item)
+        elif isinstance(obj, dict):
+            for item_key, item in obj:
+                hashes += recursive_hash(item_key)
+                hashes += recursive_hash(item)
+    else:
+        # TODO: remove the generic python hash from other checks and use a more secure one
+        # As the python hash does not produce unique hashes for different runs
+        # and also for different python versions
+        # to be modified in the hashing PR
+        # Adding a temp fix for now
+        serde_bytes = _serialize(obj, to_bytes=True)
+        hash_bytes = hashlib.sha256(serde_bytes).digest()
+        hashes += int.from_bytes(hash_bytes, byteorder="big")
+    return hashes
```

### Comparing `syft-0.8.1b1/src/syft/util/version_compare.py` & `syft-0.8.1b2/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b1/src/syft.egg-info/PKG-INFO` & `syft-0.8.1b2/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b1
+Version: 0.8.1b2
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b1 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b2 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.1b1/src/syft.egg-info/SOURCES.txt` & `syft-0.8.1b2/src/syft.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 src/syft/service/action/action_object.py
 src/syft/service/action/action_permissions.py
 src/syft/service/action/action_service.py
 src/syft/service/action/action_store.py
 src/syft/service/action/action_types.py
 src/syft/service/action/numpy.py
 src/syft/service/action/pandas.py
+src/syft/service/action/plan.py
 src/syft/service/action/verification.py
 src/syft/service/code/__init__.py
 src/syft/service/code/code_parse.py
 src/syft/service/code/unparse.py
 src/syft/service/code/user_code.py
 src/syft/service/code/user_code_parse.py
 src/syft/service/code/user_code_service.py
@@ -134,14 +135,15 @@
 src/syft/types/grid_url.py
 src/syft/types/syft_metaclass.py
 src/syft/types/syft_object.py
 src/syft/types/transforms.py
 src/syft/types/twin_object.py
 src/syft/types/uid.py
 src/syft/util/__init__.py
+src/syft/util/autoreload.py
 src/syft/util/decorators.py
 src/syft/util/experimental_flags.py
 src/syft/util/filterwarnings.py
 src/syft/util/jax_settings.py
 src/syft/util/logger.py
 src/syft/util/telemetry.py
 src/syft/util/trace_decorator.py
```

### Comparing `syft-0.8.1b1/src/syft.egg-info/requires.txt` & `syft-0.8.1b2/src/syft.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 pandas==1.5.3
 pyarrow==11.0.0
 pycapnp==1.3.0
 pydantic[email]==1.10.7
 pymongo==4.3.3
 pynacl==1.5.0
 redis==4.5.4
-requests==2.28.2
+requests==2.29.0
 RestrictedPython==6.0
 result==0.9.0
 tqdm==4.65.0
 typeguard==2.13.3
 typing_extensions==4.5.0
 sherlock[filelock,redis]==0.4.1
 uvicorn[standard]==0.21.1
@@ -53,15 +53,15 @@
 importlib-metadata==6.0.0
 isort==5.12.0
 mypy==1.1.1
 pre-commit==3.1.1
 safety==2.3.5
 
 [oblv]
-pyoblv==0.2.0
+oblv-ctl==0.3.1
 
 [test_plugins]
 pytest
 pytest-cov
 pytest-xdist[psutil]
 pytest-parallel
 pytest-asyncio
```

