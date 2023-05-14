# Comparing `tmp/aleksis_app_chronos-3.0.dev1.tar.gz` & `tmp/aleksis_app_chronos-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_chronos-3.0.dev1.tar", max compression
+gzip compressed data, was "aleksis_app_chronos-3.0b0.tar", max compression
```

## Comparing `aleksis_app_chronos-3.0.dev1.tar` & `aleksis_app_chronos-3.0b0.tar`

### file list

```diff
@@ -1,153 +1,154 @@
--rw-r--r--   0        0        0     9873 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/LICENCE.rst
--rw-r--r--   0        0        0     1835 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/README.rst
--rw-r--r--   0        0        0      153 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/__init__.py
--rw-r--r--   0        0        0      326 2023-01-24 12:27:35.991240 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6411 2023-01-24 12:27:37.019249 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/__pycache__/admin.cpython-310.pyc
--rw-r--r--   0        0        0     3980 2023-01-24 12:27:36.375243 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/__pycache__/apps.cpython-310.pyc
--rw-r--r--   0        0        0      510 2023-01-24 12:27:37.071250 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/__pycache__/form_extensions.cpython-310.pyc
--rw-r--r--   0        0        0    28777 2023-01-24 12:27:36.907248 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/__pycache__/managers.cpython-310.pyc
--rw-r--r--   0        0        0     2626 2023-01-24 12:27:36.907248 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/__pycache__/mixins.cpython-310.pyc
--rw-r--r--   0        0        0     5098 2023-01-24 12:27:37.071250 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/__pycache__/model_extensions.cpython-310.pyc
--rw-r--r--   0        0        0    40828 2023-01-24 12:27:36.899248 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/__pycache__/models.cpython-310.pyc
--rw-r--r--   0        0        0     3644 2023-01-24 12:27:37.127250 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/__pycache__/preferences.cpython-310.pyc
--rw-r--r--   0        0        0     1825 2023-01-24 12:27:37.039250 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/__pycache__/rules.cpython-310.pyc
--rw-r--r--   0        0        0     5284 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/admin.py
--rw-r--r--   0        0        0     3899 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/apps.py
--rw-r--r--   0        0        0     6133 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/filters.py
--rw-r--r--   0        0        0      335 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/form_extensions.py
--rw-r--r--   0        0        0     2013 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/forms.py
--rw-r--r--   0        0        0     4831 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/frontend/index.js
--rw-r--r--   0        0        0       56 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/frontend/messages/de.json
--rw-r--r--   0        0        0      367 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/frontend/messages/en.json
--rw-r--r--   0        0        0      463 2023-01-24 12:27:37.147251 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19469 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    12855 2023-01-24 12:27:37.151250 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    26928 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      779 2023-01-24 12:27:37.155251 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19536 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      513 2023-01-24 12:27:37.159251 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19431 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-01-24 12:27:37.155251 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19287 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    16496 2023-01-24 12:27:37.159251 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    27801 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-01-24 12:27:37.151250 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19287 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    16023 2023-01-24 12:27:37.159251 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    29893 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    30461 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/managers.py
--rw-r--r--   0        0        0     2649 2023-01-24 12:25:36.226137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/menus.py
--rw-r--r--   0        0        0    42263 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0001_initial.py
--rw-r--r--   0        0        0     8543 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0002_school_term_validity.py
--rw-r--r--   0        0        0      877 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0003_school_term_validity_fixes.py
--rw-r--r--   0        0        0     1609 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0004_substitution_extra_lesson_year.py
--rw-r--r--   0        0        0     1002 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0005_add_permissions.py
--rw-r--r--   0        0        0     2450 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0006_indexes.py
--rw-r--r--   0        0        0      679 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0007_more_permissions.py
--rw-r--r--   0        0        0     3761 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0008_unique_constraints.py
--rw-r--r--   0        0        0     1639 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0009_automaticplan.py
--rw-r--r--   0        0        0      343 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0010_remove_subject_unique_name_per_site.py
--rw-r--r--   0        0        0     2141 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0011_exam.py
--rw-r--r--   0        0        0      733 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0012_add_supervision_global_permission.py
--rw-r--r--   0        0        0     1958 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0013_move_room_to_core.py
--rw-r--r--   0        0        0        0 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/__init__.py
--rw-r--r--   0        0        0     1762 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/mixins.py
--rw-r--r--   0        0        0     5180 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/model_extensions.py
--rw-r--r--   0        0        0    45893 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/models.py
--rw-r--r--   0        0        0     3560 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/preferences.py
--rw-r--r--   0        0        0     2589 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/rules.py
--rw-r--r--   0        0        0     2644 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/static/css/chronos/timetable.css
--rw-r--r--   0        0        0      551 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/static/css/chronos/timetable_print.css
--rw-r--r--   0        0        0      462 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/static/js/chronos/date_select.js
--rw-r--r--   0        0        0      607 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/static/js/chronos/week_select.js
--rw-r--r--   0        0        0     4311 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/tables.py
--rw-r--r--   0        0        0     1926 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/all.html
--rw-r--r--   0        0        0     1049 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/edit_substitution.html
--rw-r--r--   0        0        0     1080 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/edit_supervision_substitution.html
--rw-r--r--   0        0        0     1180 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/lessons_day.html
--rw-r--r--   0        0        0     2156 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/my_timetable.html
--rw-r--r--   0        0        0     1016 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/datepicker.html
--rw-r--r--   0        0        0      619 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/elements.html
--rw-r--r--   0        0        0     1271 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/event.html
--rw-r--r--   0        0        0      989 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/extra_lesson.html
--rw-r--r--   0        0        0      115 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/group.html
--rw-r--r--   0        0        0      359 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/groups.html
--rw-r--r--   0        0        0      397 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/groups_part.html
--rw-r--r--   0        0        0     2274 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/headerbox.html
--rw-r--r--   0        0        0       83 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/holiday.html
--rw-r--r--   0        0        0     4401 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/lesson.html
--rw-r--r--   0        0        0      883 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/lessons_col.html
--rw-r--r--   0        0        0      538 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/period_time.html
--rw-r--r--   0        0        0      207 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/room.html
--rw-r--r--   0        0        0      135 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subject.html
--rw-r--r--   0        0        0      200 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subject_colour.html
--rw-r--r--   0        0        0      233 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subs/badge.html
--rw-r--r--   0        0        0      278 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subs/colour.html
--rw-r--r--   0        0        0      106 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subs/comment.html
--rw-r--r--   0        0        0      264 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subs/groups.html
--rw-r--r--   0        0        0      708 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subs/period.html
--rw-r--r--   0        0        0     1642 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subs/room.html
--rw-r--r--   0        0        0     1250 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subs/subject.html
--rw-r--r--   0        0        0     1227 2023-01-24 12:25:36.230137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subs/teachers.html
--rw-r--r--   0        0        0     1347 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/supervision.html
--rw-r--r--   0        0        0      284 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/teachers.html
--rw-r--r--   0        0        0      101 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/today.html
--rw-r--r--   0        0        0     1734 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/week_select.html
--rw-r--r--   0        0        0     2644 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/week_timetable.html
--rw-r--r--   0        0        0     3262 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/substitutions.html
--rw-r--r--   0        0        0     2899 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/substitutions_print.html
--rw-r--r--   0        0        0     1108 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/supervisions_day.html
--rw-r--r--   0        0        0     5144 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/timetable.html
--rw-r--r--   0        0        0     1532 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/timetable_print.html
--rw-r--r--   0        0        0      880 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/widget.html
--rw-r--r--   0        0        0       42 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/search/indexes/chronos/room_text.txt
--rw-r--r--   0        0        0        0 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templatetags/__init__.py
--rw-r--r--   0        0        0      797 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templatetags/common.py
--rw-r--r--   0        0        0     1346 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templatetags/week_helpers.py
--rw-r--r--   0        0        0     2775 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/tests/regression/test_regression.py
--rw-r--r--   0        0        0    11091 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/tests/test_notifications.py
--rw-r--r--   0        0        0     2430 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/urls.py
--rw-r--r--   0        0        0     7469 2023-01-24 12:27:37.043249 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/__pycache__/build.cpython-310.pyc
--rw-r--r--   0        0        0     5758 2023-01-24 12:27:36.911248 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/__pycache__/change_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     6508 2023-01-24 12:27:37.043249 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/__pycache__/chronos_helpers.cpython-310.pyc
--rw-r--r--   0        0        0     1440 2023-01-24 12:27:36.907248 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/__pycache__/date.cpython-310.pyc
--rw-r--r--   0        0        0      887 2023-01-24 12:27:36.911248 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/__pycache__/format.cpython-310.pyc
--rw-r--r--   0        0        0      502 2023-01-24 12:27:37.047250 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/__pycache__/js.cpython-310.pyc
--rw-r--r--   0        0        0     5059 2023-01-24 12:27:37.071250 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/__pycache__/notifications.cpython-310.pyc
--rw-r--r--   0        0        0     2550 2023-01-24 12:27:37.039250 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/__pycache__/predicates.cpython-310.pyc
--rw-r--r--   0        0        0    17686 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/build.py
--rw-r--r--   0        0        0     5629 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/change_tracker.py
--rw-r--r--   0        0        0     8120 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/chronos_helpers.py
--rw-r--r--   0        0        0     1069 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/date.py
--rw-r--r--   0        0        0      405 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/format.py
--rw-r--r--   0        0        0      234 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/js.py
--rw-r--r--   0        0        0     8463 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/notifications.py
--rw-r--r--   0        0        0     2371 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/predicates.py
--rw-r--r--   0        0        0    16480 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/views.py
--rw-r--r--   0        0        0      581 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/docs/Makefile
--rw-r--r--   0        0        0   126772 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/docs/_static/all_timetables.png
--rw-r--r--   0        0        0   134225 2023-01-24 12:25:36.234137 aleksis_app_chronos-3.0.dev1/docs/_static/class_timetable.png
--rw-r--r--   0        0        0   112498 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/_static/daily_lessons.png
--rw-r--r--   0        0        0   115275 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/_static/my_timetable.png
--rw-r--r--   0        0        0   121926 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/_static/print_timetable.png
--rw-r--r--   0        0        0    64368 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/_static/substitution_edit.png
--rw-r--r--   0        0        0   100602 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/_static/substitutions.png
--rw-r--r--   0        0        0   135003 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/_static/substitutions_print.png
--rw-r--r--   0        0        0      142 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/admin/00_index.rst
--rw-r--r--   0        0        0      472 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/admin/10_managing_data.rst
--rw-r--r--   0        0        0     1330 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/admin/11_notifications.rst
--rw-r--r--   0        0        0     1139 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/admin/40_preferences.rst
--rw-r--r--   0        0        0     6403 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/conf.py
--rw-r--r--   0        0        0      526 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/index.rst
--rw-r--r--   0        0        0      787 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/make.bat
--rw-r--r--   0        0        0      124 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/user/00_index.rst
--rw-r--r--   0        0        0     3219 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/user/01_using_timetables.rst
--rw-r--r--   0        0        0      797 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/user/10_substitution_plan.rst
--rw-r--r--   0        0        0      536 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/user/11_notifications.rst
--rw-r--r--   0        0        0      815 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/user/15_manage_substitutions.rst
--rw-r--r--   0        0        0      384 2023-01-24 12:25:36.238137 aleksis_app_chronos-3.0.dev1/docs/user/40_preferences.rst
--rw-r--r--   0        0        0     1997 2023-01-24 12:26:12.154467 aleksis_app_chronos-3.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     2342 2023-01-24 12:25:36.250137 aleksis_app_chronos-3.0.dev1/tox.ini
--rw-r--r--   0        0        0     3893 1970-01-01 00:00:00.000000 aleksis_app_chronos-3.0.dev1/setup.py
--rw-r--r--   0        0        0     3074 1970-01-01 00:00:00.000000 aleksis_app_chronos-3.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0    10107 2023-02-27 16:43:16.439024 aleksis_app_chronos-3.0b0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-02-27 16:43:16.439024 aleksis_app_chronos-3.0b0/LICENCE.rst
+-rw-r--r--   0        0        0     1835 2023-02-27 16:43:16.439024 aleksis_app_chronos-3.0b0/README.rst
+-rw-r--r--   0        0        0      153 2023-02-27 16:43:16.439024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/__init__.py
+-rw-r--r--   0        0        0      447 2023-02-27 16:46:06.442703 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10437 2023-02-27 16:46:07.762700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0     6047 2023-02-27 16:46:06.906702 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0      760 2023-02-27 16:46:07.822700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/__pycache__/form_extensions.cpython-311.pyc
+-rw-r--r--   0        0        0    48201 2023-02-27 16:46:07.694700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/__pycache__/managers.cpython-311.pyc
+-rw-r--r--   0        0        0     3754 2023-02-27 16:46:07.698700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0        0        0     7824 2023-02-27 16:46:07.818700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/__pycache__/model_extensions.cpython-311.pyc
+-rw-r--r--   0        0        0    70965 2023-02-27 16:46:07.686700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     5735 2023-02-27 16:46:07.898700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0     2754 2023-02-27 16:46:07.782700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     5284 2023-02-27 16:43:16.439024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/admin.py
+-rw-r--r--   0        0        0     3899 2023-02-27 16:43:16.439024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/apps.py
+-rw-r--r--   0        0        0     6133 2023-02-27 16:43:16.439024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/filters.py
+-rw-r--r--   0        0        0      335 2023-02-27 16:43:16.439024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/form_extensions.py
+-rw-r--r--   0        0        0     2013 2023-02-27 16:43:16.439024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/forms.py
+-rw-r--r--   0        0        0     6936 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/frontend/index.js
+-rw-r--r--   0        0        0      376 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/frontend/messages/de.json
+-rw-r--r--   0        0        0      368 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/frontend/messages/en.json
+-rw-r--r--   0        0        0      438 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/frontend/messages/ru.json
+-rw-r--r--   0        0        0      414 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/frontend/messages/uk.json
+-rw-r--r--   0        0        0      463 2023-02-27 16:46:08.118699 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19469 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    12855 2023-02-27 16:46:08.122700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    26928 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      779 2023-02-27 16:46:08.118699 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19536 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      513 2023-02-27 16:46:08.122700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19431 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-27 16:46:08.114699 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19287 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    16496 2023-02-27 16:46:08.118699 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27801 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-27 16:46:08.118699 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19287 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    16023 2023-02-27 16:46:08.122700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    29893 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    30461 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/managers.py
+-rw-r--r--   0        0        0     2649 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/menus.py
+-rw-r--r--   0        0        0    42263 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0001_initial.py
+-rw-r--r--   0        0        0     8543 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0002_school_term_validity.py
+-rw-r--r--   0        0        0      877 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0003_school_term_validity_fixes.py
+-rw-r--r--   0        0        0     1609 2023-02-27 16:43:16.443024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0004_substitution_extra_lesson_year.py
+-rw-r--r--   0        0        0     1002 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0005_add_permissions.py
+-rw-r--r--   0        0        0     2450 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0006_indexes.py
+-rw-r--r--   0        0        0      679 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0007_more_permissions.py
+-rw-r--r--   0        0        0     3761 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0008_unique_constraints.py
+-rw-r--r--   0        0        0     1639 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0009_automaticplan.py
+-rw-r--r--   0        0        0      343 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0010_remove_subject_unique_name_per_site.py
+-rw-r--r--   0        0        0     2141 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0011_exam.py
+-rw-r--r--   0        0        0      733 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0012_add_supervision_global_permission.py
+-rw-r--r--   0        0        0     1958 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0013_move_room_to_core.py
+-rw-r--r--   0        0        0        0 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/__init__.py
+-rw-r--r--   0        0        0     1762 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/mixins.py
+-rw-r--r--   0        0        0     5180 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/model_extensions.py
+-rw-r--r--   0        0        0    45891 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/models.py
+-rw-r--r--   0        0        0     3560 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/preferences.py
+-rw-r--r--   0        0        0     2589 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/rules.py
+-rw-r--r--   0        0        0     2478 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/static/css/chronos/timetable.css
+-rw-r--r--   0        0        0      519 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/static/css/chronos/timetable_print.css
+-rw-r--r--   0        0        0      449 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/static/js/chronos/date_select.js
+-rw-r--r--   0        0        0      579 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/static/js/chronos/week_select.js
+-rw-r--r--   0        0        0     4311 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/tables.py
+-rw-r--r--   0        0        0     1926 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/all.html
+-rw-r--r--   0        0        0     1049 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/edit_substitution.html
+-rw-r--r--   0        0        0     1080 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/edit_supervision_substitution.html
+-rw-r--r--   0        0        0     1180 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/lessons_day.html
+-rw-r--r--   0        0        0     2156 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/my_timetable.html
+-rw-r--r--   0        0        0     1016 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/datepicker.html
+-rw-r--r--   0        0        0      619 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/elements.html
+-rw-r--r--   0        0        0     1271 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/event.html
+-rw-r--r--   0        0        0      989 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/extra_lesson.html
+-rw-r--r--   0        0        0      115 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/group.html
+-rw-r--r--   0        0        0      359 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/groups.html
+-rw-r--r--   0        0        0      397 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/groups_part.html
+-rw-r--r--   0        0        0     2274 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/headerbox.html
+-rw-r--r--   0        0        0       83 2023-02-27 16:43:16.447024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/holiday.html
+-rw-r--r--   0        0        0     4401 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/lesson.html
+-rw-r--r--   0        0        0      883 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/lessons_col.html
+-rw-r--r--   0        0        0      538 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/period_time.html
+-rw-r--r--   0        0        0      207 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/room.html
+-rw-r--r--   0        0        0      135 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subject.html
+-rw-r--r--   0        0        0      200 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subject_colour.html
+-rw-r--r--   0        0        0      233 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subs/badge.html
+-rw-r--r--   0        0        0      278 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subs/colour.html
+-rw-r--r--   0        0        0      106 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subs/comment.html
+-rw-r--r--   0        0        0      264 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subs/groups.html
+-rw-r--r--   0        0        0      708 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subs/period.html
+-rw-r--r--   0        0        0     1642 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subs/room.html
+-rw-r--r--   0        0        0     1250 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subs/subject.html
+-rw-r--r--   0        0        0     1227 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subs/teachers.html
+-rw-r--r--   0        0        0     1347 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/supervision.html
+-rw-r--r--   0        0        0      284 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/teachers.html
+-rw-r--r--   0        0        0      101 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/today.html
+-rw-r--r--   0        0        0     1734 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/week_select.html
+-rw-r--r--   0        0        0     2644 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/week_timetable.html
+-rw-r--r--   0        0        0     3262 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/substitutions.html
+-rw-r--r--   0        0        0     2899 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/substitutions_print.html
+-rw-r--r--   0        0        0     1108 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/supervisions_day.html
+-rw-r--r--   0        0        0     5144 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/timetable.html
+-rw-r--r--   0        0        0     1532 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/timetable_print.html
+-rw-r--r--   0        0        0      880 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/widget.html
+-rw-r--r--   0        0        0        0 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templatetags/__init__.py
+-rw-r--r--   0        0        0      797 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templatetags/common.py
+-rw-r--r--   0        0        0     1346 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templatetags/week_helpers.py
+-rw-r--r--   0        0        0     2775 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/tests/regression/test_regression.py
+-rw-r--r--   0        0        0    11089 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/tests/test_notifications.py
+-rw-r--r--   0        0        0     2430 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/urls.py
+-rw-r--r--   0        0        0    15617 2023-02-27 16:46:07.790700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/__pycache__/build.cpython-311.pyc
+-rw-r--r--   0        0        0     9644 2023-02-27 16:46:07.702700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/__pycache__/change_tracker.cpython-311.pyc
+-rw-r--r--   0        0        0    12513 2023-02-27 16:46:07.786700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/__pycache__/chronos_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     2080 2023-02-27 16:46:07.694700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/__pycache__/date.cpython-311.pyc
+-rw-r--r--   0        0        0     1257 2023-02-27 16:46:07.702700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/__pycache__/format.cpython-311.pyc
+-rw-r--r--   0        0        0      743 2023-02-27 16:46:07.790700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/__pycache__/js.cpython-311.pyc
+-rw-r--r--   0        0        0    11358 2023-02-27 16:46:07.822700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/__pycache__/notifications.cpython-311.pyc
+-rw-r--r--   0        0        0     4090 2023-02-27 16:46:07.782700 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/__pycache__/predicates.cpython-311.pyc
+-rw-r--r--   0        0        0    17685 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/build.py
+-rw-r--r--   0        0        0     5629 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/change_tracker.py
+-rw-r--r--   0        0        0     8117 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/chronos_helpers.py
+-rw-r--r--   0        0        0     1069 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/date.py
+-rw-r--r--   0        0        0      405 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/format.py
+-rw-r--r--   0        0        0      234 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/js.py
+-rw-r--r--   0        0        0     8463 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/notifications.py
+-rw-r--r--   0        0        0     2368 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/predicates.py
+-rw-r--r--   0        0        0    16480 2023-02-27 16:43:16.451024 aleksis_app_chronos-3.0b0/aleksis/apps/chronos/views.py
+-rw-r--r--   0        0        0      581 2023-02-27 16:43:16.455024 aleksis_app_chronos-3.0b0/docs/Makefile
+-rw-r--r--   0        0        0   126772 2023-02-27 16:43:16.455024 aleksis_app_chronos-3.0b0/docs/_static/all_timetables.png
+-rw-r--r--   0        0        0   134225 2023-02-27 16:43:16.459024 aleksis_app_chronos-3.0b0/docs/_static/class_timetable.png
+-rw-r--r--   0        0        0   112498 2023-02-27 16:43:16.459024 aleksis_app_chronos-3.0b0/docs/_static/daily_lessons.png
+-rw-r--r--   0        0        0   115275 2023-02-27 16:43:16.459024 aleksis_app_chronos-3.0b0/docs/_static/my_timetable.png
+-rw-r--r--   0        0        0   121926 2023-02-27 16:43:16.463024 aleksis_app_chronos-3.0b0/docs/_static/print_timetable.png
+-rw-r--r--   0        0        0    64368 2023-02-27 16:43:16.463024 aleksis_app_chronos-3.0b0/docs/_static/substitution_edit.png
+-rw-r--r--   0        0        0   100602 2023-02-27 16:43:16.463024 aleksis_app_chronos-3.0b0/docs/_static/substitutions.png
+-rw-r--r--   0        0        0   135003 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/_static/substitutions_print.png
+-rw-r--r--   0        0        0      142 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/admin/00_index.rst
+-rw-r--r--   0        0        0      472 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/admin/10_managing_data.rst
+-rw-r--r--   0        0        0     1330 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/admin/11_notifications.rst
+-rw-r--r--   0        0        0     1139 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/admin/40_preferences.rst
+-rw-r--r--   0        0        0     6400 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/conf.py
+-rw-r--r--   0        0        0      526 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/make.bat
+-rw-r--r--   0        0        0      124 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/user/00_index.rst
+-rw-r--r--   0        0        0     3219 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/user/01_using_timetables.rst
+-rw-r--r--   0        0        0      797 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/user/10_substitution_plan.rst
+-rw-r--r--   0        0        0      536 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/user/11_notifications.rst
+-rw-r--r--   0        0        0      815 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/user/15_manage_substitutions.rst
+-rw-r--r--   0        0        0      384 2023-02-27 16:43:16.471024 aleksis_app_chronos-3.0b0/docs/user/40_preferences.rst
+-rw-r--r--   0        0        0     1989 2023-02-27 16:43:54.686952 aleksis_app_chronos-3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-02-27 16:43:16.487024 aleksis_app_chronos-3.0b0/tox.ini
+-rw-r--r--   0        0        0     3821 1970-01-01 00:00:00.000000 aleksis_app_chronos-3.0b0/setup.py
+-rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 aleksis_app_chronos-3.0b0/PKG-INFO
```

### Comparing `aleksis_app_chronos-3.0.dev1/CHANGELOG.rst` & `aleksis_app_chronos-3.0b0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,41 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-Unreleased
-----------
+`3.0b0` - 2023-02-16
+--------------------
+
+This version requires AlekSIS-Core 3.0. It is incompatible with any previous
+version.
+
+Removed
+~~~~~~~
+
+* `Room` model is now available in AlekSIS-Core 3.0
+* Legacy menu integration for AlekSIS-Core pre-3.0
 
 Added
 ~~~~~
 
