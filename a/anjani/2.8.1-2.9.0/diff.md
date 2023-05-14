# Comparing `tmp/anjani-2.8.1.tar.gz` & `tmp/anjani-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anjani-2.8.1.tar", max compression
+gzip compressed data, was "anjani-2.9.0.tar", max compression
```

## Comparing `anjani-2.8.1.tar` & `anjani-2.9.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    35148 2023-01-23 08:38:21.480353 anjani-2.8.1/LICENSE
--rw-r--r--   0        0        0     1608 2023-01-23 08:38:21.480353 anjani-2.8.1/README.md
--rw-r--r--   0        0        0      869 2023-01-24 03:23:44.323352 anjani-2.8.1/anjani/__init__.py
--rw-r--r--   0        0        0      806 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/__main__.py
--rw-r--r--   0        0        0     3168 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/action.py
--rw-r--r--   0        0        0    11423 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/command.py
--rw-r--r--   0        0        0      795 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/core/__init__.py
--rw-r--r--   0        0        0     2653 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/core/anjani_bot.py
--rw-r--r--   0        0        0      922 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/core/anjani_mixin_base.py
--rw-r--r--   0        0        0     9294 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/core/command_dispatcher.py
--rw-r--r--   0        0        0     1475 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/core/database_provider.py
--rw-r--r--   0        0        0    11592 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/core/event_dispatcher.py
--rw-r--r--   0        0        0     3613 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/core/plugin_extenter.py
--rw-r--r--   0        0        0    12964 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/core/telegram_bot.py
--rw-r--r--   0        0        0     1254 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/custom_plugins/__init__.py
--rw-r--r--   0        0        0     5114 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/custom_plugins/example.py
--rw-r--r--   0        0        0     4479 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/error.py
--rw-r--r--   0        0        0     8650 2023-01-24 03:23:44.323352 anjani-2.8.1/anjani/filters.py
--rw-r--r--   0        0        0     1010 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/language/__init__.py
--rw-r--r--   0        0        0    30359 2023-01-24 03:23:44.323352 anjani-2.8.1/anjani/language/en.yml
--rw-r--r--   0        0        0    37214 2023-01-24 03:23:44.323352 anjani-2.8.1/anjani/language/id.yml
--rw-r--r--   0        0        0     2127 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/listener.py
--rw-r--r--   0        0        0     4258 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/main.py
--rw-r--r--   0        0        0     4440 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugin.py
--rw-r--r--   0        0        0     1254 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/__init__.py
--rw-r--r--   0        0        0     7913 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/admins.py
--rw-r--r--   0        0        0     3810 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/backups.py
--rw-r--r--   0        0        0     7073 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/canonical.py
--rw-r--r--   0        0        0     5464 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/debug.py
--rw-r--r--   0        0        0    42453 2023-01-24 03:23:37.823354 anjani-2.8.1/anjani/plugins/federation.py
--rw-r--r--   0        0        0     5822 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/filters.py
--rw-r--r--   0        0        0     5453 2023-01-24 03:23:37.823354 anjani-2.8.1/anjani/plugins/language.py
--rw-r--r--   0        0        0    13610 2023-01-24 03:23:44.323352 anjani-2.8.1/anjani/plugins/lockings.py
--rw-r--r--   0        0        0    12541 2023-01-24 03:23:44.323352 anjani-2.8.1/anjani/plugins/main.py
--rw-r--r--   0        0        0     5992 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/misc.py
--rw-r--r--   0        0        0     4778 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/muting.py
--rw-r--r--   0        0        0     9015 2023-01-24 03:23:44.323352 anjani-2.8.1/anjani/plugins/notes.py
--rw-r--r--   0        0        0     2403 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/purge.py
--rw-r--r--   0        0        0     6572 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/reporting.py
--rw-r--r--   0        0        0    14063 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/restriction.py
--rw-r--r--   0        0        0     4103 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/rules.py
--rw-r--r--   0        0        0    28981 2023-01-24 03:23:44.323352 anjani-2.8.1/anjani/plugins/spam_prediction.py
--rw-r--r--   0        0        0    12378 2023-01-24 03:23:37.823354 anjani-2.8.1/anjani/plugins/spam_shield.py
--rw-r--r--   0        0        0     4127 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/staff_tools.py
--rw-r--r--   0        0        0     7022 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/stats.py
--rw-r--r--   0        0        0    16522 2023-01-23 08:38:21.480353 anjani-2.8.1/anjani/plugins/users.py
--rw-r--r--   0        0        0    16013 2023-01-24 03:23:37.833354 anjani-2.8.1/anjani/plugins/welcome.py
--rw-r--r--   0        0        0      932 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/__init__.py
--rw-r--r--   0        0        0     1148 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/async_helper.py
--rw-r--r--   0        0        0     2153 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/config.py
--rw-r--r--   0        0        0     8192 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/converter.py
--rw-r--r--   0        0        0     1040 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/db/__init__.py
--rw-r--r--   0        0        0     3304 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/db/base.py
--rw-r--r--   0        0        0     4331 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/db/change_stream.py
--rw-r--r--   0        0        0     8496 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/db/client.py
--rw-r--r--   0        0        0     6747 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/db/client_session.py
--rw-r--r--   0        0        0    17722 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/db/collection.py
--rw-r--r--   0        0        0     7389 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/db/command_cursor.py
--rw-r--r--   0        0        0     6445 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/db/cursor.py
--rw-r--r--   0        0        0     6889 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/db/cursor_base.py
--rw-r--r--   0        0        0     9279 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/db/db.py
--rw-r--r--   0        0        0      863 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/db/errors.py
--rw-r--r--   0        0        0     1259 2023-01-24 03:23:44.323352 anjani-2.8.1/anjani/util/db/typings.py
--rw-r--r--   0        0        0     1445 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/error.py
--rw-r--r--   0        0        0     2109 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/misc.py
--rw-r--r--   0        0        0     3351 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/system.py
--rw-r--r--   0        0        0    10999 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/tg.py
--rw-r--r--   0        0        0     2364 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/time.py
--rw-r--r--   0        0        0     1819 2023-01-23 08:38:21.490353 anjani-2.8.1/anjani/util/types.py
--rw-r--r--   0        0        0     2804 2023-01-24 03:23:44.323352 anjani-2.8.1/pyproject.toml
--rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 anjani-2.8.1/setup.py
--rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 anjani-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-01-23 08:38:21.480353 anjani-2.9.0/LICENSE
+-rw-r--r--   0        0        0     1608 2023-01-23 08:38:21.480353 anjani-2.9.0/README.md
+-rw-r--r--   0        0        0      869 2023-02-08 11:36:14.005726 anjani-2.9.0/anjani/__init__.py
+-rw-r--r--   0        0        0      806 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/__main__.py
+-rw-r--r--   0        0        0     3168 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/action.py
+-rw-r--r--   0        0        0    11423 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/command.py
+-rw-r--r--   0        0        0      795 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/core/__init__.py
+-rw-r--r--   0        0        0     2649 2023-02-08 11:27:36.545896 anjani-2.9.0/anjani/core/anjani_bot.py
+-rw-r--r--   0        0        0      922 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/core/anjani_mixin_base.py
+-rw-r--r--   0        0        0     9294 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/core/command_dispatcher.py
+-rw-r--r--   0        0        0     1475 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/core/database_provider.py
+-rw-r--r--   0        0        0    11592 2023-01-29 15:25:01.609916 anjani-2.9.0/anjani/core/event_dispatcher.py
+-rw-r--r--   0        0        0     3613 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/core/plugin_extenter.py
+-rw-r--r--   0        0        0    13033 2023-02-08 11:27:36.545896 anjani-2.9.0/anjani/core/telegram_bot.py
+-rw-r--r--   0        0        0     1254 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/custom_plugins/__init__.py
+-rw-r--r--   0        0        0     5114 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/custom_plugins/example.py
+-rw-r--r--   0        0        0     4479 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/error.py
+-rw-r--r--   0        0        0     8650 2023-02-08 11:36:14.005726 anjani-2.9.0/anjani/filters.py
+-rw-r--r--   0        0        0     1010 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/language/__init__.py
+-rw-r--r--   0        0        0    30527 2023-02-08 11:36:14.005726 anjani-2.9.0/anjani/language/en.yml
+-rw-r--r--   0        0        0    37434 2023-02-08 11:36:14.005726 anjani-2.9.0/anjani/language/id.yml
+-rw-r--r--   0        0        0     2127 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/listener.py
+-rw-r--r--   0        0        0     4304 2023-02-08 11:27:36.545896 anjani-2.9.0/anjani/main.py
+-rw-r--r--   0        0        0     4440 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/plugin.py
+-rw-r--r--   0        0        0     1254 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/plugins/__init__.py
+-rw-r--r--   0        0        0     7913 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/plugins/admins.py
+-rw-r--r--   0        0        0     3810 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/plugins/backups.py
+-rw-r--r--   0        0        0     7073 2023-01-28 07:59:39.225948 anjani-2.9.0/anjani/plugins/canonical.py
+-rw-r--r--   0        0        0     5464 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/plugins/debug.py
+-rw-r--r--   0        0        0    42453 2023-02-08 11:36:14.005726 anjani-2.9.0/anjani/plugins/federation.py
+-rw-r--r--   0        0        0     9266 2023-02-08 11:29:00.415868 anjani-2.9.0/anjani/plugins/filters.py
+-rw-r--r--   0        0        0     5453 2023-02-08 11:36:14.005726 anjani-2.9.0/anjani/plugins/language.py
+-rw-r--r--   0        0        0    13610 2023-02-08 11:36:14.005726 anjani-2.9.0/anjani/plugins/lockings.py
+-rw-r--r--   0        0        0    12541 2023-02-08 11:36:14.005726 anjani-2.9.0/anjani/plugins/main.py
+-rw-r--r--   0        0        0     5992 2023-02-08 11:36:14.005726 anjani-2.9.0/anjani/plugins/misc.py
+-rw-r--r--   0        0        0     4778 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/plugins/muting.py
+-rw-r--r--   0        0        0     9015 2023-02-08 11:36:14.005726 anjani-2.9.0/anjani/plugins/notes.py
+-rw-r--r--   0        0        0     2403 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/plugins/purge.py
+-rw-r--r--   0        0        0     6572 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/plugins/reporting.py
+-rw-r--r--   0        0        0    14062 2023-02-08 11:29:00.415868 anjani-2.9.0/anjani/plugins/restriction.py
+-rw-r--r--   0        0        0     4103 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/plugins/rules.py
+-rw-r--r--   0        0        0    29333 2023-02-08 11:36:14.005726 anjani-2.9.0/anjani/plugins/spam_prediction.py
+-rw-r--r--   0        0        0    12378 2023-02-08 11:36:14.005726 anjani-2.9.0/anjani/plugins/spam_shield.py
+-rw-r--r--   0        0        0     4127 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/plugins/staff_tools.py
+-rw-r--r--   0        0        0     7022 2023-01-23 08:38:21.480353 anjani-2.9.0/anjani/plugins/stats.py
+-rw-r--r--   0        0        0    16522 2023-02-08 11:29:00.415868 anjani-2.9.0/anjani/plugins/users.py
+-rw-r--r--   0        0        0    16013 2023-02-08 11:36:14.005726 anjani-2.9.0/anjani/plugins/welcome.py
+-rw-r--r--   0        0        0      932 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/__init__.py
+-rw-r--r--   0        0        0     1148 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/async_helper.py
+-rw-r--r--   0        0        0     2153 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/config.py
+-rw-r--r--   0        0        0     8192 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/converter.py
+-rw-r--r--   0        0        0     1040 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/db/__init__.py
+-rw-r--r--   0        0        0     3304 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/db/base.py
+-rw-r--r--   0        0        0     4331 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/db/change_stream.py
+-rw-r--r--   0        0        0     8496 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/db/client.py
+-rw-r--r--   0        0        0     6747 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/db/client_session.py
+-rw-r--r--   0        0        0    17722 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/db/collection.py
+-rw-r--r--   0        0        0     7389 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/db/command_cursor.py
+-rw-r--r--   0        0        0     6445 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/db/cursor.py
+-rw-r--r--   0        0        0     6889 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/db/cursor_base.py
+-rw-r--r--   0        0        0     9279 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/db/db.py
+-rw-r--r--   0        0        0      863 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/db/errors.py
+-rw-r--r--   0        0        0     1259 2023-01-26 04:22:33.523681 anjani-2.9.0/anjani/util/db/typings.py
+-rw-r--r--   0        0        0     1445 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/error.py
+-rw-r--r--   0        0        0     2109 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/misc.py
+-rw-r--r--   0        0        0     3351 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/system.py
+-rw-r--r--   0        0        0    10999 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/tg.py
+-rw-r--r--   0        0        0     2364 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/time.py
+-rw-r--r--   0        0        0     1819 2023-01-23 08:38:21.490353 anjani-2.9.0/anjani/util/types.py
+-rw-r--r--   0        0        0     2804 2023-02-08 11:36:14.005726 anjani-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 anjani-2.9.0/setup.py
+-rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 anjani-2.9.0/PKG-INFO
```

### Comparing `anjani-2.8.1/LICENSE` & `anjani-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/README.md` & `anjani-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/__init__.py` & `anjani-2.9.0/anjani/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-__version__ = "2.8.1"
+__version__ = "2.9.0"
 
 __description__ = "Telegram group management bot with spam protection."
 
 DEFAULT_CONFIG_PATH = "config.env"
