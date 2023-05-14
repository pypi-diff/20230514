# Comparing `tmp/scaled-0.7.tar.gz` & `tmp/scaled-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaled-0.7.tar", last modified: Sun Feb 12 01:12:06 2023, max compression
+gzip compressed data, was "scaled-0.9.tar", last modified: Sun Feb 12 04:01:37 2023, max compression
```

## Comparing `scaled-0.7.tar` & `scaled-0.9.tar`

### file list

```diff
@@ -1,93 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.578039 scaled-0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.566039 scaled-0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.570039 scaled-0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-12 01:11:51.000000 scaled-0.7/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-12 01:11:51.000000 scaled-0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-02-12 01:11:51.000000 scaled-0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-02-12 01:12:06.578039 scaled-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-02-12 01:11:51.000000 scaled-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.570039 scaled-0.7/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-12 01:11:51.000000 scaled-0.7/benchmarks/dask_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-12 01:11:51.000000 scaled-0.7/benchmarks/dask_remote_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-02-12 01:11:51.000000 scaled-0.7/benchmarks/scaled_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-12 01:11:51.000000 scaled-0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-12 01:11:51.000000 scaled-0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-12 01:11:51.000000 scaled-0.7/run_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-12 01:11:51.000000 scaled-0.7/run_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.570039 scaled-0.7/scaled/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-12 01:11:51.000000 scaled-0.7/scaled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-12 01:11:51.000000 scaled-0.7/scaled/about.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.570039 scaled-0.7/scaled/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-02-12 01:11:51.000000 scaled-0.7/scaled/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.570039 scaled-0.7/scaled/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-02-12 01:11:51.000000 scaled-0.7/scaled/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-02-12 01:11:51.000000 scaled-0.7/scaled/cluster/combo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-12 01:11:51.000000 scaled-0.7/scaled/cluster/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.570039 scaled-0.7/scaled/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-02-12 01:11:51.000000 scaled-0.7/scaled/entry_points/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-02-12 01:11:51.000000 scaled-0.7/scaled/entry_points/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.574039 scaled-0.7/scaled/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-02-12 01:11:51.000000 scaled-0.7/scaled/io/async_binder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-02-12 01:11:51.000000 scaled-0.7/scaled/io/async_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-12 01:11:51.000000 scaled-0.7/scaled/io/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-02-12 01:11:51.000000 scaled-0.7/scaled/io/sync_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.574039 scaled-0.7/scaled/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/protocol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.574039 scaled-0.7/scaled/protocol/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/protocol/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-02-12 01:11:51.000000 scaled-0.7/scaled/protocol/python/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.574039 scaled-0.7/scaled/protocol/python/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/protocol/python/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-02-12 01:11:51.000000 scaled-0.7/scaled/protocol/python/serializer/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-02-12 01:11:51.000000 scaled-0.7/scaled/protocol/python/serializer/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.574039 scaled-0.7/scaled/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.574039 scaled-0.7/scaled/scheduler/client_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/client_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/client_manager/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.574039 scaled-0.7/scaled/scheduler/function_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/function_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/function_manager/vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.574039 scaled-0.7/scaled/scheduler/task_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/task_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/task_manager/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.574039 scaled-0.7/scaled/scheduler/worker_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/worker_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.574039 scaled-0.7/scaled/scheduler/worker_manager/allocators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/worker_manager/allocators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/worker_manager/allocators/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/worker_manager/allocators/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/worker_manager/allocators/queued.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-02-12 01:11:51.000000 scaled-0.7/scaled/scheduler/worker_manager/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.574039 scaled-0.7/scaled/utility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-02-12 01:11:51.000000 scaled-0.7/scaled/utility/event_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.574039 scaled-0.7/scaled/utility/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/utility/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-02-12 01:11:51.000000 scaled-0.7/scaled/utility/logging/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-02-12 01:11:51.000000 scaled-0.7/scaled/utility/logging/scoped_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-02-12 01:11:51.000000 scaled-0.7/scaled/utility/logging/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-02-12 01:11:51.000000 scaled-0.7/scaled/utility/zmq_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.574039 scaled-0.7/scaled/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/scaled/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-02-12 01:11:51.000000 scaled-0.7/scaled/worker/async_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-02-12 01:11:51.000000 scaled-0.7/scaled/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.570039 scaled-0.7/scaled.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-02-12 01:12:06.000000 scaled-0.7/scaled.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-02-12 01:12:06.000000 scaled-0.7/scaled.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 01:12:06.000000 scaled-0.7/scaled.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-12 01:12:06.000000 scaled-0.7/scaled.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-12 01:12:06.000000 scaled-0.7/scaled.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-12 01:12:06.000000 scaled-0.7/scaled.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 01:12:06.578039 scaled-0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 01:12:06.578039 scaled-0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 01:11:51.000000 scaled-0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-02-12 01:11:51.000000 scaled-0.7/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-02-12 01:11:51.000000 scaled-0.7/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-12 01:11:51.000000 scaled-0.7/tests/test_worker_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.680169 scaled-0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.672169 scaled-0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.676169 scaled-0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-12 04:01:20.000000 scaled-0.9/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-12 04:01:20.000000 scaled-0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-02-12 04:01:20.000000 scaled-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-02-12 04:01:37.680169 scaled-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-02-12 04:01:20.000000 scaled-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.676169 scaled-0.9/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-12 04:01:20.000000 scaled-0.9/benchmarks/dask_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-12 04:01:20.000000 scaled-0.9/benchmarks/dask_remote_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-12 04:01:20.000000 scaled-0.9/benchmarks/scaled_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-12 04:01:20.000000 scaled-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-12 04:01:20.000000 scaled-0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-12 04:01:20.000000 scaled-0.9/run_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-12 04:01:20.000000 scaled-0.9/run_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.676169 scaled-0.9/scaled/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-12 04:01:20.000000 scaled-0.9/scaled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-12 04:01:20.000000 scaled-0.9/scaled/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-02-12 04:01:20.000000 scaled-0.9/scaled/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.676169 scaled-0.9/scaled/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-02-12 04:01:20.000000 scaled-0.9/scaled/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-02-12 04:01:20.000000 scaled-0.9/scaled/cluster/combo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-12 04:01:20.000000 scaled-0.9/scaled/cluster/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.676169 scaled-0.9/scaled/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-02-12 04:01:20.000000 scaled-0.9/scaled/entry_points/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-02-12 04:01:20.000000 scaled-0.9/scaled/entry_points/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.676169 scaled-0.9/scaled/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-02-12 04:01:20.000000 scaled-0.9/scaled/io/async_binder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-02-12 04:01:20.000000 scaled-0.9/scaled/io/async_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-12 04:01:20.000000 scaled-0.9/scaled/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-02-12 04:01:20.000000 scaled-0.9/scaled/io/sync_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.676169 scaled-0.9/scaled/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/protocol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.676169 scaled-0.9/scaled/protocol/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/protocol/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-02-12 04:01:20.000000 scaled-0.9/scaled/protocol/python/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.676169 scaled-0.9/scaled/protocol/python/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/protocol/python/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-02-12 04:01:20.000000 scaled-0.9/scaled/protocol/python/serializer/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-02-12 04:01:20.000000 scaled-0.9/scaled/protocol/python/serializer/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.680169 scaled-0.9/scaled/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.680169 scaled-0.9/scaled/scheduler/client_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/client_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/client_manager/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.680169 scaled-0.9/scaled/scheduler/function_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/function_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/function_manager/vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.680169 scaled-0.9/scaled/scheduler/task_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/task_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/task_manager/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.680169 scaled-0.9/scaled/scheduler/worker_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/worker_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.680169 scaled-0.9/scaled/scheduler/worker_manager/allocators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/worker_manager/allocators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/worker_manager/allocators/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/worker_manager/allocators/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/worker_manager/allocators/queued.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-02-12 04:01:20.000000 scaled-0.9/scaled/scheduler/worker_manager/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.680169 scaled-0.9/scaled/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-02-12 04:01:20.000000 scaled-0.9/scaled/utility/event_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.680169 scaled-0.9/scaled/utility/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/utility/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-02-12 04:01:20.000000 scaled-0.9/scaled/utility/logging/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-02-12 04:01:20.000000 scaled-0.9/scaled/utility/logging/scoped_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-02-12 04:01:20.000000 scaled-0.9/scaled/utility/logging/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-02-12 04:01:20.000000 scaled-0.9/scaled/utility/zmq_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.680169 scaled-0.9/scaled/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/scaled/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-02-12 04:01:20.000000 scaled-0.9/scaled/worker/async_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-02-12 04:01:20.000000 scaled-0.9/scaled/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.676169 scaled-0.9/scaled.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-02-12 04:01:37.000000 scaled-0.9/scaled.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-02-12 04:01:37.000000 scaled-0.9/scaled.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 04:01:37.000000 scaled-0.9/scaled.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-12 04:01:37.000000 scaled-0.9/scaled.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-12 04:01:37.000000 scaled-0.9/scaled.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-12 04:01:37.000000 scaled-0.9/scaled.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 04:01:37.680169 scaled-0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:37.680169 scaled-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 04:01:20.000000 scaled-0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-02-12 04:01:20.000000 scaled-0.9/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-02-12 04:01:20.000000 scaled-0.9/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-12 04:01:20.000000 scaled-0.9/tests/test_worker_collection.py
```

### Comparing `scaled-0.7/.github/workflows/main.yml` & `scaled-0.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `scaled-0.7/LICENSE` & `scaled-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scaled-0.7/README.md` & `scaled-0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: scaled
+Version: 0.9
+Summary: Scale Distribution Framework
+Author-email: Zhuo Yin <zhuoyin@gmail.com>
+License: BSD-3-Clause
+Project-URL: Home, https://github.com/yzard/scaled
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Scaled
 This project is aiming the target that provides simple and efficient and reliable way for distributing computing 
 framework, centralized scheduler and stable protocol when client and worker talking to scheduler
 
 # Introduction
 The goal for this project should be as simple as possible
 - It built on top of zmq
@@ -19,48 +30,41 @@
 # How to use it
 
 ## Start local scheduler and cluster at the same time in the code
 
 ```python
 import random
 
