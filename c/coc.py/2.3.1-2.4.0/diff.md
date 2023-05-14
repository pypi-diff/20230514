# Comparing `tmp/coc.py-2.3.1.tar.gz` & `tmp/coc.py-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coc.py-2.3.1.tar", last modified: Fri Feb  3 00:28:44 2023, max compression
+gzip compressed data, was "coc.py-2.4.0.tar", last modified: Sun May 14 19:12:13 2023, max compression
```

## Comparing `coc.py-2.3.1.tar` & `coc.py-2.4.0.tar`

### file list

```diff
@@ -1,57 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:28:44.485720 coc.py-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-03 00:28:30.000000 coc.py-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-03 00:28:30.000000 coc.py-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-02-03 00:28:44.485720 coc.py-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-02-03 00:28:30.000000 coc.py-2.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:28:44.477720 coc.py-2.3.1/coc/
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/clans.py
--rw-r--r--   0 runner    (1001) docker     (123)    70748 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/entry_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    39764 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/events.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:28:44.473720 coc.py-2.3.1/coc/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:28:44.481720 coc.py-2.3.1/coc/ext/discordlinks/
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/ext/discordlinks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:28:44.481720 coc.py-2.3.1/coc/ext/fullwarapi/
--rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/ext/fullwarapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/hero.py
--rw-r--r--   0 runner    (1001) docker     (123)    20985 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/login.py
--rw-r--r--   0 runner    (1001) docker     (123)    21152 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/miscmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/player_clan.py
--rw-r--r--   0 runner    (1001) docker     (123)    26138 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/players.py
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/raid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/spell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:28:44.485720 coc.py-2.3.1/coc/static/
--rw-r--r--   0 runner    (1001) docker     (123)   135500 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/static/buildings.json
--rw-r--r--   0 runner    (1001) docker     (123)   271286 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/static/characters.json
--rw-r--r--   0 runner    (1001) docker     (123)   130902 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/static/heroes.json
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/static/object_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)    43766 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/static/pets.json
--rw-r--r--   0 runner    (1001) docker     (123)    53705 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/static/spells.json
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/static/supers.json
--rw-r--r--   0 runner    (1001) docker     (123)   575079 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/static/texts_EN.json
--rw-r--r--   0 runner    (1001) docker     (123)    41725 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/static/townhall_levels.json
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/static/update_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/troop.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/war_attack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/war_clans.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/war_members.py
--rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-02-03 00:28:30.000000 coc.py-2.3.1/coc/wars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 00:28:44.481720 coc.py-2.3.1/coc.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-02-03 00:28:44.000000 coc.py-2.3.1/coc.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-03 00:28:44.000000 coc.py-2.3.1/coc.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 00:28:44.000000 coc.py-2.3.1/coc.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-03 00:28:44.000000 coc.py-2.3.1/coc.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-03 00:28:44.000000 coc.py-2.3.1/coc.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-02-03 00:28:30.000000 coc.py-2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-03 00:28:30.000000 coc.py-2.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 00:28:44.485720 coc.py-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-03 00:28:30.000000 coc.py-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.286276 coc.py-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-14 19:11:58.000000 coc.py-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-14 19:11:58.000000 coc.py-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-14 19:12:13.286276 coc.py-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-14 19:11:58.000000 coc.py-2.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.282276 coc.py-2.4.0/coc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/clans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80631 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/entry_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39759 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/events.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.278276 coc.py-2.4.0/coc/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.282276 coc.py-2.4.0/coc/ext/discordlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/ext/discordlinks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.282276 coc.py-2.4.0/coc/ext/fullwarapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/ext/fullwarapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.282276 coc.py-2.4.0/coc/ext/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/ext/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/ext/triggers/cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/ext/triggers/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/hero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22005 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21796 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/miscmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/player_clan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26903 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/players.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/raid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/spell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.286276 coc.py-2.4.0/coc/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   135500 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/buildings.json
+-rw-r--r--   0 runner    (1001) docker     (123)   271286 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/characters.json
+-rw-r--r--   0 runner    (1001) docker     (123)   130902 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/heroes.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/object_ids.json
+-rw-r--r--   0 runner    (1001) docker     (123)    43766 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/pets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53705 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/spells.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/supers.json
+-rw-r--r--   0 runner    (1001) docker     (123)   575079 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/texts_EN.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41725 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/townhall_levels.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/update_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/troop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/war_attack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/war_clans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/war_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/wars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.282276 coc.py-2.4.0/coc.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-14 19:12:13.000000 coc.py-2.4.0/coc.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-14 19:12:13.000000 coc.py-2.4.0/coc.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 19:12:13.000000 coc.py-2.4.0/coc.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-14 19:12:13.000000 coc.py-2.4.0/coc.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-14 19:12:13.000000 coc.py-2.4.0/coc.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-14 19:11:58.000000 coc.py-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-14 19:11:58.000000 coc.py-2.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 19:12:13.286276 coc.py-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-14 19:11:58.000000 coc.py-2.4.0/setup.py
```

### Comparing `coc.py-2.3.1/LICENSE` & `coc.py-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/PKG-INFO` & `coc.py-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 2.3.1
+Version: 2.4.0
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
-Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, doluk
+Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
 Keywords: coc,clash of clans,coc.py,clash api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -74,23 +74,23 @@
     async def main():
         async with coc.Client() as coc_client:
             try:
                 await coc_client.login("email", "password")
             except coc.invalidcredentials as error:
                 exit(error)
 
-            player = await client.get_player("tag")
+            player = await coc_client.get_player("tag")
             print(f"{player.name} has {player.trophies} trophies!")
 
-            clans = await client.search_clans(name="best clan ever", limit=5)
+            clans = await coc_client.search_clans(name="best clan ever", limit=5)
             for clan in clans:
                 print(f"{clan.name} ({clan.tag}) has {clan.member_count} members")
 
             try:
-                war = await client.get_current_war("#clantag")
+                war = await coc_client.get_current_war("#clantag")
                 print(f"{war.clan_tag} is currently in {war.state} state.")
             except coc.privatewarlog:
                 print("uh oh, they have a private war log!")
 
     if __name__ == "__main__":
         try:
             asyncio.run(main())
```

### Comparing `coc.py-2.3.1/README.rst` & `coc.py-2.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,23 @@
     async def main():
         async with coc.Client() as coc_client:
             try:
                 await coc_client.login("email", "password")
             except coc.invalidcredentials as error:
                 exit(error)
 
-            player = await client.get_player("tag")
+            player = await coc_client.get_player("tag")
             print(f"{player.name} has {player.trophies} trophies!")
 
-            clans = await client.search_clans(name="best clan ever", limit=5)
+            clans = await coc_client.search_clans(name="best clan ever", limit=5)
             for clan in clans:
                 print(f"{clan.name} ({clan.tag}) has {clan.member_count} members")
 
             try:
-                war = await client.get_current_war("#clantag")
+                war = await coc_client.get_current_war("#clantag")
                 print(f"{war.clan_tag} is currently in {war.state} state.")
             except coc.privatewarlog:
                 print("uh oh, they have a private war log!")
 
     if __name__ == "__main__":
         try:
             asyncio.run(main())
```

### Comparing `coc.py-2.3.1/coc/__init__.py` & `coc.py-2.4.0/coc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,22 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = "2.3.1"
+__version__ = "2.4.0"
 
 from .abc import BasePlayer, BaseClan
 from .clans import RankedClan, Clan
 from .client import Client
 from .events import PlayerEvents, ClanEvents, WarEvents, EventsClient, ClientEvents
 from .enums import (
+    PlayerHouseElementType,
     Resource,
     Role,
     WarRound,
     ACHIEVEMENT_ORDER,
     BUILDER_TROOPS_ORDER,
     HERO_ORDER,
     PETS_ORDER,
@@ -69,14 +70,15 @@
     CapitalDistrict,
     Icon,
     GoldPassSeason,
     League,
     LegendStatistics,
     LoadGameData,
     Location,
+    PlayerHouseElement,
     Timestamp,
     TimeDelta,
     Label,
     WarLeague,
 )
 from .players import Player, ClanMember, RankedPlayer
 from .player_clan import PlayerClan
