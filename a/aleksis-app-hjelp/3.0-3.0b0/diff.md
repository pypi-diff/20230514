# Comparing `tmp/aleksis_app_hjelp-3.0.tar.gz` & `tmp/aleksis_app_hjelp-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_hjelp-3.0.tar", max compression
+gzip compressed data, was "aleksis_app_hjelp-3.0b0.tar", max compression
```

## Comparing `aleksis_app_hjelp-3.0.tar` & `aleksis_app_hjelp-3.0b0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     3375 2023-05-14 18:24:28.487195 aleksis_app_hjelp-3.0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-05-14 18:24:28.487195 aleksis_app_hjelp-3.0/LICENCE.rst
--rw-r--r--   0        0        0     1430 2023-05-14 18:24:28.487195 aleksis_app_hjelp-3.0/README.rst
--rw-r--r--   0        0        0      151 2023-05-14 18:24:28.487195 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/__init__.py
--rw-r--r--   0        0        0      441 2023-05-14 18:37:39.312755 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      788 2023-05-14 18:37:42.280896 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0     1172 2023-05-14 18:37:40.780825 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     7962 2023-05-14 18:37:42.200893 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0     2522 2023-05-14 18:37:42.432903 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0     1636 2023-05-14 18:37:42.312898 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0      289 2023-05-14 18:24:28.487195 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/admin.py
--rw-r--r--   0        0        0      727 2023-05-14 18:24:28.487195 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/apps.py
--rw-r--r--   0        0        0     3678 2023-05-14 18:24:28.487195 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/forms.py
--rw-r--r--   0        0        0     3740 2023-05-14 18:24:28.487195 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/frontend/index.js
--rw-r--r--   0        0        0      276 2023-05-14 18:24:28.491195 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/frontend/messages/de.json
--rw-r--r--   0        0        0      263 2023-05-14 18:24:28.491195 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/frontend/messages/en.json
--rw-r--r--   0        0        0      323 2023-05-14 18:24:28.491195 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/frontend/messages/ru.json
--rw-r--r--   0        0        0      351 2023-05-14 18:24:28.491195 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/frontend/messages/uk.json
--rw-r--r--   0        0        0      463 2023-05-14 18:37:42.860924 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    12551 2023-05-14 18:24:28.491195 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10750 2023-05-14 18:37:42.812922 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18875 2023-05-14 18:24:28.495195 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      468 2023-05-14 18:37:42.816922 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    12784 2023-05-14 18:24:28.503196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      511 2023-05-14 18:37:42.740918 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    12564 2023-05-14 18:24:28.507196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-14 18:37:42.808921 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    12421 2023-05-14 18:24:28.507196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    12968 2023-05-14 18:37:42.772920 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19312 2023-05-14 18:24:28.507196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-14 18:37:42.752919 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    12421 2023-05-14 18:24:28.507196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    13162 2023-05-14 18:37:42.824922 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19508 2023-05-14 18:24:28.511196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0   180881 2023-05-14 18:24:28.511196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/migrations/0001_initial.py
--rw-r--r--   0        0        0      694 2023-05-14 18:24:28.511196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/migrations/0002_change_max_length.py
--rw-r--r--   0        0        0      593 2023-05-14 18:24:28.511196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/migrations/0003_faqsection_position_and_show.py
--rw-r--r--   0        0        0     2160 2023-05-14 18:24:28.511196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/migrations/0004_unique_constraints.py
--rw-r--r--   0        0        0   862506 2023-05-14 18:24:28.519196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/migrations/0005_update_icon_choices.py
--rw-r--r--   0        0        0        0 2023-05-14 18:24:28.519196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/migrations/__init__.py
--rw-r--r--   0        0        0     4267 2023-05-14 18:24:28.519196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/models.py
--rw-r--r--   0        0        0     1423 2023-05-14 18:24:28.519196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/preferences.py
--rw-r--r--   0        0        0     1306 2023-05-14 18:24:28.519196 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/rules.py
--rw-r--r--   0        0        0     1991 2023-05-14 18:24:28.547198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/static/css/hjelp/hjelp.css
--rw-r--r--   0        0        0      850 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/static/js/hjelp/order_faq.js
--rw-r--r--   0        0        0      754 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/ask.html
--rw-r--r--   0        0        0     2179 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/faq.html
--rw-r--r--   0        0        0     5034 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/feedback.html
--rw-r--r--   0        0        0      752 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/feedback_submitted.html
--rw-r--r--   0        0        0      422 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/hjelp_crud_views.html
--rw-r--r--   0        0        0     6740 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/issue_report.html
--rw-r--r--   0        0        0      839 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/issue_report_submitted.html
--rw-r--r--   0        0        0     4906 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/order_faq.html
--rw-r--r--   0        0        0      971 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/question_submitted.html
--rw-r--r--   0        0        0      968 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/templated_email/faq.email
--rw-r--r--   0        0        0     3777 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/templated_email/feedback.email
--rw-r--r--   0        0        0     1099 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/templated_email/html_mail.css
--rw-r--r--   0        0        0     1312 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/templated_email/rebus.email
--rw-r--r--   0        0        0     1019 2023-05-14 18:24:28.551198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/urls.py
--rw-r--r--   0        0        0    11647 2023-05-14 18:24:28.555198 aleksis_app_hjelp-3.0/aleksis/apps/hjelp/views.py
--rw-r--r--   0        0        0      581 2023-05-14 18:24:28.555198 aleksis_app_hjelp-3.0/docs/Makefile
--rw-r--r--   0        0        0    65324 2023-05-14 18:24:28.555198 aleksis_app_hjelp-3.0/docs/_static/ask_a_question.png
--rw-r--r--   0        0        0    87871 2023-05-14 18:24:28.555198 aleksis_app_hjelp-3.0/docs/_static/faq.png
--rw-r--r--   0        0        0    70659 2023-05-14 18:24:28.559198 aleksis_app_hjelp-3.0/docs/_static/faq_question.png
--rw-r--r--   0        0        0    61621 2023-05-14 18:24:28.559198 aleksis_app_hjelp-3.0/docs/_static/faq_section.png
--rw-r--r--   0        0        0    83597 2023-05-14 18:24:28.559198 aleksis_app_hjelp-3.0/docs/_static/feedback.png
--rw-r--r--   0        0        0    82288 2023-05-14 18:24:28.559198 aleksis_app_hjelp-3.0/docs/_static/issue_categories.png
--rw-r--r--   0        0        0    79521 2023-05-14 18:24:28.563199 aleksis_app_hjelp-3.0/docs/_static/issue_category.png
--rw-r--r--   0        0        0    75643 2023-05-14 18:24:28.563199 aleksis_app_hjelp-3.0/docs/_static/manage_faq.png
--rw-r--r--   0        0        0    72918 2023-05-14 18:24:28.563199 aleksis_app_hjelp-3.0/docs/_static/report_issue.png
--rw-r--r--   0        0        0      122 2023-05-14 18:24:28.571199 aleksis_app_hjelp-3.0/docs/admin/00_index.rst
--rw-r--r--   0        0        0     1084 2023-05-14 18:24:28.571199 aleksis_app_hjelp-3.0/docs/admin/10_managing_faqs.rst
--rw-r--r--   0        0        0     1643 2023-05-14 18:24:28.571199 aleksis_app_hjelp-3.0/docs/admin/15_managing_issue_report_form.rst
--rw-r--r--   0        0        0      570 2023-05-14 18:24:28.571199 aleksis_app_hjelp-3.0/docs/admin/40_preferences.rst
--rw-r--r--   0        0        0     6396 2023-05-14 18:24:28.571199 aleksis_app_hjelp-3.0/docs/conf.py
--rw-r--r--   0        0        0      526 2023-05-14 18:24:28.571199 aleksis_app_hjelp-3.0/docs/index.rst
--rw-r--r--   0        0        0      787 2023-05-14 18:24:28.571199 aleksis_app_hjelp-3.0/docs/make.bat
--rw-r--r--   0        0        0       74 2023-05-14 18:24:28.571199 aleksis_app_hjelp-3.0/docs/user/00_index.rst
--rw-r--r--   0        0        0      652 2023-05-14 18:24:28.571199 aleksis_app_hjelp-3.0/docs/user/01_faq.rst
--rw-r--r--   0        0        0      689 2023-05-14 18:24:28.571199 aleksis_app_hjelp-3.0/docs/user/10_issue_reporting.rst
--rw-r--r--   0        0        0      783 2023-05-14 18:24:28.571199 aleksis_app_hjelp-3.0/docs/user/20_feedback.rst
--rw-r--r--   0        0        0     1799 2023-05-14 18:25:52.387183 aleksis_app_hjelp-3.0/pyproject.toml
--rw-r--r--   0        0        0     2730 2023-05-14 18:24:28.571199 aleksis_app_hjelp-3.0/tox.ini
--rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 aleksis_app_hjelp-3.0/setup.py
--rw-r--r--   0        0        0     2562 1970-01-01 00:00:00.000000 aleksis_app_hjelp-3.0/PKG-INFO
+-rw-r--r--   0        0        0     3207 2023-02-23 17:32:07.597629 aleksis_app_hjelp-3.0b0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-02-23 17:32:07.597629 aleksis_app_hjelp-3.0b0/LICENCE.rst
+-rw-r--r--   0        0        0     1430 2023-02-23 17:32:07.597629 aleksis_app_hjelp-3.0b0/README.rst
+-rw-r--r--   0        0        0      151 2023-02-23 17:32:07.597629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/__init__.py
+-rw-r--r--   0        0        0      441 2023-02-23 17:34:13.045408 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      788 2023-02-23 17:34:14.053407 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0     1172 2023-02-23 17:34:13.425408 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     7962 2023-02-23 17:34:14.021407 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     2522 2023-02-23 17:34:14.121406 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0     1636 2023-02-23 17:34:14.069407 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0      289 2023-02-23 17:32:07.597629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/admin.py
+-rw-r--r--   0        0        0      727 2023-02-23 17:32:07.597629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/apps.py
+-rw-r--r--   0        0        0     3678 2023-02-23 17:32:07.597629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/forms.py
+-rw-r--r--   0        0        0     3740 2023-02-23 17:32:07.597629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/frontend/index.js
+-rw-r--r--   0        0        0      276 2023-02-23 17:32:07.597629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/frontend/messages/de.json
+-rw-r--r--   0        0        0      263 2023-02-23 17:32:07.601629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/frontend/messages/en.json
+-rw-r--r--   0        0        0      323 2023-02-23 17:32:07.601629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/frontend/messages/ru.json
+-rw-r--r--   0        0        0      351 2023-02-23 17:32:07.601629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/frontend/messages/uk.json
+-rw-r--r--   0        0        0      463 2023-02-23 17:34:14.153406 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12551 2023-02-23 17:32:07.601629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10750 2023-02-23 17:34:14.153406 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18875 2023-02-23 17:32:07.601629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      468 2023-02-23 17:34:14.165406 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12784 2023-02-23 17:32:07.601629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      511 2023-02-23 17:34:14.161406 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12564 2023-02-23 17:32:07.601629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-23 17:34:14.153406 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12421 2023-02-23 17:32:07.601629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    12968 2023-02-23 17:34:14.157406 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19312 2023-02-23 17:32:07.601629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-23 17:34:14.153406 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12421 2023-02-23 17:32:07.601629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    13162 2023-02-23 17:34:14.157406 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19508 2023-02-23 17:32:07.605629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0   180881 2023-02-23 17:32:07.605629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      694 2023-02-23 17:32:07.605629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/migrations/0002_change_max_length.py
+-rw-r--r--   0        0        0      593 2023-02-23 17:32:07.605629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/migrations/0003_faqsection_position_and_show.py
+-rw-r--r--   0        0        0     2160 2023-02-23 17:32:07.605629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/migrations/0004_unique_constraints.py
+-rw-r--r--   0        0        0   862506 2023-02-23 17:32:07.609629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/migrations/0005_update_icon_choices.py
+-rw-r--r--   0        0        0        0 2023-02-23 17:32:07.609629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/migrations/__init__.py
+-rw-r--r--   0        0        0     4267 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/models.py
+-rw-r--r--   0        0        0     1423 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/preferences.py
+-rw-r--r--   0        0        0     1306 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/rules.py
+-rw-r--r--   0        0        0     1991 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/static/css/hjelp/hjelp.css
+-rw-r--r--   0        0        0      850 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/static/js/hjelp/order_faq.js
+-rw-r--r--   0        0        0      754 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/ask.html
+-rw-r--r--   0        0        0     2160 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/faq.html
+-rw-r--r--   0        0        0     5034 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/feedback.html
+-rw-r--r--   0        0        0      752 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/feedback_submitted.html
+-rw-r--r--   0        0        0      422 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/hjelp_crud_views.html
+-rw-r--r--   0        0        0     6740 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/issue_report.html
+-rw-r--r--   0        0        0      839 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/issue_report_submitted.html
+-rw-r--r--   0        0        0     4906 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/order_faq.html
+-rw-r--r--   0        0        0      971 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/question_submitted.html
+-rw-r--r--   0        0        0      968 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/templated_email/faq.email
+-rw-r--r--   0        0        0     3777 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/templated_email/feedback.email
+-rw-r--r--   0        0        0     1099 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/templated_email/html_mail.css
+-rw-r--r--   0        0        0     1312 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/templated_email/rebus.email
+-rw-r--r--   0        0        0     1019 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/urls.py
+-rw-r--r--   0        0        0    11647 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/views.py
+-rw-r--r--   0        0        0      581 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/docs/Makefile
+-rw-r--r--   0        0        0    65324 2023-02-23 17:32:07.613629 aleksis_app_hjelp-3.0b0/docs/_static/ask_a_question.png
+-rw-r--r--   0        0        0    87871 2023-02-23 17:32:07.617629 aleksis_app_hjelp-3.0b0/docs/_static/faq.png
+-rw-r--r--   0        0        0    70659 2023-02-23 17:32:07.617629 aleksis_app_hjelp-3.0b0/docs/_static/faq_question.png
+-rw-r--r--   0        0        0    61621 2023-02-23 17:32:07.617629 aleksis_app_hjelp-3.0b0/docs/_static/faq_section.png
+-rw-r--r--   0        0        0    83597 2023-02-23 17:32:07.617629 aleksis_app_hjelp-3.0b0/docs/_static/feedback.png
+-rw-r--r--   0        0        0    82288 2023-02-23 17:32:07.617629 aleksis_app_hjelp-3.0b0/docs/_static/issue_categories.png
+-rw-r--r--   0        0        0    79521 2023-02-23 17:32:07.617629 aleksis_app_hjelp-3.0b0/docs/_static/issue_category.png
+-rw-r--r--   0        0        0    75643 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/docs/_static/manage_faq.png
+-rw-r--r--   0        0        0    72918 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/docs/_static/report_issue.png
+-rw-r--r--   0        0        0      122 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     1084 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/docs/admin/10_managing_faqs.rst
+-rw-r--r--   0        0        0     1643 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/docs/admin/15_managing_issue_report_form.rst
+-rw-r--r--   0        0        0      570 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/docs/admin/40_preferences.rst
+-rw-r--r--   0        0        0     6398 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/docs/conf.py
+-rw-r--r--   0        0        0      526 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/docs/make.bat
+-rw-r--r--   0        0        0       74 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/docs/user/00_index.rst
+-rw-r--r--   0        0        0      652 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/docs/user/01_faq.rst
+-rw-r--r--   0        0        0      689 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/docs/user/10_issue_reporting.rst
+-rw-r--r--   0        0        0      783 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/docs/user/20_feedback.rst
+-rw-r--r--   0        0        0     1803 2023-02-23 17:32:32.457585 aleksis_app_hjelp-3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-02-23 17:32:07.621629 aleksis_app_hjelp-3.0b0/tox.ini
+-rw-r--r--   0        0        0     3088 1970-01-01 00:00:00.000000 aleksis_app_hjelp-3.0b0/setup.py
+-rw-r--r--   0        0        0     2566 1970-01-01 00:00:00.000000 aleksis_app_hjelp-3.0b0/PKG-INFO
```

### Comparing `aleksis_app_hjelp-3.0/CHANGELOG.rst` & `aleksis_app_hjelp-3.0b0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,16 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`3.0`_ - 2023-05-14
--------------------
-
-Fixed
-~~~~~
-
-* Icons in the FAQ were not rendered
-
-`3.0b0`_ - 2023-02-22
----------------------
+`3.0b0` - 2023-02-22
+--------------------
 
 This version requires AlekSIS-Core 3.0. It is incompatible with any previous
 version.
 
 Removed
 ~~~~~~~
 
