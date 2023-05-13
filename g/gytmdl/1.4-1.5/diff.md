# Comparing `tmp/gytmdl-1.4.tar.gz` & `tmp/gytmdl-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gytmdl-1.4.tar", last modified: Fri Apr 14 01:29:31 2023, max compression
+gzip compressed data, was "gytmdl-1.5.tar", last modified: Sat May 13 22:32:33 2023, max compression
```

## Comparing `gytmdl-1.4.tar` & `gytmdl-1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1176 2023-04-14 01:29:26.637009 gytmdl-1.4/.github/workflows/main.yml
--rw-r--r--   0        0        0       80 2023-04-14 01:29:26.637009 gytmdl-1.4/.gitignore
--rw-r--r--   0        0        0     2350 2023-04-14 01:29:26.637009 gytmdl-1.4/README.md
--rw-r--r--   0        0        0     4145 2023-04-14 01:29:26.637009 gytmdl-1.4/gytmdl/__init__.py
--rw-r--r--   0        0        0       58 2023-04-14 01:29:26.637009 gytmdl-1.4/gytmdl/__main__.py
--rw-r--r--   0        0        0     6713 2023-04-14 01:29:26.637009 gytmdl-1.4/gytmdl/gytmdl.py
--rw-r--r--   0        0        0      456 2023-04-14 01:29:26.637009 gytmdl-1.4/pyproject.toml
--rw-r--r--   0        0        0       18 2023-04-14 01:29:26.637009 gytmdl-1.4/requirements.txt
--rw-r--r--   0        0        0     2674 1970-01-01 00:00:00.000000 gytmdl-1.4/PKG-INFO
+-rw-r--r--   0        0        0     1176 2023-05-13 22:32:29.661591 gytmdl-1.5/.github/workflows/main.yml
+-rw-r--r--   0        0        0       80 2023-05-13 22:32:29.661591 gytmdl-1.5/.gitignore
+-rw-r--r--   0        0        0     2692 2023-05-13 22:32:29.661591 gytmdl-1.5/README.md
+-rw-r--r--   0        0        0     4145 2023-05-13 22:32:29.661591 gytmdl-1.5/gytmdl/__init__.py
+-rw-r--r--   0        0        0       58 2023-05-13 22:32:29.661591 gytmdl-1.5/gytmdl/__main__.py
+-rw-r--r--   0        0        0     6718 2023-05-13 22:32:29.661591 gytmdl-1.5/gytmdl/gytmdl.py
+-rw-r--r--   0        0        0      456 2023-05-13 22:32:29.661591 gytmdl-1.5/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-05-13 22:32:29.661591 gytmdl-1.5/requirements.txt
+-rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 gytmdl-1.5/PKG-INFO
```

### Comparing `gytmdl-1.4/.github/workflows/main.yml` & `gytmdl-1.5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gytmdl-1.4/README.md` & `gytmdl-1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Glomatico's YouTube Music Downloader
-Download YouTube Music songs/albums/playlists with tags from YouTube Music in 128kbps AAC/128kbps Opus/256kbps AAC and following the iTunes standard.
+Download YouTube Music songs/albums/playlists with tags from YouTube Music in 256kbps AAC/128kbps Opus/128kbps AAC.
+
+## Why not just use yt-dlp directly?
+While this project uses yt-dlp under the hood to download songs from YouTube Music, it has the advantage of utilizing [YouTube Music's API](https://github.com/sigma67/ytmusicapi) to get songs metadata, ensuring that you get the correct tags for your songs. This includes information such as track number, square cover, lyrics, year, etc.
 
 ## Setup
 1. Install Python 3.8 or higher
 2. Install gytmdl with pip
     ```
     pip install gytmdl
     ```
```

### Comparing `gytmdl-1.4/gytmdl/__init__.py` & `gytmdl-1.5/gytmdl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import shutil
 import argparse
 import traceback
 from .gytmdl import Gytmdl
 
-__version__ = '1.4'
+__version__ = '1.5'
 
 
 def main():
     if not shutil.which('ffmpeg'):
         raise Exception('ffmpeg is not on PATH')
     parser = argparse.ArgumentParser(
         description='Download YouTube Music songs/albums/playlists with tags from YouTube Music',
```

### Comparing `gytmdl-1.4/gytmdl/gytmdl.py` & `gytmdl-1.5/gytmdl/gytmdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         video_id = ytmusic_watch_playlist['tracks'][0]['videoId']
         ytmusic_album = self.ytmusic.get_album(ytmusic_watch_playlist['tracks'][0]['album']['id'])
         tags = {
             '\xa9alb': [ytmusic_album['title']],
             'aART': [self.get_artist(ytmusic_album['artists'])],
             '\xa9ART': [self.get_artist(ytmusic_watch_playlist['tracks'][0]['artists'])],
             '\xa9cmt': [f'https://music.youtube.com/watch?v={video_id}'],
-            'covr': [MP4Cover(self.get_cover(f'{ytmusic_watch_playlist["tracks"][0]["thumbnail"][0]["url"].split("=")[0]}=w600'))],
+            'covr': [MP4Cover(self.get_cover(f'{ytmusic_watch_playlist["tracks"][0]["thumbnail"][0]["url"].split("=")[0]}=w1200-l94'))],
             '\xa9nam': [ytmusic_watch_playlist['tracks'][0]['title']],
             'stik': [1],
         }
         if ytmusic_album.get('year'):
             tags['\xa9day'] = [ytmusic_album['year']]
         if ytmusic_watch_playlist['lyrics']:
             lyrics = self.ytmusic.get_lyrics(ytmusic_watch_playlist['lyrics'])['lyrics']
```

### Comparing `gytmdl-1.4/PKG-INFO` & `gytmdl-1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: gytmdl
-Version: 1.4
+Version: 1.5
 Summary: Download YouTube Music songs/albums/playlists with tags from YouTube Music
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: yt-dlp
 Requires-Dist: ytmusicapi
 Project-URL: repository, https://github.com/glomatico/gytmdl
 
 # Glomatico's YouTube Music Downloader
-Download YouTube Music songs/albums/playlists with tags from YouTube Music in 128kbps AAC/128kbps Opus/256kbps AAC and following the iTunes standard.
+Download YouTube Music songs/albums/playlists with tags from YouTube Music in 256kbps AAC/128kbps Opus/128kbps AAC.
+
+## Why not just use yt-dlp directly?
+While this project uses yt-dlp under the hood to download songs from YouTube Music, it has the advantage of utilizing [YouTube Music's API](https://github.com/sigma67/ytmusicapi) to get songs metadata, ensuring that you get the correct tags for your songs. This includes information such as track number, square cover, lyrics, year, etc.
 
 ## Setup
 1. Install Python 3.8 or higher
 2. Install gytmdl with pip
     ```
     pip install gytmdl
     ```
```