-from scaled.client.client import Client
+from scaled.client import Client
 from scaled.cluster.combo import SchedulerClusterCombo
-from scaled.utility.zmq_config import ZMQConfig, ZMQType
-from scaled.utility.logging.scoped_logger import ScopedLogger
-from scaled.utility.logging.utility import setup_logger
 
 
 def calculate(sec: int):
-  return sec * 1
+    return sec * 1
 
 
 def main():
-  setup_logger()
-  config = ZMQConfig(type=ZMQType.tcp, host="127.0.0.1", port=2345)
-
-  cluster = SchedulerClusterCombo(address=config, n_workers=10, event_loop="uvloop")
-  client = Client(config=config)
+    address = "tcp://127.0.0.1:2345"
 
-  tasks = [random.randint(0, 100) for _ in range(100000)]
+    cluster = SchedulerClusterCombo(address=address, n_workers=10, event_loop="uvloop")
+    client = Client(address=address)
 
-  with ScopedLogger(f"submit {len(tasks)} tasks"):
+    tasks = [random.randint(0, 100) for _ in range(100000)]
     futures = [client.submit(calculate, i) for i in tasks]
 
-  with ScopedLogger(f"gather {len(futures)} results"):
     results = [future.result() for future in futures]
 
-  assert results == tasks
+    assert results == tasks
 
