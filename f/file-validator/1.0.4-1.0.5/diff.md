# Comparing `tmp/file_validator-1.0.4.tar.gz` & `tmp/file_validator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\Progamming Project\file-validator\dist\.tmp-s6uepjsh\file_validator-1.0.4.tar", last modified: Sat Mar 25 06:04:49 2023, max compression
+gzip compressed data, was "F:\Progamming Project\file-validator\dist\.tmp-bu9hge84\file_validator-1.0.5.tar", last modified: Sun May 14 21:26:04 2023, max compression
```

## Comparing `file_validator-1.0.4.tar` & `file_validator-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 06:04:49.408696 file_validator-1.0.4/
--rw-rw-rw-   0        0        0      115 2023-03-23 16:55:55.000000 file_validator-1.0.4/AUTHORS.md
--rw-rw-rw-   0        0        0     2474 2023-03-23 16:55:55.000000 file_validator-1.0.4/CONTRIBUTING.md
--rw-rw-rw-   0        0        0      162 2023-03-23 16:55:55.000000 file_validator-1.0.4/HISTORY.md
--rw-rw-rw-   0        0        0     1091 2023-03-23 16:55:55.000000 file_validator-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      310 2023-03-23 16:55:55.000000 file_validator-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     7939 2023-03-25 06:04:49.409694 file_validator-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6080 2023-03-23 16:55:55.000000 file_validator-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-25 06:04:49.360700 file_validator-1.0.4/file_validator/
--rw-rw-rw-   0        0        0      141 2023-03-25 06:03:46.000000 file_validator-1.0.4/file_validator/__init__.py
--rw-rw-rw-   0        0        0     2765 2023-03-24 20:22:40.000000 file_validator-1.0.4/file_validator/constants.py
--rw-rw-rw-   0        0        0     3978 2023-03-24 17:55:46.000000 file_validator-1.0.4/file_validator/exceptions.py
--rw-rw-rw-   0        0        0      807 2023-03-23 16:55:55.000000 file_validator-1.0.4/file_validator/forms.py
--rw-rw-rw-   0        0        0    13071 2023-03-25 06:03:45.000000 file_validator-1.0.4/file_validator/models.py
-drwxrwxrwx   0        0        0        0 2023-03-25 06:04:49.248698 file_validator-1.0.4/file_validator/templates/
-drwxrwxrwx   0        0        0        0 2023-03-25 06:04:49.391694 file_validator-1.0.4/file_validator/templates/file_validator/
--rw-rw-rw-   0        0        0      127 2023-03-23 16:55:55.000000 file_validator-1.0.4/file_validator/templates/file_validator/file_input_widget.html
--rw-rw-rw-   0        0        0     4204 2023-03-24 17:42:59.000000 file_validator-1.0.4/file_validator/utils.py
--rw-rw-rw-   0        0        0    16159 2023-03-24 19:32:40.000000 file_validator-1.0.4/file_validator/validators.py
--rw-rw-rw-   0        0        0      214 2023-03-23 16:55:55.000000 file_validator-1.0.4/file_validator/widgets.py
-drwxrwxrwx   0        0        0        0 2023-03-25 06:04:49.390695 file_validator-1.0.4/file_validator.egg-info/
--rw-rw-rw-   0        0        0     7939 2023-03-25 06:04:49.000000 file_validator-1.0.4/file_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-03-25 06:04:49.000000 file_validator-1.0.4/file_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 06:04:49.000000 file_validator-1.0.4/file_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-03-25 06:04:49.000000 file_validator-1.0.4/file_validator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-25 06:04:48.000000 file_validator-1.0.4/file_validator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      206 2023-03-25 06:04:49.000000 file_validator-1.0.4/file_validator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-25 06:04:49.000000 file_validator-1.0.4/file_validator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      846 2023-03-25 06:04:49.410700 file_validator-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2860 2023-03-25 06:03:46.000000 file_validator-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 21:26:04.150998 file_validator-1.0.5/
+-rw-rw-rw-   0        0        0      115 2023-03-23 16:55:55.000000 file_validator-1.0.5/AUTHORS.md
+-rw-rw-rw-   0        0        0     2474 2023-03-23 16:55:55.000000 file_validator-1.0.5/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0      162 2023-03-23 16:55:55.000000 file_validator-1.0.5/HISTORY.md
+-rw-rw-rw-   0        0        0     1091 2023-03-23 16:55:55.000000 file_validator-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      310 2023-03-23 16:55:55.000000 file_validator-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     8148 2023-05-14 21:26:04.150998 file_validator-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6289 2023-05-14 21:22:48.000000 file_validator-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 21:26:04.140994 file_validator-1.0.5/file_validator/
+-rw-rw-rw-   0        0        0      136 2023-05-14 21:24:59.000000 file_validator-1.0.5/file_validator/__init__.py
+-rw-rw-rw-   0        0        0     2765 2023-03-30 15:19:51.000000 file_validator-1.0.5/file_validator/constants.py
+-rw-rw-rw-   0        0        0     3978 2023-03-30 15:19:51.000000 file_validator-1.0.5/file_validator/exceptions.py
+-rw-rw-rw-   0        0        0      807 2023-05-14 21:22:48.000000 file_validator-1.0.5/file_validator/forms.py
+-rw-rw-rw-   0        0        0    13267 2023-05-14 21:22:48.000000 file_validator-1.0.5/file_validator/models.py
+drwxrwxrwx   0        0        0        0 2023-05-14 21:26:04.008122 file_validator-1.0.5/file_validator/templates/
+drwxrwxrwx   0        0        0        0 2023-05-14 21:26:04.149992 file_validator-1.0.5/file_validator/templates/file_validator/
+-rw-rw-rw-   0        0        0      127 2023-03-23 16:55:55.000000 file_validator-1.0.5/file_validator/templates/file_validator/file_input_widget.html
+-rw-rw-rw-   0        0        0     4204 2023-05-14 21:22:48.000000 file_validator-1.0.5/file_validator/utils.py
+-rw-rw-rw-   0        0        0    16723 2023-05-14 21:22:48.000000 file_validator-1.0.5/file_validator/validators.py
+-rw-rw-rw-   0        0        0      214 2023-05-14 21:22:48.000000 file_validator-1.0.5/file_validator/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-14 21:26:04.148997 file_validator-1.0.5/file_validator.egg-info/
+-rw-rw-rw-   0        0        0     8148 2023-05-14 21:26:03.000000 file_validator-1.0.5/file_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-05-14 21:26:04.000000 file_validator-1.0.5/file_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 21:26:03.000000 file_validator-1.0.5/file_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-14 21:26:03.000000 file_validator-1.0.5/file_validator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-14 21:26:03.000000 file_validator-1.0.5/file_validator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      206 2023-05-14 21:26:03.000000 file_validator-1.0.5/file_validator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-14 21:26:03.000000 file_validator-1.0.5/file_validator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      846 2023-05-14 21:26:04.152994 file_validator-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2774 2023-05-14 21:24:59.000000 file_validator-1.0.5/setup.py
```

### Comparing `file_validator-1.0.4/CONTRIBUTING.md` & `file_validator-1.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.4/LICENSE` & `file_validator-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.4/PKG-INFO` & `file_validator-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_validator
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python validation library to validate files using type, mime, extension, magic numbers and size ✅
 Home-page: https://github.com/file-validator/file-validator
 Author: Reza Shakeri
 Author-email: rzashakeri@outlook.com
 License: MIT license
 Project-URL: Documentation, https://file-validator.github.io/
 Project-URL: Homepage, https://github.com/file-validator
