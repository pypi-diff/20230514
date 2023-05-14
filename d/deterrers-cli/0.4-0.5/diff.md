# Comparing `tmp/deterrers-cli-0.4.tar.gz` & `tmp/deterrers-cli-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deterrers-cli-0.4.tar", last modified: Thu Apr 20 14:03:30 2023, max compression
+gzip compressed data, was "deterrers-cli-0.5.tar", last modified: Sun May 14 17:57:16 2023, max compression
```

## Comparing `deterrers-cli-0.4.tar` & `deterrers-cli-0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-20 14:03:30.405842 deterrers-cli-0.4/
--rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 21:11:45.000000 deterrers-cli-0.4/LICENSE
--rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 21:06:33.000000 deterrers-cli-0.4/MANIFEST.in
--rw-r--r--   0 lars      (1000) lars      (1000)     2178 2023-04-20 14:03:30.405842 deterrers-cli-0.4/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)     1908 2023-04-17 13:28:29.000000 deterrers-cli-0.4/README.md
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-20 14:03:30.405842 deterrers-cli-0.4/deterrers_cli.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)     2178 2023-04-20 14:03:30.000000 deterrers-cli-0.4/deterrers_cli.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      304 2023-04-20 14:03:30.000000 deterrers-cli-0.4/deterrers_cli.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-20 14:03:30.000000 deterrers-cli-0.4/deterrers_cli.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       61 2023-04-20 14:03:30.000000 deterrers-cli-0.4/deterrers_cli.egg-info/entry_points.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       32 2023-04-20 14:03:30.000000 deterrers-cli-0.4/deterrers_cli.egg-info/requires.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-20 14:03:30.000000 deterrers-cli-0.4/deterrers_cli.egg-info/top_level.txt
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-20 14:03:30.405842 deterrers-cli-0.4/deterrerscli/
--rw-r--r--   0 lars      (1000) lars      (1000)     2649 2023-04-20 14:00:49.000000 deterrers-cli-0.4/deterrerscli/__main__.py
--rw-r--r--   0 lars      (1000) lars      (1000)       32 2023-04-20 13:51:57.000000 deterrers-cli-0.4/requirements.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-20 14:03:30.405842 deterrers-cli-0.4/setup.cfg
--rw-r--r--   0 lars      (1000) lars      (1000)      782 2023-04-20 13:51:57.000000 deterrers-cli-0.4/setup.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-05-14 17:57:16.178369 deterrers-cli-0.5/
+-rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 21:11:45.000000 deterrers-cli-0.5/LICENSE
+-rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 21:06:33.000000 deterrers-cli-0.5/MANIFEST.in
+-rw-r--r--   0 lars      (1000) lars      (1000)     2178 2023-05-14 17:57:16.178369 deterrers-cli-0.5/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)     1908 2023-04-17 13:28:29.000000 deterrers-cli-0.5/README.md
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-05-14 17:57:16.178369 deterrers-cli-0.5/deterrers_cli.egg-info/
+-rw-r--r--   0 lars      (1000) lars      (1000)     2178 2023-05-14 17:57:16.000000 deterrers-cli-0.5/deterrers_cli.egg-info/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      326 2023-05-14 17:57:16.000000 deterrers-cli-0.5/deterrers_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-05-14 17:57:16.000000 deterrers-cli-0.5/deterrers_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       61 2023-05-14 17:57:16.000000 deterrers-cli-0.5/deterrers_cli.egg-info/entry_points.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       32 2023-05-14 17:57:16.000000 deterrers-cli-0.5/deterrers_cli.egg-info/requires.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-05-14 17:57:16.000000 deterrers-cli-0.5/deterrers_cli.egg-info/top_level.txt
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-05-14 17:57:16.178369 deterrers-cli-0.5/deterrerscli/
+-rw-r--r--   0 lars      (1000) lars      (1000)     2787 2023-05-14 17:56:05.000000 deterrers-cli-0.5/deterrerscli/__main__.py
+-rw-r--r--   0 lars      (1000) lars      (1000)      631 2023-05-14 17:56:05.000000 deterrers-cli-0.5/deterrerscli/types.py
+-rw-r--r--   0 lars      (1000) lars      (1000)       32 2023-04-20 13:51:57.000000 deterrers-cli-0.5/requirements.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-05-14 17:57:16.178369 deterrers-cli-0.5/setup.cfg
+-rw-r--r--   0 lars      (1000) lars      (1000)      782 2023-05-14 17:56:05.000000 deterrers-cli-0.5/setup.py
```

### Comparing `deterrers-cli-0.4/LICENSE` & `deterrers-cli-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deterrers-cli-0.4/PKG-INFO` & `deterrers-cli-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deterrers-cli
-Version: 0.4
+Version: 0.5
 Summary: Command line client for DETERRERS
 Home-page: https://github.com/virtUOS/proteuscmd
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `deterrers-cli-0.4/README.md` & `deterrers-cli-0.5/README.md`

 * *Files identical despite different names*