```

### Comparing `anjani-2.8.1/anjani/__main__.py` & `anjani-2.9.0/anjani/__main__.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/action.py` & `anjani-2.9.0/anjani/action.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/command.py` & `anjani-2.9.0/anjani/command.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/core/__init__.py` & `anjani-2.9.0/anjani/core/__init__.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/core/anjani_bot.py` & `anjani-2.9.0/anjani/core/anjani_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
 import logging
-from typing import Any, Optional
+from typing import Optional
 
 import aiohttp
 import pyrogram
 
 from anjani.util.config import TelegramConfig
 
 from .command_dispatcher import CommandDispatcher
@@ -72,12 +72,13 @@
 
         self.log.info("Stopping")
         if self.loaded:
             await self.dispatch_event("stop")
             if self.client.is_connected:
                 await self.client.stop()
         await self.http.close()
-        await self.db.close()
 
         self.log.info("Running post-stop hooks")
         if self.loaded:
             await self.dispatch_event("stopped")
+
+        await self.db.close()
```

### Comparing `anjani-2.8.1/anjani/core/anjani_mixin_base.py` & `anjani-2.9.0/anjani/core/anjani_mixin_base.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/core/command_dispatcher.py` & `anjani-2.9.0/anjani/core/command_dispatcher.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/core/database_provider.py` & `anjani-2.9.0/anjani/core/database_provider.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/core/event_dispatcher.py` & `anjani-2.9.0/anjani/core/event_dispatcher.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/core/plugin_extenter.py` & `anjani-2.9.0/anjani/core/plugin_extenter.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/core/telegram_bot.py` & `anjani-2.9.0/anjani/core/telegram_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         # Initialize Telegram client with gathered parameters
         self.client = Client(
             name="anjani",
             api_id=api_id,
             api_hash=api_hash,
             bot_token=bot_token,
             workdir="anjani",
+            workers=int(self.config.get("workers", Client.WORKERS)),
             parse_mode=ParseMode.MARKDOWN,
         )
 
     async def start(self: "Anjani") -> None:
         if self.__running:
             raise RuntimeError("This bot instance is already running")