@@ -148,8 +140,7 @@
 .. _2.0rc2: https://edugit.org/AlekSIS/Official/AlekSIS-App-Hjelp/-/tags/2.0rc2
 .. _2.0rc3: https://edugit.org/AlekSIS/Official/AlekSIS-App-Hjelp/-/tags/2.0rc3
 .. _2.0: https://edugit.org/AlekSIS/Official/AlekSIS-App-Hjelp/-/tags/2.0
 .. _2.0.1: https://edugit.org/AlekSIS/Official/AlekSIS-App-Hjelp/-/tags/2.0.1
 .. _2.0.2: https://edugit.org/AlekSIS/Official/AlekSIS-App-Hjelp/-/tags/2.0.2
 .. _2.1: https://edugit.org/AlekSIS/Official/AlekSIS-App-Hjelp/-/tags/2.1
 .. _3.0b0: https://edugit.org/AlekSIS/Official/AlekSIS-App-Hjelp/-/tags/3.0b0
-.. _3.0: https://edugit.org/AlekSIS/Official/AlekSIS-App-Hjelp/-/tags/3.0
```

### Comparing `aleksis_app_hjelp-3.0/LICENCE.rst` & `aleksis_app_hjelp-3.0b0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/README.rst` & `aleksis_app_hjelp-3.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/__pycache__/admin.cpython-311.pyc` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/__pycache__/admin.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5c276164 (Sun May 14 18:24:28 2023 UTC)
+moddate:  0x17a3f763 (Thu Feb 23 17:32:07 2023 UTC)
 files sz: 289
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/__pycache__/apps.cpython-311.pyc` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/__pycache__/apps.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5c276164 (Sun May 14 18:24:28 2023 UTC)
+moddate:  0x17a3f763 (Thu Feb 23 17:32:07 2023 UTC)
 files sz: 727
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/__pycache__/models.cpython-311.pyc` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/__pycache__/models.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5c276164 (Sun May 14 18:24:28 2023 UTC)
+moddate:  0x17a3f763 (Thu Feb 23 17:32:07 2023 UTC)
 files sz: 4267
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/__pycache__/preferences.cpython-311.pyc` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/__pycache__/preferences.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5c276164 (Sun May 14 18:24:28 2023 UTC)
+moddate:  0x17a3f763 (Thu Feb 23 17:32:07 2023 UTC)
 files sz: 1423
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/__pycache__/rules.cpython-311.pyc` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/__pycache__/rules.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5c276164 (Sun May 14 18:24:28 2023 UTC)
+moddate:  0x17a3f763 (Thu Feb 23 17:32:07 2023 UTC)
 files sz: 1306
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/apps.py` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/forms.py` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/frontend/index.js` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/la/LC_MESSAGES/django.po` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/migrations/0001_initial.py` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/migrations/0002_change_max_length.py` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/migrations/0002_change_max_length.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/migrations/0003_faqsection_position_and_show.py` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/migrations/0003_faqsection_position_and_show.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/migrations/0004_unique_constraints.py` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/migrations/0004_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/migrations/0005_update_icon_choices.py` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/migrations/0005_update_icon_choices.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/models.py` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/preferences.py` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/rules.py` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/static/css/hjelp/hjelp.css` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/static/css/hjelp/hjelp.css`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/static/js/hjelp/order_faq.js` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/static/js/hjelp/order_faq.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/ask.html` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/ask.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/faq.html` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/faq.html`

 * *Files 7% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 {% block browser_title %}FAQ ({% trans "Frequently Asked Questions" %}){% endblock browser_title %}
 
 {% block content %}
     {% for section in sections %}
       <section>
         <h4>
-          <i class="material-icons iconify" data-icon="mdi:{{ section.icon }}" {% firstof  section.icon_color "black" %}-text"></i>
+          <i class="material-icons iconify" data-icon="{{ section.icon }}" {% firstof  section.icon_color "black" %}-text"></i>
           {{ section.name }}
         </h4>
 
         <ul class="collapsible">
           {% for question in section.visible_questions %}
             <li>
               <div class="collapsible-header">
-                <i class="material-icons iconify" data-icon="mdi:{% firstof question.icon "frequently-asked-questions" %}"></i>
+                <i class="material-icons iconify" data-icon="{% firstof question.icon "question_answer" %}"></i>
                 {{ question.question_text }}
               </div>
               <div class="collapsible-body">
                 {{ question.answer_text|add_class_to_el:"ul, browser-default"|safe }}
               </div>
             </li>
           {% empty %}
```

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/feedback.html` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/feedback.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/feedback_submitted.html` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/feedback_submitted.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/issue_report.html` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/issue_report.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/issue_report_submitted.html` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/issue_report_submitted.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/order_faq.html` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/order_faq.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/hjelp/question_submitted.html` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/hjelp/question_submitted.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/templated_email/faq.email` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/templated_email/faq.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/templated_email/feedback.email` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/templated_email/feedback.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/templated_email/html_mail.css` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/templated_email/html_mail.css`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/templates/templated_email/rebus.email` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/templates/templated_email/rebus.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/urls.py` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/aleksis/apps/hjelp/views.py` & `aleksis_app_hjelp-3.0b0/aleksis/apps/hjelp/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/Makefile` & `aleksis_app_hjelp-3.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/_static/ask_a_question.png` & `aleksis_app_hjelp-3.0b0/docs/_static/ask_a_question.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/_static/faq.png` & `aleksis_app_hjelp-3.0b0/docs/_static/faq.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/_static/faq_question.png` & `aleksis_app_hjelp-3.0b0/docs/_static/faq_question.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/_static/faq_section.png` & `aleksis_app_hjelp-3.0b0/docs/_static/faq_section.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/_static/feedback.png` & `aleksis_app_hjelp-3.0b0/docs/_static/feedback.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/_static/issue_categories.png` & `aleksis_app_hjelp-3.0b0/docs/_static/issue_categories.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/_static/issue_category.png` & `aleksis_app_hjelp-3.0b0/docs/_static/issue_category.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/_static/manage_faq.png` & `aleksis_app_hjelp-3.0b0/docs/_static/manage_faq.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/_static/report_issue.png` & `aleksis_app_hjelp-3.0b0/docs/_static/report_issue.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/admin/10_managing_faqs.rst` & `aleksis_app_hjelp-3.0b0/docs/admin/10_managing_faqs.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/admin/15_managing_issue_report_form.rst` & `aleksis_app_hjelp-3.0b0/docs/admin/15_managing_issue_report_form.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/admin/40_preferences.rst` & `aleksis_app_hjelp-3.0b0/docs/admin/40_preferences.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/conf.py` & `aleksis_app_hjelp-3.0b0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = "AlekSIS-App-Hjelp"
 copyright = "2018-2022 The AlekSIS team"
 author = "The AlekSIS Team"
 
 # The short X.Y version
 version = "3.0"
 # The full version, including alpha/beta/rc tags
