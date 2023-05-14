# Comparing `tmp/mafic-2.3.1.tar.gz` & `tmp/mafic-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafic-2.3.1.tar", max compression
+gzip compressed data, was "mafic-2.4.0.tar", max compression
```

## Comparing `mafic-2.3.1.tar` & `mafic-2.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1070 2023-05-09 22:38:17.961736 mafic-2.3.1/LICENSE
--rw-r--r--   0        0        0     3315 2023-05-09 22:38:17.961736 mafic-2.3.1/README.md
--rw-r--r--   0        0        0      886 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/__init__.py
--rw-r--r--   0        0        0     3554 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/__libraries.py
--rw-r--r--   0        0        0     1559 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/__main__.py
--rw-r--r--   0        0        0     4490 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/errors.py
--rw-r--r--   0        0        0     5617 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/events.py
--rw-r--r--   0        0        0    27782 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/filter.py
--rw-r--r--   0        0        0     7397 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/ip.py
--rw-r--r--   0        0        0    39072 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/node.py
--rw-r--r--   0        0        0    24952 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/player.py
--rw-r--r--   0        0        0     1232 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/playlist.py
--rw-r--r--   0        0        0      674 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/plugin.py
--rw-r--r--   0        0        0     8715 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/pool.py
--rw-r--r--   0        0        0        0 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/py.typed
--rw-r--r--   0        0        0     3648 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/region.py
--rw-r--r--   0        0        0     1031 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/search_type.py
--rw-r--r--   0        0        0     3437 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/stats.py
--rw-r--r--   0        0        0     5254 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/strategy.py
--rw-r--r--   0        0        0     4797 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/track.py
--rw-r--r--   0        0        0      747 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/type_variables.py
--rw-r--r--   0        0        0      199 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/typings/__init__.py
--rw-r--r--   0        0        0     2996 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/typings/common.py
--rw-r--r--   0        0        0     4712 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/typings/http.py
--rw-r--r--   0        0        0     2385 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/typings/incoming.py
--rw-r--r--   0        0        0      602 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/typings/misc.py
--rw-r--r--   0        0        0     1189 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/typings/outgoing.py
--rw-r--r--   0        0        0      117 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/utils/__init__.py
--rw-r--r--   0        0        0     1203 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/utils/classproperty.py
--rw-r--r--   0        0        0      745 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/warnings.py
--rw-r--r--   0        0        0     3766 2023-05-09 22:38:17.965736 mafic-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-14 14:24:27.975055 mafic-2.4.0/LICENSE
+-rw-r--r--   0        0        0     3315 2023-05-14 14:24:27.975055 mafic-2.4.0/README.md
+-rw-r--r--   0        0        0      886 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/__init__.py
+-rw-r--r--   0        0        0     3554 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/__libraries.py
+-rw-r--r--   0        0        0     1559 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/__main__.py
+-rw-r--r--   0        0        0     4490 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/errors.py
+-rw-r--r--   0        0        0     5617 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/events.py
+-rw-r--r--   0        0        0    27782 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/filter.py
+-rw-r--r--   0        0        0     7397 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/ip.py
+-rw-r--r--   0        0        0    39388 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/node.py
+-rw-r--r--   0        0        0    25321 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/player.py
+-rw-r--r--   0        0        0     1232 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/playlist.py
+-rw-r--r--   0        0        0      674 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/plugin.py
+-rw-r--r--   0        0        0     8715 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/pool.py
+-rw-r--r--   0        0        0        0 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/py.typed
+-rw-r--r--   0        0        0     3648 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/region.py
+-rw-r--r--   0        0        0     1031 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/search_type.py
+-rw-r--r--   0        0        0     3437 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/stats.py
+-rw-r--r--   0        0        0     5254 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/strategy.py
+-rw-r--r--   0        0        0     4797 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/track.py
+-rw-r--r--   0        0        0      747 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/type_variables.py
+-rw-r--r--   0        0        0      199 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/typings/__init__.py
+-rw-r--r--   0        0        0     2996 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/typings/common.py
+-rw-r--r--   0        0        0     4712 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/typings/http.py
+-rw-r--r--   0        0        0     2385 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/typings/incoming.py
+-rw-r--r--   0        0        0      602 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/typings/misc.py
+-rw-r--r--   0        0        0     1189 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/typings/outgoing.py
+-rw-r--r--   0        0        0      117 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/utils/__init__.py
+-rw-r--r--   0        0        0     1203 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/utils/classproperty.py
+-rw-r--r--   0        0        0      745 2023-05-14 14:24:27.979055 mafic-2.4.0/mafic/warnings.py
+-rw-r--r--   0        0        0     3766 2023-05-14 14:24:27.979055 mafic-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.4.0/PKG-INFO
```

### Comparing `mafic-2.3.1/LICENSE` & `mafic-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/README.md` & `mafic-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/__init__.py` & `mafic-2.4.0/mafic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .track import *
 from .warnings import *
 
 __title__ = "mafic"
 __author__ = "ooliver1"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present ooliver1"