```

### Comparing `coc.py-2.3.1/coc/abc.py` & `coc.py-2.4.0/coc/abc.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/clans.py` & `coc.py-2.4.0/coc/clans.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/client.py` & `coc.py-2.4.0/coc/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     )
 
     def __init__(
         self,
         *,
         key_count: int = 1,
         key_names: str = "Created with coc.py Client",
-        throttle_limit: int = 10,
+        throttle_limit: int = 30,
         loop: asyncio.AbstractEventLoop = None,
         correct_tags: bool = True,
         throttler: Type[Union[BasicThrottler, BatchThrottler]] = BasicThrottler,
         connector=None,
         timeout: float = 30.0,
         cache_max_size: int = 10000,
         stats_max_size: int = 1000,
@@ -219,15 +219,14 @@
 
         # cache
         self._players = {}
         self._clans = {}
         self._wars = {}
 
     async def __aenter__(self):
-        self.__init__()
         return self
 
     async def __aexit__(self, *args):
         await self.close()
 
     def _create_client(self, email, password):
         return HTTPClient(
@@ -308,35 +307,35 @@
         Parameters
         ----------
         keys: list[str]
             Keys or tokens as found from https://developer.clashofclans.com.
 
 
         """
+        self.correct_key_count = len(keys)
         self.http = http = self._create_client(None, None)
         http._keys = keys
         http.keys = cycle(http._keys)
-        http.key_count = len(keys)
         self.loop.run_until_complete(http.create_session(self.connector, self.timeout))
         self._create_holders()
 
         LOG.debug("HTTP connection created. Client is ready for use.")
 
     async def login_with_tokens(self, *tokens: str) -> None:
         """Creates an HTTP connection ready for use with the tokens you provide.
 
         Parameters
         ----------
         tokens: list[str]
             Tokens as found from https://developer.clashofclans.com under "My account" -> <your key> -> "token".
         """
+        self.correct_key_count = len(tokens)
         self.http = http = self._create_client(None, None)
         http._keys = tokens
         http.keys = cycle(http._keys)
-        http.key_count = len(tokens)
         await http.create_session(self.connector, self.timeout)
         self._create_holders()
 
         LOG.debug("HTTP connection created. Client is ready for use.")
 
     async def close(self) -> None:
         """Closes the HTTP connection from within a loop function such as
@@ -363,14 +362,15 @@
         name: str = None,
         war_frequency: str = None,
         location_id: int = None,
         min_members: int = None,
         max_members: int = None,
         min_clan_points: int = None,
         min_clan_level: int = None,
+        label_ids: List[Union[Label, int]] = [],
         limit: int = None,
         before: str = None,
         after: str = None,
         cls: Type[Clan] = Clan,
         **kwargs,
     ) -> List[Clan]:
         """Search all clans by name and/or filtering the results using various criteria.
@@ -390,16 +390,20 @@
             The minimum number of members.
         max_members : int, optional
             The maximum number of members.
         min_clan_points : int, optional
             The minumum clan points.
         min_clan_level : int, optional
             The minimum clan level.
+        label_ids: :class:`List`[Union[:class:`coc.Label`, :class:`int`]]
+            List of Labels or Label ids
         limit : int
             The number of clans to search for.
+        cls:
+            Target class to use to model that data returned
 
         Raises
         -------
         RuntimeError
             At least one filtering parameter must be passed.
         TypeError
             The ``cls`` parameter must be a subclass of :class:`Clan`.
@@ -425,14 +429,16 @@
             name=name,
             warFrequency=war_frequency,
             locationId=location_id,
             minMembers=min_members,
             maxMembers=max_members,
             minClanPoints=min_clan_points,
             minClanLevel=min_clan_level,
+            label_ids=",".join([str(x.id) if isinstance(x, Label) else str(x) for x in label_ids
+                                if isinstance(x, (Label, int,))]),
             limit=limit,
             before=before,
             after=after,
         )
 
         return [cls(data=n, client=self, **kwargs) for n in data.get("items", [])]
 
@@ -442,14 +448,17 @@
         Clan tags can be found using clan search operation.
 
         Parameters
         -----------
         tag : str
             The clan tag to search for.
 
+        cls:
+            Target class to use to model that data returned
+
         Raises
         -------
         TypeError
             The ``cls`` parameter must be a subclass of :class:`Clan`.
 
         NotFound
             No clan was found with the supplied tag.
@@ -491,14 +500,17 @@
                 print(clan.name)
 
         Parameters
         -----------
         tags : Iterable[:class:`str`]
             An iterable of clan tags to search for.
 
+        cls:
+            Target class to use to model that data returned
+
         Raises
         ------
         TypeError
             The ``cls`` parameter must be a subclass of :class:`Clan`.
 
 
         Yields
@@ -507,23 +519,35 @@
             A clan matching one of the tags requested.
         """
         if not issubclass(cls, Clan):
             raise TypeError("cls must be a subclass of Clan.")
 
         return ClanIterator(self, tags, cls, **kwargs)
 
-    async def get_members(self, clan_tag: str, cls: Type[ClanMember] = ClanMember, **kwargs) -> List[ClanMember]:
+    async def get_members(self, clan_tag: str, *, limit: int = 0, after: str = "", before: str = "",
+                          cls: Type[ClanMember] = ClanMember, **kwargs) -> List[ClanMember]:
         """List clan members.
 
         This is equivilant to ``(await Client.get_clan('tag')).members``.
 
         Parameters
         -----------
         clan_tag : str
             The clan tag to search for.
+        cls:
+            Target class to use to model that data returned
+        limit:
+            class:`int`: Number of members to retrieve
+
+        after:
+            class:`str`: Pagination string to get page after
+
+        before:
+            class:`str`: Pagination string to get page before
+
 
         Raises
         -------
         TypeError
             The ``cls`` parameter must be a subclass of :class:`ClanMember`.
 
         NotFound
@@ -543,23 +567,34 @@
         """
         if not issubclass(cls, ClanMember):
             raise TypeError("cls must be a subclass of ClanMember.")
 
         if self.correct_tags:
             clan_tag = correct_tag(clan_tag)
 
-        data = await self.http.get_clan(clan_tag)
+        args = {}
+        if limit:
+            args['limit'] = limit
+        if after:
+            args['after'] = after
+        if before:
+            args['before'] = before
+
+        data = await self.http.get_clan_members(clan_tag, **args)
         return [cls(data=mdata, client=self, **kwargs) for mdata in data.get("memberList", [])]
 
     async def get_warlog(
         self,
         clan_tag: str,
         cls: Type[ClanWarLogEntry] = ClanWarLogEntry,
         page: bool = False,
-        limit: int = 0
+        *,
+        limit: int = 0,
+        after: str = "",
+        before: str = ""
     ) -> ClanWarLog:
         """
         Retrieve a clan's clan war log. By default, this will return
         all the clan's log available in the API. This will of course consume
         memory. The option of limiting the amount of log items fetched
         can be controlled with the `limit` parameter. Additionally, if
         `paginate` is set to True, and an async for loop is performed
@@ -572,29 +607,35 @@
             Please see documentation for :class:`ClanWarLogEntry` for different attributes
             which are present when the entry is a regular clan war or a league clan war.
             The difference can be found with :attr:`ClanWarLogEntry.is_league_entry`.
 
 
         Parameters
         -----------
-        cls:
-            Target class to use to model that data returned
-
         clan_tag:
             class:`str`: The clan tag to search for.
 
+        cls:
+            Target class to use to model that data returned
+
         page:
             class:`bool`: Enable fetching logs while only holding the
             same amount of logs as `limit`. If `paginate` is set to True,
             and `limit` is set to default of 0, then `limit` will be set to
             10 automatically.
 
         limit:
             class:`int`: Number of logs to retrieve
 
+        after:
+            class:`str`: Pagination string to get page after
+
+        before:
+            class:`str`: Pagination string to get page before
+
         Raises
         ------
         TypeError
             The ``cls`` parameter must be a subclass of :class:`ClanWarLogEntry`.
 
         NotFound
             No clan was found with the supplied tag.
@@ -629,53 +670,64 @@
             limit = limit if limit else 10
 
         try:
             return await ClanWarLog.init_cls(client=self,
                                              clan_tag=clan_tag,
                                              page=page,
                                              limit=limit,
-                                             model=cls)
+                                             model=cls,
+                                             after=after,
+                                             before=before)
         except Forbidden as exception:
             raise PrivateWarLog(exception.response,
                                 exception.reason) from exception
 
     async def get_raidlog(
             self,
             clan_tag: str,
             cls: Type[RaidLogEntry] = RaidLogEntry,
             page: bool = False,
-            limit: int = 0
+            *,
+            limit: int = 0,
+            after: str = "",
+            before: str = ""
     ) -> RaidLog:
         """
         Retrieve a clan's Capital Raid Log. By default, this will return
         all the clan's log available in the API. This will of course consume
         memory. The option of limiting the amount of log items fetched
         can be controlled with the `limit` parameter. Additionally, if
         `paginate` is set to True, and an async for loop is performed
         on this object, then additional log items will be fetched but only
         consume the same amount of memory space at all time.
 
 
         Parameters
         -----------
-        cls:
-            Target class to use to model that data returned
-
         clan_tag:
             class:`str`: The clan tag to search for.
 
+        cls:
+            Target class to use to model that data returned
+
         page:
             class:`bool`: Enable fetching logs while only holding the
             same amount of logs as `limit`. If `paginate` is set to True,
             and `limit` is set to default of 0, then `limit` will be set to
             10 automatically.
 
         limit:
             class:`int`: Number of logs to retrieve
 
+        after:
+            class:`str`: Pagination string to get page after
+
+        before:
+            class:`str`: Pagination string to get page before
+
         Raises
         ------
         TypeError
             The ``cls`` parameter must be a subclass of :class:`RaidLogEntry`.
 
         NotFound
             No clan was found with the supplied tag.
@@ -711,15 +763,17 @@
             limit = limit if limit else 10
 
         try:
             return await RaidLog.init_cls(client=self,
                                           clan_tag=clan_tag,
                                           page=page,
                                           limit=limit,
-                                          model=cls)
+                                          model=cls,
+                                          after=after,
+                                          before=before)
         except Forbidden as exception:
             raise PrivateWarLog(exception.response,
                                 exception.reason) from exception
 
     async def get_clan_war(self, clan_tag: str, cls: Type[ClanWar] = ClanWar, **kwargs) -> ClanWar:
         """
         Retrieve information about clan's current clan war
@@ -734,15 +788,15 @@
         TypeError
             The ``cls`` parameter must be a subclass of :class:`ClanWar`.
 
         NotFound
             No clan was found with the supplied tag.
 
         PrivateWarLog
-            The clan's warlog is private.
+            The clan's war log is private.
 
         Maintenance
             The API is currently in maintenance.
 
         GatewayError
             The API hit an unexpected gateway exception.
 
@@ -797,14 +851,17 @@
                 print(clan_war.opponent)
 
         Parameters
         -----------
         clan_tags : Iterable[:class:`str`]
             An iterable of clan tags to search for.
 
+        cls:
+            Target class to use to model that data returned
+
         Raises
         ------
         TypeError
             The ``cls`` parameter must be a subclass of :class:`ClanWar`.
 
         NotFound
             No clan was found with the supplied tag.
@@ -838,14 +895,17 @@
         """Retrieve information about clan's current clan war league group.
 
         Parameters
         -----------
         clan_tag : str
             The clan tag to search for.
 
+        cls:
+            Target class to use to model that data returned
+
         Raises
         ------
         TypeError
             The ``cls`` parameter must be a subclass of :class:`ClanWarLeagueGroup`.
 
         NotFound
             No clan was found with the supplied tag.
@@ -893,14 +953,17 @@
         Retrieve information about a clan war league war.
 
         Parameters
         -----------
         war_tag : str
             The league war tag to search for.
 
+        cls:
+            Target class to use to model that data returned
+
         Raises
         ------
         TypeError
             The ``cls`` parameter must be a subclass of :class:`ClanWar`.
 
         NotFound
             No clan was found with the supplied tag.
@@ -911,15 +974,15 @@
         GatewayError
             The API hit an unexpected gateway exception.
 
 
         Returns
         --------
         :class:`ClanWar`
