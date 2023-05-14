# Comparing `tmp/tmux_conf-0.15.8.tar.gz` & `tmp/tmux_conf-0.15.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmux_conf-0.15.8.tar", last modified: Mon Dec 12 03:19:02 2022, max compression
+gzip compressed data, was "tmux_conf-0.15.9.tar", last modified: Thu Dec 15 19:08:26 2022, max compression
```

## Comparing `tmux_conf-0.15.8.tar` & `tmux_conf-0.15.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2022-12-12 03:19:02.389494 tmux_conf-0.15.8/
--rw-r--r--   0 jaclu      (501) staff       (20)     1072 2022-10-11 13:49:33.000000 tmux_conf-0.15.8/LICENSE
--rw-r--r--   0 jaclu      (501) staff       (20)     7996 2022-12-12 03:19:02.389038 tmux_conf-0.15.8/PKG-INFO
--rw-r--r--   0 jaclu      (501) staff       (20)     7332 2022-12-12 01:58:36.000000 tmux_conf-0.15.8/README.md
--rw-r--r--   0 jaclu      (501) staff       (20)     1593 2022-12-12 03:11:51.000000 tmux_conf-0.15.8/pyproject.toml
--rw-r--r--   0 jaclu      (501) staff       (20)       38 2022-12-12 03:19:02.389593 tmux_conf-0.15.8/setup.cfg
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2022-12-12 03:19:02.381440 tmux_conf-0.15.8/src/
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2022-12-12 03:19:02.386546 tmux_conf-0.15.8/src/tmux_conf/
--rw-r--r--   0 jaclu      (501) staff       (20)      202 2022-11-09 10:03:24.000000 tmux_conf-0.15.8/src/tmux_conf/__init__.py
--rw-r--r--   0 jaclu      (501) staff       (20)      269 2022-12-12 03:12:01.000000 tmux_conf-0.15.8/src/tmux_conf/constants.py
--rw-r--r--   0 jaclu      (501) staff       (20)     5618 2022-11-14 13:36:13.000000 tmux_conf-0.15.8/src/tmux_conf/embedded_scripts.py
--rw-r--r--   0 jaclu      (501) staff       (20)    17132 2022-12-12 03:06:26.000000 tmux_conf-0.15.8/src/tmux_conf/plugins.py
--rw-r--r--   0 jaclu      (501) staff       (20)    23372 2022-11-14 13:54:01.000000 tmux_conf-0.15.8/src/tmux_conf/tmux_conf.py
--rw-r--r--   0 jaclu      (501) staff       (20)     4780 2022-11-09 10:03:03.000000 tmux_conf-0.15.8/src/tmux_conf/utils.py
--rw-r--r--   0 jaclu      (501) staff       (20)     3398 2022-11-14 13:32:13.000000 tmux_conf-0.15.8/src/tmux_conf/vers_check.py
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2022-12-12 03:19:02.388457 tmux_conf-0.15.8/src/tmux_conf.egg-info/
--rw-r--r--   0 jaclu      (501) staff       (20)     7996 2022-12-12 03:19:02.000000 tmux_conf-0.15.8/src/tmux_conf.egg-info/PKG-INFO
--rw-r--r--   0 jaclu      (501) staff       (20)      370 2022-12-12 03:19:02.000000 tmux_conf-0.15.8/src/tmux_conf.egg-info/SOURCES.txt
--rw-r--r--   0 jaclu      (501) staff       (20)        1 2022-12-12 03:19:02.000000 tmux_conf-0.15.8/src/tmux_conf.egg-info/dependency_links.txt
--rw-r--r--   0 jaclu      (501) staff       (20)       10 2022-12-12 03:19:02.000000 tmux_conf-0.15.8/src/tmux_conf.egg-info/top_level.txt
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2022-12-15 19:08:26.644983 tmux_conf-0.15.9/
+-rw-r--r--   0 jaclu      (501) staff       (20)     1072 2022-12-12 14:51:08.000000 tmux_conf-0.15.9/LICENSE
+-rw-r--r--   0 jaclu      (501) staff       (20)     7996 2022-12-15 19:08:26.644538 tmux_conf-0.15.9/PKG-INFO
+-rw-r--r--   0 jaclu      (501) staff       (20)     7332 2022-12-12 14:51:08.000000 tmux_conf-0.15.9/README.md
+-rw-r--r--   0 jaclu      (501) staff       (20)     1593 2022-12-15 19:07:27.000000 tmux_conf-0.15.9/pyproject.toml
+-rw-r--r--   0 jaclu      (501) staff       (20)       38 2022-12-15 19:08:26.645091 tmux_conf-0.15.9/setup.cfg
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2022-12-15 19:08:26.637104 tmux_conf-0.15.9/src/
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2022-12-15 19:08:26.642180 tmux_conf-0.15.9/src/tmux_conf/
+-rw-r--r--   0 jaclu      (501) staff       (20)      202 2022-12-12 14:51:08.000000 tmux_conf-0.15.9/src/tmux_conf/__init__.py
+-rw-r--r--   0 jaclu      (501) staff       (20)      269 2022-12-15 19:07:12.000000 tmux_conf-0.15.9/src/tmux_conf/constants.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     5698 2022-12-14 17:36:04.000000 tmux_conf-0.15.9/src/tmux_conf/embedded_scripts.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    16555 2022-12-15 18:53:00.000000 tmux_conf-0.15.9/src/tmux_conf/plugins.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    23447 2022-12-15 18:49:51.000000 tmux_conf-0.15.9/src/tmux_conf/tmux_conf.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     4780 2022-12-12 17:30:59.000000 tmux_conf-0.15.9/src/tmux_conf/utils.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     3364 2022-12-15 18:41:09.000000 tmux_conf-0.15.9/src/tmux_conf/vers_check.py
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2022-12-15 19:08:26.644045 tmux_conf-0.15.9/src/tmux_conf.egg-info/
+-rw-r--r--   0 jaclu      (501) staff       (20)     7996 2022-12-15 19:08:26.000000 tmux_conf-0.15.9/src/tmux_conf.egg-info/PKG-INFO
+-rw-r--r--   0 jaclu      (501) staff       (20)      370 2022-12-15 19:08:26.000000 tmux_conf-0.15.9/src/tmux_conf.egg-info/SOURCES.txt
+-rw-r--r--   0 jaclu      (501) staff       (20)        1 2022-12-15 19:08:26.000000 tmux_conf-0.15.9/src/tmux_conf.egg-info/dependency_links.txt
+-rw-r--r--   0 jaclu      (501) staff       (20)       10 2022-12-15 19:08:26.000000 tmux_conf-0.15.9/src/tmux_conf.egg-info/top_level.txt
```

### Comparing `tmux_conf-0.15.8/LICENSE` & `tmux_conf-0.15.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.15.8/PKG-INFO` & `tmux_conf-0.15.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmux_conf
-Version: 0.15.8
+Version: 0.15.9
 Summary: Generates version checked tmux conf
 Author-email: Jacob Lundqvist <Jacob.Lundqvist@gmail.com>
 Project-URL: Homepage, https://github.com/jaclu/tmux-conf
 Project-URL: documentation, https://github.com/jaclu/tmux-conf
 Project-URL: repository, https://github.com/jaclu/tmux-conf
 Project-URL: Bug Tracker, https://github.com/jaclu/tmux-conf/issues
 Keywords: tmux,automation
