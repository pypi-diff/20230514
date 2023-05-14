# Comparing `tmp/aec-cli-2.8.0.tar.gz` & `tmp/aec-cli-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/aec/aec/dist/.tmp-o6qfwa9_/aec-cli-2.8.0.tar", last modified: Thu Mar 16 22:39:57 2023, max compression
+gzip compressed data, was "/home/runner/work/aec/aec/dist/.tmp-q7ingtiv/aec-cli-2.9.0.tar", last modified: Wed Apr  5 08:07:28 2023, max compression
```

## Comparing `aec-cli-2.8.0.tar` & `aec-cli-2.9.0.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:57.000000 aec-cli-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-16 22:39:22.000000 aec-cli-2.8.0/.darglint
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:57.000000 aec-cli-2.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-16 22:39:22.000000 aec-cli-2.8.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-16 22:39:22.000000 aec-cli-2.8.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:57.000000 aec-cli-2.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-16 22:39:22.000000 aec-cli-2.8.0/.github/workflows/drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-16 22:39:22.000000 aec-cli-2.8.0/.github/workflows/pythonapp.yml
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-16 22:39:22.000000 aec-cli-2.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-16 22:39:22.000000 aec-cli-2.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-16 22:39:22.000000 aec-cli-2.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-16 22:39:22.000000 aec-cli-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-16 22:39:22.000000 aec-cli-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-03-16 22:39:22.000000 aec-cli-2.8.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-03-16 22:39:57.000000 aec-cli-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-03-16 22:39:22.000000 aec-cli-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:57.000000 aec-cli-2.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-03-16 22:39:22.000000 aec-cli-2.8.0/docs/ami.md
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-16 22:39:22.000000 aec-cli-2.8.0/docs/compute-optimizer.md
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-03-16 22:39:22.000000 aec-cli-2.8.0/docs/ec2.md
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-16 22:39:22.000000 aec-cli-2.8.0/docs/ssm.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-16 22:39:22.000000 aec-cli-2.8.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-03-16 22:39:22.000000 aec-cli-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-16 22:39:22.000000 aec-cli-2.8.0/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 22:39:57.000000 aec-cli-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-16 22:39:22.000000 aec-cli-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:57.000000 aec-cli-2.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:57.000000 aec-cli-2.8.0/src/aec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:57.000000 aec-cli-2.8.0/src/aec/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/command/ami.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/command/compute_optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20014 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/command/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/command/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:57.000000 aec-cli-2.8.0/src/aec/config-example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/config-example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/config-example/ec2.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:57.000000 aec-cli-2.8.0/src/aec/config-example/userdata/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/config-example/userdata/amzn-install-docker.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:57.000000 aec-cli-2.8.0/src/aec/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/util/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/util/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/util/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/util/docgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/util/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/util/ec2_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/util/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-16 22:39:22.000000 aec-cli-2.8.0/src/aec/util/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:57.000000 aec-cli-2.8.0/src/aec_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-03-16 22:39:57.000000 aec-cli-2.8.0/src/aec_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-16 22:39:57.000000 aec-cli-2.8.0/src/aec_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 22:39:57.000000 aec-cli-2.8.0/src/aec_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 22:39:57.000000 aec-cli-2.8.0/src/aec_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-16 22:39:57.000000 aec-cli-2.8.0/src/aec_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-16 22:39:57.000000 aec-cli-2.8.0/src/aec_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:57.000000 aec-cli-2.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 22:39:22.000000 aec-cli-2.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-03-16 22:39:22.000000 aec-cli-2.8.0/tests/test_ami.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-16 22:39:22.000000 aec-cli-2.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-16 22:39:22.000000 aec-cli-2.8.0/tests/test_compute_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-16 22:39:22.000000 aec-cli-2.8.0/tests/test_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-16 22:39:22.000000 aec-cli-2.8.0/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-03-16 22:39:22.000000 aec-cli-2.8.0/tests/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-16 22:39:22.000000 aec-cli-2.8.0/tests/test_ssm.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-16 22:39:22.000000 aec-cli-2.8.0/toast.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:07:28.000000 aec-cli-2.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:07:28.000000 aec-cli-2.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-05 08:06:01.000000 aec-cli-2.9.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-05 08:06:01.000000 aec-cli-2.9.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:07:28.000000 aec-cli-2.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-05 08:06:01.000000 aec-cli-2.9.0/.github/workflows/drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-05 08:06:01.000000 aec-cli-2.9.0/.github/workflows/pythonapp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-05 08:06:01.000000 aec-cli-2.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-05 08:06:01.000000 aec-cli-2.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-05 08:06:01.000000 aec-cli-2.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-05 08:06:01.000000 aec-cli-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-05 08:06:01.000000 aec-cli-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-05 08:06:01.000000 aec-cli-2.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-05 08:07:28.000000 aec-cli-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-05 08:06:01.000000 aec-cli-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:07:28.000000 aec-cli-2.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-05 08:06:01.000000 aec-cli-2.9.0/docs/ami.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-05 08:06:01.000000 aec-cli-2.9.0/docs/compute-optimizer.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-04-05 08:06:01.000000 aec-cli-2.9.0/docs/ec2.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-04-05 08:06:01.000000 aec-cli-2.9.0/docs/ssm.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-05 08:06:01.000000 aec-cli-2.9.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-05 08:06:01.000000 aec-cli-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-05 08:06:01.000000 aec-cli-2.9.0/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 08:07:28.000000 aec-cli-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-05 08:06:01.000000 aec-cli-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:07:28.000000 aec-cli-2.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:07:28.000000 aec-cli-2.9.0/src/aec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:07:28.000000 aec-cli-2.9.0/src/aec/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/command/ami.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/command/compute_optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20602 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/command/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/command/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:07:28.000000 aec-cli-2.9.0/src/aec/config-example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/config-example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/config-example/ec2.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:07:28.000000 aec-cli-2.9.0/src/aec/config-example/userdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/config-example/userdata/amzn-install-docker.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:07:28.000000 aec-cli-2.9.0/src/aec/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/util/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/util/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/util/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/util/docgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/util/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/util/ec2_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/util/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-05 08:06:01.000000 aec-cli-2.9.0/src/aec/util/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:07:28.000000 aec-cli-2.9.0/src/aec_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-05 08:07:28.000000 aec-cli-2.9.0/src/aec_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-05 08:07:28.000000 aec-cli-2.9.0/src/aec_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 08:07:28.000000 aec-cli-2.9.0/src/aec_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 08:07:28.000000 aec-cli-2.9.0/src/aec_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-05 08:07:28.000000 aec-cli-2.9.0/src/aec_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-05 08:07:28.000000 aec-cli-2.9.0/src/aec_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:07:28.000000 aec-cli-2.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:06:01.000000 aec-cli-2.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-05 08:06:01.000000 aec-cli-2.9.0/tests/test_ami.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-05 08:06:01.000000 aec-cli-2.9.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-05 08:06:01.000000 aec-cli-2.9.0/tests/test_compute_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-05 08:06:01.000000 aec-cli-2.9.0/tests/test_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-05 08:06:01.000000 aec-cli-2.9.0/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-04-05 08:06:01.000000 aec-cli-2.9.0/tests/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-05 08:06:01.000000 aec-cli-2.9.0/tests/test_ssm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-05 08:06:01.000000 aec-cli-2.9.0/toast.yml
```

### Comparing `aec-cli-2.8.0/.github/release-drafter.yml` & `aec-cli-2.9.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/.github/workflows/pythonapp.yml` & `aec-cli-2.9.0/.github/workflows/pythonapp.yml`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/.pre-commit-config.yaml` & `aec-cli-2.9.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -9,29 +9,23 @@
         stages: [push]
       - id: end-of-file-fixer
         stages: [push]
   - repo: https://github.com/crate-ci/typos
     rev: v1.13.23
     hooks:
       - id: typos
+        stages: [push]
   # vscode & the cli uses these too so they has been installed into the virtualenv
   - repo: local
     hooks:
       - id: black
         name: black
         entry: .venv/bin/black
         language: system
         types: [python]
-      # use docformatter from the venv so that it reads from pyproject.toml
-      - id: docformatter
-        name: docformatter
-        entry: .venv/bin/docformatter
-        args: [--in-place]
-        language: system
-        types: [python]
       - id: ruff
         name: ruff
         entry: .venv/bin/ruff
         language: system
         types: [python]
   # these hooks require the project's virtualenv
   - repo: local
```

