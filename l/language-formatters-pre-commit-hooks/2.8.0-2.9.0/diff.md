# Comparing `tmp/language_formatters_pre_commit_hooks-2.8.0.tar.gz` & `tmp/language_formatters_pre_commit_hooks-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "language_formatters_pre_commit_hooks-2.8.0.tar", last modified: Fri Mar 17 13:29:26 2023, max compression
+gzip compressed data, was "language_formatters_pre_commit_hooks-2.9.0.tar", last modified: Sun May 14 07:04:33 2023, max compression
```

## Comparing `language_formatters_pre_commit_hooks-2.8.0.tar` & `language_formatters_pre_commit_hooks-2.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:29:26.707004 language_formatters_pre_commit_hooks-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15484 2023-03-17 13:29:26.707004 language_formatters_pre_commit_hooks-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:29:26.707004 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/google_java_formatter.version
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/ktlint.version
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pre_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_golang.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_ini.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_java.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_kotlin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_rust.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:29:26.707004 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15484 2023-03-17 13:29:26.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-17 13:29:26.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 13:29:26.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-17 13:29:26.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-17 13:29:26.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-17 13:29:26.000000 language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-17 13:29:26.707004 language_formatters_pre_commit_hooks-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-17 13:29:24.000000 language_formatters_pre_commit_hooks-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:04:33.825240 language_formatters_pre_commit_hooks-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-05-14 07:04:33.825240 language_formatters_pre_commit_hooks-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:04:33.825240 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/google_java_formatter.version
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/ktlint.version
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pre_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_golang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_kotlin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_rust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:04:33.825240 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-05-14 07:04:33.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-14 07:04:33.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 07:04:33.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-14 07:04:33.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-14 07:04:33.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-14 07:04:33.000000 language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-14 07:04:33.825240 language_formatters_pre_commit_hooks-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-14 07:04:31.000000 language_formatters_pre_commit_hooks-2.9.0/setup.py
```

### Comparing `language_formatters_pre_commit_hooks-2.8.0/LICENSE` & `language_formatters_pre_commit_hooks-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `language_formatters_pre_commit_hooks-2.8.0/PKG-INFO` & `language_formatters_pre_commit_hooks-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: language_formatters_pre_commit_hooks
-Version: 2.8.0
+Version: 2.9.0
 Summary: List of pre-commit hooks meant to format your source code.
 Home-page: https://github.com/macisamuele/language-formatters-pre-commit-hooks
 Author: Samuele Maci
 Author-email: macisamuele@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
@@ -77,14 +77,24 @@
 2. Create your feature branch (`git checkout -b my-new-feature`)
 3. Add your modifications
 4. Push to the branch (`git push origin my-new-feature`)
 5. Create new Pull Request
 
 ## FAQ
 
+### How to deal with different Google Java Formatter versions?
+
+```yaml
+  - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
+    rev: ...
+    hooks:
+      - id: pretty-format-java
+        args: [--autofix, --aosp, --google-java-formatter-version=1.16.0]
+```
+
 ### How to deal with multiple Java versions?
 
 This might be relevant for `pretty-format-java` and `pretty-format-kotlin` hooks.
 The hooks depends on having `java` on version **11** or greater installed on your machine.
 
 As you're working with _compiled-to-JVM_ languages, we assume that you have `java` installed on your system. You might not have the minimum required version installed.
 
@@ -141,55 +151,67 @@
 ## License
 
 `language-formatters-pre-commit-hooks` is licensed with [`Apache License version 2.0`](http://www.apache.org/licenses/LICENSE-2.0.html).
 
 Changelog
 =========
 
+2.9.0 (2023-05-13)
+------------------
+
+- Update GoogleJavaFormatter to 1.17.0
+- Update KTLint to 0.49.1
+- Bug fix pretty-format-yaml
+  Sequecence item indentation should condider offset as part of the indentation, [#154 (comment)](https://github.com/macisamuele/language-formatters-pre-commit-hooks/issues/154#issuecomment-1546778156) has more details.
+  Thanks [@datalogics-kam](https://github.com/datalogics-kam) and [@fmigneault](https://github.com/fmigneault) for reporting the issue and helping me identify the underlying root cause.
+
 2.8.0 (2023-03-17)
 ------------------
-- Update GoogleJavaFormatter to 1.16.0
 
+- Update GoogleJavaFormatter to 1.16.0
 
 2.7.0 (2023-02-18)
 ------------------
+
 - Add support for customisable offset in `pretty-format-yaml` - [PR #143](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/143)
 - Update KTLint to 0.48.2
 
 2.6.0 (2023-01-20)
 ------------------
+
 - Fix `pertty-format-toml` to be compatible with latest `toml-sort` libraries - Thanks [@liblaf](https://github.com/liblaf) and [@stewartHutchins](https://github.com/stewartHutchins) for the support on having toml prettification working again
   The fix has been carried over multiple PRs ([PR #134](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/134), [PR #136](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/136) and [PR #137](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/137)).
 - Internal build fix (failures caused by `tox` major release) - [PR #141](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/141), inspired from [PR #135](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/135) - Thanks [@malmans2](https://github.com/malmans2) for the support
 - Update KTlint to 0.48.1 - [PR #140](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/140) - Thanks [@detouched](https://github.com/detouched) for the upgrade
 
-
 2.5.0 (2022-12-05)
 ------------------
+
 - Lift JDK 16+ restriction - [PR #123](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/123) - [@harti2006](https://github.com/harti2006) thanks for your contribution
 - Update KTlint to 0.47.1 - [PR #125](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/125)
 - pretty_format_rust does no longer use explicit rust versions - [PR #126](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/126)
 
 2.4.0 (2022-07-01)
 ------------------
+
 - Update GoogleJavaFormatter to 1.15.0
 - Update KTlint to 0.45.1
 - Ensure Python 3.10 support and drop Python3.6 guaranteed support - [PR #114](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/114) / [PR #115](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/115)
 - Updated prettifier library for INI files (from `configobj` to `config_formatter`) to provide more deterministic output and proper comments handling - [PR #113](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/113) - [@Delgan](https://github.com/Delgan) thanks for your contribution
 - `pretty-format-yaml` allows customization of max line length - [PR #104](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/104)
 - More explicit error messages in case of prettifier failires - [PR #116](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/116)
 - Use explicit encoding within INI prettifier - [PR #102](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/102) - [@hbre](https://github.com/hbre) thanks for your contribution
 
 2.3.0 (2022-02-17)
 ------------------
+
 - Update GoogleJavaFormatter to 1.14.0
 - Update KTlint to 0.44.0
 - Use explicit encoding within YAML prettifier - [PR #92](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/92) - [@passionsfrucht](https://github.com/passionsfrucht) thanks for your contribution
 
-
 2.2.0 (2021-08-08)
 ------------------
 
 - Make download of external artifacts resilient to systems with temporary directory on different disk partitions - [@psmit](https://github.com/psmit) and [@kbalston](https://github.com/kbalston) thanks for your contribution
 - Make usage of Google Java Formatter compatible with JDK16+ - [@ostrya](https://github.com/ostrya) thanks for your contribution
 - Update GoogleJavaFormatter to 1.11.0
 - Bump KTlint to 0.42.1
```