-* Add support for operation with SPA.
+* Support for SPA in AlekSIS-Core 3.0
 
 Changed
 ~~~~~~~
 
 * Improve rendering of substituted or cancelled items on daily lessons/supervisions pages.
 
 Fixed
 ~~~~~
 
-* Migrations wouldn't run on new installations due to a faulty reference to SchoolTerm.
 * The daily lessons page did not work correctly due to faulty pre-filtering of lessons.
-* Substitution form teacher selections also included students
+* Substitution form teacher selections also included students in some cases
 * Getting the max and min periods for events failed due to using always the current school term.
   Typically, that caused problems when the schedule changed (more or less periods on a day). 
 
 `2.5`_ - 2022-11-12
 -------------------
 
 Added
@@ -362,7 +370,8 @@
 .. _2.2: https://edugit.org/AlekSIS/Official/AlekSIS-App-Chronos/-/tags/2.2
 .. _2.2.1: https://edugit.org/AlekSIS/Official/AlekSIS-App-Chronos/-/tags/2.2.1
 .. _2.3: https://edugit.org/AlekSIS/Official/AlekSIS-App-Chronos/-/tags/2.3
 .. _2.4: https://edugit.org/AlekSIS/Official/AlekSIS-App-Chronos/-/tags/2.4
 .. _2.4.1: https://edugit.org/AlekSIS/Official/AlekSIS-App-Chronos/-/tags/2.4.1
 .. _2.4.2: https://edugit.org/AlekSIS/Official/AlekSIS-App-Chronos/-/tags/2.4.2
 .. _2.5: https://edugit.org/AlekSIS/Official/AlekSIS-App-Chronos/-/tags/2.5
