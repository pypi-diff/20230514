# Comparing `tmp/devblaze-0.0.1.tar.gz` & `tmp/devblaze-0.0.2.tar.gz`

## Comparing `devblaze-0.0.1.tar` & `devblaze-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 devblaze-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 devblaze-0.0.1/Makefile
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 devblaze-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 devblaze-0.0.1/.idea/devblaze.iml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 devblaze-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devblaze-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 devblaze-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 devblaze-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 devblaze-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 devblaze-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devblaze-0.0.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 devblaze-0.0.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.1/.ruff_cache/content/2f88094502ec7f89
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.1/.ruff_cache/content/35fe71a4dd87ac17
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.1/.ruff_cache/content/5eb4f5434501f633
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.1/.ruff_cache/content/609322798689986d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.1/.ruff_cache/content/75c6f13fc972def1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.1/.ruff_cache/content/7b71c0436bbfd443
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.1/.ruff_cache/content/99e45b1bd08c7e6a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.1/.ruff_cache/content/a71860a9be908f3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.1/.ruff_cache/content/aa0d0bc3ca67ba4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.1/.ruff_cache/content/d62bd5c9e0fb954f
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 devblaze-0.0.1/devblaze/__init__.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 devblaze-0.0.1/devblaze/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devblaze-0.0.1/devblaze/textual_utils/__init__.py
--rw-r--r--   0        0        0     9770 2020-02-02 00:00:00.000000 devblaze-0.0.1/devblaze/textual_utils/screen.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 devblaze-0.0.1/devblaze/textual_utils/static/cookiecutter.css
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 devblaze-0.0.1/scripts/format.sh
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 devblaze-0.0.1/scripts/lint.sh
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 devblaze-0.0.1/scripts/test.sh
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 devblaze-0.0.1/tests/test_version.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 devblaze-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 devblaze-0.0.1/LICENSE
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 devblaze-0.0.1/README.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 devblaze-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 devblaze-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 devblaze-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 devblaze-0.0.2/Makefile
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 devblaze-0.0.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/devblaze.iml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 devblaze-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/2f88094502ec7f89
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/35fe71a4dd87ac17
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/5eb4f5434501f633
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/609322798689986d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/75c6f13fc972def1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/7b71c0436bbfd443
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/99e45b1bd08c7e6a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/a71860a9be908f3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/aa0d0bc3ca67ba4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 devblaze-0.0.2/.ruff_cache/content/d62bd5c9e0fb954f
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 devblaze-0.0.2/devblaze/__init__.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 devblaze-0.0.2/devblaze/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devblaze-0.0.2/devblaze/textual_utils/__init__.py
+-rw-r--r--   0        0        0     9770 2020-02-02 00:00:00.000000 devblaze-0.0.2/devblaze/textual_utils/screen.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 devblaze-0.0.2/devblaze/textual_utils/static/cookiecutter.css
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 devblaze-0.0.2/scripts/format.sh
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 devblaze-0.0.2/scripts/lint.sh
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 devblaze-0.0.2/scripts/test.sh
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 devblaze-0.0.2/tests/test_version.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 devblaze-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 devblaze-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 devblaze-0.0.2/README.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 devblaze-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 devblaze-0.0.2/PKG-INFO
```

### Comparing `devblaze-0.0.1/CONTRIBUTING.md` & `devblaze-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.1/.idea/workspace.xml` & `devblaze-0.0.2/.idea/workspace.xml`

 * *Files 20% similar despite different names*

#### Comparing `devblaze-0.0.1/.idea/workspace.xml` & `devblaze-0.0.2/.idea/workspace.xml`

```diff
@@ -1,19 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="d840212d-598e-4435-aba3-358a7098e15e" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/.idea/devblaze.iml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/devblaze.iml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/devblaze/main.py" beforeDir="false" afterPath="$PROJECT_DIR$/devblaze/main.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/devblaze/textual/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/devblaze/textual_utils/__init__.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/devblaze/textual/screen.py" beforeDir="false" afterPath="$PROJECT_DIR$/devblaze/textual_utils/screen.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/devblaze/textual/static/cookiecutter.css" beforeDir="false" afterPath="$PROJECT_DIR$/devblaze/textual_utils/static/cookiecutter.css" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -68,15 +64,15 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="d840212d-598e-4435-aba3-358a7098e15e" name="Changes" comment=""/>
       <created>1684009865090</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1684009865090</updated>
-      <workItem from="1684009866089" duration="5798000"/>
+      <workItem from="1684009866089" duration="6828000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
 </project>
```

### Comparing `devblaze-0.0.1/.idea/inspectionProfiles/Project_Default.xml` & `devblaze-0.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.1/devblaze/main.py` & `devblaze-0.0.2/devblaze/main.py`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.1/devblaze/textual_utils/screen.py` & `devblaze-0.0.2/devblaze/textual_utils/screen.py`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.1/devblaze/textual_utils/static/cookiecutter.css` & `devblaze-0.0.2/devblaze/textual_utils/static/cookiecutter.css`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.1/.gitignore` & `devblaze-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.1/LICENSE` & `devblaze-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.1/README.md` & `devblaze-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,12 +31,12 @@
 
 ## Why DevBlaze?
 
 Traditional cookiecutter templates are great, but DevBlaze takes it a step further. By leveraging the Textual library, DevBlaze provides a more interactive and user-friendly interface, making the process of creating new Django projects even easier and more enjoyable.
    
 ## Contributing
 
-Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for more details.
+Contributions are welcome! Please see [CONTRIBUTING.md](https://github.com/godd0t/devblaze/blob/main/CONTRIBUTING.md) for more details.
 
 ## License
 
-DevBlaze is licensed under the [MIT License](LICENSE).
+DevBlaze is licensed under the [MIT License](https://github.com/godd0t/devblaze/blob/main/LICENSE).
```

### Comparing `devblaze-0.0.1/pyproject.toml` & `devblaze-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devblaze-0.0.1/PKG-INFO` & `devblaze-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devblaze
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool for creating and managing development and production environments.
 License: MIT License
         
         Copyright (c) 2023 Lirim Shala
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -76,12 +76,12 @@
 
 ## Why DevBlaze?
 
 Traditional cookiecutter templates are great, but DevBlaze takes it a step further. By leveraging the Textual library, DevBlaze provides a more interactive and user-friendly interface, making the process of creating new Django projects even easier and more enjoyable.
    
 ## Contributing
 
-Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for more details.
+Contributions are welcome! Please see [CONTRIBUTING.md](https://github.com/godd0t/devblaze/blob/main/CONTRIBUTING.md) for more details.
 
 ## License
 
-DevBlaze is licensed under the [MIT License](LICENSE).
+DevBlaze is licensed under the [MIT License](https://github.com/godd0t/devblaze/blob/main/LICENSE).
```