-  cluster.shutdown()
-  client.disconnect()
+    client.disconnect()
+    cluster.shutdown()
 
 
 if __name__ == "__main__":
-  main()
+    main()
 ```
 
 ## Start scheduler and cluster independently
 
 use `scaled_scheduler` to start scheduler, for example:
 ```bash
 scaled_scheduler --allocator-type queued tcp://0.0.0.0:8516
@@ -68,20 +72,21 @@
 
 use `scaled_cluster` to start workers:
 ```bash
 scaled_worker -n 10 tcp://127.0.0.1:8516
 ```
 
 Then you can write simply write client code as:
+
 ```python
-from scaled.utility.zmq_config import ZMQConfig, ZMQType
-from scaled.client.client import Client
+from scaled.client import Client
+
 
 def foobar(foo: int):
     return foo
 
-config = ZMQConfig(type=ZMQType.tcp, host="127.0.0.1", port=2345)
-client = Client(config=config)
+
+client = Client(address="tcp://127.0.0.1:2345")
 future = client.submit(foobar, 1)
 
 print(future.result())
-```
+```
```

### Comparing `scaled-0.7/benchmarks/dask_local_test.py` & `scaled-0.9/benchmarks/dask_local_test.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/benchmarks/dask_remote_test.py` & `scaled-0.9/benchmarks/dask_remote_test.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/benchmarks/scaled_test.py` & `scaled-0.9/benchmarks/scaled_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import random
 
-from scaled.client.client import Client
+from scaled.client import Client
 from scaled.cluster.combo import SchedulerClusterCombo