```

### Comparing `anjani-2.8.1/anjani/custom_plugins/__init__.py` & `anjani-2.9.0/anjani/custom_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/custom_plugins/example.py` & `anjani-2.9.0/anjani/custom_plugins/example.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/error.py` & `anjani-2.9.0/anjani/error.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/filters.py` & `anjani-2.9.0/anjani/filters.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/language/__init__.py` & `anjani-2.9.0/anjani/language/__init__.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/language/en.yml` & `anjani-2.9.0/anjani/language/en.yml`

 * *Files 2% similar despite different names*

```diff
@@ -278,15 +278,15 @@
 filters-added: "Successfully added `{}` as filters."
 filters-removed: "Successfully removed `{}` from filters."
 filter-help: "Usage: `/filter <trigger> <text>`."
 filter-stop-help: "Usage: `/stop <trigger>`."
 filters-chat-nofilter: This chat has no filters.
 filters-chat-nokeyword: "No filters named `{}` on this chat."
 filters-rmall: "Successfully removed {} filters in this chat."
-filters-list: "Filters in **{}**:"
+filters-list: "Filters in **{}**:\n"
 #endregion
 #region language
 language-button: Language
 language-help: |
   This bot comes up with multi language support.
   You can choose your language preference!\n
   **Available languages:**
@@ -475,26 +475,30 @@
 #endregion
 #region spam prediction
 spampredict-button: Spam Prediction
 spampredict-help: |
   For addition we currently developing a spam protection using a machine learning. The bot will detect and delete spam messages from your chats.
   You can also help us to train our model by casting a vote on @SpamPredictionLog. You will earn a reputation point with some benefit in the future 😉.\n
   **Admin Commands:**