```

### Comparing `tmux_conf-0.15.8/README.md` & `tmux_conf-0.15.9/README.md`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.15.8/pyproject.toml` & `tmux_conf-0.15.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tmux_conf"
-version = "0.15.8"
+version = "0.15.9"
 authors = [
   { name="Jacob Lundqvist", email="Jacob.Lundqvist@gmail.com" },
 ]
 description = "Generates version checked tmux conf"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["tmux", "automation"]
```

### Comparing `tmux_conf-0.15.8/src/tmux_conf/embedded_scripts.py` & `tmux_conf-0.15.9/src/tmux_conf/embedded_scripts.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,19 @@
     def create(self, scr_name: str, script, use_bash=False):
         """Creates a script, supplied as a list of lines
         script lines can be regular lines as string, or multi-line strings
 
         Where the script should be run, just call run_it() with
         the script name, and code will be generated to call it the right way.
 
-        calling self.run_it('activate_tpm')  will insert code like:
-          run "cut -c3- /home/jaclu/t2/tmux/tmux.conf | sh -s activate_tpm"
+        calling self.run_it('activate_tpm')  will (depending on config file)
+        insert code like:
+          run "cut -c3- /home/jaclu/.tmux.conf | sh -s activate_tpm"
         or:
-          run "/home/jaclu/t2/tmux/scripts/activate_tpm.sh"
+          run "/home/jaclu/.tmux/scripts/activate_tpm.sh"
 
         depending on self._use_embedded_scripts
         """
         if self._use_embedded_scripts:
             if use_bash:
                 self._bash_scripts.append(scr_name)
             self._scripts += script
