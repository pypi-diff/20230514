# Comparing `tmp/aw-cli-1.5.tar.gz` & `tmp/aw-cli-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aw-cli-1.5.tar", last modified: Thu Mar 16 15:49:47 2023, max compression
+gzip compressed data, was "aw-cli-1.5.1.tar", last modified: Sun May 14 12:34:12 2023, max compression
```

## Comparing `aw-cli-1.5.tar` & `aw-cli-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-03-16 15:49:47.046956 aw-cli-1.5/
--rw-r--r--   0 fexh      (1000) fexh      (1000)    35149 2023-03-16 15:43:36.000000 aw-cli-1.5/LICENSE
--rw-r--r--   0 fexh      (1000) fexh      (1000)     2371 2023-03-16 15:49:47.046956 aw-cli-1.5/PKG-INFO
--rw-r--r--   0 fexh      (1000) fexh      (1000)     2110 2023-03-16 15:43:36.000000 aw-cli-1.5/README.md
-drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-03-16 15:49:47.046956 aw-cli-1.5/aw_cli.egg-info/
--rw-r--r--   0 fexh      (1000) fexh      (1000)     2371 2023-03-16 15:49:47.000000 aw-cli-1.5/aw_cli.egg-info/PKG-INFO
--rw-r--r--   0 fexh      (1000) fexh      (1000)      300 2023-03-16 15:49:47.000000 aw-cli-1.5/aw_cli.egg-info/SOURCES.txt
--rw-r--r--   0 fexh      (1000) fexh      (1000)        1 2023-03-16 15:49:47.000000 aw-cli-1.5/aw_cli.egg-info/dependency_links.txt
--rw-r--r--   0 fexh      (1000) fexh      (1000)       42 2023-03-16 15:49:47.000000 aw-cli-1.5/aw_cli.egg-info/entry_points.txt
--rw-r--r--   0 fexh      (1000) fexh      (1000)       58 2023-03-16 15:49:47.000000 aw-cli-1.5/aw_cli.egg-info/requires.txt
--rw-r--r--   0 fexh      (1000) fexh      (1000)        6 2023-03-16 15:49:47.000000 aw-cli-1.5/aw_cli.egg-info/top_level.txt
-drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-03-16 15:49:47.046956 aw-cli-1.5/awcli/
--rw-r--r--   0 fexh      (1000) fexh      (1000)        0 2023-03-16 15:43:36.000000 aw-cli-1.5/awcli/__init__.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)    24642 2023-03-16 15:43:36.000000 aw-cli-1.5/awcli/run.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)    12022 2023-03-16 15:43:36.000000 aw-cli-1.5/awcli/utilities.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)       38 2023-03-16 15:49:47.046956 aw-cli-1.5/setup.cfg
--rw-r--r--   0 fexh      (1000) fexh      (1000)      899 2023-03-16 15:43:36.000000 aw-cli-1.5/setup.py
-drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-03-16 15:49:47.046956 aw-cli-1.5/tests/
--rw-r--r--   0 fexh      (1000) fexh      (1000)      473 2023-03-16 15:43:36.000000 aw-cli-1.5/tests/test_run.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)     2880 2023-03-16 15:43:36.000000 aw-cli-1.5/tests/test_utilities.py
+drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-05-14 12:34:12.579430 aw-cli-1.5.1/
+-rw-r--r--   0 fexh      (1000) fexh      (1000)    35149 2023-05-14 12:33:54.000000 aw-cli-1.5.1/LICENSE
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     2374 2023-05-14 12:34:12.579430 aw-cli-1.5.1/PKG-INFO
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     2111 2023-05-14 12:33:54.000000 aw-cli-1.5.1/README.md
+drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-05-14 12:34:12.579430 aw-cli-1.5.1/aw_cli.egg-info/
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     2374 2023-05-14 12:34:12.000000 aw-cli-1.5.1/aw_cli.egg-info/PKG-INFO
+-rw-r--r--   0 fexh      (1000) fexh      (1000)      300 2023-05-14 12:34:12.000000 aw-cli-1.5.1/aw_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 fexh      (1000) fexh      (1000)        1 2023-05-14 12:34:12.000000 aw-cli-1.5.1/aw_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 fexh      (1000) fexh      (1000)       42 2023-05-14 12:34:12.000000 aw-cli-1.5.1/aw_cli.egg-info/entry_points.txt
+-rw-r--r--   0 fexh      (1000) fexh      (1000)       47 2023-05-14 12:34:12.000000 aw-cli-1.5.1/aw_cli.egg-info/requires.txt
+-rw-r--r--   0 fexh      (1000) fexh      (1000)        6 2023-05-14 12:34:12.000000 aw-cli-1.5.1/aw_cli.egg-info/top_level.txt
+drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-05-14 12:34:12.579430 aw-cli-1.5.1/awcli/
+-rw-r--r--   0 fexh      (1000) fexh      (1000)        0 2023-05-14 12:33:54.000000 aw-cli-1.5.1/awcli/__init__.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)    24766 2023-05-14 12:33:54.000000 aw-cli-1.5.1/awcli/run.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)    12080 2023-05-14 12:33:54.000000 aw-cli-1.5.1/awcli/utilities.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)       38 2023-05-14 12:34:12.579430 aw-cli-1.5.1/setup.cfg
+-rw-r--r--   0 fexh      (1000) fexh      (1000)      920 2023-05-14 12:33:54.000000 aw-cli-1.5.1/setup.py
+drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-05-14 12:34:12.579430 aw-cli-1.5.1/tests/
+-rw-r--r--   0 fexh      (1000) fexh      (1000)      473 2023-05-14 12:33:54.000000 aw-cli-1.5.1/tests/test_run.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     2880 2023-05-14 12:33:54.000000 aw-cli-1.5.1/tests/test_utilities.py
```

### Comparing `aw-cli-1.5/LICENSE` & `aw-cli-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aw-cli-1.5/PKG-INFO` & `aw-cli-1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: aw-cli
-Version: 1.5
+Version: 1.5.1
 Summary: guarda anime dal terminale e molto altro!
 Home-page: https://github.com/fexh10/aw-cli
 Author: fexh10
 License: GPL-3.0
 Requires-Python: >3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aw-cli
 <h3 align="center">
