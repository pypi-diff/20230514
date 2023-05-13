# Comparing `tmp/representty-0.1.3.tar.gz` & `tmp/representty-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "representty-0.1.3.tar", max compression
+gzip compressed data, was "representty-0.1.4.tar", max compression
```

## Comparing `representty-0.1.3.tar` & `representty-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1657 2023-05-12 07:49:03.414011 representty-0.1.3/README.md
--rw-r--r--   0        0        0      935 2023-05-12 07:49:12.077566 representty-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4082 2023-05-10 21:15:40.076464 representty-0.1.3/representty.py
--rw-r--r--   0        0        0     2431 2023-05-12 07:49:27.538511 representty-0.1.3/setup.py
--rw-r--r--   0        0        0     2554 2023-05-12 07:49:27.538671 representty-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2109 2023-05-13 22:03:52.113201 representty-0.1.4/README.md
+-rw-r--r--   0        0        0      935 2023-05-13 22:04:13.362330 representty-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4607 2023-05-13 22:03:52.113684 representty-0.1.4/representty.py
+-rw-r--r--   0        0        0     2892 2023-05-13 22:04:25.238652 representty-0.1.4/setup.py
+-rw-r--r--   0        0        0     3006 2023-05-13 22:04:25.238817 representty-0.1.4/PKG-INFO
```

### Comparing `representty-0.1.3/README.md` & `representty-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # representty
 
 `representty` is a tiny presentation framework. TL;DR: You write your slides in
 Markdown, `rich` renders individual slides, and the whole thing happens in an
 IPython shell.
 
