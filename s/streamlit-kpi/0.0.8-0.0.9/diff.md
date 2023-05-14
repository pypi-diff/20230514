# Comparing `tmp/streamlit-kpi-0.0.8.tar.gz` & `tmp/streamlit-kpi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-kpi-0.0.8.tar", last modified: Fri Mar 17 15:46:22 2023, max compression
+gzip compressed data, was "streamlit-kpi-0.0.9.tar", last modified: Fri Mar 17 16:15:17 2023, max compression
```

## Comparing `streamlit-kpi-0.0.8.tar` & `streamlit-kpi-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:46:22.409290 streamlit-kpi-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-17 15:46:09.000000 streamlit-kpi-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-17 15:46:09.000000 streamlit-kpi-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-17 15:46:22.409290 streamlit-kpi-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-03-17 15:46:09.000000 streamlit-kpi-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 15:46:22.409290 streamlit-kpi-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-17 15:46:09.000000 streamlit-kpi-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:46:22.405290 streamlit-kpi-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:46:22.409290 streamlit-kpi-0.0.8/src/streamlit_kpi/
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-03-17 15:46:09.000000 streamlit-kpi-0.0.8/src/streamlit_kpi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:46:22.409290 streamlit-kpi-0.0.8/src/streamlit_kpi/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-17 15:46:09.000000 streamlit-kpi-0.0.8/src/streamlit_kpi/frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-03-17 15:46:09.000000 streamlit-kpi-0.0.8/src/streamlit_kpi/frontend/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-17 15:46:09.000000 streamlit-kpi-0.0.8/src/streamlit_kpi/frontend/streamlit-component-lib.js
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-03-17 15:46:09.000000 streamlit-kpi-0.0.8/src/streamlit_kpi/frontend/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:46:22.409290 streamlit-kpi-0.0.8/src/streamlit_kpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-17 15:46:22.000000 streamlit-kpi-0.0.8/src/streamlit_kpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-17 15:46:22.000000 streamlit-kpi-0.0.8/src/streamlit_kpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 15:46:22.000000 streamlit-kpi-0.0.8/src/streamlit_kpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-17 15:46:22.000000 streamlit-kpi-0.0.8/src/streamlit_kpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-17 15:46:22.000000 streamlit-kpi-0.0.8/src/streamlit_kpi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:15:17.664352 streamlit-kpi-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-17 16:14:51.000000 streamlit-kpi-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-17 16:14:51.000000 streamlit-kpi-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-17 16:15:17.664352 streamlit-kpi-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-17 16:14:51.000000 streamlit-kpi-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 16:15:17.664352 streamlit-kpi-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-17 16:14:51.000000 streamlit-kpi-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:15:17.660352 streamlit-kpi-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:15:17.660352 streamlit-kpi-0.0.9/src/streamlit_kpi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-03-17 16:14:51.000000 streamlit-kpi-0.0.9/src/streamlit_kpi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:15:17.664352 streamlit-kpi-0.0.9/src/streamlit_kpi/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-17 16:14:51.000000 streamlit-kpi-0.0.9/src/streamlit_kpi/frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-03-17 16:14:51.000000 streamlit-kpi-0.0.9/src/streamlit_kpi/frontend/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-17 16:14:51.000000 streamlit-kpi-0.0.9/src/streamlit_kpi/frontend/streamlit-component-lib.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-03-17 16:14:51.000000 streamlit-kpi-0.0.9/src/streamlit_kpi/frontend/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:15:17.664352 streamlit-kpi-0.0.9/src/streamlit_kpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-17 16:15:17.000000 streamlit-kpi-0.0.9/src/streamlit_kpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-17 16:15:17.000000 streamlit-kpi-0.0.9/src/streamlit_kpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 16:15:17.000000 streamlit-kpi-0.0.9/src/streamlit_kpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-17 16:15:17.000000 streamlit-kpi-0.0.9/src/streamlit_kpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-17 16:15:17.000000 streamlit-kpi-0.0.9/src/streamlit_kpi.egg-info/top_level.txt
```

### Comparing `streamlit-kpi-0.0.8/LICENSE` & `streamlit-kpi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-kpi-0.0.8/PKG-INFO` & `streamlit-kpi-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: streamlit-kpi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Streamlit component for displaying KPI's
 Author: Anthony Alteirac
 Author-email: anthony@alteirac.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Test it Live !
 <a href="https://aalteirac-kpi.streamlit.app/" title="3d-badge"><img src="https://static.streamlit.io/badges/streamlit_badge_black_white.svg"></a><br>
 
 # streamlit-kpi
 