-            The league war assosiated with the war tag
+            The league war associated with the war tag
         """
         # pylint: disable=protected-access
         if not issubclass(cls, ClanWar):
             raise TypeError("cls must be a subclass of LeagueWar.")
 
         if self.correct_tags:
             war_tag = correct_tag(war_tag)
@@ -960,14 +1023,16 @@
 
         Parameters
         -----------
         war_tags : Iterable[:class:`str`]
             An iterable of war tags to search for.
         clan_tag: :class:`str`
             An optional clan tag. If present, this will only return wars which belong to this clan.
+        cls:
+            Target class to use to model that data returned
 
         Raises
         ------
         TypeError
             The ``cls`` parameter must be a subclass of :class:`ClanWar`.
 
         Yields
@@ -1011,14 +1076,17 @@
             An iterable of clan tag to search for.
 
         cwl_round: :class:`WarRound`
             An enum detailing the type of round to get. Could be ``coc.WarRound.previous_war``,
             ``coc.WarRound.current_war`` or ``coc.WarRound.preparation``.
             This defaults to ``coc.WarRound.current_war``.
 
+        cls:
+            Target class to use to model that data returned
+
         Raises
         -------
         TypeError
             The ``cls`` parameter must be a subclass of :class:`ClanWar`.
 
         NotFound
             No clan was found with the supplied tag.
@@ -1062,26 +1130,39 @@
         except (NotFound, GatewayError) as exception:
             # either they're not in cwl (NotFound)
             # or it's an API bug where league group endpoint will timeout when the clan is searching (GatewayError)
             if get_war is None:
                 raise PrivateWarLog(exception.response, exception.reason) from exception
             return get_war
 
-        is_prep = league_group.state == "preparation"
-
+        if league_group.state == "notInWar" or league_group.state == "groupNotFound":
+            return None
+        last_round_active = league_group.number_of_rounds == len(league_group.rounds)
+        if last_round_active and league_group.state != "ended":
+            # there are the supposed number of rounds, but without any call we are unable to know if the last round is
+            # currently in preparation or already in war
+            async for war in self.get_league_wars(league_group.rounds[-1], cls=cls, **kwargs):
+                if war.state == 'inWar':
+                    # last round is already in war
+                    last_round_active = True
+                    break
+                elif war.state == 'preparation':
+                    # last round is still in preparation
+                    last_round_active = False
+                    break
         if cwl_round is WarRound.current_war and league_group.state == "preparation":
             return None  # for round 1 and 15min prep between rounds this is a shortcut.
         elif cwl_round is WarRound.current_preparation and league_group.state == "ended":
             return None  # for the end of CWL there's no next prep day.
-        elif cwl_round is WarRound.previous_war and len(league_group.rounds) == 1:
-            return None  # no previous war for first rounds.
-        elif cwl_round is WarRound.current_war and league_group.state == "ended":
-            round_tags = league_group.rounds[-1] # for the end of CWL current_war should give the last war
-        elif cwl_round is WarRound.previous_war and is_prep:
-            round_tags = league_group.rounds[-2]
+        elif cwl_round is WarRound.current_war and (last_round_active or league_group.state == "ended"):
+            round_tags = league_group.rounds[-1]  # for the end of CWL current_war should give the last war
+        elif cwl_round is WarRound.previous_war and (last_round_active or league_group.state == "ended"):
+            round_tags = league_group.rounds[-2]  # for the end of CWL previous_war should give the second last war
+        elif cwl_round is WarRound.previous_war and len(league_group.rounds) < 3:
+            return None  # no previous war for two rounds.
         elif cwl_round is WarRound.previous_war:
             round_tags = league_group.rounds[-3]
         elif cwl_round is WarRound.current_war:
             round_tags = league_group.rounds[-2]
         elif cwl_round is WarRound.current_preparation:
             round_tags = league_group.rounds[-1]
         else:
@@ -1131,28 +1212,31 @@
                 print(war.type)
 
         Parameters
         -----------
         clan_tags : Iterable[:class:`str`]
             An iterable of clan tags to search for.
 
+        cls:
+            Target class to use to model that data returned
+
         Raises
         ------
         TypeError
             The ``cls`` parameter must be a subclass of :class:`ClanWar`.
 
         Yields
         --------
         :class:`ClanWar`
             The clan war of a requested tag.
         """
         if not isinstance(clan_tags, Iterable):
             raise TypeError("Tags are not an iterable.")
         if not issubclass(cls, ClanWar):
-            raise TypeError("cls must be a subclass of either ClanWar.")
+            raise TypeError("cls must be a subclass of ClanWar.")
 
         return CurrentWarIterator(client=self, tags=clan_tags, cls=cls, **kwargs)
 
     # locations
     async def search_locations(self, *, limit: int = None, before: str = None, after: str = None) -> List[Location]:
         """List all available locations
 
@@ -1234,179 +1318,217 @@
         """
         data = await self.http.search_locations(limit=None, before=None, after=None)
         locations = [Location(data=n) for n in data["items"]]
 
         return get(locations, name=location_name)
 
     async def get_location_clans(
-        self, location_id: int = "global", *, limit: int = None, before: str = None, after: str = None
+        self, location_id: int = "global", *, limit: int = None,
+            before: str = None, after: str = None, cls: Type[RankedClan] = RankedClan
     ) -> List[RankedClan]:
         """Get clan rankings for a specific location
 
         Parameters
         -----------
         location_id : int
             The Location ID to search for. Defaults to all locations (``global``).
         limit : int
             The number of results to fetch.
         before : str, optional
             For use with paging. Not implemented yet.
         after: str, optional
             For use with paging. Not implemented yet.
+        cls:
+            Target class to use to model that data returned
 
         Raises
         ------
+        TypeError
+            The ``cls`` parameter must be a subclass of :class:`RankedClan`.
+
         Maintenance
             The API is currently in maintenance.
 
         GatewayError
             The API hit an unexpected gateway exception.
 
 
         Returns
         --------
         List[:class:`RankedClan`]
             The top clans for the requested location.
         """
-
+        if not issubclass(cls, RankedClan):
+            raise TypeError("cls must be a subclass of RankedClan.")
         data = await self.http.get_location_clans(location_id, limit=limit, before=before, after=after)
-        return [RankedClan(data=n, client=self) for n in data["items"]]
+        return [cls(data=n, client=self) for n in data["items"]]
 
     async def get_location_clans_capital(
-        self, location_id: int = "global", *, limit: int = None, before: str = None, after: str = None
+        self, location_id: int = "global", *, limit: int = None,
+            before: str = None, after: str = None, cls: Type[RankedClan] = RankedClan
     ) -> List[RankedClan]:
         """Get clan capital rankings for a specific location
 
         Parameters
         -----------
         location_id : int
             The Location ID to search for. Defaults to all locations (``global``).
         limit : int
             The number of results to fetch.
         before : str, optional
             For use with paging. Not implemented yet.
         after: str, optional
             For use with paging. Not implemented yet.
+        cls:
+            Target class to use to model that data returned
 
         Raises
         ------
+        TypeError
+            The ``cls`` parameter must be a subclass of :class:`RankedClan`.
+
         Maintenance
             The API is currently in maintenance.
 
         GatewayError
             The API hit an unexpected gateway exception.
 
 
         Returns
         --------
         List[:class:`RankedClan`]
             The top clans for the requested location.
         """
-
+        if not issubclass(cls, RankedClan):
+            raise TypeError("cls must be a subclass of RankedClan.")
         data = await self.http.get_location_clans_capital(location_id, limit=limit, before=before, after=after)
-        return [RankedClan(data=n, client=self) for n in data["items"]]
+        return [cls(data=n, client=self) for n in data["items"]]
 
     async def get_location_players(
-        self, location_id: int = "global", *, limit: int = None, before: str = None, after: str = None
+        self, location_id: int = "global", *, limit: int = None,
+            before: str = None, after: str = None, cls: Type[RankedPlayer] = RankedPlayer
     ) -> List[RankedPlayer]:
         """Get player rankings for a specific location
 
         Parameters
         -----------
         location_id : int
             The Location ID to search for. Defaults to all locations (global).
         limit : int
             The number of results to fetch.
         before : str, optional
             For use with paging. Not implemented yet.
         after: str, optional
             For use with paging. Not implemented yet.
+        cls:
+            Target class to use to model that data returned
 
         Raises
         ------
+        TypeError
+            The ``cls`` parameter must be a subclass of :class:`RankedPlayer`.
+
         Maintenance
             The API is currently in maintenance.
 
         GatewayError
             The API hit an unexpected gateway exception.
 
 
         Returns
         --------
         List[:class:`RankedPlayer`]
             The top players for the requested location.
         """
+        if not issubclass(cls, RankedPlayer):
+            raise TypeError("cls must be a subclass of RankedPlayer.")
         data = await self.http.get_location_players(location_id, limit=limit, before=before, after=after)
-        return [RankedPlayer(data=n, client=self) for n in data["items"]]
+        return [cls(data=n, client=self) for n in data["items"]]
 
     async def get_location_clans_versus(
-        self, location_id: int = "global", *, limit: int = None, before: str = None, after: str = None
+        self, location_id: int = "global", *, limit: int = None,
+            before: str = None, after: str = None, cls: Type[RankedClan] = RankedClan
     ) -> List[RankedClan]:
         """Get clan versus rankings for a specific location
 
         Parameters
         -----------
         location_id : int
             The Location ID to search for. Defaults to all locations (global).
         limit : int
             The number of results to fetch.
         before : str, optional
             For use with paging. Not implemented yet.
         after: str, optional
             For use with paging. Not implemented yet.
+        cls:
+            Target class to use to model that data returned
 
         Raises
         ------
+        TypeError
+            The ``cls`` parameter must be a subclass of :class:`RankedClan`.
+
         Maintenance
             The API is currently in maintenance.
 
         GatewayError
             The API hit an unexpected gateway exception.
 
 
         Returns
         --------
         List[:class:`RankedClan`]
             The top versus-clans for the requested location.
         """
+        if not issubclass(cls, RankedClan):
+            raise TypeError("cls must be a subclass of RankedClan.")
         data = await self.http.get_location_clans_versus(location_id, limit=limit, before=before, after=after)