@@ -71,15 +72,16 @@
             fname = f"{script_dir}/{scr_name}.sh"
             with open(fname, "w", encoding="utf-8") as f:
                 for line in script:
                     f.write(f"{line}\n")
 
             #  Make it run able
             f = pathlib.Path(fname)
-            f.chmod(f.stat().st_mode | stat.S_IEXEC | stat.S_IXGRP | stat.S_IXOTH)
+            f.chmod(f.stat().st_mode | stat.S_IEXEC |
+                    stat.S_IXGRP | stat.S_IXOTH)
 
     def run_it(self, scr_name: str, in_bg: bool = False) -> str:
         """Generate the code to run an embedded/external script"""
         cmd = "run "
         if in_bg:
             cmd += "-b "
         cmd += '"'
@@ -142,23 +144,25 @@
                 output.append(f"# {script_line}")
         output.append('# "$@" #  This triggers the embedded script')
         return output
 
     def get_dir(self):
         """Retrieves the location where scripts should be saved"""
         if self._use_embedded_scripts:
-            raise SyntaxError("get_dir() called when use_embedded_scripts is True")
+            raise SyntaxError(
+                "get_dir() called when use_embedded_scripts is True")
 
         if tilde_home_dir(self._conf_file) == "~/.tmux.conf":
             scripts_dir = os.path.expanduser("~/.tmux/scripts")
         else:
             conf_file = os.path.expanduser(self._conf_file)
 
             xdg_home = os.environ.get(XDG_CONFIG_HOME)
             # pylint: disable=consider-using-assignment-expr
             if xdg_home:
                 conf_base = xdg_home
             else:
                 conf_base = os.path.dirname(os.path.dirname(conf_file))
 
-            scripts_dir = os.path.expanduser(os.path.join(conf_base, "tmux", "scripts"))
+            scripts_dir = os.path.expanduser(
+                os.path.join(conf_base, "tmux", "scripts"))
         return scripts_dir
```

### Comparing `tmux_conf-0.15.8/src/tmux_conf/plugins.py` & `tmux_conf-0.15.9/src/tmux_conf/plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             if short_name:
                 # Try to return only actual plugin name, without provider
                 if full_name.find("/") > -1:
                     name = full_name.split("/")[1]
             result.append(name)
         return result
 
-    def get_deploy_dir(self) -> str:
+    def get_plugin_dir(self) -> str:
         """Returns dir where plugins will be installed."""
         plugins_dir, _ = self.get_env()
         return plugins_dir
 
     # ================================================================
     #
     #        Rest is mostly for internal usage
@@ -142,83 +142,77 @@
         #
         max_l_name = 0
         for name in self._used_plugins:
             max_l_name = max(max_l_name, len(name) + 2)
 
         if self._used_plugins:
             print("\n\t-----   Plugins used   -----")
-            print(f'{"Plugin":<{max_l_name}}|  Min version\n')
+            print(f'{"Plugin":<{max_l_name}}|  Min version')
 
         #
         #  Create list of items in plugins dir
         #
-        # plugin_items = next(os.walk(self.get_deploy_dir()))[1]
+        # plugin_items = next(os.walk(self.get_plugin_dir()))[1]
         plugin_items = []
-        plugin_dir = self.get_deploy_dir()
+        plugin_dir = self.get_plugin_dir()
         if os.path.exists(plugin_dir):
             for f in os.scandir(plugin_dir):
                 if f.is_dir():
                     plugin_items.append((f.path.split("/")[-1]))
+        _ = self._remove_if_found(plugin_items, "tpm")
 
-        if "tpm" in plugin_items:
-            plugin_items.remove("tpm")
         #
         #  When exec'ing the plugin code below, write output to stdout,
         #  not to config file. Since program will exit after displaying
         #  plugin details, no need to reset this variable.
         #
         verbose = self._plugins_display == 3
 
-        missing_plugins = []
         for name, info in self._used_plugins.items():
             if verbose:
