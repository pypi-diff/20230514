# Comparing `tmp/test_helper_vbot3-1.0.tar.gz` & `tmp/test_helper_vbot3-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_helper_vbot3-1.0.tar", last modified: Sun May 14 08:28:12 2023, max compression
+gzip compressed data, was "test_helper_vbot3-1.1.tar", last modified: Sun May 14 16:10:45 2023, max compression
```

## Comparing `test_helper_vbot3-1.0.tar` & `test_helper_vbot3-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 08:28:12.719166 test_helper_vbot3-1.0/
--rw-rw-rw-   0        0        0     1094 2023-05-13 15:59:41.000000 test_helper_vbot3-1.0/LICENSE
--rw-rw-rw-   0        0        0       60 2023-05-13 16:18:16.000000 test_helper_vbot3-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      563 2023-05-14 08:28:12.719166 test_helper_vbot3-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       39 2023-05-13 15:59:41.000000 test_helper_vbot3-1.0/README.md
--rw-rw-rw-   0        0        0      110 2023-04-18 12:37:07.000000 test_helper_vbot3-1.0/pyproject.toml
--rw-rw-rw-   0        0        0      707 2023-05-14 08:28:12.719166 test_helper_vbot3-1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 08:28:12.703541 test_helper_vbot3-1.0/test_helper_vbot3.egg-info/
--rw-rw-rw-   0        0        0      563 2023-05-14 08:28:12.000000 test_helper_vbot3-1.0/test_helper_vbot3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-05-14 08:28:12.000000 test_helper_vbot3-1.0/test_helper_vbot3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 08:28:12.000000 test_helper_vbot3-1.0/test_helper_vbot3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-14 08:28:12.000000 test_helper_vbot3-1.0/test_helper_vbot3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-14 08:28:12.000000 test_helper_vbot3-1.0/test_helper_vbot3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 08:28:12.719166 test_helper_vbot3-1.0/tester_vbot3/
--rw-rw-rw-   0        0        0     3629 2023-05-14 08:25:59.000000 test_helper_vbot3-1.0/tester_vbot3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 16:10:45.304287 test_helper_vbot3-1.1/
+-rw-rw-rw-   0        0        0     1094 2023-05-13 15:59:41.000000 test_helper_vbot3-1.1/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-05-14 08:37:46.000000 test_helper_vbot3-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1036 2023-05-14 16:10:45.304287 test_helper_vbot3-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-05-14 08:39:31.000000 test_helper_vbot3-1.1/README.md
+-rw-rw-rw-   0        0        0      110 2023-05-14 08:37:46.000000 test_helper_vbot3-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      707 2023-05-14 16:10:45.319913 test_helper_vbot3-1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 16:10:45.304287 test_helper_vbot3-1.1/test_helper_vbot3.egg-info/
+-rw-rw-rw-   0        0        0     1036 2023-05-14 16:10:45.000000 test_helper_vbot3-1.1/test_helper_vbot3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-05-14 16:10:45.000000 test_helper_vbot3-1.1/test_helper_vbot3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 16:10:45.000000 test_helper_vbot3-1.1/test_helper_vbot3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-14 16:10:45.000000 test_helper_vbot3-1.1/test_helper_vbot3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-14 16:10:45.000000 test_helper_vbot3-1.1/test_helper_vbot3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 16:10:45.304287 test_helper_vbot3-1.1/tester_vbot3/
+-rw-rw-rw-   0        0        0     3152 2023-05-14 15:59:18.000000 test_helper_vbot3-1.1/tester_vbot3/__init__.py
```

### Comparing `test_helper_vbot3-1.0/LICENSE` & `test_helper_vbot3-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `test_helper_vbot3-1.0/setup.cfg` & `test_helper_vbot3-1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6573 745f 6865 6c70 6572 5f76   = test_helper_v
 00000020: 626f 7433 0d0a 7665 7273 696f 6e20 3d20  bot3..version = 
-00000030: 312e 300d 0a61 7574 686f 7220 3d20 5669  1.0..author = Vi
+00000030: 312e 310d 0a61 7574 686f 7220 3d20 5669  1.1..author = Vi
 00000040: 7461 6c79 2042 6f67 6f6d 6f6c 6f76 0d0a  taly Bogomolov..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 206d  author_email = m
 00000060: 6169 6c40 7669 7461 6c79 2d62 6f67 6f6d  ail@vitaly-bogom
 00000070: 6f6c 6f76 2e72 750d 0a64 6573 6372 6970  olov.ru..descrip
 00000080: 7469 6f6e 203d 2054 6573 7465 7220 666f  tion = Tester fo
 00000090: 7220 5662 6f74 330d 0a6c 6f6e 675f 6465  r Vbot3..long_de
 000000a0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
```

### Comparing `test_helper_vbot3-1.0/tester_vbot3/__init__.py` & `test_helper_vbot3-1.1/tester_vbot3/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,41 +24,30 @@
         """Get method emulator."""
         self.timeout = timeout
         if url not in self.calls:
             self.calls[url] = 0
         self.calls[url] += 1
 
 
-def start_command_dflt(message, bot):
-    """Handle private /start command."""
-    user = bot.user_entry_point(message)
-    bot.reply(message, "Hi ID {}".format(user.key.id()))
-
-
 class Vbot3Tester(TestFlask, TestGae3, Telemulator):
     """Tester for Vbot3."""
 
     teleuser = None
     private = None
     group = None
 
-    def init(self, flask_app, vbot3, bot_name, bot_username, queue_yaml_dir, start_command_cust=None):
+    def init(self, flask_app, vbot3, bot_name, bot_username, queue_yaml_dir):
         """Init tests stuff."""
         TestFlask.set_up(self, flask_app)
         TestGae3.set_up(self, queue_yaml_dir)
         self.set_tested_bot(vbot3, name=bot_name, username=bot_username)
 
-        start_command = start_command_cust or start_command_dflt
-        vbot3.private_command('start')(lambda msg: start_command(msg, vbot3))
-        vbot3.set_default_content_handlers()  # must be last in handlers chain
-
         self.teleuser = self.api.create_user('Test', 'User', language_code='en')
         self.private = self.teleuser.private()
         self.group = self.teleuser.create_group("Test group")
-        self.private_command('/start')
 
     def tearDown(self):
         """Clear tests."""
         TestGae3.tear_down(self)
         super().tearDown()
 
     def private_command(self, cmd, from_user=None):
```

