# Comparing `tmp/hoyo-daily-logins-helper-2.2.0.tar.gz` & `tmp/hoyo-daily-logins-helper-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo-daily-logins-helper-2.2.0.tar", last modified: Fri May 12 03:43:10 2023, max compression
+gzip compressed data, was "hoyo-daily-logins-helper-2.2.1.tar", last modified: Sun May 14 01:48:02 2023, max compression
```

## Comparing `hoyo-daily-logins-helper-2.2.0.tar` & `hoyo-daily-logins-helper-2.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/hoyo-daily-logins-helper.toml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:43:10.482711 hoyo-daily-logins-helper-2.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 03:43:10.000000 hoyo-daily-logins-helper-2.2.0/src/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-12 03:42:53.000000 hoyo-daily-logins-helper-2.2.0/src/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:48:02.479201 hoyo-daily-logins-helper-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:48:02.475201 hoyo-daily-logins-helper-2.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:48:02.479201 hoyo-daily-logins-helper-2.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-14 01:48:02.479201 hoyo-daily-logins-helper-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/hoyo-daily-logins-helper.toml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:48:02.479201 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:48:02.479201 hoyo-daily-logins-helper-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:48:02.479201 hoyo-daily-logins-helper-2.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-14 01:48:02.000000 hoyo-daily-logins-helper-2.2.1/src/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-14 01:47:41.000000 hoyo-daily-logins-helper-2.2.1/src/scheduler.py
```

### Comparing `hoyo-daily-logins-helper-2.2.0/.github/workflows/deploy.yml` & `hoyo-daily-logins-helper-2.2.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.0/.github/workflows/tests.yml` & `hoyo-daily-logins-helper-2.2.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.0/.gitignore` & `hoyo-daily-logins-helper-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.0/LICENSE` & `hoyo-daily-logins-helper-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.0/PKG-INFO` & `hoyo-daily-logins-helper-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.2.0
+Version: 2.2.1
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hoyo-daily-logins-helper-2.2.0/README.md` & `hoyo-daily-logins-helper-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.0/hoyo-daily-logins-helper.toml.template` & `hoyo-daily-logins-helper-2.2.1/hoyo-daily-logins-helper.toml.template`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/PKG-INFO` & `hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.2.0
+Version: 2.2.1
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hoyo-daily-logins-helper-2.2.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt` & `hoyo-daily-logins-helper-2.2.1/hoyo_daily_logins_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.0/pyproject.toml` & `hoyo-daily-logins-helper-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 keywords = ["genshin", "genshin-impact", "starrail", "honkai-starrail", "game"]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
 dependencies = [
     "requests",
     "comboparse",
+    "scheduler",
     "pytz",
-    "apscheduler",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 hoyo-daily-logins-helper = "src.main:main"
 
 [tool.setuptools]
```

### Comparing `hoyo-daily-logins-helper-2.2.0/src/games.py` & `hoyo-daily-logins-helper-2.2.1/src/games.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.0/src/http.py` & `hoyo-daily-logins-helper-2.2.1/src/http.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.2.0/src/main.py` & `hoyo-daily-logins-helper-2.2.1/src/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,11 +196,11 @@
         if account_identifiers[index]:
             identifier = account_identifiers[index]
 
         game_perform_checkin(identifier, game, cookie, args.language)
 
 
 def has_legacy_environment_variable() -> bool:
-    for env_var in ["LANG", "LANGUAGE", "COOKIE", "GAME"]:
+    for env_var in ["LANGUAGE", "COOKIE", "GAME"]:
         if env_var in os.environ:
             return True
     return False
```

### Comparing `hoyo-daily-logins-helper-2.2.0/src/scheduler.py` & `hoyo-daily-logins-helper-2.2.1/src/scheduler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import logging
+from datetime import datetime, timezone, time
+from time import sleep
 
-from apscheduler.schedulers.blocking import BlockingScheduler
-from apscheduler.triggers.cron import CronTrigger
-from pytz import timezone
+import pytz
+from scheduler import Scheduler
 
 from src.games import game_perform_checkin
 
 _RESET_TIME = {
     # running this one hour after reset to prevent potential fuckery with
     # timezones
     "hour": 5,
     "minute": 1,
 }
 
 _RESET_TIMES = {
-    "Asia": CronTrigger(timezone=timezone("Etc/GMT+8"), **_RESET_TIME),
-    "EU": CronTrigger(timezone=timezone("Etc/GMT+1"), **_RESET_TIME),
-    "NA": CronTrigger(timezone=timezone("Etc/GMT-5"), **_RESET_TIME)
+    "Asia": time(tzinfo=pytz.timezone("Etc/GMT+8"), **_RESET_TIME),
+    "EU": time(tzinfo=pytz.timezone("Etc/GMT+1"), **_RESET_TIME),
+    "NA": time(tzinfo=pytz.timezone("Etc/GMT-5"), **_RESET_TIME),
 }
 
 
 def run_scheduler(config_data: dict, language: str):
     logging.info("Run in scheduler mode")
 
-    # only show warnings and above from apscheduler
-    logging.getLogger("apscheduler").setLevel(logging.WARNING)
+    tz = datetime.now(timezone.utc).astimezone().tzinfo
 
-    scheduler = BlockingScheduler()
+    schedule = Scheduler(tzinfo=tz)
 
     accounts = config_data.get("accounts", [])
     default_region = config_data.get("config", {}).get("region", None)
 
     for index, account in enumerate(accounts):
         region = account.get("region", default_region)
 
@@ -43,39 +43,52 @@
             continue
 
         identifier = account.get("identifier", None)
 
         if not identifier:
             identifier = f"Account #{index}"
 
-        scheduler.add_job(
-            create_checkin_job(
-                identifier,
-                account.get("game"),
-                account.get("cookie"),
-                language,
-            ),
-            _RESET_TIMES[region]
+        checkin_job = create_checkin_job(
+            identifier,
+            account.get("game"),
+            account.get("cookie"),
+            language,
+        )
+
+        job = schedule.daily(
+            _RESET_TIMES[region],
+            checkin_job
+        )
+
+        due_in_hours = round(
+            job.timedelta(datetime.now(tz=tz)).total_seconds() / 60 / 60,#
+            1
         )
 
         logging.info(
-            f"Added account '{identifier}' to scheduler, region: '{region}'"
+            f"Added account '{identifier}' to scheduler, region: '{region}', "
+            f"next fire time in {due_in_hours} hours"
         )
 
-    if len(scheduler.get_jobs()) == 0:
+    if len(schedule.jobs) == 0:
         logging.error("No jobs scheduled")
         exit(1)
 
-    scheduler.start()
+    logging.debug("Job schedule:")
+    logging.debug(schedule)
+
+    while True:
+        schedule.exec_jobs()
+        sleep(60)
 
 
 def create_checkin_job(
-    account_ident: str,
-    game: str,
-    cookie_str: str,
-    language: str
+        account_ident: str,
+        game: str,
+        cookie_str: str,
+        language: str
 ):
     def _checkin_job():
         logging.info(f"Running scheduler for '{account_ident}'...")
         game_perform_checkin(account_ident, game, cookie_str, language)
 
     return _checkin_job
```