-__version__ = "2.3.1"
+__version__ = "2.4.0"
 """The current version of mafic, using `PEP 440`_ format.
 
 .. _PEP 440: https://peps.python.org/pep-0440/
 """
 
 del __libraries
```

### Comparing `mafic-2.3.1/mafic/__libraries.py` & `mafic-2.4.0/mafic/__libraries.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/__main__.py` & `mafic-2.4.0/mafic/__main__.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/errors.py` & `mafic-2.4.0/mafic/errors.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/events.py` & `mafic-2.4.0/mafic/events.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/filter.py` & `mafic-2.4.0/mafic/filter.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/ip.py` & `mafic-2.4.0/mafic/ip.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/node.py` & `mafic-2.4.0/mafic/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -876,31 +876,35 @@
             "DELETE", f"sessions/{self._session_id}/players/{guild_id}"
         )
 
     def update(
         self,
         *,
         guild_id: int,
-        track: Track | None = MISSING,
+        track: Track | str | None = MISSING,
         position: int | None = None,
         end_time: int | None = None,
         volume: int | None = None,
         no_replace: bool | None = None,
         pause: bool | None = None,
         filter: Filter | None = None,
-    ) -> Coro[None]:
+    ) -> Coro[PlayerPayload]:
         """Update a player.
 
         Parameters
         ----------
         guild_id:
             The guild ID to update the player for.
         track:
             The track to update the player with.
+            This can be either a :class:`Track` or an identifier.
             Setting this to ``None`` will clear the track.
+
+            .. versionchanged:: 2.4
+                The track can now be a :class:`str` to play an identifier.
         position:
             The position to update the player with.
         end_time:
             The position in the track to stop playing.
         volume:
             The volume to set.
         no_replace:
@@ -909,15 +913,18 @@
             Whether to pause the player.
         filter:
             The filter to apply to the player.
         """
         data: UpdatePlayerPayload = {}
 
         if track is not MISSING:
-            data["encodedTrack"] = track.id if track is not None else None
+            if isinstance(track, Track) or track is None:
+                data["encodedTrack"] = track.id if track is not None else None
+            else:
+                data["identifier"] = track
 
         if position is not None:
             data["position"] = position
 
         if end_time is not None:
             data["endTime"] = end_time