### Comparing `aec-cli-2.8.0/CONTRIBUTING.md` & `aec-cli-2.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/LICENSE` & `aec-cli-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/Makefile` & `aec-cli-2.9.0/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 ## create venv and install this package and hooks
 install: $(venv) node_modules $(if $(value CI),,install-hooks)
 
 ## format all code
 format: $(venv)
 	$(venv)/bin/black .
-	$(venv)/bin/docformatter . --in-place -e build dist node_modules typings
 	$(venv)/bin/ruff .
 
 ## lint code and run static type check
 check: lint pyright
 
 ## lint and format code
 lint: $(venv)
```

### Comparing `aec-cli-2.8.0/PKG-INFO` & `aec-cli-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aec-cli
-Version: 2.8.0
+Version: 2.9.0
 Summary: AWS EC2 CLI
 License: MIT License
         
         Copyright (c) 2019 SEEK
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `aec-cli-2.8.0/README.md` & `aec-cli-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/docs/ami.md` & `aec-cli-2.9.0/docs/ami.md`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/docs/compute-optimizer.md` & `aec-cli-2.9.0/docs/compute-optimizer.md`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/docs/ec2.md` & `aec-cli-2.9.0/docs/ec2.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 Run `aec ec2 -h` for help:
 
 <!-- [[[cog
 from aec.main import build_parser
 cog.out(f"```\n{build_parser()._subparsers._actions[1].choices['ec2'].format_help()}```")
 ]]] -->
+
 ```
 usage: aec ec2 [-h] {create-key-pair,describe,launch,logs,modify,start,stop,tag,tags,status,templates,terminate,user-data} ...
 
 optional arguments:
   -h, --help            show this help message and exit
 
 subcommands:
