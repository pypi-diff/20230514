# Comparing `tmp/wagtail-resume-2.1.1.tar.gz` & `tmp/wagtail_resume-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-resume-2.1.1.tar", max compression
+gzip compressed data, was "wagtail_resume-2.2.0.tar", max compression
```

## Comparing `wagtail-resume-2.1.1.tar` & `wagtail_resume-2.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1069 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/LICENSE
--rw-r--r--   0        0        0     3496 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/README.md
--rw-r--r--   0        0        0     2126 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/__init__.py
--rw-r--r--   0        0        0      138 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/apps.py
--rw-r--r--   0        0        0     6128 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/blocks.py
--rw-r--r--   0        0        0     1085 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/locale/sv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3652 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/migrations/0001_initial.py
--rw-r--r--   0        0        0     2110 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/migrations/0002_auto_20191227_0916.py
--rw-r--r--   0        0        0     3930 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/migrations/0003_auto_20200110_1525.py
--rw-r--r--   0        0        0      467 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/migrations/0004_auto_20200110_1656.py
--rw-r--r--   0        0        0     4123 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/migrations/0005_auto_20200227_1224.py
--rw-r--r--   0        0        0      724 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py
--rw-r--r--   0        0        0      792 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py
--rw-r--r--   0        0        0     4757 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/migrations/0008_auto_20220211_1557.py
--rw-r--r--   0        0        0      953 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py
--rw-r--r--   0        0        0        0 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/migrations/__init__.py
--rw-r--r--   0        0        0     3733 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/models.py
--rw-r--r--   0        0        0        0 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/static/wagtail_resume/css/.gitkeep
--rw-r--r--   0        0        0     2573 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/static/wagtail_resume/css/resume_page.css
--rw-r--r--   0        0        0        0 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/static/wagtail_resume/images/.gitkeep
--rw-r--r--   0        0        0        0 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/static/wagtail_resume/js/.gitkeep
--rw-r--r--   0        0        0      392 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/blocks/contributions_block.html
--rw-r--r--   0        0        0     1366 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/blocks/education_block.html
--rw-r--r--   0        0        0      698 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html
--rw-r--r--   0        0        0      645 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html
--rw-r--r--   0        0        0      653 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/localization_dropdown.html
--rw-r--r--   0        0        0      107 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/resume_page.html
--rw-r--r--   0        0        0     2775 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/resume_page_body.html
--rw-r--r--   0        0        0      564 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/resume_page_head.html
--rw-r--r--   0        0        0        0 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/templatetags/__init__.py
--rw-r--r--   0        0        0      139 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/templatetags/wagtail_resume_extras.py
--rw-r--r--   0        0        0      142 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/urls.py
--rw-r--r--   0        0        0     2080 2022-10-09 16:57:25.685153 wagtail-resume-2.1.1/wagtail_resume/views.py
--rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 wagtail-resume-2.1.1/setup.py
--rw-r--r--   0        0        0     5125 1970-01-01 00:00:00.000000 wagtail-resume-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/LICENSE
+-rw-r--r--   0        0        0     3496 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/README.md
+-rw-r--r--   0        0        0     2092 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/wagtail_resume/__init__.py
+-rw-r--r--   0        0        0      138 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/wagtail_resume/apps.py
+-rw-r--r--   0        0        0     6123 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/wagtail_resume/blocks.py
+-rw-r--r--   0        0        0     1085 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3477 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/wagtail_resume/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1955 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/wagtail_resume/migrations/0002_auto_20191227_0916.py
+-rw-r--r--   0        0        0     3655 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/wagtail_resume/migrations/0003_auto_20200110_1525.py
+-rw-r--r--   0        0        0      467 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/wagtail_resume/migrations/0004_auto_20200110_1656.py
+-rw-r--r--   0        0        0     3843 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/wagtail_resume/migrations/0005_auto_20200227_1224.py
+-rw-r--r--   0        0        0      694 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py
+-rw-r--r--   0        0        0      792 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py
+-rw-r--r--   0        0        0     4472 2023-05-13 23:02:39.103381 wagtail_resume-2.2.0/wagtail_resume/migrations/0008_auto_20220211_1557.py
+-rw-r--r--   0        0        0      953 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py
+-rw-r--r--   0        0        0    18241 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py
+-rw-r--r--   0        0        0        0 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/migrations/__init__.py
+-rw-r--r--   0        0        0     3716 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/models.py
+-rw-r--r--   0        0        0        0 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/static/wagtail_resume/css/.gitkeep
+-rw-r--r--   0        0        0     2573 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/static/wagtail_resume/css/resume_page.css
+-rw-r--r--   0        0        0        0 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/static/wagtail_resume/images/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/static/wagtail_resume/js/.gitkeep
+-rw-r--r--   0        0        0      392 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/blocks/contributions_block.html
+-rw-r--r--   0        0        0     1366 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html
+-rw-r--r--   0        0        0      698 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html
+-rw-r--r--   0        0        0      645 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html
+-rw-r--r--   0        0        0      653 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html
+-rw-r--r--   0        0        0      107 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/resume_page.html
+-rw-r--r--   0        0        0     2775 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html
+-rw-r--r--   0        0        0      564 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html
+-rw-r--r--   0        0        0        0 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/templatetags/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/templatetags/wagtail_resume_extras.py
+-rw-r--r--   0        0        0      142 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/urls.py
+-rw-r--r--   0        0        0     2075 2023-05-13 23:02:39.107381 wagtail_resume-2.2.0/wagtail_resume/views.py
+-rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 wagtail_resume-2.2.0/PKG-INFO
```

### Comparing `wagtail-resume-2.1.1/LICENSE` & `wagtail_resume-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-resume-2.1.1/README.md` & `wagtail_resume-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-resume-2.1.1/pyproject.toml` & `wagtail_resume-2.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "wagtail-resume"
 authors = ["Adin Hodovic <hodovicadin@gmail.com>"]
 license = "MIT"
