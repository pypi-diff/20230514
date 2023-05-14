# Comparing `tmp/nasim-0.9.0.tar.gz` & `tmp/nasim-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nasim-0.9.0.tar", last modified: Mon Dec 20 22:08:01 2021, max compression
+gzip compressed data, was "dist/nasim-0.9.1.tar", last modified: Thu May 19 11:46:28 2022, max compression
```

## Comparing `nasim-0.9.0.tar` & `nasim-0.9.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2021-12-20 22:08:01.000000 nasim-0.9.0/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     7261 2021-12-20 22:08:01.000000 nasim-0.9.0/PKG-INFO
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     5303 2021-12-20 21:57:28.000000 nasim-0.9.0/README.rst
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2021-12-20 22:08:01.000000 nasim-0.9.0/nasim/
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     6287 2020-11-20 00:24:44.000000 nasim-0.9.0/nasim/__init__.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2021-12-20 22:08:01.000000 nasim-0.9.0/nasim/agents/
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)        0 2020-02-22 04:38:22.000000 nasim-0.9.0/nasim/agents/__init__.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     3487 2020-11-20 00:24:44.000000 nasim-0.9.0/nasim/agents/bruteforce_agent.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)    13374 2020-11-23 05:05:07.000000 nasim-0.9.0/nasim/agents/dqn_agent.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     8005 2021-12-20 22:00:43.000000 nasim-0.9.0/nasim/agents/keyboard_agent.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)    10171 2021-12-20 18:50:32.000000 nasim-0.9.0/nasim/agents/ql_agent.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)    12068 2020-11-23 05:05:07.000000 nasim-0.9.0/nasim/agents/ql_replay_agent.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     3261 2020-11-20 00:24:44.000000 nasim-0.9.0/nasim/agents/random_agent.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2161 2020-09-20 07:59:34.000000 nasim-0.9.0/nasim/demo.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2021-12-20 22:08:01.000000 nasim-0.9.0/nasim/envs/
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)       67 2020-10-18 02:11:31.000000 nasim-0.9.0/nasim/envs/__init__.py
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)    25790 2021-03-15 00:07:26.000000 nasim-0.9.0/nasim/envs/action.py
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)    14390 2020-12-17 02:13:58.000000 nasim-0.9.0/nasim/envs/environment.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     1399 2020-08-01 13:05:07.000000 nasim-0.9.0/nasim/envs/gym_env.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)    15697 2020-12-17 03:07:06.000000 nasim-0.9.0/nasim/envs/host_vector.py
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     9179 2021-03-15 00:07:26.000000 nasim-0.9.0/nasim/envs/network.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     6704 2021-12-20 21:55:23.000000 nasim-0.9.0/nasim/envs/observation.py
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)    17102 2021-12-20 17:43:58.000000 nasim-0.9.0/nasim/envs/render.py
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     9315 2021-12-20 19:05:00.000000 nasim-0.9.0/nasim/envs/state.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     3899 2020-08-11 11:39:18.000000 nasim-0.9.0/nasim/envs/utils.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2021-12-20 22:08:01.000000 nasim-0.9.0/nasim/scenarios/
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2617 2020-08-01 13:01:05.000000 nasim-0.9.0/nasim/scenarios/__init__.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2021-12-20 22:08:01.000000 nasim-0.9.0/nasim/scenarios/benchmark/
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     1810 2021-12-20 17:43:58.000000 nasim-0.9.0/nasim/scenarios/benchmark/__init__.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     3520 2021-12-20 18:37:07.000000 nasim-0.9.0/nasim/scenarios/benchmark/generated.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     3856 2020-08-12 10:38:10.000000 nasim-0.9.0/nasim/scenarios/benchmark/medium-multi-site.yaml
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2660 2020-08-12 10:26:27.000000 nasim-0.9.0/nasim/scenarios/benchmark/medium-single-site.yaml
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     2954 2020-10-18 02:11:31.000000 nasim-0.9.0/nasim/scenarios/benchmark/medium.yaml
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2264 2021-12-20 17:43:58.000000 nasim-0.9.0/nasim/scenarios/benchmark/small-honeypot.yaml
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2793 2020-08-11 11:34:52.000000 nasim-0.9.0/nasim/scenarios/benchmark/small-linear.yaml
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2145 2021-12-20 17:43:58.000000 nasim-0.9.0/nasim/scenarios/benchmark/small.yaml
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     1670 2020-08-11 03:41:51.000000 nasim-0.9.0/nasim/scenarios/benchmark/tiny-hard.yaml
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     1958 2020-08-10 23:02:30.000000 nasim-0.9.0/nasim/scenarios/benchmark/tiny-small.yaml
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     1464 2021-12-20 17:43:58.000000 nasim-0.9.0/nasim/scenarios/benchmark/tiny.yaml
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)    35703 2021-12-20 20:13:11.000000 nasim-0.9.0/nasim/scenarios/generator.py
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     3733 2020-10-18 02:11:31.000000 nasim-0.9.0/nasim/scenarios/host.py
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)    22733 2021-12-20 17:43:58.000000 nasim-0.9.0/nasim/scenarios/loader.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     7936 2021-12-20 21:58:57.000000 nasim-0.9.0/nasim/scenarios/scenario.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2003 2021-12-20 18:33:07.000000 nasim-0.9.0/nasim/scenarios/utils.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2021-12-20 22:08:01.000000 nasim-0.9.0/nasim.egg-info/
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     7261 2021-12-20 22:08:01.000000 nasim-0.9.0/nasim.egg-info/PKG-INFO
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     1363 2021-12-20 22:08:01.000000 nasim-0.9.0/nasim.egg-info/SOURCES.txt
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)        1 2021-12-20 22:08:01.000000 nasim-0.9.0/nasim.egg-info/dependency_links.txt
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)        1 2020-07-31 03:09:56.000000 nasim-0.9.0/nasim.egg-info/not-zip-safe
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)      259 2021-12-20 22:08:01.000000 nasim-0.9.0/nasim.egg-info/requires.txt
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)        6 2021-12-20 22:08:01.000000 nasim-0.9.0/nasim.egg-info/top_level.txt
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)       38 2021-12-20 22:08:01.000000 nasim-0.9.0/setup.cfg
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     1567 2021-12-20 18:12:29.000000 nasim-0.9.0/setup.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2021-12-20 22:08:01.000000 nasim-0.9.0/test/
--rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)        0 2020-10-18 02:11:31.000000 nasim-0.9.0/test/__init__.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)     1873 2020-08-09 11:20:30.000000 nasim-0.9.0/test/test_bruteforce.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)      534 2020-08-18 04:30:20.000000 nasim-0.9.0/test/test_generator.py
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)      978 2020-11-20 00:24:44.000000 nasim-0.9.0/test/test_gym_bruteforce.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2022-05-19 11:46:28.000000 nasim-0.9.1/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     7420 2022-05-19 11:46:28.000000 nasim-0.9.1/PKG-INFO
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     5430 2022-05-19 11:33:19.000000 nasim-0.9.1/README.rst
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2022-05-19 11:46:28.000000 nasim-0.9.1/nasim/
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     6287 2020-11-20 00:24:44.000000 nasim-0.9.1/nasim/__init__.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2022-05-19 11:46:28.000000 nasim-0.9.1/nasim/agents/
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)        0 2020-02-22 04:38:22.000000 nasim-0.9.1/nasim/agents/__init__.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     3487 2020-11-20 00:24:44.000000 nasim-0.9.1/nasim/agents/bruteforce_agent.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)    13374 2020-11-23 05:05:07.000000 nasim-0.9.1/nasim/agents/dqn_agent.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     8005 2021-12-20 22:00:43.000000 nasim-0.9.1/nasim/agents/keyboard_agent.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)    10171 2021-12-20 18:50:32.000000 nasim-0.9.1/nasim/agents/ql_agent.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)    12068 2020-11-23 05:05:07.000000 nasim-0.9.1/nasim/agents/ql_replay_agent.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     3261 2020-11-20 00:24:44.000000 nasim-0.9.1/nasim/agents/random_agent.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2161 2020-09-20 07:59:34.000000 nasim-0.9.1/nasim/demo.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2022-05-19 11:46:28.000000 nasim-0.9.1/nasim/envs/
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)       67 2020-10-18 02:11:31.000000 nasim-0.9.1/nasim/envs/__init__.py
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)    25790 2021-03-15 00:07:26.000000 nasim-0.9.1/nasim/envs/action.py
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)    14680 2022-05-19 11:19:13.000000 nasim-0.9.1/nasim/envs/environment.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     1399 2020-08-01 13:05:07.000000 nasim-0.9.1/nasim/envs/gym_env.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)    15697 2020-12-17 03:07:06.000000 nasim-0.9.1/nasim/envs/host_vector.py
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     9188 2022-05-19 11:29:43.000000 nasim-0.9.1/nasim/envs/network.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     6704 2021-12-20 21:55:23.000000 nasim-0.9.1/nasim/envs/observation.py
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)    17102 2021-12-20 17:43:58.000000 nasim-0.9.1/nasim/envs/render.py
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     9315 2021-12-20 19:05:00.000000 nasim-0.9.1/nasim/envs/state.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     3899 2020-08-11 11:39:18.000000 nasim-0.9.1/nasim/envs/utils.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2022-05-19 11:46:28.000000 nasim-0.9.1/nasim/scenarios/
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2617 2020-08-01 13:01:05.000000 nasim-0.9.1/nasim/scenarios/__init__.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2022-05-19 11:46:28.000000 nasim-0.9.1/nasim/scenarios/benchmark/
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     1810 2021-12-20 17:43:58.000000 nasim-0.9.1/nasim/scenarios/benchmark/__init__.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     3520 2021-12-20 18:37:07.000000 nasim-0.9.1/nasim/scenarios/benchmark/generated.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     3856 2020-08-12 10:38:10.000000 nasim-0.9.1/nasim/scenarios/benchmark/medium-multi-site.yaml
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2660 2020-08-12 10:26:27.000000 nasim-0.9.1/nasim/scenarios/benchmark/medium-single-site.yaml
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     2954 2020-10-18 02:11:31.000000 nasim-0.9.1/nasim/scenarios/benchmark/medium.yaml
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2264 2021-12-20 17:43:58.000000 nasim-0.9.1/nasim/scenarios/benchmark/small-honeypot.yaml
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2793 2020-08-11 11:34:52.000000 nasim-0.9.1/nasim/scenarios/benchmark/small-linear.yaml
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2145 2021-12-20 17:43:58.000000 nasim-0.9.1/nasim/scenarios/benchmark/small.yaml
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     1670 2020-08-11 03:41:51.000000 nasim-0.9.1/nasim/scenarios/benchmark/tiny-hard.yaml
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     1958 2020-08-10 23:02:30.000000 nasim-0.9.1/nasim/scenarios/benchmark/tiny-small.yaml
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     1464 2021-12-20 17:43:58.000000 nasim-0.9.1/nasim/scenarios/benchmark/tiny.yaml
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)    35703 2021-12-20 20:13:11.000000 nasim-0.9.1/nasim/scenarios/generator.py
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     3733 2020-10-18 02:11:31.000000 nasim-0.9.1/nasim/scenarios/host.py
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)    22733 2021-12-20 17:43:58.000000 nasim-0.9.1/nasim/scenarios/loader.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     7936 2021-12-20 21:58:57.000000 nasim-0.9.1/nasim/scenarios/scenario.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     2003 2021-12-20 18:33:07.000000 nasim-0.9.1/nasim/scenarios/utils.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2022-05-19 11:46:28.000000 nasim-0.9.1/nasim.egg-info/
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     7420 2022-05-19 11:46:28.000000 nasim-0.9.1/nasim.egg-info/PKG-INFO
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     1380 2022-05-19 11:46:28.000000 nasim-0.9.1/nasim.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)        1 2022-05-19 11:46:28.000000 nasim-0.9.1/nasim.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)        1 2020-07-31 03:09:56.000000 nasim-0.9.1/nasim.egg-info/not-zip-safe
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)      259 2022-05-19 11:46:28.000000 nasim-0.9.1/nasim.egg-info/requires.txt
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)        6 2022-05-19 11:46:28.000000 nasim-0.9.1/nasim.egg-info/top_level.txt
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)       38 2022-05-19 11:46:28.000000 nasim-0.9.1/setup.cfg
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)     1567 2022-05-19 11:36:09.000000 nasim-0.9.1/setup.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2022-05-19 11:46:28.000000 nasim-0.9.1/test/
+-rwxr-xr-x   0 jonathon  (1000) jonathon  (1000)        0 2020-10-18 02:11:31.000000 nasim-0.9.1/test/__init__.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     1873 2020-08-09 11:20:30.000000 nasim-0.9.1/test/test_bruteforce.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     1533 2022-05-19 11:27:58.000000 nasim-0.9.1/test/test_env.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)      534 2020-08-18 04:30:20.000000 nasim-0.9.1/test/test_generator.py
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)      978 2020-11-20 00:24:44.000000 nasim-0.9.1/test/test_gym_bruteforce.py
```

### Comparing `nasim-0.9.0/PKG-INFO` & `nasim-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nasim
-Version: 0.9.0
+Version: 0.9.1
 Summary: A simple and fast simulator for remote network pen-testing
 Home-page: https://networkattacksimulator.readthedocs.io
 Author: Jonathon Schwartz
 Author-email: Jonathon.Schwartz@anu.edu.au
 License: MIT
 Project-URL: Documentation, https://networkattacksimulator.readthedocs.io
 Project-URL: Source, https://github.com/Jjschwartz/NetworkAttackSimulator/
