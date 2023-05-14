# Comparing `tmp/iso3166-updates-1.0.1.tar.gz` & `tmp/iso3166-updates-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso3166-updates-1.0.1.tar", last modified: Thu May 11 23:01:45 2023, max compression
+gzip compressed data, was "iso3166-updates-1.1.0.tar", last modified: Sun May 14 18:02:32 2023, max compression
```

## Comparing `iso3166-updates-1.0.1.tar` & `iso3166-updates-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:01:45.663933 iso3166-updates-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-11 23:01:24.000000 iso3166-updates-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-11 23:01:45.663933 iso3166-updates-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-05-11 23:01:24.000000 iso3166-updates-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:01:45.659933 iso3166-updates-1.0.1/iso3166_updates/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-11 23:01:24.000000 iso3166-updates-1.0.1/iso3166_updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-05-11 23:01:24.000000 iso3166-updates-1.0.1/iso3166_updates/iso3166_updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:01:45.663933 iso3166-updates-1.0.1/iso3166_updates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-11 23:01:45.000000 iso3166-updates-1.0.1/iso3166_updates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-11 23:01:45.000000 iso3166-updates-1.0.1/iso3166_updates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 23:01:45.000000 iso3166-updates-1.0.1/iso3166_updates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 23:01:37.000000 iso3166-updates-1.0.1/iso3166_updates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-11 23:01:45.000000 iso3166-updates-1.0.1/iso3166_updates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 23:01:45.000000 iso3166-updates-1.0.1/iso3166_updates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-11 23:01:45.663933 iso3166-updates-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-11 23:01:24.000000 iso3166-updates-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:02:32.526196 iso3166-updates-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-14 18:02:14.000000 iso3166-updates-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19669 2023-05-14 18:02:32.526196 iso3166-updates-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-05-14 18:02:14.000000 iso3166-updates-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:02:32.526196 iso3166-updates-1.1.0/iso3166_updates/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-14 18:02:14.000000 iso3166-updates-1.1.0/iso3166_updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24256 2023-05-14 18:02:14.000000 iso3166-updates-1.1.0/iso3166_updates/iso3166_updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:02:32.526196 iso3166-updates-1.1.0/iso3166_updates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19669 2023-05-14 18:02:32.000000 iso3166-updates-1.1.0/iso3166_updates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-14 18:02:32.000000 iso3166-updates-1.1.0/iso3166_updates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:02:32.000000 iso3166-updates-1.1.0/iso3166_updates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:02:26.000000 iso3166-updates-1.1.0/iso3166_updates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-14 18:02:32.000000 iso3166-updates-1.1.0/iso3166_updates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 18:02:32.000000 iso3166-updates-1.1.0/iso3166_updates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-14 18:02:32.526196 iso3166-updates-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-14 18:02:14.000000 iso3166-updates-1.1.0/setup.py
```

### Comparing `iso3166-updates-1.0.1/LICENSE` & `iso3166-updates-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iso3166-updates-1.0.1/PKG-INFO` & `iso3166-updates-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
@@ -20,68 +20,72 @@
         [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates)
         
         <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
           <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
           <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
         </div>
         