@@ -32,14 +33,15 @@
     tag                 Tag EC2 instance(s).
     tags                List EC2 instances or volumes with their tags.
     status              Describe instances status checks.
     templates           Describe launch templates.
     terminate           Terminate EC2 instance.
     user-data           Describe user data for an instance.
 ```
+
 <!-- [[[end]]] -->
 
 Launch an instance named `food baby` from the [ec2 launch template](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-launch-templates.html) named `yummy`:
 
 ```
 aec ec2 launch "food baby" --template yummy
 ```
@@ -69,22 +71,24 @@
 ```
 
 List all instances in the region:
 
 <!-- [[[cog
 cog.out(f"```\n{docs('aec ec2 describe', ec2.describe(config))}\n```")
 ]]] -->
+
 ```
 aec ec2 describe
 
-  InstanceId            State     Name    Type       DnsName                                      LaunchTime                  ImageId  
+  InstanceId            State     Name    Type       DnsName                                      LaunchTime                  ImageId
  ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
-  i-b5f2c2719ad4a4204   running   alice   t3.small   ec2-54-214-90-201.compute-1.amazonaws.com    2023-03-15 23:25:13+00:00   ami-03cf127a  
+  i-b5f2c2719ad4a4204   running   alice   t3.small   ec2-54-214-90-201.compute-1.amazonaws.com    2023-03-15 23:25:13+00:00   ami-03cf127a
   i-17227103cbf97cb86   running   sam     t3.small   ec2-54-214-204-133.compute-1.amazonaws.com   2023-03-15 23:25:14+00:00   ami-03cf127a
 ```
+
 <!-- [[[end]]] -->
 
 List instances containing `gaga` in the name:
 
 ```
 aec ec2 describe -q gaga
 ```
@@ -103,18 +107,18 @@
 
 Show running instances sorted by date started (ie: LaunchTime), oldest first:
 
 ```
 aec ec2 describe -r -s LaunchTime
 ```
 