@@ -85,14 +85,18 @@
         
         .. _MIT: LICENSE
         
         
         What's new
         ----------
         
+        - 2022-05-19 (v 0.9.1) (MICRO release)
+        
+          + Fixed a few bugs and added some tests (thanks @simonsays1980 for the bug reports)
+        
         - 2021-12-20 (v 0.9.0) (MINOR release)
         
           + The value of a host is now observed when any level of access is gained on a host. This makes it so that agents can learn to decide whether to invest time in gaining root access on a host or not, depending on the host's value (thanks @jaromiru for the proposal).
           + Initial observation of reachable hosts now contains the host's address (thanks @jaromiru).
           + Added some support for custom address space bounds in when using scenario generator (thanks @jaromiru for the suggestion).
         
         - 2021-3-15 (v 0.8.0) (MINOR release)
```

### Comparing `nasim-0.9.0/README.rst` & `nasim-0.9.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,18 @@
 
 .. _MIT: LICENSE
 
 
 What's new
 ----------
 
+- 2022-05-19 (v 0.9.1) (MICRO release)
+
+  + Fixed a few bugs and added some tests (thanks @simonsays1980 for the bug reports)
+
 - 2021-12-20 (v 0.9.0) (MINOR release)
 
   + The value of a host is now observed when any level of access is gained on a host. This makes it so that agents can learn to decide whether to invest time in gaining root access on a host or not, depending on the host's value (thanks @jaromiru for the proposal).
   + Initial observation of reachable hosts now contains the host's address (thanks @jaromiru).
   + Added some support for custom address space bounds in when using scenario generator (thanks @jaromiru for the suggestion).
 
 - 2021-3-15 (v 0.8.0) (MINOR release)