-version = "2.1.1"
+version = "2.2.0"
 readme = "README.md"
 homepage = "https://github.com/adinhodovic/wagtail-resume"
 repository = "https://github.com/adinhodovic/wagtail-resume"
 documentation = "https://github.com/adinhodovic/wagtail-resume"
 description = "A Wagtail project made to simplify creation of resumes for developers."
 keywords = [
   "Resume",
@@ -14,34 +14,33 @@
   "Wagtail",
   "CMS"
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
   "Framework :: Wagtail",
-  "Framework :: Wagtail :: 3",
   "Framework :: Wagtail :: 4",
+  "Framework :: Wagtail :: 5",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 Django = "^3.2.0 || ^4.0.0"
-wagtail = "^3.0.0 || ^4.0.0"
-wagtail-markdown = "^0.10"
+wagtail = "^4.0.0 || ^5.0.0"
+wagtail-markdown = "^0.10 || ^0.11"
 wagtail-metadata = "^3.0.0 || ^4.0.0"
 weasyprint = "^52"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 isort = "5.5.2"
 pylint = "2.12.0"
```

### Comparing `wagtail-resume-2.1.1/wagtail_resume/blocks.py` & `wagtail_resume-2.2.0/wagtail_resume/blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # pylint: disable=R0903,C0301
-from wagtail.core import blocks
+from wagtail import blocks
 from wagtailmarkdown.blocks import MarkdownBlock
 
 
 class WorkExperienceBlock(blocks.StructBlock):
     class Meta:
         template = "wagtail_resume/blocks/work_experience_block.html"
         icon = "doc-full-inverse"
```

### Comparing `wagtail-resume-2.1.1/wagtail_resume/locale/sv/LC_MESSAGES/django.po` & `wagtail_resume-2.2.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail-resume-2.1.1/wagtail_resume/migrations/0001_initial.py` & `wagtail_resume-2.2.0/wagtail_resume/migrations/0001_initial.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by Django 2.2.9 on 2019-12-26 11:29
 
 from django.db import migrations, models
 import django.db.models.deletion
-import wagtail.core.blocks
-import wagtail.core.fields
+import wagtail.blocks
+import wagtail.fields
 import wagtail.images.blocks
 import wagtailmarkdown.blocks
 import wagtailmarkdown.fields
 import wagtailmetadata.models
 
 
 class Migration(migrations.Migration):
@@ -25,16 +25,16 @@
             fields=[
                 ('page_ptr', models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, related_name='+', serialize=False, to='wagtailcore.Page')),
                 ('font', models.CharField(blank=True, max_length=100, null=True)),
                 ('background_color', models.CharField(blank=True, max_length=100, null=True)),
                 ('full_name', models.CharField(blank=True, max_length=100, null=True)),
                 ('role', models.CharField(blank=True, max_length=100, null=True)),
                 ('about', wagtailmarkdown.fields.MarkdownField(blank=True, max_length=1000, null=True)),
-                ('social_links', wagtail.core.fields.StreamField([('social_link', wagtail.core.blocks.StructBlock([('text', wagtail.core.blocks.TextBlock()), ('url', wagtail.core.blocks.URLBlock()), ('logo', wagtail.images.blocks.ImageChooserBlock())], icon='group'))], blank=True, null=True)),
-                ('resume', wagtail.core.fields.StreamField([('work_experience', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Work experience')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-tools')), ('experiences', wagtail.core.blocks.ListBlock(wagtail.core.blocks.StructBlock([('role', wagtail.core.blocks.CharBlock()), ('company', wagtail.core.blocks.CharBlock()), ('url', wagtail.core.blocks.URLBlock()), ('from_date', wagtail.core.blocks.DateBlock()), ('to_date', wagtail.core.blocks.DateBlock()), ('text', wagtailmarkdown.blocks.MarkdownBlock())], icon='folder-open-inverse')))])), ('contributions', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Contributions')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-code-branch')), ('contributions', wagtail.core.blocks.ListBlock(wagtail.core.blocks.StructBlock([('title', wagtail.core.blocks.CharBlock(required=False)), ('description', wagtail.core.blocks.TextBlock(required=False)), ('url', wagtail.core.blocks.URLBlock(required=False))], icon='folder-open-inverse')))])), ('writing', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Writing')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-pencil-alt')), ('posts', wagtail.core.blocks.StreamBlock([('internal_post', wagtail.core.blocks.StructBlock([('post', wagtail.core.blocks.PageChooserBlock())], icon='doc-full-inverse')), ('external_post', wagtail.core.blocks.StructBlock([('title', wagtail.core.blocks.CharBlock()), ('url', wagtail.core.blocks.URLBlock()), ('date', wagtail.core.blocks.DateBlock())], icon='doc-full-inverse'))], icon='folder-open-inverse'))]))], blank=True, null=True)),
+                ('social_links', wagtail.fields.StreamField([('social_link', wagtail.blocks.StructBlock([('text', wagtail.blocks.TextBlock()), ('url', wagtail.blocks.URLBlock()), ('logo', wagtail.images.blocks.ImageChooserBlock())], icon='group'))], blank=True, null=True)),
+                ('resume', wagtail.fields.StreamField([('work_experience', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Work experience')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-tools')), ('experiences', wagtail.blocks.ListBlock(wagtail.blocks.StructBlock([('role', wagtail.blocks.CharBlock()), ('company', wagtail.blocks.CharBlock()), ('url', wagtail.blocks.URLBlock()), ('from_date', wagtail.blocks.DateBlock()), ('to_date', wagtail.blocks.DateBlock()), ('text', wagtailmarkdown.blocks.MarkdownBlock())], icon='folder-open-inverse')))])), ('contributions', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Contributions')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-code-branch')), ('contributions', wagtail.blocks.ListBlock(wagtail.blocks.StructBlock([('title', wagtail.blocks.CharBlock(required=False)), ('description', wagtail.blocks.TextBlock(required=False)), ('url', wagtail.blocks.URLBlock(required=False))], icon='folder-open-inverse')))])), ('writing', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Writing')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-pencil-alt')), ('posts', wagtail.blocks.StreamBlock([('internal_post', wagtail.blocks.StructBlock([('post', wagtail.blocks.PageChooserBlock())], icon='doc-full-inverse')), ('external_post', wagtail.blocks.StructBlock([('title', wagtail.blocks.CharBlock()), ('url', wagtail.blocks.URLBlock()), ('date', wagtail.blocks.DateBlock())], icon='doc-full-inverse'))], icon='folder-open-inverse'))]))], blank=True, null=True)),
                 ('photo', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='+', to='wagtailimages.Image')),
             ],
             options={
                 'abstract': False,
             },
             bases=(wagtailmetadata.models.MetadataMixin, 'wagtailcore.page'),
         ),