+.. _3.0b0: https://edugit.org/AlekSIS/Official/AlekSIS-App-Chronos/-/tags/3.0b0
```

### Comparing `aleksis_app_chronos-3.0.dev1/LICENCE.rst` & `aleksis_app_chronos-3.0b0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/README.rst` & `aleksis_app_chronos-3.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/admin.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/admin.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/apps.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/filters.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/forms.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.mo` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.mo` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.po` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/managers.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/managers.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/menus.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/menus.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0001_initial.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0002_school_term_validity.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0002_school_term_validity.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0003_school_term_validity_fixes.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0003_school_term_validity_fixes.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0004_substitution_extra_lesson_year.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0004_substitution_extra_lesson_year.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0005_add_permissions.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0005_add_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0006_indexes.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0006_indexes.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0007_more_permissions.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0007_more_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0008_unique_constraints.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0008_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0009_automaticplan.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0009_automaticplan.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0011_exam.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0011_exam.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0012_add_supervision_global_permission.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0012_add_supervision_global_permission.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/migrations/0013_move_room_to_core.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/migrations/0013_move_room_to_core.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/mixins.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/mixins.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/model_extensions.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/model_extensions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/models.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,14 @@
         This will respect the relation to validity ranges.
         """
         return cls.objects.on_day(day).filter(period=period, weekday=day.weekday()).first()
 
     @classproperty
     @cache_memoize(3600)
     def period_min(cls) -> int:
-
         return (
             cls.objects.for_current_or_all()
             .aggregate(period__min=Coalesce(Min("period"), 1))
             .get("period__min")
         )
 
     @classproperty
@@ -1076,15 +1075,14 @@
     def __str__(self):
         if self.title:
             return self.title
         else:
             return _("Event {pk}").format(pk=self.pk)
 
     def get_period_min(self, day) -> int:
-
         return (
             TimePeriod.objects.on_day(day)
             .aggregate(period__min=Coalesce(Min("period"), 1))
             .get("period__min")
         )
 
     def get_period_max(self, day) -> int:
```

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/preferences.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/rules.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/static/css/chronos/timetable_print.css` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/static/css/chronos/timetable_print.css`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-.timetable-plan .row, .timetable-plan .col {
-    display: flex;
-    padding: 0rem;
+.timetable-plan .row,
+.timetable-plan .col {
+  display: flex;
+  padding: 0rem;
 }
 
 .timetable-plan .row {
-    margin-bottom: 0rem;
+  margin-bottom: 0rem;
 }
 
-.lesson-card, .timetable-title-card {
-    margin: 0;
-    display: flex;
-    flex-grow: 1;
-    min-height: 40px;
-    box-shadow: none;
-    border: 1px solid black;
-    margin-right: -1px;
-    margin-top: -1px;
-    border-radius: 0px;
-    font-size: 11px;
+.lesson-card,
+.timetable-title-card {
+  margin: 0;
+  display: flex;
+  flex-grow: 1;
+  min-height: 40px;
+  box-shadow: none;
+  border: 1px solid black;
+  margin-right: -1px;
+  margin-top: -1px;
+  border-radius: 0px;
+  font-size: 11px;
 }
 .lesson-card .card-content > div {
-    padding: 1px;
+  padding: 1px;
 }
 
 .card .card-title {
-    font-size: 18px;
+  font-size: 18px;
 }
 
 .timetable-title-card .card-content {
-    padding: 7px;
+  padding: 7px;
 }
```

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/tables.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/all.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/all.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/edit_substitution.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/edit_substitution.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/edit_supervision_substitution.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/edit_supervision_substitution.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/lessons_day.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/lessons_day.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/my_timetable.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/my_timetable.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/datepicker.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/datepicker.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/elements.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/elements.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/event.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/event.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/extra_lesson.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/extra_lesson.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/headerbox.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/headerbox.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/lesson.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/lesson.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/lessons_col.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/lessons_col.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/period_time.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/period_time.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subs/period.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subs/period.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subs/room.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subs/room.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subs/subject.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subs/subject.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/subs/teachers.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/subs/teachers.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/supervision.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/supervision.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/week_select.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/week_select.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/partials/week_timetable.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/partials/week_timetable.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/substitutions.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/substitutions.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/substitutions_print.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/substitutions_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/supervisions_day.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/supervisions_day.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/timetable.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/timetable.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/timetable_print.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/timetable_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templates/chronos/widget.html` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templates/chronos/widget.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templatetags/common.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templatetags/common.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/templatetags/week_helpers.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/templatetags/week_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/tests/regression/test_regression.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/tests/regression/test_regression.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/tests/test_notifications.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/tests/test_notifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,14 @@
             )
 
     def test_outside_transaction(self):
         with pytest.raises(RuntimeError):
             TimetableDataChangeTracker()
 
     def test_create_detection(self):
-
         with transaction.atomic():
             tracker = TimetableDataChangeTracker()
 
             assert not tracker.changes
 
             lesson_substitution = LessonSubstitution.objects.create(
                 week=20, year=2020, lesson_period=self.period_1, cancelled=True
@@ -183,15 +182,14 @@
             change = tracker.changes[tracker.get_instance_key(lesson_substitution)]
             assert change.instance == lesson_substitution
             assert change.created
             assert not change.deleted
             assert change.changed_fields
 
     def test_change_detection(self):
-
         with transaction.atomic():
             lesson_substitution = LessonSubstitution.objects.create(
                 week=20, year=2020, lesson_period=self.period_1, cancelled=True
             )
 
             tracker = TimetableDataChangeTracker()
```

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/urls.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/build.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,14 @@
     base: List[Tuple[int, str]], wanted_week: CalendarWeek, with_holidays: bool = True
 ) -> List[dict]:
     if with_holidays:
         holidays_per_weekday = Holiday.in_week(wanted_week)
 
     weekdays = []
     for key, name in base[TimePeriod.weekday_min : TimePeriod.weekday_max + 1]:
-
         weekday = {
             "key": key,
             "name": name,
             "date": wanted_week[key],
         }
         if with_holidays:
             weekday["holiday"] = holidays_per_weekday[key] if key in holidays_per_weekday else None
```

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/change_tracker.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/change_tracker.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/chronos_helpers.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/chronos_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
     if not check_global_permission(user, "chronos.view_all_room_timetables"):
         checker.prefetch_perms(rooms)
 
         wanted_rooms = set()
 
         for room in rooms:
-            if checker.has_perm("chronos.view_room_timetable", room):
+            if checker.has_perm("core.view_room_timetable", room):
                 wanted_rooms.add(room.pk)
 
         rooms = rooms.filter(Q(pk__in=wanted_rooms))
 
     return rooms
```

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/date.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/date.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/notifications.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/notifications.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/util/predicates.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/util/predicates.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """
     Check if can access room timetable.
 
     Predicate which checks whether the user is allowed
     to access the requested room timetable.
     """
     return has_global_perm("chronos.view_all_room_timetables")(user) or has_object_perm(
-        "chronos.view_room_timetable"
+        "core.view_room_timetable"
     )(user, obj)
 
 
 @predicate
 def has_any_timetable_object(user: User) -> bool:
     """Predicate which checks whether there are any timetables the user is allowed to access."""
     return get_classes(user).exists() or get_rooms(user).exists() or get_teachers(user).exists()
```

### Comparing `aleksis_app_chronos-3.0.dev1/aleksis/apps/chronos/views.py` & `aleksis_app_chronos-3.0b0/aleksis/apps/chronos/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/Makefile` & `aleksis_app_chronos-3.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/_static/all_timetables.png` & `aleksis_app_chronos-3.0b0/docs/_static/all_timetables.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/_static/class_timetable.png` & `aleksis_app_chronos-3.0b0/docs/_static/class_timetable.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/_static/daily_lessons.png` & `aleksis_app_chronos-3.0b0/docs/_static/daily_lessons.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/_static/my_timetable.png` & `aleksis_app_chronos-3.0b0/docs/_static/my_timetable.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/_static/print_timetable.png` & `aleksis_app_chronos-3.0b0/docs/_static/print_timetable.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/_static/substitution_edit.png` & `aleksis_app_chronos-3.0b0/docs/_static/substitution_edit.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/_static/substitutions.png` & `aleksis_app_chronos-3.0b0/docs/_static/substitutions.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/_static/substitutions_print.png` & `aleksis_app_chronos-3.0b0/docs/_static/substitutions_print.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/admin/11_notifications.rst` & `aleksis_app_chronos-3.0b0/docs/admin/11_notifications.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/admin/40_preferences.rst` & `aleksis_app_chronos-3.0b0/docs/admin/40_preferences.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/conf.py` & `aleksis_app_chronos-3.0b0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = "AlekSIS-App-Chronos"
 copyright = "2018-2022 The AlekSIS team"
 author = "The AlekSIS Team"
 
 # The short X.Y version
 version = "3.0"
 # The full version, including alpha/beta/rc tags
-release = "3.0.dev1"
+release = "3.0b0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `aleksis_app_chronos-3.0.dev1/docs/index.rst` & `aleksis_app_chronos-3.0b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/make.bat` & `aleksis_app_chronos-3.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/user/01_using_timetables.rst` & `aleksis_app_chronos-3.0b0/docs/user/01_using_timetables.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/user/10_substitution_plan.rst` & `aleksis_app_chronos-3.0b0/docs/user/10_substitution_plan.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/user/11_notifications.rst` & `aleksis_app_chronos-3.0b0/docs/user/11_notifications.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/docs/user/15_manage_substitutions.rst` & `aleksis_app_chronos-3.0b0/docs/user/15_manage_substitutions.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-3.0.dev1/pyproject.toml` & `aleksis_app_chronos-3.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Chronos"
-version = "3.0.dev1"
+version = "3.0b0"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -46,16 +46,16 @@
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
 calendarweek = "^0.5.0"
-aleksis-core = "^3.0.dev3"
-aleksis-app-resint = "^3.0.dev"
+aleksis-core = "^3.0b0"
+aleksis-app-resint = "^3.0b0"
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
 
 [tool.poetry.plugins."aleksis.app"]
 chronos = "aleksis.apps.chronos.apps:ChronosConfig"
```

### Comparing `aleksis_app_chronos-3.0.dev1/setup.py` & `aleksis_app_chronos-3.0b0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,28 +22,27 @@
                           'locale/ru/LC_MESSAGES/*',
                           'locale/tr_TR/LC_MESSAGES/*',
                           'locale/uk/LC_MESSAGES/*',
                           'static/css/chronos/*',
                           'static/js/chronos/*',
                           'templates/chronos/*',
                           'templates/chronos/partials/*',
-                          'templates/chronos/partials/subs/*',
-                          'templates/search/indexes/chronos/*']}
+                          'templates/chronos/partials/subs/*']}
 
 install_requires = \
