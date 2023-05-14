# Comparing `tmp/IMDbTraktSyncer-1.1.1.tar.gz` & `tmp/IMDbTraktSyncer-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDbTraktSyncer-1.1.1.tar", last modified: Sat May 13 08:57:09 2023, max compression
+gzip compressed data, was "IMDbTraktSyncer-1.1.2.tar", last modified: Sun May 14 21:24:30 2023, max compression
```

## Comparing `IMDbTraktSyncer-1.1.1.tar` & `IMDbTraktSyncer-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 08:57:09.302025 IMDbTraktSyncer-1.1.1/
-drwxrwxrwx   0        0        0        0 2023-05-13 08:57:09.279555 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer/
--rw-rw-rw-   0        0        0    10477 2023-05-13 08:29:09.000000 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer/IMDbTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-05-13 08:29:09.000000 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0      642 2023-05-13 08:29:09.000000 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     2060 2023-05-13 08:50:24.000000 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer/imdbRatings.py
--rw-rw-rw-   0        0        0     1408 2023-05-13 08:29:09.000000 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     2516 2023-05-13 08:29:09.000000 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-13 08:57:09.299528 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6624 2023-05-13 08:57:09.000000 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-05-13 08:57:09.000000 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 08:57:09.000000 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-13 08:57:09.000000 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-13 08:57:09.000000 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-13 08:57:09.000000 IMDbTraktSyncer-1.1.1/IMDbTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     6624 2023-05-13 08:57:09.301529 IMDbTraktSyncer-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6004 2023-05-13 08:16:25.000000 IMDbTraktSyncer-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-13 08:57:09.302524 IMDbTraktSyncer-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1287 2023-05-13 08:56:51.000000 IMDbTraktSyncer-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 21:24:30.065591 IMDbTraktSyncer-1.1.2/
+drwxrwxrwx   0        0        0        0 2023-05-14 21:24:30.030559 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/
+-rw-rw-rw-   0        0        0    10477 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/IMDbTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     3511 2023-05-14 21:13:51.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     2060 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/imdbRatings.py
+-rw-rw-rw-   0        0        0     1408 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     2516 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-14 21:24:30.062595 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6624 2023-05-14 21:24:29.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-05-14 21:24:29.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 21:24:29.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-14 21:24:29.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-14 21:24:29.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-14 21:24:29.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6624 2023-05-14 21:24:30.064592 IMDbTraktSyncer-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6004 2023-05-14 21:23:43.000000 IMDbTraktSyncer-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-14 21:24:30.065591 IMDbTraktSyncer-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1287 2023-05-14 21:23:18.000000 IMDbTraktSyncer-1.1.2/setup.py
```

### Comparing `IMDbTraktSyncer-1.1.1/IMDbTraktSyncer/IMDbTraktSyncer.py` & `IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/IMDbTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.1/IMDbTraktSyncer/authTrakt.py` & `IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.1/IMDbTraktSyncer/imdbRatings.py` & `IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/imdbRatings.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.1/IMDbTraktSyncer/traktRatings.py` & `IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.1/IMDbTraktSyncer/verifyCredentials.py` & `IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.1/IMDbTraktSyncer.egg-info/PKG-INFO` & `IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.1.1
+Version: 1.1.2
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -42,15 +42,15 @@
 ## Troubleshooting, known issues, workarounds & future outlook:
 * IMDb may require a captcha on login. If you see "Not signed in" appear in the script then the script will fail and the captcha is likely to be the cause. To fix this, navigate to IMDb website in your browser, preferably Chrome and from the same computer. If logged in, logout, and log back in. It may ask you to fill in a captch, complete it and finish logging in. After logging in succesfully on your browser run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues. I'm looking into adding a captcha solver into the script to solve this problem, but it is currently not implemented. https://github.com/RileyXX/IMDb-Trakt-Syncer/issues/2
 * If you see an error about having the incorrect version of Chrome driver. Uninstall it by running `python -m pip uninstall chromedriver-py` in command line. In your Chrome browser navigate to Settings > About Chrome and check your version (112... or 111 etc). This would indicate you are on Chrome version 112. Navigate to [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that is the same Chrome version (112) already on your machine. Copy the version number you need. Then in command line run `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct chromedriver version. Run the script again and it should work. https://github.com/RileyXX/IMDb-Trakt-Syncer/issues/16
 * Due to IMDb's lack of API and lack of rating import ability, this script uses a rather unconventional method that mimics using a web browser to set ratings on IMDB. So there are many points of failure that could arise. I will try my best to keep the script updated as best possible.
 * If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
 
 ## Screenshot:
-![Demo](https://i.imgur.com/uydTDcg.png)
+![Demo](https://i.imgur.com/QXCtGrr.png)
 
 
 ## Sponsorships, Donations and Custom Projects:
 Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
 
 #### More donation options:
 - Cashapp: `$rileyxx`
```

### Comparing `IMDbTraktSyncer-1.1.1/LICENSE` & `IMDbTraktSyncer-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.1/PKG-INFO` & `IMDbTraktSyncer-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.1.1
+Version: 1.1.2
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -42,15 +42,15 @@
 ## Troubleshooting, known issues, workarounds & future outlook:
 * IMDb may require a captcha on login. If you see "Not signed in" appear in the script then the script will fail and the captcha is likely to be the cause. To fix this, navigate to IMDb website in your browser, preferably Chrome and from the same computer. If logged in, logout, and log back in. It may ask you to fill in a captch, complete it and finish logging in. After logging in succesfully on your browser run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues. I'm looking into adding a captcha solver into the script to solve this problem, but it is currently not implemented. https://github.com/RileyXX/IMDb-Trakt-Syncer/issues/2
 * If you see an error about having the incorrect version of Chrome driver. Uninstall it by running `python -m pip uninstall chromedriver-py` in command line. In your Chrome browser navigate to Settings > About Chrome and check your version (112... or 111 etc). This would indicate you are on Chrome version 112. Navigate to [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that is the same Chrome version (112) already on your machine. Copy the version number you need. Then in command line run `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct chromedriver version. Run the script again and it should work. https://github.com/RileyXX/IMDb-Trakt-Syncer/issues/16
 * Due to IMDb's lack of API and lack of rating import ability, this script uses a rather unconventional method that mimics using a web browser to set ratings on IMDB. So there are many points of failure that could arise. I will try my best to keep the script updated as best possible.
 * If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
 
 ## Screenshot:
-![Demo](https://i.imgur.com/uydTDcg.png)
+![Demo](https://i.imgur.com/QXCtGrr.png)
 
 
 ## Sponsorships, Donations and Custom Projects:
 Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
 
 #### More donation options:
 - Cashapp: `$rileyxx`
```

### Comparing `IMDbTraktSyncer-1.1.1/README.md` & `IMDbTraktSyncer-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ## Troubleshooting, known issues, workarounds & future outlook:
 * IMDb may require a captcha on login. If you see "Not signed in" appear in the script then the script will fail and the captcha is likely to be the cause. To fix this, navigate to IMDb website in your browser, preferably Chrome and from the same computer. If logged in, logout, and log back in. It may ask you to fill in a captch, complete it and finish logging in. After logging in succesfully on your browser run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues. I'm looking into adding a captcha solver into the script to solve this problem, but it is currently not implemented. https://github.com/RileyXX/IMDb-Trakt-Syncer/issues/2
 * If you see an error about having the incorrect version of Chrome driver. Uninstall it by running `python -m pip uninstall chromedriver-py` in command line. In your Chrome browser navigate to Settings > About Chrome and check your version (112... or 111 etc). This would indicate you are on Chrome version 112. Navigate to [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that is the same Chrome version (112) already on your machine. Copy the version number you need. Then in command line run `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct chromedriver version. Run the script again and it should work. https://github.com/RileyXX/IMDb-Trakt-Syncer/issues/16
 * Due to IMDb's lack of API and lack of rating import ability, this script uses a rather unconventional method that mimics using a web browser to set ratings on IMDB. So there are many points of failure that could arise. I will try my best to keep the script updated as best possible.
 * If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
 
 ## Screenshot:
-![Demo](https://i.imgur.com/uydTDcg.png)
+![Demo](https://i.imgur.com/QXCtGrr.png)
 
 
 ## Sponsorships, Donations and Custom Projects:
 Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
 
 #### More donation options:
 - Cashapp: `$rileyxx`
```

### Comparing `IMDbTraktSyncer-1.1.1/setup.py` & `IMDbTraktSyncer-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.1'
+VERSION = '1.1.2'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.'
 
 # Setting up
 setup(
     name="IMDbTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