-                sans_prefix = name.split("/")[1]
-                if sans_prefix in plugin_items:
-                    plugin_items.remove(sans_prefix)
-                    suffix = ""
-                else:
-                    suffix = " *** Not installed ***"
+                name = self._name_sans_prefix(name)
+                suffix = self._remove_if_found(
+                    plugin_items, name, " *** Not installed ***"
+                )
                 print("".ljust(len(name) + 2, "-"))
                 print(f"> {name:<{max_l_name - 2}} - {info[PLUGIN_VERS_MIN]} {suffix}")
                 info[PLUGIN_MTHD]()
                 #
                 #  Skip indention, for easier read
                 #
                 for line in info[PLUGIN_STATIC_CODE].split("\n"):
                     # if line == line.strip():
                     print(f"{line.strip()}")
                 # print()
             else:
-                sans_prefix = name.split("/")[1]
-                if sans_prefix in plugin_items:
-                    plugin_items.remove(sans_prefix)
-                    suffix = ""
-                else:
-                    suffix = " *** Not installed ***"
+                name = self._name_sans_prefix(name)
+                suffix = self._remove_if_found(
+                    plugin_items, name, " *** Not installed ***"
+                )
                 print(f"{name:<{max_l_name}} - {info[PLUGIN_VERS_MIN]} {suffix}")
 
+        #  Remove skipped plugins from plugin_items
         for _, name in self._skipped_plugins:
-            if name.find("/") > -1:
-                sans_prefix = name.split("/")[1]
-            else:
-                sans_prefix = name
-            if sans_prefix in plugin_items:
-                plugin_items.remove(sans_prefix)
+            name = self._name_sans_prefix(name)
+            _ = self._remove_if_found(plugin_items, name)
 
         if plugin_items:
             print("\n-----   Unused plugins found   -----")
             for s in plugin_items:
                 print("\t", s)
 
         if not self._skipped_plugins or self._plugins_display != 2:
             sys.exit(0)
 
         if self._skipped_plugins:
             print()
 
+        #
+        #  List all plugins installed, but not used
+        #
         max_l_v = 0
         self._skipped_plugins.sort()
         for vers, name in self._skipped_plugins:
             max_l_v = max(max_l_v, len(vers))
         print("-----   Plugins ignored   -----")
         print(f'{"Min":<{max_l_v}}|{" Plugin name":<{max_l_name}}')
         print(f'{"vers":<{max_l_v}}|\n')
@@ -301,33 +295,17 @@
             xdg_home = os.environ.get(XDG_CONFIG_HOME)
             # pylint: disable=consider-using-assignment-expr
             if xdg_home:
                 conf_base = os.path.expanduser(xdg_home)
             else:
                 conf_base = os.path.dirname(location)
 
-            if not conf_base:
-                raise SyntaxError(
-                    f"conf_base could not be extracted [{xdg_home}] "
-                    + "[tilde_home_dir({self._conf_file})]"
-                )
-
             plugins_dir = os.path.join(conf_base, "tmux", "plugins")
-            if conf_base:
-                tpm_env = f'XDG_CONFIG_HOME="{conf_base}" '
-            else:
-                tpm_env = ""
-        if plugins_dir[0] not in ("/", "~"):  # TODO: Not windows compatible
-            plugins_dir = os.path.join(os.getcwd(), plugins_dir)
+            tpm_env = os.path.expanduser(f'XDG_CONFIG_HOME="{conf_base}" ')
 
-        if tpm_env.find("~") > -1:
-            raise SyntaxError(
-                "XDG_CONFIG_HOME can not contain ~ "
-                + "tpm does not bother with expanduser :("
-            )
         return plugins_dir, tpm_env
 
     def mkscript_manual_deploy(self):
         """This script is run as tmux starts, all non-present
         plugins are installed, and an attempt is done to initialize
         each plugin.
         """
@@ -459,21 +437,19 @@
         self._es.create(self._fnc_activate_tpm, activate_tpm_sh)
         return output
 
     def clear(self):
         """To minimize risk of some bug causing massive file deletion,
         file path is double checked.
         """
-        plugins_dir = self.get_deploy_dir()
+        plugins_dir = self.get_plugin_dir()
 
         b_suspicious = False
         if "tmux/" not in plugins_dir:
             b_suspicious = True
-        elif plugins_dir in ("", "/", os.path.expanduser("~")):
-            b_suspicious = True
 
         if b_suspicious:
             raise FileNotFoundError(
                 "Refusing to clear plugins due to suspicious "
                 + f"plugin dir: [{plugins_dir}]"
             )
 
@@ -483,7 +459,18 @@
         for file_name in os.listdir(plugins_dir):
             path = os.path.join(plugins_dir, file_name)
             print(f"removing plugin {file_name}")
             try:
                 shutil.rmtree(path)
             except OSError:
                 os.remove(path)