-release = "3.0"
+release = "3.0b0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `aleksis_app_hjelp-3.0/docs/index.rst` & `aleksis_app_hjelp-3.0b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/make.bat` & `aleksis_app_hjelp-3.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/user/01_faq.rst` & `aleksis_app_hjelp-3.0b0/docs/user/01_faq.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/user/10_issue_reporting.rst` & `aleksis_app_hjelp-3.0b0/docs/user/10_issue_reporting.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/docs/user/20_feedback.rst` & `aleksis_app_hjelp-3.0b0/docs/user/20_feedback.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/pyproject.toml` & `aleksis_app_hjelp-3.0b0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Hjelp"
-version = "3.0"
+version = "3.0b0"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -34,15 +34,15 @@
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aleksis-core = "^3.0"
+aleksis-core = "^3.0b0"
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
 
 [tool.poetry.plugins."aleksis.app"]
 hjelp = "aleksis.apps.hjelp.apps:HjelpConfig"
```

### Comparing `aleksis_app_hjelp-3.0/tox.ini` & `aleksis_app_hjelp-3.0b0/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_hjelp-3.0/setup.py` & `aleksis_app_hjelp-3.0b0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,22 +18,22 @@
                         'locale/uk/LC_MESSAGES/*',
                         'static/css/hjelp/*',
                         'static/js/hjelp/*',
                         'templates/hjelp/*',
                         'templates/templated_email/*']}
 
 install_requires = \
