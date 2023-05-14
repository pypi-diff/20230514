# Comparing `tmp/shellinspector-0.8.0.tar.gz` & `tmp/shellinspector-0.9.0.tar.gz`

## Comparing `shellinspector-0.8.0.tar` & `shellinspector-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 shellinspector-0.8.0/.copier-answers.pre-commit.yaml
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 shellinspector-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 shellinspector-0.8.0/docker-compose.yml
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 shellinspector-0.8.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 shellinspector-0.8.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 shellinspector-0.8.0/docs/dev.md
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 shellinspector-0.8.0/docs/syntax.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 shellinspector-0.8.0/docs/examples/fail.inspect
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 shellinspector-0.8.0/docs/examples/local.inspect
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 shellinspector-0.8.0/docs/examples/local_sessions.inspect
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 shellinspector-0.8.0/docs/examples/remote.inspect
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shellinspector-0.8.0/docs/examples/syntax_error.inspect
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 shellinspector-0.8.0/docs/examples/whoami.inspect
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shellinspector-0.8.0/src/shellinspector/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shellinspector-0.8.0/src/shellinspector/__init__.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 shellinspector-0.8.0/src/shellinspector/__main__.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 shellinspector-0.8.0/src/shellinspector/parser.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 shellinspector-0.8.0/src/shellinspector/reporter.py
--rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 shellinspector-0.8.0/src/shellinspector/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shellinspector-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 shellinspector-0.8.0/tests/test_parser.py
--rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 shellinspector-0.8.0/tests/test_runner.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 shellinspector-0.8.0/tests/e2e/000_root.inspect
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 shellinspector-0.8.0/tests/e2e/010_create_user.inspect
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 shellinspector-0.8.0/tests/e2e/020_user.inspect
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 shellinspector-0.8.0/tests/e2e/100_local.inspect
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 shellinspector-0.8.0/tests/e2e/200_state.inspect
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 shellinspector-0.8.0/tests/e2e/210_state_gone.inspect
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 shellinspector-0.8.0/tests/e2e/300_env.inspect
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 shellinspector-0.8.0/tests/keys/README.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 shellinspector-0.8.0/tests/keys/id_ed25519
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 shellinspector-0.8.0/tests/keys/id_ed25519.pub
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 shellinspector-0.8.0/.gitignore
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 shellinspector-0.8.0/README.md
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 shellinspector-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 shellinspector-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 shellinspector-0.9.0/.copier-answers.pre-commit.yaml
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 shellinspector-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 shellinspector-0.9.0/docker-compose.yml
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 shellinspector-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 shellinspector-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 shellinspector-0.9.0/docs/dev.md
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 shellinspector-0.9.0/docs/env.md
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 shellinspector-0.9.0/docs/syntax.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 shellinspector-0.9.0/docs/examples/fail.inspect
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 shellinspector-0.9.0/docs/examples/local.inspect
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 shellinspector-0.9.0/docs/examples/local_sessions.inspect
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 shellinspector-0.9.0/docs/examples/remote.inspect
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shellinspector-0.9.0/docs/examples/syntax_error.inspect
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 shellinspector-0.9.0/docs/examples/whoami.inspect
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shellinspector-0.9.0/src/shellinspector/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shellinspector-0.9.0/src/shellinspector/__init__.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 shellinspector-0.9.0/src/shellinspector/__main__.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 shellinspector-0.9.0/src/shellinspector/parser.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 shellinspector-0.9.0/src/shellinspector/reporter.py
+-rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 shellinspector-0.9.0/src/shellinspector/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shellinspector-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     9247 2020-02-02 00:00:00.000000 shellinspector-0.9.0/tests/test_parser.py
+-rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 shellinspector-0.9.0/tests/test_runner.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 shellinspector-0.9.0/tests/e2e/000_root.inspect
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 shellinspector-0.9.0/tests/e2e/010_create_user.inspect
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 shellinspector-0.9.0/tests/e2e/020_user.inspect
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 shellinspector-0.9.0/tests/e2e/100_local.inspect
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 shellinspector-0.9.0/tests/e2e/200_state.inspect
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 shellinspector-0.9.0/tests/e2e/210_state_gone.inspect
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 shellinspector-0.9.0/tests/e2e/300_env.inspect
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 shellinspector-0.9.0/tests/keys/README.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 shellinspector-0.9.0/tests/keys/id_ed25519
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 shellinspector-0.9.0/tests/keys/id_ed25519.pub
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 shellinspector-0.9.0/.gitignore
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 shellinspector-0.9.0/README.md
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 shellinspector-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 shellinspector-0.9.0/PKG-INFO
```

### Comparing `shellinspector-0.8.0/.pre-commit-config.yaml` & `shellinspector-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `shellinspector-0.8.0/docker-compose.yml` & `shellinspector-0.9.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `shellinspector-0.8.0/.github/workflows/release.yml` & `shellinspector-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `shellinspector-0.8.0/.github/workflows/test.yml` & `shellinspector-0.9.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `shellinspector-0.8.0/docs/dev.md` & `shellinspector-0.9.0/docs/dev.md`

 * *Files identical despite different names*

### Comparing `shellinspector-0.8.0/docs/syntax.md` & `shellinspector-0.9.0/docs/syntax.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,22 @@
 
 ```
 % head -n2 /etc/passwd
 root:x:0:0:root:/root:/bin/bash
 bin:x:1:1:bin:/bin:/usr/bin/nologin
 ```
 
