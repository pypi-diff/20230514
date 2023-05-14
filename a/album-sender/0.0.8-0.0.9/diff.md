# Comparing `tmp/album_sender-0.0.8.tar.gz` & `tmp/album_sender-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/album_sender-0.0.8.tar", last modified: Sun May  3 12:10:44 2020, max compression
+gzip compressed data, was "dist/album_sender-0.0.9.tar", last modified: Thu May  7 13:28:21 2020, max compression
```

## Comparing `album_sender-0.0.8.tar` & `album_sender-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-05-03 12:10:44.000000 album_sender-0.0.8/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      791 2020-05-03 12:10:44.000000 album_sender-0.0.8/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      218 2020-03-23 13:52:41.000000 album_sender-0.0.8/README.md
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-05-03 12:10:44.000000 album_sender-0.0.8/album_sender/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1362 2020-05-03 12:10:37.000000 album_sender-0.0.8/album_sender/__init__.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-05-03 12:10:44.000000 album_sender-0.0.8/album_sender.egg-info/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      791 2020-05-03 12:10:44.000000 album_sender-0.0.8/album_sender.egg-info/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      222 2020-05-03 12:10:44.000000 album_sender-0.0.8/album_sender.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-05-03 12:10:44.000000 album_sender-0.0.8/album_sender.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       33 2020-05-03 12:10:44.000000 album_sender-0.0.8/album_sender.egg-info/requires.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       13 2020-05-03 12:10:44.000000 album_sender-0.0.8/album_sender.egg-info/top_level.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-05-03 12:10:44.000000 album_sender-0.0.8/setup.cfg
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      746 2020-05-03 12:10:32.000000 album_sender-0.0.8/setup.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-05-07 13:28:21.000000 album_sender-0.0.9/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      791 2020-05-07 13:28:21.000000 album_sender-0.0.9/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      218 2020-03-23 13:52:41.000000 album_sender-0.0.9/README.md
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-05-07 13:28:21.000000 album_sender-0.0.9/album_sender/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1642 2020-05-07 13:25:54.000000 album_sender-0.0.9/album_sender/__init__.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-05-07 13:28:21.000000 album_sender-0.0.9/album_sender.egg-info/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      791 2020-05-07 13:28:21.000000 album_sender-0.0.9/album_sender.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      222 2020-05-07 13:28:21.000000 album_sender-0.0.9/album_sender.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-05-07 13:28:21.000000 album_sender-0.0.9/album_sender.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       33 2020-05-07 13:28:21.000000 album_sender-0.0.9/album_sender.egg-info/requires.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       13 2020-05-07 13:28:21.000000 album_sender-0.0.9/album_sender.egg-info/top_level.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-05-07 13:28:21.000000 album_sender-0.0.9/setup.cfg
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      746 2020-05-07 13:28:17.000000 album_sender-0.0.9/setup.py
```

### Comparing `album_sender-0.0.8/PKG-INFO` & `album_sender-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: album_sender
-Version: 0.0.8
+Version: 0.0.9
 Summary: Telegram album sender.
 Home-page: https://github.com/gaoyunzhi/telegram_album_sender
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # album_sender
```

### Comparing `album_sender-0.0.8/album_sender/__init__.py` & `album_sender-0.0.9/album_sender/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 from PIL import Image
 from telegram import InputMediaPhoto, InputMediaVideo
 import cached_url
 import pic_cut
 from telegram_util import cutCaption
 import os
 
+def isAnimated(path):
+	gif = Image.open(path)
+	try:
+		gif.seek(1)
+	except EOFError:
+		return False
+	else:
+		return True
+
 def properSize(fn):
 	size = os.stat(fn).st_size
 	return 0 < size and size < (1 << 23)
 
 def send(chat, url, result, rotate=0):
 	suffix = '[source](%s)' % url
 
@@ -30,15 +39,19 @@
 		if rotate:
 			if rotate == True:
 				rotate = 180
 			for img_path in imgs:
 				img = Image.open(img_path)
 				img = img.rotate(rotate, expand=True)
 				img.save(img_path)
+		cap = cutCaption(result.cap, suffix, 1000)
 		group = [InputMediaPhoto(open(imgs[0], 'rb'), 
-			caption=cutCaption(result.cap, suffix, 1000), parse_mode='Markdown')] + \
+			caption=cap, parse_mode='Markdown')] + \
 			[InputMediaPhoto(open(x, 'rb')) for x in imgs[1:]]
+		if isAnimated(imgs[0]):
+			return chat.bot.send_document(chat.id, open(imgs[0], 'rb'), 
+				caption=cap, parse_mode='Markdown', timeout = 20*60)
 		return chat.bot.send_media_group(chat.id, group, timeout = 20*60)
 
 	if result.cap:
 		return [chat.send_message(cutCaption(result.cap, suffix, 4000), 
 			parse_mode='Markdown', timeout = 20*60)]
```

### Comparing `album_sender-0.0.8/album_sender.egg-info/PKG-INFO` & `album_sender-0.0.9/album_sender.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: album-sender
-Version: 0.0.8
+Version: 0.0.9
 Summary: Telegram album sender.
 Home-page: https://github.com/gaoyunzhi/telegram_album_sender
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # album_sender
```

### Comparing `album_sender-0.0.8/setup.py` & `album_sender-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="album_sender",
-    version="0.0.8",
+    version="0.0.9",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Telegram album sender.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/telegram_album_sender",
     packages=setuptools.find_packages(),
```