-from scaled.utility.zmq_config import ZMQConfig, ZMQType
+
 from scaled.utility.logging.scoped_logger import ScopedLogger
 from scaled.utility.logging.utility import setup_logger
 
 
 def sleep_print(sec: int):
     return sec * 1
 
 
 def main():
     setup_logger()
-    config = ZMQConfig(type=ZMQType.tcp, host="127.0.0.1", port=2345)
 
-    cluster = SchedulerClusterCombo(address=config, n_workers=10, event_loop="uvloop")
-    client = Client(config=config)
+    address = "tcp://127.0.0.1:2345"
+
+    cluster = SchedulerClusterCombo(address=address, n_workers=10, event_loop="uvloop")
+    client = Client(address=address)
 
     tasks = [random.randint(0, 100) for _ in range(100000)]
 
     with ScopedLogger(f"submit {len(tasks)} tasks"):
         futures = [client.submit(sleep_print, i) for i in tasks]
 
     with ScopedLogger(f"gather {len(futures)} results"):
         results = [future.result() for future in futures]
 
     assert results == tasks
 
-    cluster.shutdown()
     client.disconnect()
+    cluster.shutdown()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `scaled-0.7/pyproject.toml` & `scaled-0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/client/client.py` & `scaled-0.9/scaled/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,41 +24,41 @@
     TaskEcho,
     TaskEchoStatus,
     TaskResult, TaskStatus,
 )
 
 
 class Client:
-    def __init__(self, config: ZMQConfig, serializer: FunctionSerializerType = DefaultSerializer()):
+    def __init__(self, address: str, serializer: FunctionSerializerType = DefaultSerializer()):
         self._stop_event = threading.Event()
         self._connector = SyncConnector(
             stop_event=self._stop_event,
             prefix="C",
             context=zmq.Context.instance(),
             socket_type=zmq.DEALER,
             bind_or_connect="connect",
-            address=config,
+            address=ZMQConfig.from_string(address),
             callback=self.__on_receive,
         )
         self._serializer = serializer
 
         self._function_to_function_id_cache: dict[Callable, bytes] = dict()
         self._ready_function_ids: Set[bytes] = set()
         self._task_id_to_futures: Dict[bytes, Future] = dict()
 
         self._statistics_future: Optional[Future] = None
 
     def __del__(self):
         self.disconnect()
 
-    def submit(self, fn: Callable, *args) -> Future:
+    def submit(self, fn: Callable, *args, **kwargs) -> Future:
         function_id = self.__get_function_id(fn)
 
         task_id = uuid.uuid1().bytes
-        task = Task(task_id, function_id, b"", self._serializer.serialize_arguments(args))
+        task = Task(task_id, function_id, b"", self._serializer.serialize_arguments(args, kwargs))
         self._connector.send(MessageType.Task, task)
 
         future = Future()
         self._task_id_to_futures[task_id] = future
         return future
 
     def statistics(self):
```

### Comparing `scaled-0.7/scaled/cluster/cluster.py` & `scaled-0.9/scaled/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/cluster/combo.py` & `scaled-0.9/scaled/cluster/combo.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 from scaled.utility.zmq_config import ZMQConfig
 from scaled.cluster.cluster import ClusterProcess
 
 
 class SchedulerClusterCombo:
     def __init__(
         self,
-        address: ZMQConfig,
+        address: str,
         n_workers: int,
         heartbeat_interval: int = 1,
         event_loop: str = "builtin",
         worker_timeout_seconds: int = 10,
         function_timeout_seconds: int = 60,
         allocator_type: AllocatorType = AllocatorType.Queued,
         serializer: Serializer = DefaultSerializer(),
     ):
         self._stop_event = multiprocessing.get_context("spawn").Event()
         self._cluster = ClusterProcess(
             stop_event=self._stop_event,
-            address=address,
+            address=ZMQConfig.from_string(address),
             n_workers=n_workers,
             heartbeat_interval=heartbeat_interval,
             event_loop=event_loop,
             serializer=serializer,
         )
         self._scheduler = SchedulerProcess(
-            address=address,
+            address=ZMQConfig.from_string(address),
             stop_event=self._stop_event,
             allocator_type=allocator_type,
             worker_timeout_seconds=worker_timeout_seconds,
             function_timeout_seconds=function_timeout_seconds,
         )
 
         self._cluster.start()