### Comparing `language_formatters_pre_commit_hooks-2.8.0/README.md` & `language_formatters_pre_commit_hooks-2.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,24 @@
 2. Create your feature branch (`git checkout -b my-new-feature`)
 3. Add your modifications
 4. Push to the branch (`git push origin my-new-feature`)
 5. Create new Pull Request
 
 ## FAQ
 
+### How to deal with different Google Java Formatter versions?
+
+```yaml
+  - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
+    rev: ...
+    hooks:
+      - id: pretty-format-java
+        args: [--autofix, --aosp, --google-java-formatter-version=1.16.0]
+```
+
 ### How to deal with multiple Java versions?
 
 This might be relevant for `pretty-format-java` and `pretty-format-kotlin` hooks.
 The hooks depends on having `java` on version **11** or greater installed on your machine.
 
 As you're working with _compiled-to-JVM_ languages, we assume that you have `java` installed on your system. You might not have the minimum required version installed.
```

### Comparing `language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/__init__.py` & `language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pre_conditions.py` & `language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pre_conditions.py`

 * *Files identical despite different names*

### Comparing `language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_golang.py` & `language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_golang.py`

 * *Files identical despite different names*

### Comparing `language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_ini.py` & `language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_ini.py`

 * *Files identical despite different names*

### Comparing `language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_java.py` & `language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_java.py`

 * *Files identical despite different names*

### Comparing `language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_kotlin.py` & `language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_kotlin.py`

 * *Files identical despite different names*

### Comparing `language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_rust.py` & `language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_rust.py`

 * *Files identical despite different names*

### Comparing `language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_toml.py` & `language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_toml.py`

 * *Files identical despite different names*

### Comparing `language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/pretty_format_yaml.py` & `language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/pretty_format_yaml.py`

 * *Files 14% similar despite different names*

```diff
@@ -69,24 +69,23 @@
     )
 
     parser.add_argument("filenames", nargs="*", help="Filenames to fix")
     args = parser.parse_args(argv)
 
     status = 0
 