+Note that there is always a final new line after the expected output, so this
+will currently always fail:
+
+```
+$ echo -n a
+a
+```
+
 ##### Regex Match
 
 Interpret the specified output as a regex with `re.MULTILINE` and try to match
 it:
 
 ```
 %~ ls /home
@@ -70,14 +78,22 @@
 $~ whoami
 \Atestuser\Z
 ```
 
 Keep in mind that `\A` and `\Z` (not `^` and `$`) are needed to match start and
 end of the regex.
 
+New lines are only preserved between lines, but not after the final one.
+Otherwise this would never match, since `r"aaaa\n"` can't match `aaaa`.
+
+```
+$~ echo aaaab
+aaaa
+```
+
 ##### Ignore
 
 To just discard and ignore the output, use `_`:
 
 ```
 %_ ls /home
 %
```

### Comparing `shellinspector-0.8.0/src/shellinspector/__main__.py` & `shellinspector-0.9.0/src/shellinspector/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 error.source_line,
                 error.message,
             )
 
         return False
 
     for i, command in enumerate(commands):
-        LOGGER.debug("command[%s]: %s", i, command.short())
+        LOGGER.debug("command[%s]: %s", i, command.short)
 
     return runner.run(commands)
 
 
 def run(target_host, spec_files, identity, verbose):
     ssh_config = get_ssh_config(target_host)
     ssh_config["ssh_key"] = identity
```

### Comparing `shellinspector-0.8.0/src/shellinspector/parser.py` & `shellinspector-0.9.0/src/shellinspector/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,25 @@
     host: str
     assert_mode: AssertMode
     expected: str
     source_file: Path
     source_line_no: int
     line: str
 
+    @property
+    def line_count(self):
+        # TODO: replace this with .removesuffix("\n").count("\n")+1 once we drop py3.7
+        count = self.expected.count("\n")
+        if self.expected and self.expected[-1] != "\n":
+            count += 1
+        return count
+
+    @property
     def short(self):
-        return f"{self.execution_mode.name}({self.user}@{self.host}) `{self.command}` (expect {len(self.expected)} lines, {self.assert_mode.name})"
+        return f"{self.execution_mode.name}({self.user}@{self.host}) `{self.command}` (expect {self.line_count} lines, {self.assert_mode.name})"
 
 
 @dataclass
 class Error:
     source_file: Path
     source_line_no: int
     source_line: str
@@ -147,8 +156,13 @@
                     line,
                 )
             )
         else:
             # add output line to last command
             commands[-1].expected += line + "\n"
 
+    for cmd in commands:
+        if cmd.assert_mode == AssertMode.REGEX:
+            # remove trailing new lines for regexes, see syntax.md
+            cmd.expected = cmd.expected.rstrip("\n")
+
     return (errors, commands)