```

### Comparing `wagtail-resume-2.1.1/wagtail_resume/migrations/0002_auto_20191227_0916.py` & `wagtail_resume-2.2.0/wagtail_resume/migrations/0002_auto_20191227_0916.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Generated by Django 2.2.9 on 2019-12-27 09:16
 
 from django.db import migrations
-import wagtail.core.blocks
-import wagtail.core.fields
+import wagtail.blocks
+import wagtail.fields
 import wagtailmarkdown.blocks
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('wagtail_resume', '0001_initial'),
     ]
 
     operations = [
         migrations.AlterField(
             model_name='baseresumepage',
             name='resume',
-            field=wagtail.core.fields.StreamField([('work_experience', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Work experience')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-tools')), ('experiences', wagtail.core.blocks.ListBlock(wagtail.core.blocks.StructBlock([('role', wagtail.core.blocks.CharBlock()), ('company', wagtail.core.blocks.CharBlock()), ('url', wagtail.core.blocks.URLBlock()), ('from_date', wagtail.core.blocks.DateBlock()), ('to_date', wagtail.core.blocks.DateBlock()), ('text', wagtailmarkdown.blocks.MarkdownBlock())], icon='folder-open-inverse')))])), ('contributions', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Contributions')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-code-branch')), ('contributions', wagtail.core.blocks.ListBlock(wagtail.core.blocks.StructBlock([('title', wagtail.core.blocks.CharBlock()), ('description', wagtail.core.blocks.TextBlock()), ('url', wagtail.core.blocks.URLBlock())], icon='folder-open-inverse')))])), ('writing', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Writing')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-pencil-alt')), ('posts', wagtail.core.blocks.StreamBlock([('internal_post', wagtail.core.blocks.StructBlock([('post', wagtail.core.blocks.PageChooserBlock())], icon='doc-full-inverse')), ('external_post', wagtail.core.blocks.StructBlock([('title', wagtail.core.blocks.CharBlock()), ('url', wagtail.core.blocks.URLBlock()), ('date', wagtail.core.blocks.DateBlock())], icon='doc-full-inverse'))], icon='folder-open-inverse'))]))], blank=True, null=True),
+            field=wagtail.fields.StreamField([('work_experience', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Work experience')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-tools')), ('experiences', wagtail.blocks.ListBlock(wagtail.blocks.StructBlock([('role', wagtail.blocks.CharBlock()), ('company', wagtail.blocks.CharBlock()), ('url', wagtail.blocks.URLBlock()), ('from_date', wagtail.blocks.DateBlock()), ('to_date', wagtail.blocks.DateBlock()), ('text', wagtailmarkdown.blocks.MarkdownBlock())], icon='folder-open-inverse')))])), ('contributions', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Contributions')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-code-branch')), ('contributions', wagtail.blocks.ListBlock(wagtail.blocks.StructBlock([('title', wagtail.blocks.CharBlock()), ('description', wagtail.blocks.TextBlock()), ('url', wagtail.blocks.URLBlock())], icon='folder-open-inverse')))])), ('writing', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Writing')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-pencil-alt')), ('posts', wagtail.blocks.StreamBlock([('internal_post', wagtail.blocks.StructBlock([('post', wagtail.blocks.PageChooserBlock())], icon='doc-full-inverse')), ('external_post', wagtail.blocks.StructBlock([('title', wagtail.blocks.CharBlock()), ('url', wagtail.blocks.URLBlock()), ('date', wagtail.blocks.DateBlock())], icon='doc-full-inverse'))], icon='folder-open-inverse'))]))], blank=True, null=True),
         ),
     ]