-  /spampredict <on/off/yes/no>: Will disable or enable the message spam prediction in your group.\n
-  If enabled, the bot will automaticaly delete and log the message to @SpamPredictionLog.
+  × /spampredict <on/off/yes/no>: Will disable or enable the message spam prediction in your group.\n
+  If enabled, the bot will automaticaly delete and log the message to @SpamPredictionLog.\n
+  **User Commands:**
+  × /predict <reply>: Will predict the message if it's a spam or not*.
+  *this will consume 10 reputation point.
 spampredict-set: "Chat spam prediction turned {}."
 spampredict-view: |
   Spam Prediction Setting: **{}**.
   When enabled will automaticaly delete the message that are detected as a spam.
 spampredict-empty: message/photo text nor caption is empty to predict...
 spampredict-photo: "Reading photo text with ocr...\nThis might take a while."
 spampredict-photo-failed: "__Failed to read photo text with ocr.__\n\n"
-spampredict-unauthorized: |
-  Your reputation point is not enough to use this command! ({}/{})
-  To get a reputation point cast a vote on @SpamPredictionLog.
+spampredict-insuficent: |
+  Insuficent reputation to run prediction! ({}/{}).
+  Prediction will consume {} reputation point.
+  You can earn reputation by voting on @SpamPredictionLog.
 spampredict-failed: Prediction failed...
 spampredict-ban: "{user} has been banned!"
 spampredict-ban-no-perm: You don't have permission to ban users!
 #endregion
 #region spam shield
 spamshield-button: Spam Shield
 spamshield-help: |
```

### Comparing `anjani-2.8.1/anjani/language/id.yml` & `anjani-2.9.0/anjani/language/id.yml`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 filters-added: "Berhasil menambahkan `{}` sebagai filter."
 filters-removed: "Berhasil menghapus `{}` dari filter."
 filter-help: "Contoh: `/filter <kata kunci> <teks>`"
 filter-stop-help: "Contoh: `/stop <kata kunci>`"
 filters-chat-nofilter: Grup ini tidak memiliki filter.
 filters-chat-nokeyword: "Tidak ada filter dengan kata kunci `{}` di grup ini."
 filters-rmall: "Berhasil menghapus {} filter pada grup ini."
-filters-list: "Filter pada **{}**:"
+filters-list: "Filter pada **{}**:\n"
 #endregion
 #region language
 language-button: Bahasa
 language-help: |
   Bot ini hadir dengan dukungan multi bahasa.
   Anda dapat memilih preferensi bahasa anda!\n
   ** Bahasa yang tersedia: **
@@ -499,36 +499,40 @@
 #endregion
 #region spam prediction
 spampredict-button: Spam Prediksi
 spampredict-help: |
   Sebagai tambahan, saat ini kami sedang mengembangkan perlindungan spam menggunakan machine learning. Bot akan mendeteksi dan menghapus pesan spam dari grup anda.
   Anda juga dapat membantu kami mendidik model kami dengan memberikan suara di @SpamPredictionLog. Anda akan mendapatkan poin reputasi dengan beberapa manfaat ke depannya 😉.\n
   **Hanya Administrator yang bisa menggunakan:**
-  /spampredict <on/off/yes/no>: Akan mematikan atau menyalakan pengaruh dari perlindungan spam di grup anda.\n
-  Jika dinyalakan, bot akan otomatis menghapus dan mencatat pesan ke @SpamPredictionLog.
+  × /spampredict <on/off/yes/no>: Akan mematikan atau menyalakan pengaruh dari perlindungan spam di grup anda.\n
+  Jika dinyalakan, bot akan otomatis menghapus dan mencatat pesan ke @SpamPredictionLog.\n
+  **Perintah pengguna:**
+  × /predict <balas ke pesan>: Bot akan memprediksi apakah pesan itu spam atau tidak*.
+  *perintah ini akan memakai 10 poin reputasi anda.
 spampredict-set: "Chat spam prediksi berubah ke {}."
 spampredict-view: |
   Spam Prediction Setting: **{}**.
   Jika dinyalakan akan otomatis menghapus pesan yang terdeteksi sebagai suatu spam.
 spampredict-empty: pesan/photo teks atau keterangan media kosong untuk diprediksi...
 spampredict-photo: "Membaca teks pada foto dengan ocr...\nIni bisa saja membutuhkan waktu lama."
 spampredict-photo-failed: "__Gagal membaca teks pada foto dengan ocr.__\n\n"
-spampredict-unauthorized: |
-  Poin reputasi anda tidak cukup untuk menggunakan perintah ini! ({}/{})
+spampredict-insuficent: |
+  Poin reputasi anda tidak cukup untuk menjalankan perintah prediksi! ({}/{})
+  Prediksi akan memakai {} poin reputasi anda.
   Untuk mendapatkan poin reputasi silahkan berikan suara di @SpamPredictionLog.
 spampredict-failed: Prediksi gagal...
 spampredict-ban: "{user} telah diblokir!"
 spampredict-ban-no-perm: "Kamu tidak punya izin untuk melakukan ini!"
 #endregion
 #region spam shield
 spamshield-button: Spam Shield
 spamshield-help: |
   **Hanya Administrator yang bisa menggunakan:**
-   /spamshield <on/off/yes/no>: Akan mematikan atau menyalakan pengaruh dari perlindungan spam di grup anda.\n
-   Spam shield menggunakan Combot Anti Spam, API @Spamwatch, dan larangan global untuk menghapus sebanyak mungkin orang yang melakukan spam dari ruang obrolan anda!
+  /spamshield <on/off/yes/no>: Akan mematikan atau menyalakan pengaruh dari perlindungan spam di grup anda.\n
+  Spam shield menggunakan Combot Anti Spam, API @Spamwatch, dan larangan global untuk menghapus sebanyak mungkin orang yang melakukan spam dari ruang obrolan anda!
 banned-text: |
   #SPAM_SHIELD\n
   **Nama:** {}
   **ID:** `{}`
   **Alasan**: {}
   **Client:** {}
   Orang ini terdeteksi sebagai spambot dan sudah dikeluarkan!
```