```

### Comparing `mafic-2.3.1/mafic/player.py` & `mafic-2.4.0/mafic/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -528,28 +528,31 @@
             raw_type = search_type
 
         return await node.fetch_tracks(query, search_type=raw_type)
 
     async def update(
         self,
         *,
-        track: Track | None = MISSING,
+        track: Track | str | None = MISSING,
         position: int | None = None,
         end_time: int | None = None,
         volume: int | None = None,
         pause: bool | None = None,
         filter: Filter | None = None,
         replace: bool = False,
     ) -> None:
         """Update the player.
 
         Parameters
         ----------
         track:
-            The track to play.
+            The track to play. This can be a :class:`Track` or an identifier.
+
+            .. versionchanged:: 2.4
+                The track can now be a :class:`str` to play an identifier.
         position:
             The position to start the track at.
         end_time:
             The time to end the track at.
         volume:
             The volume to play the track at.
         pause:
@@ -563,51 +566,54 @@
         ------
         PlayerNotConnected
             If the player is not connected to a voice channel.
         """
         if self._node is None or not self._connected:
             raise PlayerNotConnected
 
-        if track is not MISSING:
-            self._current = track
-
-        if position is not None:
-            self._position = position
-
-        await self._node.update(
+        data = await self._node.update(
             guild_id=self._guild_id,
             track=track,
             position=position,
             end_time=end_time,
             volume=volume,
             pause=pause,
             filter=filter,
             no_replace=not replace,
         )
 
-        if pause is not None:
-            self._paused = pause
+        if data["track"]:
+            self._current = Track.from_data_with_info(data["track"])
+
+        if data["volume"]:
+            self._volume = data["volume"]
+
+        if data["paused"]:
+            self._paused = data["paused"]
 
     async def play(
         self,
-        track: Track,
+        track: Track | str,
         /,
         *,
         start_time: int | None = None,
         end_time: int | None = None,
         volume: int | None = None,
         replace: bool = True,
         pause: bool | None = None,
     ) -> None:
         """Play the given track.
 
         Parameters
         ----------
         track:
-            The track to play.
+            The track to play. This can be a :class:`Track` or an identifier.
+
+            .. versionchanged:: 2.4
+                The track can now be a :class:`str` to play an identifier.
         start_time:
             The position to start the track at.
         end_time:
             The time to end the track at.
         volume:
             The volume to play the track at.
         replace:
```

### Comparing `mafic-2.3.1/mafic/playlist.py` & `mafic-2.4.0/mafic/playlist.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/plugin.py` & `mafic-2.4.0/mafic/plugin.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/pool.py` & `mafic-2.4.0/mafic/pool.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/region.py` & `mafic-2.4.0/mafic/region.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/search_type.py` & `mafic-2.4.0/mafic/search_type.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/stats.py` & `mafic-2.4.0/mafic/stats.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/strategy.py` & `mafic-2.4.0/mafic/strategy.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/track.py` & `mafic-2.4.0/mafic/track.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/type_variables.py` & `mafic-2.4.0/mafic/type_variables.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/typings/common.py` & `mafic-2.4.0/mafic/typings/common.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/typings/http.py` & `mafic-2.4.0/mafic/typings/http.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/typings/incoming.py` & `mafic-2.4.0/mafic/typings/incoming.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/typings/misc.py` & `mafic-2.4.0/mafic/typings/misc.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/typings/outgoing.py` & `mafic-2.4.0/mafic/typings/outgoing.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/utils/classproperty.py` & `mafic-2.4.0/mafic/utils/classproperty.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/mafic/warnings.py` & `mafic-2.4.0/mafic/warnings.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.1/pyproject.toml` & `mafic-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mafic"
-version = "2.3.1"
+version = "2.4.0"
 description = "A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord."
 authors = ["ooliver1 <oliverwilkes2006@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ooliver1/mafic"
 homepage = "https://github.com/ooliver1/mafic"
 keywords = [
```

### Comparing `mafic-2.3.1/PKG-INFO` & `mafic-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafic
-Version: 2.3.1
+Version: 2.4.0
 Summary: A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord.
 Home-page: https://github.com/ooliver1/mafic
 License: MIT
 Keywords: nextcord,disnake,discord,disnake.py,lavalink,lavalink.py,pycord,py-cord
 Author: ooliver1
 Author-email: oliverwilkes2006@icloud.com
 Requires-Python: >=3.8,<4.0
```