```

### Comparing `wagtail-resume-2.1.1/wagtail_resume/migrations/0003_auto_20200110_1525.py` & `wagtail_resume-2.2.0/wagtail_resume/migrations/0003_auto_20200110_1525.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Generated by Django 2.2.9 on 2020-01-10 15:25
 
 from django.db import migrations
-import wagtail.core.blocks
-import wagtail.core.fields
+import wagtail.blocks
+import wagtail.fields
 import wagtailmarkdown.blocks
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('wagtail_resume', '0002_auto_20191227_0916'),
     ]
 
     operations = [
         migrations.AlterField(
             model_name='baseresumepage',
             name='resume',
-            field=wagtail.core.fields.StreamField([('work_experience', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Work experience')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-tools')), ('experiences', wagtail.core.blocks.ListBlock(wagtail.core.blocks.StructBlock([('role', wagtail.core.blocks.CharBlock()), ('company', wagtail.core.blocks.CharBlock()), ('url', wagtail.core.blocks.URLBlock()), ('from_date', wagtail.core.blocks.DateBlock()), ('to_date', wagtail.core.blocks.DateBlock()), ('text', wagtailmarkdown.blocks.MarkdownBlock())], icon='folder-open-inverse')))])), ('contributions', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Contributions')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-code-branch')), ('contributions', wagtail.core.blocks.ListBlock(wagtail.core.blocks.StructBlock([('title', wagtail.core.blocks.CharBlock()), ('description', wagtail.core.blocks.TextBlock()), ('url', wagtail.core.blocks.URLBlock())], icon='folder-open-inverse')))])), ('writing', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Writing')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-pencil-alt')), ('posts', wagtail.core.blocks.StreamBlock([('internal_post', wagtail.core.blocks.StructBlock([('post', wagtail.core.blocks.PageChooserBlock())], icon='doc-full-inverse')), ('external_post', wagtail.core.blocks.StructBlock([('title', wagtail.core.blocks.CharBlock()), ('url', wagtail.core.blocks.URLBlock()), ('date', wagtail.core.blocks.DateBlock())], icon='doc-full-inverse'))], icon='folder-open-inverse'))])), ('education', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Education')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-graduation-cap')), ('educations', wagtail.core.blocks.StreamBlock([('degree', wagtail.core.blocks.StructBlock([('degree', wagtail.core.blocks.CharBlock(default="Bachelor's degree")), ('field_of_study', wagtail.core.blocks.CharBlock(default='Computer Software Engineering')), ('degree_url', wagtail.core.blocks.URLBlock()), ('university_name', wagtail.core.blocks.CharBlock()), ('university_url', wagtail.core.blocks.URLBlock()), ('studies_starting_date', wagtail.core.blocks.DateBlock(help_text='The year will only be displayed in the resume')), ('studies_ending_date', wagtail.core.blocks.DateBlock(help_text='The year will only be displayed in the resume'))], icon='doc-full-inverse')), ('certificate', wagtail.core.blocks.StructBlock([('name', wagtail.core.blocks.CharBlock()), ('certificate_url', wagtail.core.blocks.URLBlock()), ('studies_starting_date', wagtail.core.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('studies_ending_date', wagtail.core.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('institute_name', wagtail.core.blocks.CharBlock()), ('institute_url', wagtail.core.blocks.URLBlock())], icon='doc-full-inverse')), ('course', wagtail.core.blocks.StructBlock([('name', wagtail.core.blocks.CharBlock()), ('course_url', wagtail.core.blocks.URLBlock()), ('studies_starting_date', wagtail.core.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('studies_ending_date', wagtail.core.blocks.DateBlock(help_text='The year and month will only be displayed in the resume'))], icon='doc-full-inverse'))]))]))], blank=True, null=True),
+            field=wagtail.fields.StreamField([('work_experience', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Work experience')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-tools')), ('experiences', wagtail.blocks.ListBlock(wagtail.blocks.StructBlock([('role', wagtail.blocks.CharBlock()), ('company', wagtail.blocks.CharBlock()), ('url', wagtail.blocks.URLBlock()), ('from_date', wagtail.blocks.DateBlock()), ('to_date', wagtail.blocks.DateBlock()), ('text', wagtailmarkdown.blocks.MarkdownBlock())], icon='folder-open-inverse')))])), ('contributions', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Contributions')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-code-branch')), ('contributions', wagtail.blocks.ListBlock(wagtail.blocks.StructBlock([('title', wagtail.blocks.CharBlock()), ('description', wagtail.blocks.TextBlock()), ('url', wagtail.blocks.URLBlock())], icon='folder-open-inverse')))])), ('writing', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Writing')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-pencil-alt')), ('posts', wagtail.blocks.StreamBlock([('internal_post', wagtail.blocks.StructBlock([('post', wagtail.blocks.PageChooserBlock())], icon='doc-full-inverse')), ('external_post', wagtail.blocks.StructBlock([('title', wagtail.blocks.CharBlock()), ('url', wagtail.blocks.URLBlock()), ('date', wagtail.blocks.DateBlock())], icon='doc-full-inverse'))], icon='folder-open-inverse'))])), ('education', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Education')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-graduation-cap')), ('educations', wagtail.blocks.StreamBlock([('degree', wagtail.blocks.StructBlock([('degree', wagtail.blocks.CharBlock(default="Bachelor's degree")), ('field_of_study', wagtail.blocks.CharBlock(default='Computer Software Engineering')), ('degree_url', wagtail.blocks.URLBlock()), ('university_name', wagtail.blocks.CharBlock()), ('university_url', wagtail.blocks.URLBlock()), ('studies_starting_date', wagtail.blocks.DateBlock(help_text='The year will only be displayed in the resume')), ('studies_ending_date', wagtail.blocks.DateBlock(help_text='The year will only be displayed in the resume'))], icon='doc-full-inverse')), ('certificate', wagtail.blocks.StructBlock([('name', wagtail.blocks.CharBlock()), ('certificate_url', wagtail.blocks.URLBlock()), ('studies_starting_date', wagtail.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('studies_ending_date', wagtail.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('institute_name', wagtail.blocks.CharBlock()), ('institute_url', wagtail.blocks.URLBlock())], icon='doc-full-inverse')), ('course', wagtail.blocks.StructBlock([('name', wagtail.blocks.CharBlock()), ('course_url', wagtail.blocks.URLBlock()), ('studies_starting_date', wagtail.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('studies_ending_date', wagtail.blocks.DateBlock(help_text='The year and month will only be displayed in the resume'))], icon='doc-full-inverse'))]))]))], blank=True, null=True),
         ),
     ]