### Comparing `anjani-2.8.1/anjani/listener.py` & `anjani-2.9.0/anjani/listener.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/main.py` & `anjani-2.9.0/anjani/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     loop = asyncio.new_event_loop()
 
     # Initialize config
     config_data: MutableMapping[str, Any] = {
         "api_id": os.environ.get("API_ID"),
         "api_hash": os.environ.get("API_HASH"),
         "bot_token": os.environ.get("BOT_TOKEN"),
+        "workers": os.environ.get("WORKERS"),
         "db_uri": os.environ.get("DB_URI"),
         "download_path": os.environ.get("DOWNLOAD_PATH"),
         "owner_id": os.environ.get("OWNER_ID"),
         "sw_api": os.environ.get("SW_API"),
         "log_channel": os.environ.get("LOG_CHANNEL"),
         "login_url": os.environ.get("LOGIN_URL"),
     }
```

### Comparing `anjani-2.8.1/anjani/plugin.py` & `anjani-2.9.0/anjani/plugin.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/__init__.py` & `anjani-2.9.0/anjani/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/admins.py` & `anjani-2.9.0/anjani/plugins/admins.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/backups.py` & `anjani-2.9.0/anjani/plugins/backups.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/canonical.py` & `anjani-2.9.0/anjani/plugins/canonical.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/debug.py` & `anjani-2.9.0/anjani/plugins/debug.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/federation.py` & `anjani-2.9.0/anjani/plugins/federation.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/filters.py` & `anjani-2.9.0/anjani/plugins/reporting.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Filters plugin. """
+""" Admin reporting plugin """
 # Copyright (C) 2020 - 2023  UserbotIndo Team, <https://github.com/userbotindo.git>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -10,143 +10,169 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import re
-from typing import Any, ClassVar, MutableMapping, Optional, Set, Tuple
+import asyncio
+from typing import Any, MutableMapping, Optional
 
+from pyrogram.enums.chat_member_status import ChatMemberStatus
+from pyrogram.enums.chat_type import ChatType
+from pyrogram.errors import UserNotParticipant
 from pyrogram.types import Message
 
 from anjani import command, filters, listener, plugin, util
 
 
-class Filters(plugin.Plugin):
-    name: ClassVar[str] = "Filters"
-    helpable: ClassVar[bool] = True
+class Reporting(plugin.Plugin):
+    name = "Reporting"
+    helpable = True
 
     db: util.db.AsyncCollection
-    trigger: MutableMapping[int, Set[str]] = {}
+    user_db: util.db.AsyncCollection
 
     async def on_load(self) -> None:
-        self.db = self.bot.db.get_collection("FILTERS")
-
-    async def on_start(self, _: int) -> None:
-        async for chat in self.db.find({}):
-            self.trigger[chat["chat_id"]] = set(chat["trigger"].keys())
-
-    async def on_plugin_backup(self, chat_id: int) -> MutableMapping[str, Any]:
-        data = await self.db.find_one({"chat_id": chat_id}, {"_id": False})
-        return {self.name: data} if data else {}
-
-    async def on_plugin_restore(self, chat_id: int, data: MutableMapping[str, Any]) -> None:
-        await self.db.update_one({"chat_id": chat_id}, {"$set": {data[self.name]}}, upsert=True)
+        self.db = self.bot.db.get_collection("CHAT_REPORTING")
+        self.user_db = self.bot.db.get_collection("USER_REPORTING")
 
     async def on_chat_migrate(self, message: Message) -> None:
         new_chat = message.chat.id
         old_chat = message.migrate_from_chat_id
 
         await self.db.update_one(
             {"chat_id": old_chat},
             {"$set": {"chat_id": new_chat}},
         )
 
-    @listener.priority(95)
-    async def on_message(self, message: Message) -> None:
-        if message.outgoing:
-            return
+    async def on_plugin_backup(self, chat_id: int) -> MutableMapping[str, Any]:
+        report = await self.db.find_one({"chat_id": chat_id}, {"_id": False})
+        return {self.name: report} if report else {}
 
+    async def on_plugin_restore(self, chat_id: int, data: MutableMapping[str, Any]) -> None:
+        await self.db.update_one({"chat_id": chat_id}, {"$set": data[self.name]}, upsert=True)
+
+    @listener.filters(filters.regex(r"^(?i)@admin(s)?\b") & filters.group & ~filters.outgoing)
+    async def on_message(self, message: Message) -> None:
         chat = message.chat
-        text = message.text or message.caption
+        user = message.from_user
+        if not await self.is_active(chat.id, is_private=False):
+            return
 
-        if not (text or chat):
+        # Anonymous admins, so ignore it
+        if not user:
             return
 
-        chat_trigger = self.trigger.get(chat.id, [])
-        if not chat_trigger:
+        try:
+            invoker = await chat.get_member(user.id)
+            if invoker.status in {ChatMemberStatus.OWNER, ChatMemberStatus.ADMINISTRATOR}:
+                return  # ignore command from admins
+        except UserNotParticipant:
+            pass  # keep going when user is not a member
+
+        if not message.reply_to_message:
+            await message.reply(await self.text(chat.id, "no-report-user"))
             return
 
-        await self.reply_filter(message, set(chat_trigger), text)
+        reported_user = message.reply_to_message.from_user
+        if not reported_user:  # Do nothing here, big chances are anonymous admins
+            return
 
-    async def reply_filter(self, message: Message, trigger: Set[str], text: str):
-        if not text or text.startswith("/filter") or text.startswith("/stop"):
-            return  # Igonore when command triggered
-        for i in trigger:
-            pattern = r"( |^|[^\w])" + re.escape(i) + r"( |$|[^\w])"
-            if re.search(pattern, text, flags=re.IGNORECASE):
-                filt = await self.get_filter(message.chat.id, i)
-                if not filt:
-                    return
+        if reported_user.id == self.bot.uid:
+            await message.reply_text(await self.text(chat.id, "cant-report-me"))
+            return
+        if reported_user.id == message.from_user.id:
+            await message.reply_text(await self.text(chat.id, "cant-self-report"))
+            return
 
-                await message.reply_text(filt)
-                break
+        try:
+            member = await chat.get_member(reported_user.id)
+        except UserNotParticipant:
+            await message.reply_text(await self.text(chat.id, "user-not-in-chat"))
+            return
 
-    async def get_filter(self, chat_id: int, keyword: str) -> Optional[str]:
-        data = await self.db.find_one(
-            {"chat_id": chat_id, f"trigger.{keyword}": {"$exists": True}},
-            {f"trigger.{keyword}": 1},
-        )
-        return data["trigger"][keyword] if data else None
+        if util.tg.is_staff_or_admin(member):
+            await message.reply_text(await self.text(chat.id, "cant-report-admin"))
+            return
 
-    async def save_filter(self, chat_id: int, keyword: str, content: str):
-        await self.db.update_one(
-            {"chat_id": chat_id}, {"$set": {f"trigger.{keyword}": content}}, upsert=True
-        )
+        reply_text = await self.text(chat.id, "report-notif", reported_user.mention)
+        slots = 4096 - len(reply_text)
+        async for admin in util.tg.get_chat_admins(self.bot.client, chat.id, exclude_bot=True):
+            if await self.is_active(admin.user.id, True):
+                reply_text += f"[\u200b](tg://user?id={admin.user.id})"
 
-        if self.trigger.get(chat_id):
-            self.trigger[chat_id].add(keyword)
-        else:
-            self.trigger[chat_id] = set(keyword)
+            slots -= 1
+            if slots == 0:
+                break
 
-    async def del_filter(self, chat_id: int, keyword: str) -> Tuple[bool, str]:
-        filt = self.trigger.get(chat_id)
-        if not filt:
-            return False, await self.text(chat_id, "filters-chat-nofilter")
-        if keyword not in filt:
-            return False, await self.text(chat_id, "filters-chat-nokeyword", keyword)
+        await message.reply_text(reply_text)
 
-        await self.db.update_one(
-            {"chat_id": chat_id},
-            {"$unset": {f"trigger.{keyword}": ""}},
-        )
-        self.trigger[chat_id].remove(keyword)
-        return True, ""
+    async def setting(self, chat_id: int, is_private: bool, setting: bool) -> None:
+        if is_private:
+            if setting:
+                await self.user_db.update_one(
+                    {"_id": chat_id}, {"$set": {"setting": True}}, upsert=True
+                )
+            else:
+                await self.user_db.delete_one({"_id": chat_id})
+        else:
+            if setting:
+                await self.db.update_one(
+                    {"chat_id": chat_id}, {"$set": {"setting": True}}, upsert=True
+                )
+            else:
+                await self.db.delete_one({"chat_id": chat_id})
+
+    async def is_active(self, uid: int, is_private: bool) -> bool:
+        """Get current setting default to True"""
+        if is_private:
+            data = await self.user_db.find_one({"_id": uid})
+        else:
+            data = await self.db.find_one({"chat_id": uid})
+        if not data:
+            return True
 
-    @command.filters(filters.admin_only)
-    async def cmd_filter(self, ctx: command.Context, trigger: str, *, text: str) -> str:
-        if not trigger or not text:
-            return await self.text(ctx.chat.id, "filter-help")
+        return data.get("setting", True)
 
-        await self.save_filter(ctx.chat.id, trigger, text)
-        return await self.text(ctx.chat.id, "filters-added", trigger)
+    @command.filters(filters.group)
+    async def cmd_report(self, ctx: command.Context) -> None:
+        return await self.on_message(ctx.message)
 
     @command.filters(filters.admin_only)
-    async def cmd_stop(self, ctx: command.Context, trigger: str) -> str:
-        if not trigger:
-            return await self.text(ctx.chat.id, "filter-stop-help")
-
-        deleted, out = await self.del_filter(ctx.chat.id, trigger)
-        if not deleted:
-            return out
-
-        return await self.text(ctx.chat.id, "filters-removed", trigger)
-
-    @command.filters(filters.admin_only, aliases=["rmallfilters"])
-    async def cmd_rmallfilter(self, ctx: command.Context) -> str:
-        chat_id = ctx.chat.id
-        triggers = self.trigger.pop(chat_id, None)
-        if not triggers:
-            return await self.text(chat_id, "filters-chat-nofilter")
-        await self.db.delete_one({"chat_id": chat_id})
-        return await self.text(chat_id, "filters-rmall", len(triggers))
+    async def cmd_reports(
+        self, ctx: command.Context, setting: Optional[bool] = None
+    ) -> Optional[str]:
+        """Report setting command"""
+        if ctx.msg.reply_to_message:
+            return None
+
+        chat = ctx.chat
+        private = chat.type == ChatType.PRIVATE
+
+        if setting is None:
+            if not ctx.input:
+                return await self.text(
+                    chat.id,
+                    "report-setting" if private else "chat-report-setting",
+                    await self.is_active(chat.id, private),
+                )
+
+            return await self.text(chat.id, "err-yes-no-args")
+
+        _, member = await util.tg.fetch_permissions(self.bot.client, chat.id, ctx.author.id)
+        if not member or member.status not in {
+            ChatMemberStatus.ADMINISTRATOR,
+            ChatMemberStatus.OWNER,
+        }:
+            return None
 
-    @command.filters(filters.admin_only)
-    async def cmd_filters(self, ctx: command.Context) -> str:
-        data = self.trigger.get(ctx.chat.id)
-        if not data:
-            return await self.text(ctx.chat.id, "filters-chat-nofilter")
+        if setting is True:
+            text = "report-on" if private else "chat-report-on"
+        else:
+            text = "report-off" if private else "chat-report-off"
 
-        output = await self.text(ctx.chat.id, "filters-list", ctx.chat.title)
-        output += "\n".join([f"× `{i}`" for i in sorted(data)])
-        return output
+        ret, _ = await asyncio.gather(
+            self.text(chat.id, text),
+            self.setting(chat.id, private, setting),
+        )
+        return ret
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `anjani-2.8.1/anjani/plugins/language.py` & `anjani-2.9.0/anjani/plugins/language.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/lockings.py` & `anjani-2.9.0/anjani/plugins/lockings.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/main.py` & `anjani-2.9.0/anjani/plugins/main.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/misc.py` & `anjani-2.9.0/anjani/plugins/misc.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/muting.py` & `anjani-2.9.0/anjani/plugins/muting.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/notes.py` & `anjani-2.9.0/anjani/plugins/notes.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/purge.py` & `anjani-2.9.0/anjani/plugins/purge.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/restriction.py` & `anjani-2.9.0/anjani/plugins/restriction.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
             target = reply_msg.from_user or reply_msg.sender_chat
             reason = ctx.input
 
         try:
             if isinstance(target, User) and util.tg.is_staff_or_admin(
                 await chat.get_member(target.id)
             ):
-                return await self.text(chat.id, "admin-kick")
+                return await self.text(chat.id, "admin-ban")
         except UserNotParticipant:
             # Not a participant in the chat (replying from channel discussion)
             if util.tg.is_staff(target.id):
                 return await self.text(chat.id, "admin-ban")
 
         ret, _ = await asyncio.gather(
             self.text(
```

### Comparing `anjani-2.8.1/anjani/plugins/rules.py` & `anjani-2.9.0/anjani/plugins/rules.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/spam_prediction.py` & `anjani-2.9.0/anjani/plugins/spam_prediction.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     helpable: ClassVar[bool] = True
     disabled: ClassVar[bool] = not _run_predict or not token
 
     db: util.db.AsyncCollection
     user_db: util.db.AsyncCollection
     setting_db: util.db.AsyncCollection
     model: Pipeline
-    __min_reputation: int = 300
+    __predict_cost: int = 10
 
     async def on_load(self) -> None:
         self.db = self.bot.db.get_collection("SPAM_DUMP")
         self.user_db = self.bot.db.get_collection("USERS")
         self.setting_db = self.bot.db.get_collection("SPAM_PREDICT_SETTING")
 
         await self.__load_model()
@@ -404,15 +404,15 @@
         text = text.strip()
         try:
             user = message.from_user.id
         except AttributeError:
             user = None
 
         text_norm = self._normalize_text(text)
-        if len(text_norm.split()) < 5:  # Skip short messages
+        if len(text_norm.split()) < 4:  # Skip short messages
             return
 
         response = await self._predict(text_norm)
         if response.size == 0:
             return
 
         probability = response[0][1]
@@ -699,20 +699,20 @@
     async def cmd_predict(self, ctx: command.Context) -> Optional[str]:
         """Look a prediction for a replied message"""
         chat = ctx.chat
         user = await self.user_db.find_one({"_id": ctx.author.id})
         if not user:
             return None
 
-        if user.get("reputation", 0) < self.__min_reputation:
+        if user.get("reputation", 0) < self.__predict_cost:
             return await self.text(
                 chat.id,
                 "spampredict-unauthorized",
                 user.get("reputation", 0),
-                self.__min_reputation,
+                self.__predict_cost,
             )
 
         replied = ctx.msg.reply_to_message
         if not replied:
             await ctx.respond(await ctx.get_text("error-reply-to-message"), delete_after=5)
             return None
 
@@ -736,14 +736,18 @@
                         f"**Ham Prediction**: `{self.prob_to_string(ocr_prediction[0][0])}`\n\n"
                     )
                     # Return early if content is empty, so error message not shown
                     if not content:
                         await asyncio.gather(
                             self.bot.log_stat("predicted"),
                             ctx.respond(photo_prediction),
+                            self.user_db.update_one(
+                                {"_id": ctx.author.id},
+                                {"$inc": {"reputation": -self.__predict_cost}},
+                            ),
                         )
                         return None
             else:
                 photo_prediction = await ctx.get_text("spampredict-photo-failed")
 
         if not content:
             return await ctx.get_text("spampredict-empty")
@@ -762,14 +766,17 @@
             self.bot.log_stat("predicted"),
             ctx.respond(
                 photo_prediction + "**Result Caption Text**\n\n" + textPrediction
                 if photo_prediction
                 else "**Result**\n\n" + textPrediction,
                 reply_to_message_id=None if replied.photo else replied.id,
             ),
+            self.user_db.update_one(
+                {"_id": ctx.author.id}, {"$inc": {"reputation": -self.__predict_cost}}
+            ),
         )
         return None
 
     async def setting(self, chat_id: int, setting: bool) -> None:
         """Turn on/off spam prediction in chats"""
         await self.setting_db.update_one(
             {"chat_id": chat_id}, {"$set": {"setting": setting}}, upsert=True
```

### Comparing `anjani-2.8.1/anjani/plugins/spam_shield.py` & `anjani-2.9.0/anjani/plugins/spam_shield.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/staff_tools.py` & `anjani-2.9.0/anjani/plugins/staff_tools.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/stats.py` & `anjani-2.9.0/anjani/plugins/stats.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/plugins/users.py` & `anjani-2.9.0/anjani/plugins/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 
         if user.is_scam:
             text += "<b>\n⚠️Warning this user is flagged as a scammer by Telegram⚠️</b>\n"
 
         user_db = await self.users_db.find_one({"_id": user.id})
         if user_db and self.predict_loaded:
             if user_db.get("spam", False):
-                text += "<b>\n⚠️Warning I flag this user as a scammer⚠️</b>\n"
+                text += "<b>\n⚠️Warning I flag this user as a spammer⚠️</b>\n"
 
             text += f"\n<b>Identifier:</b> <code>{user_db.get('hash', 'unknown')}</code>"
             text += f"\n<b>Reputation:</b> <code>{user_db.get('reputation', 0)}</code>"
             trust = get_trust(user_db.get("pred_sample", []))
             if trust:
                 text += f"\n<b>Trust:</b> <code>{trust:.2f}</code>"
             else:
```

### Comparing `anjani-2.8.1/anjani/plugins/welcome.py` & `anjani-2.9.0/anjani/plugins/welcome.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/__init__.py` & `anjani-2.9.0/anjani/util/__init__.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/async_helper.py` & `anjani-2.9.0/anjani/util/async_helper.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/config.py` & `anjani-2.9.0/anjani/util/config.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/converter.py` & `anjani-2.9.0/anjani/util/converter.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/db/__init__.py` & `anjani-2.9.0/anjani/util/db/__init__.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/db/base.py` & `anjani-2.9.0/anjani/util/db/base.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/db/change_stream.py` & `anjani-2.9.0/anjani/util/db/change_stream.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/db/client.py` & `anjani-2.9.0/anjani/util/db/client.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/db/client_session.py` & `anjani-2.9.0/anjani/util/db/client_session.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/db/collection.py` & `anjani-2.9.0/anjani/util/db/collection.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/db/command_cursor.py` & `anjani-2.9.0/anjani/util/db/command_cursor.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/db/cursor.py` & `anjani-2.9.0/anjani/util/db/cursor.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/db/cursor_base.py` & `anjani-2.9.0/anjani/util/db/cursor_base.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/db/db.py` & `anjani-2.9.0/anjani/util/db/db.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/db/errors.py` & `anjani-2.9.0/anjani/util/db/errors.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/db/typings.py` & `anjani-2.9.0/anjani/util/db/typings.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/error.py` & `anjani-2.9.0/anjani/util/error.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/misc.py` & `anjani-2.9.0/anjani/util/misc.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/system.py` & `anjani-2.9.0/anjani/util/system.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/tg.py` & `anjani-2.9.0/anjani/util/tg.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/time.py` & `anjani-2.9.0/anjani/util/time.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/anjani/util/types.py` & `anjani-2.9.0/anjani/util/types.py`

 * *Files identical despite different names*

### Comparing `anjani-2.8.1/pyproject.toml` & `anjani-2.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anjani"
-version = "2.8.1"
+version = "2.9.0"
 description = "Telegram group management bot"
 license = "GPL-3.0-or-later"
 authors = [
     "Gaung Ramadhan <hi@mrmiss.my.id>",
     "Adek Maulana <adekzmaulana@gmail.com>"
 ]
 readme = "README.md"
```

### Comparing `anjani-2.8.1/setup.py` & `anjani-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  'uvloop:sys_platform == "linux"': ['uvloop>=0.17.0,<0.18.0']}
 
 entry_points = \
 {'console_scripts': ['anjani = anjani.main:start']}
 
 setup_kwargs = {
     'name': 'anjani',
-    'version': '2.8.1',
+    'version': '2.9.0',
     'description': 'Telegram group management bot',
     'long_description': "# Anjani\n\n[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)\n\n[![DeepSource](https://deepsource.io/gh/userbotindo/Anjani.svg/?label=active+issues)](https://deepsource.io/gh/userbotindo/Anjani/?ref=repository-badge)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/23d2794692ad47a18849e06823aeaf6f)](https://www.codacy.com/gh/userbotindo/Anjani/dashboard?utm_source=github.com&utm_medium=referral&utm_content=userbotindo/Anjani&utm_campaign=Badge_Grade)\n\nCan be found on Telegram as [Anjani](https://t.me/dAnjani_bot).\n\nAnjani is a modern, easy-to-develop, fully async Telegram group managing bot for Telegram.\n\n## Requirements\n\n-   Python 3.9 or higher.\n-   [Telegram API key](https://docs.pyrogram.org/intro/setup#api-keys).\n-   [Telegram Bot Token](https://t.me/botfather)\n-   [MongoDB Database](https://cloud.mongodb.com/).\n\n## Features\n\n-   Easy to develop with object oriented models.\n-   Fully asynchronous with async / await.\n-   Type-hinted method making it easy to create plugins.\n-   Localization support.\n-   Class based plugin system.\n\n## [Documentation](https://userbotindo.com/anjani/docs/home)\n\n## [Installing](https://userbotindo.com/anjani/docs/install)\n\n## Plugin\n\nIf you want to make your custom plugins, refer to [Anjani's Plugins Guide](https://userbotindo.com/anjani/docs/plugin/creating-your-own-plugin).\n\n## Credits\n\n-   [Marie](https://github.com/PaulSonOfLars/tgbot)\n-   [Pyrobud](https://github.com/kdrag0n/pyrobud)\n-   [All Contributors 👥](https://github.com/userbotindo/Anjani/graphs/contributors)\n",
     'author': 'Gaung Ramadhan',
     'author_email': 'hi@mrmiss.my.id',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/userbotindo/anjani#readme',
```

### Comparing `anjani-2.8.1/PKG-INFO` & `anjani-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anjani
-Version: 2.8.1
+Version: 2.9.0
 Summary: Telegram group management bot
 Home-page: https://github.com/userbotindo/anjani#readme
 License: GPL-3.0-or-later
 Keywords: chatbot,bot,python,telegram-bot,pyrogram
 Author: Gaung Ramadhan
 Author-email: hi@mrmiss.my.id
 Requires-Python: >=3.9,<=3.11
```