-        return [RankedClan(data=n, client=self) for n in data["items"]]
+        return [cls(data=n, client=self) for n in data["items"]]
 
     async def get_location_players_versus(
-        self, location_id: int = "global", *, limit: int = None, before: str = None, after: str = None
+        self, location_id: int = "global", *, limit: int = None,
+            before: str = None, after: str = None, cls: Type[RankedPlayer] = RankedPlayer
     ) -> List[RankedPlayer]:
         """Get player versus rankings for a specific location
 
         Parameters
         -----------
         location_id : int
             The Location ID to search for. Defaults to all locations (global).
         limit : int
             The number of results to fetch.
         before : str, optional
             For use with paging. Not implemented yet.
         after: str, optional
             For use with paging. Not implemented yet.
+        cls:
+            Target class to use to model that data returned
 
         Raises
         ------
+        TypeError
+            The ``cls`` parameter must be a subclass of :class:`RankedPlayer`.
+
         Maintenance
             The API is currently in maintenance.
 
         GatewayError
             The API hit an unexpected gateway exception.
 
 
         Returns
         --------
         List[:class:`RankedPlayer`]
             The top versus players for the requested location.
         """
+        if not issubclass(cls, RankedPlayer):
+            raise TypeError("cls must be a subclass of RankedPlayer.")
         data = await self.http.get_location_players_versus(location_id, limit=limit, before=before, after=after)
-        return [RankedPlayer(data=n, client=self) for n in data["items"]]
+        return [cls(data=n, client=self) for n in data["items"]]
 
     # leagues
 
     async def search_leagues(self, *, limit: int = None, before: str = None, after: str = None) -> List[League]:
         """Get list of leagues.
 
         Parameters
@@ -1462,17 +1584,17 @@
         :class:`League`
             The league with the requested ID
         """
         data = await self.http.get_league(league_id)
         return League(data=data, client=self)
 
     async def get_league_named(self, league_name: str) -> Optional[League]:
-        """Get a location by name.
+        """Get a league by name.
 
-        This is somewhat equivilant to
+        This is somewhat equivalent to
 
         .. code-block:: python3
 
             leagues = await client.search_leagues(limit=None)
             return utils.get(leagues, name=league_name)
 
 
@@ -1488,18 +1610,198 @@
 
         GatewayError
             The API hit an unexpected gateway exception.
 
         Returns
         --------
         :class:`League`
-            The first location matching the location name. Could be ``None`` if not found.
+            The first league matching the league name. Could be ``None`` if not found.
         """
         return get(await self.search_leagues(), name=league_name)
 
+    async def search_war_leagues(self, *, limit: int = None, before: str = None, after: str = None) -> List[League]:
+        """Get list of war leagues.
+
+        Parameters
+        -----------
+        limit : int
+            Number of items to fetch. Defaults to ``None`` (all leagues).
+        before : str, optional
+            For use with paging. Not implemented yet.
+        after: str, optional
+            For use with paging. Not implemented yet.
+
+
+        Raises
+        ------
+        Maintenance
+            The API is currently in maintenance.
+
+        GatewayError
+            The API hit an unexpected gateway exception.
+
+
+        Returns
+        --------
+        List[:class:`League`]
+            The requested leagues.
+        """
+        data = await self.http.search_war_leagues(limit=limit, before=before, after=after)
+        return [League(data=n, client=self) for n in data["items"]]
+
+    async def get_war_league(self, league_id: int) -> League:
+        """
+        Get war league information
+
+        Parameters
+        -----------
+        league_id : str
+            The League ID to search for.
+
+        Raises
+        ------
+        Maintenance
+            The API is currently in maintenance.
+
+        GatewayError
+            The API hit an unexpected gateway exception.
+
+        NotFound
+            No league was found with the supplied league ID.
+
+
+        Returns
+        --------
+        :class:`League`
+            The league with the requested ID
+        """
+        data = await self.http.get_war_league(league_id)
+        return League(data=data, client=self)
+
+    async def get_war_league_named(self, league_name: str) -> Optional[League]:
+        """Get a war league by name.
+
+        This is somewhat equivalent to
+
+        .. code-block:: python3
+
+            leagues = await client.search_war_leagues(limit=None)
+            return utils.get(leagues, name=league_name)
+
+
+        Parameters
+        -----------
+        league_name : str
+            The war league name to search for
+
+        Raises
+        ------
+        Maintenance
+            The API is currently in maintenance.
+
+        GatewayError
+            The API hit an unexpected gateway exception.
+
+        Returns
+        --------
+        :class:`League`
+            The first league matching the league name. Could be ``None`` if not found.
+        """
+        return get(await self.search_war_leagues(), name=league_name)
+
+    async def search_capital_leagues(self, *, limit: int = None, before: str = None, after: str = None) -> List[League]:
+        """Get list of capital leagues.
+
+        Parameters
+        -----------
+        limit : int
+            Number of items to fetch. Defaults to ``None`` (all leagues).
+        before : str, optional
+            For use with paging. Not implemented yet.
+        after: str, optional
+            For use with paging. Not implemented yet.
+
+
+        Raises
+        ------
+        Maintenance
+            The API is currently in maintenance.
+
+        GatewayError
+            The API hit an unexpected gateway exception.
+
+
+        Returns
+        --------
+        List[:class:`League`]
+            The requested leagues.
+        """
+        data = await self.http.search_capital_leagues(limit=limit, before=before, after=after)
+        return [League(data=n, client=self) for n in data["items"]]
+
+    async def get_capital_league(self, league_id: int) -> League:
+        """
+        Get capital league information
+
+        Parameters
+        -----------
+        league_id : str
+            The League ID to search for.
+
+        Raises
+        ------
+        Maintenance
+            The API is currently in maintenance.
+
+        GatewayError
+            The API hit an unexpected gateway exception.
+
+        NotFound
+            No league was found with the supplied league ID.
+
+
+        Returns
+        --------
+        :class:`League`
+            The league with the requested ID
+        """
+        data = await self.http.get_capital_league(league_id)
+        return League(data=data, client=self)
+
+    async def get_capital_league_named(self, league_name: str) -> Optional[League]:
+        """Get a capital league by name.
+
+        This is somewhat equivalent to
+
+        .. code-block:: python3
+
+            leagues = await client.search_capital_leagues(limit=None)
+            return utils.get(leagues, name=league_name)
+
+
+        Parameters
+        -----------
+        league_name : str
+            The capital league name to search for
+
+        Raises
+        ------
+        Maintenance
+            The API is currently in maintenance.
+
+        GatewayError
+            The API hit an unexpected gateway exception.
+
+        Returns
+        --------
+        :class:`League`
+            The first league matching the league name. Could be ``None`` if not found.
+        """
+        return get(await self.search_capital_leagues(), name=league_name)
+
     async def get_seasons(self, league_id: int = 29000021) -> List[str]:
         """Get league seasons.
 
         .. note::
 
             League season information is available only for Legend League, with a league ID 29000021.
 
@@ -1619,23 +1921,27 @@
             A list of all possible player labels.
         """
         data = await self.http.get_player_labels(limit=limit, before=before, after=after)
         return [Label(data=n, client=self) for n in data["items"]]
 
     # players
 
-    async def get_player(self, player_tag: str, cls: Type[Player] = Player, load_game_data: bool = None, **kwargs) -> Player:
+    async def get_player(self, player_tag: str, cls: Type[Player] = Player,
+                         load_game_data: bool = None, **kwargs) -> Player:
         """Get information about a single player by player tag.
         Player tags can be found either in game or by from clan member lists.
 
         Parameters
         ----------
         player_tag : str
             The player tag to search for.
 
+        cls:
+            Target class to use to model that data returned
+
         Raises
         -------
         TypeError
             The ``cls`` parameter must be a subclass of :class:`Player`.
 
         NotFound
             No player was found with the supplied tag.
@@ -1679,14 +1985,17 @@
                 print(player)
 
         Parameters
         ----------
         player_tags : Iterable[:class:`str`]
             An iterable of player tags to search for.
 
+        cls:
+            Target class to use to model that data returned
+
         Raises
         ------
         TypeError
             The ``cls`` parameter must be a subclass of :class:`Player`.
 
         Yields
         ------
```

### Comparing `coc.py-2.3.1/coc/entry_logs.py` & `coc.py-2.4.0/coc/entry_logs.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,24 +40,24 @@
         return self
 
     def __next__(self) -> Union[ClanWarLogEntry, RaidLogEntry]:
         """Fetch the next item in the iter object and return the entry"""
         if self._sync_index == len(self._init_logs):
             raise StopIteration
         ret = self._model(data=self._init_logs[self._sync_index],
-                          client=self._client, response_retry=self._response_retry)
+                          client=self._client, response_retry=self._response_retry, clan_tag=self._clan_tag)
         self._sync_index += 1
         return ret
 
     def __getitem__(self, index: int) -> Union[ClanWarLogEntry, RaidLogEntry]:
         """Support indexing the object. This will not fetch any addition
         items from the endpoint"""
         try:
-            ret = self._init_logs[index]
-            return self._model(data=ret, client=self._client, response_retry=self._response_retry)
+            return self._model(data=self._init_logs[index],
+                               client=self._client, response_retry=self._response_retry, clan_tag=self._clan_tag)
         except Exception:
             raise
 
     def __aiter__(self):
         # These values are used to simulate the caller having a single list
         # of items. In reality, the list is populated on demand.
         self._max_index = len(self._init_logs)
