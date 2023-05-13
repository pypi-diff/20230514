# Comparing `tmp/mrfix-1.0.4.tar.gz` & `tmp/mrfix-1.0.5.tar.gz`

## Comparing `mrfix-1.0.4.tar` & `mrfix-1.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-1.0.4/LICENZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-1.0.4/src/mrfix/__init__.py
--rw-r--r--   0        0        0    13255 2020-02-02 00:00:00.000000 mrfix-1.0.4/src/mrfix/mrfix.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-1.0.4/.gitignore
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 mrfix-1.0.4/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 mrfix-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-1.0.5/LICENZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-1.0.5/src/mrfix/__init__.py
+-rw-r--r--   0        0        0    14011 2020-02-02 00:00:00.000000 mrfix-1.0.5/src/mrfix/mrfix.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-1.0.5/.gitignore
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 mrfix-1.0.5/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 mrfix-1.0.5/PKG-INFO
```

### Comparing `mrfix-1.0.4/LICENZE` & `mrfix-1.0.5/LICENZE`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.4/src/mrfix/mrfix.py` & `mrfix-1.0.5/src/mrfix/mrfix.py`

 * *Files 4% similar despite different names*

```diff
@@ -327,35 +327,51 @@
         try:
             self.find_element_by_partial_link_text(text).click()
             return True
         except NoSuchElementException:
             return False
 
 
-    def for_down_make_element_displayed_and_click(self, xpath_element):
-        while not MrFixUI.check_displayed_element(self, xpath_element):
+    def for_down_make_element_displayed_and_click(self, xpath_element, time_in_second):
+        start_time = time.time()
+        delta_time = 0
+        while not MrFixUI.check_displayed_element(self, xpath_element) and delta_time <= time_in_second:
             MrFixUI.pressing_down_arrow_key(self, 1)
+            stop_time = time.time()
+            delta_time = stop_time - start_time
         MrFixUI.click_element(self, xpath_element)
 
 
-    def for_up_make_element_displayed_and_click(self, xpath_element):
-        while not MrFixUI.check_displayed_element(self, xpath_element):
+    def for_up_make_element_displayed_and_click(self, xpath_element, time_in_second):
+        start_time = time.time()
+        delta_time = 0
+        while not MrFixUI.check_displayed_element(self, xpath_element) and delta_time <= time_in_second:
             MrFixUI.pressing_up_arrow_key(self, 1)
+            stop_time = time.time()
+            delta_time = stop_time - start_time
         MrFixUI.click_element(self, xpath_element)
 
 
-    def for_down_make_element_displayed_and_send(self, xpath_element, send_text):
-        while not MrFixUI.check_displayed_element(self, xpath_element):
+    def for_down_make_element_displayed_and_send(self, xpath_element, send_text, time_in_second):
+        start_time = time.time()
+        delta_time = 0
+        while not MrFixUI.check_displayed_element(self, xpath_element) and delta_time <= time_in_second:
             MrFixUI.pressing_down_arrow_key(self, 1)
+            stop_time = time.time()
+            delta_time = stop_time - start_time
         MrFixUI.send_input_text(self, xpath_element, send_text)
 
 
-    def for_up_make_element_displayed_and_send(self, xpath_element, send_text):
-        while not MrFixUI.check_displayed_element(self, xpath_element):
+    def for_up_make_element_displayed_and_send(self, xpath_element, send_text, time_in_second):
+        start_time = time.time()
+        delta_time = 0
+        while not MrFixUI.check_displayed_element(self, xpath_element) and delta_time <= time_in_second:
             MrFixUI.pressing_up_arrow_key(self, 1)
+            stop_time = time.time()
+            delta_time = stop_time - start_time
         MrFixUI.send_input_text(self, xpath_element, send_text)
 
 
     def find_href_on_page(self, link):
         link_availability = False
         if MrFixUI.check_exists_xpath(self, "//a[@href]") == True:
             elems = self.find_element(By.XPATH, "//a[@href]")
```

### Comparing `mrfix-1.0.4/.gitignore` & `mrfix-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.4/README.md` & `mrfix-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.4/pyproject.toml` & `mrfix-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system] 
 requires = ["hatchling"] 
 build-backend = "hatchling.build"
 
 [project] 
 name = "mrfix"
-version = "1.0.4"
+version = "1.0.5"
 authors = [   
   { name="Valerii Zhuravlev", email="valerzhurav2011@gmail.com" },
 ] 
 description = "A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium"
 readme = "README.md" 
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mrfix-1.0.4/PKG-INFO` & `mrfix-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrfix
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium
 Project-URL: Homepage, https://github.com/MrFix-Autotesting-Framework
 Author-email: Valerii Zhuravlev <valerzhurav2011@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