```

### Comparing `nasim-0.9.0/nasim/__init__.py` & `nasim-0.9.1/nasim/__init__.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/agents/bruteforce_agent.py` & `nasim-0.9.1/nasim/agents/bruteforce_agent.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/agents/dqn_agent.py` & `nasim-0.9.1/nasim/agents/dqn_agent.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/agents/keyboard_agent.py` & `nasim-0.9.1/nasim/agents/keyboard_agent.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/agents/ql_agent.py` & `nasim-0.9.1/nasim/agents/ql_agent.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/agents/ql_replay_agent.py` & `nasim-0.9.1/nasim/agents/ql_replay_agent.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/agents/random_agent.py` & `nasim-0.9.1/nasim/agents/random_agent.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/demo.py` & `nasim-0.9.1/nasim/demo.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/envs/action.py` & `nasim-0.9.1/nasim/envs/action.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/envs/environment.py` & `nasim-0.9.1/nasim/envs/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,17 +254,17 @@
 
         if self._renderer is None:
             self._renderer = Viewer(self.network)
 
         if mode == "readable":
             self._renderer.render_readable(obs)
         else:
-            print(
+            raise NotImplementedError(
                 "Please choose correct render mode from :"
-                f"{self.rendering_modes}"
+                f"{self.metadata['rendering.modes']}"
             )
 
     def render_state(self, mode="readable", state=None):
         """Render state.
 
         See render module for more details on modes and symbols.
 
@@ -291,30 +291,34 @@
 
         if self._renderer is None:
             self._renderer = Viewer(self.network)
 
         if mode == "readable":
             self._renderer.render_readable_state(state)
         else:
-            print("Please choose correct render mode from :"
-                  f"{self.rendering_modes}")
+            raise NotImplementedError(
+                "Please choose correct render mode from : "
+                f"{self.metadata['rendering.modes']}"
+            )
 
     def render_action(self, action):
         """Renders human readable version of action.
 
         This is mainly useful for getting a text description of the action
         that corresponds to a given integer.
 
         Parameters
         ----------
-        action : int or Action
-            the action to render
+        action : Action or int or list or NumpyArray
+            Action to render. If not Action object, then if using
+            flat actions this should be an int and if using non-flat actions
+            this should be an indexable array.
         """
-        if isinstance(action, int):
-            action = self.action_space[action]
+        if not isinstance(action, Action):
+            action = self.action_space.get_action(action)
         print(action)
 
     def render_episode(self, episode, width=7, height=7):
         """Render an episode as sequence of network graphs, where an episode
         is a sequence of (state, action, reward, done) tuples generated from
         interactions with environment.
```

### Comparing `nasim-0.9.0/nasim/envs/gym_env.py` & `nasim-0.9.1/nasim/envs/gym_env.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/envs/host_vector.py` & `nasim-0.9.1/nasim/envs/host_vector.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/envs/network.py` & `nasim-0.9.1/nasim/envs/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         total = 0
         for host_value in self.sensitive_hosts.values():
             total += host_value
         return total
 
     def get_total_discovery_value(self):
         total = 0
-        for host in self.hosts:
+        for host in self.hosts.values():
             total += host.discovery_value
         return total
 
     def get_minimal_steps(self):
         return get_minimal_steps_to_goal(
             self.topology, self.sensitive_addresses
         )
```

### Comparing `nasim-0.9.0/nasim/envs/observation.py` & `nasim-0.9.1/nasim/envs/observation.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/envs/render.py` & `nasim-0.9.1/nasim/envs/render.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/envs/state.py` & `nasim-0.9.1/nasim/envs/state.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/envs/utils.py` & `nasim-0.9.1/nasim/envs/utils.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/__init__.py` & `nasim-0.9.1/nasim/scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/benchmark/__init__.py` & `nasim-0.9.1/nasim/scenarios/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/benchmark/generated.py` & `nasim-0.9.1/nasim/scenarios/benchmark/generated.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/benchmark/medium-multi-site.yaml` & `nasim-0.9.1/nasim/scenarios/benchmark/medium-multi-site.yaml`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/benchmark/medium-single-site.yaml` & `nasim-0.9.1/nasim/scenarios/benchmark/medium-single-site.yaml`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/benchmark/medium.yaml` & `nasim-0.9.1/nasim/scenarios/benchmark/medium.yaml`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/benchmark/small-honeypot.yaml` & `nasim-0.9.1/nasim/scenarios/benchmark/small-honeypot.yaml`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/benchmark/small-linear.yaml` & `nasim-0.9.1/nasim/scenarios/benchmark/small-linear.yaml`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/benchmark/small.yaml` & `nasim-0.9.1/nasim/scenarios/benchmark/small.yaml`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/benchmark/tiny-hard.yaml` & `nasim-0.9.1/nasim/scenarios/benchmark/tiny-hard.yaml`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/benchmark/tiny-small.yaml` & `nasim-0.9.1/nasim/scenarios/benchmark/tiny-small.yaml`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/benchmark/tiny.yaml` & `nasim-0.9.1/nasim/scenarios/benchmark/tiny.yaml`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/generator.py` & `nasim-0.9.1/nasim/scenarios/generator.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/host.py` & `nasim-0.9.1/nasim/scenarios/host.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/loader.py` & `nasim-0.9.1/nasim/scenarios/loader.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/scenario.py` & `nasim-0.9.1/nasim/scenarios/scenario.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim/scenarios/utils.py` & `nasim-0.9.1/nasim/scenarios/utils.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/nasim.egg-info/PKG-INFO` & `nasim-0.9.1/nasim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nasim
-Version: 0.9.0
+Version: 0.9.1
 Summary: A simple and fast simulator for remote network pen-testing
 Home-page: https://networkattacksimulator.readthedocs.io
 Author: Jonathon Schwartz
 Author-email: Jonathon.Schwartz@anu.edu.au
 License: MIT
 Project-URL: Documentation, https://networkattacksimulator.readthedocs.io
 Project-URL: Source, https://github.com/Jjschwartz/NetworkAttackSimulator/
@@ -85,14 +85,18 @@
         
         .. _MIT: LICENSE
         
         
         What's new
         ----------
         
+        - 2022-05-19 (v 0.9.1) (MICRO release)
+        
+          + Fixed a few bugs and added some tests (thanks @simonsays1980 for the bug reports)
+        
         - 2021-12-20 (v 0.9.0) (MINOR release)
         
           + The value of a host is now observed when any level of access is gained on a host. This makes it so that agents can learn to decide whether to invest time in gaining root access on a host or not, depending on the host's value (thanks @jaromiru for the proposal).
           + Initial observation of reachable hosts now contains the host's address (thanks @jaromiru).
           + Added some support for custom address space bounds in when using scenario generator (thanks @jaromiru for the suggestion).
         
         - 2021-3-15 (v 0.8.0) (MINOR release)
```

### Comparing `nasim-0.9.0/nasim.egg-info/SOURCES.txt` & `nasim-0.9.1/nasim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,9 +40,10 @@
 nasim/scenarios/benchmark/small-linear.yaml
 nasim/scenarios/benchmark/small.yaml
 nasim/scenarios/benchmark/tiny-hard.yaml
 nasim/scenarios/benchmark/tiny-small.yaml
 nasim/scenarios/benchmark/tiny.yaml
 test/__init__.py
 test/test_bruteforce.py
+test/test_env.py
 test/test_generator.py
 test/test_gym_bruteforce.py
```

### Comparing `nasim-0.9.0/setup.py` & `nasim-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     ]
 }
 
 extras['all'] = [item for group in extras.values() for item in group]
 
 setup(
     name='nasim',
-    version='0.9.0',
+    version='0.9.1',
     url="https://networkattacksimulator.readthedocs.io",
     description="A simple and fast simulator for remote network pen-testing",
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     author="Jonathon Schwartz",
     author_email="Jonathon.Schwartz@anu.edu.au",
     license="MIT",
```

### Comparing `nasim-0.9.0/test/test_bruteforce.py` & `nasim-0.9.1/test/test_bruteforce.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/test/test_generator.py` & `nasim-0.9.1/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `nasim-0.9.0/test/test_gym_bruteforce.py` & `nasim-0.9.1/test/test_gym_bruteforce.py`

 * *Files identical despite different names*