-    if args.indent < args.offset + 2:
-        print(
-            "Indent should be at least 2 more than offset. \n"
-            "Invalid output could be resulting otherwise. \n"
-            "indent={}, offset={}".format(args.indent, args.offset)
-        )
-        return 1
+    if args.indent < 0:  # pragma: no cover
+        print("indent argument ({}) cannot be negative. Defaulting it to 2".format(args.indent), file=sys.stderr)
+        args.indent = 2
+    if args.offset < 0:  # pragma: no cover
+        print("offset argument ({}) cannot be negative. Defaulting it to 0".format(args.offset), file=sys.stderr)
+        args.offset = 0
 
     yaml = YAML()
-    yaml.indent(mapping=args.indent, sequence=args.indent, offset=args.offset)
+    yaml.indent(mapping=args.indent, sequence=args.indent + args.offset, offset=args.offset)
     yaml.preserve_quotes = args.preserve_quotes
     # Prevent ruamel.yaml to wrap yaml lines
     yaml.width = args.line_width  # type: ignore  # mypy recognise yaml.width as None
 
     separator = "---\n"
 
     for yaml_file in set(args.filenames):
```

### Comparing `language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks/utils.py` & `language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks/utils.py`

 * *Files identical despite different names*

### Comparing `language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks.egg-info/PKG-INFO` & `language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: language-formatters-pre-commit-hooks
-Version: 2.8.0
+Version: 2.9.0
 Summary: List of pre-commit hooks meant to format your source code.
 Home-page: https://github.com/macisamuele/language-formatters-pre-commit-hooks
 Author: Samuele Maci
 Author-email: macisamuele@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
@@ -77,14 +77,24 @@
 2. Create your feature branch (`git checkout -b my-new-feature`)
 3. Add your modifications
 4. Push to the branch (`git push origin my-new-feature`)
 5. Create new Pull Request
 
 ## FAQ
 
+### How to deal with different Google Java Formatter versions?
+
+```yaml
+  - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
+    rev: ...
+    hooks:
+      - id: pretty-format-java
+        args: [--autofix, --aosp, --google-java-formatter-version=1.16.0]
+```
+
 ### How to deal with multiple Java versions?
 
 This might be relevant for `pretty-format-java` and `pretty-format-kotlin` hooks.
 The hooks depends on having `java` on version **11** or greater installed on your machine.
 
 As you're working with _compiled-to-JVM_ languages, we assume that you have `java` installed on your system. You might not have the minimum required version installed.
 
