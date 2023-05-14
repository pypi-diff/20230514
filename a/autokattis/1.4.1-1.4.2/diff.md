# Comparing `tmp/autokattis-1.4.1.tar.gz` & `tmp/autokattis-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autokattis-1.4.1.tar", last modified: Thu May 11 11:23:06 2023, max compression
+gzip compressed data, was "autokattis-1.4.2.tar", last modified: Sun May 14 10:58:30 2023, max compression
```

## Comparing `autokattis-1.4.1.tar` & `autokattis-1.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-11 11:23:06.968742 autokattis-1.4.1/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    35148 2023-05-04 07:45:56.000000 autokattis-1.4.1/LICENSE
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2580 2023-05-11 11:23:06.966265 autokattis-1.4.1/PKG-INFO
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2226 2023-05-11 09:23:16.000000 autokattis-1.4.1/README.md
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-11 11:23:06.858511 autokattis-1.4.1/autokattis/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       24 2023-05-11 09:21:05.000000 autokattis-1.4.1/autokattis/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-11 11:23:06.948409 autokattis-1.4.1/autokattis/api/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    21653 2023-05-11 09:21:15.000000 autokattis-1.4.1/autokattis/api/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-11 11:23:06.952473 autokattis-1.4.1/autokattis/database/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)   133880 2023-05-08 08:31:18.000000 autokattis-1.4.1/autokattis/database/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-11 11:23:06.960671 autokattis-1.4.1/autokattis/scraper/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       37 2023-05-11 07:47:42.000000 autokattis-1.4.1/autokattis/scraper/__init__.py
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     3031 2023-05-11 07:45:04.000000 autokattis-1.4.1/autokattis/scraper/country.py
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      977 2023-05-11 07:45:16.000000 autokattis-1.4.1/autokattis/scraper/university.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-11 11:23:06.964169 autokattis-1.4.1/autokattis/utils/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      518 2023-05-11 07:23:19.000000 autokattis-1.4.1/autokattis/utils/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-11 11:23:06.945490 autokattis-1.4.1/autokattis.egg-info/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2580 2023-05-11 11:23:06.000000 autokattis-1.4.1/autokattis.egg-info/PKG-INFO
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      400 2023-05-11 11:23:06.000000 autokattis-1.4.1/autokattis.egg-info/SOURCES.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)        1 2023-05-11 11:23:06.000000 autokattis-1.4.1/autokattis.egg-info/dependency_links.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       80 2023-05-11 11:23:06.000000 autokattis-1.4.1/autokattis.egg-info/requires.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       11 2023-05-11 11:23:06.000000 autokattis-1.4.1/autokattis.egg-info/top_level.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       38 2023-05-11 11:23:06.969106 autokattis-1.4.1/setup.cfg
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      878 2023-05-11 11:22:31.000000 autokattis-1.4.1/setup.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 10:58:30.663660 autokattis-1.4.2/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    35148 2023-05-04 07:45:56.000000 autokattis-1.4.2/LICENSE
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2580 2023-05-14 10:58:30.662660 autokattis-1.4.2/PKG-INFO
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2226 2023-05-11 09:23:16.000000 autokattis-1.4.2/README.md
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 10:58:30.620660 autokattis-1.4.2/autokattis/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       24 2023-05-11 09:21:05.000000 autokattis-1.4.2/autokattis/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 10:58:30.651657 autokattis-1.4.2/autokattis/api/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    22006 2023-05-14 10:57:37.000000 autokattis-1.4.2/autokattis/api/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 10:58:30.653658 autokattis-1.4.2/autokattis/database/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)   133880 2023-05-08 08:31:18.000000 autokattis-1.4.2/autokattis/database/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 10:58:30.659657 autokattis-1.4.2/autokattis/scraper/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       37 2023-05-11 07:47:42.000000 autokattis-1.4.2/autokattis/scraper/__init__.py
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     3031 2023-05-11 07:45:04.000000 autokattis-1.4.2/autokattis/scraper/country.py
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      977 2023-05-11 07:45:16.000000 autokattis-1.4.2/autokattis/scraper/university.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 10:58:30.661665 autokattis-1.4.2/autokattis/utils/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      518 2023-05-11 07:23:19.000000 autokattis-1.4.2/autokattis/utils/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 10:58:30.649658 autokattis-1.4.2/autokattis.egg-info/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2580 2023-05-14 10:58:30.000000 autokattis-1.4.2/autokattis.egg-info/PKG-INFO
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      400 2023-05-14 10:58:30.000000 autokattis-1.4.2/autokattis.egg-info/SOURCES.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)        1 2023-05-14 10:58:30.000000 autokattis-1.4.2/autokattis.egg-info/dependency_links.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       80 2023-05-14 10:58:30.000000 autokattis-1.4.2/autokattis.egg-info/requires.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       11 2023-05-14 10:58:30.000000 autokattis-1.4.2/autokattis.egg-info/top_level.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       38 2023-05-14 10:58:30.663660 autokattis-1.4.2/setup.cfg
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      878 2023-05-14 10:36:19.000000 autokattis-1.4.2/setup.py
```

### Comparing `autokattis-1.4.1/LICENSE` & `autokattis-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.1/PKG-INFO` & `autokattis-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autokattis
-Version: 1.4.1
+Version: 1.4.2
 Summary: Updated Kattis API wrapper
 Home-page: https://github.com/RussellDash332/autokattis
 Download-URL: https://pypi.org/project/autokattis/
 Author: Russell Saerang
 Author-email: russellsaerang@gmail.com
 License: MIT
 Keywords: Kattis