@@ -88,15 +88,15 @@
         """
         # If paging is not enabled, do not fetch  any more items only
         # iterate over the items in the self._war_logs
         if not self._page:
             if self._async_index == len(self._logs):
                 raise StopAsyncIteration
             ret = self._model(data=self._logs[self._async_index],
-                              client=self._client, response_retry=self._response_retry)
+                              client=self._client, response_retry=self._response_retry, clan_tag=self._clan_tag)
             self._async_index += 1
             return ret
 
         # If paging is enabled, update self._war_logs if the end of the
         # array is reached
         ret: Union[ClanWarLogEntry, RaidLogEntry]
 
@@ -111,15 +111,15 @@
             self._min_index = self._max_index
             self._max_index = self._max_index + len(self._logs)
             ret = self._logs[self._async_index - self._min_index]
         else:
             raise StopAsyncIteration
 
         self._async_index += 1
-        return self._model(data=ret, client=self._client, response_retry=self._response_retry)
+        return self._model(data=ret, client=self._client, response_retry=self._response_retry, clan_tag=self._clan_tag)
 
     async def _paginate(self) -> None:
         """
         Request data from the endpoint and update the iter variables with
         the new data. `self._fetch_endpoint` is a child defined method.
         """
         self._page_data = await self._fetch_endpoint(self._client,
@@ -175,18 +175,24 @@
     @classmethod
     async def init_cls(cls,
                        client: Client,
                        clan_tag: str,
                        model: Type[ClanWarLogEntry],
                        limit: int,
                        page: bool = True,
+                       after: str = None,
+                       before: str = None
                        ) -> ClanWarLog:
 
         # Add the limit if specified
         args = {"limit": limit} if limit else {}
+        if after:
+            args["after"] = after
+        if before:
+            args["before"] = before
 
         json_resp = await cls._fetch_endpoint(client, clan_tag, **args)
         return ClanWarLog(client=client, clan_tag=clan_tag, limit=limit,
                           page=page, json_resp=json_resp, model=model)
 
     @staticmethod
     async def _fetch_endpoint(client: Client, clan_tag: str,
@@ -206,18 +212,24 @@
     @classmethod
     async def init_cls(cls,
                        client: Client,
                        clan_tag: str,
                        model: Type[RaidLogEntry],
                        limit: int,
                        page: bool = True,
+                       after: str = None,
+                       before: str = None
                        ) -> RaidLog:
 
         # Add the limit if specified
         args = {"limit": limit} if limit else {}
+        if after:
+            args["after"] = after
+        if before:
+            args["before"] = before
 
         json_resp = await cls._fetch_endpoint(client, clan_tag, **args)
         return RaidLog(client=client, clan_tag=clan_tag, limit=limit,
                        page=page, json_resp=json_resp, model=model)
 
     @staticmethod
     async def _fetch_endpoint(client: Client, clan_tag: str,
```

### Comparing `coc.py-2.3.1/coc/enums.py` & `coc.py-2.4.0/coc/enums.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,35 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from enum import Enum
 
 
+class PlayerHouseElementType(Enum):
+    """Enum to map the type of element of the player house."""
+
+    ground = "ground"
+    roof = "roof"
+    foot = "foot"  # API docs say this exists, but unable to find it anywhere. Looks like this means `walls`
+    deco = "decoration"
+    walls = "walls"
+
+    def __str__(self):
+        return self.in_game_name
+
+    @property
+    def in_game_name(self) -> str:
+        """Get a neat client-facing string value for the element type."""
+        lookup = {PlayerHouseElementType.ground: "Ground", PlayerHouseElementType.roof: "Roof",
+                  PlayerHouseElementType.foot: "Foot", PlayerHouseElementType.deco: "Decoration",
+                  PlayerHouseElementType.walls: "Walls"}
+        return lookup[self]
+
+
 class Role(Enum):
     """Enum to map a player's role in the clan."""
 
     member = "member"
     elder = "admin"
     co_leader = "coLeader"
     leader = "leader"
```

### Comparing `coc.py-2.3.1/coc/errors.py` & `coc.py-2.4.0/coc/errors.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/events.py` & `coc.py-2.4.0/coc/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
 
     @classmethod
     def new_war(cls, tags=None, custom_class=None, retry_interval=None):
         """Alias for the preparation start time changes, which is equal to a new war started"""
 
         async def wrapped(cached_war: ClanWar, war: ClanWar, callback):
             if cached_war.preparation_start_time and war.preparation_start_time \
-                    and cached_war.preparation_start_time.timestamp != war.preparation_start_time.time:
+                    and cached_war.preparation_start_time.time != war.preparation_start_time.time:
                 await callback(war)
             elif war.preparation_start_time and not cached_war.preparation_start_time:
                 # no war on endpoint, so new war is for sure new
                 await callback(war)
         return _ValidateEvent.shortcut_register(wrapped, tags, custom_class, retry_interval, WarEvents.event_type)
```

### Comparing `coc.py-2.3.1/coc/events.pyi` & `coc.py-2.4.0/coc/events.pyi`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/ext/discordlinks/__init__.py` & `coc.py-2.4.0/coc/ext/discordlinks/__init__.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/ext/fullwarapi/__init__.py` & `coc.py-2.4.0/coc/ext/fullwarapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,19 +164,19 @@
         Optional[:class:`ClanWar`]
             War result, or ``None`` if no war found.
         """
         data = await self._request("GET",
                                    f"/war_result?clan_tag={correct_tag(clan_tag, '%23')}"
                                    f"&prep_start={str(preparation_start)}")
         try:
-            return ClanWar(data=data["response"], client=self.coc_client)
+            return ClanWar(data=data["response"], client=self.coc_client, clan_tag=coc.utils.correct_tag(clan_tag))
         except (IndexError, KeyError, TypeError, ValueError):
             return None
 
-    async def war_result_log(self, clan_tag: str) -> Optional[Generator[ClanWar]]:
+    async def war_result_log(self, clan_tag: str) -> Optional[Generator[ClanWar, None, None]]:
         """Get all stored war results for a clan.
 
         Parameters
         ----------
         clan_tag: str
             The clan tag to find war result for.
 
@@ -185,17 +185,16 @@
         Optional[Generator[:class:`ClanWar`]]
             Generator of war results, or ``None`` if no wars found.
         """
         data = await self._request("GET",
                                    f"/war_result_log?clan_tag={correct_tag(clan_tag, '%23')}")
         try:
             responses = data["log"]
-
-            generator = (ClanWar(data=response["response"], client=self.coc_client) for response in responses)
-            return generator
+            return (ClanWar(data=response["response"], client=self.coc_client,
+                            clan_tag=coc.utils.correct_tag(clan_tag)) for response in responses)
         except (IndexError, KeyError, TypeError, ValueError):
             return None
 
     async def register_war(self, clan_tag: str, preparation_start: int = 0):
         """Registers a war.
 
         Parameters
```

### Comparing `coc.py-2.3.1/coc/hero.py` & `coc.py-2.4.0/coc/hero.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,21 +71,21 @@
     upgrade_resource: "Resource"
     upgrade_time: "TimeDelta"
     ability_time: int
     required_th_level: int
     regeneration_time: "TimeDelta"
     is_loaded: bool = False
 
-    def __repr__(cls):
+    def __repr__(self):
         attrs = [
-            ("name", cls.name),
-            ("id", cls.id),
+            ("name", self.name),
+            ("id", self.id),
         ]
         return "<%s %s>" % (
-            cls.__name__, " ".join("%s=%r" % t for t in attrs),)
+            self.__class__.__name__, " ".join("%s=%r" % t for t in attrs),)
 
     @property
     def is_max_for_townhall(self) -> bool:
         """:class:`bool`: Returns whether the hero is the max level for the player's townhall level."""
         if self.is_max:
             return True
 
@@ -167,21 +167,21 @@
     speed: int
     upgrade_cost: int
     upgrade_resource: "Resource"
     upgrade_time: "TimeDelta"
     is_loaded: bool = False
     required_th_level: int
 
-    def __repr__(cls):
+    def __repr__(self):
         attrs = [
-            ("name", cls.name),
-            ("id", cls.id),
+            ("name", self.name),
+            ("id", self.id),
         ]
         return "<%s %s>" % (
-            cls.__name__, " ".join("%s=%r" % t for t in attrs),)
+            self.__class__.__name__, " ".join("%s=%r" % t for t in attrs),)
 
     @property
     def is_max_for_townhall(self) -> bool:
         """:class:`bool`: Returns whether the hero pet is the max level for the player's townhall level."""
         if self.is_max:
             return True
```

### Comparing `coc.py-2.3.1/coc/http.py` & `coc.py-2.4.0/coc/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         "lock",
     )
 
     def __init__(self, sleep_time):
         self.sleep_time = sleep_time
         self.last_run = None
         self.lock = asyncio.Lock()
+        LOG.debug("BasicThrottler initialized with sleeptime %s", self.sleep_time)
 
     async def __aenter__(self):
         async with self.lock:
             last_run = self.last_run
             if last_run:
                 difference = process_time() - last_run
                 need_to_sleep = self.sleep_time - difference
@@ -104,14 +105,16 @@
 
     def __init__(self, rate_limit, per=1.0, retry_interval=0.001):
         self.rate_limit = rate_limit
         self.per = per
         self.retry_interval = retry_interval
 
         self._task_logs = deque()
+        LOG.debug("BatchThrottler initialized with rate_limit %s, per %s, retry_interval %s", self.rate_limit, self.per,
+                  self. retry_interval)
 
     async def __aenter__(self):
         while True:
             now = process_time()
 
             # Pop items(which are start times) that are no longer in the
             # time window
@@ -277,17 +280,19 @@
                             self.stats[route.stats_key] = perf
 
                         LOG.debug("API HTTP Request: %s", str(log_info))
                         data = await json_or_text(response)
 
                         try:
                             # set a callback to remove the item from cache once it's stale.
-                            delta = int(response.headers["Cache-Control"].strip("max-age="))
-                            data["_response_retry"] = delta
-                            if isinstance(cache, FIFO) and not self.client.realtime:
+                            delta = int(response.headers["Cache-Control"].strip("max-age=").strip("public max-age="))
+                            # encounter for changed description in cache control header. for realtime it is always
+                            # 600 but that is not true. Correct is 0
+                            data["_response_retry"] = delta if 'realtime' not in url else 0
+                            if isinstance(cache, FIFO) and 'realtime' not in url:
                                 self.cache[cache_control_key] = data
                                 LOG.debug("Cache-Control max age: %s seconds, key: %s", delta, cache_control_key)
                                 self.loop.call_later(delta, self._cache_remove, cache_control_key)
 
                         except (KeyError, AttributeError, ValueError):
                             # the request didn't contain cache control headers so skip any cache handling.
                             # if the API returns a timeout error (504) it will return a string of HTML.
@@ -410,17 +415,29 @@
         return self.request(Route("GET", "/locations/{}/rankings/players-versus".format(location_id), **kwargs))
 
     # leagues
 
     def search_leagues(self, **kwargs):
         return self.request(Route("GET", "/leagues", **kwargs))
 