```

### Comparing `scaled-0.7/scaled/cluster/scheduler.py` & `scaled-0.9/scaled/cluster/scheduler.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/entry_points/cluster.py` & `scaled-0.9/scaled/entry_points/cluster.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/entry_points/scheduler.py` & `scaled-0.9/scaled/entry_points/scheduler.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/io/async_binder.py` & `scaled-0.9/scaled/io/async_binder.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/io/async_connector.py` & `scaled-0.9/scaled/io/async_connector.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/io/sync_connector.py` & `scaled-0.9/scaled/io/sync_connector.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/protocol/python/message.py` & `scaled-0.9/scaled/protocol/python/message.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/protocol/python/serializer/default.py` & `scaled-0.9/scaled/protocol/python/serializer/default.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pickle
-from typing import Any, Callable, Tuple
+from typing import Any, Callable, Dict, Tuple
 
 import cloudpickle
 
 from scaled.protocol.python.serializer.mixins import Serializer
 
 
 class DefaultSerializer(Serializer):
@@ -12,19 +12,19 @@
         return cloudpickle.dumps(fn)
 
     @staticmethod
     def deserialize_function(payload: bytes) -> Callable:
         return cloudpickle.loads(payload)
 
     @staticmethod
-    def serialize_arguments(args: Tuple[Any, ...]) -> bytes:
-        return pickle.dumps(args, protocol=pickle.HIGHEST_PROTOCOL)
+    def serialize_arguments(args: Tuple[Any, ...], kwargs: Dict) -> bytes:
+        return pickle.dumps((args, kwargs), protocol=pickle.HIGHEST_PROTOCOL)
 
     @staticmethod
-    def deserialize_arguments(payload: bytes) -> Tuple[Any, ...]:
+    def deserialize_arguments(payload: bytes) -> Tuple[Tuple[Any, ...], Dict]:
         return pickle.loads(payload)
 
     @staticmethod
     def serialize_result(result: Any) -> bytes:
         return pickle.dumps(result, protocol=pickle.HIGHEST_PROTOCOL)
 
     @staticmethod
```

### Comparing `scaled-0.7/scaled/protocol/python/serializer/mixins.py` & `scaled-0.9/scaled/protocol/python/serializer/mixins.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import abc
-from typing import Any, Callable, Tuple, TypeVar
+from typing import Any, Callable, Dict, Tuple, TypeVar
 
 
 class Serializer(metaclass=abc.ABCMeta):
     @staticmethod
     @abc.abstractmethod
     def serialize_function(fn: Callable) -> bytes:
         raise NotImplementedError()
@@ -11,15 +11,15 @@
     @staticmethod
     @abc.abstractmethod
     def deserialize_function(payload: bytes) -> Callable:
         raise NotImplementedError()
 
     @staticmethod
     @abc.abstractmethod
-    def serialize_arguments(args: Tuple[Any, ...]) -> bytes:
+    def serialize_arguments(args: Tuple[Any, ...], kwargs: Dict) -> bytes:
         raise NotImplementedError()
 
     @staticmethod
     @abc.abstractmethod
     def deserialize_arguments(payload: bytes) -> Tuple[Any, ...]:
         raise NotImplementedError()
```

### Comparing `scaled-0.7/scaled/scheduler/client_manager/vanilla.py` & `scaled-0.9/scaled/scheduler/client_manager/vanilla.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/scheduler/function_manager/vanilla.py` & `scaled-0.9/scaled/scheduler/function_manager/vanilla.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/scheduler/main.py` & `scaled-0.9/scaled/scheduler/main.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/scheduler/mixins.py` & `scaled-0.9/scaled/scheduler/mixins.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/scheduler/task_manager/vanilla.py` & `scaled-0.9/scaled/scheduler/task_manager/vanilla.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/scheduler/worker_manager/allocators/mixins.py` & `scaled-0.9/scaled/scheduler/worker_manager/allocators/mixins.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/scheduler/worker_manager/allocators/one_to_one.py` & `scaled-0.9/scaled/scheduler/worker_manager/allocators/one_to_one.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/scheduler/worker_manager/allocators/queued.py` & `scaled-0.9/scaled/scheduler/worker_manager/allocators/queued.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/scheduler/worker_manager/vanilla.py` & `scaled-0.9/scaled/scheduler/worker_manager/vanilla.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/utility/event_loop.py` & `scaled-0.9/scaled/utility/event_loop.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/utility/logging/decorators.py` & `scaled-0.9/scaled/utility/logging/decorators.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/utility/logging/scoped_logger.py` & `scaled-0.9/scaled/utility/logging/scoped_logger.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/utility/logging/utility.py` & `scaled-0.9/scaled/utility/logging/utility.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/utility/zmq_config.py` & `scaled-0.9/scaled/utility/zmq_config.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/worker/async_agent.py` & `scaled-0.9/scaled/worker/async_agent.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/scaled/worker/worker.py` & `scaled-0.9/scaled/worker/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,21 +135,21 @@
 
         task = self._task_queue.get()
         try:
             if task.function_id not in self._cached_functions:
                 self._cached_functions[task.function_id] = self._serializer.deserialize_function(task.function_content)
 
             function = self._cached_functions[task.function_id]