```

### Comparing `autokattis-1.4.1/README.md` & `autokattis-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.1/autokattis/api/__init__.py` & `autokattis-1.4.2/autokattis/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 import requests
 import seaborn as sns
 import warnings
 import zipfile
 
 from bs4 import BeautifulSoup as bs
+from collections import Counter
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from ..database import LANGUAGES, COUNTRIES, UNIVERSITIES
 from ..utils import guess_id
 
 warnings.warn = lambda *args, **kwargs: None # suppress warnings
 
 class Kattis(requests.Session):
@@ -41,18 +42,27 @@
             'user': self.user,
             'password': self.password
         }
         response = self.post(f'{self.BASE_URL}/login/email', data=data)
         assert response.ok, 'Cannot login to Kattis'
         print('Logged in to Kattis!', flush=True)
 
-        self.homepage = response.text
-        regex_result = re.findall(r'/users/([^/]+)/settings', self.homepage)
-        assert len(regex_result) == 1, f'Regex found several possible usernames, {regex_result}'
-        self.user = regex_result[0]
+        self.homepage = bs(response.content, features='lxml')
+        names = []
+        for a in self.homepage.find_all('a'):
+            href = a.get('href')
+            if href:
+                paths = href.split('/')
+                if len(paths) > 2 and paths[1] == 'users':
+                    names.append(paths[2])
+        ctr = Counter(names)
+        max_freq = max(ctr.values())
+        candidate_usernames = [name for name in ctr if ctr[name] == max_freq]
+        print(f'Candidate username(s): {candidate_usernames}')
+        self.user = candidate_usernames[0]
 
     def problems(self, show_solved=True, show_partial=True, show_tried=False, show_untried=False):
         '''
         Gets all Kattis problems based on some filters.
         Returns a JSON-like structure with these fields:
             name, fastest, shortest, total, acc, difficulty, category, link
 
@@ -301,15 +311,15 @@
 
     def suggest(self):
         '''
         Retrieves suggested problems based on what you have solved so far.
         Returns a JSON-like structure containing the suggested problems points and its difficulty.
         '''
 
-        soup = bs(self.homepage, features='lxml')
+        soup = self.homepage
         table = soup.find_all('table', class_='table2 report_grid-problems_table')[0]
         data = []
         for row in table.tbody.find_all('tr'):
             header = row.find('th')
             if header:
                 difficulty = header.text
             column = row.find('td')
@@ -330,21 +340,21 @@
 
         Default: ranklist of people around you.
         '''
 
         assert country == None or university == None, 'Both of country and university cannot be given at the same time!'
 
         if country == university == None:
-            soup = bs(self.homepage, features='lxml')
+            soup = self.homepage
             table = soup.find_all('table', class_='table2 report_grid-problems_table')[1]
             data = []
             for row in table.tbody.find_all('tr'):
                 columns = row.find_all('td')
                 rank, name, pts, *_ = [column.text.strip() for column in columns]
-                rank = int(rank)
+                rank = int(rank) if rank.isdigit() else None
                 pts = float(re.findall(r'[\d\.]+', pts)[0])
                 findall = columns[1].find_all('a')
 
                 new_data = {
                     'rank': rank,
                     'name': name,
                     'points': pts,
```

### Comparing `autokattis-1.4.1/autokattis/database/__init__.py` & `autokattis-1.4.2/autokattis/database/__init__.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.1/autokattis/scraper/country.py` & `autokattis-1.4.2/autokattis/scraper/country.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.1/autokattis/scraper/university.py` & `autokattis-1.4.2/autokattis/scraper/university.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.1/autokattis/utils/__init__.py` & `autokattis-1.4.2/autokattis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.1/autokattis.egg-info/PKG-INFO` & `autokattis-1.4.2/autokattis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autokattis
-Version: 1.4.1
+Version: 1.4.2
 Summary: Updated Kattis API wrapper
 Home-page: https://github.com/RussellDash332/autokattis
 Download-URL: https://pypi.org/project/autokattis/
 Author: Russell Saerang
 Author-email: russellsaerang@gmail.com
 License: MIT
 Keywords: Kattis
```

### Comparing `autokattis-1.4.1/setup.py` & `autokattis-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='autokattis',
-    version='1.4.1',
+    version='1.4.2',
     description='Updated Kattis API wrapper',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Russell Saerang',
     author_email='russellsaerang@gmail.com',
```

