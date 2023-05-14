# Comparing `tmp/musiclib-1.9.3.tar.gz` & `tmp/musiclib-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musiclib-1.9.3.tar", last modified: Sat Dec 24 16:04:32 2022, max compression
+gzip compressed data, was "musiclib-1.9.4.tar", last modified: Sun Jan 15 19:34:16 2023, max compression
```

## Comparing `musiclib-1.9.3.tar` & `musiclib-1.9.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 16:04:32.161282 musiclib-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2022-12-24 16:04:32.161282 musiclib-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2022-12-24 16:04:22.000000 musiclib-1.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2022-12-24 16:04:32.161282 musiclib-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-24 16:04:22.000000 musiclib-1.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 16:04:32.157282 musiclib-1.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 16:04:32.157282 musiclib-1.9.3/src/musiclib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/chord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 16:04:32.157282 musiclib-1.9.3/src/musiclib/midi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/midi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/midi/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/midi/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/noterange.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/noteset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13526 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/piano.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/pitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/progression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/rhythm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/scale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 16:04:32.157282 musiclib-1.9.3/src/musiclib/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/util/etc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/util/sequence_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/util/typeguards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 16:04:32.161282 musiclib-1.9.3/src/musiclib/voice_leading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/voice_leading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/voice_leading/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/voice_leading/transition.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2022-12-24 16:04:22.000000 musiclib-1.9.3/src/musiclib/voice_leading/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 16:04:32.157282 musiclib-1.9.3/src/musiclib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2022-12-24 16:04:32.000000 musiclib-1.9.3/src/musiclib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      854 2022-12-24 16:04:32.000000 musiclib-1.9.3/src/musiclib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-24 16:04:32.000000 musiclib-1.9.3/src/musiclib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2022-12-24 16:04:32.000000 musiclib-1.9.3/src/musiclib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-24 16:04:32.000000 musiclib-1.9.3/src/musiclib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 19:34:16.525750 musiclib-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-01-15 19:34:16.525750 musiclib-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-01-15 19:34:02.000000 musiclib-1.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-01-15 19:34:16.525750 musiclib-1.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-15 19:34:02.000000 musiclib-1.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 19:34:16.521750 musiclib-1.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 19:34:16.521750 musiclib-1.9.4/src/musiclib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/chord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 19:34:16.525750 musiclib-1.9.4/src/musiclib/midi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/midi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/midi/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/midi/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/noterange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/noteset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13526 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/piano.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/pitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/progression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/rhythm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 19:34:16.525750 musiclib-1.9.4/src/musiclib/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/util/etc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/util/sequence_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/util/typeguards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 19:34:16.525750 musiclib-1.9.4/src/musiclib/voice_leading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/voice_leading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/voice_leading/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/voice_leading/transition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-01-15 19:34:02.000000 musiclib-1.9.4/src/musiclib/voice_leading/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 19:34:16.521750 musiclib-1.9.4/src/musiclib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-01-15 19:34:16.000000 musiclib-1.9.4/src/musiclib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-01-15 19:34:16.000000 musiclib-1.9.4/src/musiclib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-15 19:34:16.000000 musiclib-1.9.4/src/musiclib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-15 19:34:16.000000 musiclib-1.9.4/src/musiclib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-15 19:34:16.000000 musiclib-1.9.4/src/musiclib.egg-info/top_level.txt
```

### Comparing `musiclib-1.9.3/PKG-INFO` & `musiclib-1.9.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musiclib
-Version: 1.9.3
+Version: 1.9.4
 Summary: set of tools to work with scales, modes, modulations, chord progressions, voice leading, rhythm and more
 Home-page: https://github.com/tandav/musiclib
 Author: Alexander Rodionov
 Author-email: tandav@tandav.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
```

### Comparing `musiclib-1.9.3/README.md` & `musiclib-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/setup.cfg` & `musiclib-1.9.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = musiclib
-version = 1.9.3
+version = 1.9.4
 description = set of tools to work with scales, modes, modulations, chord progressions, voice leading, rhythm and more
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tandav/musiclib
 author = Alexander Rodionov
 author_email = tandav@tandav.me
 classifiers = 
@@ -84,15 +84,15 @@
 max-line-length = 200
 max-complexity = 10
 recursive = true
 aggressive = 3
 jobs = 8
 
 [bumpver]
-current_version = "v1.9.3"
+current_version = "v1.9.4"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = True
 tag = True
 
 [bumpver:file_patterns]
 setup.cfg =
```

### Comparing `musiclib-1.9.3/src/musiclib/chord.py` & `musiclib-1.9.4/src/musiclib/chord.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib/config.py` & `musiclib-1.9.4/src/musiclib/config.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib/midi/parse.py` & `musiclib-1.9.4/src/musiclib/midi/parse.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib/midi/player.py` & `musiclib-1.9.4/src/musiclib/midi/player.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib/note.py` & `musiclib-1.9.4/src/musiclib/note.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib/noterange.py` & `musiclib-1.9.4/src/musiclib/noterange.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib/noteset.py` & `musiclib-1.9.4/src/musiclib/noteset.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
             self.root = root
             root_i = self.notes_octave_fit.index(self.root)
             self.notes_ascending = self.notes_octave_fit[root_i:] + self.notes_octave_fit[:root_i]
             self.intervals_ascending = tuple(note - self.root for note in self.notes_ascending)
         self.intervals = frozenset(self.intervals_ascending)
         self.note_to_interval = dict(zip(self.notes_ascending, self.intervals_ascending))
         self.bits = intervals_to_bits(self.intervals)
+        self.bits_notes = tuple(int(Note(note) in self.notes) for note in config.chromatic_notes)
         self.name = self.__class__.intervals_to_name.get(self.intervals)
 
         self.key = self.notes, self.root
         self.note_i = {note: i for i, note in enumerate(self.notes_ascending)}
 
     @property
     def rootless(self) -> NoteSet:
```

### Comparing `musiclib-1.9.3/src/musiclib/piano.py` & `musiclib-1.9.4/src/musiclib/piano.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib/pitch.py` & `musiclib-1.9.4/src/musiclib/pitch.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib/progression.py` & `musiclib-1.9.4/src/musiclib/progression.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib/rhythm.py` & `musiclib-1.9.4/src/musiclib/rhythm.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib/scale.py` & `musiclib-1.9.4/src/musiclib/scale.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib/util/sequence_builder.py` & `musiclib-1.9.4/src/musiclib/util/sequence_builder.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib/voice_leading/checks.py` & `musiclib-1.9.4/src/musiclib/voice_leading/checks.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib/voice_leading/transition.py` & `musiclib-1.9.4/src/musiclib/voice_leading/transition.py`

 * *Files identical despite different names*

### Comparing `musiclib-1.9.3/src/musiclib.egg-info/PKG-INFO` & `musiclib-1.9.4/src/musiclib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musiclib
-Version: 1.9.3
+Version: 1.9.4
 Summary: set of tools to work with scales, modes, modulations, chord progressions, voice leading, rhythm and more
 Home-page: https://github.com/tandav/musiclib
 Author: Alexander Rodionov
 Author-email: tandav@tandav.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
```

### Comparing `musiclib-1.9.3/src/musiclib.egg-info/SOURCES.txt` & `musiclib-1.9.4/src/musiclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