+    def search_capital_leagues(self, **kwargs):
+        return self.request(Route("GET", "/capitalleagues", **kwargs))
+
+    def search_war_leagues(self, **kwargs):
+        return self.request(Route("GET", "/warleagues", **kwargs))
+
     def get_league(self, league_id):
         return self.request(Route("GET", "/leagues/{}".format(league_id)))
 
+    def get_capital_league(self, league_id):
+        return self.request(Route("GET", "/capitalleagues/{}".format(league_id)))
+
+    def get_war_league(self, league_id):
+        return self.request(Route("GET", "/warleagues/{}".format(league_id)))
+
     def get_league_seasons(self, league_id, **kwargs):
         return self.request(Route("GET", "/leagues/{}/seasons".format(league_id), **kwargs))
 
     def get_league_season_info(self, league_id, season_id, **kwargs):
         return self.request(Route("GET", "/leagues/{}/seasons/{}".format(league_id, season_id), **kwargs))
 
     # players
@@ -455,27 +472,28 @@
             if resp.status == 403:
                 LOG.error("Invalid credentials used when attempting to log in")
                 await self.close()
                 raise InvalidCredentials()
 
             LOG.info("Successfully logged into the developer site.")
 
-            resp_paylaod = await resp.json()
-            ip = json_loads(base64_b64decode(resp_paylaod["temporaryAPIToken"].split(".")[1] + "====").decode("utf-8"))["limits"][1]["cidrs"][0].split("/")[0]
+            resp_payload = await resp.json()
+            ip = json_loads(base64_b64decode(resp_payload["temporaryAPIToken"].split(".")[1] + "====").decode("utf-8"))["limits"][1]["cidrs"][0].split("/")[0]
 
             LOG.info("Found IP address to be %s", ip)
 
             resp = await session.post("https://developer.clashofclans.com/api/apikey/list")
             keys = (await resp.json())["keys"]
-            self._keys.extend(key["key"] for key in keys if key["name"] == self.key_names and ip in key["cidrRanges"])
+            self._keys.extend(key["key"] for c, key in enumerate(keys) if key["name"] == self.key_names and ip in key[
+                "cidrRanges"] and c <= self.key_count)
 
             LOG.info("Retrieved %s valid keys from the developer site.", len(self._keys))
 
             if len(self._keys) < self.key_count:
-                for key in keys:
+                for key in keys[:]:
                     if key["name"] != self.key_names or ip in key["cidrRanges"]:
                         continue
                     LOG.info(
                             "Deleting key with the name %s and IP %s (not matching our current IP address).",
                             self.key_names, key["cidrRanges"],
                     )
                     resp = await session.post("https://developer.clashofclans.com/api/apikey/revoke", json={"id": key["id"]})
```

### Comparing `coc.py-2.3.1/coc/iterators.py` & `coc.py-2.4.0/coc/iterators.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/login.py` & `coc.py-2.4.0/coc/login.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/miscmodels.py` & `coc.py-2.4.0/coc/miscmodels.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from datetime import datetime
 from typing import Any, Type, TypeVar, Optional
-
+from .enums import PlayerHouseElementType
 from .utils import from_timestamp
 
 T = TypeVar("T")
 
 
 def try_enum(_class: Type[T], data: Any, **kwargs) -> Optional[T]:
     """Helper function to create a class from the given data."""
@@ -689,7 +689,28 @@
         self.duration = self.end_time.time - self.start_time.time
 
     def __eq__(self, other):
         return (isinstance(other, GoldPassSeason)
                 and self.start_time == other.start_time
                 and self.end_time == other.end_time)
 