-Streamlit component for displaying KPIs
+Streamlit component for displaying KPIs, easy layout to fit all your needs !
+
+![ScreenShot](https://raw.githubusercontent.com/aalteirac/streamlit-kpi/master/screen.png)
 
 ## Installation instructions 
 
 ```sh
 pip install streamlit-kpi
 ```
```

#### html2text {}

```diff
@@ -1,33 +1,35 @@
-Metadata-Version: 2.1 Name: streamlit-kpi Version: 0.0.8 Summary: Streamlit
+Metadata-Version: 2.1 Name: streamlit-kpi Version: 0.0.9 Summary: Streamlit
 component for displaying KPI's Author: Anthony Alteirac Author-email:
 anthony@alteirac.com Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE ## Test it Live ! [https://static.streamlit.io/
 badges/streamlit_badge_black_white.svg]
-# streamlit-kpi Streamlit component for displaying KPIs ## Installation
-instructions ```sh pip install streamlit-kpi ``` ## Usage instructions
-```python import streamlit as st from streamlit_kpi import streamlit_kpi
-streamlit_kpi(key="first_kpi",height='200',title='Monthly
-Sales',value=25000,icon='fa-solid fa-globe',progressValue=100,unit='Kâ¬') """
-Parameters: key: Optional str, default is '', the streamlit component key,
-higly recommended title: Mandatory str, the title... value: Mandatory str or
-int or float, the value... icon: Optional str, default is 'fa-solid fa-globe',
-any Font Awesome class (v6.3). See https://fontawesome.com/search?o=r&m=free
-icon: Optional str, default is '', the value unit appended after the value
-textAlign: Optional str, default is 'left', title and value alignement
-backgroundColor: Optional str, default is '#f3f3f3', widget background color
-can be str like blue, orange, transparent... or HEX color titleColor: Optional
-str, default is 'dark', title font color, can be str like blue, orange... or
-HEX color valueColor: Optional str, default is 'dark', value font color, can be
-str like blue, orange... or HEX color progressColor: Optional str, default is
-'green', progress color, can be str like blue, orange... or HEX color
-iconColor: Optional str, default is 'black', icon font color, can be str like
-blue, orange... or HEX color animate: Optional bool, default is True, activate
-or not the animation animateDuration: Optional int, default is 2000, the
-animation duration in milliseconds progressValue: Optional int, default is 100,
-the progress bar completion, from 0 to 100 iconOpacity: Optional int, default
-is 50, the opacity of the icon, from 0 to 100, 0 is invisible iconTop: Optional
-int, default is 47, the icon position from the top, from 0 to 100 iconLeft:
-Optional int, default is 100, the icon position from the left, from 0 to 100
-showProgress: Optional bool, default is True, show or hide the progress bar
-showIcon: Optional bool, default is True, show or hide the icon height:
-Optional int, default is 250, the height of the whole widget """ ```
+# streamlit-kpi Streamlit component for displaying KPIs, easy layout to fit all
+your needs ! ![ScreenShot](https://raw.githubusercontent.com/aalteirac/
+streamlit-kpi/master/screen.png) ## Installation instructions ```sh pip install
+streamlit-kpi ``` ## Usage instructions ```python import streamlit as st from
+streamlit_kpi import streamlit_kpi streamlit_kpi
+(key="first_kpi",height='200',title='Monthly Sales',value=25000,icon='fa-solid
+fa-globe',progressValue=100,unit='Kâ¬') """ Parameters: key: Optional str,
+default is '', the streamlit component key, higly recommended title: Mandatory
+str, the title... value: Mandatory str or int or float, the value... icon:
+Optional str, default is 'fa-solid fa-globe', any Font Awesome class (v6.3).
+See https://fontawesome.com/search?o=r&m=free icon: Optional str, default is
+'', the value unit appended after the value textAlign: Optional str, default is
+'left', title and value alignement backgroundColor: Optional str, default is
+'#f3f3f3', widget background color can be str like blue, orange, transparent...
+or HEX color titleColor: Optional str, default is 'dark', title font color, can
+be str like blue, orange... or HEX color valueColor: Optional str, default is
+'dark', value font color, can be str like blue, orange... or HEX color
+progressColor: Optional str, default is 'green', progress color, can be str
+like blue, orange... or HEX color iconColor: Optional str, default is 'black',
+icon font color, can be str like blue, orange... or HEX color animate: Optional
+bool, default is True, activate or not the animation animateDuration: Optional
+int, default is 2000, the animation duration in milliseconds progressValue:
+Optional int, default is 100, the progress bar completion, from 0 to 100
+iconOpacity: Optional int, default is 50, the opacity of the icon, from 0 to
+100, 0 is invisible iconTop: Optional int, default is 47, the icon position
+from the top, from 0 to 100 iconLeft: Optional int, default is 100, the icon
+position from the left, from 0 to 100 showProgress: Optional bool, default is
+True, show or hide the progress bar showIcon: Optional bool, default is True,
+show or hide the icon height: Optional int, default is 250, the height of the
+whole widget """ ```
```

### Comparing `streamlit-kpi-0.0.8/README.md` & `streamlit-kpi-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 ## Test it Live !
 <a href="https://aalteirac-kpi.streamlit.app/" title="3d-badge"><img src="https://static.streamlit.io/badges/streamlit_badge_black_white.svg"></a><br>
 
 # streamlit-kpi
 
-Streamlit component for displaying KPIs
+Streamlit component for displaying KPIs, easy layout to fit all your needs !
+
+![ScreenShot](https://raw.githubusercontent.com/aalteirac/streamlit-kpi/master/screen.png)
 
 ## Installation instructions 
 
 ```sh
 pip install streamlit-kpi
 ```
```

#### html2text {}

```diff
@@ -1,30 +1,32 @@
 ## Test it Live ! [https://static.streamlit.io/badges/
 streamlit_badge_black_white.svg]
-# streamlit-kpi Streamlit component for displaying KPIs ## Installation
-instructions ```sh pip install streamlit-kpi ``` ## Usage instructions
-```python import streamlit as st from streamlit_kpi import streamlit_kpi
-streamlit_kpi(key="first_kpi",height='200',title='Monthly
-Sales',value=25000,icon='fa-solid fa-globe',progressValue=100,unit='Kâ¬') """
-Parameters: key: Optional str, default is '', the streamlit component key,
-higly recommended title: Mandatory str, the title... value: Mandatory str or
-int or float, the value... icon: Optional str, default is 'fa-solid fa-globe',
-any Font Awesome class (v6.3). See https://fontawesome.com/search?o=r&m=free
-icon: Optional str, default is '', the value unit appended after the value
-textAlign: Optional str, default is 'left', title and value alignement
-backgroundColor: Optional str, default is '#f3f3f3', widget background color
-can be str like blue, orange, transparent... or HEX color titleColor: Optional
-str, default is 'dark', title font color, can be str like blue, orange... or
-HEX color valueColor: Optional str, default is 'dark', value font color, can be
-str like blue, orange... or HEX color progressColor: Optional str, default is
-'green', progress color, can be str like blue, orange... or HEX color
-iconColor: Optional str, default is 'black', icon font color, can be str like
-blue, orange... or HEX color animate: Optional bool, default is True, activate
-or not the animation animateDuration: Optional int, default is 2000, the
-animation duration in milliseconds progressValue: Optional int, default is 100,
-the progress bar completion, from 0 to 100 iconOpacity: Optional int, default
-is 50, the opacity of the icon, from 0 to 100, 0 is invisible iconTop: Optional
-int, default is 47, the icon position from the top, from 0 to 100 iconLeft:
-Optional int, default is 100, the icon position from the left, from 0 to 100
-showProgress: Optional bool, default is True, show or hide the progress bar
-showIcon: Optional bool, default is True, show or hide the icon height:
-Optional int, default is 250, the height of the whole widget """ ```
+# streamlit-kpi Streamlit component for displaying KPIs, easy layout to fit all
+your needs ! ![ScreenShot](https://raw.githubusercontent.com/aalteirac/
+streamlit-kpi/master/screen.png) ## Installation instructions ```sh pip install
+streamlit-kpi ``` ## Usage instructions ```python import streamlit as st from
+streamlit_kpi import streamlit_kpi streamlit_kpi
+(key="first_kpi",height='200',title='Monthly Sales',value=25000,icon='fa-solid
+fa-globe',progressValue=100,unit='Kâ¬') """ Parameters: key: Optional str,
+default is '', the streamlit component key, higly recommended title: Mandatory
+str, the title... value: Mandatory str or int or float, the value... icon:
+Optional str, default is 'fa-solid fa-globe', any Font Awesome class (v6.3).
+See https://fontawesome.com/search?o=r&m=free icon: Optional str, default is
+'', the value unit appended after the value textAlign: Optional str, default is
+'left', title and value alignement backgroundColor: Optional str, default is
+'#f3f3f3', widget background color can be str like blue, orange, transparent...
+or HEX color titleColor: Optional str, default is 'dark', title font color, can
+be str like blue, orange... or HEX color valueColor: Optional str, default is
+'dark', value font color, can be str like blue, orange... or HEX color
+progressColor: Optional str, default is 'green', progress color, can be str
+like blue, orange... or HEX color iconColor: Optional str, default is 'black',
+icon font color, can be str like blue, orange... or HEX color animate: Optional
+bool, default is True, activate or not the animation animateDuration: Optional
+int, default is 2000, the animation duration in milliseconds progressValue:
+Optional int, default is 100, the progress bar completion, from 0 to 100
+iconOpacity: Optional int, default is 50, the opacity of the icon, from 0 to
+100, 0 is invisible iconTop: Optional int, default is 47, the icon position
+from the top, from 0 to 100 iconLeft: Optional int, default is 100, the icon
+position from the left, from 0 to 100 showProgress: Optional bool, default is
+True, show or hide the progress bar showIcon: Optional bool, default is True,
+show or hide the icon height: Optional int, default is 250, the height of the
+whole widget """ ```
```

### Comparing `streamlit-kpi-0.0.8/setup.py` & `streamlit-kpi-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-kpi",
     #begin 
-    version="0.0.8", 
+    version="0.0.9", 
     #end
     author="Anthony Alteirac",
     author_email="anthony@alteirac.com",
     description="Streamlit component for displaying KPI's",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
```

### Comparing `streamlit-kpi-0.0.8/src/streamlit_kpi/__init__.py` & `streamlit-kpi-0.0.9/src/streamlit_kpi/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-kpi-0.0.8/src/streamlit_kpi/frontend/index.html` & `streamlit-kpi-0.0.9/src/streamlit_kpi/frontend/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-kpi-0.0.8/src/streamlit_kpi/frontend/main.js` & `streamlit-kpi-0.0.9/src/streamlit_kpi/frontend/main.js`

 * *Files identical despite different names*

### Comparing `streamlit-kpi-0.0.8/src/streamlit_kpi/frontend/streamlit-component-lib.js` & `streamlit-kpi-0.0.9/src/streamlit_kpi/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-kpi-0.0.8/src/streamlit_kpi/frontend/style.css` & `streamlit-kpi-0.0.9/src/streamlit_kpi/frontend/style.css`

 * *Files identical despite different names*

### Comparing `streamlit-kpi-0.0.8/src/streamlit_kpi.egg-info/PKG-INFO` & `streamlit-kpi-0.0.9/src/streamlit_kpi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: streamlit-kpi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Streamlit component for displaying KPI's
 Author: Anthony Alteirac
 Author-email: anthony@alteirac.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Test it Live !
 <a href="https://aalteirac-kpi.streamlit.app/" title="3d-badge"><img src="https://static.streamlit.io/badges/streamlit_badge_black_white.svg"></a><br>
 
 # streamlit-kpi
 
-Streamlit component for displaying KPIs
+Streamlit component for displaying KPIs, easy layout to fit all your needs !
+
+![ScreenShot](https://raw.githubusercontent.com/aalteirac/streamlit-kpi/master/screen.png)
 
 ## Installation instructions 
 
 ```sh
 pip install streamlit-kpi
 ```
```

#### html2text {}

```diff
@@ -1,33 +1,35 @@
-Metadata-Version: 2.1 Name: streamlit-kpi Version: 0.0.8 Summary: Streamlit
+Metadata-Version: 2.1 Name: streamlit-kpi Version: 0.0.9 Summary: Streamlit
 component for displaying KPI's Author: Anthony Alteirac Author-email:
 anthony@alteirac.com Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE ## Test it Live ! [https://static.streamlit.io/
 badges/streamlit_badge_black_white.svg]
-# streamlit-kpi Streamlit component for displaying KPIs ## Installation
-instructions ```sh pip install streamlit-kpi ``` ## Usage instructions
-```python import streamlit as st from streamlit_kpi import streamlit_kpi
-streamlit_kpi(key="first_kpi",height='200',title='Monthly
-Sales',value=25000,icon='fa-solid fa-globe',progressValue=100,unit='Kâ¬') """
-Parameters: key: Optional str, default is '', the streamlit component key,
-higly recommended title: Mandatory str, the title... value: Mandatory str or
-int or float, the value... icon: Optional str, default is 'fa-solid fa-globe',
-any Font Awesome class (v6.3). See https://fontawesome.com/search?o=r&m=free
-icon: Optional str, default is '', the value unit appended after the value
-textAlign: Optional str, default is 'left', title and value alignement
-backgroundColor: Optional str, default is '#f3f3f3', widget background color
-can be str like blue, orange, transparent... or HEX color titleColor: Optional
-str, default is 'dark', title font color, can be str like blue, orange... or
-HEX color valueColor: Optional str, default is 'dark', value font color, can be
-str like blue, orange... or HEX color progressColor: Optional str, default is
-'green', progress color, can be str like blue, orange... or HEX color
-iconColor: Optional str, default is 'black', icon font color, can be str like
-blue, orange... or HEX color animate: Optional bool, default is True, activate
-or not the animation animateDuration: Optional int, default is 2000, the
-animation duration in milliseconds progressValue: Optional int, default is 100,
-the progress bar completion, from 0 to 100 iconOpacity: Optional int, default
-is 50, the opacity of the icon, from 0 to 100, 0 is invisible iconTop: Optional
-int, default is 47, the icon position from the top, from 0 to 100 iconLeft:
-Optional int, default is 100, the icon position from the left, from 0 to 100
-showProgress: Optional bool, default is True, show or hide the progress bar
-showIcon: Optional bool, default is True, show or hide the icon height:
-Optional int, default is 250, the height of the whole widget """ ```
+# streamlit-kpi Streamlit component for displaying KPIs, easy layout to fit all
+your needs ! ![ScreenShot](https://raw.githubusercontent.com/aalteirac/
+streamlit-kpi/master/screen.png) ## Installation instructions ```sh pip install
+streamlit-kpi ``` ## Usage instructions ```python import streamlit as st from
+streamlit_kpi import streamlit_kpi streamlit_kpi
+(key="first_kpi",height='200',title='Monthly Sales',value=25000,icon='fa-solid
+fa-globe',progressValue=100,unit='Kâ¬') """ Parameters: key: Optional str,
+default is '', the streamlit component key, higly recommended title: Mandatory
+str, the title... value: Mandatory str or int or float, the value... icon:
+Optional str, default is 'fa-solid fa-globe', any Font Awesome class (v6.3).
+See https://fontawesome.com/search?o=r&m=free icon: Optional str, default is
+'', the value unit appended after the value textAlign: Optional str, default is
+'left', title and value alignement backgroundColor: Optional str, default is
+'#f3f3f3', widget background color can be str like blue, orange, transparent...
+or HEX color titleColor: Optional str, default is 'dark', title font color, can
+be str like blue, orange... or HEX color valueColor: Optional str, default is
+'dark', value font color, can be str like blue, orange... or HEX color
+progressColor: Optional str, default is 'green', progress color, can be str
+like blue, orange... or HEX color iconColor: Optional str, default is 'black',
+icon font color, can be str like blue, orange... or HEX color animate: Optional
+bool, default is True, activate or not the animation animateDuration: Optional
+int, default is 2000, the animation duration in milliseconds progressValue:
+Optional int, default is 100, the progress bar completion, from 0 to 100
+iconOpacity: Optional int, default is 50, the opacity of the icon, from 0 to
+100, 0 is invisible iconTop: Optional int, default is 47, the icon position
+from the top, from 0 to 100 iconLeft: Optional int, default is 100, the icon
+position from the left, from 0 to 100 showProgress: Optional bool, default is
+True, show or hide the progress bar showIcon: Optional bool, default is True,
+show or hide the icon height: Optional int, default is 250, the height of the
+whole widget """ ```
```