### Comparing `deterrers-cli-0.4/deterrers_cli.egg-info/PKG-INFO` & `deterrers-cli-0.5/deterrers_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deterrers-cli
-Version: 0.4
+Version: 0.5
 Summary: Command line client for DETERRERS
 Home-page: https://github.com/virtUOS/proteuscmd
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `deterrers-cli-0.4/deterrerscli/__main__.py` & `deterrers-cli-0.5/deterrerscli/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import click
 import deterrersapi
-import pathlib
 import json
+import pathlib
 import yaml
 
+from deterrerscli.types import IPV4_TYPE
+
 deterrers = None
 
 profiles = click.Choice(
         ('', 'HTTP', 'SSH', 'HTTP+SSH', 'Multipurpose'),
         case_sensitive=False)
 host_firewalls = click.Choice(
         ('', 'UFW', 'FirewallD', 'nftables'),
@@ -36,46 +38,46 @@
     '''
     data = deterrers.hosts()
     print_format(data, format)
 
 
 @cli.command()
 @click.option('--format', default='json', help='Output format (json or yaml)')
-@click.argument('ipv4')
+@click.argument('ipv4', type=IPV4_TYPE)
 def get(format, ipv4):
     '''Get information about an IP address in DETERRERS.
     '''
     data = deterrers.get(ipv4)
     print_format(data, format)
 
 
 @cli.command()
-@click.argument('ipv4')
+@click.argument('ipv4', type=IPV4_TYPE)
 def delete(ipv4):
     '''Delete IP address from DETERRERS.
     '''
     deterrers.delete(ipv4)
 
 
 @cli.command()
 @click.option('--admin', '-a', multiple=True, required=True)
 @click.option('--profile', '-p', default='', type=profiles)
 @click.option('--firewall', '-f', default='', type=host_firewalls)
-@click.argument('ipv4')
+@click.argument('ipv4', type=IPV4_TYPE)
 def add(ipv4, admin, profile, firewall):
     '''Add IP address to DETERRERS.
     '''
     deterrers.add(ipv4, admin, profile, firewall)
 
 
 @cli.command()
 @click.option('--admin', '-a', default=None, multiple=True)
 @click.option('--profile', '-p', default=None, type=profiles)
 @click.option('--firewall', '-f', default=None, type=host_firewalls)
-@click.argument('ipv4')
+@click.argument('ipv4', type=IPV4_TYPE)
 def update(ipv4, admin, profile, firewall):
     '''Update IP address in DETERRERS.
 
     Fields which are not specified will not be changed.
     The option `admin` can be used multiple times.
     '''
     admin = admin or None
@@ -86,23 +88,23 @@
 def action():
     '''Activate firewall profile or block IP address in perimeter firewall.
     '''
     pass
 
 
 @action.command()
-@click.argument('ipv4')
+@click.argument('ipv4', type=IPV4_TYPE)
 def register(ipv4):
     '''Activate profile in perimeter firewall.
     '''
     deterrers.action(ipv4, 'register')
 
 
 @action.command()
-@click.argument('ipv4')
+@click.argument('ipv4', type=IPV4_TYPE)
 def block(ipv4):
     '''Block IP address perimeter firewall.
     '''
     deterrers.action(ipv4, 'block')
 
 
 if __name__ == '__main__':
```

### Comparing `deterrers-cli-0.4/setup.py` & `deterrers-cli-0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     path = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(path, filename), encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='deterrers-cli',
-    version='0.4',
+    version='0.5',
     description='Command line client for DETERRERS',
     url='https://github.com/virtUOS/proteuscmd',
     author='Lars Kiesow',
     author_email='lkiesow@uos.de',
     license='MIT',
     packages=['deterrerscli'],
     license_files=('LICENSE'),
```