```

### Comparing `wagtail-resume-2.1.1/wagtail_resume/migrations/0005_auto_20200227_1224.py` & `wagtail_resume-2.2.0/wagtail_resume/migrations/0005_auto_20200227_1224.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Generated by Django 2.2.9 on 2020-02-27 12:24
 
 from django.db import migrations
-import wagtail.core.blocks
-import wagtail.core.fields
+import wagtail.blocks
+import wagtail.fields
 import wagtailmarkdown.blocks
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('wagtail_resume', '0004_auto_20200110_1656'),
     ]
 
     operations = [
         migrations.AlterField(
             model_name='baseresumepage',
             name='resume',
-            field=wagtail.core.fields.StreamField([('work_experience', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Work experience')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-tools')), ('experiences', wagtail.core.blocks.ListBlock(wagtail.core.blocks.StructBlock([('role', wagtail.core.blocks.CharBlock()), ('company', wagtail.core.blocks.CharBlock()), ('url', wagtail.core.blocks.URLBlock()), ('from_date', wagtail.core.blocks.DateBlock()), ('to_date', wagtail.core.blocks.DateBlock(required=False)), ('currently_working_here', wagtail.core.blocks.BooleanBlock(help_text='Check this box if you are currently working here and it will indicate so on the resume.', required=False)), ('text', wagtailmarkdown.blocks.MarkdownBlock())], icon='folder-open-inverse')))])), ('contributions', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Contributions')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-code-branch')), ('contributions', wagtail.core.blocks.ListBlock(wagtail.core.blocks.StructBlock([('title', wagtail.core.blocks.CharBlock()), ('description', wagtail.core.blocks.TextBlock()), ('url', wagtail.core.blocks.URLBlock())], icon='folder-open-inverse')))])), ('writing', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Writing')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-pencil-alt')), ('posts', wagtail.core.blocks.StreamBlock([('internal_post', wagtail.core.blocks.StructBlock([('post', wagtail.core.blocks.PageChooserBlock())], icon='doc-full-inverse')), ('external_post', wagtail.core.blocks.StructBlock([('title', wagtail.core.blocks.CharBlock()), ('url', wagtail.core.blocks.URLBlock()), ('date', wagtail.core.blocks.DateBlock())], icon='doc-full-inverse'))], icon='folder-open-inverse'))])), ('education', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Education')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-graduation-cap')), ('educations', wagtail.core.blocks.StreamBlock([('degree', wagtail.core.blocks.StructBlock([('degree', wagtail.core.blocks.CharBlock(default="Bachelor's degree")), ('field_of_study', wagtail.core.blocks.CharBlock(default='Computer Software Engineering')), ('degree_url', wagtail.core.blocks.URLBlock()), ('university_name', wagtail.core.blocks.CharBlock()), ('university_url', wagtail.core.blocks.URLBlock()), ('studies_starting_date', wagtail.core.blocks.DateBlock(help_text='The year will only be displayed in the resume')), ('studies_ending_date', wagtail.core.blocks.DateBlock(help_text='The year will only be displayed in the resume'))], icon='doc-full-inverse')), ('certificate', wagtail.core.blocks.StructBlock([('name', wagtail.core.blocks.CharBlock()), ('certificate_url', wagtail.core.blocks.URLBlock()), ('studies_starting_date', wagtail.core.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('studies_ending_date', wagtail.core.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('institute_name', wagtail.core.blocks.CharBlock()), ('institute_url', wagtail.core.blocks.URLBlock())], icon='doc-full-inverse')), ('course', wagtail.core.blocks.StructBlock([('name', wagtail.core.blocks.CharBlock()), ('course_url', wagtail.core.blocks.URLBlock()), ('studies_starting_date', wagtail.core.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('studies_ending_date', wagtail.core.blocks.DateBlock(help_text='The year and month will only be displayed in the resume'))], icon='doc-full-inverse'))]))]))], blank=True, null=True),
+            field=wagtail.fields.StreamField([('work_experience', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Work experience')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-tools')), ('experiences', wagtail.blocks.ListBlock(wagtail.blocks.StructBlock([('role', wagtail.blocks.CharBlock()), ('company', wagtail.blocks.CharBlock()), ('url', wagtail.blocks.URLBlock()), ('from_date', wagtail.blocks.DateBlock()), ('to_date', wagtail.blocks.DateBlock(required=False)), ('currently_working_here', wagtail.blocks.BooleanBlock(help_text='Check this box if you are currently working here and it will indicate so on the resume.', required=False)), ('text', wagtailmarkdown.blocks.MarkdownBlock())], icon='folder-open-inverse')))])), ('contributions', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Contributions')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-code-branch')), ('contributions', wagtail.blocks.ListBlock(wagtail.blocks.StructBlock([('title', wagtail.blocks.CharBlock()), ('description', wagtail.blocks.TextBlock()), ('url', wagtail.blocks.URLBlock())], icon='folder-open-inverse')))])), ('writing', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Writing')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-pencil-alt')), ('posts', wagtail.blocks.StreamBlock([('internal_post', wagtail.blocks.StructBlock([('post', wagtail.blocks.PageChooserBlock())], icon='doc-full-inverse')), ('external_post', wagtail.blocks.StructBlock([('title', wagtail.blocks.CharBlock()), ('url', wagtail.blocks.URLBlock()), ('date', wagtail.blocks.DateBlock())], icon='doc-full-inverse'))], icon='folder-open-inverse'))])), ('education', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Education')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-graduation-cap')), ('educations', wagtail.blocks.StreamBlock([('degree', wagtail.blocks.StructBlock([('degree', wagtail.blocks.CharBlock(default="Bachelor's degree")), ('field_of_study', wagtail.blocks.CharBlock(default='Computer Software Engineering')), ('degree_url', wagtail.blocks.URLBlock()), ('university_name', wagtail.blocks.CharBlock()), ('university_url', wagtail.blocks.URLBlock()), ('studies_starting_date', wagtail.blocks.DateBlock(help_text='The year will only be displayed in the resume')), ('studies_ending_date', wagtail.blocks.DateBlock(help_text='The year will only be displayed in the resume'))], icon='doc-full-inverse')), ('certificate', wagtail.blocks.StructBlock([('name', wagtail.blocks.CharBlock()), ('certificate_url', wagtail.blocks.URLBlock()), ('studies_starting_date', wagtail.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('studies_ending_date', wagtail.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('institute_name', wagtail.blocks.CharBlock()), ('institute_url', wagtail.blocks.URLBlock())], icon='doc-full-inverse')), ('course', wagtail.blocks.StructBlock([('name', wagtail.blocks.CharBlock()), ('course_url', wagtail.blocks.URLBlock()), ('studies_starting_date', wagtail.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('studies_ending_date', wagtail.blocks.DateBlock(help_text='The year and month will only be displayed in the resume'))], icon='doc-full-inverse'))]))]))], blank=True, null=True),
         ),
     ]