-['aleksis-app-resint>=3.0.dev,<4.0',
- 'aleksis-core>=3.0.dev3,<4.0',
+['aleksis-app-resint>=3.0b0,<4.0',
+ 'aleksis-core>=3.0b0,<4.0',
  'calendarweek>=0.5.0,<0.6.0']
 
 entry_points = \
 {'aleksis.app': ['chronos = aleksis.apps.chronos.apps:ChronosConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-chronos',
-    'version': '3.0.dev1',
+    'version': '3.0b0',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Χρόνος (digital timetables)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Χρόνος (digital timetables)\n=====================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\n* Consider object-level rules and permissions\n* Export timetables as PDF\n* Search in rooms\n* Show absent groups in timetable\n* Show absent teachers in timetable\n* Show affected groups in timetable\n* Show affected teachers in timetable\n* Show supervisions in timetable\n* Timetables per day\n* Timetables per group\n* Timetables per person\n* Timetables per room\n* Timetables per week\n* Smart timetable\n\nLicence\n-------\n\n::\n\n  Copyright © 2018, 2019, 2020, 2021, 2022 Jonathan Weth <dev@jonathanweth.de>\n  Copyright © 2018, 2019 Frank Poetzsch-Heffter <p-h@katharineum.de>\n  Copyright © 2019, 2020, 2022 Dominik George <dominik.george@teckids.org>\n  Copyright © 2019, 2021 Hangzhi Yu <yuha@katharineum.de>\n  Copyright © 2019 Julian Leucker <leuckeju@katharineum.de>\n  Copyright © 2019 Tom Teichler <tom.teichler@teckids.org>\n  Copyright © 2021 Lloyd Meins <meinsll@katharineum.de>\n\n  Licenced under the EUPL, version 1.2 or later, by Teckids e.V. (Bonn, Germany).\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://aleksis.org/\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Dominik George',
     'author_email': 'dominik.george@teckids.org',
     'maintainer': 'Jonathan Weth',
     'maintainer_email': 'wethjo@katharineum.de',
     'url': 'https://aleksis.org/',
```

### Comparing `aleksis_app_chronos-3.0.dev1/PKG-INFO` & `aleksis_app_chronos-3.0b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-chronos
-Version: 3.0.dev1
+Version: 3.0b0
 Summary: AlekSIS (School Information System) — App Χρόνος (digital timetables)
 Home-page: https://aleksis.org/
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,timetable,plans
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Jonathan Weth
@@ -17,16 +17,16 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Typing :: Typed
-Requires-Dist: aleksis-app-resint (>=3.0.dev,<4.0)
-Requires-Dist: aleksis-core (>=3.0.dev3,<4.0)
+Requires-Dist: aleksis-app-resint (>=3.0b0,<4.0)
+Requires-Dist: aleksis-core (>=3.0b0,<4.0)
 Requires-Dist: calendarweek (>=0.5.0,<0.6.0)
 Project-URL: Documentation, https://aleksis.org/AlekSIS/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS-App-Chronos
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Χρόνος (digital timetables)
 =====================================================================
```