@@ -64,14 +64,15 @@
 [![CodeFactor](https://www.codefactor.io/repository/github/file-validator/file-validator/badge)](https://www.codefactor.io/repository/github/file-validator/file-validator)
 [![black](https://github.com/file-validator/file-validator/actions/workflows/black.yml/badge.svg?branch=master)](https://github.com/file-validator/file-validator/actions/workflows/black.yml)
 [![docs](https://github.com/file-validator/file-validator/actions/workflows/deploy.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/deploy.yml)
 [![Pylint](https://github.com/file-validator/file-validator/actions/workflows/pylint.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/pylint.yml)
 [![Workflow for Codecov](https://github.com/file-validator/file-validator/actions/workflows/Codecov.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/Codecov.yml)
 [![Python package](https://github.com/file-validator/file-validator/actions/workflows/python-package.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/python-package.yml)
 [![CodeQL](https://github.com/file-validator/file-validator/actions/workflows/codeql.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/codeql.yml)
+[![Percentage of issues still open](http://isitmaintained.com/badge/open/file-validator/file-validator.svg)](http://isitmaintained.com/project/file-validator/file-validator "Percentage of issues still open")
 
 ## What Is File Validator? ✅
 
 It is a Python library for file validation based on **MIME**, **size**, **type** and **magic numbers** that supports Django.
 
 ## Why should we use this library? 🧐
```

### Comparing `file_validator-1.0.4/README.md` & `file_validator-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 [![CodeFactor](https://www.codefactor.io/repository/github/file-validator/file-validator/badge)](https://www.codefactor.io/repository/github/file-validator/file-validator)
 [![black](https://github.com/file-validator/file-validator/actions/workflows/black.yml/badge.svg?branch=master)](https://github.com/file-validator/file-validator/actions/workflows/black.yml)
 [![docs](https://github.com/file-validator/file-validator/actions/workflows/deploy.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/deploy.yml)
 [![Pylint](https://github.com/file-validator/file-validator/actions/workflows/pylint.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/pylint.yml)
 [![Workflow for Codecov](https://github.com/file-validator/file-validator/actions/workflows/Codecov.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/Codecov.yml)
 [![Python package](https://github.com/file-validator/file-validator/actions/workflows/python-package.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/python-package.yml)
 [![CodeQL](https://github.com/file-validator/file-validator/actions/workflows/codeql.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/codeql.yml)
+[![Percentage of issues still open](http://isitmaintained.com/badge/open/file-validator/file-validator.svg)](http://isitmaintained.com/project/file-validator/file-validator "Percentage of issues still open")
 
 ## What Is File Validator? ✅
 
 It is a Python library for file validation based on **MIME**, **size**, **type** and **magic numbers** that supports Django.
 
 ## Why should we use this library? 🧐
```

### Comparing `file_validator-1.0.4/file_validator/constants.py` & `file_validator-1.0.5/file_validator/constants.py`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.4/file_validator/exceptions.py` & `file_validator-1.0.5/file_validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.4/file_validator/forms.py` & `file_validator-1.0.5/file_validator/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""this file provides forms for django."""
+"""This file provides forms for django."""
 from django import forms
 
 from file_validator.widgets import FileInputWidget
 
 
 class ValidatedFileField(forms.FileField):
-    """validated file filed for django."""
+    """Validated file filed for django."""
 
     widget = FileInputWidget
 
     def __init__(self, *, accept=None, custom_css_class=None, multiple=None, **kwargs):
         self.accept = accept
         self.multiple = multiple
         self.custom_css_class = custom_css_class
```

### Comparing `file_validator-1.0.4/file_validator/models.py` & `file_validator-1.0.5/file_validator/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,18 @@
         kwargs["libraries"] = self.libraries
         kwargs["max_upload_file_size"] = self.max_upload_file_size
         return name, path, args, kwargs
 
     def clean(self, *args, **kwargs):
         data = super().clean(*args, **kwargs)
         current_file = data.file
-        file_mime_guessed_by_django = current_file.content_type
+        try:
+            file_mime_guessed_by_django = current_file.content_type
+        except AttributeError:
+            file_mime_guessed_by_django = None
         file_size = data.size
         file_path = TemporaryUploadedFile.temporary_file_path(current_file)
         try:
             file_validator = FileValidator(
                 file_path=file_path,
                 libraries=self.libraries,
                 acceptable_mimes=self.acceptable_mimes,
@@ -145,15 +148,15 @@
             ) from error
         setattr(data, "validation_data", file_validator.result_of_validation)
         return data
 
 
 @deconstructible
 class DjangoFileValidator:
-    """file validator for django."""
+    """File validator for django."""
 
     def __init__(
         self,
         libraries: list = None,
         acceptable_mimes: list = None,
         acceptable_types: list = None,
         max_upload_file_size: int = None,
@@ -201,15 +204,18 @@
 
         is_type_supported(acceptable_types=self.acceptable_types)
 
     def __call__(self, value):
         current_file = value.file
         file_size = value.size
         file_path = TemporaryUploadedFile.temporary_file_path(current_file)
-        file_mime_guessed_by_django = current_file.content_type
+        try:
+            file_mime_guessed_by_django = current_file.content_type
+        except AttributeError:
+            file_mime_guessed_by_django = None
         try:
             file_validator = FileValidator(
                 file_path=file_path,
                 libraries=self.libraries,
                 acceptable_mimes=self.acceptable_mimes,
                 acceptable_types=self.acceptable_types,
                 max_upload_file_size=self.max_upload_file_size,
@@ -259,15 +265,15 @@
 
     def __hash__(self):
         return hash(self.max_upload_file_size)
 
 
 @deconstructible
 class FileSizeValidator:
-    """size validator for django."""
+    """Size validator for django."""
 
     def __init__(
         self,
         max_upload_file_size: int = None,
     ):
         """
         :type max_upload_file_size: int
```

### Comparing `file_validator-1.0.4/file_validator/utils.py` & `file_validator-1.0.5/file_validator/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""utils for file validator."""
+"""Utils for file validator."""
 from itertools import groupby
 
 from filetype import is_archive, is_audio, is_font, is_image, is_video
 from termcolor import colored
 
 from file_validator.constants import (
     ALL_SUPPORTED_LIBRARIES,
@@ -57,15 +57,15 @@
     status=None,
     library=None,
     file_name=None,
     file_extension=None,
     file_mime=None,
     **kwargs
 ) -> dict:
-    """generates information about file validated."""
+    """Generates information about file validated."""
     result = {}
     file_type = kwargs.get("file_type")
     if status is not None:
         result.update({"status": status})
     if library is not None:
         result.update({"library": library})
     if file_name is not None:
@@ -93,15 +93,15 @@
         return FONT
     if is_archive(file_path):
         return ARCHIVE
     return None
 
 
 def parameters_are_empty(acceptable_types: list, acceptable_mimes: list):
-    """this function check whether parameters are empty or no?"""
+    """This function check whether parameters are empty or no?"""
     if acceptable_types is None and acceptable_mimes is None:
         raise EmptyParametersException(colored(PARAMETERS_ARE_EMPTY, "red"))
 
 
 def is_type_supported(acceptable_types: list):
     """This function check whether the type is supported by file-validator
     library, List of supported types: font, audio, video, image, archive."""
```

### Comparing `file_validator-1.0.4/file_validator/validators.py` & `file_validator-1.0.5/file_validator/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,16 +91,16 @@
         current_file = Path(self.file_path)
         if (
             self.max_upload_file_size is not None
             and file_size > self.max_upload_file_size
         ):
             raise SizeValidationException(
                 error_message(
-                    current_file_name=current_file.name,
                     current_file_size=naturalsize(file_size),
+                    current_file_name=current_file.name,
                     max_file_size=naturalsize(self.max_upload_file_size),
                     message=FILE_SIZE_IS_NOT_VALID,
                 ),
             )
         result_of_validation = {
             "file_size": naturalsize(file_size),
             "max_upload_file_size": naturalsize(self.max_upload_file_size)
@@ -369,33 +369,44 @@
         )
         self.result_of_validation.update({FILETYPE: result_of_validation})
         return result_of_validation
 
     def django(self):
         """This method for validating file based on mime using data from
         django."""
-        current_file = Path(self.file_path)
-        file_type = self.file_mime_guessed_by_django.split("/")[0]
-        if self.file_mime_guessed_by_django not in self.acceptable_mimes:
-            raise FileValidationException(
-                colored(
-                    error_message(
-                        current_file_extension=current_file.suffix,
-                        current_file_name=current_file.name,
-                        current_file_mime=self.file_mime_guessed_by_django,
-                        current_file_type=file_type,
-                        acceptable_mimes=self.acceptable_mimes,
-                        acceptable_types=self.acceptable_types,
-                        acceptable_extensions=self.acceptable_extensions,
+        try:
+            current_file = Path(self.file_path)
+            file_type = self.file_mime_guessed_by_django.split("/")[0]
+            if self.file_mime_guessed_by_django not in self.acceptable_mimes:
+                raise FileValidationException(
+                    colored(
+                        error_message(
+                            current_file_extension=current_file.suffix,
+                            current_file_name=current_file.name,
+                            current_file_mime=self.file_mime_guessed_by_django,
+                            current_file_type=file_type,
+                            acceptable_mimes=self.acceptable_mimes,
+                            acceptable_types=self.acceptable_types,
+                            acceptable_extensions=self.acceptable_extensions,
+                        ),
+                        "red",
                     ),
-                    "red",
-                ),
+                )
+            result_of_validation = generate_information_about_file(
+                status=OK,
+                file_name=current_file.name,
+                file_mime=self.file_mime_guessed_by_django,
+                file_type=file_type,
+                file_extension=current_file.suffix,
             )
-        result_of_validation = generate_information_about_file(
-            status=OK,
-            file_name=current_file.name,
-            file_mime=self.file_mime_guessed_by_django,
-            file_type=file_type,
-            file_extension=current_file.suffix,
-        )
-        self.result_of_validation.update({DJANGO: result_of_validation})
-        return result_of_validation
+            self.result_of_validation.update({DJANGO: result_of_validation})
+            return result_of_validation
+        except AttributeError:
+            result_of_validation = generate_information_about_file(
+                status="Fail",
+                file_name=current_file.name,
+                file_mime="NOT_FOUND",
+                file_type="NOT_FOUND",
+                file_extension=current_file.suffix,
+            )
+            self.result_of_validation.update({DJANGO: result_of_validation})
+            return result_of_validation
```

### Comparing `file_validator-1.0.4/file_validator.egg-info/PKG-INFO` & `file_validator-1.0.5/file_validator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-validator
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python validation library to validate files using type, mime, extension, magic numbers and size ✅
 Home-page: https://github.com/file-validator/file-validator
 Author: Reza Shakeri
 Author-email: rzashakeri@outlook.com
 License: MIT license
 Project-URL: Documentation, https://file-validator.github.io/
 Project-URL: Homepage, https://github.com/file-validator
@@ -64,14 +64,15 @@
 [![CodeFactor](https://www.codefactor.io/repository/github/file-validator/file-validator/badge)](https://www.codefactor.io/repository/github/file-validator/file-validator)
 [![black](https://github.com/file-validator/file-validator/actions/workflows/black.yml/badge.svg?branch=master)](https://github.com/file-validator/file-validator/actions/workflows/black.yml)
 [![docs](https://github.com/file-validator/file-validator/actions/workflows/deploy.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/deploy.yml)
 [![Pylint](https://github.com/file-validator/file-validator/actions/workflows/pylint.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/pylint.yml)
 [![Workflow for Codecov](https://github.com/file-validator/file-validator/actions/workflows/Codecov.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/Codecov.yml)
 [![Python package](https://github.com/file-validator/file-validator/actions/workflows/python-package.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/python-package.yml)
 [![CodeQL](https://github.com/file-validator/file-validator/actions/workflows/codeql.yml/badge.svg)](https://github.com/file-validator/file-validator/actions/workflows/codeql.yml)
+[![Percentage of issues still open](http://isitmaintained.com/badge/open/file-validator/file-validator.svg)](http://isitmaintained.com/project/file-validator/file-validator "Percentage of issues still open")
 
 ## What Is File Validator? ✅
 
 It is a Python library for file validation based on **MIME**, **size**, **type** and **magic numbers** that supports Django.
 
 ## Why should we use this library? 🧐
```

### Comparing `file_validator-1.0.4/file_validator.egg-info/SOURCES.txt` & `file_validator-1.0.5/file_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.4/setup.cfg` & `file_validator-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.4
+current_version = 1.0.5
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `file_validator-1.0.4/setup.py` & `file_validator-1.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,84 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-from setuptools import find_packages, setup
-
-with open("README.md", encoding="utf-8") as readme_file:
-    readme = readme_file.read()
-
-with open("HISTORY.md", encoding="utf-8") as history_file:
-    history = history_file.read()
-
-requirements = [
-    "humanize==4.4.0",
-    "filetype==1.1.0",
-    "termcolor==1.1.0",
-    "puremagic==1.14",
-    "python-dotenv==0.21.1",
-    "django",
-    "python-magic-bin==0.4.14 ; platform_system == 'Windows'",
-    "python-magic==0.4.27 ; platform_system != 'Windows'",
-]
-
-
-test_requirements = [
-    "pytest>=3",
-]
-
-setup(
-    author="Reza Shakeri",
-    author_email="rzashakeri@outlook.com",
-    python_requires=">=3.8",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Natural Language :: English",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Framework :: Django",
-        "Topic :: Multimedia",
-        "Topic :: Multimedia :: Sound/Audio",
-        "Topic :: Multimedia :: Video",
-        "Topic :: Security",
-        "Topic :: Software Development :: Libraries",
-    ],
-    description="Python validation library to validate files "
-    "using type, mime, extension, magic numbers and size ✅",
-    entry_points={
-        "console_scripts": [
-            "file_validator=file_validator.cli:main",
-        ],
-    },
-    install_requires=requirements,
-    license="MIT license",
-    long_description=readme + "\n\n" + history,
-    long_description_content_type="text/markdown",
-    include_package_data=True,
-    keywords=[
-        "file_validator",
-        "file",
-        "validator",
-        "image_validator",
-        "audio_validator",
-        "video_validator",
-        "django",
-    ],
-    name="file_validator",
-    packages=find_packages(include=["file_validator", "file_validator.*"]),
-    test_suite="tests",
-    tests_require=test_requirements,
-    url="https://github.com/file-validator/file-validator",
-    version="1.0.4",
-    zip_safe=False,
-    project_urls={
-        "Documentation": "https://file-validator.github.io/",
-        "Homepage": "https://github.com/file-validator",
-        "Issue tracker": "https://github.com/file-validator/file-validator/issues",
-        "Release notes": "https://github.com/file-validator/file-validator/releases",
-        "Source": "https://github.com/file-validator/file-validator",
-        "Discussions": "https://github.com/orgs/file-validator/discussions",
-        "History Of Changes": "https://file-validator.github.io/docs/history/",
-    },
-)
+#!/usr/bin/env python
+"""The setup script."""
+from setuptools import find_packages, setup
+
+with open("README.md", encoding="utf-8") as readme_file:
+    readme = readme_file.read()
+
+with open("HISTORY.md", encoding="utf-8") as history_file:
+    history = history_file.read()
+
+requirements = [
+    "humanize==4.4.0",
+    "filetype==1.1.0",
+    "termcolor==1.1.0",
+    "puremagic==1.14",
+    "python-dotenv==0.21.1",
+    "django",
+    "python-magic-bin==0.4.14 ; platform_system == 'Windows'",
+    "python-magic==0.4.27 ; platform_system != 'Windows'",
+]
+
+
+test_requirements = [
+    "pytest>=3",
+]
+
+setup(
+    author="Reza Shakeri",
+    author_email="rzashakeri@outlook.com",
+    python_requires=">=3.8",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Framework :: Django",
+        "Topic :: Multimedia",
+        "Topic :: Multimedia :: Sound/Audio",
+        "Topic :: Multimedia :: Video",
+        "Topic :: Security",
+        "Topic :: Software Development :: Libraries",
+    ],
+    description="Python validation library to validate files "
+    "using type, mime, extension, magic numbers and size ✅",
+    entry_points={
+        "console_scripts": [
+            "file_validator=file_validator.cli:main",
+        ],
+    },
+    install_requires=requirements,
+    license="MIT license",
+    long_description=readme + "\n\n" + history,
+    long_description_content_type="text/markdown",
+    include_package_data=True,
+    keywords=[
+        "file_validator",
+        "file",
+        "validator",
+        "image_validator",
+        "audio_validator",
+        "video_validator",
+        "django",
+    ],
+    name="file_validator",
+    packages=find_packages(include=["file_validator", "file_validator.*"]),
+    test_suite="tests",
+    tests_require=test_requirements,
+    url="https://github.com/file-validator/file-validator",
+    version="1.0.5",
+    zip_safe=False,
+    project_urls={
+        "Documentation": "https://file-validator.github.io/",
+        "Homepage": "https://github.com/file-validator",
+        "Issue tracker": "https://github.com/file-validator/file-validator/issues",
+        "Release notes": "https://github.com/file-validator/file-validator/releases",
+        "Source": "https://github.com/file-validator/file-validator",
+        "Discussions": "https://github.com/orgs/file-validator/discussions",
+        "History Of Changes": "https://file-validator.github.io/docs/history/",
+    },
+)
```