```

### Comparing `wagtail-resume-2.1.1/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py` & `wagtail_resume-2.2.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Generated by Django 3.2.6 on 2022-01-12 18:29
 
 from django.db import migrations
-import wagtail.core.blocks
-import wagtail.core.fields
+import wagtail.blocks
+import wagtail.fields
 import wagtail.images.blocks
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('wagtail_resume', '0005_auto_20200227_1224'),
     ]
 
     operations = [
         migrations.AlterField(
             model_name='baseresumepage',
             name='social_links',
-            field=wagtail.core.fields.StreamField([('social_link', wagtail.core.blocks.StructBlock([('text', wagtail.core.blocks.TextBlock()), ('url', wagtail.core.blocks.URLBlock()), ('logo', wagtail.images.blocks.ImageChooserBlock(required=False))], icon='group'))], blank=True, null=True),
+            field=wagtail.fields.StreamField([('social_link', wagtail.blocks.StructBlock([('text', wagtail.blocks.TextBlock()), ('url', wagtail.blocks.URLBlock()), ('logo', wagtail.images.blocks.ImageChooserBlock(required=False))], icon='group'))], blank=True, null=True),
         ),
     ]
```

### Comparing `wagtail-resume-2.1.1/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py` & `wagtail_resume-2.2.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py`

 * *Files identical despite different names*

### Comparing `wagtail-resume-2.1.1/wagtail_resume/migrations/0008_auto_20220211_1557.py` & `wagtail_resume-2.2.0/wagtail_resume/migrations/0008_auto_20220211_1557.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by Django 3.2.12 on 2022-02-11 15:57
 
 from django.db import migrations, models