@@ -141,55 +151,67 @@
 ## License
 
 `language-formatters-pre-commit-hooks` is licensed with [`Apache License version 2.0`](http://www.apache.org/licenses/LICENSE-2.0.html).
 
 Changelog
 =========
 
+2.9.0 (2023-05-13)
+------------------
+
+- Update GoogleJavaFormatter to 1.17.0
+- Update KTLint to 0.49.1
+- Bug fix pretty-format-yaml
+  Sequecence item indentation should condider offset as part of the indentation, [#154 (comment)](https://github.com/macisamuele/language-formatters-pre-commit-hooks/issues/154#issuecomment-1546778156) has more details.
+  Thanks [@datalogics-kam](https://github.com/datalogics-kam) and [@fmigneault](https://github.com/fmigneault) for reporting the issue and helping me identify the underlying root cause.
+
 2.8.0 (2023-03-17)
 ------------------
-- Update GoogleJavaFormatter to 1.16.0
 
+- Update GoogleJavaFormatter to 1.16.0
 
 2.7.0 (2023-02-18)
 ------------------
+
 - Add support for customisable offset in `pretty-format-yaml` - [PR #143](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/143)
 - Update KTLint to 0.48.2
 
 2.6.0 (2023-01-20)
 ------------------
+
 - Fix `pertty-format-toml` to be compatible with latest `toml-sort` libraries - Thanks [@liblaf](https://github.com/liblaf) and [@stewartHutchins](https://github.com/stewartHutchins) for the support on having toml prettification working again
   The fix has been carried over multiple PRs ([PR #134](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/134), [PR #136](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/136) and [PR #137](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/137)).
 - Internal build fix (failures caused by `tox` major release) - [PR #141](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/141), inspired from [PR #135](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/135) - Thanks [@malmans2](https://github.com/malmans2) for the support
 - Update KTlint to 0.48.1 - [PR #140](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/140) - Thanks [@detouched](https://github.com/detouched) for the upgrade
 
-
 2.5.0 (2022-12-05)
 ------------------
+
 - Lift JDK 16+ restriction - [PR #123](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/123) - [@harti2006](https://github.com/harti2006) thanks for your contribution
 - Update KTlint to 0.47.1 - [PR #125](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/125)
 - pretty_format_rust does no longer use explicit rust versions - [PR #126](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/126)
 
 2.4.0 (2022-07-01)
 ------------------
+
 - Update GoogleJavaFormatter to 1.15.0
 - Update KTlint to 0.45.1
 - Ensure Python 3.10 support and drop Python3.6 guaranteed support - [PR #114](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/114) / [PR #115](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/115)
 - Updated prettifier library for INI files (from `configobj` to `config_formatter`) to provide more deterministic output and proper comments handling - [PR #113](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/113) - [@Delgan](https://github.com/Delgan) thanks for your contribution
 - `pretty-format-yaml` allows customization of max line length - [PR #104](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/104)
 - More explicit error messages in case of prettifier failires - [PR #116](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/116)
 - Use explicit encoding within INI prettifier - [PR #102](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/102) - [@hbre](https://github.com/hbre) thanks for your contribution
 
 2.3.0 (2022-02-17)
 ------------------
+
 - Update GoogleJavaFormatter to 1.14.0
 - Update KTlint to 0.44.0
 - Use explicit encoding within YAML prettifier - [PR #92](https://github.com/macisamuele/language-formatters-pre-commit-hooks/pull/92) - [@passionsfrucht](https://github.com/passionsfrucht) thanks for your contribution
 
-
 2.2.0 (2021-08-08)
 ------------------
 
 - Make download of external artifacts resilient to systems with temporary directory on different disk partitions - [@psmit](https://github.com/psmit) and [@kbalston](https://github.com/kbalston) thanks for your contribution
 - Make usage of Google Java Formatter compatible with JDK16+ - [@ostrya](https://github.com/ostrya) thanks for your contribution
 - Update GoogleJavaFormatter to 1.11.0
 - Bump KTlint to 0.42.1
```

### Comparing `language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks.egg-info/SOURCES.txt` & `language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `language_formatters_pre_commit_hooks-2.8.0/language_formatters_pre_commit_hooks.egg-info/entry_points.txt` & `language_formatters_pre_commit_hooks-2.9.0/language_formatters_pre_commit_hooks.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `language_formatters_pre_commit_hooks-2.8.0/setup.cfg` & `language_formatters_pre_commit_hooks-2.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 description = List of pre-commit hooks meant to format your source code.
 name = language_formatters_pre_commit_hooks
 license = Apache License 2.0
 license_file = LICENSE
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 url = https://github.com/macisamuele/language-formatters-pre-commit-hooks
-version = 2.8.0
+version = 2.9.0
 
 [options]
 install_requires = 
 	config_formatter
 	packaging
 	requests
 	ruamel.yaml
```

### Comparing `language_formatters_pre_commit_hooks-2.8.0/setup.py` & `language_formatters_pre_commit_hooks-2.9.0/setup.py`

 * *Files identical despite different names*