+[![asciicast](https://asciinema.org/a/584388.svg)](https://asciinema.org/a/584388)
+
 ## File Format
 
 A slide deck is mostly a Markdown file. Individual slides are seperated by a
 bunch of equals signs.
 
 Additionally, you can start a line with:
 
@@ -18,14 +20,21 @@
     - `!!some command`: execute the command with `os.system()` the first time
       this slide is visited.
     - `!import somemodule`: silently import the given module.
     - `!set flag`/`!unset flag`: set/unset a named flag. These can influence
       `representty` behaviour. See [flags](#flags).
     - `!setlocal flag`/`!unsetlocal flag`: (un)set a flag, but reset to
       original value at the end of the slide.
+    - `!image someimage`: Display an image. This only works if you have
+      `viu` installed.
+    - `!up some_int`: Move the cursor up by some amount. Useful for drawing
+      over images.
+    - `!printf something`: Call `printf` with the given args. Better than
+      plain `!!printf`, because it will be executed every time the slide is
+      displayed by default.
 
 Python code blocks (language starts with `py`) are not just rendered, but also
 executed.
 
 ## Commands
 
 The presenter is dropped into a more-or-less normal IPython shell. A few
```

### Comparing `representty-0.1.3/pyproject.toml` & `representty-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "representty"
-version = "0.1.3"
+version = "0.1.4"
 description = "Tiny presentation tool based on rich and markdown"
 authors = ["L3viathan <git@l3vi.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/L3viathan/representty"
 keywords = ["presentation"]
 classifiers = [
```

### Comparing `representty-0.1.3/representty.py` & `representty-0.1.4/representty.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,25 @@
                 if "PRACTICE" in os.environ:
                     line = f"\x1b[1;31m\x1b[3m{line}\x1b[0m"
                 else:
                     continue
             elif line.strip().startswith("!import "):
                 exec(line.strip("! \n"), globals())
                 continue
+            elif line.strip().startswith("!image "):
+                os.system(f"viu -t {line.removeprefix('!image ').strip()}")
+                continue
+            elif line.strip().startswith("!printf "):
+                # to work without needing alwaysexec
+                os.system(line.strip().lstrip("!"))
+                continue
+            elif line.strip().startswith("!up "):
+                how_much = int(line.removeprefix("!up "))
+                os.system(f"printf '\e[{how_much}A'")
+                continue
             elif line.strip().startswith("!unset"):
                 flag = line.strip().split()[1]
                 self.flags -= {flag}
                 if line.strip().startswith("!unsetlocal"):
                     unset_local.add(flag)
                 continue
             elif line.strip().startswith("!set"):
```

### Comparing `representty-0.1.3/setup.py` & `representty-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 ['ipython', 'rich>=13.3.1,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['rtty = representty:just_call_the_script']}
 
 setup_kwargs = {
     'name': 'representty',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Tiny presentation tool based on rich and markdown',
-    'long_description': '# representty\n\n`representty` is a tiny presentation framework. TL;DR: You write your slides in\nMarkdown, `rich` renders individual slides, and the whole thing happens in an\nIPython shell.\n\n## File Format\n\nA slide deck is mostly a Markdown file. Individual slides are seperated by a\nbunch of equals signs.\n\nAdditionally, you can start a line with:\n\n- `//`: comment; the line is ignored (unless the environment variable\n  `PRACTICE` is set).\n- `!`: special instruction. The line is not included in the output, but can do\n  a variety of things:\n    - `!!some command`: execute the command with `os.system()` the first time\n      this slide is visited.\n    - `!import somemodule`: silently import the given module.\n    - `!set flag`/`!unset flag`: set/unset a named flag. These can influence\n      `representty` behaviour. See [flags](#flags).\n    - `!setlocal flag`/`!unsetlocal flag`: (un)set a flag, but reset to\n      original value at the end of the slide.\n\nPython code blocks (language starts with `py`) are not just rendered, but also\nexecuted.\n\n## Commands\n\nThe presenter is dropped into a more-or-less normal IPython shell. A few\nsingle-letter commands exist which control the slide show:\n\n- `d`: (Re)draw the current slide.\n- `n`: Go to the next slide.\n- `p`: Go to the previous slide.\n- `q`: Quit.\n- `g`: Go to a numbered slide (you will be prompted for a slide number).\n- `s`: Go to a slide by searching for a keyword (you will be prompted).\n\n## Flags\n\n- `exec`: whether to execute Python code in code blocks. Default: set.\n- `alwaysexec`: Always execute shell commands (`!!`), rather than just at the\n  first printing of the slide. Default: unset.\n',
+    'long_description': '# representty\n\n`representty` is a tiny presentation framework. TL;DR: You write your slides in\nMarkdown, `rich` renders individual slides, and the whole thing happens in an\nIPython shell.\n\n[![asciicast](https://asciinema.org/a/584388.svg)](https://asciinema.org/a/584388)\n\n## File Format\n\nA slide deck is mostly a Markdown file. Individual slides are seperated by a\nbunch of equals signs.\n\nAdditionally, you can start a line with:\n\n- `//`: comment; the line is ignored (unless the environment variable\n  `PRACTICE` is set).\n- `!`: special instruction. The line is not included in the output, but can do\n  a variety of things:\n    - `!!some command`: execute the command with `os.system()` the first time\n      this slide is visited.\n    - `!import somemodule`: silently import the given module.\n    - `!set flag`/`!unset flag`: set/unset a named flag. These can influence\n      `representty` behaviour. See [flags](#flags).\n    - `!setlocal flag`/`!unsetlocal flag`: (un)set a flag, but reset to\n      original value at the end of the slide.\n    - `!image someimage`: Display an image. This only works if you have\n      `viu` installed.\n    - `!up some_int`: Move the cursor up by some amount. Useful for drawing\n      over images.\n    - `!printf something`: Call `printf` with the given args. Better than\n      plain `!!printf`, because it will be executed every time the slide is\n      displayed by default.\n\nPython code blocks (language starts with `py`) are not just rendered, but also\nexecuted.\n\n## Commands\n\nThe presenter is dropped into a more-or-less normal IPython shell. A few\nsingle-letter commands exist which control the slide show:\n\n- `d`: (Re)draw the current slide.\n- `n`: Go to the next slide.\n- `p`: Go to the previous slide.\n- `q`: Quit.\n- `g`: Go to a numbered slide (you will be prompted for a slide number).\n- `s`: Go to a slide by searching for a keyword (you will be prompted).\n\n## Flags\n\n- `exec`: whether to execute Python code in code blocks. Default: set.\n- `alwaysexec`: Always execute shell commands (`!!`), rather than just at the\n  first printing of the slide. Default: unset.\n',
     'author': 'L3viathan',
     'author_email': 'git@l3vi.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/L3viathan/representty',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `representty-0.1.3/PKG-INFO` & `representty-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: representty
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tiny presentation tool based on rich and markdown
 Home-page: https://github.com/L3viathan/representty
 License: MIT
 Keywords: presentation
 Author: L3viathan
 Author-email: git@l3vi.de
 Requires-Python: >=3.10,<4.0
@@ -25,14 +25,16 @@
 
 # representty
 
 `representty` is a tiny presentation framework. TL;DR: You write your slides in
 Markdown, `rich` renders individual slides, and the whole thing happens in an
 IPython shell.
 
+[![asciicast](https://asciinema.org/a/584388.svg)](https://asciinema.org/a/584388)
+
 ## File Format
 
 A slide deck is mostly a Markdown file. Individual slides are seperated by a
 bunch of equals signs.
 
 Additionally, you can start a line with:
 
@@ -43,14 +45,21 @@
     - `!!some command`: execute the command with `os.system()` the first time
       this slide is visited.
     - `!import somemodule`: silently import the given module.
     - `!set flag`/`!unset flag`: set/unset a named flag. These can influence
       `representty` behaviour. See [flags](#flags).
     - `!setlocal flag`/`!unsetlocal flag`: (un)set a flag, but reset to
       original value at the end of the slide.
+    - `!image someimage`: Display an image. This only works if you have
+      `viu` installed.
+    - `!up some_int`: Move the cursor up by some amount. Useful for drawing
+      over images.
+    - `!printf something`: Call `printf` with the given args. Better than
+      plain `!!printf`, because it will be executed every time the slide is
+      displayed by default.
 
 Python code blocks (language starts with `py`) are not just rendered, but also
 executed.
 
 ## Commands
 
 The presenter is dropped into a more-or-less normal IPython shell. A few
```