-import wagtail.core.blocks
-import wagtail.core.fields
+import wagtail.blocks
+import wagtail.fields
 import wagtailmarkdown.blocks
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('wagtail_resume', '0007_baseresumepage_pdf_generation_visibility'),
@@ -17,10 +17,10 @@
             model_name='baseresumepage',
             name='pdf_generation_visibility',
             field=models.CharField(choices=[('always', 'Always visible'), ('authenticated', 'Only logged in users'), ('never', 'Never visible')], default='authenticated', help_text='\n            PDF generation is a heavy blocking operation,\n            so it is recommended to only show it to logged in users. If available to everyone, ensure that you have multiple workers running.\n        ', max_length=64),
         ),
         migrations.AlterField(
             model_name='baseresumepage',
             name='resume',
-            field=wagtail.core.fields.StreamField([('work_experience', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Work experience')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-tools')), ('experiences', wagtail.core.blocks.ListBlock(wagtail.core.blocks.StructBlock([('role', wagtail.core.blocks.CharBlock()), ('company', wagtail.core.blocks.CharBlock()), ('url', wagtail.core.blocks.URLBlock()), ('location', wagtail.core.blocks.CharBlock(required=False)), ('from_date', wagtail.core.blocks.DateBlock()), ('to_date', wagtail.core.blocks.DateBlock(required=False)), ('currently_working_here', wagtail.core.blocks.BooleanBlock(help_text='Check this box if you are currently working here and it will indicate so on the resume.', required=False)), ('text', wagtailmarkdown.blocks.MarkdownBlock())], icon='folder-open-inverse')))])), ('contributions', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Contributions')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-code-branch')), ('contributions', wagtail.core.blocks.ListBlock(wagtail.core.blocks.StructBlock([('title', wagtail.core.blocks.CharBlock()), ('description', wagtail.core.blocks.TextBlock()), ('url', wagtail.core.blocks.URLBlock())], icon='folder-open-inverse')))])), ('writing', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Writing')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-pencil-alt')), ('posts', wagtail.core.blocks.StreamBlock([('internal_post', wagtail.core.blocks.StructBlock([('post', wagtail.core.blocks.PageChooserBlock())], icon='doc-full-inverse')), ('external_post', wagtail.core.blocks.StructBlock([('title', wagtail.core.blocks.CharBlock()), ('url', wagtail.core.blocks.URLBlock()), ('date', wagtail.core.blocks.DateBlock())], icon='doc-full-inverse'))], icon='folder-open-inverse'))])), ('education', wagtail.core.blocks.StructBlock([('heading', wagtail.core.blocks.CharBlock(default='Education')), ('fa_icon', wagtail.core.blocks.CharBlock(default='fas fa-graduation-cap')), ('educations', wagtail.core.blocks.StreamBlock([('degree', wagtail.core.blocks.StructBlock([('degree', wagtail.core.blocks.CharBlock(default="Bachelor's degree")), ('field_of_study', wagtail.core.blocks.CharBlock(default='Computer Software Engineering')), ('degree_url', wagtail.core.blocks.URLBlock()), ('university_name', wagtail.core.blocks.CharBlock()), ('university_url', wagtail.core.blocks.URLBlock()), ('studies_starting_date', wagtail.core.blocks.DateBlock(help_text='The year will only be displayed in the resume')), ('studies_ending_date', wagtail.core.blocks.DateBlock(help_text='The year will only be displayed in the resume'))], icon='doc-full-inverse')), ('certificate', wagtail.core.blocks.StructBlock([('name', wagtail.core.blocks.CharBlock()), ('certificate_url', wagtail.core.blocks.URLBlock()), ('studies_starting_date', wagtail.core.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('studies_ending_date', wagtail.core.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('institute_name', wagtail.core.blocks.CharBlock()), ('institute_url', wagtail.core.blocks.URLBlock())], icon='doc-full-inverse')), ('course', wagtail.core.blocks.StructBlock([('name', wagtail.core.blocks.CharBlock()), ('course_url', wagtail.core.blocks.URLBlock()), ('studies_starting_date', wagtail.core.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('studies_ending_date', wagtail.core.blocks.DateBlock(help_text='The year and month will only be displayed in the resume'))], icon='doc-full-inverse'))]))]))], blank=True, null=True),
+            field=wagtail.fields.StreamField([('work_experience', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Work experience')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-tools')), ('experiences', wagtail.blocks.ListBlock(wagtail.blocks.StructBlock([('role', wagtail.blocks.CharBlock()), ('company', wagtail.blocks.CharBlock()), ('url', wagtail.blocks.URLBlock()), ('location', wagtail.blocks.CharBlock(required=False)), ('from_date', wagtail.blocks.DateBlock()), ('to_date', wagtail.blocks.DateBlock(required=False)), ('currently_working_here', wagtail.blocks.BooleanBlock(help_text='Check this box if you are currently working here and it will indicate so on the resume.', required=False)), ('text', wagtailmarkdown.blocks.MarkdownBlock())], icon='folder-open-inverse')))])), ('contributions', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Contributions')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-code-branch')), ('contributions', wagtail.blocks.ListBlock(wagtail.blocks.StructBlock([('title', wagtail.blocks.CharBlock()), ('description', wagtail.blocks.TextBlock()), ('url', wagtail.blocks.URLBlock())], icon='folder-open-inverse')))])), ('writing', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Writing')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-pencil-alt')), ('posts', wagtail.blocks.StreamBlock([('internal_post', wagtail.blocks.StructBlock([('post', wagtail.blocks.PageChooserBlock())], icon='doc-full-inverse')), ('external_post', wagtail.blocks.StructBlock([('title', wagtail.blocks.CharBlock()), ('url', wagtail.blocks.URLBlock()), ('date', wagtail.blocks.DateBlock())], icon='doc-full-inverse'))], icon='folder-open-inverse'))])), ('education', wagtail.blocks.StructBlock([('heading', wagtail.blocks.CharBlock(default='Education')), ('fa_icon', wagtail.blocks.CharBlock(default='fas fa-graduation-cap')), ('educations', wagtail.blocks.StreamBlock([('degree', wagtail.blocks.StructBlock([('degree', wagtail.blocks.CharBlock(default="Bachelor's degree")), ('field_of_study', wagtail.blocks.CharBlock(default='Computer Software Engineering')), ('degree_url', wagtail.blocks.URLBlock()), ('university_name', wagtail.blocks.CharBlock()), ('university_url', wagtail.blocks.URLBlock()), ('studies_starting_date', wagtail.blocks.DateBlock(help_text='The year will only be displayed in the resume')), ('studies_ending_date', wagtail.blocks.DateBlock(help_text='The year will only be displayed in the resume'))], icon='doc-full-inverse')), ('certificate', wagtail.blocks.StructBlock([('name', wagtail.blocks.CharBlock()), ('certificate_url', wagtail.blocks.URLBlock()), ('studies_starting_date', wagtail.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('studies_ending_date', wagtail.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('institute_name', wagtail.blocks.CharBlock()), ('institute_url', wagtail.blocks.URLBlock())], icon='doc-full-inverse')), ('course', wagtail.blocks.StructBlock([('name', wagtail.blocks.CharBlock()), ('course_url', wagtail.blocks.URLBlock()), ('studies_starting_date', wagtail.blocks.DateBlock(help_text='The year and month will only be displayed in the resume')), ('studies_ending_date', wagtail.blocks.DateBlock(help_text='The year and month will only be displayed in the resume'))], icon='doc-full-inverse'))]))]))], blank=True, null=True),
         ),
     ]