+
 Guarda anime dal terminale e molto altro!<br /> Gli anime vengono presi da <a href="https://www.animeworld.tv/">AnimeWorld</a>
 
 </h3>
 
 ## Anteprima
 https://user-images.githubusercontent.com/90156014/210212814-e73ba7af-ce12-43ad-95ff-dcd85b39a45c.mp4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aw-cli Version: 1.5 Summary: guarda anime dal
+Metadata-Version: 2.1 Name: aw-cli Version: 1.5.1 Summary: guarda anime dal
 terminale e molto altro! Home-page: https://github.com/fexh10/aw-cli Author:
 fexh10 License: GPL-3.0 Requires-Python: >3.10 Description-Content-Type: text/
 markdown License-File: LICENSE # aw-cli
                 **** Guarda anime dal terminale e molto altro!
                   Gli anime vengono presi da AnimeWorld ****
 ## Anteprima https://user-images.githubusercontent.com/90156014/210212814-
 e73ba7af-ce12-43ad-95ff-dcd85b39a45c.mp4 ## Indice - [Installazione]
```

### Comparing `aw-cli-1.5/README.md` & `aw-cli-1.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # aw-cli
 <h3 align="center">
+
 Guarda anime dal terminale e molto altro!<br /> Gli anime vengono presi da <a href="https://www.animeworld.tv/">AnimeWorld</a>
 
 </h3>
 
 ## Anteprima
 https://user-images.githubusercontent.com/90156014/210212814-e73ba7af-ce12-43ad-95ff-dcd85b39a45c.mp4
```

### Comparing `aw-cli-1.5/aw_cli.egg-info/PKG-INFO` & `aw-cli-1.5.1/aw_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: aw-cli
-Version: 1.5
+Version: 1.5.1
 Summary: guarda anime dal terminale e molto altro!
 Home-page: https://github.com/fexh10/aw-cli
 Author: fexh10
 License: GPL-3.0
 Requires-Python: >3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aw-cli
 <h3 align="center">
+
 Guarda anime dal terminale e molto altro!<br /> Gli anime vengono presi da <a href="https://www.animeworld.tv/">AnimeWorld</a>
 
 </h3>
 
 ## Anteprima
 https://user-images.githubusercontent.com/90156014/210212814-e73ba7af-ce12-43ad-95ff-dcd85b39a45c.mp4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aw-cli Version: 1.5 Summary: guarda anime dal
+Metadata-Version: 2.1 Name: aw-cli Version: 1.5.1 Summary: guarda anime dal
 terminale e molto altro! Home-page: https://github.com/fexh10/aw-cli Author:
 fexh10 License: GPL-3.0 Requires-Python: >3.10 Description-Content-Type: text/
 markdown License-File: LICENSE # aw-cli
                 **** Guarda anime dal terminale e molto altro!
                   Gli anime vengono presi da AnimeWorld ****
 ## Anteprima https://user-images.githubusercontent.com/90156014/210212814-
 e73ba7af-ce12-43ad-95ff-dcd85b39a45c.mp4 ## Indice - [Installazione]