+
+    def _name_sans_prefix(self, name: str) -> str:
+        if name.find("/") > -1:
+            name = name.split("/")[1]
+        return name
+
+    def _remove_if_found(self, lst: list, item: str, warning: str = "") -> str:
+        if item in lst:
+            lst.remove(item)
+            warning = ""
+        return warning
```

### Comparing `tmux_conf-0.15.8/src/tmux_conf/tmux_conf.py` & `tmux_conf-0.15.9/src/tmux_conf/tmux_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,14 +438,15 @@
             return
 
         #
         #  Convert to lines actually to be written
         #
         lines: list[str] = []
         for raw_line in cmd.split("\n"):
+            ## print(f">> raw_line [{raw_line}]")
             #
             #  Returns a list of lines. If input contained a -N and notes
             #  are not supported by this tmux, the note is extracted and
             #  the following is returned.
             #  self.use_notes_as_comments = True
             #   - empty string, vertical spacer
             #   - note as a comment
@@ -487,17 +488,18 @@
             or line.find("-N") < 0
             or (self.vers_ok("3.1") and self.use_notes_as_comments)
         ):
             return [line]
         parts = line.split("-N")
         pre = parts[0].strip()
         post = parts[1].strip()
+        print(f">> pre [{pre}] [{post}]")
         if not post:
             # Propably an -N at end of line, so not related to a note
-            return [line]
+            return [pre]
         p0 = post[0]
         if p0 in {'"', "'"}:
             end_note = post[1:].find(p0)
             x = end_note + 1
             note = post[1:x]
             y = end_note + 2
             post = post[y:]
@@ -556,16 +558,15 @@
 
         """
         # Do a basic sanity check
         if self.is_tmux_bin(cmd):
             self.tmux_bin = cmd
             self.define_tmux_vers()
         else:
-            print(f"ERROR: tmux bin seems invalid: {cmd}")
-            sys.exit(1)
+            sys.exit(f"ERROR: tmux bin seems invalid: {cmd}")
 
     def find_tmux_bin(self, cmd: str = "") -> bool:
         if not cmd:
             #  Use the first that gives something
             cmd = self.find_cmd_1() or self.find_cmd_2() or self.find_cmd_3()
 
         if cmd:
@@ -658,15 +659,15 @@
             print(f"found {cmd} in PATH")
         return cmd
 
     def find_cmd_3(self):
         """Finally try some likely locations"""
         cmd = ""
         for c in (
-            "/usr/local/bin",
+            "/usr/local/bin/tmux",
             "/home/linuxbrew/.linuxbrew/bin/tmux",
             "~/.asdf/shims/tmux",
         ):
             c2 = expanduser_plus(c)
             if is_executable(c2):
                 cmd = c2
                 break
```

### Comparing `tmux_conf-0.15.8/src/tmux_conf/utils.py` & `tmux_conf-0.15.9/src/tmux_conf/utils.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.15.8/src/tmux_conf/vers_check.py` & `tmux_conf-0.15.9/src/tmux_conf/vers_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,16 @@
         #  for compatibility checks only the first two are needed
         #  This syntax handles both normal tmux and tmate
         #
         parts = self._vers.split(".")
         v_maj = parts[0]
         try:
             v_min = parts[1]
-        except IndexError as exc:
-            print(f"ERROR: Failed to extract v_min: {self._vers}")
-            raise IndexError from exc
+        except IndexError:
+            raise IndexError(f"ERROR: Failed to extract v_min: {self._vers}")
         try:
             self.v_maj = int(v_maj)
         except ValueError as exc:
             print(f"Error: v_maj was not int: {self._vers}")
             raise ValueError from exc
         self.v_min, self.v_suffix = self.get_sub_vers(v_min)
```

### Comparing `tmux_conf-0.15.8/src/tmux_conf.egg-info/PKG-INFO` & `tmux_conf-0.15.9/src/tmux_conf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmux-conf
-Version: 0.15.8
+Version: 0.15.9
 Summary: Generates version checked tmux conf
 Author-email: Jacob Lundqvist <Jacob.Lundqvist@gmail.com>
 Project-URL: Homepage, https://github.com/jaclu/tmux-conf
 Project-URL: documentation, https://github.com/jaclu/tmux-conf
 Project-URL: repository, https://github.com/jaclu/tmux-conf
 Project-URL: Bug Tracker, https://github.com/jaclu/tmux-conf/issues
 Keywords: tmux,automation
```