-            args = self._serializer.deserialize_arguments(task.function_args)
-            result = self._serializer.serialize_result(function(*args))
+            args, kwargs = self._serializer.deserialize_arguments(task.function_args)
+            result = self._serializer.serialize_result(function(*args, **kwargs))
             self._agent_connector.send(MessageType.TaskResult, TaskResult(task.task_id, TaskStatus.Success, result))
         except Exception as e:
             logging.exception(f"{self.get_prefix()} error when processing {task=}:")
             self._agent_connector.send(
-                MessageType.TaskResult, TaskResult(task.task_id, TaskStatus.Failed, str(e).encode())
+                MessageType.TaskResult, TaskResult(task.task_id,  TaskStatus.Failed, str(e).encode())
             )
 
     def __on_connector_receive(self, message_type: MessageType, message: MessageVariant):
         if message_type == MessageType.Task:
             self.__connector_process_task(message)
             return
```

### Comparing `scaled-0.7/scaled.egg-info/SOURCES.txt` & `scaled-0.9/scaled.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 run_scheduler.py
 .github/workflows/main.yml
 benchmarks/dask_local_test.py
 benchmarks/dask_remote_test.py
 benchmarks/scaled_test.py
 scaled/__init__.py
 scaled/about.py
+scaled/client.py
 scaled.egg-info/PKG-INFO
 scaled.egg-info/SOURCES.txt
 scaled.egg-info/dependency_links.txt
 scaled.egg-info/entry_points.txt
 scaled.egg-info/requires.txt
 scaled.egg-info/top_level.txt
-scaled/client/__init__.py
-scaled/client/client.py
 scaled/cluster/__init__.py
 scaled/cluster/cluster.py
 scaled/cluster/combo.py
 scaled/cluster/scheduler.py
 scaled/entry_points/__init__.py
 scaled/entry_points/cluster.py
 scaled/entry_points/scheduler.py
```

### Comparing `scaled-0.7/tests/test_client.py` & `scaled-0.9/tests/test_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 import random
 
 import unittest
 
-from scaled.client.client import Client
-from scaled.utility.zmq_config import ZMQConfig, ZMQType
+from scaled.client import Client
 from scaled.utility.logging.scoped_logger import ScopedLogger
 from scaled.utility.logging.utility import setup_logger
 
 
 def sleep_print(sec: int):
     # time.sleep(sec)
     return sec * 1
@@ -16,25 +15,23 @@
 
 class TestClient(unittest.TestCase):
     def setUp(self) -> None:
         setup_logger()
 
     def test_client(self):
         # need server
-        config = ZMQConfig(type=ZMQType.tcp, host="127.0.0.1", port=2345)
-        client = Client(config=config)
+        client = Client(address="tcp://127.0.0.1:2345")
 
         tasks = [random.randint(0, 100) for _ in range(10000)]
         with ScopedLogger(f"submit {len(tasks)} tasks"):
             futures = [client.submit(sleep_print, i) for i in tasks]
 
         with ScopedLogger(f"gather {len(futures)} results"):
             results = [future.result() for future in futures]
 
         self.assertEqual(results, tasks)
         client.disconnect()
 
     def test_monitor(self):
-        config = ZMQConfig(type=ZMQType.tcp, host="127.0.0.1", port=2345)
-        client = Client(config=config)
+        client = Client(address="tcp://127.0.0.1:2345")
         print(json.dumps(client.statistics(), indent=4))
         client.disconnect()
```

### Comparing `scaled-0.7/tests/test_worker.py` & `scaled-0.9/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `scaled-0.7/tests/test_worker_collection.py` & `scaled-0.9/tests/test_worker_collection.py`

 * *Files identical despite different names*