+
+class PlayerHouseElement:
+    """Represents an element of a player house.
+
+    Attributes
+    ----------
+    id:
+        :class:`int`: The id of the house element
+    type:
+        :class:`PlayerHouseElementType`: The type of the house element
+    """
+    __slots__ = ("id", "type")
+
+    def __init__(self, *, data):
+        self.id = data.get("id")
+        self.type = data.get("type") and PlayerHouseElementType(value=data["type"])
+
+    def __eq__(self, other):
+        return (isinstance(other, PlayerHouseElement)
+                and self.id == other.id
+                and self.type == other.type)
```

### Comparing `coc.py-2.3.1/coc/player_clan.py` & `coc.py-2.4.0/coc/player_clan.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/players.py` & `coc.py-2.4.0/coc/players.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from typing import Optional, List, TYPE_CHECKING
 
 
-from .miscmodels import try_enum, Achievement, Label, League, LegendStatistics
+from .miscmodels import PlayerHouseElement, try_enum, Achievement, Label, League, LegendStatistics
 from .enums import (
     Role,
     HERO_ORDER,
     BUILDER_TROOPS_ORDER,
     HOME_TROOP_ORDER,
     SPELL_ORDER,
     SIEGE_MACHINE_ORDER,
@@ -232,37 +232,41 @@
         "builder_hall",
         "best_versus_trophies",
         "versus_attack_wins",
         "clan_capital_contributions",
         "legend_statistics",
         "war_opted_in",
         "_achievements",
+        "_player_house_elements",
         "_heroes",
         "_pets",
         "_labels",
         "_spells",
         "_home_troops",
         "_builder_troops",
         "_super_troops",
         "achievement_cls",
+        "player_house_element_cls",
         "hero_cls",
         "label_cls",
         "spell_cls",
         "troop_cls",
         "pet_cls",
 
         "_iter_achievements",
+        "_iter_player_house_elements",
         "_iter_heroes",
         "_iter_labels",
         "_iter_spells",
         "_iter_troops",
         "_iter_pets",
 
         "_cs_labels",
         "_cs_achievements",
+        "_cs_player_house_elements",
         "_cs_troops",
         "_cs_home_troops",
         "_cs_builder_troops",
         "_cs_siege_machines",
         "_cs_pets",
         "_cs_super_troops",
         "_cs_heroes",
@@ -281,14 +285,15 @@
         self._spells = None  # type: Optional[dict]
         self._home_troops: dict = {}
         self._builder_troops: dict = {}
         self._super_troops: list = []
         self._pets = None # type: Optional[dict]
 
         self.achievement_cls = Achievement
+        self.player_house_element_cls = PlayerHouseElement
         self.hero_cls = Hero
         self.label_cls = Label
         self.spell_cls = Spell
         self.troop_cls = Troop
         self.pet_cls = Pet
 
         if self._client and self._client._troop_holder.loaded:
@@ -325,26 +330,29 @@
             self.war_opted_in: Optional[bool] = True if data["warPreference"] == "in" else False
         except KeyError:
             # not in a clan / war preference not there
             self.war_opted_in: Optional[bool] = None
 
         label_cls = self.label_cls
         achievement_cls = self.achievement_cls
+        player_house_element_cls = self.player_house_element_cls
         troop_loader = self._client._troop_holder.load if self._client else None
         hero_loader =  self._client._hero_holder.load if self._client else None
         spell_loader = self._client._spell_holder.load if self._client else None
         pet_loader = self._client._pet_holder.load if self._client else None
 
         if self._game_files_loaded:
             pet_lookup = [p.name for p in self._client._pet_holder.items]
         else:
             pet_lookup = PETS_ORDER
 
         self._iter_labels = (label_cls(data=ldata, client=self._client) for ldata in data_get("labels", []))
         self._iter_achievements = (achievement_cls(data=adata) for adata in data_get("achievements", []))
+        self._iter_player_house_elements = (player_house_element_cls(data=adata)
+                                            for adata in data_get("playerHouse", {}).get("elements", []))
         self._iter_troops = (
             troop_loader(
                 data=tdata,
                 townhall=self.town_hall,
                 default=self.troop_cls,
                 load_game_data=self._load_game_data,
             ) for tdata in data_get("troops", []) if tdata["name"] not in pet_lookup
@@ -417,14 +425,19 @@
                         item._load_from_parent(holder.get(item.name))
 
     @cached_property("_cs_labels")
     def labels(self) -> List[Label]:
         """List[:class:`Label`]: A :class:`List` of :class:`Label`s that the player has."""
         return list(self._iter_labels)
 
+    @cached_property("_cs_player_house_elements")
+    def player_house_elements(self) -> List[PlayerHouseElement]:
+        """List[:class:`PlayerHouseElement`]: A :class:`List` of :class:`PlayerHouseElement`s that the player has."""
+        return list(self._iter_player_house_elements)
+
     @cached_property("_cs_achievements")
     def achievements(self) -> List[Achievement]:
         """List[:class:`Achievement`]: A list of the player's achievements."""
         # at the time of writing, the API presents achievements in the order
         # added to the game which doesn't match in-game order.
         achievement_dict = {a.name: a for a in self._iter_achievements}
         sorted_achievements = {}
```

### Comparing `coc.py-2.3.1/coc/raid.py` & `coc.py-2.4.0/coc/raid.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,67 +57,54 @@
     __slots__ = ("tag",
                  "name",
                  "attack_count",
                  "attack_limit",
                  "bonus_attack_limit",
                  "capital_resources_looted",
                  "raid_log_entry",
-                 "_attacks",
+                 "_cs_attacks",
                  "_client")
 
     def __init__(self, *, data, client, raid_log_entry):
         super().__init__(data=data, client=client)
         self._client = client
         self.raid_log_entry = raid_log_entry
-        self._attacks = []
         self._from_data(data)
 
     def __repr__(self):
         attrs = [
             ("tag", self.tag),
             ("raid_log_entry", repr(self.raid_log_entry)),
             ("attack_count", self.attack_count)
         ]
         return "<%s %s>" % (self.__class__.__name__, " ".join("%s=%r" % t for t in attrs),)
 
     def __eq__(self, other):
-        if isinstance(other, RaidMember):
-            if (self.tag == other.tag
-                    and self.attack_count == other.attack_count
-                    and self.attack_limit == other.attack_limit
-                    and self.bonus_attack_limit == other.bonus_attack_limit
-                    and self.capital_resources_looted == other.capital_resources_looted
-            ):
-                return True
-        return False
+        return (isinstance(other, RaidMember)
+                and self.tag == other.tag
+                and self.raid_log_entry == other.raid_log_entry)
 
     def _from_data(self, data):
         data_get = data.get
 
         self.name: str = data_get("name")
         self.tag: str = data_get("tag")
         self.attack_count: int = data_get("attacks")
         self.attack_limit: int = data_get("attackLimit")
         self.bonus_attack_limit: int = data_get("bonusAttackLimit")
         self.capital_resources_looted: int = data_get("capitalResourcesLooted")
 
-    @property
+    @cached_property("_cs_attacks")
     def attacks(self):
         """List[:class:`RaidAttack`]: The member's attacks in this raid log entry.
         Can be empty due to missing parts in the API response.
         """
-        list_attacks = self._attacks  # type: List[RaidAttack]
-        if list_attacks:
-            return list_attacks
-
-        list_attacks = list(attack for attack_raid in self.raid_log_entry.attack_log
-                            for district in attack_raid.districts for attack in district.attacks
-                            if attack and attack.attacker_tag == self.tag)
-        self._attacks = list_attacks
-        return list_attacks
+        return list(attack for attack_raid in self.raid_log_entry.attack_log
+                    for district in attack_raid.districts for attack in district.attacks
+                    if attack and attack.attacker_tag == self.tag)
 
 
 class RaidAttack:
     """Represents a Raid attack
 
     Attributes
     ----------
@@ -157,36 +144,34 @@
             ("attacker_tag", self.attacker_tag),
             ("destruction", self.destruction),
             ("stars", self.stars),
         ]
         return "<%s %s>" % (self.__class__.__name__, " ".join("%s=%r" % t for t in attrs),)
 
     def __eq__(self, other):
-        if isinstance(other, RaidAttack):
-            if (self.attacker_tag == other.attacker_tag
+        return (isinstance(other, RaidAttack)
+                and self.attacker_tag == other.attacker_tag
                 and self.destruction == other.destruction
-                and self.stars == other.stars
                 and self.raid_clan == other.raid_clan
                 and self.district == other.district
-            ):
-                return True
-        return False
+                and self.stars == other.stars)
 
     def __init__(self, data, client, raid_log_entry, raid_clan, district):
         self.raid_log_entry = raid_log_entry
         self.raid_clan = raid_clan
         self.district = district
         self._client = client
         self._raw_data = data if client and client.raw_attribute else None
         self._from_data(data)
 
     def _from_data(self, data: dict) -> None:
         self.attacker_tag = data["attacker"]["tag"]
         self.attacker_name = data["attacker"]["name"]
         self.destruction = data["destructionPercent"]
+        self.stars = data["stars"]
 
     @property
     def attacker(self) -> "RaidMember":
         """:class:`RaidMember`: Returns the attacking player."""
         return self.raid_log_entry.get_member(self.attacker_tag)
 
 
@@ -212,25 +197,17 @@
     raid_log_entry:
         :class:`RaidLogEntry` - The raid log entry this district belongs to
     raid_clan:
         :class:`RaidClan` - The raid clan this district belongs to
     """
 
     def __eq__(self, other):
-        if isinstance(other, RaidDistrict):
-            if (self.id == other.id
-                and self.name == other.name
-                and self.hall_level == other.hall_level
-                and self.destruction == other.destruction
-                and self.looted == other.looted
-                and self.raid_clan == other.raid_clan
-                and self.attack_count == other.attack_count
-            ):
-                return True
-        return False
+        return (isinstance(other, RaidDistrict)
+                and self.id == other.id
+                and self.raid_clan == other.raid_clan)
 
     __slots__ = ("id",
                  "name",
                  "hall_level",
                  "destruction",
                  "attack_count",
                  "looted",
@@ -247,15 +224,14 @@
         attrs = [("id", self.id),
                  ("raid_log_entry", repr(self.raid_log_entry)),
                  ("raid_clan", repr(self.raid_clan)),
                  ("hall_level", self.hall_level),
                  ("destruction", self.destruction)]
         return "<%s %s>" % (self.__class__.__name__, " ".join("%s=%r" % t for t in attrs),)
 
-
     def __init__(self, *, data, client, raid_log_entry, raid_clan):
         self.id: int = data.get("id")
         self.name: str = data.get("name")
         self.hall_level: int = data.get("districtHallLevel")
         self.destruction: float = data.get("destructionPercent")
         self.attack_count: int = data.get("attackCount")
         self.looted: int = data.get("totalLooted")
@@ -308,14 +284,15 @@
         "destroyed_district_count",
         "raid_log_entry",
         "_districts",
         "_attacks",
         "_client",
         "_response_retry",
         "_cs_raid_districts",
+        "_cs_looted",
         "_iter_raid_districts",
         "_raw_data"
     )
 
     def __init__(self, *, data, client, raid_log_entry, index=0, **_):
         self._client = client
         self._raw_data = data if client and client.raw_attribute else None
@@ -323,23 +300,19 @@
         self.tag = data.get("attacker", data.get("defender")).get("tag")
         self.name = data.get("attacker", data.get("defender")).get("name")
         self.badge = try_enum(Badge, data=data.get("attacker", data.get("defender")).get("badgeUrls"),
                               client=self._client)
         self.level = data.get("attacker", data.get("defender")).get("level")
         self.raid_log_entry = raid_log_entry
         self.index = index
-        self._attacks = []
         self._from_data(data)
 
     def __eq__(self, other):
         return (isinstance(other, RaidClan)
                 and self.tag == other.tag
-                and self.attack_count == other.attack_count
-                and self.district_count == other.district_count
-                and self.destroyed_district_count == other.destroyed_district_count
                 and self.raid_log_entry.start_time == other.raid_log_entry.start_time
                 and self.index == other.index)
 
     def __repr__(self):
         attrs = [
             ("tag", self.tag),
             ("name", self.name),
@@ -363,24 +336,30 @@
 
     @cached_property("_cs_raid_districts")
     def districts(self) -> typing.List[RaidDistrict]:
         """List[:class:`RaidDistrict`]: A :class:`List` of :class:`RaidDistrict` that the clan
         attacked."""
         return list(self._iter_raid_districts)
 
-    @property
+    @cached_property("_cs_raid_attacks")
     def attacks(self) -> typing.List[RaidAttack]:
         """List[:class:`RaidAttack`]: Returns all attacks in the raid against this clan."""
-        list_attacks = self._attacks  # type: List[RaidAttack]
-        if list_attacks:
-            return list_attacks
-
-        list_attacks = list(attack for district in self.districts for attack in district.attacks)
-        self._attacks = list_attacks
-        return list_attacks
+        return list(attack for district in self.districts for attack in district.attacks)
+
+    @cached_property("_cs_looted")
+    def looted(self) -> int:
+        """:class:`int`: The amount of loot the raid clan got on all districts."""
+        loot = 0
+        for district in self.districts:
+            loot += district.looted
+        return loot
+
+    @property
+    def is_finished(self) -> bool:
+        return self.destroyed_district_count == self.district_count
 
 
 class RaidLogEntry:
     """Represents a Clash of Clans Raid Log Entry
 
     Attributes
     ----------
@@ -400,39 +379,44 @@
         :class:`int`: The number of destroyed enemy districts
     offensive_reward:
         :class:`int`: The amount of offensive reward
     defensive_reward:
         :class:`int`: The amount of defensive reward
     """
 
-    __slots__ = ("state",
+    __slots__ = ("clan_tag",
+                 "state",
                  "start_time",
                  "end_time",
                  "total_loot",
                  "completed_raid_count",
                  "attack_count",
                  "destroyed_district_count",
                  "offensive_reward",
                  "defensive_reward",
                  "_raw_data",
                  "_cs_attack_log",
                  "_cs_defense_log",
                  "_cs_members",
+                 "_cs_total_defensive_loot",
+                 "_cs_defense_attack_count",
+                 "_cs_defensive_destroyed_district_count",
                  "_iter_members",
                  "_iter_attack_log",
                  "_iter_defense_log",
                  "_members",
                  "_attack_log",
                  "_defense_log",
                  "_client",
                  "_response_retry"
                  )
 
     def __init__(self, *, data, client, **kwargs):
         self._client = client
+        self.clan_tag = kwargs['clan_tag'] if "clan_tag" in kwargs else ""
         self._response_retry = kwargs['response_retry'] if "response_retry" in kwargs else 0
         self._raw_data = data if client and client.raw_attribute else None
         self._from_data(data)
         self._members = {}
         self._attack_log = []
         self._defense_log = []
 
@@ -440,26 +424,17 @@
         attrs = [
             ("state", self.state),
             ("start_time", self.start_time),
         ]
         return "<%s %s>" % (self.__class__.__name__, " ".join("%s=%r" % t for t in attrs),)
 
     def __eq__(self, other):
-        if isinstance(other, RaidLogEntry):
-            if (self.start_time == other.start_time
-                    and self.completed_raid_count == other.completed_raid_count
-                    and self.destroyed_district_count == other.destroyed_district_count
-                    and self.attack_count == other.attack_count
-                    and self.attack_log == other.attack_log
-                    and self.defense_log == other.defense_log
-            ):
-                return True
-
-        return False
-
+        return (isinstance(other, RaidLogEntry)
+                and self.start_time == other.start_time
+                and self.clan_tag == other.clan_tag)
 
     def _from_data(self, data: dict) -> None:
         data_get = data.get
 
         self.state: str = data_get("state")
         self.start_time = try_enum(Timestamp, data=data_get("startTime"))
         self.end_time = try_enum(Timestamp, data=data_get("endTime"))
@@ -496,22 +471,45 @@
     @cached_property("_cs_defense_log")
     def defense_log(self) -> typing.List[RaidClan]:
         """List[:class:`RaidClan`]: A list of raid clans which represents all the defensive raids of a season.
         """
         list_defense_log = self._defense_log = [m for m in self._iter_defense_log]
         return list_defense_log
 
+    @cached_property("_cs_total_defensive_loot")
+    def total_defensive_loot(self) -> int:
+        """:class:`int`: The total amount of loot taken by all opponents of the raid weekend."""
+        loot = 0
+        for clan in self.defense_log:
+            loot += clan.looted
+        return loot
+
+    @cached_property("_cs_defense_attack_count")
+    def defense_attack_count(self) -> int:
+        """:class:`int`: The total amount of opponent attacks in the raid weekend."""
+        count = 0
+        for clan in self.defense_log:
+            count += clan.attack_count
+        return count
+
+    @cached_property("_cs_defensive_destroyed_district_count")
+    def defensive_destroyed_district_count(self) -> int:
+        """:class:`int`: The total amount of districts destroyed by opponents."""
+        count = 0
+        for clan in self.defense_log:
+            count += clan.destroyed_district_count
+        return count
+
     def get_member(self, tag: str) -> typing.Optional[RaidMember]:
         """Get a member of the clan for the given tag, or ``None`` if not found.
 
         Returns
         --------
         The clan member who matches the tag.: Optional[:class:`RaidMember`]"""
         tag = correct_tag(tag)
         if not self._members:
             _ = self.members
 
         try:
             return self._members[tag]
         except KeyError:
             return None
-
```

### Comparing `coc.py-2.3.1/coc/spell.py` & `coc.py-2.4.0/coc/spell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Type, Dict, List
 from pathlib import Path
 
 from .abc import DataContainer, DataContainerHolder
 from .enums import Resource
 from .miscmodels import TimeDelta
 
-
 SPELLS_FILE_PATH = Path(__file__).parent.joinpath(Path("static/spells.json"))
 
 
 class Spell(DataContainer):
     """Represents a Spell object as returned by the API, optionally filled with game data.
 
     Attributes
@@ -63,21 +62,21 @@
     training_resource: "Resource"
     training_time: "TimeDelta"
 
     is_elixir_spell: bool = False
     is_dark_spell: bool = False
     is_loaded: bool = False
 
-    def __repr__(cls):
+    def __repr__(self):
         attrs = [
-            ("name", cls.name),
-            ("id", cls.id),
+            ("name", self.name),
+            ("id", self.id),
         ]
         return "<%s %s>" % (
-            cls.__name__, " ".join("%s=%r" % t for t in attrs),)
+            self.__class__.__name__, " ".join("%s=%r" % t for t in attrs),)
 
     @property
     def is_max_for_townhall(self):
         """:class:`bool`:
             Returns a boolean that indicates whether the spell is the max level for the player's townhall level.
         """
         if self.is_max:
@@ -86,15 +85,15 @@
         # 1. Hero/troop levels in-game are 1-indexed, UnitStat is 1-indexed
         # 2. TH-lab levels in-game and here are 1-indexed
         # 3. We then want to check that for the level less than this troop the req'd
         #    TH is less than or equal to current TH,
         #    and for troop level above, it requires a higher TH than we currently have.
         #    Maybe there's a better way to go about doing this.
         return self.lab_to_townhall[self.__class__.lab_level[self.level]] <= self._townhall \
-                    < self.lab_to_townhall[self.__class__.lab_level[self.level + 1]]
+             < self.lab_to_townhall[self.__class__.lab_level[self.level + 1]]
 
     @classmethod
     def get_max_level_for_townhall(cls, townhall):
         """Get the maximum level for a spell for a given townhall level.
 
         Parameters
         ----------
```

### Comparing `coc.py-2.3.1/coc/static/buildings.json` & `coc.py-2.4.0/coc/static/buildings.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/static/characters.json` & `coc.py-2.4.0/coc/static/characters.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/static/heroes.json` & `coc.py-2.4.0/coc/static/heroes.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/static/object_ids.json` & `coc.py-2.4.0/coc/static/object_ids.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/static/pets.json` & `coc.py-2.4.0/coc/static/pets.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/static/spells.json` & `coc.py-2.4.0/coc/static/spells.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/static/supers.json` & `coc.py-2.4.0/coc/static/supers.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/static/texts_EN.json` & `coc.py-2.4.0/coc/static/texts_EN.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/static/townhall_levels.json` & `coc.py-2.4.0/coc/static/townhall_levels.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/static/update_static.py` & `coc.py-2.4.0/coc/static/update_static.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/troop.py` & `coc.py-2.4.0/coc/troop.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import ujson
 
 from .abc import DataContainer, DataContainerHolder
 from .enums import Resource
 from .miscmodels import TimeDelta, try_enum
 from .utils import UnitStat
 
-
 TROOPS_FILE_PATH = Path(__file__).parent.joinpath(Path("static/characters.json"))
 SUPER_TROOPS_FILE_PATH = Path(__file__).parent.joinpath(Path("static/supers.json"))
 
 
 class Troop(DataContainer):
     """Represents a Troop object as returned by the API, optionally filled with game data.
 
@@ -98,22 +97,21 @@
 
     is_elixir_troop: bool = False
     is_dark_troop: bool = False
     is_siege_machine: bool = False
     is_super_troop: bool = False
     is_loaded: bool = False
 
-    def __repr__(cls):
+    def __repr__(self):
         attrs = [
-            ("name", cls.name),
-            ("id", cls.id),
+            ("name", self.name),
+            ("id", self.id),
         ]
         return "<%s %s>" % (
-            cls.__name__, " ".join("%s=%r" % t for t in attrs),)
-
+            self.__class__.__name__, " ".join("%s=%r" % t for t in attrs),)
 
     @classmethod
     def _inject_super_meta(cls, troop_meta):
         cls.is_super_troop = True
 
         cls.cooldown = try_enum(UnitStat, [TimeDelta(hours=hours) for hours in troop_meta.get("CooldownH", [])])
         cls.duration = try_enum(UnitStat, [TimeDelta(hours=hours) for hours in troop_meta.get("DurationH", [])])
@@ -133,15 +131,15 @@
         # 1. Hero/troop levels in-game are 1-indexed, UnitStat is 1-indexed
         # 2. TH-lab levels in-game and here are 1-indexed
         # 3. We then want to check that for the level less than this troop the req'd
         #    TH is less than or equal to current TH,
         #    and for troop level above, it requires a higher TH than we currently have.
         #    Maybe there's a better way to go about doing this.
         return self.lab_to_townhall[self.__class__.lab_level[self.level]] <= self._townhall \
-                    < self.lab_to_townhall[self.__class__.lab_level[self.level + 1]]
+             < self.lab_to_townhall[self.__class__.lab_level[self.level + 1]]
 
     @classmethod
     def get_max_level_for_townhall(cls, townhall):
         """Get the maximum level for a troop for a given townhall level.
 
         Parameters
         ----------
@@ -219,8 +217,7 @@
         return troop(data=data, townhall=townhall)
 
     def get(self, name, home_village=True) -> Optional[Type[Troop]]:
         try:
             return self.item_lookup[(name, home_village)]
         except KeyError:
             return None
-
```

### Comparing `coc.py-2.3.1/coc/utils.py` & `coc.py-2.4.0/coc/utils.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/war_attack.py` & `coc.py-2.4.0/coc/war_attack.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/war_clans.py` & `coc.py-2.4.0/coc/war_clans.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/war_members.py` & `coc.py-2.4.0/coc/war_members.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc/wars.py` & `coc.py-2.4.0/coc/wars.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.3.1/coc.py.egg-info/PKG-INFO` & `coc.py-2.4.0/coc.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 2.3.1
+Version: 2.4.0
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
-Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, doluk
+Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
 Keywords: coc,clash of clans,coc.py,clash api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -74,23 +74,23 @@
     async def main():
         async with coc.Client() as coc_client:
             try:
                 await coc_client.login("email", "password")
             except coc.invalidcredentials as error:
                 exit(error)
 
-            player = await client.get_player("tag")
+            player = await coc_client.get_player("tag")
             print(f"{player.name} has {player.trophies} trophies!")
 
-            clans = await client.search_clans(name="best clan ever", limit=5)
+            clans = await coc_client.search_clans(name="best clan ever", limit=5)
             for clan in clans:
                 print(f"{clan.name} ({clan.tag}) has {clan.member_count} members")
 
             try:
-                war = await client.get_current_war("#clantag")
+                war = await coc_client.get_current_war("#clantag")
                 print(f"{war.clan_tag} is currently in {war.state} state.")
             except coc.privatewarlog:
                 print("uh oh, they have a private war log!")
 
     if __name__ == "__main__":
         try:
             asyncio.run(main())
```

### Comparing `coc.py-2.3.1/coc.py.egg-info/SOURCES.txt` & `coc.py-2.4.0/coc.py.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 coc.py.egg-info/PKG-INFO
 coc.py.egg-info/SOURCES.txt
 coc.py.egg-info/dependency_links.txt
 coc.py.egg-info/requires.txt
 coc.py.egg-info/top_level.txt
 coc/ext/discordlinks/__init__.py
 coc/ext/fullwarapi/__init__.py
+coc/ext/triggers/__init__.py
+coc/ext/triggers/cron.py
+coc/ext/triggers/triggers.py
 coc/static/buildings.json
 coc/static/characters.json
 coc/static/heroes.json
 coc/static/object_ids.json
 coc/static/pets.json
 coc/static/spells.json
 coc/static/supers.json
```

### Comparing `coc.py-2.3.1/pyproject.toml` & `coc.py-2.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coc.py"
 authors = [{ name = "mathsman5133" }]
-maintainers = [{ name = "majordoobie" }, { name = "MagicTheDev" }, { name = "Kuchenmampfer" }, { name = "doluk" }]
-version = "2.3.1"
+maintainers = [{ name = "majordoobie" }, { name = "MagicTheDev" }, { name = "Kuchenmampfer" }, { name = "lukasthaler" }, { name = "doluk" }]
+version = "2.4.0"
 description = "A python wrapper for the Clash of Clans API"
 requires-python = ">=3.7.3"
 readme = "README.rst"
 license = { text = "MIT" }
 keywords = ["coc", "clash of clans", "coc.py", "clash api"]
 classifiers = ["Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
@@ -26,12 +26,12 @@
 docs = ["sphinx",
     "sphinx_rtd_theme",
     "sphinxcontrib_trio",
     "autodocsumm",
 ]
 
 [tool.setuptools]
-packages = ["coc", "coc.ext.discordlinks", "coc.static", "coc.ext.fullwarapi"]
+packages = ["coc", "coc.ext.discordlinks", "coc.static", "coc.ext.fullwarapi", "coc.ext.triggers"]
 include-package-data = true
 
 [tool.setuptools.package-data]
 coc = ["events.pyi"]
```