-        > Automated scripts that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
+        > Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
         
         Table of Contents
         -----------------
           * [Introduction](#introduction)
+          * [API][#API]
+          * [Staying up to date](#stayinguptodate)
           * [Requirements](#requirements)
           * [Installation](#installation)
           * [Usage](#usage)
           * [Directories](#Directories)
           * [Issues](#Issues)
           * [Contact](#contact)
           * [References](#references)
         
         Introduction
         ------------
-        `iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
+        `iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
         
         The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
         
         ## Problem Statement:
         
-        The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates sometimes being published at various times throughout the year [[4]](#references). 
+        The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
         
         This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
         
-        ## Intended Audience:
-        
-        This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (except 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API. 
-        
         <strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
         
-        Updates
-        -------
-        **Last Updated:**
+        ## Intended Audience:
         
-        The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
-        The object storing all updates both locally (iso3166-updates.json) and on the API are consistenly checked for the latest updates using a Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO3166-2 wiki's to check for the latest updates within a certain period e.g the past 3 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the main GCP Cloud Function returns the latest data. Additionally, a GitHub Issue in the `iso3166-2` repository will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` JSONs and repo.
-        Ultimately, this function ensures that the software and assoicated APIs are up-to-date with the latest ISO3166-2 information for all countries/territories/subdivisions etc.
+        This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
         
         API
         ---
         An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
         
         > https://www.iso3166-updates.com/api
         
-        Two query string parameters/paths are available in the API. The 2 letter alpha2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP" - or appended to the base url - "/alpha2/YE". A single alpha2 or list of them can be passed to the API (e.g "FR", "DE", "GY", "HU", "ID"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "2017", "2010-2015", "<2009", ">2002"). The API is hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below.
+        Three query string parameters/paths are available in the API - `alpha2`, `year` and `months`. The 2 letter alpha-2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP". A single alpha-2 or list of them can be passed to the API (e.g "FR", "DE", "HU, ID, MA"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "?year=2017", "2010-2015", "<2009", ">2002"). Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?month=6", "?month=48").
+        
+        The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
         
         The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
         
-         <!-- "?year" can be a specific year or year range to get updates for (e.g "2017", "2010-2015"), you can also get updates less than or greater than a year (e.g ">2004", "<2020") and "?months" which allows you to get the updates of the past X months. If months and year input params are set then months will take precedence. -->
         <p align="center">
           <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
         </p>
         
+        Staying up to date
+        ------------------
+        The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
+        The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
+        
+        Additionally, a GitHub Issue in the `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
+        
+        Ultimately, this Cloud Function ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
+        
         Requirements
         ------------
         * [python][python] >= 3.7
         * [pandas][pandas] >= 1.4.3
         * [numpy][numpy] >= 1.23.2
         * [requests][requests] >= 2.28.1
         * [beautifulsoup4][beautifulsoup4] >= 4.11.1
@@ -108,15 +112,15 @@
         ```python
         import iso3166_updates as iso3166_updates
         ```
         
         **Input parameters to get_updates function:**
         ```python
           # -alpha2 ALPHA2, --alpha2 ALPHA2
-          #                       Alpha2 code/s of ISO3166 countries to check for updates.
+          #                       Alpha-2 code/s of ISO3166 countries to check for updates.
           # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
           #                       Filename for exported ISO3166 updates csv file.
           # -export_json_filename EXPORT_JSON_FILENAME, --export_json_filename EXPORT_JSON_FILENAME
           #                       Filename for exported ISO3166 updates json file.
           # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
           #                       Folder where to store exported ISO files.
           # -export_json, --export_json
@@ -125,15 +129,15 @@
           #                       Whether to export all found updates to csv files in export folder.
           # -year YEAR, --year YEAR
           #                       Selected year to check for updates.
           # -concat_updates, --concat_updates
           #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
         ```
         
-        **Get all listed changes/updates for all countries which happens by default if no alpha2 codes specified in input param, export csv and json to folder "iso3166-updates":**
+        **Get all listed changes/updates for all countries which happens by default if no alpha-2 codes specified in input param, export csv and json to folder "iso3166-updates":**
         ```python
         iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
         ```
         
         **Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
         ```python
         iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
@@ -161,28 +165,28 @@
         
         **Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
         ```python
         iso3166_updates.get_updates("YE", year="<2010")
         ```
         
         The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
-        Edition/Newsletter, Date Issued, Description of change in newsletter and Code/Subdivision change. 
+        <b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> 
         
         * Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
         * Date Issued: Date that the change was communicated.
-        * Description of change in newsletter: More in-depth info about the change/update that was made.
         * Code/Subdivision change: Overall summary of change/update made.
+        * Description of change in newsletter: More in-depth info about the change/update that was made.
         
         E.g. The output format of the exported CSV for AD (Andorra) is:
         
-        | Edition/Newsletter | Date Issued | Description of change in newsletter | Code/Subdivision change |   
+        | Edition/Newsletter | Date Issued | Code/Subdivision change | Description of change in newsletter |   
         |:-------------------|:------------|------------------------------------:|------------------------:|
-        | Newsletter I-8     | 2007-04-17  | Addition of the administrative subdivisions...   | Subdivisions added: 7 parishes...                 | 
-        | Online Browsing Platform (OBP) | 2014-11-03 | Update List Source | No subdivision changes listed |
-        | Online Browsing Platform (OBP) | 2015-11-27 | Update List Source | No subdivision changes listed | 
+        | Newsletter I-8     | 2007-04-17  | Subdivisions added: 7 parishes...   | Addition of the administrative subdivisions...                 | 
+        | Online Browsing Platform (OBP) | 2014-11-03 | No subdivision changes listed | Update List Source |
+        | Online Browsing Platform (OBP) | 2015-11-27 | No subdivision changes listed | Update List Source | 
         
         E.g. The output format of the exported JSON for AD (Andorra) is:
         ```javascript
         {
           AD: [
               {
                 "Code/Subdivision change": "",
@@ -207,15 +211,15 @@
         ```
         
         Directories
         -----------
         * `/docs` - documentation for `iso3166-updates` Python package.
         * `/iso3166_updates` - source code for `iso3166-updates` Python package.
         * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
-        * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Func that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt.
+        * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Function that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt files.
         * `/tests` - unit and integration tests for `iso3166-updates`.
         
         Issues
         ------
         Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
         
         Contact
@@ -226,14 +230,15 @@
         References
         ----------
         \[1\]: ISO3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
         \[2\]: ISO3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
         \[3\]: ISO Country Codes Collection: https://www.iso.org/publication/PUB500001 <br>
         \[4\]: ISO Country Codes: https://www.iso.org/iso-3166-country-codes.html <br>
         \[5\]: ISO3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
+        \[6\]: ISO3166-2 flag-icons repo: https://github.com/amckenna41/iso3166-flag-icons <br>
         
         Support
         -------
         <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
         
         [Back to top](#TOP)
```

### Comparing `iso3166-updates-1.0.1/README.md` & `iso3166-updates-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,68 +10,72 @@
 [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates)
 
 <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
   <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
 </div>
 
-> Automated scripts that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
+> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
 
 Table of Contents
 -----------------
   * [Introduction](#introduction)
+  * [API][#API]
+  * [Staying up to date](#stayinguptodate)
   * [Requirements](#requirements)
   * [Installation](#installation)
   * [Usage](#usage)
   * [Directories](#Directories)
   * [Issues](#Issues)
   * [Contact](#contact)
   * [References](#references)
 
 Introduction
 ------------
-`iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
+`iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
 
 The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
 
 ## Problem Statement:
 
-The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates sometimes being published at various times throughout the year [[4]](#references). 
+The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
 
 This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
 
-## Intended Audience:
-
-This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (except 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API. 
-
 <strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
 
-Updates
--------
-**Last Updated:**
+## Intended Audience:
 
-The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
-The object storing all updates both locally (iso3166-updates.json) and on the API are consistenly checked for the latest updates using a Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO3166-2 wiki's to check for the latest updates within a certain period e.g the past 3 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the main GCP Cloud Function returns the latest data. Additionally, a GitHub Issue in the `iso3166-2` repository will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` JSONs and repo.
-Ultimately, this function ensures that the software and assoicated APIs are up-to-date with the latest ISO3166-2 information for all countries/territories/subdivisions etc.
+This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
 
 API
 ---
 An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
 
 > https://www.iso3166-updates.com/api
 
-Two query string parameters/paths are available in the API. The 2 letter alpha2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP" - or appended to the base url - "/alpha2/YE". A single alpha2 or list of them can be passed to the API (e.g "FR", "DE", "GY", "HU", "ID"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "2017", "2010-2015", "<2009", ">2002"). The API is hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below.
+Three query string parameters/paths are available in the API - `alpha2`, `year` and `months`. The 2 letter alpha-2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP". A single alpha-2 or list of them can be passed to the API (e.g "FR", "DE", "HU, ID, MA"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "?year=2017", "2010-2015", "<2009", ">2002"). Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?month=6", "?month=48").
+
+The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
 
 The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
 
- <!-- "?year" can be a specific year or year range to get updates for (e.g "2017", "2010-2015"), you can also get updates less than or greater than a year (e.g ">2004", "<2020") and "?months" which allows you to get the updates of the past X months. If months and year input params are set then months will take precedence. -->
 <p align="center">
   <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
 </p>
 
+Staying up to date
+------------------
+The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
+The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
+
+Additionally, a GitHub Issue in the `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
+
+Ultimately, this Cloud Function ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
+
 Requirements
 ------------
 * [python][python] >= 3.7
 * [pandas][pandas] >= 1.4.3
 * [numpy][numpy] >= 1.23.2
 * [requests][requests] >= 2.28.1
 * [beautifulsoup4][beautifulsoup4] >= 4.11.1
@@ -98,15 +102,15 @@
 ```python
 import iso3166_updates as iso3166_updates
 ```
 
 **Input parameters to get_updates function:**
 ```python
   # -alpha2 ALPHA2, --alpha2 ALPHA2
-  #                       Alpha2 code/s of ISO3166 countries to check for updates.
+  #                       Alpha-2 code/s of ISO3166 countries to check for updates.
   # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
   #                       Filename for exported ISO3166 updates csv file.
   # -export_json_filename EXPORT_JSON_FILENAME, --export_json_filename EXPORT_JSON_FILENAME
   #                       Filename for exported ISO3166 updates json file.
   # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
   #                       Folder where to store exported ISO files.
   # -export_json, --export_json
@@ -115,15 +119,15 @@
   #                       Whether to export all found updates to csv files in export folder.
   # -year YEAR, --year YEAR
   #                       Selected year to check for updates.
   # -concat_updates, --concat_updates
   #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
 ```
 
-**Get all listed changes/updates for all countries which happens by default if no alpha2 codes specified in input param, export csv and json to folder "iso3166-updates":**
+**Get all listed changes/updates for all countries which happens by default if no alpha-2 codes specified in input param, export csv and json to folder "iso3166-updates":**
 ```python
 iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
 ```
 
 **Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
 ```python
 iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
@@ -151,28 +155,28 @@
 
 **Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
 ```python
 iso3166_updates.get_updates("YE", year="<2010")
 ```
 
 The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
-Edition/Newsletter, Date Issued, Description of change in newsletter and Code/Subdivision change. 
+<b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> 
 
 * Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
 * Date Issued: Date that the change was communicated.
-* Description of change in newsletter: More in-depth info about the change/update that was made.
 * Code/Subdivision change: Overall summary of change/update made.
+* Description of change in newsletter: More in-depth info about the change/update that was made.
 
 E.g. The output format of the exported CSV for AD (Andorra) is:
 
-| Edition/Newsletter | Date Issued | Description of change in newsletter | Code/Subdivision change |   
+| Edition/Newsletter | Date Issued | Code/Subdivision change | Description of change in newsletter |   
 |:-------------------|:------------|------------------------------------:|------------------------:|
-| Newsletter I-8     | 2007-04-17  | Addition of the administrative subdivisions...   | Subdivisions added: 7 parishes...                 | 
-| Online Browsing Platform (OBP) | 2014-11-03 | Update List Source | No subdivision changes listed |
-| Online Browsing Platform (OBP) | 2015-11-27 | Update List Source | No subdivision changes listed | 
+| Newsletter I-8     | 2007-04-17  | Subdivisions added: 7 parishes...   | Addition of the administrative subdivisions...                 | 
+| Online Browsing Platform (OBP) | 2014-11-03 | No subdivision changes listed | Update List Source |
+| Online Browsing Platform (OBP) | 2015-11-27 | No subdivision changes listed | Update List Source | 
 
 E.g. The output format of the exported JSON for AD (Andorra) is:
 ```javascript
 {
   AD: [
       {
         "Code/Subdivision change": "",
@@ -197,15 +201,15 @@
 ```
 
 Directories
 -----------
 * `/docs` - documentation for `iso3166-updates` Python package.
 * `/iso3166_updates` - source code for `iso3166-updates` Python package.
 * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
-* `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Func that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt.
+* `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Function that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt files.
 * `/tests` - unit and integration tests for `iso3166-updates`.
 
 Issues
 ------
 Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
 
 Contact
@@ -216,14 +220,15 @@
 References
 ----------
 \[1\]: ISO3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
 \[2\]: ISO3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
 \[3\]: ISO Country Codes Collection: https://www.iso.org/publication/PUB500001 <br>
 \[4\]: ISO Country Codes: https://www.iso.org/iso-3166-country-codes.html <br>
 \[5\]: ISO3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
+\[6\]: ISO3166-2 flag-icons repo: https://github.com/amckenna41/iso3166-flag-icons <br>
 
 Support
 -------
 <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 [Back to top](#TOP)
```

### Comparing `iso3166-updates-1.0.1/iso3166_updates/iso3166_updates.py` & `iso3166-updates-1.1.0/iso3166_updates/iso3166_updates.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,40 +55,46 @@
     :export_filename : str (default = "iso3166-updates")
         filename for csv output of inputted country's ISO3166-2 updates. 
     :export_json_filename : str (default = "iso3166-updates")
         filename for json output of all country's ISO3166-2 updates. 
     :export_folder : str (default = "../iso3166-updates")
         folder name to store all csv outputs for all country's ISO3166-2 updates. 
     :concat_updates : bool (default = True)
-        if multiple alpha-2 codes input, concatenate updates into one json file or into seperately
+        if multiple alpha-2 codes input, concatenate updates into one JSOn file or into seperately
         named files in export folder. Not available for csv output.
     :export_json : bool (default = True)
         export all ISO3166 updates for inputted country's into json format. 
     :export_csv : bool (default = False)
         export all ISO3166 updates for inputted country's to csv files in export folder.
 
     Returns
     -------
-    None
+    :all_changes : dict
+        dictionary of all found ISO3166 updates from users inputted alpha2 codes and or year
+        parameter values.
     """
     year_range = False
     greater_than = False
     less_than = False
     
     #if alpha-2 codes input param isn't str or list raise type error
     if not isinstance(alpha2_codes, str) and not isinstance(alpha2_codes, list):
         raise TypeError('alpha2_codes input param should be a 2 letter '
             'ISO3166 alpha-2 code or a list of the same, got input of type {}.'.format(type(alpha2_codes)))
 
-    #if single str input for alpha2 codes param then convert to array, remove whitespace
-    if isinstance(alpha2_codes, str):
+    #if single str input for alpha-2 codes param then convert to array, remove whitespace
+    if (isinstance(alpha2_codes, str)):
         alpha2_codes = alpha2_codes.replace(' ', '').split(',')
 
+    #if list with 1 string of multiple alpha-2 codes, convert to multiple list elements e.g ['HI, LA'] will be converted to ['HI', 'LA']
+    if (isinstance(alpha2_codes, list) and len(alpha2_codes) == 1 and ',' in alpha2_codes[0]):
+        alpha2_codes = alpha2_codes[0].replace(' ', '').split(',')
+
     #if single str input for Year param then convert to array, remove whitespace
-    if isinstance(year, str):
+    if (isinstance(year, str)):
         year = year.replace(' ', '').split(',')
 
     #use all ISO3166 codes if invalid alpha-2 code input, otherwise convert alpha-2 to array
     if (alpha2_codes == []):
         alpha2_codes = sorted(list(iso3166.countries_by_alpha2.keys()))
 
     #sort codes in alphabetical order
@@ -138,19 +144,15 @@
     #object to store all country updates/changes
     all_changes = {}
 
     export_fname = export_filename + '-'
 
     #iterate over all input ISO country codes
     for alpha2 in alpha2_codes:
-
-        # if len(alpha2_codes) == 1: 
-        #     export_fname = export_filename + alpha-2  
-        # else:
-        #     export_fname += "," + alpha-2
+        
         export_fname = export_filename + '-' + alpha2  
 
         #skip to next iteration if alpha-2 not valid
         if (alpha2 not in list(iso3166.countries_by_alpha2.keys())):
             continue
 
         print("ISO Code: {} ({})".format(alpha2, wiki_base_url + alpha2))
@@ -227,28 +229,38 @@
             def convert_date_format(row):
                 """ convert date in rows of df into dd-mm-yyyy data format from date object. """
                 return datetime.datetime.strptime(row.replace('\n', ''), '%Y-%m-%d').strftime('%d-%m-%Y')
 
             #convert date column into dd-mm-yyyy format  
             iso3166_df["Date Issued"] = iso3166_df["Date Issued"].apply(convert_date_format)
 
-            #export to csv
+            #export to csv, append extension if applicable
             if (export_csv): 
-                iso3166_df.to_csv(os.path.join(export_folder, export_fname + '.csv'), index=False)
+                if (os.path.splitext(export_json_filename)[1] != ".csv"):
+                    export_fname = export_fname + ".csv"
+                iso3166_df.to_csv(os.path.join(export_folder, export_fname), index=False)
         
             #add ISO updates to object of all ISO3166 updates, convert to json 
             all_changes[alpha2] = json.loads(iso3166_df.to_json(orient='records'))
 
         #reset export filename var 
         export_fname = export_filename
 
+    #append list of alpha-2 codes to exported json filename if 10 or less codes input,
+    #and codes are not already in filename and the multiple outputs are to be concatenated (concat_updates=True)
+    if (len(alpha2_codes) <= 10 and not (any(code in export_json_filename for code in alpha2_codes)) and concat_updates==True):
+        alpha2_str = ','.join(alpha2_codes)
+        if (os.path.splitext(export_json_filename)[1] == ".json"):
+            export_json_filename = os.path.splitext(export_json_filename)[0]
+        export_json_filename = export_json_filename + "-" + alpha2_str + ".json"
+
     #append extension to json filename, if applicable 
-    if (os.path.splitext(export_json_filename)[1] != "json"):
+    if (os.path.splitext(export_json_filename)[1] != ".json"):
         export_json_filename = export_json_filename + ".json"
-
+        
     #export all ISO3166 updates to json, store in export folder dir
     if (export_json):
         if (all_changes):   #checking if all_changes obj isn't empty
             if (concat_updates):
                 #concatenate updates into the same json
                 with open(os.path.join(export_folder, export_json_filename), "w") as write_file:
                     json.dump(all_changes, write_file, indent=4, ensure_ascii=False)
@@ -256,14 +268,16 @@
                 #seperate country updates into individual json files
                 for update in all_changes:
                     with open(os.path.join(export_folder, os.path.splitext(export_json_filename)[0] + "-" + update + ".json"), "w") as write_file:
                         json.dump(all_changes[update], write_file, indent=4, ensure_ascii=False)
             
             print("All ISO3166 changes exported to folder {}.".format(export_folder))
     
+    return all_changes
+
 def get_updates_df(iso3166_updates_table, year=[], year_range=False, less_than=False, greater_than=False):
     """
     Convert parsed html table, from the Changes Section in the respective ISO3166-2 wiki
     page, into a pandas dataframe. Convert columns/headers using correct naming 
     conventions. If year param not empty then remove any rows that don't have 
     specified year(s) or year range.
 
@@ -477,15 +491,15 @@
     parser.add_argument('-export_folder', '--export_folder', type=str, required=False, default="test-iso3166-updates", 
         help='Folder where to store exported ISO files.')
     parser.add_argument('-export_json', '--export_json', action="store_false", required=False, 
         help='Whether to export all found updates to json.')
     parser.add_argument('-export_csv', '--export_csv', required=False, action="store_true", 
         help='Whether to export all found updates to csv files in export folder.')
     parser.add_argument('-concat_updates', '--concat_updates', action="store_true", default=True, required=False, 
-        help='Whether to concatenate updates of individual countrys into the same json file or seperate.')
+        help='Whether to concatenate updates of individual countrys into the same json file or individual. Only applies to JSON files, not CSVs.')
 
     #parse input args
     args = parser.parse_args()
     alpha2_codes = [args.alpha2]
     if (',' in alpha2_codes[0]):
         alpha2_codes = alpha2_codes[0].split(',')
     export_filename = args.export_filename
```

### Comparing `iso3166-updates-1.0.1/iso3166_updates.egg-info/PKG-INFO` & `iso3166-updates-1.1.0/iso3166_updates.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
@@ -20,68 +20,72 @@
         [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates)
         
         <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
           <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
           <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
         </div>
         
-        > Automated scripts that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
+        > Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
         
         Table of Contents
         -----------------
           * [Introduction](#introduction)
+          * [API][#API]
+          * [Staying up to date](#stayinguptodate)
           * [Requirements](#requirements)
           * [Installation](#installation)
           * [Usage](#usage)
           * [Directories](#Directories)
           * [Issues](#Issues)
           * [Contact](#contact)
           * [References](#references)
         
         Introduction
         ------------
-        `iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
+        `iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
         
         The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
         
         ## Problem Statement:
         
-        The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates sometimes being published at various times throughout the year [[4]](#references). 
+        The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
         
         This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
         
-        ## Intended Audience:
-        
-        This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (except 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API. 
-        
         <strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
         
-        Updates
-        -------
-        **Last Updated:**
+        ## Intended Audience:
         
-        The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
-        The object storing all updates both locally (iso3166-updates.json) and on the API are consistenly checked for the latest updates using a Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO3166-2 wiki's to check for the latest updates within a certain period e.g the past 3 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the main GCP Cloud Function returns the latest data. Additionally, a GitHub Issue in the `iso3166-2` repository will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` JSONs and repo.
-        Ultimately, this function ensures that the software and assoicated APIs are up-to-date with the latest ISO3166-2 information for all countries/territories/subdivisions etc.
+        This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
         
         API
         ---
         An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
         
         > https://www.iso3166-updates.com/api
         
-        Two query string parameters/paths are available in the API. The 2 letter alpha2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP" - or appended to the base url - "/alpha2/YE". A single alpha2 or list of them can be passed to the API (e.g "FR", "DE", "GY", "HU", "ID"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "2017", "2010-2015", "<2009", ">2002"). The API is hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below.
+        Three query string parameters/paths are available in the API - `alpha2`, `year` and `months`. The 2 letter alpha-2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP". A single alpha-2 or list of them can be passed to the API (e.g "FR", "DE", "HU, ID, MA"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "?year=2017", "2010-2015", "<2009", ">2002"). Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?month=6", "?month=48").
+        
+        The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
         
         The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
         
-         <!-- "?year" can be a specific year or year range to get updates for (e.g "2017", "2010-2015"), you can also get updates less than or greater than a year (e.g ">2004", "<2020") and "?months" which allows you to get the updates of the past X months. If months and year input params are set then months will take precedence. -->
         <p align="center">
           <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
         </p>
         
+        Staying up to date
+        ------------------
+        The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
+        The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
+        
+        Additionally, a GitHub Issue in the `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
+        
+        Ultimately, this Cloud Function ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
+        
         Requirements
         ------------
         * [python][python] >= 3.7
         * [pandas][pandas] >= 1.4.3
         * [numpy][numpy] >= 1.23.2
         * [requests][requests] >= 2.28.1
         * [beautifulsoup4][beautifulsoup4] >= 4.11.1
@@ -108,15 +112,15 @@
         ```python
         import iso3166_updates as iso3166_updates
         ```
         
         **Input parameters to get_updates function:**
         ```python
           # -alpha2 ALPHA2, --alpha2 ALPHA2
-          #                       Alpha2 code/s of ISO3166 countries to check for updates.
+          #                       Alpha-2 code/s of ISO3166 countries to check for updates.
           # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
           #                       Filename for exported ISO3166 updates csv file.
           # -export_json_filename EXPORT_JSON_FILENAME, --export_json_filename EXPORT_JSON_FILENAME
           #                       Filename for exported ISO3166 updates json file.
           # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
           #                       Folder where to store exported ISO files.
           # -export_json, --export_json
@@ -125,15 +129,15 @@
           #                       Whether to export all found updates to csv files in export folder.
           # -year YEAR, --year YEAR
           #                       Selected year to check for updates.
           # -concat_updates, --concat_updates
           #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
         ```
         
-        **Get all listed changes/updates for all countries which happens by default if no alpha2 codes specified in input param, export csv and json to folder "iso3166-updates":**
+        **Get all listed changes/updates for all countries which happens by default if no alpha-2 codes specified in input param, export csv and json to folder "iso3166-updates":**
         ```python
         iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
         ```
         
         **Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
         ```python
         iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
@@ -161,28 +165,28 @@
         
         **Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
         ```python
         iso3166_updates.get_updates("YE", year="<2010")
         ```
         
         The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
-        Edition/Newsletter, Date Issued, Description of change in newsletter and Code/Subdivision change. 
+        <b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> 
         
         * Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
         * Date Issued: Date that the change was communicated.
-        * Description of change in newsletter: More in-depth info about the change/update that was made.
         * Code/Subdivision change: Overall summary of change/update made.
+        * Description of change in newsletter: More in-depth info about the change/update that was made.
         
         E.g. The output format of the exported CSV for AD (Andorra) is:
         
-        | Edition/Newsletter | Date Issued | Description of change in newsletter | Code/Subdivision change |   
+        | Edition/Newsletter | Date Issued | Code/Subdivision change | Description of change in newsletter |   
         |:-------------------|:------------|------------------------------------:|------------------------:|
-        | Newsletter I-8     | 2007-04-17  | Addition of the administrative subdivisions...   | Subdivisions added: 7 parishes...                 | 
-        | Online Browsing Platform (OBP) | 2014-11-03 | Update List Source | No subdivision changes listed |
-        | Online Browsing Platform (OBP) | 2015-11-27 | Update List Source | No subdivision changes listed | 
+        | Newsletter I-8     | 2007-04-17  | Subdivisions added: 7 parishes...   | Addition of the administrative subdivisions...                 | 
+        | Online Browsing Platform (OBP) | 2014-11-03 | No subdivision changes listed | Update List Source |
+        | Online Browsing Platform (OBP) | 2015-11-27 | No subdivision changes listed | Update List Source | 
         
         E.g. The output format of the exported JSON for AD (Andorra) is:
         ```javascript
         {
           AD: [
               {
                 "Code/Subdivision change": "",
@@ -207,15 +211,15 @@
         ```
         
         Directories
         -----------
         * `/docs` - documentation for `iso3166-updates` Python package.
         * `/iso3166_updates` - source code for `iso3166-updates` Python package.
         * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
-        * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Func that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt.
+        * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Function that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt files.
         * `/tests` - unit and integration tests for `iso3166-updates`.
         
         Issues
         ------
         Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
         
         Contact
@@ -226,14 +230,15 @@
         References
         ----------
         \[1\]: ISO3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
         \[2\]: ISO3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
         \[3\]: ISO Country Codes Collection: https://www.iso.org/publication/PUB500001 <br>
         \[4\]: ISO Country Codes: https://www.iso.org/iso-3166-country-codes.html <br>
         \[5\]: ISO3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
+        \[6\]: ISO3166-2 flag-icons repo: https://github.com/amckenna41/iso3166-flag-icons <br>
         
         Support
         -------
         <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
         
         [Back to top](#TOP)
```

### Comparing `iso3166-updates-1.0.1/setup.cfg` & `iso3166-updates-1.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iso3166-updates
-version = 1.0.1
+version = 1.1.0
 description = A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = AJ McKenna
 author_email = amckenna41@qub.ac.uk
 url = https://github.com/amckenna41/iso3166-updates
 download_url = https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
```

### Comparing `iso3166-updates-1.0.1/setup.py` & `iso3166-updates-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pathlib
 from setuptools import setup, find_packages
 import sys
 # import iso3166_updates
 
 #software metadata
 __name__ = 'iso3166-updates'
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 __description__ = "A Python package that pulls the latest updates & changes to all ISO3166 listed countries."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-updates'
 __download_url__ = "https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip"
 __status__ = 'Development'
```