-['aleksis-core>=3.0,<4.0']
+['aleksis-core>=3.0b0,<4.0']
 
 entry_points = \
 {'aleksis.app': ['hjelp = aleksis.apps.hjelp.apps:HjelpConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-hjelp',
-    'version': '3.0',
+    'version': '3.0b0',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Hjelp (FAQ, issue reporting and support)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Hjelp (FAQ and support)\n=================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\n* Report issues\n* Frequently asked questions\n* Ask questions\n* Feedback\n\nLicence\n-------\n\n::\n\n  Copyright © 2019, 2020, 2021, 2022 Jonathan Weth <dev@jonathanweth.de>\n  Copyright © 2019, 2020, 2021 Julian Leucker <leuckeju@katharineum.de>\n  Copyright © 2019, 2020, 2021 Hangzhi Yu <yuha@katharineum.de>\n  Copyright © 2019 Frank Poetzsch-Heffter <p-h@katharineum.de>\n  Copyright © 2020 Dominik George <dominik.george@teckids.org>  \n  Copyright © 2020 Tom Teichler <tom.teichler@teckids.org>\n\n  Licenced under the EUPL, version 1.2 or later, by Teckids e.V. (Bonn, Germany).\n\nPlease see the LICENCE file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://aleksis.org/\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Julian Leucker',
     'author_email': 'leuckeju@katharineum.de',
     'maintainer': 'Jonathan Weth',
     'maintainer_email': 'dev@jonathanweth.de',
     'url': 'https://aleksis.org/',
```

### Comparing `aleksis_app_hjelp-3.0/PKG-INFO` & `aleksis_app_hjelp-3.0b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-hjelp
-Version: 3.0
+Version: 3.0b0
 Summary: AlekSIS (School Information System) — App Hjelp (FAQ, issue reporting and support)
 Home-page: https://aleksis.org/
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,support,feedback
 Author: Julian Leucker
 Author-email: leuckeju@katharineum.de
 Maintainer: Jonathan Weth
@@ -17,15 +17,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Typing :: Typed
-Requires-Dist: aleksis-core (>=3.0,<4.0)
+Requires-Dist: aleksis-core (>=3.0b0,<4.0)
 Project-URL: Documentation, https://aleksis.org/AlekSIS/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS-App-Hjelp
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Hjelp (FAQ and support)
 =================================================================
```