```

### Comparing `wagtail-resume-2.1.1/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py` & `wagtail_resume-2.2.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py`

 * *Files identical despite different names*

### Comparing `wagtail-resume-2.1.1/wagtail_resume/models.py` & `wagtail_resume-2.2.0/wagtail_resume/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.db import models
 from django.utils.text import Truncator
-from wagtail.admin.edit_handlers import FieldPanel, MultiFieldPanel
-from wagtail.core import blocks, fields
-from wagtail.core.models import Page
+from wagtail import blocks, fields
+from wagtail.admin.panels import FieldPanel, MultiFieldPanel
 from wagtail.images.blocks import ImageChooserBlock
 from wagtail.images.models import Image
+from wagtail.models import Page
 from wagtailmarkdown.edit_handlers import MarkdownPanel
 from wagtailmarkdown.fields import MarkdownField
 from wagtailmetadata.models import MetadataMixin
 
 from .blocks import (
     ContributionsBlock,
     EducationBlock,
```

### Comparing `wagtail-resume-2.1.1/wagtail_resume/static/wagtail_resume/css/resume_page.css` & `wagtail_resume-2.2.0/wagtail_resume/static/wagtail_resume/css/resume_page.css`

 * *Files identical despite different names*

### Comparing `wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/blocks/education_block.html` & `wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html` & `wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html` & `wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/localization_dropdown.html` & `wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html`

 * *Files identical despite different names*

### Comparing `wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/resume_page_body.html` & `wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html`

 * *Files identical despite different names*

### Comparing `wagtail-resume-2.1.1/wagtail_resume/templates/wagtail_resume/resume_page_head.html` & `wagtail_resume-2.2.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html`

 * *Files identical despite different names*

### Comparing `wagtail-resume-2.1.1/wagtail_resume/views.py` & `wagtail_resume-2.2.0/wagtail_resume/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.http import (
     HttpResponse,
     HttpResponseBadRequest,
     HttpResponseForbidden,
     HttpResponseNotFound,
 )
 from django.utils.text import slugify
-from wagtail.core.models import Page
+from wagtail.models import Page
 from weasyprint import HTML
 
 from wagtail_resume.templatetags.wagtail_resume_extras import space_to_plus
 
 logger = logging.getLogger("weasyprint")
 logger.addHandler(logging.NullHandler())
 logger.setLevel(40)  # Only show errors, use 50
```

### Comparing `wagtail-resume-2.1.1/PKG-INFO` & `wagtail_resume-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: wagtail-resume
-Version: 2.1.1
+Version: 2.2.0
 Summary: A Wagtail project made to simplify creation of resumes for developers.
 Home-page: https://github.com/adinhodovic/wagtail-resume
 License: MIT
 Keywords: Resume,Django,Wagtail,CMS
 Author: Adin Hodovic
 Author-email: hodovicadin@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Django (>=3.2.0,<5.0.0)
-Requires-Dist: wagtail (>=3.0.0,<5.0.0)
-Requires-Dist: wagtail-markdown (>=0.10,<0.11)
+Requires-Dist: wagtail (>=4.0.0,<6.0.0)
+Requires-Dist: wagtail-markdown (>=0.10,<0.12)
 Requires-Dist: wagtail-metadata (>=3.0.0,<5.0.0)
 Requires-Dist: weasyprint (>=52,<53)
 Project-URL: Documentation, https://github.com/adinhodovic/wagtail-resume
 Project-URL: Repository, https://github.com/adinhodovic/wagtail-resume
 Description-Content-Type: text/markdown
 
 # Wagtail resume
```

