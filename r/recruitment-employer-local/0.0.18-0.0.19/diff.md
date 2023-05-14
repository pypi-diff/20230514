# Comparing `tmp/recruitment-employer-local-0.0.18.tar.gz` & `tmp/recruitment-employer-local-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recruitment-employer-local-0.0.18.tar", last modified: Sun May 14 20:34:39 2023, max compression
+gzip compressed data, was "recruitment-employer-local-0.0.19.tar", last modified: Sun May 14 20:46:25 2023, max compression
```

## Comparing `recruitment-employer-local-0.0.18.tar` & `recruitment-employer-local-0.0.19.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:34:39.443374 recruitment-employer-local-0.0.18/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:34:39.443374 recruitment-employer-local-0.0.18/CirclesVacanciesScrapers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 20:34:24.000000 recruitment-employer-local-0.0.18/CirclesVacanciesScrapers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-14 20:34:24.000000 recruitment-employer-local-0.0.18/CirclesVacanciesScrapers/database_vacancies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-14 20:34:24.000000 recruitment-employer-local-0.0.18/CirclesVacanciesScrapers/indeed_com_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-14 20:34:24.000000 recruitment-employer-local-0.0.18/CirclesVacanciesScrapers/monster_com_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-14 20:34:39.443374 recruitment-employer-local-0.0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 20:34:24.000000 recruitment-employer-local-0.0.18/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-14 20:34:24.000000 recruitment-employer-local-0.0.18/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:34:39.443374 recruitment-employer-local-0.0.18/recruitment_employer_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-14 20:34:39.000000 recruitment-employer-local-0.0.18/recruitment_employer_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-14 20:34:39.000000 recruitment-employer-local-0.0.18/recruitment_employer_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:34:39.000000 recruitment-employer-local-0.0.18/recruitment_employer_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 20:34:39.000000 recruitment-employer-local-0.0.18/recruitment_employer_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:34:39.443374 recruitment-employer-local-0.0.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-14 20:34:24.000000 recruitment-employer-local-0.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:46:25.101202 recruitment-employer-local-0.0.19/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:46:25.101202 recruitment-employer-local-0.0.19/CirclesVacanciesScrapers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 20:46:14.000000 recruitment-employer-local-0.0.19/CirclesVacanciesScrapers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-14 20:46:14.000000 recruitment-employer-local-0.0.19/CirclesVacanciesScrapers/database_vacancies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-14 20:46:14.000000 recruitment-employer-local-0.0.19/CirclesVacanciesScrapers/indeed_com_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-14 20:46:14.000000 recruitment-employer-local-0.0.19/CirclesVacanciesScrapers/monster_com_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-14 20:46:25.101202 recruitment-employer-local-0.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 20:46:14.000000 recruitment-employer-local-0.0.19/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-14 20:46:14.000000 recruitment-employer-local-0.0.19/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:46:25.101202 recruitment-employer-local-0.0.19/recruitment_employer_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-14 20:46:25.000000 recruitment-employer-local-0.0.19/recruitment_employer_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-14 20:46:25.000000 recruitment-employer-local-0.0.19/recruitment_employer_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:46:25.000000 recruitment-employer-local-0.0.19/recruitment_employer_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 20:46:25.000000 recruitment-employer-local-0.0.19/recruitment_employer_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:46:25.101202 recruitment-employer-local-0.0.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-14 20:46:14.000000 recruitment-employer-local-0.0.19/setup.py
```

### Comparing `recruitment-employer-local-0.0.18/CirclesVacanciesScrapers/database_vacancies.py` & `recruitment-employer-local-0.0.19/CirclesVacanciesScrapers/database_vacancies.py`

 * *Files identical despite different names*

### Comparing `recruitment-employer-local-0.0.18/CirclesVacanciesScrapers/indeed_com_scraper.py` & `recruitment-employer-local-0.0.19/CirclesVacanciesScrapers/indeed_com_scraper.py`

 * *Files identical despite different names*

### Comparing `recruitment-employer-local-0.0.18/CirclesVacanciesScrapers/monster_com_scraper.py` & `recruitment-employer-local-0.0.19/CirclesVacanciesScrapers/monster_com_scraper.py`

 * *Files identical despite different names*

### Comparing `recruitment-employer-local-0.0.18/setup.py` & `recruitment-employer-local-0.0.19/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='recruitment-employer-local',
-     version='0.0.18',
+     version='0.0.19',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local recruitment scrapers Python",
      long_description="This is a package for sharing common Logger function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