-Show a custom set of columns
+Show a custom set of [columns](#columns)
 
 ```
-aec ec2 describe -c SubnetId,Name
+aec ec2 describe -c Name,SubnetId,Volumes
 ```
 
 Show instances and all their tags:
 
 ```
 aec ec2 tags
 
@@ -183,7 +187,63 @@
 ```
 aec ec2 describe -it i-02a840e0ca609c432 -c StateReason
 
   StateReason
  ─────────────────────────────────────────────────────────────────────────────────────────────
   {'Code': 'Client.InternalError', 'Message': 'Client.InternalError: Client error on launch'}
 ```
+
+## Columns
+
+Columns special to aec:
+
+- `DnsName` - PublicDnsName if available otherwise PrivateDnsName
+- `Name` - Name tag
+- `State` - state name
+- `Type` - instance type
+- `Volumes` - volumes attached to the instance
+
+Columns returned by the EC2 API:
+
+```
+AmiLaunchIndex
+Architecture
+BlockDeviceMappings
+CapacityReservationSpecification
+ClientToken
+CpuOptions
+CurrentInstanceBootMode
+EbsOptimized
+EnaSupport
+EnclaveOptions
+HibernationOptions
+Hypervisor
+IamInstanceProfile
+ImageId
+InstanceId
+InstanceType
+KeyName
+LaunchTime
+MaintenanceOptions
+MetadataOptions
+Monitoring
+NetworkInterfaces
+Placement
+PlatformDetails
+PrivateDnsName
+PrivateDnsNameOptions
+PrivateIpAddress
+ProductCodes
+PublicDnsName
+RootDeviceName
+RootDeviceType
+SecurityGroups
+SourceDestCheck
+State
+StateTransitionReason
+SubnetId
+Tags
+UsageOperation
+UsageOperationUpdateTime
+VirtualizationType
+VpcId
+```
```

### Comparing `aec-cli-2.8.0/docs/ssm.md` & `aec-cli-2.9.0/docs/ssm.md`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/pyproject.toml` & `aec-cli-2.9.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -4,37 +4,36 @@
 dynamic = ["version"]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["AWS", "EC2", "command line", "cli"]
 classifiers = ["License :: OSI Approved :: MIT License"]
 requires-python = ">=3.7"
 dependencies = [
-    "boto3==1.26.89",
+    "boto3==1.26.106",
     "importlib_resources==5.12.0",
     "pytoml==0.1.21",
-    "pytz==2022.7.1",
+    "pytz==2023.3",
     "requests==2.28.2",
-    "rich==13.3.2",
+    "rich==13.3.3",
     "typing_extensions==4.5.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black~=23.1",
     "build~=0.7",
-    "boto3-stubs[ec2,compute-optimizer,ssm,s3]==1.26.89",
+    "boto3-stubs[ec2,compute-optimizer,ssm,s3]",
     "cogapp~=3.3",
     "darglint~=1.8",
-    "docformatter~=1.5",
-    "moto[ec2]==4.1.4",
+    "moto[ec2]~=4.1",
     "pre-commit~=2.20",
     "pyfakefs~=5.1",
     "pytest~=7.2",
     "pytest-mock~=3.8",
-    "ruff~=0.0.254",
+    "ruff~=0.0.259",
     "twine~=4.0",
 ]
 
 [project.scripts]
 aec = "aec.main:main"
 
 [project.urls]
@@ -42,23 +41,18 @@
 
 [build-system]
 requires = ["setuptools", "setuptools_scm[toml]", "wheel"]
 
 # enable setuptools_scm to set the version based on git tags
 [tool.setuptools_scm]
 
-[tool.black]
 # use PyCharm default line length of 120
-line-length = 120
 
-[tool.docformatter]
-pre-summary-newline = true
-recursive = true
-wrap-descriptions = 120
-wrap-summaries = 120
+[tool.black]
+line-length = 120
 
 [tool.ruff]
 line-length = 120
 
 # rules to enable/ignore
 select = [
     # pyflakes
@@ -89,26 +83,22 @@
     "ANN102",
     "ANN204",
     # allow == True because pandas dataframes overload equality
     "E712",
 ]
 # first-party imports for sorting
 src = ["src"]
-# pyupgrade target
-target-version = "py37"
 fix = true
 show-fixes = true
 
 [tool.ruff.pyupgrade]
 # Preserve types, even if a file imports `from __future__ import annotations`.
 keep-runtime-typing = true
 
 [tool.ruff.per-file-ignores]
-# imports in __init__.py don't need to be used in __init__.py
-"__init__.py" = ["F401"]
 # test functions don't need return types
 "tests/*" = ["ANN201", "ANN202"]
 # main.py can have long lines
 "src/aec/main.py" = ["E501"]
 
 [tool.ruff.flake8-annotations]
 # allow *args: Any, **kwargs: Any
```

### Comparing `aec-cli-2.8.0/src/aec/command/ami.py` & `aec-cli-2.9.0/src/aec/command/ami.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec/command/compute_optimizer.py` & `aec-cli-2.9.0/src/aec/command/compute_optimizer.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec/command/ec2.py` & `aec-cli-2.9.0/src/aec/command/ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 import base64
 import os
 import os.path
+from collections import defaultdict
 from time import sleep
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, cast
 
 import boto3
 from typing_extensions import TypedDict
 
 from aec.util.ec2 import describe_running_instances_names
 from aec.util.errors import NoInstancesError
 from aec.util.threads import executor
 
 if TYPE_CHECKING:
     from mypy_boto3_ec2.literals import InstanceTypeType
     from mypy_boto3_ec2.type_defs import (
         BlockDeviceMappingTypeDef,
+        DescribeVolumesResultTypeDef,
         FilterTypeDef,
         InstanceStatusSummaryTypeDef,
         TagSpecificationTypeDef,
         TagTypeDef,
     )
 
 import aec.command.ami as ami_cmd
@@ -36,14 +38,15 @@
 class Instance(TypedDict, total=False):
     InstanceId: str
     State: str
     Name: Optional[str]
     Type: str
     DnsName: str
     SubnetId: str
+    Volumes: List[str]
 
 
 def launch(
     config: Config,
     name: str,
     ami: Optional[str] = None,
     template: Optional[str] = None,
@@ -218,23 +221,35 @@
 
     filters = to_filters(ident, name_match)
     if show_running_only:
         filters.append({"Name": "instance-state-name", "Values": ["pending", "running"]})
 
     kwargs: Dict[str, Any] = {"MaxResults": 1000, "Filters": filters}
 
-    response = ec2_client.describe_instances(**kwargs)
-
-    # import json; print(json.dumps(response))
+    response_fut = executor.submit(ec2_client.describe_instances, **kwargs)
 
     cols = columns.split(",")
 
     # don't sort by cols we aren't showing
     sort_cols = [sc for sc in sort_by.split(",") if sc in cols]
 
+    if "Volumes" in columns:
+        # fetch volume info
+        volumes_response: DescribeVolumesResultTypeDef = executor.submit(ec2_client.describe_volumes).result()
+        volumes: Dict[str, List[str]] = defaultdict(list)
+        for v in volumes_response["Volumes"]:
+            for a in v["Attachments"]:
+                volumes[a["InstanceId"]].append(f'Size={v["Size"]} GiB')
+    else:
+        volumes = {}
+
+    response = response_fut.result()
+
+    # import json; print(json.dumps(response))
+
     instances: List[Instance] = []
     while True:
         for r in response["Reservations"]:
             for i in r["Instances"]:
                 if include_terminated or i["State"]["Name"] != "terminated":
                     desc: Instance = {}
 
@@ -242,17 +257,17 @@
                         if col == "State":
                             desc[col] = i["State"]["Name"]
                         elif col == "Name":
                             desc[col] = util_tags.get_value(i, "Name")
                         elif col == "Type":
                             desc[col] = i["InstanceType"]
                         elif col == "DnsName":
-                            desc[col] = (
-                                i["PublicDnsName"] if i.get("PublicDnsName", None) != "" else i["PrivateDnsName"]
-                            )
+                            desc[col] = i["PublicDnsName"] or i["PrivateDnsName"]
+                        elif col == "Volumes":
+                            desc[col] = volumes.get(i["InstanceId"], [])
                         else:
                             desc[col] = i.get(col, None)
 
                     instances.append(desc)
 
         next_token = response.get("NextToken", None)
         if next_token:
```

### Comparing `aec-cli-2.8.0/src/aec/command/ssm.py` & `aec-cli-2.9.0/src/aec/command/ssm.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec/config-example/ec2.toml` & `aec-cli-2.9.0/src/aec/config-example/ec2.toml`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec/config-example/userdata/amzn-install-docker.yaml` & `aec-cli-2.9.0/src/aec/config-example/userdata/amzn-install-docker.yaml`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec/main.py` & `aec-cli-2.9.0/src/aec/main.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec/util/cli.py` & `aec-cli-2.9.0/src/aec/util/cli.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec/util/config.py` & `aec-cli-2.9.0/src/aec/util/config.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec/util/configure.py` & `aec-cli-2.9.0/src/aec/util/configure.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec/util/display.py` & `aec-cli-2.9.0/src/aec/util/display.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec/util/docgen.py` & `aec-cli-2.9.0/src/aec/util/docgen.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec/util/ec2.py` & `aec-cli-2.9.0/src/aec/util/ec2.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec/util/ec2_types.py` & `aec-cli-2.9.0/src/aec/util/ec2_types.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec/util/errors.py` & `aec-cli-2.9.0/src/aec/util/errors.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/src/aec_cli.egg-info/PKG-INFO` & `aec-cli-2.9.0/src/aec_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aec-cli
-Version: 2.8.0
+Version: 2.9.0
 Summary: AWS EC2 CLI
 License: MIT License
         
         Copyright (c) 2019 SEEK
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `aec-cli-2.8.0/src/aec_cli.egg-info/SOURCES.txt` & `aec-cli-2.9.0/src/aec_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.darglint
 .gitignore
 .pre-commit-config.yaml
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
```

### Comparing `aec-cli-2.8.0/tests/test_ami.py` & `aec-cli-2.9.0/tests/test_ami.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/tests/test_cli.py` & `aec-cli-2.9.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/tests/test_compute_optimizer.py` & `aec-cli-2.9.0/tests/test_compute_optimizer.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/tests/test_ec2.py` & `aec-cli-2.9.0/tests/test_ec2.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,23 +173,14 @@
 
     instances = describe(config=mock_aws_config)
     print(instances)
 
     assert len(instances) == 1
 
 
-def test_tag(mock_aws_config: Config):
-    launch(mock_aws_config, "alice", ami_id)
-
-    instances = tag(mock_aws_config, ["Project=top secret"], "alice")
-
-    assert len(instances) == 1
-    assert instances[0]["Tag: Project"] == "top secret"
-
-
 def test_describe_by_name(mock_aws_config: Config):
     launch(mock_aws_config, "alice", ami_id)
     launch(mock_aws_config, "alex", ami_id)
 
     instances = describe(config=mock_aws_config, ident="alice")
 
     assert len(instances) == 1
@@ -256,34 +247,45 @@
 
 def test_describe_columns(mock_aws_config: Config):
     launch(mock_aws_config, "sam", ami_id)
 
     del mock_aws_config["key_name"]
     launch(mock_aws_config, "alice", ami_id)
 
-    instances = describe(config=mock_aws_config, columns="SubnetId,Name,MissingKey")
+    instances = describe(config=mock_aws_config, columns="SubnetId,Name,MissingKey,Volumes")
     print(instances)
 
     assert len(instances) == 2
     assert instances[0]["Name"] == "alice"
     assert instances[1]["Name"] == "sam"
     assert "subnet" in instances[0]["SubnetId"]
     assert "subnet" in instances[1]["SubnetId"]
+    assert instances[0]["Volumes"] == ["Size=15 GiB"]
+    assert instances[1]["Volumes"] == ["Size=15 GiB"]
 
     # MissingKey will appear without values
     assert instances[0]["MissingKey"] is None  # type: ignore
     assert instances[1]["MissingKey"] is None  # type: ignore
 
 
 def describe_instance0(region_name: str, instance_id: str):
     ec2_client = boto3.client("ec2", region_name=region_name)
     instances = ec2_client.describe_instances(InstanceIds=[instance_id])
     return instances["Reservations"][0]["Instances"][0]
 
 
+def test_tag(mock_aws_config: Config):
+    launch(mock_aws_config, "alice", ami_id)
+
+    instances = tag(mock_aws_config, ["Project=top secret"], "alice")
+
+    assert len(instances) == 1
+    assert instances[0]["Tag: Project"] == "top secret"
+
+
 def test_tags(mock_aws_config: Config):
     mock_aws_config["additional_tags"] = {"Owner": "alice@testlab.io", "Project": "top secret"}
     launch(mock_aws_config, "alice", ami_id)
 
     instances = instance_tags(config=mock_aws_config)
 
     assert len(instances) == 1
```

### Comparing `aec-cli-2.8.0/tests/test_ssm.py` & `aec-cli-2.9.0/tests/test_ssm.py`

 * *Files identical despite different names*

### Comparing `aec-cli-2.8.0/toast.yml` & `aec-cli-2.9.0/toast.yml`

 * *Files identical despite different names*