```

### Comparing `aw-cli-1.5/awcli/run.py` & `aw-cli-1.5.1/awcli/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,16 +131,15 @@
         path (str): il percorso dove salvare l'episodio.
     """
 
     url_ep = anime.get_episodio(ep)
     nome_video = anime.ep_name(ep)
     
     # se l'episodio non è ancora stato scaricato lo scarico, altrimenti skippo
-    my_print(nome_video, color="blu", end="")
-    my_print(":\n" if nome_os == "Android" else ": ", end="")
+    my_print(nome_video, color="blu", end=":\n")
     if not os.path.exists(f"{path}/{nome_video}.mp4"):
         SDL = SmartDL(url_ep, f"{path}/{nome_video}.mp4")
         SDL.start()
     else:
         my_print("già scaricato, skippo...", color="giallo")
 
 
@@ -194,27 +193,29 @@
     """
 
     if syncpl:
         open_Syncplay(url_server, nome_video)
     elif (nome_os == "Android"):
         # apro il player utilizzando bash e riproduco un video
         os.system(f'''am start --user 0 -a android.intent.action.VIEW -d "{url_server}" -n is.xyz.mpv/.MPVActivity > /dev/null 2>&1 &''')
-    else:
+    elif nome_os == "Windows":
         import mpv
         
         player = mpv.MPV(input_default_bindings=True,input_vo_keyboard=True, osc=True)
 
         # avvio il player
         player.fullscreen = True
         player.playlist_pos = 0
         player["keep-open"] = True
         player["media-title"] = nome_video
         player.play(url_server)
         player.wait_for_shutdown()
         player.terminate()
+    elif nome_os == "Linux":
+        os.system(f'''mpv "{url_server}" --force-media-title="{nome_video}" --fullscreen --keep-open &>/dev/null''')
 
 
 def openVLC(url_server: str, nome_video: str):
     """
     Apre VLC per riprodurre il video.
 
     Args:
@@ -345,15 +346,15 @@
         openMPV(url_server, nome_video) if mpv else openVLC(url_server, nome_video)
 
         #se non sono in modalità offline aggiungo l'anime alla cronologia
         if not offline:
             addToCronologia(ep)
 
         #update watchlist anilist se ho fatto l'accesso
-        if tokenAnilist != 'tokenAnilist: False':
+        if tokenAnilist != 'tokenAnilist: False' and not offline:
             updateAnilist(tokenAnilist, ratingAnilist, preferitoAnilist, ep)
 
 
 def getCronologia() -> tuple[list, list]:
     """
     Prende i dati dalla cronologia.
```

### Comparing `aw-cli-1.5/awcli/utilities.py` & `aw-cli-1.5.1/awcli/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,16 +246,20 @@
     dl = bs.find_all(class_='meta col-sm-6')
     for a in dl[1].find_all("a"):
         if "filter?status=0"in a.get('href'):
             status = 0
             break
     #cerco l'id di anilist
     id_anilist = 0
-    if tokenAnilist != 'tokenAnilist: False':
-        id_anilist = bs.find(class_='anilist control tip tippy-desktop-only').get('href').replace("https://anilist.co/anime/", "")
+    try:
+        if tokenAnilist != 'tokenAnilist: False':
+            id_anilist = bs.find(class_='anilist control tip tippy-desktop-only').get('href').replace("https://anilist.co/anime/", "")
+    except AttributeError:
+        pass
+
     return url_episodi, status, id_anilist
 
 def printAnimeInfo(dt: list, dd: list, trama: str) -> str:
     """
     Stampa a schermo le informazioni
     e la trama relative all'anime selezioanto.
     Chiede all'utente se guardare l'anime oppure tornare indietro.
```

### Comparing `aw-cli-1.5/setup.py` & `aw-cli-1.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 installRequires = [
         "bs4",
         "requests",
-        "python-mpv",
         "lxml",
         "pySmartDL",
         "hpcomt",
         "wheel",
         "regex",]
 if os.name == 'nt':
     installRequires.append("psutil")
     installRequires.append("pywinauto")
+    installRequires.append("python-mpv")
 
 setup(
     name="aw-cli",
     packages=find_packages(include=["awcli"]),
-    version="1.5",
+    version="1.5.1",
     python_requires=">3.10",
     description="guarda anime dal terminale e molto altro!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="fexh10",
     url="https://github.com/fexh10/aw-cli",
     license="GPL-3.0",
```

### Comparing `aw-cli-1.5/tests/test_utilities.py` & `aw-cli-1.5.1/tests/test_utilities.py`

 * *Files identical despite different names*

