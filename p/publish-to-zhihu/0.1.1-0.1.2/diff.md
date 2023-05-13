# Comparing `tmp/publish_to_zhihu-0.1.1.tar.gz` & `tmp/publish_to_zhihu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "publish_to_zhihu-0.1.1.tar", max compression
+gzip compressed data, was "publish_to_zhihu-0.1.2.tar", max compression
```

## Comparing `publish_to_zhihu-0.1.1.tar` & `publish_to_zhihu-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1090 2023-05-11 23:45:42.640554 publish_to_zhihu-0.1.1/LICENSE
--rw-r--r--   0        0        0       23 2023-05-11 23:45:42.645559 publish_to_zhihu-0.1.1/publish_to_zhihu/__init__.py
--rw-r--r--   0        0        0      338 2023-05-11 23:45:42.646554 publish_to_zhihu-0.1.1/publish_to_zhihu/console.py
--rw-r--r--   0        0        0     1177 2023-05-11 23:45:42.646554 publish_to_zhihu-0.1.1/publish_to_zhihu/convert_latex.py
--rw-r--r--   0        0        0     3623 2023-05-13 18:13:22.429142 publish_to_zhihu-0.1.1/publish_to_zhihu/prepare_md.py
--rw-r--r--   0        0        0     2725 2023-05-11 23:45:42.647555 publish_to_zhihu-0.1.1/publish_to_zhihu/upload_images.py
--rw-r--r--   0        0        0      932 2023-05-13 18:18:27.674336 publish_to_zhihu-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1224 2023-05-11 23:45:42.641554 publish_to_zhihu-0.1.1/README.md
--rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 publish_to_zhihu-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-05-11 23:45:42.640554 publish_to_zhihu-0.1.2/LICENSE
+-rw-r--r--   0        0        0       23 2023-05-11 23:45:42.645559 publish_to_zhihu-0.1.2/publish_to_zhihu/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-11 23:45:42.646554 publish_to_zhihu-0.1.2/publish_to_zhihu/console.py
+-rw-r--r--   0        0        0     1177 2023-05-11 23:45:42.646554 publish_to_zhihu-0.1.2/publish_to_zhihu/convert_latex.py
+-rw-r--r--   0        0        0     3632 2023-05-13 22:08:57.679141 publish_to_zhihu-0.1.2/publish_to_zhihu/prepare_md.py
+-rw-r--r--   0        0        0     2725 2023-05-11 23:45:42.647555 publish_to_zhihu-0.1.2/publish_to_zhihu/upload_images.py
+-rw-r--r--   0        0        0      932 2023-05-13 22:09:51.798818 publish_to_zhihu-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4329 2023-05-13 22:06:47.223028 publish_to_zhihu-0.1.2/README.md
+-rw-r--r--   0        0        0     4953 1970-01-01 00:00:00.000000 publish_to_zhihu-0.1.2/PKG-INFO
```

### Comparing `publish_to_zhihu-0.1.1/LICENSE` & `publish_to_zhihu-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `publish_to_zhihu-0.1.1/publish_to_zhihu/convert_latex.py` & `publish_to_zhihu-0.1.2/publish_to_zhihu/convert_latex.py`

 * *Files identical despite different names*

### Comparing `publish_to_zhihu-0.1.1/publish_to_zhihu/prepare_md.py` & `publish_to_zhihu-0.1.2/publish_to_zhihu/prepare_md.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 import argparse
 import os
 import re
 
 from .upload_images import upload_images
 
-# IMAGE_LINK_RE = re.compile(
-#     r"!\[[^\]]*\]\((?P<filename>.*?)(?=\"|\))(?P<optionalpart>\".*\")?\)"
-# )
-
-
 OBSIDIAN_IMAGE_LINK_RE = re.compile(r"!\[\[([^\]]*)\]\]")
 
 
 def append_newline_to_list_items(markdown_string):
     # Regular expression pattern to match unordered and ordered list items
     pattern = r"(^[-*+]\s|\d+\.\s)"
 
@@ -28,24 +23,23 @@
 
     # Join the modified lines back into a single string
     modified_string = "\n".join(lines)
     return modified_string
 
 
 def ensure_image_link_newline(markdown_string):
-    # Regular expression pattern to match image links
-    pattern = r"!\[.*?\]\(.*?\)"
-
     # Find all image links in the markdown string
-    image_links = re.findall(pattern, markdown_string)
+    image_links = re.findall(OBSIDIAN_IMAGE_LINK_RE, markdown_string)
 
     # Iterate over each image link and ensure it appears at the beginning of a newline
     for image_link in image_links:
         # Replace the image link with a newline + image link
-        markdown_string = markdown_string.replace(image_link, "\n" + image_link)
+        markdown_string = markdown_string.replace(
+            f"![[{image_link}]]", "\n" + f"![[{image_link}]]"
+        )
 
     return markdown_string
 
 
 def process_image_link(container, conn_str, image_folder, re_match):
     image_link = re_match.group(1)
     if not image_link.startswith("http://") and not image_link.startswith("https://"):
@@ -55,14 +49,17 @@
             image_folder,
             [image_link],
             overwrite=True,
         )
         image_link = uploaded_urls[0]
     return f"![]({image_link})"
 
+    # not needed for mdnice
+    # return f'<img src="{image_link}" class="origin_image zh-lightbox-thumb lazy">\n'
+
 
 def main():
     parser = argparse.ArgumentParser(
         description="""
     Convert standard Markdown file to mdnice Format
     1. Upload all the images
 
@@ -92,18 +89,19 @@
 
     for file_path in files:
         output_file_path = os.path.join(output_folder, os.path.split(file_path)[1])
         with open(file_path, encoding="utf-8") as in_f, open(
             output_file_path, "w", encoding="utf-8"
         ) as out_f:
             content = in_f.read()
+            new_content = ensure_image_link_newline(content)
             new_content = OBSIDIAN_IMAGE_LINK_RE.sub(
                 lambda m: process_image_link(container, conn_str, image_link_root, m),
-                content,
+                new_content,
             )
-            new_content = append_newline_to_list_items(new_content)
-            new_content = ensure_image_link_newline(new_content)
+            # not needed for mdnice
+            # new_content = append_newline_to_list_items(new_content)
             out_f.write(new_content)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `publish_to_zhihu-0.1.1/publish_to_zhihu/upload_images.py` & `publish_to_zhihu-0.1.2/publish_to_zhihu/upload_images.py`

 * *Files identical despite different names*

### Comparing `publish_to_zhihu-0.1.1/pyproject.toml` & `publish_to_zhihu-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "publish_to_zhihu"
-version = "0.1.1"
+version = "0.1.2"
 description = "Publish markdown to Zhihu"
 authors = ["Anselm Wang <anselmwang@gmail.com>"]
 homepage = "https://github.com/anselmwang/publish_to_zhihu"
 repository = "https://github.com/anselmwang/publish_to_zhihu"
 readme= "README.md"
 
 [tool.poetry.dependencies]
```