```

### Comparing `shellinspector-0.8.0/src/shellinspector/reporter.py` & `shellinspector-0.9.0/src/shellinspector/reporter.py`

 * *Files identical despite different names*

### Comparing `shellinspector-0.8.0/src/shellinspector/runner.py` & `shellinspector-0.9.0/src/shellinspector/runner.py`

 * *Files identical despite different names*

### Comparing `shellinspector-0.8.0/tests/test_parser.py` & `shellinspector-0.9.0/tests/test_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,14 +42,50 @@
     assert commands[2].execution_mode == ExecutionMode.ROOT
     assert commands[2].command == "ls dir"
     assert commands[2].assert_mode == AssertMode.REGEX
     assert commands[2].source_file == Path("/dev/null")
     assert commands[2].source_line_no == 8
 
 
+def test_parse_whitespace_literal():
+    errors, commands = parse(
+        "/dev/null",
+        [
+            "$ echo ab",
+            "a",
+            "b",
+        ],
+    )
+
+    assert len(errors) == 0
+    assert len(commands) == 1
+
+    assert commands[0].expected == "a\nb\n"
+
+
+def test_parse_whitespace_regex():
+    errors, commands = parse(
+        "/dev/null",
+        [
+            "%~ /usr/bin/which --help",
+            "Usage: /usr/bin/which [options] [--] COMMAND [...]",
+            "Write the full path of COMMAND",
+        ],
+    )
+
+    assert len(errors) == 0
+    assert len(commands) == 1
+
+    # no trailing newline at the end because this confuses the regex
+    assert (
+        commands[0].expected
+        == "Usage: /usr/bin/which [options] [--] COMMAND [...]\nWrite the full path of COMMAND"
+    )
+
+
 def test_parse_error():
     path = Path(__file__).parent / "virtual.spec"
     errors, commands = parse(
         path,
         [
             "random text1",
             "random text2",
@@ -268,21 +304,37 @@
         ],
     )
 
     assert len(errors) == 1
     assert "test_not_existent.spec does not exist" in errors[0].message
 
 
-def test_command_short():
+def test_command_short_literal():
     cmd = Command(
         ExecutionMode.USER,
         "echo a",
         None,
         None,
         "local",
         AssertMode.LITERAL,
-        "a",
+        "a\nb\n",
+        "/some.spec",
+        1,
+        "$ echo a\nb",
+    )
+    assert cmd.short == "USER(None@local) `echo a` (expect 2 lines, LITERAL)"
+
+
+def test_command_short_regex():
+    cmd = Command(
+        ExecutionMode.USER,
+        "echo a",
+        None,
+        None,
+        "local",
+        AssertMode.REGEX,
+        "a\nb",
         "/some.spec",
         1,
-        "$ echo a",
+        "$ echo a\nb",
     )
-    assert cmd.short() == "USER(None@local) `echo a` (expect 1 lines, LITERAL)"
+    assert cmd.short == "USER(None@local) `echo a` (expect 2 lines, REGEX)"
```

### Comparing `shellinspector-0.8.0/tests/test_runner.py` & `shellinspector-0.9.0/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `shellinspector-0.8.0/.gitignore` & `shellinspector-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `shellinspector-0.8.0/README.md` & `shellinspector-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `shellinspector-0.8.0/pyproject.toml` & `shellinspector-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ]
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=shellinspector --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 build-exe = "pyinstaller --onefile --noconfirm --name shellinspector.amd64 src/shellinspector/__main__.py"
 
 [[tool.hatch.envs.test.matrix]]
-python = ["37", "38", "39", "310", "311"]
+python = ["38", "39", "310", "311"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "src/shellinspector/__about__.py",
 ]
```

### Comparing `shellinspector-0.8.0/PKG-INFO` & `shellinspector-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellinspector
-Version: 0.8.0
+Version: 0.9.0
 Project-URL: Documentation, https://github.com/uberspace/shellinspector#readme
 Project-URL: Issues, https://github.com/uberspace/shellinspector/issues
 Project-URL: Source, https://github.com/uberspace/shellinspector
 Author-email: "uberspace.de" <hallo@uberspace.de>
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

